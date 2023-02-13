---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Informazioni sulla mappatura dei file in [!DNL Adobe Workfront Fusion]
description: Alcuni moduli hanno la capacità di elaborare i file. Questi moduli possono restituire un file di output da inviare per un’ulteriore elaborazione o richiedere che venga loro trasmesso un file per l’elaborazione. Prima che questi moduli possano funzionare insieme per elaborare i file, devono essere mappati tra loro.
author: Becky
feature: Workfront Fusion
exl-id: 9ed5f176-86d8-4139-b582-c2f58aaed8d4
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 0%

---

# Informazioni sulla mappatura dei file in [!DNL Adobe Workfront Fusion]

Alcuni moduli hanno la capacità di elaborare i file. Questi moduli possono restituire un file di output da inviare per un’ulteriore elaborazione o richiedere che venga loro trasmesso un file per l’elaborazione. Prima che questi moduli possano funzionare insieme per elaborare i file, devono essere mappati tra loro.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</td> 
  </tr>  </tbody> 
</table>

Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, vedi [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## File di mappatura

I moduli che hanno la capacità di lavorare con i file richiedono due informazioni:

* Nome file
* Contenuto del file (dati)

Quando mappi un file, scegli i moduli nel tuo scenario da cui desideri ottenere i dati. Il nome del file e il contenuto del file vengono quindi mappati automaticamente così come sono.

>[!NOTE]
>
>Se devi elaborare un file da un URL, ti consigliamo di utilizzare il `HTTP > Get a File` modulo per scaricare il file dall&#39;URL, quindi mappare il file dal `HTTP > Get a File` nel campo del modulo desiderato nel tuo scenario.

>[!INFO]
>
>**Esempio:** Questo esempio mostra come scaricare documenti da [!DNL Adobe Workfront] a [!DNL Google Drive]. La [!DNL Workfront] attivare [!UICONTROL Registra] restituisce informazioni dettagliate su ciascun documento, inclusi nome e ID.
>
>Il modulo successivo, [!UICONTROL Scarica documento], scarica i dati effettivi in modo che possano essere caricati su Google Drive.
>
>Per mappare queste informazioni su [!DNL Google Drive] affinché possa essere caricato, devi specificare il file di origine da cui verranno mappate le informazioni. Se selezioni la [!DNL Workfront] > [!UICONTROL Scarica documento] opzione nel file di origine, [!DNL Workfront Fusion] mappa il nome file e il contenuto del file in modo che il documento da [!DNL Workfront] viene caricato nella cartella Google specificata.
>
>![](assets/wf-download-document-350x605.png)
>
>Tuttavia, se si desidera rinominare il file ma mantenere i dati così come sono, è possibile utilizzare il [!UICONTROL Mappa] per mappare separatamente il nome del file e il contenuto del file. Immetti il nome completo del file, inclusa l’estensione . Sono supportati i formati di testo e i formati binari, come foto, video e PDF.
>
>![](assets/use-the-map-option-350x358.png)
