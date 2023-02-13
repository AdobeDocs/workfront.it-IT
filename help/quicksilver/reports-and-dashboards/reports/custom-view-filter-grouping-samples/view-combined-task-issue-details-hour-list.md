---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Visualizza: dati combinati di attività e problemi in un elenco di ore"'
description: Questa visualizzazione ora combina le colonne Nome attività e Nome problema, nonché le ore pianificate attività e problema utilizzando il tag di confronto. Poiché una voce oraria può appartenere solo a un’attività o a un problema, entrambi gli oggetti non possono essere visualizzati contemporaneamente nella stessa colonna. Ogni riga della visualizzazione viene compilata con le informazioni di un'attività o di un problema.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: cf1137fd-c26a-4907-afe9-2373d3434631
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '657'
ht-degree: 0%

---

# Visualizza: dati combinati di attività ed emissione in un elenco di ore

Questa visualizzazione ora combina le colonne Nome attività e Nome problema, nonché le ore pianificate attività e problema utilizzando l&#39;opzione

```
sharecol
```

tag . Poiché una voce oraria può appartenere solo a un’attività o a un problema, entrambi gli oggetti non possono essere visualizzati contemporaneamente nella stessa colonna. Ogni riga della visualizzazione viene compilata con le informazioni di un&#39;attività o di un problema.

Per ulteriori informazioni sulle

```
sharecol
```

tag, vedi [Visualizza: unire informazioni da più colonne in una colonna condivisa](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md).\
![custom_view_hours_with_task_and_issue_information.png](assets/custom-view-hours-with-350x48.png)

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

## Visualizza i dettagli combinati delle attività e dei problemi in un elenco di ore

Per applicare questa visualizzazione:

1. Vai a un elenco di ore.
1. Da **Visualizza** menu a discesa, seleziona **Nuova vista**.

1. In **Anteprima a colonne** eliminare tutte le colonne tranne una.
1. Fai clic sull’intestazione della colonna rimanente, quindi fai clic su **Passa alla modalità testo**.
1. Passa il puntatore del mouse sull’area della modalità testo e fai clic su **Fare clic per modificare il testo**.
1. Rimuovi il testo che trovi nella **Modalità testo** e sostituirlo con il seguente codice:
   <pre>column.1.querysort=project:name<br>column.1.short=false<br>column.1.stretch=0<br>column.1.valuefield=project:name<br>column.1.valueformat=HTML<br>column.1.width=100<br>column.2.description=Attività o Problema<br>column.2.link.linkproperty.0.name=ID<br>column.2.link.linkproperty.0.valuefield=task:ID<br>column.2.link.linkproperty.0.valueformat=int<br>column.2.link.lookup=link.view<br>column.2.link.value.field=task:objCode<br>column.2.link.valueformat=val<br>column.2.linkedname=task<br>column.2.listsort=nidificato(task).string(name)<br>column.2.name=Task o Issue<br>column.2.querysort=task:name<br>column.2.sharecol=true<br>column.2.short=false<br>column.2.stretch=0<br>column.2.valuefield=task:name<br>column.2.valueformat=HTML<br>column.2.width=100<br>column.3.descriptionkey=optask<br>column.3.link.linkproperty.0.name=ID<br>column.3.link.linkproperty.0.valuefield=opTask:ID<br>column.3.link.linkproperty.0.valueformat=int<br>column.3.link.lookup=link.view<br>column.3.link.value.field=opTask:objCode<br>column.3.link.valueformat=val<br>column.3.linkedname=optask<br>column.3.listsort=nidificato(opTask).string(name)<br>column.3.namekey=opTask<br>column.3.querysort=opTask:name<br>column.3.short=false<br>column.3.stretch=0<br>column.3.valueField=opTask:name<br>column.3.valueformat=HTML<br>column.3.width=1<br>column.4.valuefield=task:work<br>column.4.sharecol=true<br>column.4.linkedname=task<br>column.4.valueformat=doubleAsInt<br>column.4.namekey=view.relatedcolumn<br>column.4.querysort=task:work<br>column.4.textmode=true<br>column.4.namekeyargkey.0=task<br>column.4.namekeyargkey.1=work<br>column.4.displayname=Sforzo pianificato<br>column.5.displayname=Sforzo pianificato<br>column.5.viewalias=opTask:workrequired<br>column.5.linkedname=opTask<br>column.5.valueField=opTask:workRequired<br>column.5.valueformat=composto<br>column.5.querysort=opTask:workRequired<br>column.5.namekeyargkey.0=opTask<br>column.5.namekeyargkey.1=workrequired<br>column.5.namekey=view.relatedcolumn<br>column.5.textmode=true<br>column.6.descriptionkey=hours<br>column.6.linkedname=direct<br>column.6.listsort=doubleAsDouble(hours)<br>column.6.namekey=hours.abbr<br>column.6.querysort=hours<br>column.6.short=false<br>column.6.stretch=0<br>column.6.valuefield=hours<br>column.6.valueformat=doubleAsString<br>column.6.width=75<br>column.7.descriptionkey=entrydate<br>column.7.linkedname=direct<br>column.7.listsort=atDateAsAtDate(entryDate)<br>column.7.namekey=entrydate.abbr<br>column.7.querysort=entryDate<br>column.7.short=false<br>column.7.stretch=0<br>column.7.valueField=entryDate<br>column.7.valueformat=atDate<br>column.7.width=75<br>column.8.descriptionkey=description<br>column.8.linkedname=direct<br>column.8.listsort=string(description)<br>column.8.namekey=description.abbr<br>column.8.querysort=description<br>column.8.short=false<br>column.8.stretch=0<br>column.8.valuefield=description<br>column.8.valueformat=HTML<br>column.8.width=150</pre>

1. Fai clic su **Salva visualizzazione**.
