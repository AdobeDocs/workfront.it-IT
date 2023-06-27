---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Modulo Iterator in Adobe Workfront Fusion
description: Un modulo Iterator è un tipo speciale di modulo che converte un array in una serie di bundle. Ogni elemento array viene prodotto come bundle separato.
author: Becky
feature: Workfront Fusion
exl-id: d356276d-e5d9-496f-85cd-cb60a8f8f377
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '657'
ht-degree: 0%

---

# [!UICONTROL Iteratore] modulo in [!DNL Adobe Workfront Fusion]

Un [!UICONTROL Iteratore] Il modulo è un tipo speciale di modulo che converte un array in una serie di bundle. Ogni elemento array viene prodotto come bundle separato.

Per ulteriori informazioni, consulta [Tipi di moduli](../../workfront-fusion/modules/module-types.md) e [Mappare un array in Adobe Workfront Fusion](../../workfront-fusion/mapping/map-an-array.md).

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
   <td>Per utilizzare le funzionalità descritte in questo articolo, la tua organizzazione deve acquistare Adobe Workfront Fusion e Adobe Workfront.</td> 
  </tr> 
 </tbody> 
</table>

Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, consulta [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL Iteratore] configurazione del modulo

Hai impostato un [!UICONTROL Iteratore] lo stesso che hai impostato per qualsiasi altro modulo. Il [!UICONTROL Array] contiene l’array da convertire o dividere in bundle separati.

![](assets/set-up-iterator-350x190.jpg)

Per ulteriori informazioni, consulta [Configurare le impostazioni di un modulo in Adobe Workfront Fusion](../../workfront-fusion/modules/configure-a-modules-settings.md).

>[!INFO]
>
>**Esempi:**
>
>* Lo scenario seguente mostra come recuperare le e-mail con allegati e salvarli come file singoli in una [!DNL Dropbox] cartella.
>
>   Le e-mail possono contenere una matrice di allegati. Il [!UICONTROL Iteratore] inserito dopo il primo modulo consente di gestire separatamente ogni allegato. Il [!UICONTROL Iteratore] Il modulo divide l’array di allegati in singoli bundle. Ogni bundle, con un allegato, viene quindi salvato uno alla volta in un [!DNL Dropbox] cartella. Il [!UICONTROL Iteratore] la configurazione del modulo è mostrata sopra: [!UICONTROL Array] deve contenere `Attachments` array.
>
>   ![](assets/attachments-array-350x154.jpg)
>
>* Per la tua comodità, molti [!DNL Workfront Fusion] le app offrono specializzato [!UICONTROL Iteratore] moduli con una configurazione semplificata. Ad esempio, il [!UICONTROL E-mail] l&#39;app contiene lo speciale [!UICONTROL Iteratore] modulo [!UICONTROL E-mail] > [!UICONTROL Itera allegati] che produrrà gli stessi risultati del generale [!UICONTROL Iteratore] modulo.
>
>   ![](assets/specialized-iterators-350x135.jpg)


## Risoluzione dei problemi: il pannello Mappatura non visualizza gli elementi mappabili in [!UICONTROL Iteratore] modulo

Quando un [!UICONTROL Iteratore] Il modulo non contiene informazioni sulla struttura degli elementi dell’array, il pannello di mappatura nei moduli che seguono [!UICONTROL Iteratore] Il modulo visualizza solo 2 elementi sotto [!UICONTROL Iteratore] modulo :`Total number of bundles` e `Bundle order position`:

![](assets/mapping-panel-doesnt-display-350x147.png)

Questo perché ogni modulo è responsabile della fornitura di informazioni sugli elementi prodotti, in modo che possano essere visualizzati correttamente nel pannello di mappatura nei moduli successivi. Tuttavia, in alcuni casi diversi moduli potrebbero non essere in grado di fornire queste informazioni; ad esempio, [!UICONTROL JSON] > [!UICONTROL Analizza JSON] o [!UICONTROL Webhook] > [!UICONTROL Webhook personalizzato] moduli con struttura dati mancante.

La soluzione consiste nell’eseguire manualmente lo scenario per consentire al modulo di acquisire informazioni sugli elementi generati, in modo da poter fornire le informazioni ai moduli seguenti.

Ad esempio, se hai un [!UICONTROL JSON] > [!UICONTROL Analizza JSON] modulo senza una struttura di dati come segue:

![](assets/json-parse-json-350x285.png)

E poi se connetti un [!UICONTROL Iteratore] non sarà possibile mappare l&#39;output del modulo al campo Array nel pannello di configurazione del [!UICONTROL Iteratore] modulo :

![](assets/connect-iterator-module-350x146.png)

Per risolvere questo problema, avvia manualmente lo scenario nell’editor dello scenario. Puoi scollegare i moduli dopo [!UICONTROL JSON] > [!UICONTROL Analizza JSON] per evitare che il flusso proceda ulteriormente. Oppure puoi fare clic con il pulsante destro del mouse sulla [!UICONTROL JSON] > [!UICONTROL Analizza JSON] e scegliere **[!UICONTROL Esegui solo questo modulo]** dal menu di scelta rapida per eseguire solo [!UICONTROL JSON] > [!UICONTROL Analizza JSON] modulo.

Quando [!UICONTROL JSON] > [!UICONTROL Analizza JSON] viene eseguito, viene informato sugli elementi generati e fornisce tali informazioni a tutti i moduli successivi, incluso il modulo Iterator. Il pannello di mappatura nella configurazione dell’iteratore visualizza quindi gli elementi:

![](assets/mapping-panel-displays-items-350x131.png)

Inoltre, il pannello di mappatura nei moduli che sono connessi dopo il [!UICONTROL Iteratore] Il modulo visualizza gli elementi contenuti negli elementi dell’array:

![](assets/items-contained-in-array-350x156.png)

Se non riesci a visualizzare alcuni elementi nel pannello di mappatura di un modulo, esegui lo scenario una volta in modo che tutti i moduli possano conoscere gli elementi generati e fornire queste informazioni ai seguenti moduli.
