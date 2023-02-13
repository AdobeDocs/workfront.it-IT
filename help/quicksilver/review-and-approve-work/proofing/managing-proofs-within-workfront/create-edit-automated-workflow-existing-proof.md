---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Creare o modificare un flusso di lavoro automatizzato per una bozza esistente
description: I flussi di lavoro automatizzati semplificano la gestione del processo di revisione se il processo è complesso o se invii regolarmente contenuti da rivedere agli stessi gruppi di persone. Quando crei una bozza con un flusso di lavoro automatizzato, la bozza viene spostata da un passaggio all’altro fino all’approvazione finale. I partecipanti ricevono una notifica quando è il loro turno di rivedere il documento.
author: Courtney
feature: Digital Content and Documents
exl-id: 852f960f-1b57-4a8a-a928-407ad52418e6
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '1225'
ht-degree: 1%

---

# Creare o modificare un flusso di lavoro automatizzato per una bozza esistente

I flussi di lavoro automatizzati semplificano la gestione del processo di revisione se il processo è complesso o se invii regolarmente contenuti da rivedere agli stessi gruppi di persone. Quando crei una bozza con un flusso di lavoro automatizzato, la bozza viene spostata da un passaggio all’altro fino all’approvazione finale. I partecipanti ricevono una notifica quando è il loro turno di rivedere il documento.

Per informazioni sulla creazione di un flusso di lavoro automatizzato per una nuova bozza, consulta [Creare una bozza avanzata con un flusso di lavoro automatizzato](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Piano attuale: Pro o superiore</p> <p>oppure</p> <p>Piano legacy: Premium</p> <p>Per ulteriori informazioni sulla verifica dell’accesso con i diversi piani, consulta <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accesso alle funzionalità di correzione in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano attuale: Lavoro o piano</p> <p>Piano legacy: Qualsiasi (è necessario che la correzione sia attivata per l’utente)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Profilo autorizzazione bozza </td> 
   <td>Manager o superiore</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica accesso ai documenti</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il ruolo o il profilo delle autorizzazioni di prova, contattare l&#39;amministratore Workfront o Workfront Proof.

## Crea o modifica un flusso di lavoro automatizzato per una bozza esistente:

1. Passa il puntatore del mouse sul documento nell&#39;area Documenti, quindi fai clic su Flusso di lavoro di correzione.

   Oppure

   Se rivedi la bozza nel visualizzatore di correzione, fai clic su **Flusso di lavoro** ![](assets/workflow-icon-proofing-viewer.png) nel pannello a sinistra, fai clic sull’icona Modifica ![](assets/edit-icon-proofing-viewer.png) per aprire le impostazioni del flusso di lavoro automatizzato per la bozza.

1. (Condizionale) Se la bozza al momento utilizza un flusso di lavoro di base (senza aree di visualizzazione), fai clic su **Converti in flusso di lavoro automatizzato** nella schermata visualizzata.

   >[!NOTE]
   >
   >Non puoi modificare il primo passaggio quando effettui la conversione da un flusso di lavoro di base a un flusso di lavoro automatizzato, ma puoi aggiungere e configurare nuovi passaggi.

1. Condizionale) Per utilizzare un modello di flusso di lavoro automatizzato creato e condiviso dall’amministratore Adobe Workfront, fai clic su **Aggiungi modello**, seleziona il modello nella casella visualizzata, quindi fai clic su **Aggiungi modello**.

   Per ulteriori informazioni, consulta [Utilizzo dei modelli di flusso di lavoro automatizzati](#about-using-automated-workflow-templates) in questo articolo.

1. Aggiungi uno stadio al flusso di lavoro automatizzato:

   1. Fai clic su **Nuovo stadio** nell&#39;angolo in alto a destra.
   1. Nella casella visualizzata, digita un **Nome** per il palco.
   1. (Facoltativo) Imposta una scadenza per l’area di visualizzazione.
   1. In **Attiva fase** scegliete come attivare l’area di visualizzazione:


      <table>
      <tbody>
      <tr>
      <td><strong>Creazione a prova di</strong></td>
      <td>L’area di visualizzazione diventa attiva automaticamente perché la bozza è già stata creata.</td>
      </tr>
      <tr>
      <td><strong>Quando la scadenza della fase precedente viene superata</strong></td>
      <td>Fai clic sull’area di visualizzazione precedente nel <strong>Stadio principale</strong> elenco a discesa .</td>
      </tr>
      <tr>
      <td><strong>In una data e un’ora specifiche</strong></td>
      <td>Fai clic sul pulsante <strong>On</strong> per selezionare la data, quindi fare clic sulla casella a destra per selezionare l'ora.</td>
      </tr>
      <tr>
      <td><strong>Tutte le decisioni vengono approvate o approvate con modifiche sullo stadio padre</strong></td>
      <td>Fai clic sull’area di visualizzazione principale <strong>Stadio principale</strong> elenco a discesa.</td>
      </tr>
      <tr>
      <td><strong>Tutte le decisioni sono approvate sullo stadio padre</strong></td>
      <td>Fai clic sull’area di visualizzazione principale <strong>Stadio principale</strong> elenco a discesa.</td>
      </tr>
      <tr>
      <td><strong>Tutte le decisioni sono prese</strong></td>
      <td>Fai clic sull’area di visualizzazione principale <strong>Stadio principale</strong> elenco a discesa.</td>
      </tr>
      </tbody>
      </table>


   1. Immetti un nome di contatto o un indirizzo e-mail e configura le impostazioni per i revisori per l’area di visualizzazione.

      Per informazioni sull&#39;aggiunta dei revisori, consulta [Informazioni sull’aggiunta di revisori a un passaggio](#about-adding-reviewers-to-a-stage) in questo articolo.

   1. Utilizza una delle opzioni seguenti per configurare ulteriormente l’area di visualizzazione:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader"><strong>Opzioni scadenza</strong> </td>
         <td><p>Per impostare una scadenza per l’area di visualizzazione, fai clic su un’opzione nel <strong>Opzioni della scadenza</strong> elenco a discesa. Quindi, sotto <strong>Termine</strong>, effettua una delle seguenti operazioni:</p>
          <ul>
           <li>Se hai scelto <strong>Imposta data specifica</strong>: Seleziona la data e l’ora di scadenza desiderate.</li>
           <li>Se hai scelto <strong>Calcola dalla data di attivazione dell’area di visualizzazione</strong>: Selezionare il numero di giorni lavorativi che si desidera aggiungere alla data di attivazione dell’area di visualizzazione per determinare la scadenza.</li>
          </ul></td>
        </tr>
        <tr>
         <td role="rowheader">Blocca fase</td>
         <td>Specificare quando è possibile bloccare l'area di visualizzazione. </td>
        </tr>
        <tr>
         <td role="rowheader">Principale responsabile delle decisioni</td>
         <td><p>Seleziona il decision maker principale nell’area di visualizzazione (disponibile solo dopo l’aggiunta di almeno una persona allo stadio con un ruolo di approvatore o superiore). Se selezioni un modulo decisionale principale, la <strong>È necessaria una sola decisione</strong> in questo passaggio l’opzione è disabilitata.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Occorre solo una decisione</td>
         <td>Termina l'intero processo di revisione quando uno dei decisori prende una decisione.<p>Questa opzione non è disponibile se hai designato un utente nel <strong>Decisore principale</strong> menu a discesa.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Stage privato</td>
         <td>Consente solo alle persone seguenti di visualizzare i commenti e le decisioni prese durante questa fase: Supervisori, amministratori di Adobe Workfront e amministratori di Workfront Proof</td>
        </tr>
        <tr>
         <td role="rowheader">Informa le persone tramite e-mail</td>
         <td>Avvisi ai revisori con una notifica e-mail quando tocca loro lavorare sulla bozza.</td>
        </tr>
       </tbody>
      </table>

   1. Fai clic su **Aggiungi fase**.

1. Ripeti il passaggio precedente in base alle esigenze per aggiungere altri stadi.

   Quando si aggiungono aree di visualizzazione al flusso di lavoro automatizzato, sullo schermo viene visualizzato un diagramma che le rappresenta:

   ![](assets/workflow-diagram-existing-proof-qs-350x215.png)

1. Al termine dell’aggiunta delle aree di visualizzazione, fai clic su **Fine**.

## Utilizzo dei modelli di flusso di lavoro automatizzati {#about-using-automated-workflow-templates}

Quando utilizzi un modello di flusso di lavoro automatizzato, considera quanto segue:

1. Le impostazioni di un modello di flusso di lavoro automatizzato determinano le operazioni che è possibile eseguire con il flusso di lavoro automatico per una bozza. Ad esempio, se il pulsante Aggiungi un passaggio è disabilitato nel modello, questo non è visibile perché lavori con le impostazioni del flusso di lavoro automatizzato per la bozza.
1. Quando una persona viene aggiunta a una pagina in un modello di flusso di lavoro automatizzato, ma è già presente come revisore sulla bozza, l’applicazione del modello rimuove il revisore dal passaggio. Se non aggiungi un altro revisore all’area di visualizzazione, viene visualizzato un messaggio per richiedere di aggiungerne uno.
1. La possibilità di modificare un modello di flusso di lavoro automatizzato dipende dalle impostazioni del modello configurate dall’amministratore di Workfront, come descritto in . Se la possibilità di modificare il modello è disabilitata, solo il proprietario del modello può modificarlo.

## Informazioni sull’aggiunta di revisori a un passaggio {#about-adding-reviewers-to-a-stage}

Quando aggiungi revisori a un&#39;area di visualizzazione, considera quanto segue:

* Dopo aver aggiunto un utente a un passaggio, puoi configurare le impostazioni per tale utente sulla bozza, ad esempio il ruolo di bozza e le autorizzazioni aggiuntive che dovrebbe disporre e il tipo di avvisi e-mail che riceverà quando gli utenti formulano commenti e decisioni sulla bozza.
* Puoi trascinare uno o più utenti da un passaggio all’altro. Puoi trascinare gli utenti direttamente su un altro passaggio, oppure puoi trascinare gli utenti su un altro passaggio **Fasi** diagramma. Per selezionare più utenti, premere Maiusc+Ctrl (su Windows) o Maiusc+Comando (su Mac).
* È possibile aggiungere un revisore a una bozza una sola volta, il che significa che non è possibile aggiungere la stessa persona a più di una fase della bozza.
* I revisori che non vengono aggiunti a uno stadio privato non possono vedere tale stadio sulla prova o sui commenti fatti in tale fase.
* Per impostazione predefinita, l’aggiunta di un utente a un’area di visualizzazione consente all’utente di accedere alla bozza dal momento in cui viene creata.

   L’amministratore di Workfront può impedire agli utenti di accedere alla bozza finché il flusso di lavoro non entra nell’area in cui è stato aggiunto l’utente. Per ulteriori informazioni, consulta in .
