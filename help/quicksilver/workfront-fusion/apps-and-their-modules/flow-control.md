---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Controllo del flusso in Adobe Workfront Fusion
description: Quando crei o modifichi uno scenario, puoi configurare le impostazioni per controllare il modo in cui i dati scorrono all’interno di esso.
author: Becky
feature: Workfront Fusion
exl-id: 0f315192-c15e-48e8-a5b6-827c300f0e5c
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '637'
ht-degree: 1%

---

# Controllo del flusso in Adobe Workfront Fusion

Quando crei o modifichi uno scenario, puoi configurare le impostazioni per controllare il modo in cui i dati scorrono all’interno di esso.

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
   <p>Fabbisogno di licenza corrente: No [!DNL Workfront Fusion] requisito di licenza.</p>
   <p>Oppure</p>
   <p>Requisito licenza legacy: [!UICONTROL [!DNL Workfront Fusion] per l'automazione e l'integrazione del lavoro], [!UICONTROL [!DNL Workfront Fusion] per automazione lavoro]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>
   <p>Fabbisogno prodotto corrente: se si dispone di [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront] Pianifica, la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare la funzionalità descritta in questo articolo. [!DNL Workfront Fusion] è incluso in [!UICONTROL Ultimate] [!DNL Workfront] piano.</p>
   <p>Oppure</p>
   <p>Requisiti del prodotto legacy: la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare la funzionalità descritta in questo articolo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, consulta [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Ripetitore

È possibile utilizzare una [!UICONTROL Ripetitore] per ripetere un&#39;operazione un determinato numero di volte. A [!UICONTROL Ripetitore] Il modulo genera bundle uno dopo l’altro.

Ad esempio, puoi utilizzare un’ [!UICONTROL Ripetitore] per inviare cinque e-mail con gli oggetti &quot;Hello 1&quot;, &quot;Hello 2&quot; e così via, collegando **[!UICONTROL E-mail] >[!UICONTROL Inviami un’e-mail]** al modulo [!UICONTROL Ripetitore] modulo.

Per utilizzare una [!UICONTROL Ripetitore] modulo:

1. Fai clic su [!UICONTROL Controllo del flusso] icona ![](assets/flow-control-icon.gif) nella parte inferiore della schermata, quindi fai clic su **[!UICONTROL Ripetitore]** nel menu visualizzato.
1. Fai clic su [!UICONTROL Ripetitore] , quindi fai clic su **[!UICONTROL Connetti automaticamente]** nella casella visualizzata.
1. In [!UICONTROL Controllo del flusso] nella casella visualizzata, digita il numero di ripetizioni (bundle generati) che desideri **[!UICONTROL Si ripete]** casella.

   Nel nostro esempio di e-mail, digita 5.

   ![](assets/repeater-2-350x207.png)

   Il valore dell&#39;elemento aumenta in ogni ripetizione di questo valore specificato nella **[!UICONTROL Passaggio]** , che è possibile visualizzare selezionando **[!UICONTROL Mostra impostazioni avanzate]**. Questo numero è 1 per impostazione predefinita.

1. Clic **[!UICONTROL OK]** per chiudere **[!UICONTROL Controllo del flusso]** casella.

1. Fai clic sull’app o sul modulo di servizio connesso al [!UICONTROL Ripetitore] modulo.
1. Nella casella visualizzata digitare le informazioni che si desidera ripetere.

   Nel nostro esempio di e-mail, digita Hello nel [!UICONTROL Oggetto] box, quindi map `i` dal modulo ripetitore.

   ![](assets/repeater-3-350x207.png)

| Voce | Descrizione |
|---|---|
| [!UICONTROL Valore iniziale] | Immetti o mappa il numero che desideri che il modulo imposti come `i` nella prima iterazione. Il valore predefinito è 1. |
| [!UICONTROL Si ripete] | Immetti o mappa il numero di volte in cui desideri che il modulo si ripeta. Questo numero deve essere maggiore o uguale a 0 e minore o uguale a 10.000. |
| [!UICONTROL Step] | Questo è il numero di cui il modulo aumenta il valore di `i`. Il valore predefinito è 1. |

{style="table-layout:auto"}

>[!NOTE]
>
>Il numero di ripetizioni non è determinato dal valore di `i`, come si farebbe in un loop nella programmazione. Il modulo ripeterà il numero di volte indicato nel [!UICONTROL Si ripete] campo. Il valore `i` modifiche con ogni iterazione del [!DNL repeater] e possono essere mappati su moduli successivi. L’esempio precedente mappa il valore di `i` nel messaggio Hello, che si traduce in messaggi che recitano &quot;Hello 1,&quot; Hello 2,&quot; e così via.

## [!UICONTROL Iteratore]

Un [!UICONTROL Iteratore] è un tipo speciale di modulo che converte un array in una serie di bundle. Ogni elemento dell’array sarà un bundle separato nel [!UICONTROL Iteratore] output del modulo. Per ulteriori informazioni, consulta [[!UICONTROL Iteratore] modulo in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).

## Aggregatore array

Un aggregatore di array è un tipo speciale di modulo che consente di unire più bundle in un singolo bundle. Per ulteriori informazioni, consulta [[!UICONTROL Aggregatore] modulo in Adobe Workfront Fusion](../../workfront-fusion/modules/aggregator-module.md).

## [!UICONTROL Router]

Il [!UICONTROL Router] consente di diramare il flusso in più route ed elaborare i dati all&#39;interno di ciascuna route in modo diverso. Una volta al [!UICONTROL Router] il modulo riceve un bundle, lo inoltra a ogni route connessa nell&#39;ordine in cui le route sono state collegate al [!UICONTROL Router] modulo. Per ulteriori informazioni, consulta [Modulo router in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/router-module.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Directives</h2>
<p>The error handling directives allow you to control how your scenario reacts to errors. For more information, see <a href="../../workfront-fusion/errors/advanced-error-handling.md" class="MCXref xref">Advanced error handling in Adobe Workfront Fusion</a> and <a href="../../workfront-fusion/errors/directives-for-error-handling.md" class="MCXref xref">Directives for error handling in Adobe Workfront Fusion</a>.</p>
</div>
-->
