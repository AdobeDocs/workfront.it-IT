---
product-area: documents;setup
navigation-topic: create-proofs-within-workfront
title: Creare una bozza avanzata con un flusso di lavoro automatizzato
description: Un flusso di lavoro automatizzato semplifica la gestione del processo di revisione se il processo è complesso o se invii regolarmente contenuti per la revisione agli stessi utenti. La bozza si sposta da un ambiente di staging all’altro e Adobe Workfront notifica a ogni utente quando è il momento di rivederla. Per ulteriori informazioni sui flussi di lavoro automatizzati, consulta Panoramica sui flussi di lavoro automatizzati.
author: Courtney
feature: Digital Content and Documents
exl-id: 977fe1bc-458f-4301-8056-dc51c61edb6c
source-git-commit: afc0cbb93e26eb29abfb1b00b32c79c1b65ff3eb
workflow-type: tm+mt
source-wordcount: '1856'
ht-degree: 0%

---

# Creare una bozza avanzata con un flusso di lavoro automatizzato

Un flusso di lavoro automatizzato semplifica la gestione del processo di revisione se il processo è complesso o se invii regolarmente contenuti per la revisione agli stessi utenti. La bozza si sposta da un ambiente di staging all’altro e Adobe Workfront notifica a ogni utente quando è il momento di rivederla. Per ulteriori informazioni sui flussi di lavoro automatizzati, consulta [Panoramica del flusso di lavoro automatizzato](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Piano corrente: Pro o superiore</p> <p>oppure</p> <p>Piano legacy: Seleziona o superiore</p> <p>Per ulteriori informazioni sulla verifica dell'accesso con i diversi piani, vedere <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accesso alla funzionalità di verifica in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano corrente: Lavoro o Piano</p> <p>Piano legacy: qualsiasi (per l’utente deve essere abilitata la verifica)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Profilo autorizzazione bozza </td> 
   <td>Manager o superiore</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modifica accesso ai documenti</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, la mansione o il profilo di autorizzazione della bozza disponibile, contattare l&#39;amministratore Workfront o Workfront Proof.

## Creare una bozza avanzata con un flusso di lavoro automatizzato

1. Vai al progetto, all’attività o al problema nel punto in cui desideri inserire la bozza, quindi fai clic sul pulsante **Documenti** scheda.
1. Clic **Aggiungi nuovo** > Bozza, carica il contenuto, quindi utilizza le sezioni elencate di seguito.

   oppure

   Passa il puntatore del mouse su un documento esistente, quindi fai clic su **Crea bozza** > **Bozza avanzata** e utilizzare le sezioni elencate di seguito.

## Configurare le fasi della bozza

1. Nella sezione Tipo di flusso di lavoro scegliere **Automatizzato**.
1. (Facoltativo) Se desideri utilizzare un modello di flusso di lavoro automatizzato creato e condiviso con te dall’amministratore di Workfront, fai clic su **Aggiungi modello**, seleziona il modello nella casella visualizzata, quindi fai clic su **Aggiungi modello**.

   >[!NOTE]
   >
   >Quando si utilizza un modello di flusso di lavoro automatizzato, tenere presente quanto segue:
   >   
   >* Le impostazioni di un modello di flusso di lavoro automatico determinano le operazioni che è possibile eseguire con il flusso di lavoro automatico per una bozza. Ad esempio, se il pulsante Aggiungi un’area di visualizzazione è disabilitato nel modello, non sarà visibile durante l’utilizzo delle impostazioni del flusso di lavoro automatico per la bozza.
   >* Quando una persona viene aggiunta a un’area di un modello di flusso di lavoro automatico, ma è anche già presente come revisore sulla bozza, l’applicazione del modello rimuove il revisore dall’area di visualizzazione. Se non si aggiunge un altro revisore all&#39;area di visualizzazione, verrà visualizzato un messaggio che richiede di aggiungerne uno.
   >* La possibilità di modificare un modello di flusso di lavoro automatico dipende dalle impostazioni del modello configurate dall&#39;amministratore di Workfront, come descritto in . Se la possibilità di modificare il modello è disabilitata, solo il proprietario del modello può modificarlo.

1. Configura la prima fase del flusso di lavoro automatizzato:

   1. (Facoltativo) Per creare un nome per la prima fase, fare clic su **Fase 1**, quindi digita il nome.
   1. In **Destinatari** per l&#39;area di visualizzazione, aggiungere i revisori all&#39;area di visualizzazione.

      >[!NOTE]
      >
      >Quando si aggiungono revisori a una fase, tenere presente quanto segue:
      >   
      >* Puoi aggiungere utenti esterni a una fase con un indirizzo e-mail.
      >* Dopo aver aggiunto un utente a un’area di visualizzazione, puoi configurare le impostazioni per tale utente nella bozza.
      >* È possibile trascinare gli utenti direttamente in un&#39;altra fase oppure trascinare gli utenti in una fase della **Fasi** diagramma. Per selezionare più utenti, premere MAIUSC+Ctrl (su Windows) o MAIUSC+Comando (su Mac).
      >* È possibile aggiungere un revisore a una bozza una sola volta, il che significa che non è possibile aggiungere la stessa persona a più fasi della bozza.
      >* I revisori che non vengono aggiunti a una fase privata non possono vedere tale fase sulla bozza o sui commenti fatti in quella fase.
      >* Per impostazione predefinita, l’aggiunta di un utente a una fase consente a tale utente di accedere alla visualizzazione della bozza dal momento in cui viene creata. L’amministratore di Workfront può impedire agli utenti di accedere alla bozza fino a quando il flusso di lavoro non entra nella fase in cui l’utente è stato aggiunto.

   1. Clic **Impostazioni fase**.
   1. Fai clic su un **Attiva fase** per indicare la modalità di attivazione della fase.

      Per la prima fase, è possibile selezionare solo **Alla creazione della bozza**, **In una data e un’ora specifiche**, o **Manualmente**.

   1. (Condizionale) Se hai selezionato **In una data e un’ora specifiche** nel passaggio precedente, seleziona la data e l’ora in cui desideri attivare la fase nel **Attiva il** che viene visualizzata.

   1. Utilizza una delle opzioni seguenti per configurare ulteriormente la fase.

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">Imposta scadenza fase</td>
         <td><p>Per impostare una scadenza per la fase, fare clic su un'opzione nella <strong>Opzioni scadenza</strong> elenco a discesa. Quindi, sotto <strong>Scadenza</strong>, eseguire una delle operazioni seguenti:</p>
          <ul>
           <li>Se si sceglie <strong>Imposta data specifica</strong>: seleziona la data e l’ora di scadenza desiderate.</li>
           <li>Se si sceglie <strong>Calcola dalla data di attivazione della fase</strong>: seleziona il numero di giorni lavorativi da aggiungere alla data di attivazione della fase per determinare la scadenza.</li>
          </ul></td>
        </tr>
        <tr>
         <td role="rowheader">Fase di blocco</td>
         <td>Specificare quando è possibile bloccare lo stage. </td>
        </tr>
        <tr>
         <td role="rowheader">Trasferisci i diritti di decisione primari a</td>
         <td><p>Selezionare il decisore principale sullo stadio (disponibile solo dopo aver aggiunto almeno una persona allo stadio con il ruolo di Approvatore di bozza o superiore). Se si seleziona un responsabile delle decisioni principale, <strong>È necessaria una sola decisione</strong> in questa fase l'opzione è disattivata.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Richiedi una sola decisione per questa fase</td>
         <td>Termina l’intero processo di revisione quando uno dei responsabili decisionali prende una decisione.<p>Questa opzione non è disponibile se hai designato un utente nel <strong>Principale responsabile delle decisioni</strong>menu a discesa.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Rendi privata questa fase</td>
         <td>Consente solo alle persone seguenti di visualizzare i commenti e le decisioni prese durante questa fase: supervisori, amministratori Workfront e amministratori di bozze Workfront</td>
        </tr>
       </tbody>
      </table>

1. Per aggiungere e configurare un&#39;altra fase:

   1. Clic **Nuova fase**.
   1. (Facoltativo) Per creare un nome per la prima fase, fare clic su **Fase 2** (o **Fase 3**, **Fase 4** e così via), quindi digita il nome.

   1. Fai clic su **Attiva fase**, quindi selezionare un&#39;opzione per specificare se la fase viene attivata automaticamente o manualmente.

      Oltre alle opzioni **Alla creazione della bozza**, **In una data e un’ora specifiche**, o **Manualmente**, puoi selezionare un’opzione che dipende da ciò che si è verificato nel passaggio precedente:

      ![](assets/activate-stage-options-for-stage-2-plus-350x177.png)

   1. Se è stata selezionata un&#39;opzione Attiva fase che dipende da quanto si è verificato nel passaggio precedente, utilizzare le opzioni visualizzate per configurare l&#39;impostazione di attivazione.

      Ad esempio, se hai selezionato **Quando lo stato della fase precedente cambia**, seleziona la **Fase precedente**, quindi seleziona lo stato in **Stato modificato in** casella.

1. Ripetere il passaggio precedente in base alle esigenze per aggiungere altre fasi.

   Quando aggiungi fasi al flusso di lavoro automatico, sullo schermo viene visualizzato un diagramma che le rappresenta:

   ![](assets/stages-diagram-350x213.png)

1. Continua con [Configurare le impostazioni e-mail per la bozza](#configure-email-settings-for-the-proof) di seguito.

## Configurare le impostazioni e-mail per la bozza {#configure-email-settings-for-the-proof}

1. In **Notifica e-mail** , seleziona se inviare notifiche e-mail e un messaggio personalizzato agli utenti selezionati in [Creare una bozza avanzata con un flusso di lavoro automatizzato](#workflow) più avanti in questo articolo:

   <table>
      <tbody>
      <tr>
      <td>Notifica i destinatari relativamente a questa bozza</td>
      <td>Seleziona questa opzione per inviare una notifica e-mail agli utenti. Quando <strong>Condivisione di base</strong> è selezionato in <strong>Flusso di lavoro</strong> , al momento della creazione della bozza viene inviata una notifica e-mail. Quando <strong>Flusso di lavoro automatico</strong> è selezionato in <strong>Flusso di lavoro</strong> , viene inviata una notifica e-mail quando la bozza entra nella fase del flusso di lavoro automatizzato a cui è associato l’utente.</td>
      </tr>
      <tr>
      <td>Aggiungi messaggio personalizzato</td>
      <td>Seleziona questa opzione per includere un messaggio personalizzato nella notifica. È possibile specificare un oggetto e il corpo del messaggio. Il corpo del messaggio può includere formattazione RTF, ad esempio grassetto, punti elenco e collegamenti ipertestuali.</td>
      </tr>
      </tbody>
      </table>


1. Continua con [Configura impostazioni bozza](#configure-proof-settings) di seguito.

## Configura impostazioni bozza {#configure-proof-settings}

1. In **Impostazioni bozza** , selezionare una delle opzioni seguenti:

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
      <td>Quando questa opzione è selezionata, i revisori possono scaricare il file originale da cui è stata creata la bozza.<br>Quando questa opzione è deselezionata, l’icona Scarica non è più visibile.<br>Questa opzione è attivata per impostazione predefinita.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Condividi bozza tramite URL pubblico o codice incorporato</td> 
      <td>Quando questa opzione è selezionata, la bozza può essere condivisa tramite un URL pubblico o un codice di incorporamento.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Iscriviti alla bozza tramite URL pubblico o codice di incorporamento</td> 
      <td>Quando questa opzione è selezionata, le persone che non sono state aggiunte esplicitamente alla bozza possono abbonarsi alla bozza. Alla persona che si abbona alla bozza vengono assegnati il ruolo e l’e-mail definiti nelle seguenti impostazioni:
       <ul>
        <li><strong>Ruolo del sottoscrittore:</strong> Ruolo di bozza predefinito assegnato a tutti i revisori che si abbonano alla bozza.</li>
        <li><strong>Impostazioni degli avvisi e-mail per gli abbonati:</strong> L’avviso e-mail predefinito assegnato a tutti i revisori che si abbonano alla bozza.</li>
       </ul><p>
        <ul>
         <li><strong>L’accesso alla bozza tramite il collegamento e-mail è necessario per:</strong> Specifica se il sottoscrittore riceve un’e-mail con un collegamento alla bozza. Puoi selezionare <strong>Nessuna e-mail</strong> (non è necessario un collegamento e-mail per accedere alla bozza), <strong>Solo e-mail di notifica bozza</strong> (l’abbonato riceve un collegamento alla bozza via e-mail senza alcuna verifica), oppure <strong>E-mail di notifica per convalida e bozza</strong> (l’abbonato riceve un collegamento alla bozza tramite e-mail e deve fare clic sul collegamento per accedere a una bozza; lo scopo di questa opzione è garantire che l’utente abbia inserito un indirizzo e-mail corretto al quale ha accesso).</li>
        </ul><p><strong>Nota:</strong> Se alle bozze è allegato un flusso di lavoro automatico, tutti gli abbonamenti genereranno e-mail di conferma ai proprietari delle bozze, in modo che possano decidere a quale fase aggiungere la persona.<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Clic **Crea bozza**.

   Workfront inizia a generare una bozza dei documenti o dei siti web selezionati. A seconda delle dimensioni e del tipo di file, il tempo di ritardo per il caricamento di un documento può variare. Attendi, poiché la generazione di file più grandi richiede più tempo. Puoi spostarti dalla pagina e Workfront continua a generare il file. La dimensione massima per il caricamento dei file è di 4 GB.

1. Una volta generata la bozza, fai clic su **Apri bozza** per avviare il visualizzatore di bozze.

   ![](assets/open-proof-350x132.png)

   Gli utenti che non hanno la funzione di verifica attivata sul proprio account possono comunque visualizzare il documento e aggiungere commenti alla bozza [.](../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md)
