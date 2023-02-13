---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Condividere una bozza in Adobe Workfront
description: È possibile condividere un documento protetto all’interno di Adobe Workfront condividendo il documento o aggiungendo utenti alla bozza.
author: Courtney
feature: Digital Content and Documents
exl-id: a5438db3-6507-4ebc-a27c-65f02c45783e
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '1137'
ht-degree: 0%

---

# Condividere una bozza in Adobe Workfront

È possibile condividere un documento protetto all’interno di Adobe Workfront condividendo il documento o aggiungendo utenti alla bozza.

Se condividi la bozza, come spiegato in questo articolo, il destinatario ha lo stesso accesso al documento e alla bozza. Inoltre, puoi richiedere l’approvazione della bozza al destinatario.

>[!TIP]
>
>Puoi anche condividere una bozza all’interno del visualizzatore di correzione. Per istruzioni, consulta [Condividere una bozza dal visualizzatore di bozze](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md).

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
   <td role="rowheader">Ruolo bozza</td> 
   <td>Autore o moderatore</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica accesso ai documenti</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il ruolo o il profilo delle autorizzazioni di prova, contattare l&#39;amministratore Workfront o Workfront Proof.

## Condivisione di un collegamento a una bozza

La condivisione di un collegamento a prova consente agli utenti di Workfront di visualizzare l’accesso. Gli utenti possono commentare la bozza e iscriversi alle notifiche e-mail relative alla bozza utilizzando le proprie credenziali di accesso Workfront. Gli utenti che non dispongono di prove possono aggiungere commenti e iscriversi utilizzando un indirizzo e-mail e un nome visualizzato.

>[!IMPORTANT]
>
>L’impostazione Consenti prova di condivisione tramite URL pubblico o codice di incorporamento deve essere abilitata.

1. Selezionare il documento contenente la bozza che si desidera condividere con gli utenti.

   È possibile selezionare un solo documento. Non è possibile condividere il collegamento per più documenti contemporaneamente.

1. Fai clic su **Condividi** > **Collegamento di prova**.
1. In **Collegamento di bozza** nella casella visualizzata, effettuare una delle seguenti operazioni:

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

## Aggiungere utenti a una bozza

Puoi aggiungere qualsiasi utente Workfront alla bozza se disponi dei diritti di modifica sulla bozza. Se la bozza ha più fasi, aggiungi l’utente a un singolo passaggio

>[!NOTE]
>
>Tieni presente quanto segue se utilizzi un piano Workfront legacy in cui la correzione può essere abilitata e disabilitata per un utente:
>
>* Per poter esaminare la bozza, non è necessario che i destinatari dispongano di prove abilitate.
>* Quando Flusso di lavoro automatico è abilitato e aggiungi un utente alla bozza per la quale non è abilitata la correzione, viene creata una nuova fase all’interno del flusso di lavoro automatico. L’utente che aggiungi viene aggiunto automaticamente a questa nuova fase quando visualizza la bozza per la prima volta. (Per ulteriori informazioni, consulta [Panoramica del flusso di lavoro automatizzato](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).)
>


### Aggiungere utenti a una bozza esistente dalla scheda Documenti

1. Selezionare il documento contenente la bozza a cui si desidera aggiungere gli utenti.
1. Se la bozza non dispone di un flusso di lavoro automatizzato (fasi), fai clic sul pulsante **Altro** nell&#39;angolo superiore destro della sezione Stage 1, quindi fare clic su **Condividi** nel menu a discesa .

   Oppure

   Se la bozza dispone di un flusso di lavoro automatizzato, fai clic sul pulsante **Altro** nell’angolo in alto a destra dello stage in cui si desidera aggiungere il revisore, quindi fare clic su **Condividi** nel menu a discesa .

1. In **Condividi questa versione** casella visualizzata, sotto **Condividi**, inizia a digitare il nome o l’indirizzo e-mail di un utente con cui desideri condividere la bozza, quindi fai clic sul nome quando viene visualizzato nell’elenco a discesa.

1. (Facoltativo) Ripeti questo passaggio per aggiungere più utenti alla bozza.
1. (Facoltativo) Imposta una scadenza per i revisori.
1. (Facoltativo) Assicurati **Informa le persone tramite e-mail** viene selezionato se desideri comunicare ai revisori di averli aggiunti alla bozza.
1. (Facoltativo) **Aggiungere un messaggio personalizzato** all’e-mail.
1. Dopo aver aggiunto tutti i revisori, fai clic su **Condividi**.

### Aggiungi gli utenti a una bozza esistente dal visualizzatore di correzione

È possibile aggiungere utenti a una bozza durante la revisione di una bozza nel visualizzatore per correzione Web e nel visualizzatore per correzione desktop.

Per ulteriori informazioni, consulta [Condividere una bozza aggiungendo utenti](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md#sharing-with-individual-users) nell&#39;articolo [Condividere una bozza dal visualizzatore di bozze](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md)

## Relazione sulle approvazioni di bozze

Puoi creare un rapporto che riporta le approvazioni di correzione condivise in Workfront. Questo rapporto fornisce le seguenti informazioni di approvazione della bozza nel sistema:

* Documento inviato per l&#39;approvazione
* Nome dell&#39;approvatore
* Versione di prova
* ID bozza
* Data creazione bozza

Puoi accedere a questa approvazione quando crei un report basato su un oggetto, come descritto in [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Per ulteriori informazioni sul rapporto dell&#39;oggetto Proof Approvals (Approvazioni bozza), consulta la sezione [Rapporto sugli oggetti](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects) sezione [Comprendere gli oggetti in Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)

## Approvare una bozza condivisa

Quando un utente ti aggiunge a una bozza e concede il ruolo Approvatore o il ruolo Revisore e approvatore tramite Flusso di lavoro automatizzato, la richiesta di approvazione viene visualizzata nella scheda Approvazioni nella tua home o area Lavoro personale. Puoi quindi visualizzare la bozza e prendere una decisione di approvazione sulla bozza direttamente da Workfront.

Per informazioni su come prendere decisioni di approvazione dall&#39;area Lavoro personale, vedere [Approvare i lavori dall&#39;area Home](../../../review-and-approve-work/manage-approvals/approving-work.md#approving-work-from-the-home-area) o [Approvazione del lavoro](../../../review-and-approve-work/manage-approvals/approving-work.md#approving-work-from-the-my-work-area) in [Approvazione del lavoro](../../../review-and-approve-work/manage-approvals/approving-work.md).
