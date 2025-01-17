---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Modulo Iterator in Adobe Workfront Fusion
description: La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione. Questo articolo è stato dichiarato obsoleto, ma contiene un collegamento al nuovo articolo che descrive questa funzionalità.
author: Becky
feature: Workfront Fusion
exl-id: d356276d-e5d9-496f-85cd-cb60a8f8f377
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '704'
ht-degree: 0%

---

# Modulo [!UICONTROL Iterator] in [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione.
>
>Le informazioni contenute in questo articolo sono ora disponibili nell’articolo:
>
>* [Modulo iteratore](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/modules/iterator-module.html)
>
>Aggiorna eventuali segnalibri.
>
>Questo articolo non è più in fase di aggiornamento e verrà rimosso nel prossimo futuro.

Un modulo [!UICONTROL Iterator] è un tipo speciale di modulo che converte un array in una serie di bundle. Ogni elemento array viene prodotto come bundle separato.

Per ulteriori informazioni, vedere [Tipi di moduli](../../workfront-fusion/modules/module-types.md) e [Mappare un array in Adobe Workfront Fusion](../../workfront-fusion/mapping/map-an-array.md).

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
   <td>Per utilizzare le funzionalità descritte in questo articolo, la tua organizzazione deve acquistare Adobe Workfront Fusion e Adobe Workfront.</td> 
  </tr> 
 </tbody> 
</table>

Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

Per informazioni sulle [!DNL Adobe Workfront Fusion] licenze, vedere [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Configurazione del modulo [!UICONTROL Iterator]

Il modulo [!UICONTROL Iterator] viene configurato allo stesso modo di qualsiasi altro modulo. Il campo [!UICONTROL Array] contiene l&#39;array da convertire o dividere in bundle separati.

![](assets/set-up-iterator-350x190.jpg)

Per ulteriori informazioni, vedere [Configurare le impostazioni di un modulo in Adobe Workfront Fusion](../../workfront-fusion/modules/configure-a-modules-settings.md).

>[!INFO]
>
>**Esempi:**
>
>* Lo scenario seguente mostra come recuperare le e-mail con allegati e salvare gli allegati come file singoli in una cartella [!DNL Dropbox] selezionata.
>
>   Le e-mail possono contenere una matrice di allegati. Il modulo [!UICONTROL Iterator] inserito dopo il primo modulo consentirà di gestire separatamente ogni allegato. Il modulo [!UICONTROL Iterator] divide l&#39;array di allegati in singoli bundle. Ogni bundle, con un allegato, viene quindi salvato uno alla volta in una cartella [!DNL Dropbox] selezionata. La configurazione del modulo [!UICONTROL Iterator] è mostrata sopra: il campo [!UICONTROL Array] deve contenere l&#39;array `Attachments`.
>
>   ![](assets/attachments-array-350x154.jpg)
>
>* Per comodità, molte app [!DNL Workfront Fusion] offrono moduli [!UICONTROL Iterator] specializzati con una configurazione semplificata. Ad esempio, l&#39;app [!UICONTROL E-mail] contiene il modulo speciale [!UICONTROL Iterator] [!UICONTROL E-mail] > [!UICONTROL Itera allegati] che produrrà gli stessi risultati del modulo generale [!UICONTROL Iterator].
>
>   ![](assets/specialized-iterators-350x135.jpg)


## Risoluzione dei problemi: il pannello di mappatura non visualizza gli elementi mappabili nel modulo [!UICONTROL Iterator]

Quando un modulo [!UICONTROL Iterator] non dispone di informazioni sulla struttura degli elementi dell&#39;array, il pannello di mappatura nei moduli successivi al modulo [!UICONTROL Iterator] visualizza solo 2 elementi nel modulo [!UICONTROL Iterator]:`Total number of bundles` e `Bundle order position`:

![](assets/mapping-panel-doesnt-display-350x147.png)

Questo perché ogni modulo è responsabile della fornitura di informazioni sugli elementi prodotti, in modo che possano essere visualizzati correttamente nel pannello di mappatura nei moduli successivi. In alcuni casi, tuttavia, diversi moduli potrebbero non essere in grado di fornire queste informazioni. Ad esempio, [!UICONTROL JSON] > [!UICONTROL Analizza JSON] o [!UICONTROL Webhook] > [!UICONTROL Webhook personalizzato] moduli con struttura dati mancante.

La soluzione consiste nell’eseguire manualmente lo scenario per consentire al modulo di acquisire informazioni sugli elementi generati, in modo da poter fornire le informazioni ai moduli seguenti.

Ad esempio, se disponi di un modulo [!UICONTROL JSON] > [!UICONTROL Analizza JSON] senza una struttura dati come indicato di seguito:

![](assets/json-parse-json-350x285.png)

Quindi, se si collega un modulo [!UICONTROL Iterator] ad esso, non sarà possibile mappare l&#39;output del modulo al campo Array nel pannello di configurazione del modulo [!UICONTROL Iterator]:

![](assets/connect-iterator-module-350x146.png)

Per risolvere questo problema, avvia manualmente lo scenario nell’editor dello scenario. Puoi scollegare i moduli dopo il modulo [!UICONTROL JSON] > [!UICONTROL Analizza JSON] per impedire che il flusso proceda ulteriormente. Oppure puoi fare clic con il pulsante destro del mouse sul modulo [!UICONTROL JSON] > [!UICONTROL Analizza JSON] e scegliere **[!UICONTROL Esegui questo modulo solo]** dal menu di scelta rapida per eseguire solo il modulo [!UICONTROL JSON] > [!UICONTROL Analizza JSON].

Durante l&#39;esecuzione di [!UICONTROL JSON] > [!UICONTROL Analizza JSON], viene a conoscenza degli elementi generati e fornisce queste informazioni a tutti i moduli successivi, incluso il modulo Iterator. Il pannello di mappatura nella configurazione dell’iteratore visualizza quindi gli elementi:

![](assets/mapping-panel-displays-items-350x131.png)

Inoltre, il pannello di mappatura nei moduli connessi dopo il modulo [!UICONTROL Iterator] visualizza gli elementi contenuti negli elementi dell&#39;array:

![](assets/items-contained-in-array-350x156.png)

Se non riesci a visualizzare alcuni elementi nel pannello di mappatura di un modulo, esegui lo scenario una volta in modo che tutti i moduli possano conoscere gli elementi generati e fornire queste informazioni ai seguenti moduli.
