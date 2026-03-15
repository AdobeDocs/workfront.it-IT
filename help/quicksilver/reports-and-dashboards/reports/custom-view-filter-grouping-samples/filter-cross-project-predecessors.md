---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filtro: visualizzare predecessori tra progetti incompleti'
description: Questo filtro attività restituisce predecessori tra progetti incompleti.
author: Lisa and Courtney
feature: Reports and Dashboards
exl-id: 7ee2432c-1d82-454e-a73a-f1f6b6a5c10d
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '199'
ht-degree: 25%

---

# Filtro: visualizzare predecessori tra progetti incompleti

<!--Audited: 10/2024-->

Questo filtro attività restituisce predecessori tra progetti incompleti.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td> 
   <p>Collaboratore o richiesta di modifica di un filtro </p>
   <p>Standard o piano per modificare un report</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso a report, dashboard, calendari</p> <p>Modificare l'accesso a Filtri, Viste, Raggruppamenti per modificare un filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
   <td> <p>Gestire le autorizzazioni per un report</p>  </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Filtrare i predecessori tra progetti

Per applicare questo filtro:

1. Consente di passare a un elenco di attività o a una relazione sulle attività.
1. Dal menu a discesa **Filtro**, seleziona **Nuovo filtro**.

1. (Condizionale) Fare clic su **Modalità testo** se è stato eseguito l&#39;accesso al filtro da un elenco o **Passare alla modalità testo** se è stato eseguito l&#39;accesso al filtro da un report.
1. Nella nuova area, incollate il seguente codice:
   <pre>predecessorsMM:projectID=FIELD:projectID<br>predecessorsMM:projectID_Mod=ne<br>percentComplete=100<br>percentComplete_Mod=ne</pre>

1. (Condizionale) Fare clic su **Salva filtro** se è stato eseguito l&#39;accesso al filtro da un report oppure su **Applica**, quindi su **Salva come nuovo** se è stato eseguito l&#39;accesso al filtro da un elenco di attività.
