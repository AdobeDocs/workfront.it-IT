---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Visualizza: Ore effettive rispetto alle ore pianificate nella stessa colonna di un''attività Visualizza'''
description: In questa visualizzazione attività, la quantità effettiva di ore registrate in un'attività viene visualizzata nel corso delle ore pianificate per ogni attività.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c1179283-dc2e-40d3-b8e0-4b1b79f83ad3
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 1%

---

# Visualizza: Ore effettive rispetto alle ore pianificate nella stessa colonna di un&#39;attività Visualizza

In questa visualizzazione dell&#39;attività, la quantità effettiva di ore registrate in un&#39;attività viene visualizzata nelle ore pianificate per ogni attività.

![actual_vs_scheduled_in_task_report.png](assets/actual-vs-planned-in-task-report-350x58.png)

## Requisiti di accesso

Per eseguire la procedura descritta in questo articolo, è necessario disporre delle accesso seguenti:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Systems Piano Workfront*</td> 
   <td> <p>Qualunque</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Systems Workfront*</td> 
   <td> <p>Richiesta di modifica di una visualizzazione </p>
   <p>piano per modificare un report</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modifica accesso a Report, Dashboard, Calendari per modificare un report</p> <p>Modificare l'accesso a Filtri, Viste, Raggruppamenti per modificare una vista</p> <p><b>NOTA</b>

Se ancora non hai accesso, chiedi all&#39;amministratore di Workfront se ha impostato ulteriori restrizioni nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crea o modificare i livelli</a> di accesso personalizzati.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un report</p> <p>Per informazioni sulla richiesta di accesso aggiuntivi, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiesta di accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni su quale piano, tipo di licenza o accesso disponi, contatta l&#39;amministratore di Workfront.

## Visualizza Ore effettive rispetto alle ore pianificate in una vista attività

Per applicare questa visualizzazione:

1. Vai a un elenco di attività.
1. Dal menu a discesa **Visualizza**, selezionare **Nuova visualizzazione**.

1. Nell&#39;area **Anteprima colonna** eliminare tutte le colonne tranne una.
1. Fai clic sull&#39;intestazione della colonna rimanente, quindi fai clic su **Passa a modalità** testo.
1. Passate il puntatore del mouse sull&#39;area della modalità testo e fate clic su **Click per modificare il testo**.
1. Rimuovi il testo individuato nella **casella Modalità** testo e sostituirlo con il codice riportato di seguito:
   <pre>column.0.descriptionkey=name<br>column.0.collegare.linkproperty.0.name=ID<br>column.0.collegare.linkproperty.0.valuefield=ID<br>column.0.collegare.linkproperty.0.valueformat=int<br>column.0.collegare.lookup=collegare.view<br>column.0.collegare.valuefield=objCode<br>column.0.collegare.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.viewalias=assignments<br>column.1.displayname=<br>column.1.linkedname=direct<br>column.1.namekey=assignments<br>column.1.valuefield=assignmentsListString<br>column.1.valueformat=HTML<br>column.1.tile.name=component.assignmentslist<br>column.2.displayname=Ore<br>effettive/pianificate column.2.linkedname=direct<br>column.2.namekey=actualWorkRequired<br>column.2.querysort=actualWork<br>column.2.textmode=true<br>column.2.valueexpression=CONCAT({actualWorkRequired}/60,' / ',{workRequired}/60)<br>column.2.valuefield=actualWorkRequired<br>column.2.valueformat=compound<br>column.2.viewalias=actualworkrequired<br>column.3.aggregator.function=SUM<br>column.3.aggregator.valueexpression=SUB({actualWork}, {workRequired})<br>column.3.aggregator.valueformat=compound<br>column.3.displayname=Hours Variance<br>column.3.linkedname=direct<br>column.3.textmode=true<br>column.3.valueexpression=SUB({actualWork}, {workRequired})/60<br>column.3.valueformat=customNumberAsString</pre>

1. Fai clic su **Salva vista**.
