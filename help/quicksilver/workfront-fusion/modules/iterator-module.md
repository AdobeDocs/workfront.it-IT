---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Modulo iteratore in Adobe Workfront Fusion
description: Un modulo Iterator è un tipo speciale di modulo che converte un array in una serie di bundle. Ogni elemento dell’array viene emesso come bundle separato.
author: Becky
feature: Workfront Fusion
exl-id: d356276d-e5d9-496f-85cd-cb60a8f8f377
source-git-commit: a2060e7179f2295bfd42da84bd7bca9862ad0a17
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 0%

---

# [!UICONTROL Iteratore] modulo in [!DNL Adobe Workfront Fusion]

Un [!UICONTROL Iteratore] modulo è un tipo speciale di modulo che converte un array in una serie di bundle. Ogni elemento dell’array viene emesso come bundle separato.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>Per utilizzare le funzionalità descritte in questo articolo, la tua organizzazione deve acquistare Adobe Workfront Fusion e Adobe Workfront.</td> 
  </tr> 
 </tbody> 
</table>

Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, vedi [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL Iteratore] configurazione del modulo

Imposta un [!UICONTROL Iteratore] nello stesso modo in cui si imposta qualsiasi altro modulo. La [!UICONTROL Array] il campo contiene l&#39;array da convertire o dividere in bundle separati.

![](assets/set-up-iterator-350x190.jpg)

Per ulteriori informazioni, consulta [Configurare le impostazioni di un modulo in Adobe Workfront Fusion](../../workfront-fusion/modules/configure-a-modules-settings.md).

>[!INFO]
>
>**Esempi:**
>
>* Lo scenario seguente mostra come recuperare e-mail con allegati e salvare gli allegati come file singoli in una selezione [!DNL Dropbox] cartella.
   >
   >   Le e-mail possono contenere una matrice di allegati. La [!UICONTROL Iteratore] Il modulo inserito dopo il primo modulo consente di gestire separatamente ogni allegato. La [!UICONTROL Iteratore] Il modulo divide l&#39;array di allegati in singoli bundle. Ogni bundle, con un solo allegato, viene quindi salvato uno alla volta in un [!DNL Dropbox] cartella. La [!UICONTROL Iteratore] la configurazione del modulo è mostrata sopra: la [!UICONTROL Array] il campo deve contenere `Attachments` array.
   >
   >   ![](assets/attachments-array-350x154.jpg)
>
>* Per vostra comodità, molti [!DNL Workfront Fusion] app specializzate [!UICONTROL Iteratore] moduli con configurazione semplificata. Ad esempio, il [!UICONTROL E-mail] l&#39;app contiene lo speciale [!UICONTROL Iteratore] modulo [!UICONTROL E-mail] > [!UICONTROL Itera allegati] che produrrà gli stessi risultati del [!UICONTROL Iteratore] modulo .
   >
   >   ![](assets/specialized-iterators-350x135.jpg)



## Risoluzione dei problemi: Il pannello di mappatura non visualizza gli elementi mappabili in [!UICONTROL Iteratore] modulo

Quando un [!UICONTROL Iteratore] Il modulo non contiene informazioni sulla struttura degli elementi dell&#39;array, il pannello di mappatura nei moduli che seguono [!UICONTROL Iteratore] il modulo visualizza solo 2 elementi sotto [!UICONTROL Iteratore] modulo :`Total number of bundles` e `Bundle order position`:

![](assets/mapping-panel-doesnt-display-350x147.png)

Questo perché ogni modulo è responsabile di fornire informazioni sugli elementi che genera in modo che questi elementi possano essere visualizzati correttamente nel pannello di mappatura nei moduli successivi. Tuttavia, in alcuni casi diversi moduli potrebbero non essere in grado di fornire tali informazioni; ad esempio, [!UICONTROL JSON] > [!UICONTROL Analizza JSON] o [!UICONTROL Webhook] > [!UICONTROL Webhook personalizzato] moduli con struttura dati mancante.

La soluzione consiste nell’eseguire manualmente lo scenario per fare in modo che il modulo apprenda gli elementi che genera in modo da fornire le informazioni ai moduli seguenti.

Ad esempio, se hai una [!UICONTROL JSON] > [!UICONTROL Analizza JSON] modulo senza struttura dati come segue:

![](assets/json-parse-json-350x285.png)

E poi se connetti un [!UICONTROL Iteratore] non sarà possibile mappare l&#39;output del modulo al campo Array nel pannello di configurazione del modulo [!UICONTROL Iteratore] modulo :

![](assets/connect-iterator-module-350x146.png)

Per risolvere questo problema, avvia manualmente lo scenario nell’editor di scenari. Puoi scollegare i moduli dopo la [!UICONTROL JSON] > [!UICONTROL Analizza JSON] modulo per impedire che il flusso proceda ulteriormente. Oppure puoi fare clic con il pulsante destro del mouse sul pulsante [!UICONTROL JSON] > [!UICONTROL Analizza JSON] modulo e scegli **[!UICONTROL Esegui solo questo modulo]** dal menu di scelta rapida per eseguire solo l’ [!UICONTROL JSON] > [!UICONTROL Analizza JSON] modulo .

Quando il [!UICONTROL JSON] > [!UICONTROL Analizza JSON] esegue, apprende gli elementi che genera e fornisce tali informazioni a tutti i moduli successivi, incluso il modulo Iterator. Il pannello di mappatura nella configurazione dell&#39;iteratore visualizza quindi gli elementi:

![](assets/mapping-panel-displays-items-350x131.png)

Inoltre, il pannello di mappatura nei moduli che sono collegati dopo il [!UICONTROL Iteratore] il modulo visualizza gli elementi contenuti negli elementi dell&#39;array:

![](assets/items-contained-in-array-350x156.png)

Se non è possibile visualizzare alcuni elementi nel pannello di mappatura di un modulo, esegui lo scenario una volta in modo che tutti i moduli possano apprendere gli elementi che producono e fornire tali informazioni ai moduli seguenti.
