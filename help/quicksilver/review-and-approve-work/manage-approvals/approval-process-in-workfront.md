---
content-type: overview
product-area: projects
navigation-topic: approvals
title: Panoramica del processo di approvazione
description: È possibile creare un processo di approvazione e allegarlo a un oggetto per assicurarsi che gli utenti designati verifichino determinate modifiche prima che l'oggetto progredisca.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: dd0822b6-80f1-4a2e-bf6a-0c425984f4d0
source-git-commit: e4de185f172b173dcc3ad966afa69ffb3bc479eb
workflow-type: tm+mt
source-wordcount: '1752'
ht-degree: 0%

---

# Panoramica del processo di approvazione

<!-- Audited: 12/2023 -->

È possibile creare un processo di approvazione e allegarlo a un oggetto per assicurarsi che gli utenti designati verifichino determinate modifiche prima che l&#39;oggetto progredisca.

Questa funzione è disponibile per i seguenti tipi di oggetti in Adobe Workfront:

* Elemento di lavoro (progetto, attività o problema, modello, attività modello)
* Documento
* Bozza

Questo articolo contiene informazioni generali sui processi di approvazione associati agli elementi di lavoro.
Per istruzioni sulla creazione di un processo di approvazione, vedere [Creare un processo di approvazione per gli elementi di lavoro](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Tipi di processi di approvazione per gli elementi di lavoro

Se sei un amministratore di Adobe Workfront o un utente con accesso amministrativo ai processi di approvazione, puoi creare i seguenti processi di approvazione per progetti, attività e problemi:

* **Processo di approvazione globale a livello di sistema**: gli utenti possono allegarli a uno dei seguenti elementi:

   * Un progetto, un’attività o un problema nella sezione Approvazioni
   * Nella casella Modifica progetto dell&#39;area Processo di approvazione predefinito attività
   * Nella sezione Dettagli coda o Argomento coda di un progetto nelle aree Processo di approvazione predefinito. Il progetto deve essere abilitato come coda di richieste.

* **Processo di approvazione globale a livello di gruppo**: gli utenti possono allegarli ai seguenti elementi:

   * Progetto, attività o problema appartenente al gruppo associato al processo di approvazione nella sezione Approvazioni
   * Nella casella Modifica progetto dell&#39;area Processo di approvazione predefinito attività per un progetto appartenente al gruppo associato al processo di approvazione
   * Nella sezione Dettagli coda o Argomento coda di un progetto nelle aree Processo di approvazione predefinito. Il progetto deve essere abilitato come coda di richieste e deve appartenere al gruppo associato al processo di approvazione.

  Per informazioni sulla creazione di un processo di approvazione a livello di sistema o di gruppo, vedere [Creare un processo di approvazione per gli elementi di lavoro](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

* **Processo di approvazione a utente singolo**: da utilizzare con un progetto, un&#39;attività, un problema, un modello o un&#39;attività modello. Questo tipo di processo di approvazione influisce solo sull&#39;oggetto associato e non è disponibile per essere associato ad altri oggetti.

  Per informazioni sulla creazione di un processo di approvazione a utente singolo, vedere [Associare un processo di approvazione nuovo o esistente al lavoro](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

>[!NOTE]
>
>In questo articolo viene utilizzato il termine &quot;processo di approvazione globale&quot; per differenziarlo dal termine &quot;processo di approvazione a utente singolo&quot;. Un processo di approvazione globale può essere utilizzato ripetutamente.
>
>Il termine &quot;processo di approvazione globale a livello di gruppo&quot; si riferisce a un processo di approvazione che può essere utilizzato ripetutamente per gli elementi e con stati associati solo a un gruppo specifico.

Per informazioni sulla creazione di un processo di approvazione a livello di sistema o di gruppo, vedere [Creare un processo di approvazione per gli elementi di lavoro](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Considerazioni sui processi di approvazione

* È necessario creare il progetto, l’attività, il problema, il modello o l’attività modello prima di associare il processo di approvazione.
* Un processo di approvazione è sempre associato a due elementi essenziali:

   * Ogni processo di approvazione corrisponde a un determinato stato di elemento di lavoro nel sistema Workfront. Quando si modifica lo stato di un elemento di lavoro, un&#39;approvazione allegata per tale stato richiede la conferma della modifica dello stato prima che sia possibile assegnare il nuovo stato all&#39;elemento.

     >[!TIP]
     >
     >
     >   
     >   
     >   * È possibile associare un&#39;approvazione a livello di gruppo a uno stato globale o di gruppo.
     >   * Non è possibile modificare lo stato di un articolo che utilizza un processo di approvazione in uno stato diverso da quello associato al processo di approvazione.
     >   
     >   
     >     Se ad esempio si dispone di un&#39;approvazione dell&#39;attività associata allo stato In corso, al momento della concessione dell&#39;approvazione lo stato dell&#39;attività verrà automaticamente modificato in In corso. Non può cambiare automaticamente il suo stato in Completato o in qualsiasi altro stato non associato all’approvazione.
     >   
     >   
     >

   * Le entità associate a un processo di approvazione possono essere utenti, ruoli o team. Gli utenti sono in ultima analisi responsabili dell’accettazione o del rifiuto dell’approvazione. Puoi assegnare le approvazioni agli utenti che svolgono un determinato ruolo nel progetto. Ad esempio, puoi assegnare un’approvazione a un Proprietario del progetto o a uno Sponsor. Per ulteriori informazioni, vedere [Creare un processo di approvazione per gli elementi di lavoro](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

     Esistono i seguenti scenari:

      * Quando si assegna un&#39;approvazione alle mansioni, qualsiasi utente del team di progetto associato alla mansione può prendere una decisione in merito all&#39;approvazione. Il ruolo associato all’approvazione può essere il ruolo principale o qualsiasi altro ruolo.

        Per informazioni sul team di progetto, vedere [Panoramica team di progetto](../../manage-work/projects/planning-a-project/project-team-overview.md).

      * Quando si assegna un&#39;approvazione a un team, qualsiasi membro di tale team può prendere una decisione sull&#39;approvazione. Il team associato all’approvazione può essere il proprio team predefinito o uno qualsiasi degli altri team.

        Per informazioni sui ruoli e i team di un utente, vedere [Modificare il profilo di un utente](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Quando si crea un elemento di lavoro, non viene automaticamente associato un processo di approvazione. Se desideri utilizzarne uno, devi allegarne manualmente uno. Per informazioni su come allegare un processo di approvazione a un elemento, vedere [Associare un processo di approvazione nuovo o esistente a un lavoro](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
* L’amministratore di Workfront o un utente con accesso amministrativo ai processi di approvazione può creare un processo di approvazione globale a livello di sistema da utilizzare in tutto il sistema. Un amministratore di gruppo con accesso amministrativo ai processi di approvazione può creare un processo di approvazione globale a livello di gruppo per l&#39;utilizzo solo da parte di un determinato gruppo che gestisce.
* Se non si desidera utilizzare un processo di approvazione globale predefinito a livello di sistema o di gruppo per un elemento di lavoro, è possibile creare e allegare un processo di approvazione a utente singolo quando si dispone delle autorizzazioni Gestione per l&#39;oggetto al quale si desidera allegare il processo di approvazione.

  >[!NOTE]
  >
  >È possibile utilizzare un processo di approvazione monouso una sola volta per l&#39;elemento specifico per il quale è stato creato. È possibile associare stati globali e stati a livello di gruppo ai processi di approvazione a utente singolo per progetti, attività, problemi, modelli e attività modello.

* Quando si allega un processo di approvazione a livello di gruppo a un elemento utilizzando gli stati personalizzati a livello di gruppo, la modifica del gruppo del progetto potrebbe creare un conflitto tra gli stati di approvazione del gruppo precedente e quelli esistenti a livello di sistema. Prima di aggiornare il gruppo, è consigliabile rimuovere i processi di approvazione a livello di gruppo sul progetto, le relative attività o i problemi. Per informazioni sulla creazione di processi di approvazione a livello di gruppo, vedere [Processi di approvazione a livello di gruppo](../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md). Per informazioni sulla creazione di stati di gruppo personalizzati, vedere [Creare o modificare lo stato di un gruppo](../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md). Per informazioni sull&#39;aggiornamento del gruppo di un progetto, vedere [Modifica progetti](../../manage-work/projects/manage-projects/edit-projects.md).

## Flusso di lavoro del processo di approvazione

In questa sezione vengono illustrate le seguenti informazioni sull&#39;approvazione degli elementi di lavoro:

* [Utilizzo degli stati nei processi di approvazione](#how-approval-processes-rely-on-statuses)
* [Utilizzo di un processo di approvazione in un flusso di lavoro tipico](#how-a-typical-workflow-uses-an-approval-process)

### Come i processi di approvazione si basano sugli stati {#how-approval-processes-rely-on-statuses}

L&#39;associazione di uno stato a un processo di approvazione garantisce che l&#39;articolo si sposti tra i reparti nell&#39;ordine corretto.

**Esempio:** È possibile allegare un processo di approvazione allo stato del reparto marketing che richiede l&#39;approvazione del reparto finanziario. Quindi, quando qualcuno cambia lo stato di un elemento di lavoro in &quot;Reparto marketing&quot;, l&#39;elemento non può essere spostato in quel reparto fino a quando il reparto finanziario non lo firma.

Per ulteriori informazioni sugli stati degli elementi di lavoro, vedere gli articoli seguenti:

* [Accedere all&#39;elenco degli stati del progetto di sistema](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md)
* [Accedere all&#39;elenco degli stati delle attività di sistema](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md)
* [Accedere all’elenco degli stati dei problemi di sistema](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md)

### Utilizzo di un processo di approvazione in un flusso di lavoro tipico {#how-a-typical-workflow-uses-an-approval-process}

Lo scenario seguente illustra come un processo di approvazione consente agli utenti di approvare il lavoro mentre un oggetto Workfront procede attraverso un flusso di lavoro costituito da diversi passaggi in questo ordine:

1. L’amministratore di Workfront o un utente con accesso amministrativo ai processi di approvazione crea un processo di approvazione per un progetto, un’attività o un problema.

   >[!NOTE]
   >
   >È possibile allegare i processi di approvazione del progetto a un modello e i processi di approvazione delle attività a un&#39;attività modello. Dopo questa operazione, quando un utente utilizza il modello per creare un progetto, il processo di approvazione diventa un processo di approvazione rispettivamente di un progetto o di un&#39;attività. Un processo di approvazione a utente singolo associato a un modello o a un&#39;attività modello rimane un processo di approvazione a utente singolo per progetti e attività.

1. Un utente con l’autorizzazione Manage (Gestisci) per il progetto, l’attività o il problema allega il processo di approvazione all’elemento o crea un’approvazione per un singolo utente.
1. L&#39;utente assegnato all&#39;elemento di lavoro cambia lo stato in cui si trova l&#39;utente che avvia il processo di approvazione. La persona che ha creato il processo di approvazione ha definito la relazione tra lo stato e il processo di approvazione.
1. Gli approvatori designati ricevono una notifica relativa al processo di approvazione in sospeso ed esaminano l&#39;elemento di lavoro.
1. Il processo di approvazione termina dopo che gli approvatori designati hanno approvato tutte le fasi del processo. Oppure, se rifiutano un passaggio, lo stato viene reimpostato su uno stato predefinito o viene creato un problema. La persona che ha creato il processo di approvazione ha definito quale di questi passaggi automatici si verifica dopo un rifiuto.

**Esempio:** un team addetto alla pubblicità ha creato uno stato denominato Pronto per la stampa e un processo di approvazione denominato Conclusione di Designer/Copywriter associato a questo stato. Questo processo di approvazione è configurato per:

* Richiedi l&#39;approvazione del progettista e del redattore del team
* Avvia ogni volta che qualcuno cambia lo stato di un elemento di lavoro in Pronto per la stampa

Il proprietario di un progetto di brochure allega il processo di approvazione della conclusione del copywriter/Designer al progetto di brochure.

Quando un utente del progetto cambia lo stato in Pronto per la stampa, il redattore e il designer ricevono una notifica in cui viene richiesto di approvare o rifiutare il progetto. Durante il processo di approvazione, quando si decide se approvarlo o meno, lo stato dei progetti viene visualizzato come Pronto per la stampa - In attesa di approvazione.

Dopo che entrambi hanno approvato la brochure in Workfront, lo stato del progetto cambia in Pronto per la stampa.

## Processi di approvazione dei documenti

Le approvazioni dei documenti vengono utilizzate per un&#39;approvazione più generale. Il feedback viene acquisito in formato chat nella scheda Aggiornamenti. È possibile utilizzare i pulsanti di approvazione per approvare, rifiutare o approvare con modifiche.

Per aggiungere approvatori a un documento dopo che è stato caricato in Workfront, vedi [Richiedi approvazioni documento](../../review-and-approve-work/manage-approvals/request-document-approvals.md).

## Processi di approvazione bozza

Le approvazioni delle bozze vengono utilizzate per una revisione più approfondita e in genere includono flussi di lavoro più complicati. Il feedback viene acquisito con gli strumenti di markup nel visualizzatore di bozze. È possibile utilizzare i pulsanti di approvazione per approvare, rifiutare o approvare con modifiche.

Per aggiungere un flusso di lavoro automatico a una bozza di documento e designare determinati utenti nel flusso di lavoro come approvatori della bozza, vedere [Creare una bozza avanzata con un flusso di lavoro automatico](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

## Configurazione delle impostazioni per i processi di approvazione degli elementi di lavoro

In qualità di amministratore di Workfront, puoi configurare le impostazioni globali per i processi di approvazione degli elementi di lavoro nel tuo sistema. Queste impostazioni determinano diverse regole per i processi di approvazione, ad esempio per quanto tempo una decisione di approvazione deve rimanere aperta o come gestisci la delega di approvazione nel sistema. Per ulteriori informazioni sulle impostazioni del processo di approvazione, vedere [Configurare le impostazioni di approvazione globali](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md).
