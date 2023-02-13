---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Panoramica sullo stato dell'avanzamento dell'attività
description: Adobe Workfront determina lo stato di avanzamento di un'attività osservando l'avanzamento dell'attività nella relativa timeline. È possibile configurare Workfront per determinare la condizione di un progetto in base al valore dello stato di avanzamento delle attività. Per ulteriori informazioni sulla configurazione della condizione del progetto, consulta l’articolo Panoramica della condizione e del tipo di condizione del progetto.
author: Alina
feature: Work Management
exl-id: 38e5f89e-bdfa-433c-9371-3c3003ada3a3
source-git-commit: 65f25a3b1198f491f7357efef11e2ae075e9721a
workflow-type: tm+mt
source-wordcount: '805'
ht-degree: 1%

---

# Panoramica sullo stato dell&#39;avanzamento dell&#39;attività

Adobe Workfront determina lo stato di avanzamento di un&#39;attività osservando l&#39;avanzamento dell&#39;attività nella relativa timeline. È possibile configurare Workfront per determinare la condizione di un progetto in base al valore dello stato di avanzamento delle attività. Per ulteriori informazioni sulla configurazione della condizione del progetto, consulta l’articolo [Panoramica del tipo di condizione e condizione del progetto](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

## Criteri che determinano lo stato di avanzamento delle attività

Per informazioni sullo stato di avanzamento di un progetto, consulta [Panoramica sullo stato di avanzamento del progetto](../../../manage-work/projects/planning-a-project/project-progress-status.md).

Per informazioni sul tracciamento dell’avanzamento delle attività, consulta [Panoramica sulla modalità di tracciamento delle attività](../../../manage-work/tasks/task-information/task-tracking-mode.md).

I seguenti criteri determinano lo stato di avanzamento di un&#39;attività:

<table> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Stato di Avanzamento</strong> </p> </th> 
   <th> <p><strong>Determinazione dei criteri</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr valign="top"> 
   <td scope="col"> <p> </p> <p><strong>Nei Tempi</strong> </p> </td> 
   <td scope="col"> <p>Un'attività è considerata <strong>Ora di attivazione</strong> quando tutte le date previste corrispondono alle date previste. Questo stato di avanzamento potrebbe inoltre indicare che il progetto è in anticipo rispetto alla pianificazione e che le date previste potrebbero essere precedenti alle date previste.</p> <p>Per ulteriori informazioni sulle date previste, vedi <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">Panoramica della data di completamento prevista per progetti, attività e problemi</a>.</p> <p>Per ulteriori informazioni sulla data di completamento pianificata dell'attività, vedere i seguenti articoli:</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-start-date.md" class="MCXref xref">Panoramica dell'attività Data inizio prevista</a> </p> </li> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Panoramica dell'attività Data completamento pianificata</a> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><p></p> <p><strong>A Rischio</strong> </p> </td> 
   <td><p>Un'attività è considerata <strong>A rischio</strong> quando la data di completamento stimata è successiva alla data di completamento pianificata e successiva alla data di completamento prevista. Ciò può verificarsi quando un'attività presenta un vincolo di <strong>Deve terminare il</strong> o <strong>Deve iniziare</strong> ma la percentuale di completamento o le relazioni predecessori dell'attività mostrano che non può terminare o iniziare alle date specificate. </p><p> Impostazione del vincolo di attività su <strong>Deve terminare il</strong> imposta manualmente la data di completamento pianificata su una data specifica. In questo caso, la data di completamento prevista corrisponde alla data di completamento pianificata. Nel caso di questo vincolo, Workfront analizza l'attività per calcolare quando terminerà in base alla percentuale di completamento. Questo calcolo viene memorizzato come Data di scadenza stimata. Se la Data di scadenza prevista è successiva alla Data di completamento prevista, l'attività è considerata a rischio di ritardo. </p> <p> Impostazione del vincolo di attività su <strong>Deve iniziare</strong> imposta manualmente la data di inizio pianificata su una data specifica. La data di inizio prevista in questo caso corrisponde alla data di inizio pianificata. Nel caso di questo vincolo, Workfront analizza l'attività per calcolare quando verrà avviata in base alle relazioni predecessori. Questo calcolo viene memorizzato come Data di inizio stimata. Se esiste un predecessore imposto che non consente l'inizio dell'attività alla data di inizio specificata, la data di inizio stimata può essere successiva alla data di completamento prevista. Il compito è considerato a rischio di ritardo. </p> <p>Nota: In genere, le date stimate corrispondono a date previste, tranne quando <strong>Deve iniziare</strong> o <strong>Deve terminare il</strong> sono utilizzati. In questi casi, le date stimate continuano a essere calcolate in base alla percentuale di completamento e ad altri fattori (relazioni predecessori), mentre le date previste vengono forzate a corrispondere alle date pianificate impostate manualmente.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Indietro</strong> </p> </td> 
   <td> <p>Un'attività viene considerata come <strong>Dietro</strong> quando la data di completamento stimata è successiva o uguale alla data di completamento pianificata e prima della data di completamento prevista.</p> <p>La data di completamento prevista è una visualizzazione in tempo reale di quando l'attività verrà completata in base all'avanzamento precedente. Anche se l'attività è stata avviata in ritardo, non è ancora considerata in ritardo, perché le date di completamento previste e previste sono ancora in futuro e l'attività potrebbe essere ancora completata in tempo.</p> <p>Nota: La <strong>Dietro</strong> e <strong>A rischio</strong> Lo stato di avanzamento è quasi identico. Tuttavia, <strong>A rischio</strong> indica che esistono alcuni vincoli di task forzati (devono terminare il giorno, devono iniziare il giorno, date corrette) in una o entrambe le date previste. Se l'attività non presenta vincoli forzati, le date previste sono uguali alle date stimate e riflettono il calcolo del sistema della data di completamento in base all'avanzamento corrente dell'attività. L'attività non è ancora considerata in ritardo, perché le date di completamento previste e previste sono ancora in futuro e l'attività potrebbe essere ancora completata in tempo.<br>Per ulteriori informazioni sulle date previste e stimate, vedi <a href="../../../manage-work/tasks/task-information/differentiate-projected-estimated-dates.md" class="MCXref xref">Differenziare tra date previste e date stimate </a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>In Ritardo</strong> </p> </td> 
   <td> <p>Un'attività è <strong>In ritardo</strong> quando la data di completamento pianificata è anteriore alla data odierna.<br></p> </td> 
  </tr> 
 </tbody> 
</table>

## Aggiornamenti dello stato di avanzamento dell&#39;attività nel tempo

I diversi tipi di data nei nostri progetti ci spiegano come avvengono le attività nel tempo:

* Nei Tempi

   ![](assets/on-time-progress-status-350x233.png)

* A Rischio

   ![](assets/at-risk-progress-status-350x233.png)

* Indietro

   ![](assets/behind-progress-status-350x233.png)

* In Ritardo

   ![](assets/late-progress-status-350x233.png)
