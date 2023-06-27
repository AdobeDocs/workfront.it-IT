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
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 0%

---

# [!UICONTROL Aggregatore] modulo in [!DNL Adobe Workfront Fusion]

Un modulo aggregatore è un tipo di modulo progettato per unire diversi bundle di dati in un singolo bundle.

Per ulteriori informazioni sui tipi di modulo, vedi [Tipi di moduli](../../workfront-fusion/modules/module-types.md).

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
  </tr> 
 </tbody> 
</table>

Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, consulta [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL Aggregatore] modulo

Quando un [!UICONTROL Aggregatore] viene eseguito, esegue le seguenti operazioni:

* Accumula tutti i bundle ricevuti durante il funzionamento di un singolo modulo di origine.
* Restituisce un singolo bundle con un array contenente un elemento per ogni bundle accumulato. Il contenuto degli elementi dell’array dipende da [!UICONTROL Aggregatore] e la relativa configurazione.

L&#39;immagine seguente mostra una configurazione tipica della [!UICONTROL Aggregatore] modulo :

![](assets/array-aggregator-350x190.png)

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Source Module]</p> </td> 
   <td> <p>Il modulo da cui inizierà l’aggregazione del bundle. Il modulo sorgente è in genere un iteratore o un modulo di ricerca che produce una serie di bundle. Quando si imposta il modulo di origine dell'aggregatore (e si chiude la relativa configurazione), il percorso tra il modulo di origine e il modulo dell'aggregatore viene racchiuso in un'area grigia in modo da poter vedere chiaramente l'inizio e la fine dell'aggregazione. 
   </p> <p>Per ulteriori informazioni sugli iteratori, consulta <a href="../../workfront-fusion/modules/iterator-module.md" class="MCXref xref">Modulo [!UICONTROL Iterator] in [!DNL Adobe Workfront Fusion]</a></p> <p>Per ulteriori informazioni sui moduli di ricerca, consulta Moduli di ricerca in <a href="../../workfront-fusion/modules/module-types.md" class="MCXref xref">Tipi di moduli</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Tipo di struttura di destinazione]</p> </td> 
   <td> <p>(Applicabile solo per il modulo [!UICONTROL Array aggregator].) La struttura obiettivo in cui i dati sono aggregati. L'opzione predefinita, [!UICONTROL Custom], consente di scegliere gli elementi da aggregare nel bundle di output di A[!UICONTROL ray aggregator] <code>Array </code>elemento:</p> <p> <img src="assets/output-bundle's-array-item-350x213.png" style="width: 350;height: 213;"> </p> <p>Dopo aver connesso altri moduli dopo il modulo [!UICONTROL Array aggregator] e aver ripristinato la configurazione del modulo, il menu a discesa del tipo di struttura [!UICONTROL Target] conterrà tutti i moduli seguenti e i relativi campi di tipo Array of Collections, come illustrato nel campo [!UICONTROL Attachments] del [!DNL Slack] &gt;[!UICONTROL Crea un messaggio] modulo:</p> <p> <img src="assets/array-aggregator-slack-350x253.png" style="width: 350;height: 253;"> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Campi aggregati]</td> 
   <td>Selezionare i campi che si desidera includere nell'output del modulo aggregatore.</td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Raggruppa per]</p> </td> 
   <td> <p>L'output dell'aggregatore può essere suddiviso in più gruppi con l'aiuto del campo [!UICONTROL Group by]. Il campo [!UICONTROL Group by] può contenere una formula valutata per il bundle di input di ogni aggregatore. L’aggregatore restituisce quindi un bundle per ogni valore di formula distinto. Ogni bundle contiene due elementi:</p> 
    <ul> 
     <li><code>Key </code>contiene il valore distinto.</li> 
     <li><code>Array </code>contiene i dati aggregati dai bundle per i quali la formula ha valutato l'attributo <code>Key </code>valore.</li> 
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
>Bundle generati dai moduli tra il modulo di origine e [!UICONTROL Aggregatore] non sono generati da [!UICONTROL Aggregatore] , in modo che non siano accessibili dai moduli nel flusso dopo [!UICONTROL Aggregatore]. Se hai bisogno di dati provenienti da un bundle generato da un modulo tra il modulo sorgente e [!UICONTROL Aggregatore] , assicurati di includere l&#39;elemento specificato nel [!UICONTROL Aggregatore] configurazione del modulo (come nella [!UICONTROL Campi aggregati] nella configurazione del [!UICONTROL Aggregatore array] modulo ).


>[!INFO]
>
>**Esempio:** Caso d’uso: compressione di tutti gli allegati e-mail e caricamento del file ZIP in [!DNL Dropbox]
>
>Lo scenario seguente mostra come:
>
>* Controlla le e-mail in arrivo in una cassetta postale: [!UICONTROL E-mail] >[!UICONTROL Guarda le e-mail] il trigger genera un bundle con l&#39;elemento `Attachments[]`, che è un array contenente tutti gli allegati dell’e-mail.
>
>* Itera gli allegati dell’e-mail: [!UICONTROL E-mail] >[!UICONTROL Itera allegati] iteratore prende gli elementi dal `Attachments[]` array uno per uno e li invia ulteriormente come bundle separati.
>
>* Aggrega i bundle generati da [!UICONTROL E-mail] >[!UICONTROL Itera allegati] modulo: [!UICONTROL Archivia] >[!UICONTROL Creare un aggregatore di archivi] accumula tutti i bundle che riceve ed emette un singolo bundle contenente il file ZIP.
>
>* Carica il file ZIP risultante in [!DNL Dropbox]: [!DNL Dropbox] > [!UICONTROL Carica un file] ottiene il file ZIP da [!UICONTROL Archivia] > [!UICONTROL Creare un archivio] e lo carica su [!DNL Dropbox].
>
>![](assets/dropbox-archive-350x87.png)
>
>Di seguito è riportato un esempio di configurazione di [!UICONTROL Archivia] > [!UICONTROL Creare un archivio] aggregatore:
>
>![](assets/archive-create-an-archive-350x484.png)
