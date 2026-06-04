---
content-type: overview
product-area: projects
navigation-topic: task-constraints
title: Panoramica sui vincoli delle attività
description: I vincoli dell'attività determinano quando un'attività deve iniziare e finire in un progetto.
author: Alina
feature: Work Management
exl-id: 91b0844b-95a3-4d18-9fdb-a907dd42e1bf
TQID: https://experienceleague.adobe.com/R38RC6-vr-nRp4R7W4WDdJk2KkAuegb6yOfmNLdn7Dc
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b91c0848-76c4-4da4-8b81-3aade0518dd0id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 694
ht-degree: 7%

---

# Panoramica sui vincoli attività

<!-- Audited: 12/2023 -->

I vincoli dell&#39;attività determinano quando un&#39;attività deve iniziare e finire in un progetto.

## Panoramica sui vincoli delle attività

Durante la creazione del piano di progetto, è possibile prendere decisioni sulla sequenza e sull&#39;intervallo di tempo delle attività del progetto. Le attività possono funzionare indipendentemente da qualsiasi sequenza di attività, ma potrebbero influire sulla sequenza temporale del progetto. I vincoli di attività consentono a un project manager di pianificare quando determinate attività possono essere avviate o completate in un progetto.

A seconda del vincolo utilizzato, potrebbe essere necessario specificare una Data inizio pianificata, una Data completamento pianificata o entrambe per l&#39;attività.

I tipi di vincolo che richiedono date definite influiscono sulle relazioni dei predecessori.

>[!TIP]
>
>Si consiglia di utilizzare un tipo di vincolo che non richieda date specifiche se si utilizzano relazioni predecessori tra attività.

Nella tabella seguente vengono visualizzati i vincoli e le relative abbreviazioni. Le abbreviazioni vengono utilizzate negli elenchi delle attività e durante la creazione di file di importazione Kick-Start. Fare clic sul titolo collegato di ogni vincolo attività per ulteriori informazioni su tale tipo di vincolo.

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col>
 <thead> 
  <tr> 
   <th> <p><strong>Nome Vincolo</strong> </p> </th> 
   <th> <p><strong>Abbreviazione</strong> </p> </th> 
   <th> <p><strong>Descrizione</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/as-soon-as-possible.md" class="MCXref xref">Panoramica Vincolo Attività: Il Prima Possibile</a> </p> </td> 
   <td scope="col"> <p>ASAP</p> </td>
   <td scope="col"> <p>Posiziona l'ora di inizio dell'attività il più vicino possibile all'inizio del progetto.</p> 
   <p>Si tratta del vincolo predefinito se il progetto utilizza una modalità di programmazione a partire dalla data di inizio e se la data di inizio predefinita del sistema per una nuova attività è impostata su In base alla data pianificata del progetto. </p>
   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/as-late-as-possible.md" class="MCXref xref">Panoramica Vincolo Attività: Il Più Tardi Possibile </a> </p> </td> 
   <td scope="col"> <p>PTP</p> </td> 
   <td scope="col"> <p>Posiziona il tempo di completamento dell'attività il più vicino possibile alla fine del progetto.</p> 
   <p>Si tratta del vincolo predefinito quando la modalità di pianificazione del progetto è impostata su Data completamento e il valore predefinito del sistema o del gruppo per la data di inizio di un'attività è impostato su Basato sulla data pianificata del progetto. </p>
   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/earliest-available-time.md" class="MCXref xref">Panoramica vincolo attività: primo orario disponibile</a> </p> </td> 
   <td scope="col"> <p>POD</p> </td> 
 <td scope="col"> <p>Consente di pianificare l'inizio di un'attività il prima possibile dopo aver considerato le relazioni precedenti.</p> </td>
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/latest-available-time.md" class="MCXref xref">Panoramica Vincolo Attività: Ultimo Orario Disponibile</a> </p> </td> 
   <td scope="col"> <p>UOT</p> </td> 
   <td scope="col"> <p>Pianifica l'inizio di un'attività al più tardi nel momento disponibile dopo aver considerato le relazioni predecessore-successore nel progetto.</p> </td>
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/start-no-earlier-than.md" class="MCXref xref">Panoramica Vincolo Attività: Iniziare Non Prima Di</a> </p> </td> 
   <td scope="col"> <p>INPD</p> </td> 
   <td scope="col"> <p>Programma l'inizio di un'attività dopo la data specificata.</p> 
   <p>Questo è il vincolo predefinito se la modalità di programmazione del progetto è dalla data di inizio e se la data di inizio predefinita del sistema o del gruppo per una nuova attività è impostata su Oggi.   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/start-no-later-than.md" class="MCXref xref">Panoramica Vincolo Attività: Iniziare Non Più Tardi Di</a> </p> </td> 
   <td scope="col"> <p>INDD</p> </td> 
   <td scope="col"> <p>Programma l'inizio di un'attività prima della data specificata.</p> 
   <p>Si tratta del vincolo predefinito se la modalità di programmazione del progetto è impostata su Data completamento e se il sistema o il gruppo predefinito per la data di inizio di un'attività è impostato su Oggi. 
   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/finish-no-earlier-than.md" class="MCXref xref">Panoramica Vincolo Attività: Fine Non Prima Di</a> </p> </td> 
   <td scope="col"> <p>FNPD</p> </td>
   <td scope="col"> <p>Consente di pianificare il completamento di un'attività dopo la data specificata.</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/finish-no-later-than.md" class="MCXref xref">Panoramica vincolo attività: termina non più tardi di</a> </p> </td> 
   <td scope="col"> <p>FNDD</p> </td> 
   <td scope="col"> <p>Programma il completamento di un'attività prima della data specificata.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/must-start-on.md" class="MCXref xref">Panoramica vincolo attività: deve iniziare il</a> </p> </td> 
   <td scope="col"> <p>DIA</p> </td> 
   <td scope="col"> <p>Consente di programmare l'inizio esatto di un'attività in una data specifica.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/must-finish-on.md" class="MCXref xref">Panoramica Vincolo Attività: Deve Terminare Il</a> </p> </td> 
   <td scope="col"> <p>DFA</p> </td> 
   <td scope="col"> <p>Consente di pianificare la fine di un'attività in una data specifica.</p> </td>
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/fixed-dates.md" class="MCXref xref">Panoramica vincolo attività: date fisse</a> </p> </td> 
   <td> <p>FISSD</p> </td> 
   <td> <p>Programma l'inizio e la fine di un'attività in date specifiche.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Panoramica dei vincoli predefiniti

Quando si creano nuove attività, Workfront seleziona automaticamente un Vincolo attività.

Workfront utilizza due variabili per decidere quale vincolo attività è selezionato per impostazione predefinita per una nuova attività:

* Il campo **Pianificazione progetto da** nel progetto.

  Per informazioni sul campo Pianificazione progetto da, vedere [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md).

* Preferenza **Data inizio** configurata dall&#39;amministratore di Workfront o gruppo nell&#39;area **Attività e problemi** di **Configurazione**.

  Per informazioni sulle preferenze per attività e problemi, consulta la sezione [Nuovi valori predefiniti attività](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md#new-task-defaults) in [Configurare le preferenze per attività e problemi a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

Nella tabella seguente viene illustrato il vincolo attività predefinito quando si scelgono variabili diverse per il progetto e le nuove attività:

| Pianificazione progetto da | Data di inizio attività | Vincolo attività predefinito |
|---|---|---|
| Data di inizio | Sulla base della data pianificata del progetto | Più Presto Possibile |
| Data di inizio | Oggi | Iniziare non Prima di |
| Data di completamento | Sulla base della data pianificata del progetto | Più tardi possibile |
| Data di completamento | Oggi | Iniziare non Dopo di |
