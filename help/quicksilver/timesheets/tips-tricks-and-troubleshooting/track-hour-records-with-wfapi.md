---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: Tracciare i record di ore con l’API di Adobe Workfront
description: Se la tua organizzazione utilizza Adobe Workfront per immettere le ore lavorate, ma utilizza un altro strumento come sistema di registrazione per tali dati, puoi utilizzare l’API Workfront per sincronizzare i dati tra i due sistemi.
author: Lisa
feature: Timesheets
exl-id: b26f8156-f9dc-43e7-8e0d-8c0905dc7a12
source-git-commit: 69cd5fb1d089b81b7a1673609b92537137b6b68e
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 0%

---

# Tracciare i record di ore con l’API di Adobe Workfront

Se la tua organizzazione utilizza Adobe Workfront per immettere le ore lavorate, ma utilizza un altro strumento come sistema di registrazione per tali dati, puoi utilizzare l’API Workfront per sincronizzare i dati tra i due sistemi.

Non è possibile tenere traccia semplicemente del record delle ore perché, se l’immissione delle ore viene rimossa, l’intero record viene eliminato e richiede di estrarre l’intero set di dati e confrontarlo con il set di dati precedente. Fortunatamente, tutte le transazioni orarie vengono registrate in Workfront Journal Entries.

Dopo aver recuperato una serie iniziale di tutte le ore correnti nel sistema, è possibile tenere traccia di tutte le modifiche tramite le voci del diario.
<pre>GET /attask/api/v5.0/JRNLE/search?subObjCode=HOUR&amp;fields=changeType,aux2,newNumberVal,oldNumberVal,subObjCode,subObjID</pre><pre>{<br>"data": [<br>{<br>"ID": "5785406d008d93dd35665f14d90d4929",<br>"objCode": "JRNLE",<br>"changeType": "A",<br>"aux2": "Brad Littler",<br>"newNumberVal": 1,<br>"oldNumberVal": null,<br>"subObjCode": "HOUR",<br>"subObjID": "5785406d008d93dce3f7f2e0e8eda4ea"<br>},<br>{<br>"ID": "57854124008da2b9f372c01f8b9054bf",<br>"objCode": "JRNLE",<br>"changeType": "D",<br>"aux2": "Brad Littler",<br>"newNumberVal": null,<br>"oldNumberVal": 1,<br>"subObjCode": "HOUR",<br>"subObjID": "5785406d008d93dce3f7f2e0e8eda4ea"<br>},<br>{<br>"ID": "5785416f008db05ecee934663a968366",<br>"objCode": "JRNLE",<br>"changeType": "A",<br>"aux2": "Brad Littler",<br>"newNumberVal": 1,<br>"oldNumberVal": null,<br>"subObjCode": "HOUR",<br>"subObjID": "5785416f008db05d9d2925c12b10f521"<br>},<br>{<br>"ID": "57854176008db22fe974b7c67feea6b2",<br>"objCode": "JRNLE",<br>"changeType": "E",<br>"aux2": "Brad Littler"<br>" "HOUR",<br>"subObjID": "5785416f008db05d9d2925c12b10f521"<br>}<br>]<br>}<br><br></pre>Di seguito è riportata una descrizione dei campi inclusi:

* **changeType:** Il tipo di modifica da apportare all&#39;oggetto:

   * **A:** Aggiungi

   * **E:** Modifica

   * **D:** Elimina

* **aux2:** nome dell&#39;utente a cui si riferisce il record di ore.

* **newNumberVal:** Nuovo valore del record delle ore (questo valore sarà nullo se changeType è D).

* **oldNumberVal:** Valore precedente del record ore.

* **subObjCode:** Tipo di record in fase di modifica (dovrebbe sempre essere ORA).

* **subObjID:** ID del record delle ore.

È possibile utilizzare queste informazioni per individuare i record delle ore modificati, modificati o eliminati. Puoi quindi utilizzare subObjID per recuperare ulteriori informazioni dai record delle ore, se necessario.
