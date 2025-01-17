---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Mappa elementi utilizzando le funzioni in [!DNL Adobe Workfront Fusion]
description: La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione. Questo articolo è stato dichiarato obsoleto, ma contiene un collegamento al nuovo articolo che descrive questa funzionalità.
author: Becky
feature: Workfront Fusion
exl-id: e64d9b1e-8576-43db-ac29-0d386a482fbc
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 1%

---

# Mappa elementi utilizzando le funzioni in [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione.
>
>Le informazioni contenute in questo articolo sono ora disponibili nell’articolo:
>
>* [Mappare un elemento utilizzando le funzioni](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/map-data/map-using-functions.html)
>
>Aggiorna eventuali segnalibri.
>
>Questo articolo non è più in fase di aggiornamento e verrà rimosso nel prossimo futuro.

Quando mappate gli elementi, potete utilizzare le funzioni per creare formule semplici o complesse. Le funzioni disponibili in [!DNL Adobe Workfront Fusion] sono simili a quelle disponibili in Excel e in alcuni linguaggi di programmazione:

* Valutano logica generale, matematica, testo, date e array.
* Consentono di eseguire logica condizionale e trasformazioni dei valori degli elementi, ad esempio la conversione di un testo in maiuscolo, il ritaglio del testo, la conversione di una data in un formato diverso e altro ancora.

Per ulteriori informazioni, vedere [Mappare le informazioni da un modulo all&#39;altro in Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).


## Requisiti di accesso

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto">

<col>  
 <col>  
 <tbody>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront] piano</td>  
   <td> <p>Qualsiasi</p> </td>  
  </tr>  
  <tr data-mc-conditions="">  
   <td role="rowheader">[!DNL Adobe Workfront] licenza</td>  
   <td> <p>Nuovo: [!UICONTROL Standard]</p><p>Oppure</p><p>Corrente: [!UICONTROL Work] o versione successiva</p> </td>  
  </tr>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licenza**</td>  
   <td> 
   <p>Corrente: nessun requisito di licenza [!DNL Workfront Fusion].</p> 
   <p>Oppure</p> 
   <p>Legacy: qualsiasi </p> 
   </td>  
  </tr>  
  <tr>  
   <td role="rowheader">Prodotto</td>  
   <td> 
   <p>Nuovo:</p> <ul><li>Piano [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Workfront]: l'organizzazione deve acquistare [!DNL Adobe Workfront Fusion].</li><li>[!UICONTROL Ultimate] [!DNL Workfront] Il piano [!DNL Workfront Fusion] è incluso.</li></ul> 
   <p>Oppure</p> 
   <p>Corrente: la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion].</p> 
   </td>  
  </tr> 
 </tbody>  
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Per informazioni sulle [!DNL Adobe Workfront Fusion] licenze, vedere [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).


## Panoramica della scheda Mappatura

Per aprire il pannello [!UICONTROL mapping] per un campo:

1. Fai clic su **Scenari** nel pannello a sinistra.
1. Scegli uno scenario.

![](assets/open-functions-bar.png)


### Mappatura delle schede del pannello

Di seguito sono riportate le schede del pannello di mappatura:

* **Funzioni generali** ![](assets/toolbar-icon-general-function.png) - Per ulteriori informazioni, vedere [Funzioni generali in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/general-functions.md).

* **Funzioni matematiche** ![](assets/toolbar-icon-math-functions.png). Per ulteriori informazioni, vedere [Funzioni matematiche in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/math-functions.md).

* **Funzioni testo e binarie** ![](assets/toolbar-icon-text&binary-functions.png). Per ulteriori informazioni, vedere [Funzioni stringa in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/string-functions.md).

* **Data e ora** ![](assets/toolbar-icon-date&time-functions.png) - Per ulteriori informazioni, consulta le [Funzioni data e ora in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/date-and-time-functions.md) e gli articoli seguenti:

   * [Token per la formattazione di data e ora in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md)
   * [Token per l&#39;analisi di data e ora in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-parsing.md)

* **Funzioni per l&#39;utilizzo degli array** ![](assets/toolbar-icon-functions-for-arrays.png). Per ulteriori informazioni, vedere [Funzioni array in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/array-functions.md).

* **Mappa altre funzioni** ![](assets/toolbar-icon-functions-you-map-from-other-modules.png) visualizza gli elementi che è possibile mappare da altri moduli. Questa scheda non è sempre disponibile.

![](assets/functions-toolbar-350x189.png)

## Inserisci funzioni nei campi

Per inserire una funzione in un campo:

1. Fare clic sul nome della funzione.

   Oppure

   Trascina la funzione nel campo.


>[!BEGINSHADEBOX]

**Esempio:** alcuni tipi di dati impediscono agli utenti di immettere più di un determinato numero di caratteri. Puoi utilizzare la funzione di sottostringa per limitare un valore a un determinato numero di caratteri.

In questo esempio, la funzione di sottostringa limita il nome del progetto a 50 caratteri.

![](assets/example-meet-length-restriction-350x184.png)

>[!ENDSHADEBOX]

## Nidificazione delle funzioni

È possibile nidificare le funzioni l&#39;una nell&#39;altra.

## Utilizza le funzioni [!DNL Google Sheets]

Se [!DNL Workfront Fusion] non include una funzione che si desidera utilizzare, ma è disponibile in [!DNL Google Sheets], è possibile utilizzarla eseguendo la procedura seguente:

1. In [!DNL Google Sheets] creare un nuovo foglio di calcolo vuoto.
1. In [!DNL Workfront Fusion], apri lo scenario.
1. Aggiungi il modulo **[!DNL Google Sheets]** >**[!UICONTROL Aggiorna cella]** allo scenario.

   Per istruzioni sull&#39;aggiunta di un modulo, vedere [Aggiungere un modulo in uno scenario](../../workfront-fusion/scenarios/create-a-scenario.md#add) nell&#39;articolo [Creare uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. Configura il modulo:

   1. Scegliere il nuovo foglio di calcolo creato nel campo **[!UICONTROL Foglio di calcolo]**.
   1. Inserire la formula contenente le funzioni [!DNL Google Sheets] nel campo **[!UICONTROL Valore]**.

      Puoi utilizzare come di consueto l’output dei moduli precedenti.

      ![](assets/exploit-google-sheet-functions-350x218.png)

1. Inserire il modulo **[!UICONTROL Fogli Google] >[!UICONTROL Ottieni una cella]** per ottenere il risultato calcolato.
1. Configura il modulo utilizzando lo stesso ID cella utilizzato nel passaggio 4.

   ![](assets/exploit-google-sheet-functions-2-350x187.png)
