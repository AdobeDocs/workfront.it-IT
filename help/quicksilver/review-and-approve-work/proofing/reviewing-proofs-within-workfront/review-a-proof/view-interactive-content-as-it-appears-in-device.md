---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: Modificare la risoluzione della bozza interattiva nel visualizzatore di correzione
description: È possibile visualizzare in anteprima l’aspetto di una bozza interattiva su vari dispositivi, per vedere in che modo il contenuto viene visualizzato e risponde in base a risoluzioni diverse.
author: Courtney
feature: Digital Content and Documents
exl-id: 99165790-0c34-4540-92d9-956ae178a874
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '579'
ht-degree: 1%

---

# Modificare la risoluzione della bozza interattiva nel visualizzatore di correzione

È possibile visualizzare in anteprima l’aspetto di una bozza interattiva su vari dispositivi, per vedere in che modo il contenuto viene visualizzato e risponde in base a risoluzioni diverse.

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

## Visualizzazioni di dispositivi e risoluzione nei visualizzatori per correzione desktop e nei visualizzatori per correzione web

L’amministratore di Adobe Workfront ha configurato il sistema in modo da poter esaminare il contenuto interattivo nel visualizzatore per correzione desktop o, come contenuto incluso in un file ZIP, nel visualizzatore per correzione Web:

* Nel visualizzatore per correzione desktop, è possibile visualizzare il modo in cui il contenuto viene visualizzato e risponde sia in diverse risoluzioni che su vari dispositivi. Quando un revisore specifica un determinato dispositivo, il contenuto viene visualizzato come lo sarebbe su quel dispositivo, con le specifiche dell&#39;interfaccia utente per il dispositivo. Ad esempio, un pulsante rosso su una marca di smartphone può essere blu su un marchio diverso.

* Nel visualizzatore per correzione web, è possibile visualizzare il contenuto interattivo così come viene visualizzato nelle risoluzioni per i vari dispositivi. Tuttavia, il visualizzatore per correzione web non emula il contenuto utilizzando le specifiche dell’interfaccia su questi dispositivi, ad esempio il colore del pulsante.

   >[!NOTE]
   >
   >L’amministratore di Workfront può configurare dispositivi personalizzati per gli utenti dell’organizzazione, come descritto in Configurazione di dispositivi personalizzati per bozze interattive nell’articolo .

## Visualizzare una bozza con un dispositivo o un&#39;impostazione di risoluzione preimpostati

1. Passare all&#39;elenco dei documenti contenente la bozza che si desidera aprire.
1. Passa il puntatore del mouse sul documento, quindi fai clic su **Prova aperta**.
1. Fai clic su **Reattivo** al centro del visualizzatore di correzione.

   ![Resolution_option_in_DPV.png](assets/resolution-option-in-dpv-350x64.png)

1. Nell’elenco dei dispositivi e delle risoluzioni visualizzati nel Visualizzatore correzione desktop fare clic su quello desiderato.

   Oppure

   Nell’elenco delle risoluzioni visualizzate del visualizzatore per correzione Web fare clic su quello desiderato.

   Se hai bisogno di informazioni sulle differenze tra questi due visualizzatori, consulta [Panoramica sulle differenze tra il visualizzatore per correzione web e il visualizzatore per correzione desktop](../../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).

   Viene eseguito il rendering della bozza interattiva nella risoluzione selezionata.

## Visualizzare una bozza con un&#39;impostazione di risoluzione personalizzata

1. Passare all&#39;elenco dei documenti contenente la bozza che si desidera aprire.
1. Passa il puntatore del mouse sul documento, quindi fai clic su **Prova aperta**.
1. Fai clic su **Reattivo** al centro del visualizzatore di correzione.
1. Digita una **Reattivo** risoluzione.

   ![Type_a_custom_resolution_DPV.png](assets/type-a-custom-resolution-dpv.png)

   Oppure

   Passa il puntatore del mouse sul contenuto interattivo e trascina il bordo blu nell’angolo in basso a destra o sul bordo destro o inferiore alla risoluzione desiderata.

   ![Drag_blue_edge_for_resolution.png](assets/drag-blue-edges-for-resolution-350x251.png)

   La risoluzione personalizzata viene visualizzata nelle seguenti posizioni:

   * In **Risoluzione** nel centro inferiore del visualizzatore.\
      ![Screenshot_2018-05-15_10-27-54.png](assets/screenshot-2018-05-15-10-27-54.png)

   * In tutti i commenti i revisori aggiungono alla bozza. Ogni commento include la risoluzione dello schermo selezionata al momento della creazione del commento da parte del revisore.
