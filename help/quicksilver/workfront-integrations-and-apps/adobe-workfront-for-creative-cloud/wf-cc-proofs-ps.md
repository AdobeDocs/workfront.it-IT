---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: Caricare bozze da Adobe Photoshop
description: Puoi caricare le tue tavole da disegno come bozze direttamente in Adobe Workfront per una revisione e un'approvazione complete.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: cbb12ee7-949e-44a1-9340-3ef93c003b21
source-git-commit: ab523ea5136b11a3ee1b6fa5746a1165f4b9d397
workflow-type: tm+mt
source-wordcount: '596'
ht-degree: 0%

---

# Carica bozze da [!DNL Photoshop]

Puoi caricare le tue tavole da disegno come bozze direttamente in [!DNL Adobe Workfront] per un esame e un&#39;approvazione approfonditi.

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

&#42;Per informazioni sul piano, il ruolo o il profilo delle autorizzazioni di prova, contattare l&#39;amministratore Workfront o Workfront Proof.

## Prerequisiti

* È necessario installare [!DNL Adobe Workfront for Photoshop] plugin prima di poter caricare le bozze da [!DNL Adobe Photoshop].

   Per istruzioni, consulta [Installa [!DNL Adobe Workfront for Photoshop]](../../workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-ps.md).

## Carica una bozza di base

1. Fai clic sul pulsante **[!UICONTROL Menu]** nell&#39;angolo in alto a destra, quindi seleziona **[!UICONTROL Elenco lavori]**. È inoltre possibile utilizzare il menu per passare agli oggetti principali.

   ![](assets/go-back-to-work-list-350x314.png)

1. Passa all’elemento di lavoro in cui desideri caricare una bozza.
1. Fai clic sul pulsante **[!UICONTROL Documento]** icona ![](assets/documents.png) nella barra di navigazione.
1. Fai clic su **[!UICONTROL Nuovo file]** vicino al fondo del plugin.
1. Abilita la **[!UICONTROL Creare una bozza]** alternare.
1. Scegli la **[!UICONTROL Tipo di risorsa]** dal menu a discesa.

   ![](assets/plugin-create-proof-350x182.png)

1. In **[!UICONTROL Approvazioni di prova]** sezione , seleziona **[!UICONTROL Base]**.
1. (Facoltativo) Aggiungi approvatori.
1. (Facoltativo) Digita un commento nella sezione **[!UICONTROL Aggiornamenti]** area.

   ![](assets/plugin-proof-approvals-350x450.png)

1. (Facoltativo) Digita un nome per la bozza in**[!UICONTROL Nome della bozza]** casella di testo.
1. (Facoltativo) Seleziona **[!UICONTROL Aggiungi file esterno]** per aggiungere un file dal computer.
1. Fai clic su **[!UICONTROL Carica]**.

   ![](assets/plugin-files-350x307.png)\
   Il documento viene visualizzato nel [!UICONTROL Documenti] nell’area del plug-in e nell’app desktop.

## Caricare una bozza automatica

1. Fai clic sul pulsante **[!UICONTROL Menu]** nell&#39;angolo in alto a destra, quindi seleziona **[!UICONTROL Elenco lavori]**. È inoltre possibile utilizzare il menu per passare agli oggetti principali.

   ![](assets/go-back-to-work-list-350x314.png)

1. Passa all’elemento di lavoro in cui desideri caricare una bozza.
1. Fai clic sul pulsante **[!UICONTROL Documento]** icona ![](assets/documents.png) nella barra di navigazione.

1. Fai clic su **[!UICONTROL Nuovo file]** vicino al fondo del plugin.
1. Abilita la **[!UICONTROL Creare una bozza]** seleziona , quindi **[!UICONTROL Tipo di risorsa]** dal menu a discesa.

   ![](assets/plugin-create-proof-350x182.png)

1. In **[!UICONTROL Approvazioni di prova]** sezione , seleziona **[!UICONTROL Automatico]**.
1. (Facoltativo) In **[!UICONTROL Modello di flusso di lavoro]** digitare il nome di un modello di flusso di lavoro della bozza.

<!-- {{adjust-proof-settings}} -->

1. (Facoltativo) Digita un commento nella sezione **[!UICONTROL Aggiornamenti]** area.

   ![](assets/copy-of-proof-approvals-advanced-350x424.png) <!--new screenshot -->

1. (Facoltativo) Digita un nome per la bozza nella **[!UICONTROL Nome della bozza]** casella di testo.
1. (Facoltativo) Seleziona **[!UICONTROL Aggiungi file esterno]** per aggiungere un file dal computer.
1. Fai clic su **[!UICONTROL Carica]**.

   ![](assets/plugin-files-350x307.png)\
   Il documento viene visualizzato nel [!UICONTROL Documenti] nell’area del plug-in e nell’app desktop.

## Carica una nuova versione di prova

Puoi caricare una nuova versione di una bozza. Il plug-in ricorda il flusso di lavoro di correzione impostato sulla versione precedente, ma puoi modificarlo se lo desideri.

1. Fai clic sul pulsante **[!UICONTROL Menu]** nell&#39;angolo in alto a destra, quindi seleziona **[!UICONTROL Elenco lavori]**. È inoltre possibile utilizzare il menu per passare agli oggetti principali.

   ![](assets/go-back-to-work-list-350x314.png)

1. Vai all&#39;elemento di lavoro in cui devi caricare un documento.
1. Fai clic sul pulsante **[!UICONTROL Documento]** icona ![](assets/documents.png)nella barra di navigazione.

1. Fai clic su **[!UICONTROL Nuova versione]** vicino al fondo del plugin..
1. Scegli la **[!UICONTROL Tipo di risorsa]** dal menu a discesa.
1. Abilita la **[!UICONTROL Creare una bozza]** seleziona , quindi **[!UICONTROL Tipo di risorsa]** dal menu a discesa.

   ![](assets/plugin-create-proof-350x182.png)

1. In **[!UICONTROL Prove di omologazione]** sezione, scegli **[!UICONTROL Base]** o **[!UICONTROL Automatico]**.

1. Aggiungi **[!UICONTROL Revisori]** o **[!UICONTROL Modello di flusso di lavoro]** in base al tipo di approvazione selezionato al punto 7.

1. (Facoltativo) Digita un commento nella sezione **[!UICONTROL Aggiornamenti]** area.
1. Fai clic su **[!UICONTROL Carica]**.\
   Il documento viene visualizzato nel [!UICONTROL Documenti] nell’area del plug-in e nell’app desktop.
