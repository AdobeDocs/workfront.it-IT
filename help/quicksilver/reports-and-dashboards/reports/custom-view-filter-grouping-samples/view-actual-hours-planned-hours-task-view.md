---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Vista: ore effettive rispetto alle ore pianificate nella stessa colonna di una vista attività'
description: In questa visualizzazione attività, la quantità effettiva di ore registrate in un'attività viene visualizzata sulle ore pianificate per ogni attività. Anche lo scostamento ore tra le ore pianificate e quelle effettive viene visualizzato in una colonna separata.
author: Courtney
feature: Reports and Dashboards
exl-id: c1179283-dc2e-40d3-b8e0-4b1b79f83ad3
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 25%

---

# Vista: ore effettive rispetto alle ore pianificate nella stessa colonna di una vista attività

In questa visualizzazione attività, la quantità effettiva di ore registrate in un&#39;attività viene visualizzata sulle ore pianificate per ogni attività. Anche lo scostamento ore tra le ore pianificate e quelle effettive viene visualizzato in una colonna separata.

![actual_vs_scheduled_in_task_report.png](assets/actual-vs-planned-in-task-report-350x58.png)

## Requisiti di accesso

<!--Audited: 10/2024-->

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

## Visualizza ore effettive su ore pianificate in una visualizzazione attività

Per applicare questa visualizzazione:

1. Consente di passare a un elenco di attività.
1. Dal menu a discesa **Visualizza**, seleziona **Nuova vista**.
1. Nell&#39;area **Anteprima colonna**, eliminare tutte le colonne tranne una.
1. Fare clic sull&#39;intestazione della colonna rimanente, quindi fare clic su **Passa alla modalità testo**.
1. Passa il mouse sull&#39;area della modalità testo e fai clic su **Modifica modalità testo**.
1. Rimuovete il testo trovato nella casella della modalità testo e sostituitelo con il codice seguente:

   ```
   column.0.descriptionkey=name
   column.0.link.linkproperty.0.name=ID
   column.0.link.linkproperty.0.valuefield=ID
   column.0.link.linkproperty.0.valueformat=int
   column.0.link.lookup=link.view
   column.0.link.valuefield=objCode
   column.0.link.valueformat=val
   column.0.linkedname=direct
   column.0.listsort=string(name)
   column.0.namekey=name.abbr
   column.0.querysort=name
   column.0.shortview=false
   column.0.stretch=100
   column.0.valuefield=name
   column.0.valueformat=HTML
   column.0.width=150
   column.1.viewalias=assignments
   column.1.displayname=
   column.1.linkedname=direct
   column.1.namekey=assignments
   column.1.valuefield=assignmentsListString
   column.1.valueformat=HTML
   column.1.tile.name=component.assignmentslist
   column.2.displayname=Actual/ Planned Hours
   column.2.linkedname=direct
   column.2.namekey=actualworkrequired
   column.2.querysort=actualWork
   column.2.textmode=true
   column.2.valueexpression=CONCAT({actualWorkRequired}/60,' / ',{workRequired}/60)
   column.2.valuefield=actualWorkRequired
   column.2.valueformat=compound
   column.2.viewalias=actualworkrequired
   column.3.aggregator.function=SUM
   column.3.aggregator.valueexpression=SUB({actualWork}, {workRequired})
   column.3.aggregator.valueformat=compound
   column.3.displayname=Hours Variance
   column.3.linkedname=direct
   column.3.textmode=true
   column.3.valueexpression=SUB({actualWork}, {workRequired})/60
   column.3.valueformat=customNumberAsString
   ```

1. Fai clic su **Fine**, quindi su **Salva vista**.
