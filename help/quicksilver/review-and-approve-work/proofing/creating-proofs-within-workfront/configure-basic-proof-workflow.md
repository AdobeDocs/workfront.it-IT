---
product-area: documents;setup
navigation-topic: create-proofs-within-workfront
title: Creare una bozza avanzata con un flusso di lavoro di base
description: Con un flusso di lavoro di base, puoi assegnare diversi revisori a una bozza, ma non sono organizzati in fasi. Tutti i revisori aggiunti possono accedere alla bozza immediatamente dopo la creazione.
author: Courtney
feature: Digital Content and Documents
exl-id: 4f5d0c0e-e070-4f32-89c4-3b511a3b7fdc
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '1831'
ht-degree: 1%

---

# Creare una bozza avanzata con un flusso di lavoro di base

Con un flusso di lavoro di base, puoi assegnare diversi revisori a una bozza, ma non sono organizzati in fasi. Tutti i revisori aggiunti possono accedere alla bozza immediatamente dopo la creazione.

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

## Creare una bozza avanzata con un flusso di lavoro di base

1. Vai al progetto, all&#39;attività o al problema in cui desideri ottenere la bozza, quindi fai clic sul pulsante **Documenti** scheda .
1. Fai clic su **Aggiungi nuovo** > Prova, carica il contenuto, quindi passa alle sezioni elencate di seguito.

   oppure

   Passa il puntatore del mouse su un documento esistente, quindi fai clic sul pulsante **Crea bozza** > **Prove avanzate** e procedere attraverso le sezioni elencate di seguito.

## Configurare il flusso di lavoro e aggiungere revisori

1. Nella sezione Tipo di flusso di lavoro , scegli **Base**.
1. Specifica gli utenti da aggiungere, quindi scegli un ruolo di bozza.

   ![](assets/new-proof---roles-350x213.png)

1. Nella tabella seguente sono elencati tutti i ruoli e i diritti associati.

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
      <th> <p><strong>Aggiungi marcature</strong> </p> </th> 
      <th> <p><strong>Aggiungi commenti</strong> </p> </th> 
      <th> <p><strong>Modifica commenti personalizzati in assenza di risposte</strong> </p> </th> 
      <th> <p><strong>Prendere una decisione</strong> </p> </th> 
      <th> <p><strong>Elimina i commenti degli altri</strong> </p> </th> 
      <th>Risolvere i commenti</th> 
      <th>Applicare azioni ai commenti</th> 
      <th> <p><strong>Modificare la bozza</strong> </p> </th> 
      <th>Condividi la bozza con altri</th> 
      <th>Crea nuova versione</th> 
      <th> <p><strong>Visualizza richieste di approvazione nell'area Home</strong> </p> </th> 
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

1. Gli utenti che utilizzano nuovi piani Workfront possono assegnare ruoli di autore o moderatore a qualsiasi utente del sistema. Gli utenti che utilizzano piani legacy possono assegnare ruoli di autore o moderatore a qualsiasi utente con una licenza a prova nel sistema.
1. (Facoltativo) Con il menu a discesa ancora aperto, seleziona le autorizzazioni aggiuntive disponibili nella parte inferiore del menu:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Risolvere i commenti e applicare azioni </td> 
      <td> <p>Consente all’utente Workfront di effettuare le seguenti operazioni:</p> 
       <ul> 
        <li>Risolvi un commento dopo che è stato affrontato, come spiegato in <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/resolve-proof-comments.md" class="MCXref xref">Risolvere i commenti della bozza</a>.</li> 
        <li>Applicare azioni ai commenti, come spiegato in <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/use-actions-on-comments-in-viewer.md" class="MCXref xref">Utilizzare azioni sui commenti della bozza</a>. </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Condividi bozza con tag</td> 
      <td> <p>Consente al revisore di aggiungere qualsiasi utente Workfront alla bozza come spiegato in <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/tag-users-to-share-proof.md" class="MCXref xref">Assegnare tag agli utenti per condividere una bozza</a>.</p> <p>Nota:  <p>Se queste due opzioni non sono disponibili (in grigio), l’utente dispone già di un profilo di autorizzazione che consente di risolvere i commenti, applicare azioni ai commenti e assegnare tag a qualsiasi utente. </p> <p>Se le opzioni non vengono visualizzate, la persona aggiunta non è un titolare di licenza Workfront.</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Ripeti i passaggi da 1 a 3 per tutti gli altri utenti aggiunti alla bozza.
1. Per ogni utente con cui condividi, nella **Avvisi e-mail** elenco a discesa, seleziona il tipo di avvisi e-mail che l’utente riceve quando gli utenti effettuano commenti e decisioni sulla bozza:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Tutte le attività</td> 
      <td>Workfront invia un’e-mail al revisore ogni volta che vi è un’attività sulla bozza, ad esempio un nuovo commento, una risposta o una decisione. <p>Questa è una grande opzione per la persona che gestisce il processo di correzione perché consente loro di vedere l'attività mentre si verifica. </p><p>Gli utenti non ricevono un avviso e-mail relativo alla propria attività.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Risposte ai miei commenti</td> 
      <td>Un’e-mail viene inviata al revisore solo se qualcuno risponde esplicitamente al proprio commento (questo esclude le proprie risposte dai propri commenti). Ciò significa che se qualcuno sulla bozza fa un nuovo commento, il revisore non viene informato.<p>Questa impostazione è consigliata per i clienti sulla prova in modo che non siano informati di altri commenti sulla prova e siano informati solo delle risposte alle proprie osservazioni.</p><p>Sebbene i revisori con questa impostazione di avviso e-mail non siano informati di altri nuovi commenti, possono comunque visualizzare tutti i commenti sulla bozza nel visualizzatore di correzione.</p><p>Per informazioni sui commenti, consulta <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Visualizza e risponde ai commenti di prova</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Decisioni</td> 
      <td>Workfront invia un’e-mail al revisore solo quando qualcuno prende una decisione.<p>Questo può essere utile per la persona che gestisce il processo di approvazione (ad esempio un project manager) e deve monitorare l’avanzamento della bozza e vedere quali utenti hanno preso la loro decisione.</p><p>Non riceverai una notifica della tua decisione a meno che non selezioni un’opzione di conferma e-mail quando invii la tua decisione.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Decisione finale</td> 
      <td>Workfront invia un'e-mail quando l'ultimo approvatore della bozza ha preso la sua decisione.<p>Questo avviso viene spesso utilizzato dal designer, che di solito non deve prendere parte alla discussione di revisione effettiva. Al momento della decisione finale, il progettista viene informato e può quindi intervenire su eventuali modifiche necessarie.</p><p>Questo avviso può essere utile anche per un responsabile di reparto che deve essere informato solo al termine del processo di revisione.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Riepilogo orario</td> 
      <td>Workfront invia un messaggio e-mail al revisore ogni ora con un riepilogo di tutti i commenti, le risposte e le decisioni che si sono verificate nell’ora.<p>L’e-mail viene inviata solo quando l’attività oltre alla tua si verifica entro l’ora passata. </p><p>Questo avviso è un buon modo per vedere una panoramica del progetto.</p><p>Un esempio di utilizzo per questo riepilogo è un revisore senior che necessita di una panoramica del progetto ma non deve essere informato immediatamente di tutte le attività sulla bozza.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Riepilogo giornaliero</td> 
      <td>Workfront invia un’e-mail con tutti i commenti, le risposte e le decisioni elencati solo nei giorni in cui è presente un’attività oltre alla tua.<p>Questo avviso è un buon modo per visualizzare un riepilogo del progetto senza essere sopraffatto da numerosi aggiornamenti durante tutto il giorno.</p><p>Un esempio di utilizzo per questo riepilogo è un responsabile del reparto che desidera monitorare l'avanzamento complessivo del progetto.</p><p>Per ulteriori informazioni, consulta <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Gestione delle notifiche per commenti e decisioni di bozza</a>.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Nessuna e-mail</td> 
      <td>Workfront non invia avvisi e-mail.<br>Questo è utile per una persona che viene aggiunta a una prova solo a scopo di riferimento e non deve essere informata di eventuali modifiche.<p>Il valore predefinito del sistema è Riepilogo giornaliero (visualizzato anche come Non impostato). Se tu o i tuoi revisori non apporti altre modifiche, tutte le tue bozze avranno questa impostazione.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Continua con [Configurare le impostazioni e-mail per la bozza](#configure-email-settings-for-the-proof) sotto.

## Configurare le impostazioni e-mail per la bozza {#configure-email-settings-for-the-proof}

1. In **Notifica e-mail** seleziona se inviare notifiche e-mail e un messaggio personalizzato agli utenti selezionati in [Creare una bozza avanzata con un flusso di lavoro di base](#workflow) in precedenza in questo articolo:

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
        </ul><p>Nota:  Se le bozze dispongono di Flusso di lavoro automatico allegato a tutte le sottoscrizioni genereranno e-mail di conferma ai proprietari delle bozze, in modo che possano decidere a quale fase aggiungere la persona.<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Crea bozza**.

   Workfront inizia a generare una bozza dei documenti o dei siti Web selezionati. A seconda delle dimensioni e del tipo di file, il tempo di ritardo nel caricamento di un documento può variare. Sii paziente, perché i file più grandi richiedono più tempo per generare. Puoi allontanarti dalla pagina e Workfront continua a generare il file. La dimensione massima di caricamento dei file è 4 GB.

1. Dopo aver generato la bozza, fai clic su **Prova aperta** per avviare il visualizzatore di correzione.

   ![](assets/open-proof-350x132.png)

   Gli utenti che non dispongono di prove abilitate sul proprio account possono comunque visualizzare il documento e inviare commenti alla bozza.