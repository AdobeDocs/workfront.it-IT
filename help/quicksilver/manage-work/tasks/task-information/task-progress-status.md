---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Panoramica sullo stato di avanzamento dell’attività
description: Adobe Workfront determina lo stato di avanzamento di un’attività osservando l’avanzamento dell’attività nella relativa sequenza temporale. È possibile configurare Workfront per determinare la condizione di un progetto in base al valore dello stato di avanzamento delle attività. Per ulteriori informazioni sulla configurazione della condizione del progetto, consulta l’articolo Panoramica della condizione e del tipo di condizione del progetto.
author: Alina
feature: Work Management
exl-id: 38e5f89e-bdfa-433c-9371-3c3003ada3a3
source-git-commit: 811d8076a0b344e863b25aa253a0fb1c102f0435
workflow-type: tm+mt
source-wordcount: '777'
ht-degree: 0%

---

# Panoramica sullo stato di avanzamento dell’attività

<!-- Audited: 1/2024 -->

Adobe Workfront determina lo stato di avanzamento di un’attività osservando l’avanzamento dell’attività nella relativa sequenza temporale. È possibile configurare Workfront per determinare la condizione di un progetto in base al valore dello stato di avanzamento delle attività. Per ulteriori informazioni sulla configurazione della condizione del progetto, vedere l&#39;articolo [Panoramica della condizione e del tipo di condizione del progetto](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

## Criteri che determinano lo stato di avanzamento delle attività

Per informazioni sullo stato di avanzamento di un progetto, vedere [Panoramica sullo stato di avanzamento del progetto](../../../manage-work/projects/planning-a-project/project-progress-status.md).

Per informazioni sul monitoraggio dell&#39;avanzamento delle attività, vedere [Panoramica sulla modalità di monitoraggio attività](../../../manage-work/tasks/task-information/task-tracking-mode.md).

I seguenti criteri determinano lo stato di avanzamento di un&#39;attività:

<table> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Stato di avanzamento</strong> </p> </th> 
   <th> <p><strong>Determinazione dei criteri</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr valign="top"> 
   <td scope="col"> <p> </p> <p><strong>Ora di attivazione</strong> </p> </td> 
   <td scope="col"> <p>Un'attività viene considerata <strong>Alla data</strong> quando tutte le date pianificate corrispondono alle date previste. Questo stato di avanzamento potrebbe anche indicare che il progetto è in anticipo rispetto alla programmazione e che le date previste potrebbero essere precedenti alle date pianificate.</p> <p>Per ulteriori informazioni sulle date previste, vedere <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">Panoramica sulla data di completamento prevista per progetti, attività e problemi</a>.</p> <p>Per ulteriori informazioni sulla data di completamento pianificata per l'attività, vedere i seguenti articoli:</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-start-date.md" class="MCXref xref">Panoramica della data di inizio pianificata dell'attività</a> </p> </li> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Panoramica della data di completamento pianificata dell'attività</a> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><p></p> <p><strong>A Rischio</strong> </p> </td> 
   <td><p>Un'attività è considerata <strong>A rischio</strong> quando la data di completamento stimata è successiva alla data di completamento pianificata e alla data di completamento prevista. Ciò può verificarsi quando un'attività ha un vincolo di <strong>Deve finire il</strong> o <strong>Deve iniziare il</strong> ma la percentuale di completamento o le relazioni predecessore dell'attività mostrano che non può finire o iniziare nelle date specificate. </p><p> Se si imposta il vincolo attività su <strong>Deve finire il</strong>, la data di completamento pianificata viene impostata manualmente su una data specifica. In questo caso, la data di completamento prevista corrisponde alla data di completamento pianificata. Nel caso di questo vincolo, Workfront analizza l’attività per calcolare quando finirà in base alla percentuale di completamento. Questo calcolo viene memorizzato come Data di scadenza stimata. Se la data di scadenza stimata è successiva alla data di completamento prevista, l'attività è considerata a rischio di ritardo. </p> <p> Se si imposta il vincolo attività su <strong>Deve iniziare il</strong>, la data di inizio pianificata viene impostata manualmente su una data specifica. In questo caso, la data di inizio prevista corrisponde alla data di inizio pianificata. Nel caso di questo vincolo, Workfront analizza l'attività per calcolare quando inizierà in base alle relazioni precedenti. Questo calcolo viene memorizzato come Data di inizio stimata. Se esiste un predecessore imposto che non consente all'attività di iniziare alla data di inizio specificata, la data di inizio stimata può essere successiva alla data di completamento prevista. L'attività è considerata a rischio di ritardo. </p> <p>Nota: in genere, le date stimate corrispondono alle date previste, tranne quando <strong>deve iniziare il</strong> o <strong>deve finire il</strong> vengono utilizzati. In questi casi, le Date stimate continuano a essere calcolate in base alla percentuale di completamento e ad altri fattori (relazioni predecessori), mentre le Date previste sono obbligate a corrispondere alle Date pianificate che sono state impostate manualmente.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Indietro</strong> </p> </td> 
   <td> <p>Un'attività è considerata <strong>Indietro</strong> quando la data di completamento stimata è successiva o uguale alla data di completamento pianificata e precedente alla data di completamento prevista.</p> <p>La Data di completamento prevista è una visualizzazione in tempo reale di quando l'attività verrà completata in base all'avanzamento precedente. Anche se l'attività è stata avviata in ritardo, non è ancora considerata in ritardo, perché le date di completamento pianificate e previste sono ancora nel futuro e l'attività potrebbe essere ancora completata in tempo.</p> <p>Nota: gli stati di avanzamento <strong>Indietro</strong> e <strong>A rischio</strong> sono quasi identici. Tuttavia, <strong>A rischio</strong> indica che sono presenti alcuni vincoli di attività forzati (Deve finire il, Deve iniziare il, Date fisse) in una o entrambe le date pianificate. Se l'attività non è soggetta a vincoli, le Date previste corrispondono alle Date stimate e riflettono il calcolo di sistema della Data di completamento in base all'avanzamento corrente dell'attività. L'attività non è ancora considerata in ritardo perché le date di completamento pianificate e previste sono ancora nel futuro e l'attività potrebbe essere completata in tempo.<br>Per ulteriori informazioni sulle date previste e stimate, vedere <a href="../../../manage-work/tasks/task-information/differentiate-projected-estimated-dates.md" class="MCXref xref">Panoramica sulle date previste e stimate </a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>In Ritardo</strong> </p> </td> 
   <td> <p>Un'attività è <strong>In ritardo</strong> quando la data di completamento pianificata è precedente alla data odierna.<br></p> </td> 
  </tr> 
 </tbody> 
</table>

<!--hiding this because some users find the images confusing, as they don't really show the dates mentioned in the descriptions above. Keep the pictures though, in case some users will complain that we hid them. 

## How task Progress Status updates over time

The different date types in our projects tell us how tasks are progressing over time:

* On Time

  ![](assets/on-time-progress-status-350x233.png)

* At Risk

  ![](assets/at-risk-progress-status-350x233.png)

* Behind

  ![](assets/behind-progress-status-350x233.png)

* Late

  ![](assets/late-progress-status-350x233.png)

-->