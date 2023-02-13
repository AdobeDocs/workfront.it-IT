---
content-type: overview
product-area: projects
navigation-topic: task-constraints
title: Panoramica sul vincolo di attività
description: I vincoli dell'attività determinano quando un'attività deve iniziare e terminare su un progetto.
author: Alina
feature: Work Management
exl-id: 91b0844b-95a3-4d18-9fdb-a907dd42e1bf
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 10%

---

# Panoramica sul vincolo di attività

I vincoli dell&#39;attività determinano quando un&#39;attività deve iniziare e terminare su un progetto.

## Panoramica dei vincoli di attività

Man mano che crei il piano di progetto, prendi decisioni sulla sequenza e l’intervallo di tempo delle attività sul progetto. Le attività possono funzionare indipendentemente da qualsiasi sequenza di attività, ma potrebbero influire sulla timeline del progetto. I vincoli task consentono a un project manager di pianificare quando determinate attività possono essere avviate o completate su un progetto.

A seconda del vincolo utilizzato, potrebbe essere necessario specificare una data di inizio pianificata, una data di completamento pianificata o entrambe per l&#39;attività.

I tipi di vincolo che richiedono date definite influiscono sulle relazioni predecessori.

>[!TIP]
>
>È consigliabile utilizzare un tipo di vincolo che non richiede date specifiche se si utilizzano relazioni precedenti tra attività.

Nella tabella seguente vengono visualizzati ogni vincolo e la relativa abbreviazione. Le abbreviazioni vengono utilizzate negli elenchi delle attività e durante la creazione di file di importazione Kick-Start. Fare clic sul titolo collegato di ciascun vincolo di attività per ulteriori informazioni su tale tipo di vincolo.

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Nome vincolo</strong> </p> </th> 
   <th> <p><strong>Abbreviazione</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/as-soon-as-possible.md" class="MCXref xref">Panoramica sul vincolo di attività: Il più presto possibile</a> </p> </td> 
   <td scope="col"> <p>ASAP</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/as-late-as-possible.md" class="MCXref xref">Panoramica sul vincolo di attività: Il più tardi possibile </a> </p> </td> 
   <td scope="col"> <p>PTP</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/earliest-available-time.md" class="MCXref xref">Panoramica sul vincolo di attività: Tempo disponibile</a> </p> </td> 
   <td scope="col"> <p>POD</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/latest-available-time.md" class="MCXref xref">Panoramica sul vincolo di attività: Ora disponibile più recente</a> </p> </td> 
   <td scope="col"> <p>UOT</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/start-no-earlier-than.md" class="MCXref xref">Panoramica sul vincolo di attività: Inizia non prima di</a> </p> </td> 
   <td scope="col"> <p>INPD</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/start-no-later-than.md" class="MCXref xref">Panoramica sul vincolo di attività: Inizia non oltre</a> </p> </td> 
   <td scope="col"> <p>INDD</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/finish-no-earlier-than.md" class="MCXref xref">Panoramica sul vincolo di attività: Fine Non Precedente A</a> </p> </td> 
   <td scope="col"> <p>FNPD</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/finish-no-later-than.md" class="MCXref xref">Panoramica sul vincolo di attività: Fine entro</a> </p> </td> 
   <td scope="col"> <p>FNDD</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/must-start-on.md" class="MCXref xref">Panoramica sul vincolo di attività: Deve iniziare</a> </p> </td> 
   <td scope="col"> <p>DIA</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/must-finish-on.md" class="MCXref xref">Panoramica sul vincolo di attività: Deve terminare il</a> </p> </td> 
   <td scope="col"> <p>DFA</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/fixed-dates.md" class="MCXref xref">Panoramica sul vincolo di attività: Date fisse</a> </p> </td> 
   <td> <p>FISSD</p> </td> 
  </tr> 
 </tbody> 
</table>

## Panoramica dei vincoli predefiniti

Quando si creano nuove attività, Workfront seleziona automaticamente un Vincolo attività.

Workfront utilizza due variabili per decidere quale Vincolo di attività è selezionato per impostazione predefinita per una nuova attività:

* La **Pianificazione del progetto da** sul progetto.

   Per informazioni sul campo Pianificazione del progetto da, vedere [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md).

* La **Data di inizio** preferenza configurata dal tuo amministratore di Workfront o di gruppo in **Attività e problemi** area **Configurazione**.

   Per informazioni sulle preferenze Attività e Problemi, consulta la sezione &quot;Nuovi valori predefiniti attività&quot; in [Configurare le preferenze relative alle attività e ai problemi a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

La tabella seguente mostra il Vincolo attività predefinito quando si scelgono variabili diverse per il progetto e le nuove attività:

| Pianificazione del progetto da | Data inizio attività | Predefinito vincolo attività |
|---|---|---|
| Data di inizio | Sulla base della data pianificata del progetto | Più Presto Possibile |
| Data di inizio | Oggi | Iniziare non Prima di |
| Data di completamento | Sulla base della data pianificata del progetto | Il più tardi possibile |
| Data di completamento | Oggi | Iniziare non Dopo di |
