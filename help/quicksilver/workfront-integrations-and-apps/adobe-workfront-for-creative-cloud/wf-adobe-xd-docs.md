---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: Carica tavole da disegno di XD come documenti in Workfront
description: Potete caricare le vostre tavole da disegno come documenti per una rapida revisione e approvazione o semplicemente per archiviarle in Adobe Workfront.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: 710035f7-339c-457c-b9b0-e51bc0e0061d
source-git-commit: a65a4568c6428768ee6bc60a59a8499efdbec9f8
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 1%

---


# Carica [!DNL XD] tavole da disegno come documenti in [!DNL Workfront]

Puoi caricare le tue tavole da disegno come documenti per una revisione e approvazione rapida o semplicemente per archiviarle in [!DNL Adobe Workfront].

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <!-- <td role="rowheader">[!DNL Adobe Workfront] package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td> 
   <p>Standard</p>
   <p>Work or higher</p> </td> 
  </tr> 
  <tr> -->
   <td role="rowheader">Prodotti aggiuntivi</td> 
   <td>È necessario disporre di una licenza [!DNL Adobe Creative Cloud] oltre a una licenza [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica accesso a [!UICONTROL Documents]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Accesso di [!UICONTROL View] o versione successiva all'oggetto in cui si desidera caricare un documento.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

* È necessario installare il plug-in [!DNL Adobe Workfront for XD] prima di caricare le bacheche XD art come documenti in Workfront.

Per istruzioni, vedere [Installa [!DNL Adobe Workfront for XD]](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-adobe-xd-install.md).

## Aggiungi un nuovo documento

1. Fai clic sull&#39;icona **[!UICONTROL Menu]** in alto a destra, quindi seleziona **[!UICONTROL Elenco lavori]**. È inoltre possibile utilizzare il menu per passare agli oggetti padre.

   ![Icona menu](assets/menu-350x440.png)

1. Passare all&#39;elemento di lavoro in cui si desidera caricare un documento.
1. Fai clic sull&#39;icona **[!UICONTROL Documento]** ![Icona documento](assets/documents.png) nella barra di navigazione.

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
      <td role="rowheader">JPG</td>
      <td>Le tavole da disegno vengono caricate come JPG nella scheda [!UICONTROL Documents] dell'elemento di lavoro in [!DNL Workfront]. <br></td>
     </tr>
     <tr>
      <td role="rowheader">SVG</td>
      <td>Le tavole da disegno vengono caricate come SVG nella scheda [!UICONTROL Documents] dell'elemento di lavoro in [!DNL Workfront]. </td>
     </tr>
     <tr>
      <td role="rowheader">PDF</td>
      <td>Scegli se vuoi che le tavole da disegno selezionate vengano caricate come <strong>singolo file PDF</strong> o <strong>più file PDF</strong>. Le tavole da disegno vengono caricate come PDF nella scheda [!UICONTROL Documents] dell'elemento di lavoro in [!DNL Workfront].</td>
     </tr>
    </tbody>
   </table>


1. Fai clic su **[!UICONTROL Carica]**.\
   Il documento verrà visualizzato nell&#39;area [!UICONTROL Documenti] del plug-in e dell&#39;app desktop.

## Aggiungi una nuova versione

1. Fai clic sull&#39;icona **[!UICONTROL Menu]** in alto a destra, quindi seleziona **[!UICONTROL Elenco lavori]**. È inoltre possibile utilizzare il menu per passare agli oggetti padre.

   ![Icona menu](assets/menu-350x440.png)

1. Passare all&#39;elemento di lavoro in cui si desidera caricare un documento.
1. Fai clic sull&#39;icona **[!UICONTROL Documento]** ![Icona documento](assets/documents.png)nella barra di navigazione.

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
      <td role="rowheader">JPG</td>
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
