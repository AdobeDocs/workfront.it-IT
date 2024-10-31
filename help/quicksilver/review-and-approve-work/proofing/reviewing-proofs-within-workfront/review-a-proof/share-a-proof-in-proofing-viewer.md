---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: Condividere una bozza dal visualizzatore di bozze
description: Puoi condividere una bozza dal visualizzatore di bozze se la condivisione è abilitata dal proprietario o dal creatore della bozza.
author: Courtney
feature: Digital Content and Documents
exl-id: 20bd2d94-1401-4a38-9042-335d0cb32a3d
source-git-commit: aaf5beb8692b2fdbb797ba908796d78b4ee8866c
workflow-type: tm+mt
source-wordcount: '1509'
ht-degree: 0%

---

# Condividere una bozza dal visualizzatore di bozze

Puoi condividere una bozza dal visualizzatore di bozze se la condivisione è abilitata dal proprietario o dal creatore della bozza.

>[!IMPORTANT]
>
>È necessario abilitare l’impostazione Consenti condivisione bozze tramite URL pubblico o codice di incorporamento.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Piano corrente: Pro o superiore</p> <p>oppure</p> <p>Piano legacy: Seleziona o Premium</p> <p>Per ulteriori informazioni sulla verifica dell'accesso con i diversi piani, vedere <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accesso alla funzionalità di verifica in Workfront</a>.</p> </td> 
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
   <td> <p>Modifica accesso ai documenti</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, la mansione o il profilo di autorizzazione della bozza di cui si dispone, contattare l&#39;amministratore di Workfront o Workfront Proof.

+++

## Condividere l’URL

Puoi condividere una bozza tramite un URL se il proprietario ha configurato la bozza per la condivisione. I proprietari delle bozze possono aggiornare le impostazioni di condivisione in qualsiasi momento. Per ulteriori informazioni, vedere [Modifica impostazioni bozza](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md).

1. Se il menu dell&#39;icona sinistra non è visualizzato, fare clic sull&#39;icona **Menu** nell&#39;angolo superiore sinistro del visualizzatore di bozze.

   ![](assets/menu-icon-in-proofing-viewer-350x188.png)

1. Nel menu dell&#39;icona a sinistra del visualizzatore di bozze, fare clic sull&#39;icona **Condividi**.

   ![Condividi_btn_in_viewer.png](assets/share-btn-in-viewer.png)

1. Nelle opzioni **Condividi bozza** visualizzate, assicurati che sia selezionato **Ottieni collegamento condivisibile**.

1.  Effettuare una delle seguenti operazioni:

   * Per copiare il collegamento negli Appunti, fare clic su **Copia collegamento**.

     Ora puoi distribuire il collegamento tramite uno strumento di terze parti, ad esempio una chat o un’applicazione e-mail.

   * Per inviare il collegamento tramite e-mail direttamente da Adobe Workfront, effettua le seguenti operazioni:

      1. Nel campo **O collegamento e-mail a**, inizia a digitare e selezionare il nome del destinatario. In alternativa, specifica l’indirizzo e-mail di un utente esterno con cui desideri condividere il messaggio.

         >[!NOTE]
         >
         >Se durante la condivisione di una bozza viene visualizzato un messaggio e-mail di alias, non creare un nuovo utente ospite immettendo l&#39;e-mail originale se esiste un messaggio e-mail di alias corrispondente.

      1. Selezionare una delle opzioni seguenti:

         <table style="table-layout:auto">
          <col>
          <col>
          <tbody>
           <tr>
            <td role="rowheader">Invia collegamento pubblico</td>
            <td><p>Include un pulsante nella notifica e-mail che indirizza gli utenti alla bozza nel visualizzatore di bozze in uso e concede l’accesso in visualizzazione.</p><p>Se <strong>Abbonati alla bozza tramite URL pubblico o codice di incorporamento</strong> è disattivato per la bozza, gli utenti possono accedere con le credenziali di accesso di Workfront per aggiungere commenti alla bozza. Se è attivata, chiunque fornisca il proprio indirizzo e-mail e nome (non è richiesta alcuna password) può firmare e aggiungere commenti alla bozza.</p></td>
           </tr>
           <tr>
            <td role="rowheader">Invia collegamento per il download</td>
            <td>Include un pulsante nella notifica e-mail che indirizza gli utenti a una pagina di download, in cui sono riportati i dettagli, il nome e la dimensione del file, con il file visualizzato in linea. Per scaricare il file, gli utenti possono fare clic sul collegamento Scarica dalla pagina di download.</td>
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

Puoi condividere una bozza tramite il codice di incorporamento se il proprietario della bozza l’ha configurata per questo.

Per condividere una bozza tramite il codice di incorporamento:

1. Nella barra degli strumenti sulla sinistra del visualizzatore di bozze, fai clic sull&#39;icona **Condividi**.

   ![Condividi_btn_in_viewer__1_.png](assets/share-btn-in-viewer--1-.png)

1. Nelle opzioni **Condividi bozza** visualizzate, fai clic su **Ottieni codice di incorporamento**, quindi su **Copia**.

## Condividere una bozza aggiungendovi utenti

Puoi aggiungere utenti a una bozza durante la revisione di una bozza se disponi di una delle seguenti autorizzazioni:

* Autorizzazioni di supervisore o amministratore
* Autorizzazioni di Manager e sei il creatore o il proprietario della bozza
* Autorizzazioni di Manager con il ruolo Bozza Autore o Moderatore

Se la bozza dispone di un flusso di lavoro automatizzato, puoi aggiungere l’utente a una singola fase. Per ulteriori informazioni, vedere [Panoramica del flusso di lavoro automatico](../../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

Per impostazione predefinita, gli utenti aggiunti alla bozza:

* Ricevi una notifica e-mail con un collegamento alla bozza.
* Può prendere decisioni di approvazione sulla bozza dall&#39;area Home, come descritto in [Approvazione del lavoro](../../../../review-and-approve-work/manage-approvals/approving-work.md).
* Non è necessario che siano abilitate prove per esaminare la bozza.

Quando il flusso di lavoro automatizzato è abilitato e si aggiunge un utente alla bozza per il quale non sono abilitati gli strumenti di correzione in Workfront, viene creata una nuova fase all’interno del flusso di lavoro automatico. L’utente che stai aggiungendo viene aggiunto automaticamente a questa nuova fase quando visualizza la bozza per la prima volta. Per ulteriori informazioni, vedere [Panoramica del flusso di lavoro automatico](../../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

Per condividere una bozza con i singoli utenti:

1. Nella barra degli strumenti sulla sinistra del visualizzatore di bozze, fai clic sull&#39;icona **Condividi**.

   ![Condividi_btn_in_viewer__2_.png](assets/share-btn-in-viewer--2-.png)

1. Fai clic su **Aggiungi destinatari** nell&#39;elenco a sinistra.
1. In **Destinatari nuova bozza**, inizia a digitare il nome di un utente con cui si desidera condividere la bozza, quindi fai clic sul nome quando viene visualizzato nell&#39;elenco a discesa.
1. (Facoltativo) Modifica le opzioni revisore a destra del nome della persona:

   * **Ruolo bozza**: per ulteriori informazioni, vedere [Gestione dei ruoli bozza in Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

   * **Fase**: (disponibile solo se la bozza dispone di un flusso di lavoro automatizzato). Per ulteriori informazioni, consulta  [Panoramica delle fasi del flusso di lavoro automatizzato](../../../../review-and-approve-work/proofing/proofing-overview/stages.md).

   * **Avvisi e-mail**: seleziona una delle opzioni seguenti per specificare in che modo la persona riceverà le notifiche sull&#39;attività nella bozza.

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
        <td>Un'e-mail viene inviata al revisore solo se qualcuno risponde esplicitamente al proprio commento (questo esclude le proprie risposte sui propri commenti). Ciò significa che se qualcuno sulla bozza fa un nuovo commento, il revisore non riceve alcuna notifica.<p>Questa impostazione è consigliata per i clienti della bozza, in modo che non ricevano alcuna notifica di altri commenti sulla bozza e ricevano solo le risposte ai propri commenti.</p><p>Anche se ai revisori con questa impostazione di avviso e-mail non vengono notificati altri nuovi commenti, possono comunque visualizzare tutti i commenti sulla bozza nel visualizzatore di bozze.</p><p>Per informazioni sui commenti, vedere <a href="../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Visualizzare e rispondere ai commenti della bozza</a>.</p></td> 
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
        <td>Workfront invia un’e-mail con tutti i commenti, le risposte e le decisioni elencati solo nei giorni in cui è presente attività oltre alla tua.<p>Questo avviso è un buon modo per visualizzare un riepilogo del progetto senza essere sommersi da più aggiornamenti durante la giornata.</p><p>Un caso d’uso di esempio per questo riepilogo è un responsabile di reparto che desidera monitorare l’avanzamento generale del progetto.</p><p>Per ulteriori informazioni, consulta <a href="../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Gestire le notifiche per i commenti e le decisioni relative alle bozze</a>.</p></td> 
       </tr> 
       <tr data-mc-conditions=""> 
        <td role="rowheader">Nessuna e-mail</td> 
        <td>Workfront non invia avvisi e-mail.<br>Questo è utile per una persona che viene aggiunta a una bozza solo a scopo di riferimento e non deve essere avvisata di eventuali modifiche.<p>L'impostazione predefinita del sistema è Riepilogo giornaliero (visualizzato anche come Non impostato). Se tu o i tuoi revisori non apportate altre modifiche, tutte le bozze dispongono di questa impostazione.</p></td> 
       </tr> 
      </tbody> 
     </table>

1. (Facoltativo) Ripeti i due passaggi precedenti per aggiungere più utenti alla bozza. 
1. (Facoltativo) Imposta una **Scadenza** per i revisori (disponibile solo se la bozza non dispone di un flusso di lavoro automatizzato).
1. (Facoltativo) Seleziona **Invia una notifica e-mail ai nuovi destinatari** per informarli che li hai aggiunti alla bozza.
1. Dopo aver aggiunto gli utenti alla bozza, fai clic su **Fine.**
