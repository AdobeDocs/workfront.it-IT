---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Moduli immagine
description: I moduli immagine di Adobe Workfront Fusion consentono di ottenere informazioni su un’immagine specifica (dimensioni, tipo e così via), convertire un’immagine in un altro formato di file e modificare direttamente le dimensioni dell’immagine.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 89efa9d5-00c9-4bb5-97b3-2b2f9d73721d
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '912'
ht-degree: 0%

---

# Moduli immagine

I moduli [!DNL Adobe Workfront Fusion] [!UICONTROL Immagine] ti consentono di ottenere informazioni su un&#39;immagine specifica (dimensioni, tipo e così via), convertire un&#39;immagine in un altro formato di file e modificare direttamente le dimensioni dell&#39;immagine.

## Requisiti di accesso

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td>
  <td> <p>[!UICONTROL Pro] o versione successiva</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licenza**</td> 
   <td>
   <p>Requisiti di licenza correnti: nessun requisito di licenza [!DNL Workfront Fusion].</p>
   <p>Oppure</p>
   <p>Requisito licenza legacy: [!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione lavoro], [!UICONTROL [!DNL Workfront Fusion] per automazione lavoro]</p>
   </td> 
  </tr> 
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

## [!UICONTROL Moduli immagine] e relativi campi

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti. Un titolo in grassetto in un modulo indica un campo obbligatorio.

* [[!UICONTROL Ridimensiona]](#resize)
* [[!UICONTROL Convertire un formato]](#convert-a-format)
* [[!UICONTROL Estrai metadati]](#extract-metadata)

### [!UICONTROL Ridimensiona]

Questo modulo di trasformazione modifica l’altezza e la larghezza di un’immagine in base ai criteri specificati.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Seleziona l’origine dell’immagine da convertire. Puoi selezionare l’output da un modulo precedente o mappare il file di dati e il nome del file. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data]</td> 
   <td>Mappa il file da convertire. Questo campo è disponibile se è stato selezionato [!UICONTROL Map] nel campo [!UICONTROL Source file].</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome file]</td> 
   <td>Immettere un nome per il file convertito. Questo campo è disponibile se è stato selezionato [!UICONTROL Map] nel campo [!UICONTROL Source file].</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL che desidero]</td> 
   <td>Selezionate se desiderate mantenere le proporzioni tra altezza e larghezza oppure modificate le quote impostandole su un valore specificato per altezza e larghezza.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Secondo]</td> 
   <td> <p>Seleziona la modalità con cui vuoi che il modulo determini le nuove dimensioni dell'immagine. Questo campo viene visualizzato se si è selezionato di mantenere il rapporto altezza-larghezza nel campo che si desidera visualizzare. Altri campi vengono visualizzati in base alla selezione effettuata in questo campo.</p> 
    <ul> 
     <li> <p>[!UICONTROL Larghezza massima]</p> <p>Riduce l'immagine alla larghezza specificata. L'altezza viene calcolata automaticamente.</p> </li> 
     <li> <p>[!UICONTROL Altezza massima]</p> <p>Riduce l'altezza di un'immagine specificata. La larghezza viene calcolata automaticamente.</p> </li> 
     <li> <p>[!UICONTROL Altezza o larghezza massima]</p> <p>Riduce un'immagine in modo che la sua altezza e larghezza non superino i valori specificati. Poiché questa opzione mantiene il rapporto altezza-larghezza, una delle quote potrebbe essere inferiore a quella specificata. Ad esempio, se altezza e larghezza sono entrambe specificate come 40, un'immagine 400x300 verrà ridotta a 40x30.</p> </li> 
     <li> <p>[!UICONTROL larghezza minima]</p> <p>Ingrandisce un'immagine alla larghezza specificata. L'altezza viene calcolata automaticamente.</p> </li> 
     <li> <p>[!UICONTROL Altezza minima]</p> <p>Ingrandisce l'immagine all'altezza specificata. La larghezza viene calcolata automaticamente.</p> </li> 
     <li> <p>[!UICONTROL Altezza o larghezza minima]</p> <p>Ingrandisce un'immagine in modo che l'altezza e la larghezza non siano inferiori ai valori specificati. Poiché questa opzione mantiene il rapporto altezza-larghezza, una delle dimensioni potrebbe essere maggiore di quella specificata. Ad esempio, se altezza e larghezza sono entrambe specificate come 300, un'immagine 40x30 verrà ingrandita a 400X300.</p> </li> 
     <li> <p>[!UICONTROL Percent]</p> <p>Modifica le dimensioni dell'immagine in base a una percentuale in base al valore specificato. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Width]</td> 
   <td>Inserisci o mappa la larghezza desiderata dell’immagine ridimensionata in pixel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Height]</td> 
   <td>Inserisci o mappa l’altezza desiderata dell’immagine ridimensionata in pixel.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Convertire un formato]

Questo modulo di trasformazione modifica il formato di un file di immagine. Questo modulo è compatibile con i seguenti formati:

* PNG
* JPG-
* GIF
* BMP

Sia il file di origine che l&#39;output devono essere in uno di questi formati. Ad esempio, il modulo [!UICONTROL Image] >[!UICONTROL Convert a format] può trasformare un file PNG in un file BMP o un BMP in un JPG.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Seleziona l’origine dell’immagine da convertire. Puoi selezionare l’output da un modulo precedente o mappare il file di dati e il nome del file. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data]</td> 
   <td>Mappa il file da convertire. Questo campo è disponibile se è stato selezionato [!UICONTROL Map] nel campo [!UICONTROL Source file].</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome file]</td> 
   <td>Immettere un nome per il file convertito. Questo campo è disponibile se è stato selezionato [!UICONTROL Map] nel campo [!UICONTROL Source file].</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Formato di output]</td> 
   <td>Selezionare il formato in cui convertire il file di origine nel modulo. </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Estrai metadati]

Questo modulo di trasformazione restituisce informazioni di base su un modulo.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Seleziona l’origine dell’immagine da convertire. Puoi selezionare l’output da un modulo precedente o mappare il file di dati e il nome del file. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data]</td> 
   <td>Mappa il file da convertire. Questo campo è disponibile se è stato selezionato Mappa nel campo [!UICONTROL Source file].</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome file]</td> 
   <td>Immettere un nome per il file convertito. Questo campo è disponibile se è stato selezionato Mappa nel campo [!UICONTROL Source file].</td> 
  </tr> 
 </tbody> 
</table>

## Possibili problemi

### Azione terminata con un errore

Esistono tre casi in cui un’azione può terminare con un errore:

* I dati ricevuti non erano nel formato JPG GIF/PNG/BMP
* È stato superato il limite massimo di larghezza/altezza durante la modifica delle dimensioni dell’immagine. La dimensione dell&#39;immagine non deve superare i 3840 px di larghezza e 2160 px di altezza
* Le dimensioni massime consentite per un&#39;immagine sono state superate durante la modifica delle dimensioni o del formato dell&#39;immagine.
