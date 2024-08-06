---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Modulo Aggregator in Adobe Workfront Fusion
description: Un modulo aggregatore è un tipo di modulo progettato per unire diversi bundle di dati in un singolo bundle.
author: Becky
feature: Workfront Fusion
exl-id: cdc32842-8717-4e05-ab19-2661ee14c12c
source-git-commit: 948fe5fc249e0dcb04655f015c8e46493159c3ed
workflow-type: tm+mt
source-wordcount: '827'
ht-degree: 0%

---

# Modulo [!UICONTROL Aggregator] in [!DNL Adobe Workfront Fusion]

Un modulo aggregatore è un tipo di modulo progettato per unire diversi bundle di dati in un singolo bundle.

Per ulteriori informazioni sui tipi di moduli, vedere [Tipi di moduli](../../workfront-fusion/modules/module-types.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

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
  </tr> 
 </tbody> 
</table>

Per conoscere il piano, il tipo di licenza o l&#39;accesso disponibili, contattare l&#39;amministratore [!DNL Workfront].

Per informazioni sulle [!DNL Adobe Workfront Fusion] licenze, vedere [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

+++

## Panoramica del modulo [!UICONTROL Aggregator]

Durante l&#39;esecuzione di un modulo [!UICONTROL Aggregator], vengono eseguite le seguenti operazioni:

* Accumula tutti i bundle ricevuti durante il funzionamento di un singolo modulo di origine.
* Restituisce un singolo bundle con un array contenente un elemento per ogni bundle accumulato. Il contenuto degli elementi dell&#39;array dipende dal modulo [!UICONTROL Aggregator] e dalla relativa configurazione.

Nell&#39;immagine seguente viene illustrata una configurazione tipica del modulo [!UICONTROL Aggregator]:

![](assets/array-aggregator-350x190.png)

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Modulo Source]</p> </td> 
   <td> <p>Il modulo da cui inizia l’aggregazione del bundle. Il modulo sorgente è in genere un iteratore o un modulo di ricerca che produce una serie di bundle.</p><p>Quando si imposta il modulo di origine dell'aggregatore (e si chiude la relativa configurazione), il percorso tra il modulo di origine e il modulo dell'aggregatore viene racchiuso in un'area grigia in modo da poter vedere chiaramente l'inizio e la fine dell'aggregazione. 
   </p> <p>Per ulteriori informazioni sugli iteratori, vedere il modulo <a href="../../workfront-fusion/modules/iterator-module.md" class="MCXref xref">[!UICONTROL Iterator] in [!DNL Adobe Workfront Fusion]</a></p> <p>Per ulteriori informazioni sui moduli di ricerca, vedere moduli di ricerca in <a href="../../workfront-fusion/modules/module-types.md" class="MCXref xref">Tipi di moduli</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Tipo di struttura di destinazione]</p> </td> 
   <td> <p>(Applicabile solo per il modulo [!UICONTROL Array aggregator].) Struttura di destinazione in cui vengono aggregati i dati. L'opzione predefinita, [!UICONTROL Custom], consente di scegliere gli elementi da aggregare nell'elemento <code>Array </code> del bundle di output dell'aggregatore di array [!UICONTROL]:</p> <p> <img src="assets/output-bundle's-array-item-350x213.png" style="width: 350;height: 213;"> </p> <p>Dopo aver connesso altri moduli dopo il modulo [!UICONTROL Array aggregator] e aver ripristinato la configurazione del modulo, il menu a discesa del tipo di struttura [!UICONTROL Target] conterrà tutti i moduli seguenti e i relativi campi che sono di tipo "Array of Collections", come mostrato nel campo [!UICONTROL Attachments] del modulo [!DNL Slack] &gt;[!UICONTROL Create a Message]:</p> <p> <img src="assets/array-aggregator-slack-350x253.png" style="width: 350;height: 253;"> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Campi aggregati]</td> 
   <td>I campi che si desidera includere nell'output del modulo aggregatore.</td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Raggruppa per]</p> </td> 
   <td> <p>L'output dell'aggregatore può essere suddiviso in più gruppi con l'aiuto del campo [!UICONTROL Group by]. Il campo [!UICONTROL Group by] può contenere una formula valutata per il bundle di input di ogni aggregatore. L’aggregatore restituisce quindi un bundle per ogni valore di formula distinto. Ogni bundle contiene due elementi:</p> 
    <ul> 
     <li><code>Key </code>contiene il valore distinto.</li> 
     <li><code>Array </code>contiene i dati aggregati dai bundle per i quali la formula ha restituito il valore <code>Key </code>.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>Interrompi elaborazione dopo un'aggregazione vuota</p> </td> 
   <td> <p>Per impostazione predefinita, il modulo [!UICONTROL Aggregator] restituisce il risultato dell'aggregazione anche nel caso in cui nessun bundle abbia raggiunto il modulo [!UICONTROL Aggregator] (ad esempio, perché sono stati tutti esclusi durante il processo). Se l'opzione [!UICONTROL Interrompi elaborazione dopo un'aggregazione vuota] è abilitata, il modulo [!UICONTROL Aggregator] non produrrà alcun bundle di output in questo caso e il flusso verrà interrotto.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>I bundle generati dai moduli tra il modulo di origine e il modulo [!UICONTROL Aggregator] non vengono generati dal modulo [!UICONTROL Aggregator], pertanto non sono accessibili dai moduli nel flusso dopo [!UICONTROL Aggregator]. Se hai bisogno di dati da un bundle generato da un modulo tra il modulo di origine e il modulo [!UICONTROL Aggregator], assicurati di includere l&#39;elemento specificato nella configurazione del modulo [!UICONTROL Aggregator] (come nel campo [!UICONTROL Aggregated fields] nella configurazione del modulo [!UICONTROL Array aggregator]).


## Scenario di esempio del funzionamento degli aggregatori

Questo scenario di esempio mostra come comprimere tutti gli allegati e-mail e caricare il file ZIP in [!DNL Dropbox].

![](assets/dropbox-archive-350x87.png)

Lo scenario seguente mostra come:

* Il primo modulo controlla una cassetta postale per le e-mail in arrivo: [!UICONTROL E-mail] >[!UICONTROL Guarda le e-mail] il trigger restituirà un bundle con l&#39;elemento `Attachments[]`, che è un array contenente tutti gli allegati dell&#39;e-mail.

* Il secondo modello esegue l&#39;iterazione degli allegati dell&#39;e-mail: [!UICONTROL E-mail] >[!UICONTROL Itera allegati] L&#39;iteratore prende gli elementi dell&#39;array `Attachments[]` uno per uno e li invia ulteriormente come bundle separati.

* Il terzo modulo aggrega i bundle generati dal modulo [!UICONTROL E-mail] >[!UICONTROL Itera allegati]: [!UICONTROL Archivio] >[!UICONTROL Crea un aggregatore di archivio] accumula tutti i bundle che riceve ed restituisce un singolo bundle contenente il file ZIP.

* L&#39;ultimo modulo carica il file ZIP risultante in [!DNL Dropbox]: [!DNL Dropbox] > [!UICONTROL Carica un file] ottiene il file ZIP dall&#39;archivio [!UICONTROL Archivio] > [!UICONTROL Crea un archivio] e lo carica in [!DNL Dropbox].



Di seguito è riportato un esempio di configurazione dell&#39;aggregatore [!UICONTROL Archive] > [!UICONTROL Create an archive]:

![](assets/archive-create-an-archive-350x484.png)
