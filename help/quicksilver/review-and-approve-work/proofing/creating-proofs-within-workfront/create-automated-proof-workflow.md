---
product-area: documents;setup
navigation-topic: create-proofs-within-workfront
title: Creare una bozza avanzata con un flusso di lavoro automatizzato
description: Un flusso di lavoro automatizzato semplifica la gestione del processo di revisione se il processo è complesso o se invii regolarmente contenuti per la revisione agli stessi utenti. La bozza si sposta da un ambiente di staging all’altro e Adobe Workfront notifica a ogni utente quando è il momento di rivederla. Per ulteriori informazioni sui flussi di lavoro automatizzati, consulta Panoramica sui flussi di lavoro automatizzati.
author: Courtney
feature: Digital Content and Documents
exl-id: 977fe1bc-458f-4301-8056-dc51c61edb6c
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '1838'
ht-degree: 0%

---

# Creare una bozza avanzata con un flusso di lavoro automatizzato

<!-- Audited: 2/2024 -->

Un flusso di lavoro automatizzato semplifica la gestione del processo di revisione se il processo è complesso o se invii regolarmente contenuti per la revisione agli stessi utenti. La bozza si sposta da un ambiente di staging all’altro e Adobe Workfront notifica a ogni utente quando è il momento di rivederla. Per ulteriori informazioni sui flussi di lavoro automatizzati, vedere [Panoramica sui flussi di lavoro automatizzati](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> <p>Nuovo: Qualsiasi</p><p>Piano corrente: Pro o superiore</p><p>Piano legacy: Seleziona o superiore</p> <p>Per ulteriori informazioni sulla verifica dell'accesso con i diversi piani, vedere <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accesso alla funzionalità di verifica in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> <p>Nuovo: Standard</p><p>Piano corrente: Lavoro o Piano</p> <p>Piano legacy: qualsiasi (per l’utente deve essere abilitata la verifica)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Profilo autorizzazione bozza </td> 
   <td>Manager o superiore</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica accesso ai documenti</p></td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creare una bozza avanzata con un flusso di lavoro automatizzato

1. Vai al progetto, all&#39;attività o al problema in cui desideri la bozza, quindi fai clic sulla scheda **Documenti**.
1. Fai clic su **Aggiungi nuovo** > Bozza, carica il contenuto, quindi individua le sezioni elencate di seguito.

   oppure

   Passa il puntatore del mouse su un documento esistente, quindi fai clic su **Crea bozza** > **Bozza avanzata** e utilizza le sezioni elencate di seguito.

## Configurare le fasi della bozza

1. Nella sezione Tipo di flusso di lavoro scegliere **Automatizzato**.
1. (Facoltativo) Se desideri utilizzare un modello di flusso di lavoro automatico creato e condiviso con te dall&#39;amministratore di Workfront, fai clic su **Aggiungi modello**, seleziona il modello nella casella visualizzata, quindi fai clic su **Aggiungi modello**.

   >[!NOTE]
   >
   >Quando si utilizza un modello di flusso di lavoro automatizzato, tenere presente quanto segue:
   >   
   >* Le impostazioni di un modello di flusso di lavoro automatico determinano le operazioni che è possibile eseguire con il flusso di lavoro automatico per una bozza. Ad esempio, se il pulsante Aggiungi un’area di visualizzazione è disabilitato nel modello, non sarà visibile durante l’utilizzo delle impostazioni del flusso di lavoro automatico per la bozza.
   >* Quando una persona viene aggiunta a un’area di un modello di flusso di lavoro automatico, ma è anche già presente come revisore sulla bozza, l’applicazione del modello rimuove il revisore dall’area di visualizzazione. Se non si aggiunge un altro revisore all&#39;area di visualizzazione, verrà visualizzato un messaggio che richiede di aggiungerne uno.
   >* La possibilità di modificare un modello di flusso di lavoro automatico dipende dalle impostazioni del modello configurate dall&#39;amministratore di Workfront, come descritto in . Se la possibilità di modificare il modello è disabilitata, solo il proprietario del modello può modificarlo.

1. Configura la prima fase del flusso di lavoro automatizzato:

   1. (Facoltativo) Se si desidera creare un nome per la prima fase, fare clic su **Fase 1**, quindi digitare il nome.
   1. Nella sezione **Destinatari** per l&#39;area di visualizzazione aggiungere i revisori all&#39;area di visualizzazione.

      >[!NOTE]
      >
      >Quando si aggiungono revisori a una fase, tenere presente quanto segue:
      >   
      >* Puoi aggiungere utenti esterni a una fase con un indirizzo e-mail.
      >* Dopo aver aggiunto un utente a un’area di visualizzazione, puoi configurare le impostazioni per tale utente nella bozza.
      >* Puoi trascinare gli utenti direttamente in un&#39;altra fase, oppure puoi trascinare gli utenti in una fase del diagramma **Fasi**. Per selezionare più utenti, premere MAIUSC+Ctrl (su Windows) o MAIUSC+Comando (su Mac).
      >* È possibile aggiungere un revisore a una bozza una sola volta, il che significa che non è possibile aggiungere la stessa persona a più fasi della bozza.
      >* I revisori che non vengono aggiunti a una fase privata non possono vedere tale fase sulla bozza o sui commenti fatti in quella fase.
      >* Per impostazione predefinita, l’aggiunta di un utente a una fase consente a tale utente di accedere alla visualizzazione della bozza dal momento in cui viene creata. L’amministratore di Workfront può impedire agli utenti di accedere alla bozza fino a quando il flusso di lavoro non entra nella fase in cui l’utente è stato aggiunto.

   1. Fare clic su **Impostazioni fase**.
   1. Fare clic su un&#39;opzione **Attiva fase** per indicare come si desidera attivare la fase.

      Per la prima fase è possibile selezionare solo **Alla creazione della bozza**, **A una data e un&#39;ora specifiche** o **Manualmente**.

   1. (Condizionale) Se hai selezionato **In una data e un&#39;ora specifiche** nel passaggio precedente, seleziona la data e l&#39;ora in cui desideri attivare la fase nella casella **Attiva il** visualizzata.

   1. Utilizza una delle opzioni seguenti per configurare ulteriormente la fase.

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">Imposta scadenza fase</td>
         <td><p>Per impostare una scadenza per la fase, fare clic su un'opzione nell'elenco a discesa <strong>Opzioni scadenza</strong>. Quindi, in <strong>Scadenza</strong>, eseguire una delle operazioni seguenti:</p>
          <ul>
           <li>Se si sceglie <strong>Imposta data specifica</strong>: selezionare la data e l'ora di scadenza desiderate.</li>
           <li>Se si sceglie <strong>Calcola dalla data di attivazione della fase</strong>: selezionare il numero di giorni lavorativi che si desidera aggiungere alla data di attivazione della fase per determinare la scadenza.</li>
          </ul></td>
        </tr>
        <tr>
         <td role="rowheader">Fase di blocco</td>
         <td>Specificare quando è possibile bloccare lo stage. </td>
        </tr>
        <tr>
         <td role="rowheader">Trasferisci i diritti di decisione primari a</td>
         <td><p>Selezionare il decisore principale sullo stadio (disponibile solo dopo aver aggiunto almeno una persona allo stadio con il ruolo di Approvatore di bozza o superiore). Se si seleziona un decisore principale, l'opzione <strong>È richiesta una sola decisione</strong> è disabilitata in questa fase.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Richiedi una sola decisione per questa fase</td>
         <td>Termina l’intero processo di revisione quando uno dei responsabili decisionali prende una decisione.<p>Questa opzione non è disponibile se hai designato un utente nel menu a discesa <strong>Principale responsabile delle decisioni</strong>.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Rendi privata questa fase</td>
         <td>Consente solo alle persone seguenti di visualizzare i commenti e le decisioni prese durante questa fase: supervisori, amministratori Workfront e amministratori Workfront Proof</td>
        </tr>
       </tbody>
      </table>

1. Per aggiungere e configurare un&#39;altra fase:

   1. Fare clic su **Nuova fase**.
   1. (Facoltativo) Se si desidera creare un nome per la prima fase, fare clic su **Fase 2** (o **Fase 3**, **Fase 4** e così via), quindi digitare il nome.

   1. Fare clic su **Attiva fase**, quindi selezionare un&#39;opzione per specificare se la fase viene attivata automaticamente o manualmente.

      Oltre alle opzioni **Durante la creazione della bozza**, **In una data e un&#39;ora specifiche** o **Manualmente**, puoi selezionare un&#39;opzione che dipende da ciò che si è verificato nel passaggio precedente:

      ![Attiva opzioni fase](assets/activate-stage-options-for-stage-2-plus-350x177.png)

   1. Se è stata selezionata un&#39;opzione Attiva fase che dipende da quanto si è verificato nel passaggio precedente, utilizzare le opzioni visualizzate per configurare l&#39;impostazione di attivazione.

      Ad esempio, se hai selezionato **Quando lo stato della fase precedente cambia**, seleziona **Fase precedente**, quindi seleziona lo stato nella casella **Stato modificato in**.

1. Ripetere il passaggio precedente in base alle esigenze per aggiungere altre fasi.

   Quando aggiungi fasi al flusso di lavoro automatico, sullo schermo viene visualizzato un diagramma che le rappresenta:

   ![Diagramma fasi](assets/stages-diagram-350x213.png)

1. Continua con [Configurare le impostazioni e-mail per la bozza](#configure-email-settings-for-the-proof) di seguito.

## Configurare le impostazioni e-mail per la bozza {#configure-email-settings-for-the-proof}

1. Nella sezione **Notifica e-mail**, seleziona se inviare notifiche e-mail e un messaggio personalizzato agli utenti selezionati in [Crea una bozza avanzata con un flusso di lavoro automatizzato](#workflow) in precedenza in questo articolo:

   <table>
      <tbody>
      <tr>
      <td>Notifica i destinatari relativamente a questa bozza</td>
      <td>Seleziona questa opzione per inviare una notifica e-mail agli utenti. Quando nella sezione <strong>Flusso di lavoro</strong> è selezionata la condivisione di base</strong>, al momento della creazione della bozza viene inviata una notifica e-mail. <strong> Quando <strong>Flusso di lavoro automatico</strong> è selezionato nella sezione <strong>Flusso di lavoro</strong>, viene inviata una notifica e-mail quando la bozza entra nella fase del Flusso di lavoro automatico a cui è associato l'utente.</td>
      </tr>
      <tr>
      <td>Aggiungi messaggio personalizzato</td>
      <td>Seleziona questa opzione per includere un messaggio personalizzato nella notifica. È possibile specificare un oggetto e il corpo del messaggio. Il corpo del messaggio può includere formattazione RTF, ad esempio grassetto, punti elenco e collegamenti ipertestuali.</td>
      </tr>
      </tbody>
      </table>


1. Continua con [Configura impostazioni bozza](#configure-proof-settings) di seguito.

## Configura impostazioni bozza {#configure-proof-settings}

1. Nella sezione **Impostazioni bozza**, selezionare una delle opzioni seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Accesso necessario: la bozza può essere condivisa solo con altri utenti</td> 
      <td>Quando questa opzione è disabilitata (impostazione predefinita), chiunque disponga dell’URL può visualizzare la bozza. <br>Quando questa opzione è selezionata:
       <ul>
        <li>Solo gli utenti di Workfront Proof possono visualizzare la bozza.</li>
        <li>Gli utenti non possono accedere alla bozza a meno che non siano stati aggiunti alla bozza.</li>
        <li>Le sottoscrizioni non possono essere abilitate.</li>
       </ul></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Per questa bozza è necessaria una sola decisione</td> 
      <td>Quando questa opzione è selezionata, la revisione viene completata dopo che un decisore prende la sua decisione.<br>Questa opzione è disabilitata per impostazione predefinita.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Richiedi la firma elettronica per le decisioni</td> 
      <td>Gli utenti devono specificare il nome utente e la password nel momento in cui prendono una decisione sulla bozza.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Blocca la bozza quando vengono prese tutte le decisioni necessarie</td> 
      <td>Quando questa impostazione è abilitata, lo stato della bozza viene bloccato dopo che tutte le decisioni sono state prese. Lo stato viene automaticamente modificato da sbloccato a bloccato quando l'approvatore finale prende la sua decisione.<br>Questa opzione è disabilitata per impostazione predefinita.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Scarica il file originale</td> 
      <td>Quando questa opzione è selezionata, i revisori possono scaricare il file originale da cui è stata creata la bozza.<br>Quando questa opzione è deselezionata, l'icona Scarica non è più visibile.<br>Questa opzione è attivata per impostazione predefinita.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Condividi bozza tramite URL pubblico o codice incorporato</td> 
      <td>Quando questa opzione è selezionata, la bozza può essere condivisa tramite un URL pubblico o un codice di incorporamento.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Iscriviti alla bozza tramite URL pubblico o codice di incorporamento</td> 
      <td>Quando questa opzione è selezionata, le persone che non sono state aggiunte esplicitamente alla bozza possono abbonarsi alla bozza. Alla persona che si abbona alla bozza vengono assegnati il ruolo e l’e-mail definiti nelle seguenti impostazioni:
       <ul>
        <li><strong>Ruolo del sottoscrittore:</strong> Ruolo di bozza predefinito assegnato a tutti i revisori che sottoscrivono la bozza.</li>
        <li><strong>Impostazioni degli avvisi e-mail per i sottoscrittori:</strong> L'avviso e-mail predefinito assegnato a tutti i revisori che si abbonano alla bozza.</li>
       </ul><p>
        <ul>
         <li><strong>Accesso alla bozza tramite collegamento e-mail richiesto per:</strong> Configurare se il sottoscrittore riceve un'e-mail con un collegamento alla bozza. È possibile selezionare <strong>Nessuna e-mail</strong> (il collegamento e-mail non è necessario per accedere alla bozza), <strong>Solo e-mail di notifica bozza</strong> (l'abbonato riceve un collegamento alla bozza tramite e-mail senza alcuna verifica) o <strong>E-mail di notifica di convalida e bozza</strong> (l'abbonato riceve un collegamento alla bozza tramite e-mail e deve fare clic sul collegamento per accedere a una bozza; lo scopo di questa opzione è verificare che l'utente abbia immesso un indirizzo e-mail corretto al quale ha accesso).</li>
        </ul><p><strong>Nota:</strong> se alle bozze è allegato un flusso di lavoro automatizzato, tutte le sottoscrizioni genereranno e-mail di conferma ai proprietari delle bozze, in modo che possano decidere a quale fase aggiungere la persona.<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Fare clic su **Crea bozza**.

   Workfront inizia a generare una bozza dei documenti o dei siti web selezionati. A seconda delle dimensioni e del tipo di file, il tempo di ritardo per il caricamento di un documento può variare. Attendi, poiché la generazione di file più grandi richiede più tempo. Puoi spostarti dalla pagina e Workfront continua a generare il file. La dimensione massima per il caricamento dei file è di 4 GB.

1. Dopo aver generato la bozza, fare clic su **Apri bozza** per avviare il visualizzatore di bozze.

   ![Apri bozza](assets/open-proof-350x132.png)

   Gli utenti che non hanno abilitato la verifica sul proprio account possono comunque visualizzare il documento e aggiungere commenti alla bozza [.](../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md)
