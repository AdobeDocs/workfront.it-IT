---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Mappare gli elementi utilizzando le funzioni in [!DNL Adobe Workfront Fusion]
description: Quando mappate gli elementi, potete utilizzare le funzioni per creare formule semplici o complesse.
author: Becky
feature: Workfront Fusion
exl-id: e64d9b1e-8576-43db-ac29-0d386a482fbc
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '532'
ht-degree: 0%

---

# Mappare gli elementi utilizzando le funzioni in [!DNL Adobe Workfront Fusion]

Quando mappate gli elementi, potete utilizzare le funzioni per creare formule semplici o complesse.

Le funzioni disponibili in [!DNL Adobe Workfront Fusion] sono simili alle funzioni in Excel e in alcuni linguaggi di programmazione. Valutano logica generale, matematica, testo, date e array. Consentono di eseguire logica condizionale e trasformazioni dei valori degli elementi, ad esempio la conversione di un testo in maiuscolo, il ritaglio del testo, la conversione di una data in un formato diverso e altro ancora. Per ulteriori informazioni, consulta [Mappare le informazioni da un modulo all’altro in Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

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
   <p>Fabbisogno di licenza corrente: No [!DNL Workfront Fusion] requisito di licenza.</p>
   <p>Oppure</p>
   <p>Requisito licenza legacy: [!UICONTROL [!DNL Workfront Fusion] per l'automazione e l'integrazione del lavoro] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>
   <p>Fabbisogno prodotto corrente: se si dispone di [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront] Pianifica, la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare la funzionalità descritta in questo articolo. [!DNL Workfront Fusion] è incluso in [!UICONTROL Ultimate] [!DNL Workfront] piano.</p>
   <p>Oppure</p>
   <p>Requisiti del prodotto legacy: la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare la funzionalità descritta in questo articolo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, consulta [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Inserisci funzioni nei campi

Se si fa clic su un campo, la [!UICONTROL mappatura] viene visualizzato il pannello. Il pannello di mappatura contiene diverse schede:

![](assets/functions-toolbar-350x189.png)

La prima scheda ![](assets/toolbar-icon-functions-you-map-from-other-modules.png) (mostrato all’apertura del pannello) mostra gli elementi che è possibile mappare da altri moduli.

Le altre schede contengono i seguenti tipi di funzioni:

* **Funzioni generali** ![](assets/toolbar-icon-general-function.png) - Consulta [Funzioni generali in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/general-functions.md) per ulteriori informazioni.

* **Funzioni matematica** ![](assets/toolbar-icon-math-functions.png) - Consulta [Funzioni matematiche in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/math-functions.md) per ulteriori informazioni.

* **Funzioni di testo e binarie** ![](assets/toolbar-icon-text&binary-functions.png) - Consulta [Funzioni stringa in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/string-functions.md) per ulteriori informazioni.

* **Data e ora** ![](assets/toolbar-icon-date&time-functions.png) - Consulta [Funzioni data e ora in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/date-and-time-functions.md) e gli articoli seguenti per ulteriori informazioni.

   * [Token per la formattazione di data e ora in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md)
   * [Token per l’analisi di data e ora in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-parsing.md)

* **Funzioni per l&#39;utilizzo degli array** ![](assets/toolbar-icon-functions-for-arrays.png) - Consulta [Funzioni array in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/array-functions.md) per ulteriori informazioni.

Per inserire una funzione in un campo:

1. Fare clic sul nome della funzione.

   Oppure

   Trascina la funzione nel campo.

>[!INFO]
>
>**Esempio:** Alcuni tipi di dati impediscono agli utenti di immettere più di un determinato numero di caratteri. Puoi utilizzare la funzione di sottostringa per limitare un valore a un determinato numero di caratteri.
>
>In questo esempio, la funzione di sottostringa limita il nome del progetto a 50 caratteri.
>
>![](assets/example-meet-length-restriction-350x184.png)

## Nidificazione delle funzioni

È possibile nidificare le funzioni l&#39;una nell&#39;altra.

## Utilizzare [!DNL Google Sheets] funzioni

Se [!DNL Workfront Fusion] non presenta una funzione che desideri utilizzare, ma è caratterizzata da [!DNL Google Sheets], è possibile utilizzarlo seguendo questi passaggi:

1. In entrata [!DNL Google Sheets], crea un nuovo foglio di calcolo vuoto.
1. In entrata [!DNL Workfront Fusion], apri lo scenario.
1. Aggiungi il **[!DNL Google Sheets]** >**[!UICONTROL Aggiornare una cella]** allo scenario.

   Per istruzioni sull’aggiunta di un modulo, consulta [Aggiungere un modulo in uno scenario](../../workfront-fusion/scenarios/create-a-scenario.md#add) nell’articolo [Creare uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. Configura il modulo:

   1. Scegli il nuovo foglio di calcolo creato in **[!UICONTROL Foglio di calcolo]** campo.
   1. Inserire la formula contenente [!DNL Google Sheets] funzioni in **[!UICONTROL Valore]** campo.

      Puoi utilizzare come di consueto l’output dei moduli precedenti.

      ![](assets/exploit-google-sheet-functions-350x218.png)

1. Inserisci il **[!UICONTROL Fogli Google] >[!UICONTROL Ottieni una cella]** per ottenere il risultato calcolato.
1. Configura il modulo utilizzando lo stesso ID cella utilizzato nel passaggio 4.

   ![](assets/exploit-google-sheet-functions-2-350x187.png)
