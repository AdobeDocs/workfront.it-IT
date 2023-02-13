---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-xd
title: Caricare XD tavole da disegno come bozze in Workfront
description: Puoi caricare le tue tavole da disegno come bozze direttamente in Adobe Workfront per una revisione e un’approvazione complete.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: d6699fd7-f130-4231-8713-0cfa8dc3c910
source-git-commit: 4a7fb18674b399b138fd981907f3a9da8e0bb30e
workflow-type: tm+mt
source-wordcount: '965'
ht-degree: 0%

---

# Carica [!DNL XD] come bozze per [!DNL Workfront]

Potete caricare le vostre tavole da disegno come bozze direttamente in [!DNL Adobe Workfront] per un esame e un&#39;approvazione approfonditi.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td> 
   <td> <p>Piano attuale: [!UICONTROL Pro] o superiore</p> <p>oppure</p> <p>Piano legacy: [!UICONTROL Premium]</p> <p>Per ulteriori informazioni sulla correzione dell’accesso ai diversi piani, consulta .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td> 
   <td> <p>Piano attuale: [!UICONTROL Work] o [!UICONTROL Proof]</p> <p>Piano legacy: Qualsiasi (è necessario che la correzione sia attivata per l’utente)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>Devi avere un [!DNL Adobe Creative Cloud] oltre a una licenza [!DNL Workfront] licenza.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Profilo autorizzazione bozza </td> 
   <td>[!UICONTROL Manager] o superiore</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Modifica accesso ai documenti</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, ruolo o profilo di autorizzazione della bozza hai, contatta il tuo [!DNL Workfront] o [!DNL Workfront Proof] amministratore.

## Prerequisiti

* È necessario installare [!DNL Adobe Workfront for XD] plugin prima di poter caricare le bozze in [!DNL Adobe XD].

   Per istruzioni, consulta [Installa [!DNL Adobe Workfront for XD]](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-adobe-xd-install.md).

## Caricare una bozza statica

1. Fai clic sul pulsante **[!UICONTROL Menu]** nell&#39;angolo in alto a destra, quindi seleziona **[!UICONTROL Elenco lavori]**. È inoltre possibile utilizzare il menu per passare agli oggetti principali.

   ![](assets/menu-350x440.png)

1. Passa all’elemento di lavoro in cui desideri caricare una bozza statica.
1. Fai clic sul pulsante **[!UICONTROL Documento]** icona ![](assets/documents.png) nella barra di navigazione.

1. Fai clic su **[!UICONTROL Nuovo file]** vicino al fondo del plugin.
1. Selezionate le tavole da disegno da caricare.

   >[!TIP]
   >
   >Per selezionare più tavole da disegno, fate clic e trascinate il mouse sulle tavole da disegno desiderate.

1. Abilita **[!UICONTROL Creare una bozza]**.

1. Denomina la bozza.

1. Scegliere il tipo di approvazione della bozza desiderato:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Basic]: </td> 
      <td> <p>I processi di approvazione di base sono ad hoc e possono includere diversi revisori in base alle esigenze: </p> 
       <ul> 
        <li> <p>(Facoltativo) Aggiungi <strong>Approvatori</strong> nella scatola.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Automatizzato]</td> 
      <td> <p>I processi di approvazione automatizzata sono precompilati dagli amministratori e includono revisori e fasi specifici. Per ulteriori informazioni, consulta <a href="../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Panoramica del flusso di lavoro automatizzato</a>.</p> 
       <ul> 
        <li> <p>Scegli un modello di flusso di lavoro dal menu a discesa.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facoltativo) Digita un commento nella sezione **[!UICONTROL Aggiornamenti]** area.

   ![](assets/proof-approvals-xd-350x396.png)

1. Scegli il formato di esportazione dal **[!UICONTROL Tipo di risorsa]** menu a discesa.


1. (Facoltativo) Se selezionate PDF come tipo di risorsa e selezionate più tavole da disegno, scegliete se esportare le tavole da disegno come **[!UICONTROL File PDF singolo]s** o **M[!UICONTROL più file PDF]**.

1. (Facoltativo) Denomina il PDF.

   ![](assets/pdf-options.png)

1. Fai clic su **[!UICONTROL Carica]**.\
   Il documento viene visualizzato nel [!UICONTROL Documenti] nell’area del plug-in e nell’app desktop.

## Caricare una bozza interattiva {#upload-an-interactive-proof}

È possibile creare una bozza interattiva per le tavole da disegno con [!DNL Workfront for Adobe] plugin. Si tratta di un processo in due fasi. Innanzitutto devi creare un collegamento interattivo, quindi devi caricare la bozza in un elemento di lavoro.

### Creare un collegamento interattivo per la tavola da disegno  {#create-an-interactive-link-for-your-art-board}

1. Apri la tavola da disegno, quindi fai clic su **[!UICONTROL Condividi]** nell’area in alto a sinistra dello schermo.
1. Specifica le impostazioni del collegamento:

   1. Assegna un nome al collegamento.
   1. Scegli un’impostazione di visualizzazione.
   1. In **[!UICONTROL Accesso collegamento]** sezione , assicurati **[!UICONTROL Chiunque con questo link]** è selezionato.

      Per generare una bozza interattiva, devi attivare questo tipo di accesso.

   1. Fai clic su **[!UICONTROL Crea collegamento]**.

1. Fai clic nuovamente su **[!UICONTROL Progettazione]** nell’area in alto a sinistra dello schermo. Procedi alla [Caricare una bozza interattiva](#upload-an-interactive-proof) di seguito.

   >[!NOTE]
   >
   >Potrebbe essere necessario riaprire il pannello dei plug-in nell’angolo in basso a sinistra dello schermo.

### Caricare una bozza interattiva

1. Fai clic sul pulsante **[!UICONTROL Menu]** nell&#39;angolo in alto a destra, quindi seleziona **[!UICONTROL Elenco lavori]**. È inoltre possibile utilizzare il menu per passare agli oggetti principali.

   ![](assets/menu-350x440.png)

1. Passa all’elemento di lavoro in cui desideri caricare una bozza interattiva.
1. Fai clic sul pulsante **[!UICONTROL Documento]** icona ![](assets/documents.png) nella barra di navigazione.

1. Fai clic su **[!UICONTROL Nuovo file]** vicino al fondo del plugin.
1. Abilita **[!UICONTROL Creare una bozza]**.

1. Scegliere il tipo di approvazione della bozza desiderato:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Basic]: </td> 
      <td> <p>I processi di approvazione di base sono ad hoc e possono includere diversi revisori in base alle esigenze: </p> 
       <ul> 
        <li> <p>(Facoltativo) Aggiungi <strong>Approvatori</strong> nella scatola.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Automatizzato]</td> 
      <td> <p>I processi di approvazione automatizzata sono precompilati dagli amministratori e includono revisori e fasi specifici. Per ulteriori informazioni, consulta <a href="../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Panoramica del flusso di lavoro automatizzato</a>.</p> 
       <ul> 
        <li> <p>Scegli un modello di flusso di lavoro dal menu a discesa.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facoltativo) Digita un commento nella sezione **[!UICONTROL Aggiornamenti]** area.

   ![](assets/proof-approvals-xd-350x396.png)

1. In **[!UICONTROL Tipo di risorsa]** menu a discesa, scegli il collegamento appena creato sotto il **Collegamenti condivisi** scheda . Per ulteriori informazioni, consulta [Creare un collegamento interattivo per la tavola da disegno](#create-an-interactive-link-for-your-artboard).\
   ![](assets/shared-links-xd-350x870.png)

1. Fai clic su **[!UICONTROL Carica]**.

   Il documento viene visualizzato nel [!UICONTROL Documenti] nell’area del plug-in e nell’app desktop.

   >[!IMPORTANT]
   >
   >Gli utenti devono avere accesso al [!UICONTROL Visualizzatore di correzione del desktop] per rivedere e approvare le bozze interattive. Per ulteriori informazioni, consulta [Installa il [!UICONTROL Visualizzatore di correzione del desktop]](../../review-and-approve-work/proofing/use-the-desktop-proofing-viewer/installing-desktop-proofing-viewer.md).

## Carica una nuova versione di prova

Puoi caricare una nuova versione di una bozza. Il plug-in ricorda il flusso di lavoro di correzione impostato sulla versione precedente, ma puoi modificarlo se lo desideri.

1. Fai clic sul pulsante **[!UICONTROL Menu]** nell&#39;angolo in alto a destra, quindi seleziona **[!UICONTROL Elenco lavori]**. È inoltre possibile utilizzare il menu per passare agli oggetti principali.

   ![](assets/menu-350x440.png)

1. Vai all&#39;elemento di lavoro in cui devi caricare un documento.
1. Fai clic sul pulsante **[!UICONTROL Documento]** icona ![](assets/documents.png)nella barra di navigazione.

1. Fai clic su **[!UICONTROL Nuova versione]** vicino al fondo del plugin.
1. Abilita **[!UICONTROL Creare una bozza]**.
1. Selezionate le tavole da disegno da caricare.

   >[!NOTE]
   >
   >Se desideri caricare una nuova versione di un file .svg, .png o .jpg, puoi caricare una sola tavola da disegno.

1. Scegliere il tipo di approvazione della bozza desiderato:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Basic]: </td> 
      <td> <p>I processi di approvazione di base sono ad hoc e possono includere diversi revisori in base alle esigenze: </p> 
       <ul> 
        <li> <p>(Facoltativo) Aggiungi <strong>Approvatori</strong> nella scatola.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Automatizzato]</td> 
      <td> <p>I processi di approvazione automatizzata sono precompilati dagli amministratori e includono revisori e fasi specifici. Per ulteriori informazioni, consulta <a href="../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Panoramica del flusso di lavoro automatizzato</a>.</p> 
       <ul> 
        <li> <p>Scegli un modello di flusso di lavoro dal menu a discesa.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Scegli il formato di esportazione dal **[!UICONTROL Tipo di risorsa]** menu a discesa.

   ![](assets/create-a-proof-xd-350x202.png)

1. (Facoltativo) Digita un commento nella sezione **[!UICONTROL Aggiornamenti]** area.

   ![](assets/proof-approvals-xd-350x396.png)

1. (Facoltativo) Se selezionate PDF come tipo di risorsa e selezionate più tavole da disegno, scegliete se esportare le tavole da disegno come **[!UICONTROL File PDF singolo]s** o **M[!UICONTROL più file PDF]**.

1. (Facoltativo) Denomina il PDF.

   ![](assets/pdf-options.png)

1. Fai clic su **[!UICONTROL Carica]**.\
   Il documento viene visualizzato nel [!UICONTROL Documenti] nell’area del plug-in e nell’app desktop.
