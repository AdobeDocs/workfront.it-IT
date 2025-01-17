---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Informazioni sulla mappatura dei file in [!DNL Adobe Workfront Fusion]
description: La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione. Questo articolo è stato dichiarato obsoleto, ma contiene un collegamento al nuovo articolo che descrive questa funzionalità.
author: Becky
feature: Workfront Fusion
exl-id: 9ed5f176-86d8-4139-b582-c2f58aaed8d4
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 1%

---

# Informazioni sulla mappatura dei file in [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione.
>
>Le informazioni contenute in questo articolo sono ora disponibili nell’articolo:
>
>* [Mappare un file tra moduli](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/map-data/map-files.html)
>
>Aggiorna eventuali segnalibri.
>
>Questo articolo non è più in fase di aggiornamento e verrà rimosso nel prossimo futuro.

Alcuni moduli sono in grado di elaborare i file. Questi moduli possono restituire un file di output da inviare per l&#39;ulteriore elaborazione o richiedere che venga trasmesso un file per l&#39;elaborazione. Prima che questi moduli possano lavorare insieme per elaborare i file, devono essere mappati l’uno sull’altro.

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
   <p>Requisito licenza legacy: [!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>
   <p>Fabbisogno prodotto corrente: se si dispone del piano [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront], l'organizzazione deve acquistare [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo. [!DNL Workfront Fusion] è incluso nel piano [!UICONTROL Ultimate] [!DNL Workfront].</p>
   <p>Oppure</p>
   <p>Requisiti del prodotto legacy: la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</p>
   </td> 
  </tr>  </tbody> 
</table>

Per conoscere il piano, il tipo di licenza o l&#39;accesso disponibili, contattare l&#39;amministratore [!DNL Workfront].

Per informazioni sulle [!DNL Adobe Workfront Fusion] licenze, vedere [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## File di mappatura

I moduli che possono lavorare con i file richiedono due informazioni:

* Nome file
* Contenuto file (dati)

Quando mappi un file, scegli i moduli nel tuo scenario da cui desideri ottenere i dati. Il nome e il contenuto del file vengono quindi mappati automaticamente così come sono.

>[!NOTE]
>
>Se devi elaborare un file da un URL, ti consigliamo di utilizzare il modulo `HTTP > Get a File` per scaricare il file dall&#39;URL e quindi di mappare il file dal modulo `HTTP > Get a File` al campo del modulo desiderato nel tuo scenario.

>[!INFO]
>
>**Esempio:** In questo esempio viene illustrato come scaricare documenti da [!DNL Adobe Workfront] a [!DNL Google Drive]. Il trigger [!DNL Workfront] [!UICONTROL Record di controllo] restituisce informazioni dettagliate su ciascun documento, inclusi il nome e l&#39;ID.
>
>Il modulo successivo, [!UICONTROL Scarica documento], scarica i dati effettivi in modo che possano essere caricati su Google Drive.
>
>Per mappare queste informazioni su [!DNL Google Drive] in modo che possano essere caricate, è necessario specificare il file di origine da cui verranno mappate le informazioni. Se si seleziona l&#39;opzione [!DNL Workfront] > [!UICONTROL Scarica documento] nel file di origine, [!DNL Workfront Fusion] associa il nome e il contenuto del file in modo che il documento di [!DNL Workfront] venga caricato nella cartella Google specificata.
>
>![](assets/wf-download-document-350x605.png)
>
>Tuttavia, se si desidera rinominare il file mantenendo i dati invariati, è possibile utilizzare l&#39;opzione [!UICONTROL Mappa] per mappare separatamente il nome e il contenuto del file. Immettere il nome completo del file, inclusa l&#39;estensione. Sono supportati i formati di testo e i formati binari, ad esempio foto, video e PDF.
>
>![](assets/use-the-map-option-350x358.png)
