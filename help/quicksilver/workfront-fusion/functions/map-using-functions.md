---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Mappare gli elementi utilizzando le funzioni in [!DNL Adobe Workfront Fusion]
description: Quando mappi elementi, puoi utilizzare le funzioni per creare formule semplici o complesse.
author: Becky
feature: Workfront Fusion
exl-id: e64d9b1e-8576-43db-ac29-0d386a482fbc
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '488'
ht-degree: 0%

---

# Mappare gli elementi utilizzando le funzioni in [!DNL Adobe Workfront Fusion]

Quando mappi elementi, puoi utilizzare le funzioni per creare formule semplici o complesse.

Le funzioni disponibili in [!DNL Adobe Workfront Fusion] sono simili alle funzioni in Excel e in alcuni linguaggi di programmazione. Valutano logica generale, matematica, testo, date e array. Consentono di eseguire logiche condizionali e trasformazioni di valori di elementi, ad esempio conversione di un testo in maiuscolo, taglio di testo, conversione di una data in un formato diverso e altro ancora. Per ulteriori informazioni, consulta [Mappare le informazioni da un modulo all&#39;altro in Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p><p>[!UICONTROL [!DNL Workfront Fusion] per automazione del lavoro</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</td> 
  </tr> 
 </tbody> 
</table>

Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, vedi [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Inserisci funzioni nei campi

Se fai clic su un campo, la [!UICONTROL mappatura] viene visualizzato il pannello . Il pannello di mappatura contiene diverse schede:

![](assets/functions-toolbar-350x189.png)

La prima scheda ![](assets/toolbar-icon-functions-you-map-from-other-modules.png) (mostrato all’apertura del pannello) mostra gli elementi che è possibile mappare da altri moduli.

Le altre schede contengono i seguenti tipi di funzioni:

* **Funzioni generali** ![](assets/toolbar-icon-general-function.png) - Vedi [Funzioni generali in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/general-functions.md) per ulteriori informazioni.

* **Funzioni matematiche** ![](assets/toolbar-icon-math-functions.png) - Vedi [Funzioni matematiche in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/math-functions.md) per ulteriori informazioni.

* **Funzioni di testo e binarie** ![](assets/toolbar-icon-text&binary-functions.png) - Vedi [Funzioni stringa in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/string-functions.md) per ulteriori informazioni.

* **Data e ora** ![](assets/toolbar-icon-date&time-functions.png) - Vedi [Funzioni di data e ora in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/date-and-time-functions.md) e gli articoli seguenti per ulteriori informazioni.

   * [Token per la formattazione di data e ora in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md)
   * [Token per l’analisi di data e ora in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-parsing.md)

* **Funzioni per l’utilizzo degli array** ![](assets/toolbar-icon-functions-for-arrays.png) - Vedi [Funzioni array in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/array-functions.md) per ulteriori informazioni.

Per inserire una funzione in un campo:

1. Fare clic sul nome della funzione.

   Oppure

   Trascina la funzione nel campo .

>[!INFO]
>
>**Esempio:** Alcuni tipi di dati impediscono agli utenti di immettere più di un certo numero di caratteri. È possibile utilizzare la funzione sottostringa per limitare un valore a un determinato numero di caratteri.
>
>In questo esempio, la funzione sottostringa limita il nome del progetto a 50 caratteri.
>
>![](assets/example-meet-length-restriction-350x184.png)

## Funzioni di nidificazione

È possibile nidificare le funzioni tra loro.

## Utilizzo [!DNL Google Sheets] Funzioni

Se [!DNL Workfront Fusion] non presenta una funzione che desideri utilizzare, ma è disponibile da [!DNL Google Sheets], puoi utilizzarlo seguendo questi passaggi:

1. In [!DNL Google Sheets], crea un nuovo foglio di calcolo vuoto.
1. In [!DNL Workfront Fusion], apri lo scenario.
1. Aggiungi il **[!DNL Google Sheets]** >**[!UICONTROL Aggiornare una cella]** allo scenario.

   Per istruzioni sull’aggiunta di un modulo, consulta [Aggiungere un modulo in uno scenario](../../workfront-fusion/scenarios/create-a-scenario.md#add) nell&#39;articolo [Crea uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. Configura il modulo:

   1. Scegli il foglio di calcolo appena creato nel **[!UICONTROL Foglio di calcolo]** campo .
   1. Inserisci la formula contenente [!DNL Google Sheets] nella **[!UICONTROL Valore]** campo .

      È possibile utilizzare come di consueto l’output dei moduli precedenti.

      ![](assets/exploit-google-sheet-functions-350x218.png)

1. Inserisci **[!UICONTROL Fogli Google] >[!UICONTROL Cella]** modulo per ottenere il risultato calcolato.
1. Configura il modulo utilizzando lo stesso ID cella utilizzato al passaggio 4.

   ![](assets/exploit-google-sheet-functions-2-350x187.png)
