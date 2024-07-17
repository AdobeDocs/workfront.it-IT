---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Pianificazione di uno scenario in Adobe Workfront Fusion
description: Per impostazione predefinita, uno scenario viene eseguito ogni 15 minuti. Puoi modificare questa impostazione definendo quando e con quale frequenza viene eseguito uno scenario attivato.
author: Becky
feature: Workfront Fusion
exl-id: bce89abe-ec37-4705-a88f-de62c8b27f49
source-git-commit: f5549be5951a2648d6a77d25bebbd4141f18d36c
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 0%

---

# Pianifica uno scenario in [!DNL Adobe Workfront Fusion]

Per impostazione predefinita, uno scenario viene eseguito ogni 15 minuti. Puoi modificare questa impostazione definendo quando e con quale frequenza viene eseguito uno scenario attivato. È possibile pianificare l&#39;esecuzione di scenari di fusione ogni 5 minuti.

## Requisiti di accesso

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto">   
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] piano*</td> 
   <td> <p>[!DNL Pro] o superiore</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza [!UICONTROL Adobe Workfront Fusion]**</td> 
  <td>
   <p>Requisiti di licenza correnti: nessun requisito di licenza [!DNL Workfront Fusion].</p>
   <p>Oppure</p>
   <p>Requisito licenza legacy: [!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione lavoro], [!UICONTROL [!DNL Workfront Fusion] per automazione lavoro]</p>
   </td>    </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>
   <p>Fabbisogno prodotto corrente: se si dispone del piano [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront], l'organizzazione deve acquistare [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo. [!DNL Workfront Fusion] è incluso nel piano [!UICONTROL Ultimate] [!DNL Workfront].</p>
   <p>Oppure</p>
   <p>Requisiti del prodotto legacy: la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Per conoscere il piano, il tipo di licenza o l&#39;accesso disponibili, contattare l&#39;amministratore [!DNL Workfront].

Per informazioni sulle [!DNL Adobe Workfront Fusion] licenze, vedere [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Pianificare uno scenario

1. Nell&#39;angolo superiore destro della pagina dei dettagli Scenario, fare clic su **[!UICONTROL Opzioni]** > **[!UICONTROL Pianificazione]**

   Oppure

   Fai clic sull&#39;icona **[!UICONTROL Pianificazione]** (orologio) nel modulo di attivazione dello scenario.

1. Immettere le informazioni nei campi seguenti:

   <table style="table-layout:auto">   
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Run scenario]</td> 
      <td> <p>Seleziona la frequenza con cui desideri eseguire lo scenario, quindi seleziona l’intervallo.</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL A intervalli regolari]</strong> </p> <p>Immetti il numero di minuti tra le esecuzioni. Il valore predefinito è 15 minuti.</p> </li> 
        <li> <p><strong>[!UICONTROL Once]</strong> </p> <p>Inserire la data e l'ora in cui si desidera eseguire lo scenario. Utilizza il formato <code>MM/DD/YYYY h:mm A</code>. Esempio: <code>06/25/2019 11:00 PM</code>.</p> </li> 
        <li> <p><strong>[!UICONTROL Ogni giorno]</strong> </p> <p>Immettere l'ora in cui si desidera eseguire lo scenario. Utilizza il formato <code>h:mm A</code>. Esempio: <code>11:00 PM</code>.</p> </li> 
        <li> <p><strong>[!UICONTROL Giorni della settimana]</strong> </p> <p>Giorni: selezionare i giorni della settimana in cui si desidera eseguire lo scenario. Puoi selezionare uno o più giorni.</p> <p>Tempo: inserire l'ora in cui si desidera eseguire lo scenario nei giorni selezionati. Utilizza il formato <code>h:mm A</code>. Esempio: <code>11:00 PM</code></p> </li> 
        <li> <p><strong>[!UICONTROL Giorni del mese]</strong> </p> <p>Giorni: selezionare i giorni del mese in cui si desidera eseguire lo scenario. Puoi selezionare uno o più giorni.</p> <p>Tempo: inserire l'ora in cui si desidera eseguire lo scenario nei giorni selezionati. Utilizza il formato <code>h:mm A</code>. Esempio: <code>11:00 PM</code></p> </li> 
        <li> <p><strong>[!UICONTROL Date specificate]</strong> </p> <p>Mesi: selezionare i mesi in cui eseguire lo scenario. Puoi selezionare uno o più mesi.</p> <p>Giorni: selezionare i giorni del mese in cui si desidera eseguire lo scenario. Puoi selezionare uno o più giorni.</p> <p>Tempo: inserire l'ora in cui si desidera eseguire lo scenario nei giorni selezionati. Utilizza il formato <code>h:mm A</code>. Esempio: <code>11:00 PM</code></p> </li> 
       </ul> <p>Nota: affinché uno scenario venga eseguito in tale data, è necessario che esista una data. Ad esempio, uno scenario pianificato solo per il 31 del mese non verrà eseguito in febbraio, aprile, giugno, settembre o novembre, perché tali mesi non hanno un giorno 31.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Advanced scheduling]</td> 
      <td>Puoi definire intervalli di tempo specifici durante i quali deve essere eseguito lo scenario. È possibile specificare intervalli di tempo, giorni feriali o mesi. Per ogni intervallo, fare clic su <strong>[!UICONTROL Add]</strong> e compilare i campi come descritto nel campo [!UICONTROL Run scenario].</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Start]</td> 
      <td>Immettere la data e l'ora dopo la quale si desidera eseguire lo scenario. Utilizza il formato <code>MM/DD/YYYY h:mm A</code>. Esempio: <code>06/25/2019 11:00 PM</code>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Fine]</td> 
      <td>Inserire la data e l'ora prima delle quali si desidera eseguire lo scenario. Utilizza il formato <code>MM/DD/YYYY h:mm A</code>. Esempio: <code>06/25/2019 11:00 PM</code>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Fare clic su **[!UICONTROL OK]** per salvare le impostazioni della pianificazione e tornare allo scenario.
