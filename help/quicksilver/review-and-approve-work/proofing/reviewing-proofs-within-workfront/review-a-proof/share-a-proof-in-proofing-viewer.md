---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: Condividere una bozza dal visualizzatore di bozze
description: Puoi condividere una bozza dal visualizzatore di prova se la condivisione è abilitata dal proprietario o dal creatore della bozza.
author: Courtney
feature: Digital Content and Documents
exl-id: 20bd2d94-1401-4a38-9042-335d0cb32a3d
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '1512'
ht-degree: 0%

---

# Condividere una bozza dal visualizzatore di bozze

Puoi condividere una bozza dal visualizzatore di prova se la condivisione è abilitata dal proprietario o dal creatore della bozza.

>[!IMPORTANT]
>
>L’impostazione Consenti prova di condivisione tramite URL pubblico o codice di incorporamento deve essere abilitata.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Piano attuale: Pro o superiore</p> <p>oppure</p> <p>Piano legacy: Seleziona o Premium</p> <p>Per ulteriori informazioni sulla verifica dell’accesso con i diversi piani, consulta <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accesso alle funzionalità di correzione in Workfront</a>.</p> </td> 
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
   <td> <p>Modifica accesso ai documenti</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il ruolo o il profilo delle autorizzazioni di prova, contattare l&#39;amministratore Workfront o Workfront Proof.

## Condividere l’URL

Puoi condividere una bozza tramite un URL se il proprietario ha configurato la bozza per la condivisione. I proprietari delle prove possono aggiornare le impostazioni di condivisione in qualsiasi momento. Per ulteriori informazioni, consulta [Modifica impostazioni bozza](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md).

1. Se il menu delle icone a sinistra non è visualizzato, fai clic sul pulsante **Menu** nell’angolo in alto a sinistra del visualizzatore di correzione.

   ![](assets/menu-icon-in-proofing-viewer-350x188.png)

1. Nel menu delle icone a sinistra del visualizzatore di correzione, fai clic sul pulsante **Condividi** icona.

   ![Share_btn_in_viewer.png](assets/share-btn-in-viewer.png)

1. In **Condividi bozza** opzioni visualizzate, assicurati **Ottieni collegamento condivisibile** è selezionato.

1.  Effettua una delle seguenti operazioni:

   * Per copiare il collegamento negli Appunti, fai clic su **Copia collegamento**.

      Ora puoi distribuire il collegamento tramite uno strumento di terze parti, ad esempio una chat o un’applicazione e-mail.

   * Per inviare il collegamento direttamente da Adobe Workfront, procedi come segue:

      1. In **Oppure invia un collegamento e-mail a** inizia a digitare e seleziona il nome del destinatario. Oppure specifica l’indirizzo e-mail di un utente esterno con cui desideri condividere l’e-mail.

         >[!NOTE]
         >
         >Se visualizzi un’e-mail di alias quando condividi una bozza, non creare un nuovo utente guest inserendo l’e-mail originale se esiste un’e-mail di alias corrispondente.

      1. Seleziona tra le seguenti opzioni:

         <table style="table-layout:auto">
          <col>
          <col>
          <tbody>
           <tr>
            <td role="rowheader">Invia collegamento pubblico</td>
            <td><p>Include un pulsante nella notifica e-mail che indirizza gli utenti alla bozza all’interno del visualizzatore di correzione che stanno utilizzando e concede l’accesso a Visualizza .</p><p>Se <strong>Iscriviti alla bozza tramite URL pubblico o codice di incorporamento</strong> è disattivato per la bozza, gli utenti possono accedere con le proprie credenziali di accesso Workfront per aggiungere commenti alla bozza. Se è attivato, chiunque fornisca il proprio indirizzo e-mail e nome (senza password richiesta) può firmare e aggiungere commenti alla bozza.</p></td>
           </tr>
           <tr>
            <td role="rowheader">Invia collegamento di download</td>
            <td>Include un pulsante nella notifica e-mail che indirizza gli utenti a una pagina di download, che fornisce i dettagli del file, il nome del file e le dimensioni del file, con il file visualizzato in linea. Gli utenti possono fare clic sul collegamento Scarica dalla pagina di download per scaricare il file.</td>
           </tr>
           <tr>
            <td role="rowheader">Aggiungi messaggio personalizzato</td>
            <td>Consente di specificare un oggetto e un corpo personalizzati per la notifica e-mail.</td>
           </tr>
          </tbody>
         </table>

      1. Fai clic su **Invia**.

         I destinatari ricevono una notifica e-mail contenente informazioni sulla bozza e sui pulsanti che hai scelto di includere.

         ![](assets/proof-share-email-350x87.png)

## Condividere il codice di incorporamento

Puoi condividere una bozza tramite codice di incorporamento se il proprietario della bozza la ha configurata per questo.

Per condividere una bozza tramite il codice di incorporamento:

1. Nella barra degli strumenti a sinistra del visualizzatore di correzione, fai clic sul pulsante **Condividi** icona.

   ![Condividi_btn_in_viewer_1_.png](assets/share-btn-in-viewer--1-.png)

1. In **Condividi bozza** opzioni visualizzate, fai clic su **Ottieni codice di incorporamento**, quindi fai clic su **Copia**.

## Condividere una bozza aggiungendo utenti

Puoi aggiungere utenti a una bozza durante la revisione di una bozza se disponi delle seguenti autorizzazioni:

* Autorizzazioni di supervisore o amministratore
* Autorizzazioni di Manager e tu sei il creatore o il proprietario della bozza
* Autorizzazioni Manager con il ruolo Autore o Moderatore

Se la bozza dispone di un flusso di lavoro automatizzato, puoi aggiungere l’utente a una singola fase. Per ulteriori informazioni, consulta [Panoramica del flusso di lavoro automatizzato](../../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

Per impostazione predefinita, gli utenti aggiunti alla bozza:

* Ricevi una notifica e-mail con un collegamento alla bozza.
* Può prendere decisioni di approvazione sulla bozza dall&#39;area Home o My Work, come descritto in [Approvazione del lavoro](../../../../review-and-approve-work/manage-approvals/approving-work.md).
* Non è necessario che la correzione sia attivata per poter esaminare la prova.

Quando Flusso di lavoro automatico è abilitato e aggiungi un utente alla bozza per la quale non è abilitata la correzione, viene creata una nuova fase all’interno del flusso di lavoro automatico. L’utente che aggiungi viene aggiunto automaticamente a questa nuova fase quando visualizza la bozza per la prima volta. Per ulteriori informazioni, consulta [Panoramica del flusso di lavoro automatizzato](../../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

Per condividere una bozza con singoli utenti:

1. Nella barra degli strumenti a sinistra del visualizzatore di correzione, fai clic sul pulsante **Condividi** icona.

   ![Condividi_btn_in_viewer_2_.png](assets/share-btn-in-viewer--2-.png)

1. Fai clic su **Aggiungi destinatari** nell&#39;elenco a sinistra.
1. Sotto **Nuovi destinatari della bozza**, inizia a digitare il nome di un utente con cui desideri condividere la bozza, quindi fai clic sul nome quando viene visualizzato nell’elenco a discesa.
1. (Facoltativo) Modificare le opzioni del revisore a destra del nome della persona:

   * **Ruolo di prova**: Per ulteriori informazioni, consulta [Gestire i ruoli delle prove in Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

   * **Stage**: Disponibile solo se la bozza dispone di un flusso di lavoro automatizzato. Per ulteriori informazioni, consulta  [Panoramica delle fasi del flusso di lavoro automatizzato](../../../../review-and-approve-work/proofing/proofing-overview/stages.md).

   * **Avvisi e-mail**: seleziona una delle seguenti opzioni per specificare in che modo la persona verrà informata dell’attività sulla bozza.

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
        <td>Un’e-mail viene inviata al revisore solo se qualcuno risponde esplicitamente al proprio commento (questo esclude le proprie risposte dai propri commenti). Ciò significa che se qualcuno sulla bozza fa un nuovo commento, il revisore non viene informato.<p>Questa impostazione è consigliata per i clienti sulla prova in modo che non siano informati di altri commenti sulla prova e siano informati solo delle risposte alle proprie osservazioni.</p><p>Sebbene i revisori con questa impostazione di avviso e-mail non siano informati di altri nuovi commenti, possono comunque visualizzare tutti i commenti sulla bozza nel visualizzatore di correzione.</p><p>Per informazioni sui commenti, consulta <a href="../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Visualizza e risponde ai commenti di prova</a>.</p></td> 
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
        <td>Workfront invia un’e-mail con tutti i commenti, le risposte e le decisioni elencati solo nei giorni in cui è presente un’attività oltre alla tua.<p>Questo avviso è un buon modo per visualizzare un riepilogo del progetto senza essere sopraffatto da numerosi aggiornamenti durante tutto il giorno.</p><p>Un esempio di utilizzo per questo riepilogo è un responsabile del reparto che desidera monitorare l'avanzamento complessivo del progetto.</p><p>Per ulteriori informazioni, consulta <a href="../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Gestione delle notifiche per commenti e decisioni di bozza</a>.</p></td> 
       </tr> 
       <tr data-mc-conditions=""> 
        <td role="rowheader">Nessuna e-mail</td> 
        <td>Workfront non invia avvisi e-mail.<br>Questo è utile per una persona che viene aggiunta a una prova solo a scopo di riferimento e non deve essere informata di eventuali modifiche.<p>Il valore predefinito del sistema è Riepilogo giornaliero (visualizzato anche come Non impostato). Se tu o i tuoi revisori non apporti altre modifiche, tutte le tue bozze avranno questa impostazione.</p></td> 
       </tr> 
      </tbody> 
     </table>

1. (Facoltativo) Ripeti i due passaggi precedenti per aggiungere più utenti alla bozza. 
1. (Facoltativo) Imposta un **Termine** per i revisori (disponibile solo se la bozza non dispone di flusso di lavoro automatizzato).
1. (Facoltativo) Seleziona **Inviare notifiche e-mail a nuovi destinatari** per far loro sapere che li hai aggiunti alla prova.
1. Al termine dell’aggiunta degli utenti alla bozza, fai clic su **Fatto.**
