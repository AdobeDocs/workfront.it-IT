---
product-area: projects
navigation-topic: manage-issues
title: Crea problemi
description: Quando lavori a un progetto, potresti scoprire che si verificano eventi imprevisti. Puoi registrare tali eventi imprevisti come problemi per un particolare progetto o per un’attività. Gli utenti con l’accesso appropriato possono visualizzare e monitorare lo stato dei problemi man mano che il progetto o l’attività progredisce al completamento, eliminando la necessità di lunghe catene di e-mail o riunioni sullo stato. A differenza delle attività, che sono eventi pianificati, i problemi rappresentano elementi di lavoro non pianificati in Adobe Workfront.
author: Alina
feature: Work Management
topic: Collaboration
role: User
exl-id: 2a4488fb-fe2f-422a-887c-996f6367afc5
source-git-commit: 609396b2eb6413c8f6e84361757f00c2cc5e3ad6
workflow-type: tm+mt
source-wordcount: '1477'
ht-degree: 0%

---

# Crea problemi

<!--Audited: 03/2025-->

<!--

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span> 

<span class="preview">For information about the current release, see [Fourth Quarter 2023 release overview](../../../product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md). </span> 

-->

Quando lavori a un progetto, potresti scoprire che si verificano eventi imprevisti. Puoi registrare tali eventi imprevisti come problemi per un particolare progetto o per un’attività. Gli utenti con l’accesso appropriato possono visualizzare e monitorare lo stato dei problemi man mano che il progetto o l’attività progredisce al completamento, eliminando la necessità di lunghe catene di e-mail o riunioni sullo stato. A differenza delle attività, che sono eventi pianificati, i problemi rappresentano elementi di lavoro non pianificati in Adobe Workfront.

Puoi anche aggiungere problemi ai progetti come richieste. Per informazioni, consulta [Creare e inviare richieste Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

>[!TIP]
>
>I problemi e le richieste vengono utilizzati in modo intercambiabile in Workfront. È possibile registrare problemi relativi a progetti e attività per indicare il lavoro imprevisto che deve essere risolto. Puoi anche inviare richieste registrate come problemi in un progetto designato come coda richieste.

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
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Nuova licenza:</p>
   <ul><li>Collaboratore o versione successiva</li>
   <li>Chiaro o superiore per modificare i problemi nella sezione Problemi di un’attività o di un progetto</li></ul>
   <p>Licenza corrente:</p>
  <ul><li>Richiedi o superiore</li> <li>Revisione o successiva per modificare i problemi nella sezione Problemi di un'attività o di un progetto</li></ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica l'accesso alle Issues</p> <p>Accesso di visualizzazione o superiore ai progetti e alle attività</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Autorizzazioni di Contribute o superiori con la possibilità di aggiungere problemi all’attività o al progetto in cui si crea il problema</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
(NOTE: in NWE Requestors CAN see the Issues tab on a project but in classic they cannot! However, even when they DO see it, they cannot enter the issues - logged this issue for it but they might decide not to fix it: https://hub.workfront.com/issue/60181e28000058980cce29597185b2d6/updates?email-source=comm)</p>
-->

## Limitazioni nella creazione dei problemi

Quando si dispone dell&#39;accesso e delle autorizzazioni corretti è possibile creare problemi in un progetto o in un&#39;attività. Tuttavia, di seguito sono riportati alcuni casi in cui potresti non essere in grado di creare problemi:

* L’amministratore di Workfront o un amministratore di gruppo deve abilitare l’aggiunta di problemi a un progetto che si trova nello stato Complete (Completato) o Dead (Inattivo) nell’area Project Preferences (Preferenze del progetto). Per informazioni sull&#39;impostazione delle preferenze di progetto, vedere [Configurare le preferenze di progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* Impossibile aggiungere problemi a un progetto in attesa di approvazione.

## Prepara il modulo per la nuova Issue

La tua organizzazione deve disporre di un processo ben definito per determinare quando e come registrare un problema. Quando si configura questo processo, il primo passaggio consiste nel creare il modulo necessario per l’invio di un problema.

Gli utenti possono aggiungere problemi a un progetto nei modi seguenti:

* Aggiungerli direttamente ad attività e progetti.
* Inviali a una coda di richieste.

Il modulo Nuovo problema può contenere informazioni importanti che saranno utili per risolvere rapidamente il problema.

È possibile configurare il modulo Nuovo problema in modo da includere le informazioni seguenti quando gli utenti aggiungono problemi al progetto o alle relative attività:

* Campi personalizzati
* Approvazioni
* Assegnazioni (Regole di Instradamento)

I campi per i nuovi problemi o richieste sono definiti nella sezione Dettagli coda del progetto in cui verranno registrati i problemi.

Per informazioni sulla configurazione della sezione Dettagli coda del progetto, vedere [Creare una coda di richieste](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Per informazioni sulla creazione di problemi inviandoli a una coda di richieste, vedere la sezione [Creare problemi immettendo una nuova richiesta](#create-issues-by-entering-a-new-request) in questo articolo.

## Creare problemi in un&#39;attività o in un progetto utilizzando il pulsante Nuovo problema

Dopo aver definito i campi di un nuovo modulo problema sul progetto, puoi iniziare a creare i problemi.

Per creare un problema su un’attività o un progetto:

1. Vai a un progetto in cui desideri creare il problema.
1. (Facoltativo) Se vuoi segnalare il problema per un&#39;attività, vai all&#39;area **Attività**, quindi fai clic sul nome di un&#39;attività.
1. Fai clic sulla sezione **Issues**.

   Viene visualizzato l’elenco dei problemi del progetto

1. Fai clic su **Nuovo problema** in alto nell&#39;elenco dei problemi.
Viene visualizzata la casella Nuovo problema.

   ![Casella nuovo problema](assets/new-issue-box-matches-new-request-ui.png)

1. (Condizionale) Se l’autore del progetto ha creato Argomenti coda o Gruppi di argomenti sul progetto, questi vengono aggiunti al modulo del nuovo problema. Specifica il **Gruppo di argomenti** o il **Argomento coda** del nuovo problema. I nomi dei gruppi di argomenti e degli argomenti della coda sono personalizzati in base all&#39;ambiente in uso.\
   Per ulteriori informazioni sulla creazione di gruppi di argomenti, vedere [Creare gruppi di argomenti](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md). Per ulteriori informazioni sulla creazione degli argomenti della coda, vedere [Creare argomenti della coda](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

   * Se nel progetto è impostato un solo Argomento coda, viene visualizzato automaticamente.
   * Se il Gruppo di argomenti non contiene argomenti di coda o gruppi di argomenti, non è disponibile alcun elemento nel menu a discesa Gruppo di argomenti.

1. Aggiungi il nome del problema nel campo **Oggetto**, quindi aggiungi una **Descrizione**.

1. (Condizionale) Se il creatore del progetto ha consentito la visualizzazione del campo **Tipo di richiesta** nel modulo Nuovo problema, seleziona il tipo di problema tra le seguenti opzioni:

   * Segnalazione Bug
   * Richiesta di Modifica
   * Problema
   * Richiesta\
     A seconda di come l’amministratore di Workfront ha configurato le preferenze del progetto, i nomi dei tipi di problema potrebbero essere diversi per te.

   >[!TIP]
   >
   >I Tipi di richiesta devono essere abilitati nella sezione Dettagli coda e anche durante la creazione dell’Argomento coda per essere visualizzati come selezione nel modulo Nuovo problema. Per informazioni, vedere i seguenti articoli:
   >* [Creare una coda di richieste](../../requests/create-and-manage-request-queues/create-request-queue.md)
   >  * [Crea argomenti coda](../../requests/create-and-manage-request-queues/create-queue-topics.md)

1. Continua a specificare i campi disponibili nel modulo **Nuovo problema**. Per ulteriori informazioni sui campi disponibili quando si immette un nuovo problema, vedere [Modifica problemi](../../../manage-work/issues/manage-issues/edit-issues.md).

   >[!IMPORTANT]
   >
   >Non tutti i campi relativi al problema sono disponibili nel modulo Nuovo problema. L’autore del progetto abilita i campi disponibili durante la creazione di un problema quando definiscono l’area Dettagli coda del progetto. Per ulteriori informazioni, vedere [Creare una coda di richieste](../../requests/create-and-manage-request-queues/create-request-queue.md).


1. (Condizionale) Se gli argomenti della coda sono associati a un modulo personalizzato, questo verrà visualizzato nel modulo **Nuovo problema**.\
   Oppure\
   Se il progetto è associato a un modulo personalizzato relativo a un problema tramite l&#39;area Dettagli coda, il modulo verrà visualizzato nel modulo **Nuovo problema**, dopo i campi predefiniti di Workfront.

   Per informazioni, vedere [Creare una coda di richieste](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. Fai clic su **Invia**.

   I problemi possono essere assegnati a più utenti, mansioni o a un team. Per ulteriori informazioni sull&#39;assegnazione e la gestione delle richieste, vedere [Gestire le richieste di lavoro e team](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).


## Crea problemi in linea per un&#39;attività o un progetto

>[!IMPORTANT]
>
>Il proprietario del progetto deve abilitare **Consenti agli utenti di aggiungere problemi in linea** durante la definizione delle impostazioni dei problemi per il progetto prima di poter aggiungere problemi in linea al progetto o alle attività. Per informazioni sulla configurazione delle impostazioni dei problemi in un progetto, vedi [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md).
>

Se desideri aggiungere rapidamente diversi problemi, puoi crearli per un’attività o un progetto in linea, aggiungendoli a un elenco di problemi.

>[!NOTE]
>
>Quando si aggiungono problemi in linea, Workfront non applica il modulo Nuovo problema ai nuovi problemi. Si sconsiglia di aggiungere problemi in linea se si desidera che gli utenti forniscano determinate informazioni durante l’inserimento dei problemi. Questo può avere un impatto negativo sulla segnalazione dei problemi e successivamente sulla capacità dell’utente assegnato al problema di disporre di tutte le informazioni necessarie per risolverlo.

Per creare problemi in linea:

1. Vai a un progetto in cui desideri creare il problema.
1. (Facoltativo) Se desideri segnalare il problema per un&#39;attività, passa alla sezione **Attività**, quindi fai clic sul nome di un&#39;attività.
1. Fai clic sulla sezione **Issues** nel pannello a sinistra.
1. Fai clic su **Aggiungi altri problemi** in fondo all&#39;elenco dei problemi.

   Viene creata una nuova riga nell’elenco dei problemi nella sezione Problemi.

   >[!TIP]
   >
   >Questa opzione è disabilitata se l’impostazione Consenti agli utenti di aggiungere problemi in linea è deselezionata nella casella Modifica progetto. Per informazioni, vedere [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md).

   ![Pulsante Aggiungi altri problemi](assets/add-more-issues-button-highlighted-issue-list-nwe-350x272.png)

1. Inizia a digitare il nome del problema nel campo Nome, quindi continua ad aggiungere ulteriori informazioni sul problema in linea.

   >[!TIP]
   >
   >I campi disponibili per la modifica in linea sono resi disponibili dalla vista applicata all’elenco dei problemi. Potresti non essere in grado di modificare in linea il seguente tipo di campi:
   >   
   >* Campi che appartengono a un altro oggetto
   >* Campi che non si dispone dell&#39;accesso per la modifica
   >* Campi che sono calcoli e che vengono aggiornati automaticamente da Workfront

1. Fai clic su Invio per terminare la modifica in linea e aggiungere il problema al progetto o all’attività.

## Crea problemi immettendo una nuova richiesta {#create-issues-by-entering-a-new-request}

Puoi designare i progetti come contenitori per la ricezione dei problemi. Questi tipi di progetti sono denominati Code di richieste in Workfront. È possibile accedere alle code di richieste dall&#39;area Richieste nel menu principale.

>[!TIP]
>
>I termini &quot;problema&quot; e &quot;richiesta&quot; sono intercambiabili in Workfront.

Per ulteriori informazioni su come impostare i progetti come Code di richieste per la ricezione di problemi, vedere [Creare una coda di richieste](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md). Per informazioni sull&#39;invio di richieste, vedere [Creare e inviare richieste Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).
