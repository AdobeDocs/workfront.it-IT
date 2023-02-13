---
product-area: documents;setup
navigation-topic: create-proofs-within-workfront
title: Creare una bozza avanzata con un flusso di lavoro automatizzato
description: Un flusso di lavoro automatizzato semplifica la gestione del processo di revisione se il processo è complesso o se si inviano regolarmente contenuti da rivedere alle stesse persone. La bozza si sposta da un passaggio all’altro e Adobe Workfront notifica a ogni utente quando tocca a lui rivederla. Per ulteriori informazioni sui flussi di lavoro automatizzati, consulta Panoramica sui flussi di lavoro automatizzati .
author: Courtney
feature: Digital Content and Documents
exl-id: 977fe1bc-458f-4301-8056-dc51c61edb6c
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '1856'
ht-degree: 0%

---

# Creare una bozza avanzata con un flusso di lavoro automatizzato

Un flusso di lavoro automatizzato semplifica la gestione del processo di revisione se il processo è complesso o se si inviano regolarmente contenuti da rivedere alle stesse persone. La bozza si sposta da un passaggio all’altro e Adobe Workfront notifica a ogni utente quando tocca a lui rivederla. Per ulteriori informazioni sui flussi di lavoro automatizzati, consulta [Panoramica del flusso di lavoro automatizzato](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Piano attuale: Pro o superiore</p> <p>oppure</p> <p>Piano legacy: Seleziona o superiore</p> <p>Per ulteriori informazioni sulla verifica dell’accesso con i diversi piani, consulta <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accesso alle funzionalità di correzione in Workfront</a>.</p> </td> 
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

## Creare una bozza avanzata con un flusso di lavoro automatizzato

1. Vai al progetto, all&#39;attività o al problema in cui desideri ottenere la bozza, quindi fai clic sul pulsante **Documenti** scheda .
1. Fai clic su **Aggiungi nuovo** > Prova, carica il contenuto, quindi passa alle sezioni elencate di seguito.

   oppure

   Passa il puntatore del mouse su un documento esistente, quindi fai clic sul pulsante **Crea bozza** > **Prove avanzate** e procedere attraverso le sezioni elencate di seguito.

## Configurare le fasi di bozza

1. Nella sezione Tipo di flusso di lavoro , scegli **Automatico**.
1. (Facoltativo) Per utilizzare un modello di flusso di lavoro automatizzato creato e condiviso dall’amministratore Workfront, fai clic su **Aggiungi modello**, seleziona il modello nella casella visualizzata, quindi fai clic su **Aggiungi modello**.

   >[!NOTE]
   >
   >Quando utilizzi un modello di flusso di lavoro automatizzato, considera quanto segue:
   >   
   >* Le impostazioni di un modello di flusso di lavoro automatizzato determinano le operazioni che è possibile eseguire con il flusso di lavoro automatico per una bozza. Ad esempio, se il pulsante Aggiungi un passaggio è disabilitato nel modello, questo non è visibile perché lavori con le impostazioni del flusso di lavoro automatizzato per la bozza.
   * Quando una persona viene aggiunta a una pagina in un modello di flusso di lavoro automatizzato, ma è già presente come revisore sulla bozza, l’applicazione del modello rimuove il revisore dal passaggio. Se non aggiungi un altro revisore all’area di visualizzazione, viene visualizzato un messaggio per richiedere di aggiungerne uno.
   * La possibilità di modificare un modello di flusso di lavoro automatizzato dipende dalle impostazioni del modello configurate dall’amministratore di Workfront, come descritto in . Se la possibilità di modificare il modello è disabilitata, solo il proprietario del modello può modificarlo.


1. Configura la prima fase del flusso di lavoro automatizzato:

   1. (Facoltativo) Per creare un nome per il primo passaggio, fai clic su **Fase 1**, quindi digita il nome.
   1. In **Destinatari** per l’area di visualizzazione, aggiungi i revisori all’area di visualizzazione.

      >[!NOTE]
      Quando aggiungi revisori a un&#39;area di visualizzazione, considera quanto segue:
      * Puoi aggiungere utenti esterni a un&#39;area di visualizzazione con un indirizzo e-mail.
      * Dopo aver aggiunto un utente a un’area di visualizzazione, puoi configurare le impostazioni per tale utente sulla bozza.
      * Puoi trascinare gli utenti direttamente su un altro passaggio, oppure puoi trascinare gli utenti su un altro passaggio **Fasi** diagramma. Per selezionare più utenti, premere Maiusc+Ctrl (su Windows) o Maiusc+Comando (su Mac).
      * È possibile aggiungere un revisore a una bozza una sola volta, il che significa che non è possibile aggiungere la stessa persona a più di una fase della bozza.
      * I revisori che non vengono aggiunti a uno stadio privato non possono vedere tale stadio sulla prova o sui commenti fatti in tale fase.
      * Per impostazione predefinita, l’aggiunta di un utente a un’area di visualizzazione consente all’utente di accedere alla bozza dal momento in cui viene creata.\
         L’amministratore di Workfront può impedire agli utenti di accedere alla bozza finché il flusso di lavoro non entra nell’area in cui è stato aggiunto l’utente.


   1. Fai clic su **Impostazioni dello stage**.
   1. Fai clic su **Attiva fase** per indicare come attivare l’area di visualizzazione.

      Per il primo passaggio, puoi selezionare solo **Creazione a prova di**, **In una data e un’ora specifiche** oppure **Manualmente**.

   1. (Condizionale) Se hai selezionato **In una data e un’ora specifiche** nel passaggio precedente, seleziona la data e l’ora in cui desideri attivare l’area di visualizzazione nel **Attiva** che appare.

   1. Utilizza una delle opzioni seguenti per configurare ulteriormente l’area di visualizzazione.

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">Imposta scadenza fase</td>
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
         <td role="rowheader">Trasferimento dei diritti di decisione principali a</td>
         <td><p>Seleziona il decision maker principale nell’area di visualizzazione (disponibile solo dopo l’aggiunta di almeno una persona allo stadio con un ruolo di approvatore o superiore). Se selezioni un modulo decisionale principale, la <strong>È necessaria una sola decisione</strong> in questo passaggio l’opzione è disabilitata.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Richiedi una sola decisione per questa fase</td>
         <td>Termina l'intero processo di revisione quando uno dei decisori prende una decisione.<p>Questa opzione non è disponibile se hai designato un utente nel <strong>Decisore principale</strong>menu a discesa.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Rendi questo palco privato</td>
         <td>Consente solo alle persone seguenti di visualizzare i commenti e le decisioni prese durante questa fase: Amministratori di supervisori, amministratori Workfront e amministratori di Workfront Proof</td>
        </tr>
       </tbody>
      </table>

1. Per aggiungere e configurare un altro passaggio:

   1. Fai clic su **Nuovo stadio**.
   1. (Facoltativo) Per creare un nome per il primo passaggio, fai clic su **Fase 2** o **Fase 3**, **Fase 4**, e così via), quindi digita il nome.

   1. Fai clic sul pulsante **Attiva fase**, quindi seleziona un’opzione per specificare se l’area di visualizzazione viene attivata automaticamente o manualmente.

      Oltre alle opzioni **Creazione a prova di**, **In una data e un’ora specifiche** oppure **Manualmente**, puoi selezionare un’opzione che dipende da cosa si è verificato nel passaggio precedente:

      ![](assets/activate-stage-options-for-stage-2-plus-350x177.png)

   1. Se hai selezionato un’opzione Attiva fase che dipende da cosa si è verificato nel passaggio precedente, utilizza le opzioni visualizzate per configurare l’impostazione di attivazione.

      Ad esempio, se hai selezionato **Quando cambia lo stato della fase precedente**, seleziona **Fase precedente**, quindi seleziona lo stato nel **Stato modificato in** scatola.

1. Ripeti il passaggio precedente in base alle esigenze per aggiungere altri stadi.

   Quando si aggiungono aree di visualizzazione al flusso di lavoro automatizzato, sullo schermo viene visualizzato un diagramma che le rappresenta:

   ![](assets/stages-diagram-350x213.png)

1. Continua con [Configurare le impostazioni e-mail per la bozza](#configure-email-settings-for-the-proof) sotto.

## Configurare le impostazioni e-mail per la bozza {#configure-email-settings-for-the-proof}

1. In **Notifica e-mail** seleziona se inviare notifiche e-mail e un messaggio personalizzato agli utenti selezionati in [Creare una bozza avanzata con un flusso di lavoro automatizzato](#workflow) in precedenza in questo articolo:

   <table>
      <tbody>
      <tr>
      <td>Notifica ai destinatari questa bozza</td>
      <td>Seleziona questa opzione per inviare una notifica e-mail agli utenti. Quando <strong>Condivisione di base</strong> è selezionato in <strong>Flusso di lavoro</strong> una notifica e-mail viene inviata quando viene creata la bozza. Quando <strong>Flusso di lavoro automatizzato</strong> è selezionato in <strong>Flusso di lavoro</strong> una notifica e-mail viene inviata quando la bozza entra nella fase del flusso di lavoro automatizzato a cui l’utente è associato.</td>
      </tr>
      <tr>
      <td>Aggiungi messaggio personalizzato</td>
      <td>Seleziona questa opzione per includere un messaggio personalizzato nella notifica. Puoi specificare un oggetto e il corpo del messaggio. Il corpo del messaggio può includere formattazione RTF, ad esempio grassetto, punti elenco e collegamenti ipertestuali.</td>
      </tr>
      </tbody>
      </table>


1. Continua con [Configurare le impostazioni di bozza](#configure-proof-settings) sotto.

## Configurare le impostazioni di bozza {#configure-proof-settings}

1. In **Impostazioni di bozza** seleziona una delle seguenti opzioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Richiedi accesso: la bozza può essere condivisa solo con altri utenti</td> 
      <td>Quando questa opzione è disabilitata (impostazione predefinita), chiunque disponga dell’URL può visualizzare la bozza. <br>Quando questa opzione è selezionata:
       <ul>
        <li>Solo gli utenti di Workfront Proof possono visualizzare la bozza.</li>
        <li>Gli utenti non possono accedere alla bozza a meno che non siano stati aggiunti alla bozza.</li>
        <li>Impossibile abilitare le sottoscrizioni.</li>
       </ul></td> 
     </tr> 
     <tr> 
      <td role="rowheader">È necessaria una sola decisione per questa prova</td> 
      <td>Quando questa opzione è selezionata, la revisione viene completata dopo che uno dei decisori ha preso la loro decisione.<br>Questa opzione è disabilitata per impostazione predefinita.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Richiedi la firma elettronica per le decisioni</td> 
      <td>Gli utenti devono specificare il proprio nome utente e la propria password al momento della decisione su una bozza.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Blocca la prova quando vengono prese tutte le decisioni necessarie</td> 
      <td>Quando questa impostazione è abilitata, lo stato della bozza viene bloccato dopo tutte le decisioni. Lo stato viene automaticamente modificato da sbloccato a bloccato quando l’approvatore finale decide.<br>Questa opzione è disabilitata per impostazione predefinita.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Scarica il file originale</td> 
      <td>Quando questa opzione è selezionata, i revisori possono scaricare il file originale da cui è stata creata la bozza.<br>Quando questa opzione è deselezionata, l’icona Scarica non è più visibile.<br>Questa opzione è attivata per impostazione predefinita.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Condividere la bozza tramite URL pubblico o codice di incorporamento</td> 
      <td>Quando questa opzione è selezionata, la bozza può essere condivisa tramite un URL pubblico o un codice di incorporamento.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Iscriviti alla bozza tramite URL pubblico o codice di incorporamento</td> 
      <td>Quando questa opzione è selezionata, le persone che non sono state aggiunte esplicitamente alla bozza possono abbonarsi alla bozza. Alla persona che si abbona alla bozza viene assegnato il ruolo e l’e-mail definiti nelle seguenti impostazioni:
       <ul>
        <li><strong>Ruolo sottoscrittore:</strong> Il ruolo di bozza predefinito assegnato a tutti i revisori che si abbonano alla bozza. </li>
        <li><strong>Impostazioni avvisi e-mail per gli abbonati:</strong> L’avviso e-mail predefinito assegnato a tutti i revisori che si abbonano alla bozza.</li>
       </ul><p>
        <ul>
         <li><strong>Accesso a prova tramite collegamento e-mail richiesto per:</strong> Configura se il sottoscrittore riceve un'e-mail con un collegamento alla bozza. È possibile selezionare <strong>Nessuna e-mail</strong> (il collegamento e-mail non è necessario per accedere alla bozza), <strong>Solo e-mail di notifica della bozza</strong> (l’abbonato riceve un collegamento alla prova tramite e-mail senza alcuna verifica), o <strong>E-mail di notifica di convalida e prova</strong> (l’utente iscritto riceve un collegamento alla bozza tramite e-mail e deve fare clic sul collegamento per accedere a una bozza, lo scopo di questa opzione è quello di garantire che la persona abbia inserito un indirizzo e-mail corretto al quale ha accesso).</li>
        </ul><p><strong>Nota:</strong> Se le bozze dispongono di Flusso di lavoro automatico allegato a tutte le sottoscrizioni genereranno e-mail di conferma ai proprietari delle bozze, in modo che possano decidere a quale fase aggiungere la persona.<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Crea bozza**.

   Workfront inizia a generare una bozza dei documenti o dei siti Web selezionati. A seconda delle dimensioni e del tipo di file, il tempo di ritardo nel caricamento di un documento può variare. Sii paziente, perché i file più grandi richiedono più tempo per generare. Puoi allontanarti dalla pagina e Workfront continua a generare il file. La dimensione massima di caricamento dei file è 4 GB.

1. Dopo aver generato la bozza, fai clic su **Prova aperta** per avviare il visualizzatore di correzione.

   ![](assets/open-proof-350x132.png)

   Gli utenti che non dispongono di prove abilitate sul proprio account possono ancora visualizzare il documento e formulare commenti sulla bozza [.](../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md)
