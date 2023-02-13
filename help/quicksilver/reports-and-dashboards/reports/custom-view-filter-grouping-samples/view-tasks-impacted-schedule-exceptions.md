---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Visualizza: attività interessate dalle eccezioni della pianificazione'
description: Questa visualizzazione attività identifica le attività che dovranno essere completate in ritardo a causa dei fine settimana, dell'orario di inattività personale o di altre eccezioni di pianificazione.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7d7c77fa-d9a7-4e91-8dae-ad3aaca6f1da
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 0%

---

# Visualizza: attività interessate dalle eccezioni della pianificazione

Questa visualizzazione attività identifica le attività che dovranno essere completate in ritardo a causa dei fine settimana, dell&#39;orario di inattività personale o di altre eccezioni di pianificazione.

Questa visualizzazione mostra quanto segue:

* Durata dei compiti
* Le date di inizio e di completamento pianificate delle attività
* Durata delle attività in base al numero di giorni tra le date di inizio previste e di completamento pianificato delle attività (Durata calendario)
* Numero del giorno nella pianificazione del progetto all&#39;avvio dell&#39;attività (Data inizio calendario)
* Durata del giorno della settimana delle attività in base al numero di giorni della settimana tra le date di inizio previste e di completamento pianificato delle attività (Durata del giorno della settimana)
* Se la Durata del giorno della settimana è maggiore della durata delle attività, il che suggerisce che ci sono giorni di eccezione nella durata delle attività, le attività sono contrassegnate come &quot;Eccezione&quot;.\
   ![Tasks_with_calendar_exception.png](assets/tasks-with-calendar-exceptions-350x51.png)

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

## Visualizza le attività interessate dalle eccezioni della pianificazione

1. Passare a un elenco di attività.
1. Da **Visualizza** menu a discesa, seleziona **Nuova vista**.

1. In **Anteprima a colonne** eliminare tutte le colonne tranne una.
1. Fai clic sull’intestazione della colonna rimanente, quindi fai clic su **Passa alla modalità testo**.
1. Passa il puntatore del mouse sull’area della modalità testo e fai clic su **Fare clic per modificare il testo**.
1. Rimuovi il testo che trovi nella **Modalità testo** e sostituirlo con il seguente codice:
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.value.field=objCode<br>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.short=false<br>column.0.stretch=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.descriptionkey=duration<br>column.1.linkedname=direct<br>column.1.listsort=intAsInt(durationMinutes)<br>column.1.namekey=duration.abbr<br>column.1.querysort=durationMinutes<br>column.1.short=false<br>column.1.stretch=0<br>column.1.valuefield=durationFieldLong<br>column.1.valueformat=composto<br>column.1.viewalias=duration<br>column.1.width=80<br>column.2.descriptionkey=plannedstartdate<br>column.2.linkedname=direct<br>column.2.listsort=atDateAsAtDate(scheduledStartDate)<br>column.2.namekey=plannedstartdate.abbr<br>column.2.querysort=scheduledStartDate<br>column.2.short=false<br>column.2.stretch=0<br>column.2.valuefield=scheduledStartDate<br>column.2.valueformat=atDate<br>column.2.width=80<br>column.3.descriptionkey=plannedcompletiondate<br>column.3.linkedname=direct<br>column.3.listsort=atDateAsAtDate(scheduledCompletionDate)<br>column.3.namekey=plannedcompletiondate.abbr<br>column.3.querysort=scheduledCompletionDate<br>column.3.short=false<br>column.3.stretch=0<br>column.3.valuefield=scheduledCompletionDate<br>column.3.valueformat=atDate<br>column.3.width=80<br>column.4.aggregator.displayformat=int<br>column.4.aggregator.function=SUM<br>column.4.aggregator.namekey=id<br>column.4.aggregator.valueexpression=DATEDIFF({scheduledCompletionDate},<br>{scheduledStartDate})+1<br>column.4.aggregator.valueformat=intAsInt<br>column.4.descriptionkey=id<br>column.4.linkedname=direct<br>column.4.listsort=intAsInt(ID)<br>column.4.name=Durata calendario<br>column.4.querysort=ID<br>column.4.short=false<br>column.4.stretch=0<br>column.4.valueexpression=DATEDIFF({scheduledCompletionDate},{scheduledStartDate})+1<br>column.4.valueformat=int<br>column.4.width=80<br>column.5.aggregator.displayformat=int<br>column.5.aggregator.function=SUM<br>column.5.aggregator.namekey=id<br>column.5.aggregator.value.expression=DATEDIFF({scheduledStartDate},{project}.<br>{scheduledStartDate})+0<br>column.5.aggregator.valueformat=intAsInt<br>column.5.descriptionkey=id<br>column.5.linkedname=direct<br>column.5.listsort=intAsInt(ID)<br>column.5.name=Data inizio calendario<br>column.5.querysort=ID<br>column.5.short=false<br>column.5.stretch=0<br>column.5.value eexpression=DATEDIFF({scheduledStartDate},{project}.{scheduledStartDate})+0<br>column.5.valueformat=int<br>column.5.width=80<br>column.6.aggregator.displayformat=int<br>column.6.aggregator.function=SUM<br>column.6.aggregator.namekey=id<br>column.6.aggregator.valueexpression=WEEKDAYDIFF({scheduledStartDate}),<br>{scheduledCompletionDate})+0<br>column.6.aggregator.valueformat=HTML<br>column.6.descriptionkey=id<br>column.6.linkedname=direct<br>column.6.listsort=intAsInt(ID)<br>column.6.name=Durata settimanale del giorno<br>column.6.querysort=ID<br>column.6.short=false<br>column.6.stretch=0<br>column.6.valueexpression=WEEKDAYDIFF({scheduledStartDate},{scheduledCompletionDate})+0<br>column.6.valueformat=int<br>column.6.width=80<br>column.7.aggregator.displayformat=int<br>column.7.aggregator.expression=IF((WEEKDAYDIFF({scheduledStartDate},{scheduledCompletionDate}))&gt;({duration}/480),"Exception",")<br>column.7.aggregator.function=SUM<br>column.7.aggregator.namekey=id<br>column.7.aggregator.valueformat=HTML<br>column.7.linkedname=direct<br>column.7.listsort=intAsInt(ID)<br>column.7.name=Schedule<br>column.7.querysort=ID<br>column.7.short=false<br>column.7.stretch=0<br>column.7.value eexpression=IF((WEEKDAYDIFF({scheduledStartDate},{scheduledCompletionDate}))&gt;({duration}/480),"Exception",")<br>column.7.valueformat=HTML<br>column.7.width=80</pre>

1. Fai clic su **Salva visualizzazione**.
