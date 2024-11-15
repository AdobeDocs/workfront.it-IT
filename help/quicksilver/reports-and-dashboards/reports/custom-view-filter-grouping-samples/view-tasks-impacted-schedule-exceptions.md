---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Visualizza: attività interessate da eccezioni di programmazione"
description: Questa visualizzazione delle attività identifica le attività che dovranno essere completate in ritardo a causa dei fine settimana, del tempo libero personale o di altre eccezioni alla programmazione.
author: Nolan
feature: Reports and Dashboards
exl-id: 7d7c77fa-d9a7-4e91-8dae-ad3aaca6f1da
source-git-commit: 66de6c952272f52876f8e912c96d1526575b6f0b
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 0%

---

# Visualizza: attività interessate da eccezioni di programmazione

<!--Audited: 11/2024-->

Questa visualizzazione delle attività identifica le attività che dovranno essere completate in ritardo a causa dei fine settimana, del tempo libero personale o di altre eccezioni alla programmazione.

In questa vista vengono visualizzati i seguenti elementi:

* Durata delle attività
* Le date di inizio pianificate e di completamento pianificate delle attività
* La durata delle attività in base al numero di giorni tra le date di inizio pianificata e di completamento pianificata delle attività (durata calendario)
* Il numero del giorno della programmazione del progetto all&#39;inizio dell&#39;attività (Data inizio calendario)
* La durata in giorni della settimana delle attività in base al numero di giorni della settimana compresi tra le date di inizio pianificata e di completamento pianificata delle attività (durata in giorni della settimana)
* Se la durata del giorno della settimana è maggiore della durata delle attività, il che indica che la durata delle attività prevede giorni di eccezione, le attività vengono contrassegnate come &quot;Eccezione&quot;.\
  ![attività_con_eccezioni_calendario.png](assets/tasks-with-calendar-exceptions-350x51.png)

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> <p> Corrente: 
   <ul>
   <li>Richiesta di modifica di una vista</li> 
   <li>Pianificare la modifica di un rapporto</li>
   </ul>
     </p>
     <p> Nuovo: 
   <ul>
   <li>Collaboratore per modificare una visualizzazione</li> 
   <li>Standard per modificare un rapporto</li>
   </ul>
     </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari per modificare un rapporto</p> <p>Modificare l'accesso a Filtri, Viste, Raggruppamenti per modificare una vista</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visualizza le attività interessate da eccezioni di programmazione

1. Consente di passare a un elenco di attività.
1. Dal menu a discesa **Visualizza**, selezionare **Nuova visualizzazione**.
1. Nell&#39;area **Anteprima colonna** eliminare tutte le colonne tranne una.
1. Fare clic sull&#39;intestazione della colonna rimanente, quindi fare clic su **Passa a modalità testo** > **Modifica modalità testo**.
1. Rimuovere il testo trovato nella casella **Modifica modalità testo** e sostituirlo con il seguente codice:

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
   column.1.descriptionkey=duration
   column.1.linkedname=direct
   column.1.listsort=intAsInt(durationMinutes)
   column.1.namekey=duration.abbr
   column.1.querysort=durationMinutes
   column.1.shortview=false
   column.1.stretch=0
   column.1.valuefield=durationFieldLong
   column.1.valueformat=compound
   column.1.viewalias=duration
   column.1.width=80
   column.2.descriptionkey=plannedstartdate
   column.2.linkedname=direct
   column.2.listsort=atDateAsAtDate(plannedStartDate)
   column.2.namekey=plannedstartdate.abbr
   column.2.querysort=plannedStartDate
   column.2.shortview=false
   column.2.stretch=0
   column.2.valuefield=plannedStartDate
   column.2.valueformat=atDate
   column.2.width=80
   column.3.descriptionkey=plannedcompletiondate
   column.3.linkedname=direct
   column.3.listsort=atDateAsAtDate(plannedCompletionDate)
   column.3.namekey=plannedcompletiondate.abbr
   column.3.querysort=plannedCompletionDate
   column.3.shortview=false
   column.3.stretch=0
   column.3.valuefield=plannedCompletionDate
   column.3.valueformat=atDate
   column.3.width=80
   column.4.aggregator.displayformat=int
   column.4.aggregator.function=SUM
   column.4.aggregator.namekey=id
   column.4.aggregator.valueexpression=DATEDIFF({plannedCompletionDate},
   {plannedStartDate})+1
   column.4.aggregator.valueformat=intAsInt
   column.4.descriptionkey=id
   column.4.linkedname=direct
   column.4.listsort=intAsInt(ID)
   column.4.name=Calendar Duration
   column.4.querysort=ID
   column.4.shortview=false
   column.4.stretch=0
   column.4.valueexpression=DATEDIFF({plannedCompletionDate},{plannedStartDate})+1
   column.4.valueformat=int
   column.4.width=80
   column.5.aggregator.displayformat=int
   column.5.aggregator.function=SUM
   column.5.aggregator.namekey=id
   column.5.aggregator.valueexpression=DATEDIFF({plannedStartDate},{project}.
   {plannedStartDate})+0
   column.5.aggregator.valueformat=intAsInt
   column.5.descriptionkey=id
   column.5.linkedname=direct
   column.5.listsort=intAsInt(ID)
   column.5.name=Calendar Start Date
   column.5.querysort=ID
   column.5.shortview=false
   column.5.stretch=0
   column.5.valueexpression=DATEDIFF({plannedStartDate},{project}.{plannedStartDate})+0
   column.5.valueformat=int
   column.5.width=80
   column.6.aggregator.displayformat=int
   column.6.aggregator.function=SUM
   column.6.aggregator.namekey=id
   column.6.aggregator.valueexpression=WEEKDAYDIFF({plannedStartDate},
   {plannedCompletionDate})+0
   column.6.aggregator.valueformat=HTML
   column.6.descriptionkey=id
   column.6.linkedname=direct
   column.6.listsort=intAsInt(ID)
   column.6.name=Week Day Duration
   column.6.querysort=ID
   column.6.shortview=false
   column.6.stretch=0
   column.6.valueexpression=WEEKDAYDIFF({plannedStartDate},{plannedCompletionDate})+0
   column.6.valueformat=int
   column.6.width=80
   column.7.aggregator.displayformat=int
   column.7.aggregator.expression=IF((WEEKDAYDIFF({plannedStartDate},{plannedCompletionDate}))>({duration}/480),"Exception","")
   column.7.aggregator.function=SUM
   column.7.aggregator.namekey=id
   column.7.aggregator.valueformat=HTML
   column.7.linkedname=direct
   column.7.listsort=intAsInt(ID)
   column.7.name=Schedule
   column.7.querysort=ID
   column.7.shortview=false
   column.7.stretch=0
   column.7.valueexpression=IF((WEEKDAYDIFF({plannedStartDate},{plannedCompletionDate}))>({duration}/480),"Exception","")
   column.7.valueformat=HTML
   column.7.width=80
   ```

1. Fai clic su **Fine** > **Salva visualizzazione**.
