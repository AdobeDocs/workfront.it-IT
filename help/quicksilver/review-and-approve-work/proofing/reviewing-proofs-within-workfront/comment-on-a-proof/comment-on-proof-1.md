---
product-area: documents
navigation-topic: comment-on-a-proof
title: Commento su una bozza
description: I commenti consentono di fornire feedback sul contenuto e collaborare con altri utenti nel visualizzatore di correzione.
author: Courtney
feature: Digital Content and Documents
exl-id: b0386786-7f90-4d1c-bd3a-1cd545430de1
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '776'
ht-degree: 0%

---

# Commento su una bozza

I commenti consentono di fornire feedback sul contenuto e collaborare con altri utenti nel visualizzatore di correzione.

Quando assegni tag agli utenti nei commenti su una bozza, gli utenti a cui puoi assegnare i tag possono variare a seconda di vari fattori, ad esempio le autorizzazioni per i singoli utenti e l’iscrizione nell’organizzazione:

* Se sei l’autore della bozza, il proprietario o disponi di autorizzazioni specifiche abilitate, puoi assegnare tag agli utenti al di fuori del flusso di lavoro della bozza e condividerla con loro.
* Se sei stato aggiunto alla bozza come utente esterno e sei membro di un altro ambiente con un account di prova diverso, puoi assegnare tag solo agli utenti dell’ambiente originale. <!--For more information, see [Proofing collaboration limitations with people outside of your organization](../../../../review-and-approve-work/proofing/tips-tricks-and-troubleshooting/collaboration-with-members-outside-of-your-organization.md)-->

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
   <td role="rowheader">Ruolo di prova</td> 
   <td>Revisore, Revisore e Approvatore, Moderatore, Autore</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica accesso ai documenti</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il ruolo o il profilo delle autorizzazioni di prova, contattare l&#39;amministratore Workfront o Workfront Proof.

## Commento su una bozza

1. Passa al progetto, all&#39;attività o al problema che contiene il documento, quindi seleziona **Documenti**.
1. Trova la bozza di cui hai bisogno, quindi fai clic su **Prova aperta**.

1. Nella parte superiore del visualizzatore di correzione, fai clic su **Aggiungi commento**.
1. (Condizionale) Se si tratta di una bozza video, riproduci la bozza video, quindi fai clic su **Aggiungi commento** nel punto del video in cui desideri inserire il commento utilizzando i playhead

   >[!TIP]
   >
   >1. Per semplificare l’utilizzo, mettere in pausa il video, fare clic nella riga di tempo in cui si desidera inserire il commento.
   >1. Per una maggiore precisione, puoi fare clic sui valori sopra le testine di riproduzione e digitare nuovi valori.
   >1. Per commentare una serie di riprese video, trascinate le testine di riproduzione a sinistra e a destra nella timeline per indicare una serie di riprese sulle quali desiderate commentare.
   >1. Per commentare una serie di riprese video, trascinate le testine di riproduzione a sinistra e a destra nella timeline per indicare una serie di riprese sulle quali desiderate commentare.


1. Per richiamare l’attenzione su una posizione specifica sulla bozza, fai clic sullo strumento di marcatura desiderato nella barra degli strumenti, quindi contrassegna l’area della bozza su cui desideri commentare:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Disegnare una linea a mano libera</strong> </td> 
      <td> <img src="assets/freehand-line.png"> </td> 
      <td>Consente di aggiungere una linea a mano libera nell’area selezionata.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Disegnare una linea</strong> </td> 
      <td> <img src="assets/line.png"> </td> 
      <td>Consente di disegnare una linea sull’area selezionata.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Disegnare una freccia</strong> </td> 
      <td> <img src="assets/arrow.png"> </td> 
      <td>Consente di aggiungere una freccia a un'area selezionata.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Evidenziare un'area</strong> </td> 
      <td> <img src="assets/highlight.png"> </td> 
      <td>Evidenzia l'area selezionata.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Disegnare un rettangolo</strong> </td> 
      <td> <img src="assets/rectangle.png"> </td> 
      <td>Consente di disegnare un rettangolo intorno a un'area.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Polline</strong> </td> 
      <td> <img src="assets/polyline.png"> </td> 
      <td> <p>Disegna una sequenza connessa di segmenti di linea che è possibile lasciare aperti o chiudere come forma. È possibile spostare o eliminare i punti aggiunti. </p> <p>Questo strumento è utile per lavorare con immagini tecniche e architettoniche.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Modifica colore, spessore o opacità del markup</strong> </td> 
      <td> <img src="assets/change-color.png"> </td> 
      <td>Consente di modificare il colore, lo spessore e l'opacità degli strumenti di marcatura.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Testo</strong> </td> 
      <td> <img src="assets/copy-of-text.png"> </td> 
      <td> <p>Questo strumento viene visualizzato a sinistra degli altri strumenti quando la bozza è un documento basato su testo. Fornisce strumenti di marcatura per commentare il testo nelle bozze. <br></p> <p>Quando fate clic su questo strumento e quindi selezionate il testo sulla bozza, le opzioni di annotazione vengono visualizzate sotto il testo selezionato.<br></p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Nelle bozze statiche, è possibile contrassegnare più aree su più pagine per un commento. Ad esempio, se desideri creare lo stesso commento su più pagine, seleziona un’area in una pagina, quindi vai alla pagina successiva in cui desideri creare lo stesso commento e seleziona un’area lì. Questo vale solo per gli strumenti di marcatura delle annotazioni regolari, non per gli strumenti di marcatura del testo.
1. Digita il tuo commento in **Aggiungi commento** a destra.
1. (Facoltativo) Per assegnare tag a un altro utente del commento e aggiungerlo al flusso di lavoro della bozza, digita @ nella casella del commento, quindi digita il nome o l’indirizzo e-mail dell’utente e seleziona l’utente nel menu visualizzato. Per ulteriori informazioni, consulta [Assegnare tag agli utenti per condividere una bozza](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/tag-users-to-share-proof.md).
1. (Facoltativo) Per allegare un file a un commento, effettuare una delle seguenti operazioni:

   * Fare clic sull&#39;icona del clip di carta nell&#39;angolo in basso a destra del commento, quindi trovare e selezionare il file da caricare.
   * Trascinare un file da una posizione del computer e rilasciarlo nell&#39;area dei commenti.

1. Fai clic su **Post**.
