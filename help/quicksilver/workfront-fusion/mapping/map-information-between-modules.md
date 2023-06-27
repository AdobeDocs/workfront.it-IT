---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Mappare le informazioni da un modulo all’altro in [!DNL Adobe Workfront Fusion]
description: La mappatura è il processo di assegnazione degli output di un modulo, strutturati in elementi, ai campi di input di un altro modulo.
author: Becky
feature: Workfront Fusion
exl-id: e8d619e9-6425-4136-ac71-47d979d68a2d
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1563'
ht-degree: 0%

---

# Mappare le informazioni da un modulo all’altro in [!DNL Adobe Workfront Fusion]

La mappatura è il processo di assegnazione degli output di un modulo, strutturati in elementi, ai campi di input di un altro modulo.

Il pannello di mappatura viene visualizzato quando si fa clic su un campo in cui si desidera inserire un valore generato da un modulo precedente in uno scenario. All’interno di un modulo, in qualsiasi campo disponibile per la mappatura, puoi creare una formula utilizzando qualsiasi combinazione di funzioni ed elementi mappati dal pannello di mappatura con testo statico digitato. Questi elementi possono essere nidificati l’uno nell’altro.

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

## Bundle ed elementi

Il funzionamento di un modulo produce zero, uno o più bundle come output. Un bundle è costituito da uno o più elementi.

Per esplorare l’output di un modulo:

1. Clic **[!UICONTROL Esegui una volta]** per eseguire il modulo.
1. Fai clic sulla bolla sopra il modulo.

   Viene visualizzato un registro contenente tutte le fasi del modulo. Puoi trovare il bundle o i bundle generati dalla fase operativa di un modulo sotto **[!UICONTROL Output]** intestazione. Ogni bundle contiene i relativi elementi e i valori di ciascun elemento.

>[!INFO]
>
>**Esempio:** Questo esempio mostra il modulo [!UICONTROL E-mail] > [!UICONTROL Guarda le e-mail]. Puoi vedere che ha eseguito 1 operazione producendo un singolo bundle che contiene vari elementi come `Date`, `Email ID (UID)`, `size`e così via.
>
>![](assets/watch-emails-350x298.png)

>[!NOTE]
>
>Gli output dei moduli racchiusi tra [!UICONTROL Iteratore] e [!UICONTROL Aggregatore] non sono accessibili oltre il [!UICONTROL Aggregatore] modulo.

## Mappare un elemento

Dopo aver creato una sequenza di moduli collegandone due o più, ogni modulo può elaborare i valori degli elementi generati dai moduli che lo precedono.

Per assegnare gli elementi ai campi di input di un modulo:

1. Fai clic sul modulo che deve elaborare l’output del modulo o dei moduli precedenti.
1. Nel pannello Impostazioni modulo visualizzato, fai clic su un campo in cui desideri utilizzare il valore di un elemento prodotto da uno o più moduli precedenti.

   Viene visualizzato il pannello di mappatura.

1. Fai clic su un elemento dal pannello di mappatura per inserirlo nel campo.
1. (Facoltativo) Per cercare un campo specifico nel pannello di mappatura, fate clic sulla barra di ricerca del pannello di mappatura e digitate il termine da cercare. Fare clic sul campo quando viene visualizzato nell&#39;elenco.

   I risultati della ricerca contengono il termine di ricerca e non fanno distinzione tra maiuscole e minuscole.

Per ulteriori informazioni, consulta [Configurare le impostazioni di un modulo in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/configure-a-modules-settings.md).

## Formule

Puoi mappare più elementi in un campo, combinarli con valori letterali (valori fissi) e utilizzare operatori e funzioni per creare formule complesse:

![](assets/operators-and-functions-350x187.png)

Puoi trovare le funzioni e gli operatori nel pannello di mappatura sotto una delle relative schede.

![](assets/functions-toolbar-350x189.png)

La prima scheda ![](assets/toolbar-icon-functions-you-map-from-other-modules.png) (mostrato all’apertura del pannello) mostra gli elementi che è possibile mappare da altri moduli.

Le altre schede contengono i seguenti tipi di funzioni:

* **Funzioni generali** ![](assets/toolbar-icon-general-function.png) - Consulta [Funzioni generali in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/general-functions.md) per ulteriori informazioni.

* **Funzioni matematica** ![](assets/toolbar-icon-math-functions.png) - Consulta [Funzioni matematiche in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/math-functions.md) per ulteriori informazioni.

* **Funzioni di testo e binarie** ![](assets/toolbar-icon-text&binary-functions.png) - Consulta [Funzioni stringa in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/string-functions.md) per ulteriori informazioni.

* **Data e ora** ![](assets/toolbar-icon-date&time-functions.png) - Consulta [Funzioni data e ora in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/date-and-time-functions.md) e gli articoli seguenti per ulteriori informazioni.

   * [Token per la formattazione di data e ora in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md)
   * [Token per l’analisi di data e ora in Adobe Workfront Fusion](../../workfront-fusion/functions/tokens-for-date-and-time-parsing.md)

* **Funzioni per l&#39;utilizzo degli array** ![](assets/toolbar-icon-functions-for-arrays.png) - Consulta [Funzioni array in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/array-functions.md) per ulteriori informazioni.

>[!TIP]
>
>Quando si crea una formula complessa che si desidera riutilizzare in un altro campo, è possibile fare clic sul campo che contiene la combinazione, utilizzare Comando-A o Ctrl-A per selezionarla, quindi copiarla e incollarla nell&#39;altro campo.

Per ulteriori informazioni sulla mappatura degli elementi tramite le funzioni, vedere [Mappare gli elementi utilizzando le funzioni in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/map-using-functions.md).

## Raccolte

Alcuni elementi possono contenere più valori di vari tipi. Si tratta di elementi di tipo raccolta.

È possibile identificare un [!UICONTROL raccolta] digita l’elemento in base al piccolo rettangolo nero visualizzato a destra dell’etichetta dell’elemento e del relativo elenco di elementi secondari espanso automaticamente:

![](assets/collection.png)

>[!NOTE]
>
>Nella maggior parte dei casi, è possibile mappare gli elementi secondari della raccolta anziché l&#39;elemento che rappresenta l&#39;intera raccolta.

Per ulteriori informazioni sulle raccolte, consulta [Tipi di dati degli elementi in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md)

## Array

Alcuni elementi possono contenere più elementi dello stesso tipo. Si tratta di elementi di tipo array.

È possibile identificare un elemento di tipo matrice tramite le parentesi quadre alla fine dell&#39;etichetta dell&#39;elemento. Fare clic sul piccolo rettangolo nero a destra dell&#39;etichetta dell&#39;elemento per visualizzare gli elementi dell&#39;elemento:

![](assets/array.png)

Per ulteriori informazioni sugli array, vedere [Tipi di dati degli elementi in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md)

### Mappare il primo elemento di un array

Se mappate i `Recipient name` elemento, viene visualizzato nel campo come segue:

![](assets/map-array-1st-element.png)

Il numero tra parentesi quadre è un indice che determina quale elemento della matrice verrà utilizzato. È impostato su 1 per impostazione predefinita.

### Mappare l’elemento n-esimo di un array

Se desideri accedere a un altro elemento, fai clic sulle parentesi quadre e modifica il valore dell’indice:

![](assets/access-another-element.png)

### Mappare l’elemento di un array con una determinata chiave

Alcuni array contengono diverse raccolte con elementi chiave e valore. Si tratta in genere di vari metadati, attributi e così via.

L’esempio seguente mostra l’output del [!DNL Jira] App.

![](assets/output-of-jira-app-350x100.png)

In questo esempio, si ottiene un nome di file da un array di allegati per l’allegato specifico con un ID di 10108.

L’output di [!DNL Jira] ha un aspetto simile al seguente:

![](assets/output-from-jira-350x261.png)

Il requisito tipico è quello di cercare un elemento in base al suo dato valore chiave e ottenere il valore corrispondente dall&#39;elemento valore. Ciò può essere ottenuto con una formula che utilizza una combinazione di `map()` e `get()` funzioni.

Di seguito è riportata una ripartizione dettagliata della formula:

1. Il primo parametro del `map()` è l&#39;intero elemento array.
1. Il secondo parametro è il nome non elaborato dell&#39;elemento valore. Per ottenere il nome non elaborato, passa il cursore del mouse sull’elemento nella [!UICONTROL mappatura] pannello:

   ![](assets/obtain-raw-name-350x124.png)

   >[!NOTE]
   >
   >Tutti i parametri fanno distinzione tra maiuscole e minuscole. Anche se in questo particolare esempio l’etichetta dell’elemento differisce dal suo nome non elaborato solo in maiuscolo, è necessario utilizzare il nome non elaborato, che è tutto un valore minuscolo a differenza dell’etichetta Valore.

1. Il terzo parametro è il nome non elaborato dell’elemento chiave:

   ![](assets/3rd-parameter-350x166.png)

1. Il quarto parametro rappresenta il valore chiave specificato.

Perché il `map()` funzione restituisce un array (poiché potrebbero esserci più elementi con il valore chiave specificato), è necessario applicare il `get()` funzione per ottenere il primo elemento:

* Il primo parametro del `get()` funzione è il risultato della `map()` funzione.

* Il secondo parametro è l’indice dell’elemento, ovvero uno.

Per ulteriori informazioni su `map()` funzione, vedi [Funzioni array in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/array-functions.md).

Per ulteriori informazioni su `get()` funzione, vedi [Funzioni generali in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/general-functions.md).

## Conversione di elementi in una serie di bundle

Gli array possono essere convertiti in una serie di bundle utilizzando [!UICONTROL Iteratore] modulo. Per ulteriori informazioni, consulta [[!UICONTROL Iteratore] modulo in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).

![](assets/series-of-bundles-350x169.png)

## Risoluzione dei problemi

### Elementi mancanti nel pannello di mappatura

Per ogni modulo, il pannello di mappatura visualizza tutti gli elementi di output elencati dall’autore del modulo. In alcuni casi, l’elenco potrebbe essere incompleto per vari motivi e alcuni elementi potrebbero mancare. [!DNL Workfront Fusion] può rilevare automaticamente gli elementi di output mancanti quando esegui il modulo nell’editor di scenari. La procedura esatta varia leggermente a seconda del tipo di modulo:

#### Trigger istantaneo

1. Fai clic con il pulsante destro del mouse sul modulo, quindi fai clic su **[!UICONTROL Esegui solo questo modulo]** nel menu visualizzato.

   Se non sono presenti webhook in coda, il modulo attende l’elaborazione di un nuovo webhook.

1. Genera un webhook.

   Ad esempio, il modulo webhook **[!DNL Slack]>[!UICONTROL Ascolta nuovi eventi]** (ricerca di nuovi messaggi del canale in un canale) invia un messaggio al canale.

1. Al termine dell’esecuzione del modulo, fai clic sulla bolla sopra il modulo per esplorarne l’output completo.

   Il pannello di mappatura contiene tutti gli elementi individuati nell’output del modulo.

#### Trigger di polling

1. Fai clic con il pulsante destro del mouse sul modulo, quindi fai clic su **[!UICONTROL Esegui solo questo modulo]** nel menu visualizzato.
1. In assenza di output, fare clic su **[!UICONTROL Scegli da dove iniziare]** e regolare le impostazioni.
1. Se non è presente alcun evento da elaborare, creane uno e torna al passaggio 2.

   Ad esempio, il modulo webhook **[!UICONTROL Gmail] >[!UICONTROL Guarda le e-mail]** invia un’e-mail alla cartella che il modulo sta guardando.

1. Al termine dell’esecuzione del modulo, fai clic sulla bolla sopra il modulo per esplorarne l’output completo.

   Il pannello di mappatura ora contiene tutti gli elementi individuati nell’output del modulo.

#### Altri moduli

Puoi scegliere di eseguire:

* L&#39;intero scenario (o solo la parte contenente il modulo)

  Se lo scenario inizia con un trigger, consulta [Trigger istantaneo](#instant-trigger) o [Trigger di polling](#polling-trigger) sopra.

* Solo il modulo singolo

Se scegli di eseguire solo il modulo singolo:

1. Fai clic con il pulsante destro del mouse sul modulo, quindi fai clic su **[!UICONTROL Esegui solo questo modulo]** nel menu visualizzato.
1. Fornisci valori di esempio per gli elementi di input, quindi fai clic su **[!UICONTROL OK]** .
1. Al termine dell’esecuzione del modulo, fai clic sulla bolla sopra il modulo per esplorarne l’output completo.

   Il pannello di mappatura ora contiene tutti gli elementi individuati nell’output del modulo.
