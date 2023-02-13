---
product-area: projects
navigation-topic: manage-issues
title: Creare problemi
description: Quando lavori a un progetto, potresti riscontrare che si verificano eventi imprevisti. È possibile registrare tali eventi imprevisti come problemi per un particolare progetto o attività. Gli utenti con accesso appropriato possono visualizzare e monitorare lo stato dei problemi man mano che il progetto o l’attività progrediscono fino al completamento, eliminando la necessità di lunghe catene di posta elettronica o riunioni di stato. A differenza delle attività, che sono eventi pianificati, i problemi rappresentano elementi di lavoro non pianificati in Adobe Workfront.
author: Alina
feature: Work Management
exl-id: 2a4488fb-fe2f-422a-887c-996f6367afc5
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1397'
ht-degree: 0%

---

# Creare problemi

Quando lavori a un progetto, potresti riscontrare che si verificano eventi imprevisti. È possibile registrare tali eventi imprevisti come problemi per un particolare progetto o attività. Gli utenti con accesso appropriato possono visualizzare e monitorare lo stato dei problemi man mano che il progetto o l’attività progrediscono fino al completamento, eliminando la necessità di lunghe catene di posta elettronica o riunioni di stato. A differenza delle attività, che sono eventi pianificati, i problemi rappresentano elementi di lavoro non pianificati in Adobe Workfront.

Puoi anche aggiungere problemi ai progetti come richieste. Per informazioni, consulta [Creare e inviare richieste Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

>[!TIP]
>
>I problemi e le richieste vengono utilizzati in modo intercambiabile in Workfront. È possibile registrare i problemi relativi a progetti e attività per indicare il lavoro imprevisto che deve essere affrontato. È inoltre possibile inviare richieste registrate come problemi in un progetto designato come coda di richiesta.

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
   <td> <p>Revisione o superiore per aggiungere problemi a un progetto o a un'attività</p> <p>Richiedi o una versione successiva per aggiungere problemi come richieste, utilizzando una coda richieste.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica accesso ai problemi</p> <p>Visualizza o consente un accesso più elevato a progetti e attività</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni sull'accesso ai problemi relativi al livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Concedere l’accesso ai problemi</a>. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Collaborare o autorizzazioni superiori con la possibilità di aggiungere problemi all'attività o al progetto in cui si crea il problema</p> <p> Per informazioni sulla concessione delle autorizzazioni per i problemi, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Condividere un problema </a></p> <p>Per informazioni sulla richiesta di autorizzazioni aggiuntive, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: in NWE Requestors CAN see the Issues tab on a project but in classic they cannot! However, even when they DO see it, they cannot enter the issues - logged this issue for it but they might decide not to fix it: https://hub.workfront.com/issue/60181e28000058980cce29597185b2d6/updates?email-source=comm)</p>
-->

## Limitazioni nella creazione dei problemi

Se disponi dell&#39;accesso e delle autorizzazioni corrette, puoi creare problemi su un progetto o un&#39;attività. Tuttavia, i seguenti casi non consentono di creare problemi:

* L’amministratore di Workfront o un amministratore di gruppo deve abilitare l’aggiunta di problemi a un progetto che si trova in uno stato Completo o Morto nell’area Preferenze progetto. Per informazioni sull&#39;impostazione delle preferenze del progetto, consulta [Configurare le preferenze del progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* Non è possibile aggiungere problemi a un progetto in sospeso.

## Preparare il modulo Nuovo problema

La tua organizzazione deve disporre di un processo ben definito per sapere quando e come registrare un problema. Quando configuri questo processo, il primo passo è quello di creare il modulo necessario per l’invio di un problema. Puoi definire quali campi Workfront e quali campi personalizzati sono disponibili per gli utenti quando inviano nuovi problemi e devono essere completati, sia che consentano di aggiungere direttamente i problemi alle attività e ai progetti o che siano presenti code di richiesta in cui vengono inviati i problemi. Il modulo Nuovo problema può contenere informazioni importanti utili per risolvere rapidamente il problema.

I campi per i nuovi problemi relativi a un progetto sono definiti nella sezione Dettagli coda del progetto in cui verranno registrati i problemi. Per informazioni sulla configurazione della sezione Dettagli coda del progetto, consulta [Creare una coda di richiesta](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Per informazioni sulla creazione dei problemi inviandoli a una coda di richiesta, vedi [Crea problemi inserendo una nuova richiesta](#create-issues-by-entering-a-new-request) in questo articolo.

## Creare problemi relativi a un&#39;attività o a un progetto utilizzando il pulsante Nuovo problema

Dopo aver definito i campi di un nuovo modulo per problemi nel progetto, puoi iniziare a creare problemi.

Per creare un problema su un&#39;attività o su un progetto:

1. Passa a un progetto in cui desideri creare il problema.
1. (Facoltativo) Se desideri segnalare il problema per un&#39;attività, vai alla **Attività** fare clic sul nome di un&#39;attività.
1. Fai clic sul pulsante **Problemi** sezione .

   ![](assets/qs-issues-icon-highlighted-on-project-350x216.png)

1. Fai clic su **Nuovo problema**.

   ![](assets/qs-issue-list-on-project-with-new-issue-button-highlighted-350x270.png)

1. (Condizionale) Se il creatore del progetto ha creato Argomenti coda o Gruppi di argomenti sul progetto, questi verranno aggiunti al nuovo modulo del problema. Specifica la **Gruppo argomenti** o **Argomento coda** del nuovo numero. Dovrebbero avere nomi personalizzati per il tuo ambiente.\
   Per ulteriori informazioni sulla creazione di gruppi di argomenti, consulta [Crea gruppi di argomenti](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md). Per ulteriori informazioni sulla creazione degli argomenti della coda, consulta [Crea argomenti coda](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

   ![](assets/new-issue-screen-when-creating-issue-from-list-project-level-nwe-350x422.png)

   * Se nel progetto è impostato un solo argomento della coda, questo viene visualizzato automaticamente.
   * Se il gruppo di argomenti non contiene argomenti o gruppi di argomenti della coda, non è disponibile nulla nel menu a discesa Gruppo di argomenti .

1. (Condizionale) Se il creatore del progetto ha consentito l’ **Tipo di problema** per visualizzare il modulo Nuovo problema, selezionare il tipo di problema tra le opzioni seguenti:

   * Segnalazione Bug
   * Richiesta di Modifica
   * Problema
   * Richiesta\
      A seconda di come l’amministratore di Workfront ha configurato le preferenze per i progetti, i nomi dei tipi di problema potrebbero essere diversi.

1. Specifica uno dei campi disponibili nella **Nuovo problema** modulo. Per ulteriori informazioni sulla definizione dei campi durante l’immissione di un nuovo problema, consulta [Modifica dei problemi](../../../manage-work/issues/manage-issues/edit-issues.md).
1. (Condizionale) Se gli argomenti della coda sono associati a un modulo personalizzato, questo verrà visualizzato nella **Nuovo problema** modulo.\
   Oppure\
   Se il progetto è associato a un modulo personalizzato per un problema tramite l’area Dettagli coda, il modulo viene visualizzato in **Nuovo problema** sotto i campi Workfront predefiniti.

   Per informazioni, consulta [Creare una coda di richiesta](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. Fai clic su **Salva nuovo problema.**

I problemi possono essere assegnati a più utenti, ruoli di lavoro o a un team. Per ulteriori informazioni sull’assegnazione e la gestione delle richieste, consulta [Gestione delle richieste di lavoro e team](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).

## Creare problemi su un&#39;attività o su un progetto in linea

>[!IMPORTANT]
>
>Il proprietario del progetto deve abilitare **Consenti agli utenti di aggiungere problemi in linea** quando definisci le impostazioni dei problemi per il progetto prima di poter aggiungere problemi in linea al progetto o alle attività. Per informazioni sulla configurazione delle impostazioni dei problemi in un progetto, consulta [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md).

Se desideri aggiungere rapidamente diversi problemi, puoi crearli per un’attività o un progetto in linea, aggiungendoli a un elenco di problemi.

>[!NOTE]
>
>Quando si aggiungono problemi in linea, Workfront non applica il modulo Nuovo problema ai nuovi problemi. Non consigliamo di aggiungere problemi in linea se desideri che gli utenti forniscano determinate informazioni quando immetti i problemi. Questo può avere un impatto negativo sulla generazione di rapporti sui problemi e in seguito sulla capacità dell’utente assegnato al problema di disporre di tutte le informazioni necessarie per risolvere il problema.

Per creare problemi in linea:

1. Passa a un progetto in cui desideri creare il problema.
1. (Facoltativo) Se desideri segnalare il problema per un&#39;attività, vai alla **Attività** fare clic sul nome di un&#39;attività.
1. Fai clic sul pulsante **Problemi** sezione .
1. Fai clic su **Aggiungi altri problemi**.

   Viene creata una nuova riga nell’elenco dei problemi nella sezione Problemi .

   >[!TIP]
   >
   >Questa opzione è disattivata se l’impostazione Consenti agli utenti di aggiungere problemi in linea è deselezionata nella casella Modifica progetto. Per informazioni, consulta [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md).

   ![](assets/add-more-issues-button-highlighted-issue-list-nwe-350x272.png)

1. Inizia a digitare il nome del problema nel campo Nome , quindi continua ad aggiungere ulteriori informazioni sul problema in linea.

   >[!TIP]
   >
   >I campi disponibili per la modifica in linea sono resi disponibili dalla visualizzazione applicata all’elenco dei problemi. Potrebbe non essere possibile modificare in linea il seguente tipo di campi:
   >   
   >* Campi appartenenti a un altro oggetto
   >* Campi per i quali non si dispone dell’accesso per la modifica
   >* Campi che sono calcoli e che vengono aggiornati automaticamente da Workfront


1. Fai clic su Invio per terminare la modifica in linea e aggiungere il problema al progetto o all’attività.

## Crea problemi inserendo una nuova richiesta {#create-issues-by-entering-a-new-request}

Puoi designare i progetti come destinatari dei problemi. Questo tipo di progetti si chiama Code di richieste in Workfront. Puoi accedere alle code di richieste tramite l’area Richieste nel menu principale.

>[!TIP]
>
>I termini &quot;problema&quot; e &quot;richiesta&quot; sono intercambiabili in Workfront.

Per ulteriori informazioni su come impostare progetti come Code di richieste per ricevere problemi, vedi [Creare una coda di richiesta](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md). Per informazioni sull&#39;invio delle richieste, vedi [Creare e inviare richieste Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).
