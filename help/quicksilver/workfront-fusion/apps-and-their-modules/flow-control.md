---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Controllo del flusso in Adobe Workfront Fusion
description: La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione. Questo articolo è stato dichiarato obsoleto, ma contiene un collegamento al nuovo articolo che descrive questa funzionalità.
author: Becky
feature: Workfront Fusion
exl-id: 0f315192-c15e-48e8-a5b6-827c300f0e5c
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '700'
ht-degree: 0%

---

# Controllo del flusso in Adobe Workfront Fusion

>[!IMPORTANT]
>
>La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione.
>
>Le informazioni contenute in questo articolo sono ora disponibili nell’articolo:
>
>* [Controllo flusso](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/tools-and-transformers/flow-control.html)
>
>Aggiorna eventuali segnalibri.
>
>Questo articolo non è più in fase di aggiornamento e verrà rimosso nel prossimo futuro.

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

## Ripetitore

È possibile utilizzare un modulo [!UICONTROL Repeater] per ripetere un&#39;attività un determinato numero di volte. Un modulo [!UICONTROL Repeater] genera bundle uno dopo l&#39;altro.

Ad esempio, puoi utilizzare un modulo [!UICONTROL Repeater] per inviare cinque e-mail con gli oggetti &quot;Hello 1&quot;, &quot;Hello 2&quot; e così via, collegando il modulo **[!UICONTROL Email] >[!UICONTROL Send me an email]** al modulo [!UICONTROL Repeater].

Per utilizzare un modulo [!UICONTROL Repeater]:

1. Fai clic sull&#39;icona ![](assets/flow-control-icon.gif) del [!UICONTROL Controllo flusso] nella parte inferiore dello schermo, quindi fai clic su **[!UICONTROL Ripetitore]** nel menu visualizzato.
1. Fai clic sul bundle [!UICONTROL Repeater], quindi fai clic su **[!UICONTROL Connetti automaticamente]** nella casella visualizzata.
1. Nella casella [!UICONTROL Controllo flusso] visualizzata digitare il numero di ripetizioni (bundle di output) desiderato nella casella **[!UICONTROL Ripetizioni]**.

   Nel nostro esempio di e-mail, digita 5.

   ![](assets/repeater-2-350x207.png)

   Il valore dell&#39;elemento aumenta in ogni ripetizione di questo valore specificato nel campo **[!UICONTROL Passaggio]**, che puoi visualizzare selezionando **[!UICONTROL Mostra impostazioni avanzate]**. Questo numero è 1 per impostazione predefinita.

1. Fare clic su **[!UICONTROL OK]** per chiudere la casella **[!UICONTROL Controllo flusso]**.

1. Fare clic sull&#39;app o sul modulo di servizio connesso al modulo [!UICONTROL Repeater].
1. Nella casella visualizzata digitare le informazioni che si desidera ripetere.

   Nel nostro esempio di e-mail, dovresti digitare Hello nella casella [!UICONTROL Oggetto], quindi mappare `i` dal modulo del ripetitore.

   ![](assets/repeater-3-350x207.png)

| Voce | Descrizione |
|---|---|
| [!UICONTROL Valore iniziale] | Immettere o mappare il numero impostato dal modulo come `i` nella prima iterazione. Il valore predefinito è 1. |
| [!UICONTROL Ripetizioni] | Immetti o mappa il numero di volte in cui desideri che il modulo si ripeta. Questo numero deve essere maggiore o uguale a 0 e minore o uguale a 10.000. |
| [!UICONTROL Passaggio] | Numero di cui il modulo aumenta il valore di `i`. Il valore predefinito è 1. |

{style="table-layout:auto"}

>[!NOTE]
>
>Il numero di ripetizioni non è determinato dal valore di `i`, poiché si troverebbe in un ciclo nella programmazione. Il modulo ripeterà il numero di volte indicato nel campo [!UICONTROL Ripeti]. Il valore `i` cambia con ogni iterazione del modulo [!DNL repeater] e può essere mappato ai moduli successivi. Nell&#39;esempio precedente il valore di `i` viene mappato nel messaggio Hello, con messaggi che indicano &quot;Hello 1&quot;, Hello 2&quot; e così via.

## [!UICONTROL Iteratore]

Un [!UICONTROL Iterator] è un tipo speciale di modulo che converte un array in una serie di bundle. Ogni elemento di array sarà un bundle separato nell&#39;output del modulo [!UICONTROL Iterator]. Per ulteriori informazioni, vedere il modulo [[!UICONTROL Iterator] in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).

## Aggregatore array

Un aggregatore di array è un tipo speciale di modulo che consente di unire più bundle in un singolo bundle. Per ulteriori informazioni, vedere il modulo [[!UICONTROL Aggregator] in Adobe Workfront Fusion](../../workfront-fusion/modules/aggregator-module.md).

## [!UICONTROL Router]

Il modulo [!UICONTROL Router] ti consente di diramare il flusso in più route ed elaborare i dati all&#39;interno di ogni route in modo diverso. Quando un modulo [!UICONTROL Router] riceve un bundle, lo inoltra a ogni route connessa nell&#39;ordine in cui le route sono state collegate al modulo [!UICONTROL Router]. Per ulteriori informazioni, vedere [Modulo router in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/router-module.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Directives</h2>
<p>The error handling directives allow you to control how your scenario reacts to errors. For more information, see <a href="../../workfront-fusion/errors/advanced-error-handling.md" class="MCXref xref">Advanced error handling in Adobe Workfront Fusion</a> and <a href="../../workfront-fusion/errors/directives-for-error-handling.md" class="MCXref xref">Directives for error handling in Adobe Workfront Fusion</a>.</p>
</div>
-->
