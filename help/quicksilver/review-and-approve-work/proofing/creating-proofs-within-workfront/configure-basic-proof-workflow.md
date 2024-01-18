---
product-area: documents;setup
navigation-topic: create-proofs-within-workfront
title: Creare una bozza avanzata con un flusso di lavoro di base
description: Con un flusso di lavoro di base, è possibile inviare più revisori a una bozza, ma non sono organizzati in più fasi. Tutti i revisori aggiunti possono accedere alla bozza immediatamente dopo la sua creazione.
author: Courtney
feature: Digital Content and Documents
exl-id: 4f5d0c0e-e070-4f32-89c4-3b511a3b7fdc
source-git-commit: 41a2d58ce00baa6460ee6ca697d4fe06363eee85
workflow-type: tm+mt
source-wordcount: '1842'
ht-degree: 1%

---

# Creare una bozza avanzata con un flusso di lavoro di base

Con un flusso di lavoro di base, è possibile inviare più revisori a una bozza, ma non sono organizzati in più fasi. Tutti i revisori aggiunti possono accedere alla bozza immediatamente dopo la sua creazione.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td>
   <p>Nuovo: Qualsiasi</p>
    <p>Piano corrente: Pro o superiore</p>
   <p>Piano legacy: Seleziona o superiore</p> <p>Per ulteriori informazioni sulla verifica dell'accesso con i diversi piani, vedere <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accesso alla funzionalità di verifica in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td>
   <p>Nuovo: Standard</p>
    <p>Corrente: Lavoro o Piano</p> <p>Piano legacy: qualsiasi (per l’utente deve essere abilitata la verifica)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Profilo autorizzazione bozza </td> 
   <td>Manager o superiore</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica accesso ai documenti</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, la mansione o il profilo di autorizzazione della bozza disponibile, contattare l&#39;amministratore Workfront o Workfront Proof.

## Creare una bozza avanzata con un flusso di lavoro di base

1. Vai al progetto, all’attività o al problema nel punto in cui desideri inserire la bozza, quindi fai clic sul pulsante **Documenti** scheda.
1. Clic **Aggiungi nuovo** > Bozza, carica il contenuto, quindi utilizza le sezioni elencate di seguito.

   oppure

   Passa il puntatore del mouse su un documento esistente, quindi fai clic su **Crea bozza** > **Bozza avanzata** e utilizzare le sezioni elencate di seguito.

## Configurare il flusso di lavoro e aggiungere i revisori

1. Nella sezione Tipo di flusso di lavoro scegliere **Base**.
1. Specifica gli utenti da aggiungere, quindi scegli un ruolo Bozza.

   ![](assets/new-proof---roles-350x213.png)

1. Nella tabella seguente sono elencati tutti i ruoli e i diritti ad essi associati.

   <table border="1" cellspacing="15" cellpadding="1"> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p> </p> </th> 
      <th> <p><strong>Visualizzare una bozza</strong> </p> </th> 
      <th> <p><strong>Aggiungi markup</strong> </p> </th> 
      <th> <p><strong>Aggiungi commenti</strong> </p> </th> 
      <th> <p><strong>Modifica i propri commenti in assenza di risposte</strong> </p> </th> 
      <th> <p><strong>Prendi una decisione</strong> </p> </th> 
      <th> <p><strong>Elimina commenti aggiunti da altri</strong> </p> </th> 
      <th>Risolvi commenti</th> 
      <th>Applica azioni ai commenti</th> 
      <th> <p><strong>Modifica la bozza</strong> </p> </th> 
      <th>Condividi la bozza con altri utenti</th> 
      <th>Crea nuova versione</th> 
      <th> <p><strong>Visualizzare le richieste di approvazione nell’area Home</strong> </p> </th> 
      <th>Aggiungi nuovi revisori</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p><strong>Sola lettura</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> </td> 
      <td>✓</td> 
      <td> <p> </p> </td> 
      <td>✓</td> 
      <td> </td> 
      <td> </td> 
      <td> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>Revisore</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> </td> 
      <td>✓</td> 
      <td> <p> </p> </td> 
      <td>✓</td> 
      <td> </td> 
      <td> </td> 
      <td> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>Approvatore</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p> </p> </td> 
      <td> </td> 
      <td>✓</td> 
      <td> <p> </p> </td> 
      <td>✓</td> 
      <td> </td> 
      <td> <p>✓</p> </td> 
      <td> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>Revisore e Approvatore</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p> </p> </td> 
      <td> </td> 
      <td>✓</td> 
      <td> <p> </p> </td> 
      <td>✓</td> 
      <td> </td> 
      <td> <p>✓</p> </td> 
      <td> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>Autore</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p> </p> </td> 
      <td>✓</td> 
      <td>✓</td> 
      <td> <p>✓</p> </td> 
      <td>✓</td> 
      <td>✓</td> 
      <td> </td> 
      <td>✓</td> 
     </tr> 
     <tr> 
      <td> <p><strong>Moderatore</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p><strong>✓</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> <p> </p> </td> 
      <td>✓</td> 
      <td>✓</td> 
      <td> <p>✓</p> </td> 
      <td>✓</td> 
      <td>✓</td> 
      <td>✓</td> 
      <td>✓</td> 
     </tr> 
    </tbody> 
   </table>

1. Gli utenti dei nuovi piani di Workfront possono assegnare ruoli di autore o moderatore a qualsiasi utente del sistema. Gli utenti che usano piani precedenti possono concedere ruoli di autore o moderatore a qualsiasi utente con una licenza Verifica nel sistema.
1. (Facoltativo) Con il menu a discesa ancora aperto, seleziona le autorizzazioni aggiuntive disponibili nella parte inferiore del menu:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Risolvere commenti e applicare azioni </td> 
      <td> <p>Consente all’utente di Workfront di effettuare le seguenti operazioni:</p> 
       <ul> 
        <li>Risolvere un commento dopo averlo affrontato, come spiegato in <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/resolve-proof-comments.md" class="MCXref xref">Risolvi commenti bozza</a>.</li> 
        <li>Applicare azioni ai commenti, come spiegato in <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/use-actions-on-comments-in-viewer.md" class="MCXref xref">Utilizzare le azioni sui commenti della bozza</a>. </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Condividi bozza con tag</td> 
      <td> <p>Consente al revisore di aggiungere qualsiasi utente Workfront alla bozza come spiegato in <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/tag-users-to-share-proof.md" class="MCXref xref">Assegnare tag agli utenti per condividere una bozza</a>.</p> <p>Nota:  <p>Se queste due opzioni non sono disponibili (sono disattivate), l’utente dispone già di un profilo di autorizzazione che consente di risolvere i commenti, applicare azioni ai commenti e assegnare tag a qualsiasi utente. </p> <p>Se le opzioni non vengono visualizzate, la persona aggiunta non è un titolare di licenza Workfront.</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Ripeti i passaggi 1-3 per tutti gli altri utenti aggiunti alla bozza.
1. Per ogni utente con cui stai condividendo, nel **Avvisi e-mail** dall’elenco a discesa, seleziona il tipo di avvisi e-mail che questo utente riceve quando le persone prendono commenti e decisioni sulla bozza:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Tutte le attività</td> 
      <td>Workfront invia un’e-mail al revisore ogni volta che si verifica un’attività sulla bozza, ad esempio un nuovo commento, una nuova risposta o una nuova decisione. <p>Si tratta di un'ottima opzione per la persona che gestisce il processo di verifica, in quanto consente di visualizzare l'attività nel momento in cui si verifica. </p><p>Gli utenti non ricevono un avviso e-mail relativo alla propria attività.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Risposte ai miei commenti</td> 
      <td>Un'e-mail viene inviata al revisore solo se qualcuno risponde esplicitamente al proprio commento (questo esclude le proprie risposte sui propri commenti). Ciò significa che se qualcuno sulla bozza fa un nuovo commento, il revisore non riceve alcuna notifica.<p>Questa impostazione è consigliata per i clienti della bozza, in modo che non ricevano alcuna notifica di altri commenti sulla bozza e ricevano solo le risposte ai propri commenti.</p><p>Anche se ai revisori con questa impostazione di avviso e-mail non vengono notificati altri nuovi commenti, possono comunque visualizzare tutti i commenti sulla bozza nel visualizzatore di bozze.</p><p>Per informazioni sui commenti, vedi <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Visualizza e rispondi ai commenti della bozza</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Decisioni</td> 
      <td>Workfront invia un'e-mail al revisore solo quando qualcuno prende una decisione.<p>Questo può essere utile per la persona che gestisce il processo di approvazione (ad esempio, un project manager) e che deve monitorare i progressi sulla bozza e vedere quali utenti hanno preso la loro decisione.</p><p>Non riceverai una notifica della tua decisione a meno che tu non selezioni un’opzione di conferma e-mail al momento dell’invio della decisione.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Decisione finale</td> 
      <td>Workfront invia un’e-mail quando l’ultimo approvatore della bozza prende la sua decisione.<p>Questo avviso viene spesso utilizzato dal progettista, che di solito non ha bisogno di partecipare alla discussione di revisione effettiva. Al momento della decisione finale, il progettista riceve una notifica e può quindi intervenire su eventuali modifiche necessarie.</p><p>Questo avviso può essere utile anche per un responsabile di reparto che deve ricevere una notifica solo al termine del processo di revisione.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Riepilogo orario</td> 
      <td>Workfront invia ogni ora un messaggio e-mail al revisore con un riepilogo di tutti i commenti, le risposte e le decisioni che si sono verificati nel corso dell’ora.<p>L’e-mail viene inviata solo quando nell’ultima ora si verifica un’attività oltre alla tua. </p><p>Questo avviso è utile per avere una panoramica del progetto.</p><p>Un caso d’uso di esempio per questo riepilogo è un revisore senior che ha bisogno di una panoramica del progetto ma non ha bisogno di essere informato immediatamente di tutte le attività sulla bozza.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Riepilogo giornaliero</td> 
      <td>Workfront invia un’e-mail con tutti i commenti, le risposte e le decisioni elencati solo nei giorni in cui è presente attività oltre alla tua.<p>Questo avviso è un buon modo per visualizzare un riepilogo del progetto senza essere sommersi da più aggiornamenti durante la giornata.</p><p>Un caso d’uso di esempio per questo riepilogo è un responsabile di reparto che desidera monitorare l’avanzamento generale del progetto.</p><p>Per ulteriori informazioni, consulta <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Gestire le notifiche per i commenti e le decisioni relativi alle bozze</a>.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Nessuna e-mail</td> 
      <td>Workfront non invia avvisi e-mail.<br>Questo è utile per una persona che viene aggiunta a una bozza solo a scopo di riferimento e non deve essere avvisata di eventuali modifiche.<p>L'impostazione predefinita del sistema è Riepilogo giornaliero (visualizzato anche come Non impostato). Se tu o i tuoi revisori non apportate altre modifiche, tutte le bozze dispongono di questa impostazione.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Continua con [Configurare le impostazioni e-mail per la bozza](#configure-email-settings-for-the-proof) di seguito.

## Configurare le impostazioni e-mail per la bozza {#configure-email-settings-for-the-proof}

1. In **Notifica e-mail** , seleziona se inviare notifiche e-mail e un messaggio personalizzato agli utenti selezionati in [Creare una bozza avanzata con un flusso di lavoro di base](#workflow) più avanti in questo articolo:

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
        <li><strong>Ruolo del sottoscrittore:</strong> Ruolo di bozza predefinito assegnato a tutti i revisori che si abbonano alla bozza. </li>
        <li><strong>Impostazioni degli avvisi e-mail per gli abbonati:</strong> L’avviso e-mail predefinito assegnato a tutti i revisori che si abbonano alla bozza.</li>
       </ul><p>
        <ul>
         <li><strong>L’accesso alla bozza tramite il collegamento e-mail è necessario per:</strong> Specifica se il sottoscrittore riceve un’e-mail con un collegamento alla bozza. Puoi selezionare <strong>Nessuna e-mail</strong> (non è necessario un collegamento e-mail per accedere alla bozza), <strong>Solo e-mail di notifica bozza</strong> (l’abbonato riceve un collegamento alla bozza via e-mail senza alcuna verifica), oppure <strong>E-mail di notifica per convalida e bozza</strong> (l’abbonato riceve un collegamento alla bozza tramite e-mail e deve fare clic sul collegamento per accedere a una bozza; lo scopo di questa opzione è garantire che l’utente abbia inserito un indirizzo e-mail corretto al quale ha accesso).</li>
        </ul><p>Nota: se alle bozze è allegato un flusso di lavoro automatico, tutti gli abbonamenti genereranno e-mail di conferma ai proprietari delle bozze, in modo che possano decidere a quale fase aggiungere la persona.<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Clic **Crea bozza**.

   Workfront inizia a generare una bozza dei documenti o dei siti web selezionati. A seconda delle dimensioni e del tipo di file, il tempo di ritardo per il caricamento di un documento può variare. Attendi, poiché la generazione di file più grandi richiede più tempo. Puoi spostarti dalla pagina e Workfront continua a generare il file. La dimensione massima per il caricamento dei file è di 4 GB.

1. Una volta generata la bozza, fai clic su **Apri bozza** per avviare il visualizzatore di bozze.

   ![](assets/open-proof-350x132.png)

   Gli utenti che non dispongono di un account di verifica abilitato possono comunque visualizzare il documento e aggiungere commenti alla bozza.