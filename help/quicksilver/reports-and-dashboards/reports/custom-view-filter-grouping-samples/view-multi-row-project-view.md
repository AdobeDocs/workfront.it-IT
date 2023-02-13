---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Visualizza: visualizzazione progetto su più righe"'
description: In questa visualizzazione del progetto è possibile - MODIFICARE ME.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 3c6028c0-2c9f-4f86-aa6c-bf089844bac8
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '589'
ht-degree: 0%

---

# Visualizza: visualizzazione progetto a più righe

In questa visualizzazione del progetto puoi:

* Visualizza le informazioni del progetto in un formato a più righe.\
   La visualizzazione utilizza il

   ```
   sharecol=true
   ```

   per combinare più campi sotto la stessa intestazione di colonna. Per ulteriori informazioni su questo tag, consulta [Visualizza: unire informazioni da più colonne in una colonna condivisa](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md).

* Utilizzare una colonna segnaposto contenente un tag di interruzione di riga di HTML (

   ```
   <br>
   ```

   ) per forzare la visualizzazione della descrizione sotto il nome del progetto, ad esempio.
* Visualizza il proprietario del progetto tra parentesi dopo il nome del progetto.
* Visualizza il Nome progetto come collegamento al progetto.

![](assets/project-multi-row-stacked-view-350x219.png)

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

## Creare una visualizzazione di progetto con più righe

1. Crea una nuova visualizzazione del progetto. Per ulteriori informazioni su come creare una nuova visualizzazione, consulta [Panoramica delle visualizzazioni in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).
1. Durante la creazione della visualizzazione, eliminare tutte le colonne tranne una.
1. Seleziona la colonna rimanente e fai clic su **Passa alla modalità testo**.
1. Copia e incolla la modalità testo all’interno della colonna:
   <pre>column.0.linkedname=direct<br>column.0.link.valueformat=val<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.value.field=objCode<br>column.0.link.lookup=link.view<br>column.0.sharecol=true<br>column.0.descriptionkey=name<br>column.0.width=150<br>column.0.querysort=name<br>column.0.valuefield=name<br>column.0.name=Nome progetto / Manager / Descrizione<br>column.0.short=false<br>column.0.stretch=100<br>column.0.textmode=true<br>column.0.listsort=string(name)<br>column.0.valueformat=HTML<br>column.1.value.expression=CONCAT(" (",{owner}).{name},")")<br>column.1.listsort=nidificato(owner).string(name)<br>column.1.width=1<br>column.1.linkedname=direct<br>column.1.querysort=owner:name<br>column.1.textmode=true<br>column.1.short=false<br>column.1.stretch=0<br>column.1.valueformat=HTML<br>column.1.sharecol=true<br>column.2.width=1<br>column.2.value=<br><br>column.2.short=false<br>column.2.sharecol=true<br>column.2.stretch=0<br>column.2.textmode=true<br>column.2.valueformat=HTML<br>column.3.styledef.style=font-color:#ccc;<br>column.3.descriptionkey=description<br>column.3.linkedname=direct<br>column.3.valuefield=description<br>column.3.listsort=string(description)<br>column.3.querysort=description<br>column.3.namekey=description.abbr<br>column.3.textmode=true<br>column.3.sharecol=true<br>column.3.stretch=0<br>column.3.short=false<br>column.3.valueformat=HTML<br>column.3.width=1<br>column.4.short=false<br>column.4.value=<br><br>column.4.sharecol=true<br>column.4.width=1<br>column.4.textmode=true<br>column.4.valueformat=HTML\<br>column.4.stretch=0<br>column.5.name=Date previste / Durata<br>column.5.width=150<br>column.5.querysort=scheduledStartDate<br>column.5.sharecol=true<br>column.5.stretch=0<br>column.5.textmode=true<br>column.5.short=false<br>column.5.linkedname=direct<br>column.5.listsort=atDateAsAtDate(scheduledStartDate)<br>column.5.valuefield=scheduledStartDate<br>column.5.valueformat=atDate<br>column.6.sharecol=true<br>column.6.stretch=0<br>column.6.width=1<br>column.6.textmode=true<br>column.6.value=-<br>column.6.valueformat=HTML<br>column.6.short=false<br>column.7.namekey=plannedcompletiondate.abbr<br>column.7.width=1<br>column.7.sharecol=true<br>column.7.short=false<br>column.7.stretch=0<br>column.7.listsort=atDateAsAtDate(scheduledCompletionDate)<br>column.7.linkedname=direct<br>column.7.descriptionkey=plannedcompletiondate<br>column.7.textmode=true<br>column.7.querysort=scheduledCompletionDate<br>column.7.valueformat=atDate<br>column.7.valueField=scheduledCompletionDate<br>column.8.value=<br><br>column.8.width=1<br>column.8.textmode=true<br>column.8.sharecol=true<br>column.8.valueformat=HTML<br>column.8.stretch=0<br>column.9.textmode=true<br>column.9.listsort=intAsInt(durationMinutes)<br>column.9.stretch=0<br>column.9.valueField=durationFieldLong<br>column.9.descriptionkey=duration<br>column.9.viewalias=duration<br>column.9.querysort=durationMinutes<br>column.9.sharecol=true<br>column.9.width=100<br>column.9.short=false<br>column.9.namekey=duration.abbr<br>column.9.linkedname=direct<br>column.9.valueformat=composto<br>column.10.textmode=true<br>column.10.stretch=0</pre>

1. Fai clic su **Salva visualizzazione**.
