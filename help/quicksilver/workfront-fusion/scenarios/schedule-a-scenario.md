---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Pianificare uno scenario in Adobe Workfront Fusion
description: Per impostazione predefinita, uno scenario viene eseguito ogni 15 minuti. È possibile modificare questa impostazione definendo quando e con quale frequenza viene eseguito uno scenario attivato.
author: Becky
feature: Workfront Fusion
exl-id: bce89abe-ec37-4705-a88f-de62c8b27f49
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 1%

---

# Pianifica uno scenario in [!DNL Adobe Workfront Fusion]

Per impostazione predefinita, uno scenario viene eseguito ogni 15 minuti. È possibile modificare questa impostazione definendo quando e con quale frequenza viene eseguito uno scenario attivato.

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
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p><p>[!UICONTROL [!DNL Workfront Fusion] per automazione del lavoro </p>  </td>    </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</td> 
  </tr> 
 </tbody> 
</table>

Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, vedi [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Pianificare uno scenario

1. Nell&#39;angolo in alto a destra della pagina dei dettagli Scenario, fai clic su **[!UICONTROL Opzioni]** > **[!UICONTROL Pianificazione]**

   Oppure

   Fai clic sul pulsante **[!UICONTROL Pianificazione]** icona (orologio) nel modulo trigger dello scenario.

1. Immetti le informazioni nei campi seguenti:

   <table style="table-layout:auto">   
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Esegui scenario]</td> 
      <td> <p>Selezionare la frequenza alla quale si desidera eseguire lo scenario, quindi selezionare l'intervallo.</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL A intervalli regolari]</strong> </p> <p>Immettere il numero di minuti tra le esecuzioni. Il valore predefinito è 15 minuti.</p> </li> 
        <li> <p><strong>[!UICONTROL Una Volta]</strong> </p> <p>Immettere la data e l'ora in cui si desidera eseguire lo scenario. Usa il formato <code>MM/DD/YYYY h:mm A</code>. Esempio: <code>06/25/2019 11:00 PM</code>.</p> </li> 
        <li> <p><strong>[!UICONTROL Ogni giorno]</strong> </p> <p>Immettere l'ora in cui si desidera eseguire lo scenario. Usa il formato <code>h:mm A</code>. Esempio: <code>11:00 PM</code>.</p> </li> 
        <li> <p><strong>[!UICONTROL Giorni della settimana]</strong> </p> <p>Giorni: Selezionare i giorni della settimana in cui si desidera eseguire lo scenario. Puoi selezionare uno o più giorni.</p> <p>Ora: Immettere l'ora in cui si desidera eseguire lo scenario nei giorni selezionati. Usa il formato <code>h:mm A</code>. Esempio: <code>11:00 PM</code></p> </li> 
        <li> <p><strong>[!UICONTROL Giorni del mese]</strong> </p> <p>Giorni: Selezionare i giorni del mese in cui si desidera eseguire lo scenario. Puoi selezionare uno o più giorni.</p> <p>Ora: Immettere l'ora in cui si desidera eseguire lo scenario nei giorni selezionati. Usa il formato <code>h:mm A</code>. Esempio: <code>11:00 PM</code></p> </li> 
        <li> <p><strong>[!UICONTROL Date specificate]</strong> </p> <p>Mesi: Selezionare i mesi che si desidera eseguire lo scenario. Puoi selezionare uno o più mesi.</p> <p>Giorni: Selezionare i giorni del mese in cui si desidera eseguire lo scenario. Puoi selezionare uno o più giorni.</p> <p>Ora: Immettere l'ora in cui si desidera eseguire lo scenario nei giorni selezionati. Usa il formato <code>h:mm A</code>. Esempio: <code>11:00 PM</code></p> </li> 
       </ul> <p>Nota: Deve esistere una data per l'esecuzione di uno scenario in quella data. Ad esempio, uno scenario pianificato solo per il 31° del mese non verrà eseguito nei mesi di febbraio, aprile, giugno, settembre o novembre, in quanto tali mesi non hanno un 31° giorno.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Pianificazione avanzata]</td> 
      <td>È possibile definire intervalli di tempo specifici durante i quali eseguire lo scenario. È possibile specificare intervalli di tempo, giorni feriali o mesi. Per ogni intervallo, fai clic su <strong>[!UICONTROL Aggiungi]</strong> e compila i campi come descritto nel campo [!UICONTROL Run scenario] .</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Start]</td> 
      <td>Immettere la data e l'ora dopo le quali si desidera eseguire lo scenario. Usa il formato <code>MM/DD/YYYY h:mm A</code>. Esempio: <code>06/25/2019 11:00 PM</code>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL End]</td> 
      <td>Immettere la data e l'ora prima della quale si desidera eseguire lo scenario. Usa il formato <code>MM/DD/YYYY h:mm A</code>. Esempio: <code>06/25/2019 11:00 PM</code>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **[!UICONTROL OK]** per salvare le impostazioni di pianificazione e tornare allo scenario.
