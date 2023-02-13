---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Moduli immagine
description: I moduli immagine Adobe Workfront Fusion consentono di ottenere informazioni su un'immagine specifica (dimensioni, tipo e così via), convertire un'immagine in un altro formato di file e modificare direttamente le dimensioni dell'immagine.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 89efa9d5-00c9-4bb5-97b3-2b2f9d73721d
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '860'
ht-degree: 0%

---

# Moduli immagine

[!DNL Adobe Workfront Fusion] [!UICONTROL Immagine] I moduli consentono di ottenere informazioni su un’immagine specifica (dimensioni, tipo e così via), convertire un’immagine in un altro formato di file e modificare direttamente le dimensioni dell’immagine.

## Requisiti di accesso

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td>
  <td> <p>[!UICONTROL Pro] o superiore</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licenza**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p>  <p>[!UICONTROL [!DNL Workfront Fusion] per automazione del lavoro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</td> 
  </tr> 
 </tbody> 
</table>

Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, vedi [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL Immagine] moduli e relativi campi

Quando si configura questo modulo, vengono visualizzati i campi seguenti. Un titolo in grassetto in un modulo indica un campo obbligatorio.

* [[!UICONTROL Ridimensiona]](#resize)
* [[!UICONTROL Convertire un formato]](#convert-a-format)
* [[!UICONTROL Estrai metadati]](#extract-metadata)

### [!UICONTROL Ridimensiona]

Questo modulo di trasformazione modifica l&#39;altezza e la larghezza di un&#39;immagine in base ai criteri specificati.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL File di origine]</td> 
   <td> <p>Selezionare l'origine dell'immagine da convertire. È possibile selezionare l'output da un modulo precedente o mappare il file di dati e il nome del file. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data]</td> 
   <td>Mappa il file da convertire. Questo campo è disponibile se hai selezionato [!UICONTROL Map] nel campo [!UICONTROL Source file] .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File name]</td> 
   <td>Immettere un nome per il file convertito. Questo campo è disponibile se hai selezionato [!UICONTROL Map] nel campo [!UICONTROL Source file] .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Voglio]</td> 
   <td>Seleziona se mantenere il rapporto altezza-larghezza o modifica le dimensioni in un'altezza e una larghezza specificate.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL in base a]</td> 
   <td> <p>Seleziona la modalità in cui desideri che il modulo determini le nuove dimensioni dell’immagine. Questo campo viene visualizzato se si è selezionato per mantenere la proporzione di altezza-larghezza nel campo che si desidera utilizzare. Altri campi vengono visualizzati in base alla selezione effettuata in questo campo.</p> 
    <ul> 
     <li> <p>[!UICONTROL Larghezza massima]</p> <p>Riduce un'immagine alla larghezza specificata. L'altezza viene calcolata automaticamente.</p> </li> 
     <li> <p>[!UICONTROL Altezza massima]</p> <p>Riduce un'immagine all'altezza specificata. La larghezza viene calcolata automaticamente.</p> </li> 
     <li> <p>[!UICONTROL Altezza o larghezza massima]</p> <p>Riduce un’immagine in modo che altezza e larghezza non superino i valori specificati. Poiché questa opzione mantiene il rapporto altezza-larghezza, una delle dimensioni può essere inferiore a quella specificata. Ad esempio, se l'altezza e la larghezza sono entrambe specificate come 40, un'immagine 400x300 verrà ridotta a 40X30.</p> </li> 
     <li> <p>[!UICONTROL Larghezza minima]</p> <p>Ingrandisce un’immagine con la larghezza specificata. L'altezza viene calcolata automaticamente.</p> </li> 
     <li> <p>[!UICONTROL Altezza minima]</p> <p>Ingrandisce un’immagine fino all’altezza specificata. La larghezza viene calcolata automaticamente.</p> </li> 
     <li> <p>[!UICONTROL Altezza o larghezza minima]</p> <p>Ingrandisce un’immagine in modo che altezza e larghezza non siano inferiori ai valori specificati. Poiché questa opzione mantiene il rapporto altezza-larghezza, una delle dimensioni può essere maggiore di quella specificata. Ad esempio, se l'altezza e la larghezza sono entrambe specificate come 300, un'immagine 40x30 verrà ingrandita a 400X300.</p> </li> 
     <li> <p>[!UICONTROL Percent]</p> <p>Modifica le dimensioni dell’immagine di una percentuale in base al valore specificato. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Width]</td> 
   <td>Immettere o mappare la larghezza desiderata dell'immagine ridimensionata in pixel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Height]</td> 
   <td>Immettere o mappare l'altezza desiderata dell'immagine ridimensionata in pixel.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Convertire un formato]

Questo modulo di trasformazione modifica il formato di un file di immagine. Questo modulo è compatibile con i seguenti formati:

* PNG
* JPG
* GIF
* BMP

Il file di origine e l&#39;output devono essere in uno di questi formati. Ad esempio, il [!UICONTROL Immagine] >[!UICONTROL Convertire un formato] Il modulo può trasformare un file PNG in un file BMP o un file BMP in un JPG.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL File di origine]</td> 
   <td> <p>Selezionare l'origine dell'immagine da convertire. È possibile selezionare l'output da un modulo precedente o mappare il file di dati e il nome del file. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data]</td> 
   <td>Mappa il file da convertire. Questo campo è disponibile se hai selezionato [!UICONTROL Map] nel campo [!UICONTROL Source file] .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File name]</td> 
   <td>Immettere un nome per il file convertito. Questo campo è disponibile se hai selezionato [!UICONTROL Map] nel campo [!UICONTROL Source file] .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Formato di output]</td> 
   <td>Selezionare il formato in cui si desidera convertire il file di origine dal modulo. </td> 
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
   <td role="rowheader">[!UICONTROL File di origine]</td> 
   <td> <p>Selezionare l'origine dell'immagine da convertire. È possibile selezionare l'output da un modulo precedente o mappare il file di dati e il nome del file. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data]</td> 
   <td>Mappa il file da convertire. Questo campo è disponibile se hai selezionato Mappa nel campo [!UICONTROL Source file] .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File name]</td> 
   <td>Immettere un nome per il file convertito. Questo campo è disponibile se hai selezionato Mappa nel campo [!UICONTROL Source file] .</td> 
  </tr> 
 </tbody> 
</table>

## Possibili problemi

### Azione terminata con un errore

Ci sono tre casi in cui un&#39;azione può terminare con un errore:

* I dati ricevuti non erano in formato JPG/GIF/PNG/BMP
* Il limite massimo di larghezza/altezza era stato superato durante la modifica delle dimensioni dell&#39;immagine. Le dimensioni dell&#39;immagine non devono superare 3840 px di larghezza e 2160 px di altezza
* La dimensione massima consentita per un&#39;immagine è stata superata durante la modifica delle dimensioni o del formato dell&#39;immagine.
