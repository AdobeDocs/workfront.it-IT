---
product-area: reporting
navigation-topic: reporting-elements
title: Utilizzare caratteri jolly basati sull’utente per generalizzare i rapporti
description: You can generalize a report by using wildcards instead of specific information when building certain reporting elements.
author: Courtney
feature: Reports and Dashboards
exl-id: 216e2869-b4f8-4cc7-9497-a12ebe00fe49
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 15%

---

# Utilizzare caratteri jolly basati sull’utente per generalizzare i rapporti

<!-- Audited: 11/2024 -->

You can generalize a report by using wildcards instead of specific information when building certain reporting elements. For example, if you want to create a report that shows the tasks assigned to a specific user, you can use the user&#39;s name in the Assigned To field of the filter. Tuttavia, se si desidera creare un report che mostra le attività assegnate all&#39;utente connesso, indipendentemente dall&#39;utente, è possibile utilizzare un carattere jolly che indichi che quando un utente visualizza il report, vengono visualizzate solo le informazioni che lo riguardano. This way, you build the report once but because you use a wildcard in the filter it produces different results every time someone else reads it.

You can use user-based wildcards when building the following reporting elements:

* Filtri
* Custom prompts
* Views when adding rules for columns

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
   <td role="rowheader">Licenza di Adobe Workfront</strong></td> 
   <td> 
    <p>Standard</p>
    <p>Piano</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica accesso a Filtri, Viste, Raggruppamenti</p> <p>Edit access to Reports, Dashboards, Calendars to edit reporting elements in a report</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
    <td> <p>Manage permissions to a report to edit reporting elements in a report</p> <p>Manage permissions to a view or filter to edit them</p></td> 
   </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

You must create a report before you can add a wildcard variable to it.

Per istruzioni sulla creazione di report, vedere [Creare un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## How-to steps

To insert a user-based wildcard in a report:

1. Go to a report for which you want to insert a user-based wildcard.
1. Fai clic su **Azioni report**, quindi su **Modifica**.

1. Click the **Filters** tab.
1. Fai clic su **Aggiungi una regola filtro**.
1. Start typing the name of the field that you want to filter by.\
   You must type fields that reference the user object or information about users.
1. Select **Equal** in the drop-down menu for the filter variable.

   >[!TIP]
   >
   >È sempre necessario selezionare la variabile di filtro **Equal** quando si utilizzano i caratteri jolly in Adobe Workfront.

1. Nella casella **Inizia a digitare il nome ...** digitare: `$$USER.ID` o `$$USER.name` se si desidera che nel report vengano visualizzate le informazioni relative all&#39;utente che effettua l&#39;accesso, in base al nome. È possibile inserire altri caratteri jolly che fanno riferimento al gruppo, al team, alla società o ad altre informazioni dell&#39;utente connesso.

   For a complete list of user-based wildcards, see [Wildcard filter variables overview](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

1. Fai clic su **Salva e Chiudi**.

## Informazioni aggiuntive

Vedi anche:

<!--outdated: * [Basic Report Creation Program](https://one.workfront.com/s/basic-report-creation-program) -->
* [Wildcard filter variables overview](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)
* [Creare o modificare filtri in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
* [Panoramica sui filtri](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Add a prompt to a report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)
* [Utilizzare la formattazione condizionale nelle viste](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)
