---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: Tracciamento dei record orari con l’API di Adobe Workfront
description: Se l’organizzazione utilizza Adobe Workfront per immettere le ore lavorate, ma utilizza un altro strumento come sistema di record per tali dati, puoi utilizzare l’API Workfront per sincronizzare i dati tra i due sistemi.
author: Alina
feature: Timesheets
exl-id: b26f8156-f9dc-43e7-8e0d-8c0905dc7a12
source-git-commit: 7786d899841cb82cc4d3832fb083c6e2bda2e197
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 0%

---

# Tracciamento dei record orari con l’API di Adobe Workfront

Se l’organizzazione utilizza Adobe Workfront per immettere le ore lavorate, ma utilizza un altro strumento come sistema di record per tali dati, puoi utilizzare l’API Workfront per sincronizzare i dati tra i due sistemi.

Il semplice tracciamento del record dell’ora non è fattibile perché, se la voce dell’ora viene rimossa, l’intero record viene eliminato, richiedendo di richiamare l’intero set di dati e di confrontarlo con il vecchio set di dati. Fortunatamente, tutte le transazioni orarie vengono registrate in Workfront Journal Entries.

Dopo aver recuperato un set iniziale di tutte le ore correnti nel sistema, è possibile tenere traccia di tutte le modifiche attraverso le scritture contabili.
<pre>GET /attask/api/v5.0/JRNLE/search?subObjCode=HOUR&amp;fields=changeType,aux2,newNumberVal,oldNumberVal,subObjCode,subObjID</pre><pre>{<br>"data": [<br>{<br>"ID": "5785406d008d93dd35665f14d90d4929",<br>"objCode": "JRNLE",<br>"changeType": "A",<br>"aux2": "Brad Littler",<br>"newNumberVal": 1<br>"oldNumberVal": nullo,<br>"subObjCode": "ORA",<br>"subObjID": "5785406d008d93dce3f7f2e0e8eda4ea"<br>},<br>{<br>"ID": "57854124008da2b9f372c01f8b9054bf",<br>"objCode": "JRNLE",<br>"changeType": "D",<br>"aux2": "Brad Littler",<br>"newNumberVal": nullo,<br>"oldNumberVal": 1<br>"subObjCode": "ORA",<br>"subObjID": "5785406d008d93dce3f7f2e0e8eda4ea"<br>},<br>{<br>"ID": "5785416f008db05ecee934663a968366",<br>"objCode": "JRNLE",<br>"changeType": "A",<br>"aux2": "Brad Littler",<br>"newNumberVal": 1<br>"oldNumberVal": nullo,<br>"subObjCode": "ORA",<br>"subObjID": "5785416f008db05d9d2925c12b10f521"<br>},<br>{<br>"ID": "57854176008db22fe974b7c67feea6b2",<br>"objCode": "JRNLE",<br>"changeType": "E",<br>"aux2": "Brad Littler",<br>"newNumberVal": 2.<br>"oldNumberVal": 1<br>"subObjCode": "ORA",<br>"subObjID": "5785416f008db05d9d2925c12b10f521"<br>}<br>]<br>}</pre>Segue una descrizione dei campi inclusi:

* **changeType:** Tipo di modifica apportata all&#39;oggetto:

   * **R:** Aggiungi

   * **E:** Modifica

   * **D:** Elimina

* **aux2:** Il nome dell&#39;utente per il quale si trova il record dell&#39;ora.

* **newNumberVal:** Nuovo valore del record dell&#39;ora (questo sarà null se changeType è D).

* **oldNumberVal:** Valore precedente del record dell&#39;ora.

* **subObjCode:** Tipo di record da modificare (deve sempre essere ORA).

* **subObjID:** ID del record Ora.

È possibile utilizzare queste informazioni per scoprire quali record orari sono stati modificati, modificati o eliminati. Puoi quindi utilizzare il subObjID per recuperare ulteriori informazioni dai record delle ore, se necessario.
