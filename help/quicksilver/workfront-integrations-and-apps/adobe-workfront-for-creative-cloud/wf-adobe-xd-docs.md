---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: Carica tavole da disegno XD come documenti in Workfront
description: Potete caricare le vostre tavole da disegno come documenti per una rapida revisione e approvazione o semplicemente per archiviarle in Adobe Workfront.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: 710035f7-339c-457c-b9b0-e51bc0e0061d
source-git-commit: 4256e1ecd16179d0a2aa8e623b05be754d8bbd2d
workflow-type: tm+mt
source-wordcount: '588'
ht-degree: 0%

---


# Carica [!DNL XD] tavole da disegno come documenti in [!DNL Workfront]

Puoi caricare le tue tavole da disegno come documenti per una revisione e approvazione rapida o semplicemente per archiviarle in [!DNL Adobe Workfront].

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <!-- <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Work] or [!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> -->
   <td role="rowheader">Prodotto</td> 
   <td>È necessario disporre di una licenza [!DNL Adobe Creative Cloud] oltre a una licenza [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modifica accesso a [!UICONTROL Documents]</p> <p>Nota: se non disponi ancora dell'accesso, chiedi all'amministratore [!DNL Workfront] se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di [!DNL Workfront] può modificare il tuo livello di accesso, vedi <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Accesso di [!UICONTROL View] o versione successiva all'oggetto in cui si desidera caricare un documento.</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore [!DNL Workfront].

+++

## Prerequisiti

* È necessario installare il plug-in [!DNL Adobe Workfront for XD] prima di caricare le bacheche grafiche XD come documenti in Workfront.

Per istruzioni, vedere [Installa [!DNL Adobe Workfront for XD]](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-adobe-xd-install.md).

## Aggiungi un nuovo documento

1. Fai clic sull&#39;icona **[!UICONTROL Menu]** in alto a destra, quindi seleziona **[!UICONTROL Elenco lavori]**. È inoltre possibile utilizzare il menu per passare agli oggetti padre.

   ![](assets/menu-350x440.png)

1. Passare all&#39;elemento di lavoro in cui si desidera caricare un documento.
1. Fai clic sull&#39;icona ![](assets/documents.png) del **[!UICONTROL Documento]** nella barra di navigazione.

1. Fai clic su **[!UICONTROL Nuovo file]** nella parte inferiore del plug-in.
1. Selezionate la tavola da disegno da caricare.

   >[!TIP]
   >
   >Per selezionare più tavole da disegno, fate clic e trascinate il mouse sulle tavole da disegno desiderate.
1. (Facoltativo) Digita un commento nell&#39;area **[!UICONTROL Aggiornamenti]**.
1. Scegli il **[!UICONTROL Tipo risorsa]** dal menu a discesa:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td colspan="2" role="rowheader">[!UICONTROL Export Format]</td>
     </tr>
     <tr>
      <td role="rowheader">PNG</td>
      <td>Le tavole da disegno vengono caricate come file PNG nella scheda [!UICONTROL Documents] dell'elemento di lavoro in [!DNL Workfront]. </td>
     </tr>
     <tr>
      <td role="rowheader">JPG-</td>
      <td>Le tavole da disegno vengono caricate come JPG nella scheda [!UICONTROL Documents] dell'elemento di lavoro in [!DNL Workfront]. <br></td>
     </tr>
     <tr>
      <td role="rowheader">SVG</td>
      <td>Le tavole da disegno vengono caricate come SVG nella scheda [!UICONTROL Documents] dell'elemento di lavoro in [!DNL Workfront]. </td>
     </tr>
     <tr>
      <td role="rowheader">PDF</td>
      <td>Scegli se vuoi che le tavole da disegno selezionate vengano caricate come <strong>file PDF singolo</strong> o <strong>più file PDF</strong>. Le tavole da disegno vengono caricate come PDF nella scheda [!UICONTROL Documents] dell'elemento di lavoro in [!DNL Workfront].</td>
     </tr>
    </tbody>
   </table>


1. Fai clic su **[!UICONTROL Carica]**.\
   Il documento verrà visualizzato nell&#39;area [!UICONTROL Documenti] del plug-in e dell&#39;app desktop.

## Aggiungi una nuova versione

1. Fai clic sull&#39;icona **[!UICONTROL Menu]** in alto a destra, quindi seleziona **[!UICONTROL Elenco lavori]**. È inoltre possibile utilizzare il menu per passare agli oggetti padre.

   ![](assets/menu-350x440.png)

1. Passare all&#39;elemento di lavoro in cui si desidera caricare un documento.
1. Fai clic sull&#39;icona **[!UICONTROL Documento]** ![](assets/documents.png)nella barra di navigazione.

1. Fare clic sul documento a cui si desidera aggiungere una nuova versione.
1. Fai clic su **[!UICONTROL Nuova versione]** nella parte inferiore del plug-in.
1. Selezionate le tavole da disegno da caricare.

   >[!NOTE]
   >
   >Se desiderate caricare una nuova versione di un SVG, PNG o JPG, potete caricare una sola tavola da disegno.

1. (Facoltativo) Digita un commento nell&#39;area **[!UICONTROL Aggiornamenti]**.

1. Scegli il **[!UICONTROL Tipo risorsa]** dal menu a discesa:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td colspan="2" role="rowheader">Formato di esportazione</td>
     </tr>
     <tr>
      <td role="rowheader">PNG</td>
      <td>La tavola da disegno viene caricata come file PNG nella scheda [!UICONTROL Documents] dell'elemento di lavoro in [!DNL Workfront]. </td>
     </tr>
     <tr>
      <td role="rowheader">JPG-</td>
      <td>La tavola da disegno viene caricata come JPG nella scheda [!UICONTROL Documents] dell'elemento di lavoro in [!DNL Workfront]. <br></td>
     </tr>
     <tr>
      <td role="rowheader">SVG</td>
      <td>La tavola da disegno viene caricata come SVG nella scheda [!UICONTROL Documents] dell'elemento di lavoro in [!DNL Workfront]. </td>
     </tr>
     <tr>
      <td role="rowheader">PDF</td>
      <td><p>Le tavole da disegno vengono caricate come PDF nella scheda [!UICONTROL Documents] dell'elemento di lavoro in [!DNL Workfront].</p>
      <p><strong>Nota</strong>: è possibile caricare una sola tavola da disegno per una nuova versione del documento.</p>
      </td>
     </tr>
    </tbody>
   </table>

1. Fai clic su **[!UICONTROL Carica]**.\
   Il documento verrà visualizzato nell&#39;area [!UICONTROL Documenti] del plug-in e dell&#39;app desktop.
