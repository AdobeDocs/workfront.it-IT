---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Visualizza: problemi con la ragione sociale del cedente'
description: Questa visualizzazione del problema visualizza il nome dell'azienda associato all'utente che ha inviato il problema.
author: Courtney
feature: Reports and Dashboards
exl-id: e628f7cf-4a7b-4125-bea6-348c72477bd7
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '211'
ht-degree: 23%

---

# Visualizzazione: problemi relativi al nome azienda del referente

<!--Audit: 11/2024-->

Questa visualizzazione del problema visualizza il nome dell&#39;azienda associato all&#39;utente che ha inviato il problema.

![custom_view_for_issues_with_originator_company_name.png](assets/custom-view-for-issues-350x33.png)

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
   <p>Collaboratore o richiesta di modifica di una visualizzazione </p>
   <p>Standard o piano per modificare un report</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso a report, dashboard, calendari</p> <p>Modificare l'accesso a Filtri, Viste, Raggruppamenti per modificare una vista</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
   <td> <p>Gestire le autorizzazioni per un report</p>  </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


+++

## Visualizza problemi con la ragione sociale del creatore

1. Vai a un elenco di problemi.
1. Dal menu a discesa **Visualizza**, seleziona **Nuova vista**.
1. Nell&#39;area **Anteprima colonna**, eliminare tutte le colonne tranne una.
1. Fare clic sull&#39;intestazione della colonna rimanente, quindi fare clic su **Passa alla modalità testo** e infine su **Modifica modalità testo**.
1. Rimuovere il testo trovato nella casella **Modifica modalità testo** e sostituirlo con il codice seguente:


   ```
   column.0.descriptionkey=name
   column.0.link.linkproperty.0.name=ID
   column.0.link.linkproperty.0.valuefield=ID
   column.0.link.linkproperty.0.valueformat=val
   column.0.link.lookup=link.view
   column.0.link.value=val(objCode)
   column.0.listsort=string(name)
   column.0.namekey=name
   column.0.querysort=name
   column.0.valuefield=name
   column.0.valueformat=HTML
   column.0.width=140
   column.1.descriptionkey=originator
   column.1.link.linkproperty.0.name=ID
   column.1.link.linkproperty.0.valuefield=ownerID
   column.1.link.linkproperty.0.valueformat=int
   column.1.link.lookup=link.view
   column.1.link.valuefield=owner:objCode
   column.1.link.valueformat=val
   column.1.listsort=nested(owner).string(name)
   column.1.namekey=originator.abbr
   column.1.querysort=owner:name
   column.1.valuefield=owner:name
   column.1.valueformat=HTML
   column.1.width=151
   column.2.descriptionkey=entrydate
   column.2.listsort=atDateAsAtDate(entryDate)
   column.2.namekey=entrydate.abbr
   column.2.querysort=entryDate
   column.2.valuefield=entryDate
   column.2.valueformat=atDate
   column.2.width=75
   column.3.descriptionkey=age
   column.3.listsort=doubleAsDouble(age)
   column.3.namekey=age
   column.3.querysort=age
   column.3.valuefield=howOld
   column.3.valueformat=val
   column.3.width=80
   column.4.viewalias=statusicons
   column.4.displayname=Flags
   column.4.linkedname=direct
   column.4.namekey=statusicons
   column.4.valuefield=
   column.4.valueformat=HTML
   column.4.querysort=
   column.4.tile.name=component.issuestatusicons
   column.4.tile.pdfcomponent=issueStatusIcons
   column.4.delimiter=
   column.4.tile.template=/WEB-INF/jsp/lists/components/issueStatusIcons.jsp
   column.5.description=Originator's Company Name
   column.5.link.linkproperty.0.name=ID
   column.5.link.linkproperty.0.valuefield=owner:companyID
   column.5.link.linkproperty.0.valueformat=int
   column.5.link.lookup=link.view
   column.5.link.valuefield=owner:company:objCode
   column.5.link.valueformat=val
   column.5.listsort=nested(owner:company).string(name)
   column.5.name=Originator Company
   column.5.querysort=owner:company:name
   column.5.valuefield=owner:company:name
   column.5.valueformat=HTML
   column.5.width=151
   ```

1. Fai clic su **Fine** > **Salva vista**.
1. (Facoltativo) Aggiornare il nome della visualizzazione, quindi fare clic su **Salva visualizzazione**.
