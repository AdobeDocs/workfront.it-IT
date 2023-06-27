---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Informazioni sulla mappatura dei file in [!DNL Adobe Workfront Fusion]
description: Alcuni moduli sono in grado di elaborare i file. Questi moduli possono restituire un file di output da inviare per l'ulteriore elaborazione o richiedere che venga trasmesso un file per l'elaborazione. Prima che questi moduli possano lavorare insieme per elaborare i file, devono essere mappati l’uno sull’altro.
author: Becky
feature: Workfront Fusion
exl-id: 9ed5f176-86d8-4139-b582-c2f58aaed8d4
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '468'
ht-degree: 0%

---

# Informazioni sulla mappatura dei file in [!DNL Adobe Workfront Fusion]

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
  </tr>  </tbody> 
</table>

Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, consulta [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## File di mappatura

I moduli che possono lavorare con i file richiedono due informazioni:

* Nome file
* Contenuto file (dati)

Quando mappi un file, scegli i moduli nel tuo scenario da cui desideri ottenere i dati. Il nome e il contenuto del file vengono quindi mappati automaticamente così come sono.

>[!NOTE]
>
>Se devi elaborare un file da un URL, ti consigliamo di utilizzare `HTTP > Get a File` per scaricare il file dall&#39;URL e quindi mappare il file dal `HTTP > Get a File` nel campo del modulo desiderato nello scenario.

>[!INFO]
>
>**Esempio:** In questo esempio viene illustrato come scaricare documenti da [!DNL Adobe Workfront] a [!DNL Google Drive]. Il [!DNL Workfront] trigger [!UICONTROL Record di controllo] restituisce informazioni dettagliate su ciascun documento, inclusi il nome e l&#39;ID.
>
>Il modulo successivo, [!UICONTROL Scarica documento], scarica i dati effettivi in modo che possano essere caricati su Google Drive.
>
>Per mappare queste informazioni a [!DNL Google Drive] per caricarlo, devi specificare il file di origine da cui verranno mappate le informazioni. Se si seleziona la [!DNL Workfront] > [!UICONTROL Scarica documento] nel file di origine, [!DNL Workfront Fusion] mappa il nome e il contenuto del file in modo che il documento da [!DNL Workfront] viene caricato nella cartella Google specificata.
>
>![](assets/wf-download-document-350x605.png)
>
>Tuttavia, se desideri rinominare il file mantenendo i dati così come sono, puoi utilizzare [!UICONTROL Mappa] per mappare separatamente il nome e il contenuto del file. Immettere il nome completo del file, inclusa l&#39;estensione. Sono supportati i formati di testo e i formati binari, ad esempio foto, video e PDF.
>
>![](assets/use-the-map-option-350x358.png)
