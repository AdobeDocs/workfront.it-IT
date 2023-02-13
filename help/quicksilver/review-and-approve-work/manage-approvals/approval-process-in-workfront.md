---
content-type: overview
product-area: projects
navigation-topic: approvals
title: Panoramica del processo di approvazione
description: È possibile creare un processo di approvazione e allegarlo a un oggetto per assicurarsi che gli utenti designati rivedano alcune modifiche prima che l'oggetto progredisca.
author: Courtney
feature: Work Management
exl-id: dd0822b6-80f1-4a2e-bf6a-0c425984f4d0
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1747'
ht-degree: 0%

---

# Panoramica del processo di approvazione

È possibile creare un processo di approvazione e allegarlo a un oggetto per assicurarsi che gli utenti designati rivedano alcune modifiche prima che l&#39;oggetto progredisca.

Questa funzione è disponibile per i seguenti tipi di oggetti in Adobe Workfront:

* Elemento di lavoro (progetto, attività o problema, modello, attività modello)
* Documento
*  Bozza

Per istruzioni sulla creazione di un processo di approvazione, consulta [Creazione di un processo di approvazione per gli elementi di lavoro](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

Questo articolo contiene informazioni generali sui processi di approvazione associati agli elementi di lavoro.

## Tipi di processi di approvazione

Se sei un amministratore di Adobe Workfront o un utente con accesso amministrativo ai processi di approvazione, puoi creare i seguenti processi di approvazione per progetti, attività e problemi:

* **Un processo di approvazione globale a livello di sistema**: Gli utenti possono allegarli a uno dei seguenti elementi:

   * Un progetto, un&#39;attività o un problema nella sezione Approvazioni
   * Nella casella Modifica progetto, l&#39;area Processo di approvazione predefinito attività
   * Nella sezione Dettagli coda o Argomento coda di un progetto, nelle aree Processo approvazione predefinito. Il progetto deve essere abilitato come coda di richiesta.

* **Un processo di approvazione globale a livello di gruppo**: Gli utenti possono allegarli ai seguenti elementi:

   * Un progetto, un task o un problema appartenente al gruppo associato al processo di approvazione nella sezione Approvazioni
   * Nella casella Modifica progetto, l&#39;area Processo di approvazione predefinito attività per un progetto appartenente al gruppo associato al processo di approvazione
   * Nella sezione Dettagli coda o Argomento coda di un progetto, nelle aree Processo approvazione predefinito. Il progetto deve essere abilitato come coda di richiesta e deve appartenere al gruppo associato al processo di approvazione.

   Per informazioni sulla creazione di un processo di approvazione a livello di sistema o di gruppo, consulta [Creazione di un processo di approvazione per gli elementi di lavoro](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

* **Un processo di approvazione ad uso singolo**: Da utilizzare con un singolo progetto, attività, problema, modello o modello. Questo tipo di processo di approvazione influisce solo sull&#39;oggetto ad esso associato e non è disponibile per essere associato ad altri oggetti.

   Per informazioni sulla creazione di un processo di approvazione a uso singolo, vedi [Associa un processo di approvazione nuovo o esistente al lavoro](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

>[!NOTE]
>
>Questo articolo utilizza il termine &quot;processo di approvazione globale&quot; per differenziarsi dal &quot;processo di approvazione a uso singolo&quot;. È possibile utilizzare ripetutamente un processo di approvazione globale.
>
>Il termine &quot;processo di approvazione globale a livello di gruppo&quot; si riferisce a un processo di approvazione che può essere utilizzato ripetutamente per gli elementi e con gli stati associati solo a un gruppo specifico.

Per informazioni sulla creazione di un processo di approvazione a livello di sistema o di un processo di approvazione a livello di gruppo, vedere [Creazione di un processo di approvazione per gli elementi di lavoro](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Considerazioni sui processi di approvazione

* È necessario creare il progetto, l&#39;attività, il problema, il modello o l&#39;attività del modello prima che il processo di approvazione possa essere associato ad essi.
* Un processo di approvazione è sempre associato a due elementi essenziali:

   * Ogni processo di approvazione corrisponde a un determinato stato dell&#39;elemento di lavoro nel sistema Workfront. Quando si modifica lo stato di un elemento di lavoro, un&#39;approvazione associata per tale stato richiede che la modifica dello stato venga confermata prima che il nuovo stato possa essere assegnato all&#39;elemento.

      >[!TIP]
      >
      >
      >   
      >   
      >   * È possibile associare un&#39;approvazione a livello di gruppo a uno stato globale o a livello di gruppo.
      >   * Non è possibile modificare lo stato di un elemento utilizzando un processo di approvazione in uno stato diverso da quello associato al processo di approvazione.

         >   
         >   
         >     Ad esempio, se si dispone di un&#39;approvazione di un&#39;attività associata allo stato In corso, al momento della concessione dell&#39;approvazione l&#39;attività cambia automaticamente il suo stato in In corso. Non può cambiare automaticamente il proprio stato in Completato o in qualsiasi altro stato non associato all&#39;approvazione.


   * Le entità associate a un processo di approvazione possono essere utenti, ruoli o team. In ultima analisi, gli utenti sono responsabili dell’accettazione o del rifiuto dell’approvazione. Puoi assegnare le approvazioni agli utenti che svolgono un ruolo specifico nel progetto. Ad esempio, puoi assegnare un&#39;approvazione a un Proprietario del progetto o Sponsor. Per ulteriori informazioni, consulta [Creazione di un processo di approvazione per gli elementi di lavoro](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

      Esistono i seguenti scenari:

      * Quando si assegna un&#39;approvazione ai ruoli di lavoro, qualsiasi utente del team di progetto associato al ruolo di lavoro può decidere in merito all&#39;approvazione. Il ruolo associato all’approvazione può essere il relativo Ruolo principale o qualsiasi Altro Ruolo.

         Per informazioni sul team di progetto, consulta [Panoramica del team di progetto](../../manage-work/projects/planning-a-project/project-team-overview.md).

      * Quando assegni un&#39;approvazione a un team, qualsiasi membro del team può prendere una decisione sull&#39;approvazione. Il team associato all&#39;approvazione può essere il proprio Home Team o uno qualsiasi degli Altri Team.

         Per informazioni sui ruoli e i team di un utente, consulta [Modificare il profilo di un utente](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Quando si crea un elemento di lavoro, non viene automaticamente allegato un processo di approvazione. Se si desidera utilizzarne uno manualmente, è necessario allegarne uno. Per informazioni sull&#39;associazione di un processo di approvazione a un elemento, vedere [Associa un processo di approvazione nuovo o esistente al lavoro](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
* L&#39;amministratore Workfront o un utente con accesso amministrativo ai processi di approvazione può creare processi di approvazione globali a livello di sistema da utilizzare in tutto il sistema. Un amministratore di gruppo con accesso amministrativo ai processi di approvazione può creare un processo di approvazione globale a livello di gruppo da utilizzare solo da un determinato gruppo gestito.
* Se non si desidera utilizzare un processo di approvazione globale predefinito a livello di sistema o di gruppo per un elemento di lavoro, è possibile creare e allegare ad esso un processo di approvazione a uso singolo quando si dispone delle autorizzazioni Gestisci per l&#39;oggetto per il quale si desidera allegare il processo di approvazione.

   >[!NOTE]
   È possibile utilizzare un processo di approvazione a uso singolo una sola volta per l&#39;elemento specifico per il quale è stato creato. È possibile associare gli stati globali e gli stati a livello di gruppo per i processi di approvazione a uso singolo per progetti, attività, problemi, modelli e task modello.

* Quando si associa un processo di approvazione a livello di gruppo a un elemento utilizzando gli stati personalizzati a livello di gruppo, la modifica del gruppo del progetto potrebbe creare un conflitto tra gli stati di approvazione del gruppo precedente e quelli esistenti a livello di sistema. È consigliabile rimuovere i processi di approvazione a livello di gruppo sul progetto, oppure i relativi compiti o problemi prima di aggiornare il gruppo. Per informazioni sulla creazione di processi di approvazione a livello di gruppo, consulta [Processi di approvazione a livello di gruppo](../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md). Per informazioni sulla creazione di stati di gruppo personalizzati, consulta [Creare o modificare uno stato di gruppo](../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md). Per informazioni sull’aggiornamento del gruppo di un progetto, consulta [Modifica progetti](../../manage-work/projects/manage-projects/edit-projects.md).

## Flusso di lavoro del processo di approvazione

In questa sezione viene illustrato quanto segue sull&#39;approvazione degli elementi di lavoro:

* [Come i processi di approvazione si basano sugli stati](#how-approval-processes-rely-on-statuses)
* [Utilizzo di un processo di approvazione da parte di un flusso di lavoro tipico](#how-a-typical-workflow-uses-an-approval-process)

### Come i processi di approvazione si basano sugli stati {#how-approval-processes-rely-on-statuses}

L&#39;associazione di uno stato a un processo di approvazione garantisce che l&#39;articolo si muova nei reparti nell&#39;ordine corretto.

**Esempio:** È possibile allegare un processo di approvazione allo stato del reparto marketing che richiede l&#39;approvazione del reparto finanziario. Poi, quando qualcuno cambia lo stato di un articolo di lavoro in &quot;Ufficio marketing&quot;, l&#39;articolo non può spostarsi in quel reparto fino a quando il reparto Finanza non si firma su di esso.

Per ulteriori informazioni sugli stati degli elementi di lavoro, vedere i seguenti articoli:

* [Accedere all’elenco degli stati del progetto di sistema](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md)
* [Accedere all&#39;elenco degli stati delle attività del sistema](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md)
* [Accedere all’elenco degli stati dei problemi del sistema](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md)

### Utilizzo di un processo di approvazione da parte di un flusso di lavoro tipico {#how-a-typical-workflow-uses-an-approval-process}

Lo scenario seguente illustra come un processo di approvazione consente agli utenti di approvare il lavoro mentre un oggetto Workfront avanza attraverso un flusso di lavoro di diversi passaggi in questo ordine:

1. L&#39;amministratore Workfront o un utente con accesso amministrativo ai processi di approvazione crea un processo di approvazione per un progetto, un&#39;attività o un problema.

   >[!NOTE]
   È possibile allegare i processi di approvazione dei progetti a un modello e i processi di approvazione delle attività a un&#39;attività modello. In questo modo, quando un utente utilizza il modello per creare un progetto, il processo di approvazione diventa rispettivamente un processo di approvazione del progetto o dell&#39;attività. Un processo di approvazione a uso singolo allegato a un modello o a un modello rimane un processo di approvazione a uso singolo per progetti e attività.

1. Un utente con l&#39;autorizzazione Gestisci per il progetto, l&#39;attività o il problema allega il processo di approvazione all&#39;elemento oppure crea un&#39;approvazione a uso singolo per l&#39;elemento.
1. Un utente assegnato all&#39;elemento di lavoro modifica il proprio stato con lo stato che avvia il processo di approvazione e inizia il processo di approvazione. (La persona che ha creato il processo di approvazione ha definito la relazione tra lo stato e il processo di approvazione.)
1. Gli approvatori designati ricevono una notifica sul processo di approvazione in sospeso e esaminano l&#39;elemento di lavoro.
1. Il processo di approvazione termina dopo che gli approvatori designati approvano tutte le fasi del processo. Oppure, se rifiutano un passaggio, lo stato viene reimpostato su uno stato predefinito o viene creato un problema. (La persona che ha creato il processo di approvazione ha definito quale di questi passaggi automatizzati avviene dopo un rifiuto.)

**Esempio:** Un team pubblicitario ha creato uno stato denominato Pronto per la stampa e un processo di approvazione denominato Designer/Copywriter Signoff associato a questo stato. Questo processo di approvazione è configurato per:

* Richiedi l&#39;approvazione del progettista e del copywriter del team
* Viene attivato ogni volta che un utente modifica lo stato di un elemento di lavoro in Pronto per la stampa

Il proprietario di un progetto di brochure allega al progetto di brochure il processo di approvazione di Designer/Copywriter Signoff.

Quando un utente del progetto modifica lo stato in Pronto per la stampa, il copywriter e il designer ricevono le notifiche che richiedono di approvarlo o rifiutarlo. Durante il processo di approvazione, quando si decide se approvarlo o meno, lo stato dei progetti viene visualizzato come Pronto per la stampa - In attesa di approvazione.

Dopo l’approvazione della brochure in Workfront, lo stato del progetto diventa Pronto per la stampa.

## Processi di approvazione dei documenti

Le approvazioni dei documenti sono utilizzate per un&#39;approvazione più generale. Il feedback viene acquisito in formato chat nella scheda Aggiornamenti. È possibile utilizzare i pulsanti di approvazione per approvare, rifiutare o approvare le modifiche.

Per aggiungere approvatori a un documento dopo averlo caricato in Workfront, consulta [Richiedere l&#39;approvazione del documento](../../review-and-approve-work/manage-approvals/request-document-approvals.md).

## Processi di approvazione della prova

Le approvazioni di prova vengono utilizzate per una revisione più approfondita e generalmente includono flussi di lavoro più complessi. Il feedback viene acquisito con strumenti di marcatura nel visualizzatore di correzione. È possibile utilizzare i pulsanti di approvazione per approvare, rifiutare o approvare le modifiche.

Per aggiungere un flusso di lavoro automatizzato a una bozza di documento e designare alcuni utenti nel flusso di lavoro come approvatori della bozza, vedi [Creare una bozza avanzata con un flusso di lavoro automatizzato](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

## Configurazione delle impostazioni per i processi di approvazione degli elementi di lavoro

In qualità di amministratore di Workfront, puoi configurare le impostazioni globali per i processi di approvazione degli elementi di lavoro nel sistema. Queste impostazioni determinano varie regole per i processi di approvazione, ad esempio per quanto tempo una decisione di approvazione deve rimanere aperta o come gestire la delega di approvazione nel sistema. Per ulteriori informazioni sulle impostazioni del processo di approvazione, vedi [Configurare le impostazioni di approvazione globali](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md).
