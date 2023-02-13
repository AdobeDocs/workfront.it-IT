---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Visualizza: Ore effettive su ore pianificate nella stessa colonna di una visualizzazione attività'
description: In questa visualizzazione attività viene visualizzata la quantità effettiva di ore registrate in un'attività nelle ore pianificate per ogni attività.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c1179283-dc2e-40d3-b8e0-4b1b79f83ad3
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 0%

---

# Visualizza: Ore effettive in ore pianificate nella stessa colonna di una visualizzazione attività

In questa visualizzazione attività viene visualizzata la quantità effettiva di ore registrate in un&#39;attività nelle ore pianificate per ogni attività.

![effettivo_vs_pianificato_in_task_report.png](assets/actual-vs-planned-in-task-report-350x58.png)

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Accesso a rapporti, dashboard, calendari</p> <p>Modificare l’accesso a Filtri, Visualizzazioni, Gruppi</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Visualizza ore effettive in ore pianificate in una visualizzazione attività

Per applicare questa visualizzazione:

1. Passare a un elenco di attività.
1. Da **Visualizza** menu a discesa, seleziona **Nuova vista**.

1. In **Anteprima a colonne** eliminare tutte le colonne tranne una.
1. Fai clic sull’intestazione della colonna rimanente, quindi fai clic su **Passa alla modalità testo**.
1. Passa il puntatore del mouse sull’area della modalità testo e fai clic su **Fare clic per modificare il testo**.
1. Rimuovi il testo che trovi nella **Modalità testo** e sostituirlo con il seguente codice:
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.value.field=objCode<br>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.short=false<br>column.0.stretch=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.viewalias=assegnazioni<br>column.1.displayname=<br>column.1.linkedname=direct<br>column.1.namekey=assegnazioni<br>column.1.valuefield=assignedListString<br>column.1.valueformat=HTML<br>column.1.tile.name=component.assignmentslist<br>column.2.displayname=Ore effettive/ pianificate<br>column.2.linkedname=direct<br>column.2.namekey=real-workrequired<br>column.2.querysort=realWork<br>column.2.textmode=true<br>column.2.valueexpression=CONCAT({currentWorkRequired}/60,' / ',{workRequired}/60)<br>column.2.valuefield=effectiveWorkRequired<br>column.2.valueformat=composto<br>column.2.viewalias=implementationworkrequired<br>column.3.aggregator.function=SUM<br>column.3.aggregator.valueexpression=SUB({effectiveWork}, {workRequired})<br>column.3.aggregator.valueformat=composto<br>column.3.displayname=Varianza ore<br>column.3.linkedname=direct<br>column.3.textmode=true<br>column.3.value.expression=SUB({currentWork}, {workRequired})/60<br>column.3.value.format=customNumberAsString</pre>

1. Fai clic su **Salva visualizzazione**.
