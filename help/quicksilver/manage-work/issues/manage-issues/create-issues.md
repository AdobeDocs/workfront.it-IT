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
source-git-commit: bdbb970aa0bb49fe9e69a15f93c96609eb2c1bfe
workflow-type: tm+mt
source-wordcount: '2035'
ht-degree: 0%

---

# Crea problemi

<!--remove Preview and Prod references when this comes to Prod-->

<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo i rilasci mensili in Produzione, le stesse funzioni sono disponibili nell’ambiente di Produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, consulta [Abilitare o disabilitare le versioni rapide per la tua organizzazione](../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

<span class="preview">Per informazioni sulla versione corrente, consulta [Panoramica sulla versione del quarto trimestre 2023](../../../product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md). </span>



Quando lavori a un progetto, potresti scoprire che si verificano eventi imprevisti. Puoi registrare tali eventi imprevisti come problemi per un particolare progetto o per un’attività. Gli utenti con l’accesso appropriato possono visualizzare e monitorare lo stato dei problemi man mano che il progetto o l’attività progredisce al completamento, eliminando la necessità di lunghe catene di e-mail o riunioni sullo stato. A differenza delle attività, che sono eventi pianificati, i problemi rappresentano elementi di lavoro non pianificati in Adobe Workfront.

Puoi anche aggiungere problemi ai progetti come richieste. Per informazioni, consulta [Creare e inviare richieste Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

>[!TIP]
>
>I problemi e le richieste vengono utilizzati in modo intercambiabile in Workfront. È possibile registrare problemi relativi a progetti e attività per indicare il lavoro imprevisto che deve essere risolto. Puoi anche inviare richieste registrate come problemi in un progetto designato come coda richieste.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Revisione o successiva per aggiungere problemi a un progetto o un'attività</p> <p>Richiesta o successiva per aggiungere problemi come richieste, utilizzando una coda di richieste.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modifica l'accesso alle Issues</p> <p>Accesso di visualizzazione o superiore ai progetti e alle attività</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni sull'accesso ai problemi nel proprio livello di accesso, vedere <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Concedere l’accesso ai problemi</a>. Per informazioni su come un amministratore di Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Autorizzazioni di Contribute o superiori con la possibilità di aggiungere problemi all’attività o al progetto in cui si crea il problema</p> <p> Per informazioni sulla concessione delle autorizzazioni per i problemi, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Condividere un problema </a></p> <p>Per informazioni sulla richiesta di autorizzazioni aggiuntive, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

<!--
(NOTE: in NWE Requestors CAN see the Issues tab on a project but in classic they cannot! However, even when they DO see it, they cannot enter the issues - logged this issue for it but they might decide not to fix it: https://hub.workfront.com/issue/60181e28000058980cce29597185b2d6/updates?email-source=comm)</p>
-->

## Limitazioni nella creazione dei problemi

Quando si dispone dell&#39;accesso e delle autorizzazioni corretti è possibile creare problemi in un progetto o in un&#39;attività. Tuttavia, di seguito sono riportati alcuni casi in cui potresti non essere in grado di creare problemi:

* L’amministratore di Workfront o un amministratore di gruppo deve abilitare l’aggiunta di problemi a un progetto che si trova nello stato Complete (Completato) o Dead (Inattivo) nell’area Project Preferences (Preferenze del progetto). Per informazioni sull&#39;impostazione delle preferenze di progetto, vedere [Configurare le preferenze di progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* Impossibile aggiungere problemi a un progetto in attesa di approvazione.

## Prepara il modulo per la nuova Issue

La tua organizzazione deve disporre di un processo ben definito per determinare quando e come registrare un problema. Quando si configura questo processo, il primo passaggio consiste nel creare il modulo necessario per l’invio di un problema. Se si consente l&#39;aggiunta diretta di problemi ad attività e progetti o se si dispone di code di richieste in cui vengono inviati problemi, è possibile definire quali campi di Workfront e quali campi personalizzati sono disponibili per gli utenti quando inviano nuovi problemi e devono essere completati. Il modulo Nuovo problema può contenere informazioni importanti che saranno utili per risolvere rapidamente il problema.

I campi per i nuovi problemi in un progetto sono definiti nella sezione Dettagli coda del progetto in cui verranno registrati i problemi. Per informazioni sulla configurazione della sezione Dettagli coda del progetto, consulta [Creare una coda di richieste](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Per informazioni sulla creazione di problemi inviandoli a una coda di richieste, vedi [Crea problemi immettendo una nuova richiesta](#create-issues-by-entering-a-new-request) in questo articolo.

## Creare problemi in un&#39;attività o in un progetto utilizzando il pulsante Nuovo problema

Dopo aver definito i campi di un nuovo modulo problema sul progetto, puoi iniziare a creare i problemi.

La creazione dei problemi varia a seconda dell’ambiente scelto per creare il problema.

### Creare problemi in un’attività o in un progetto utilizzando il pulsante Nuovo problema nell’ambiente di produzione

Per creare un problema su un’attività o un progetto:

1. Vai a un progetto in cui desideri creare il problema.
1. (Facoltativo) Se desideri segnalare il problema per un’attività, vai al **Attività** , quindi fare clic sul nome di un&#39;attività.
1. Fai clic su **Problemi** sezione.

   ![](assets/qs-issues-icon-highlighted-on-project-350x216.png)

1. Clic **Crea una Issue**.

   ![](assets/qs-issue-list-on-project-with-new-issue-button-highlighted-350x270.png)

1. (Condizionale) Se l’autore del progetto ha creato Argomenti coda o Gruppi di argomenti sul progetto, questi vengono aggiunti al modulo del nuovo problema. Specifica la **Gruppo di argomenti** o **Argomento Coda** del nuovo problema. I nomi dei gruppi di argomenti e degli argomenti della coda sono personalizzati in base all&#39;ambiente in uso.\
   Per ulteriori informazioni sulla creazione di gruppi di argomenti, vedere [Crea gruppi di argomenti](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md). Per ulteriori informazioni sulla creazione degli argomenti della coda, vedere [Crea argomenti coda](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

   ![](assets/new-issue-screen-when-creating-issue-from-list-project-level-nwe-350x422.png)

   * Se nel progetto è impostato un solo Argomento coda, viene visualizzato automaticamente.
   * Se il Gruppo di argomenti non contiene argomenti di coda o gruppi di argomenti, non è disponibile alcun elemento nel menu a discesa Gruppo di argomenti.

1. (Condizionale) Se l’autore del progetto consente il **Tipo di richiesta** da visualizzare nel modulo Nuovo problema, seleziona il tipo di problema tra le seguenti opzioni:

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


1. Aggiungi un nome per il nuovo problema nel **Nome problema** campo.
1. Continua a specificare i campi disponibili nel **Crea una Issue** modulo. Per ulteriori informazioni sui campi disponibili quando si immette un nuovo problema, vedere [Modifica problemi](../../../manage-work/issues/manage-issues/edit-issues.md).

   >[!IMPORTANT]
   >
   >Non tutti i campi relativi al problema sono disponibili nel modulo Nuovo problema. L’autore del progetto abilita i campi disponibili durante la creazione di un problema quando definiscono l’area Dettagli coda del progetto. Per ulteriori informazioni, consulta [Creare una coda di richieste](../../requests/create-and-manage-request-queues/create-request-queue.md).


1. (Condizionale) Se gli argomenti della coda sono associati a un modulo personalizzato, questo verrà visualizzato in **Crea una Issue** modulo.\
   Oppure\
   Se il progetto è associato a un modulo personalizzato relativo a un problema tramite l’area Dettagli coda, il modulo viene visualizzato in **Crea una Issue** modulo, dopo i campi predefiniti di Workfront.

   Per informazioni, consulta [Creare una coda di richieste](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. Clic **Salva nuovo problema.**

I problemi possono essere assegnati a più utenti, mansioni o a un team. Per ulteriori informazioni sull’assegnazione e la gestione delle richieste, consulta [Gestire le richieste di lavoro e team](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).

<!--When this is coming to Production, remove the "Production" section above and replace it with the following content: -->

<div class="preview">

### Creare problemi in un’attività o in un progetto utilizzando il pulsante Nuovo problema nell’ambiente di anteprima

Per creare un problema su un’attività o un progetto:

1. Vai a un progetto in cui desideri creare il problema.
1. (Facoltativo) Se desideri segnalare il problema per un’attività, vai al **Attività** , quindi fare clic sul nome di un&#39;attività.
1. Fai clic su **Problemi** sezione.

   ![](assets/qs-issues-icon-highlighted-on-project-350x216.png)

1. Clic **Crea una Issue**.
Viene visualizzata la casella Nuovo problema.

   ![](assets/new-issue-box-matches-new-request-ui.png)

1. (Condizionale) Se l’autore del progetto ha creato Argomenti coda o Gruppi di argomenti sul progetto, questi vengono aggiunti al modulo del nuovo problema. Specifica la **Gruppo di argomenti** o **Argomento Coda** del nuovo problema. I nomi dei gruppi di argomenti e degli argomenti della coda sono personalizzati in base all&#39;ambiente in uso.\
   Per ulteriori informazioni sulla creazione di gruppi di argomenti, vedere [Crea gruppi di argomenti](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md). Per ulteriori informazioni sulla creazione degli argomenti della coda, vedere [Crea argomenti coda](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

   * Se nel progetto è impostato un solo Argomento coda, viene visualizzato automaticamente.
   * Se il Gruppo di argomenti non contiene argomenti di coda o gruppi di argomenti, non è disponibile alcun elemento nel menu a discesa Gruppo di argomenti.

1. Aggiungi il nome del problema in **Oggetto** , quindi aggiungi un **Descrizione**.

1. (Condizionale) Se l’autore del progetto consente il **Tipo di richiesta** da visualizzare nel modulo Nuovo problema, seleziona il tipo di problema tra le seguenti opzioni:

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

1. Continua a specificare i campi disponibili nel **Nuovo problema** modulo. Per ulteriori informazioni sui campi disponibili quando si immette un nuovo problema, vedere [Modifica problemi](../../../manage-work/issues/manage-issues/edit-issues.md).

   >[!IMPORTANT]
   >
   >Non tutti i campi relativi al problema sono disponibili nel modulo Nuovo problema. L’autore del progetto abilita i campi disponibili durante la creazione di un problema quando definiscono l’area Dettagli coda del progetto. Per ulteriori informazioni, consulta [Creare una coda di richieste](../../requests/create-and-manage-request-queues/create-request-queue.md).


1. (Condizionale) Se gli argomenti della coda sono associati a un modulo personalizzato, questo verrà visualizzato in **Nuovo problema** modulo.\
   Oppure\
   Se il progetto è associato a un modulo personalizzato relativo a un problema tramite l’area Dettagli coda, il modulo viene visualizzato in **Nuovo problema** modulo, dopo i campi predefiniti di Workfront.

   Per informazioni, consulta [Creare una coda di richieste](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. Clic **Invia**.

   I problemi possono essere assegnati a più utenti, mansioni o a un team. Per ulteriori informazioni sull’assegnazione e la gestione delle richieste, consulta [Gestire le richieste di lavoro e team](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).

</div>

## Crea problemi in linea per un&#39;attività o un progetto

>[!IMPORTANT]
>
>Il proprietario del progetto deve abilitare **Consenti agli utenti di aggiungere problemi in linea** durante la definizione delle impostazioni dei problemi per il progetto, prima di poter aggiungere problemi in linea al progetto o alle attività. Per informazioni sulla configurazione delle impostazioni dei problemi in un progetto, vedi [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md).
>

Se desideri aggiungere rapidamente diversi problemi, puoi crearli per un’attività o un progetto in linea, aggiungendoli a un elenco di problemi.

>[!NOTE]
>
>Quando si aggiungono problemi in linea, Workfront non applica il modulo Nuovo problema ai nuovi problemi. Si sconsiglia di aggiungere problemi in linea se si desidera che gli utenti forniscano determinate informazioni durante l’inserimento dei problemi. Questo può avere un impatto negativo sulla segnalazione dei problemi e successivamente sulla capacità dell’utente assegnato al problema di disporre di tutte le informazioni necessarie per risolverlo.

Per creare problemi in linea:

1. Vai a un progetto in cui desideri creare il problema.
1. (Facoltativo) Se desideri segnalare il problema per un’attività, vai al **Attività** , quindi fare clic sul nome di un&#39;attività.
1. Fai clic su **Problemi** sezione.
1. Clic **Aggiungi altri problemi**.

   Viene creata una nuova riga nell’elenco dei problemi nella sezione Problemi.

   >[!TIP]
   >
   >Questa opzione è disabilitata se l’impostazione Consenti agli utenti di aggiungere problemi in linea è deselezionata nella casella Modifica progetto. Per informazioni, consulta [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md).

   ![](assets/add-more-issues-button-highlighted-issue-list-nwe-350x272.png)

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

Puoi designare i progetti come contenitori per la ricezione dei problemi. Questi tipi di progetti sono denominati Code di richieste in Workfront. Puoi accedere a Code di richieste tramite l’area Richieste nel menu principale.

>[!TIP]
>
>I termini &quot;problema&quot; e &quot;richiesta&quot; sono intercambiabili in Workfront.

Per ulteriori informazioni su come impostare i progetti come Code di richieste per la ricezione dei problemi, consulta [Creare una coda di richieste](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md). Per informazioni sull’invio delle richieste, consulta [Creare e inviare richieste Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).
