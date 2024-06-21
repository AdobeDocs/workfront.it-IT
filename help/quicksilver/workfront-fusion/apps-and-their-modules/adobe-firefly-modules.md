---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli Adobe Firefly
description: In un [!DNL Adobe Workfront Fusion] scenario, puoi automatizzare i flussi di lavoro che utilizzano [!DNL Adobe Firefly], oltre a collegarlo a più applicazioni e servizi di terze parti.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 1e131c27-571d-4099-9243-69572bdb3f5a
source-git-commit: f1821568ea69d370dc5b2e4cbaaf6b0a72f9fe7f
workflow-type: tm+mt
source-wordcount: '1274'
ht-degree: 0%

---

# [!DNL Adobe Firefly] moduli

In un [!DNL Adobe Workfront Fusion] scenario, puoi automatizzare i flussi di lavoro che utilizzano [!DNL Adobe Firefly], oltre a collegarlo a più applicazioni e servizi di terze parti.

Per istruzioni sulla creazione di uno scenario, consulta [Creare uno scenario](../../workfront-fusion/scenarios/create-a-scenario.md).

Per informazioni sui moduli, consulta [Moduli in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Requisiti di accesso

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza</td> 
   <td> <p>Nuovo: [!UICONTROL Standard]</p><p>Oppure</p><p>Corrente: [!UICONTROL Work] o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licenza**</td> 
   <td>
   <p>Corrente: No [!DNL Workfront Fusion] requisito di licenza.</p>
   <p>Oppure</p>
   <p>Legacy: qualsiasi </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>
   <p>Nuovo:</p> <ul><li>[!UICONTROL Select] o [!UICONTROL Prime] [!DNL Workfront] Piano: la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion].</li><li>[!UICONTROL Ultimate] [!DNL Workfront] Piano: [!DNL Workfront Fusion] è incluso.</li></ul>
   <p>Oppure</p>
   <p>Corrente: la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion].</p>
   </td> 
  </tr>
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, consulta [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Prerequisiti

Prima di utilizzare il [!DNL Adobe Firefly] connettore, è necessario assicurarsi che siano soddisfatti i seguenti prerequisiti:

* È necessario disporre di un [!DNL Adobe Firefly] account.

## Creare una connessione a [!DNL Adobe Firefly]

Per creare una connessione per [!DNL Adobe Firefly] moduli:

1. Clic **[!UICONTROL Aggiungi]** accanto alla casella Connessione.

1. Compila i campi seguenti:

   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
        <td role="rowheader">[!UICONTROL Nome connessione]</td>
        <td>
          <p>Immettere un nome per la connessione.</p>
        </td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Environment]</td>
        <td>Seleziona se ti connetti a un ambiente di produzione o non di produzione.</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Type]</td>
        <td>Specificare se ci si connette a un account di servizio o a un account personale.</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL ID client]</td>
        <td>Immetti il [!UICONTROL Adobe] [!UICONTROL ID client]. Questo si trova nella sezione dei dettagli [!UICONTROL Credentials] del [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Segreto client]</td>
        <td>Immetti il [!DNL Adobe] [!UICONTROL Segreto Client]. Questo si trova nella sezione dei dettagli [!UICONTROL Credentials] del [!DNL Adobe Developer Console]</td>
        </tr>
      </tbody>
    </table>

1. Clic **[!UICONTROL Continua]** per salvare la connessione e tornare al modulo.

## [!DNL Adobe Firefly] moduli e relativi campi

Quando si configura [!DNL Adobe Firefly] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL Adobe Firefly] I campi potrebbero essere visualizzati in base a fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se viene visualizzato il pulsante Mappa sopra un campo o una funzione, è possibile utilizzarlo per impostare variabili e funzioni per tale campo. Per ulteriori informazioni, consulta [Mappare le informazioni da un modulo all’altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Effettuare una chiamata API personalizzata

Questo modulo di azione effettua una chiamata personalizzata all’API di Firefly.

Per API specifiche disponibili, consulta [API ADOBE FIREFLY](https://developer.adobe.com/firefly-services/docs/firefly-api/) nella documentazione di Adobe Developer.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Per istruzioni sulla creazione di una connessione a [!DNL Adobe Firefly], vedi <a href="#create-a-connection-to-adobe-firefly" class="MCXref xref" >Creare una connessione a [!DNL Adobe Firefly]</a> in questo articolo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]</td>
      <td>
        <p>Inserisci un percorso relativo a <code>https://firefly-api-enterprise-stage.adobe.io/</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Method]</p>
      </td>
   <td> <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>Aggiungi le intestazioni della richiesta sotto forma di oggetto JSON standard.</p>
        <p>Ad esempio: <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] aggiunge automaticamente le intestazioni di autorizzazione.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>Aggiungi il contenuto body per la chiamata API sotto forma di oggetto JSON standard.</p> <p>Nota:  <p>Quando si utilizzano istruzioni condizionali quali <code>if</code> nel JSON, inserisci le virgolette al di fuori dell’istruzione condizionale.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

### Espandere un&#39;immagine

Questo modulo di azione espande un’immagine, facoltativamente con il contenuto di un prompt fornito.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Per istruzioni sulla creazione di una connessione a [!DNL Adobe Campaign], vedi <a href="#create-a-connection-to-adobe-firefly" class="MCXref xref" >Creare una connessione a [!DNL Adobe Firefly]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Prompt]</td> 
   <td>Immetti o mappa un prompt per il contenuto con cui desideri espandere l’immagine. Se non viene fornito alcun prompt, l’immagine viene espansa con contenuto corrispondente all’immagine originale.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Numero di varianti]</td> 
   <td>Immettere un numero compreso tra 1 e 4. Il modulo genera questo numero di varianti di immagine espanse.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Expanded image format]</td> 
   <td>Selezionare il formato di file con cui verrà salvata l'immagine espansa.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File di origine]</td> 
   <td>  <p>Selezionare un file di origine da un modulo precedente o mappare il nome del file di immagine e il file di immagine (dati) del file di origine.</p> </td> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Size]</td> 
   <td>Selezionare la dimensione desiderata per l'immagine espansa.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seed]</td> 
   <td>Inserisci o mappa un numero intero. Puoi utilizzare lo stesso valore di inizializzazione in un altro modulo Espandi un’immagine per generare un’immagine simile con stili diversi. </td> 
  </tr> 
 </tbody> 
</table>

## Riempi un’immagine

Questo modulo di azione riempie l’area nascosta di un’immagine, facoltativamente con il contenuto di un prompt fornito dall’utente.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Per istruzioni sulla creazione di una connessione a [!DNL Adobe Campaign], vedi <a href="#create-a-connection-to-adobe-firefly" class="MCXref xref" >Creare una connessione a [!DNL Adobe Firefly]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Prompt]</td> 
   <td>Immetti o mappa un prompt per il contenuto con cui desideri riempire l’immagine. Se non viene fornito alcun prompt, l’immagine verrà riempita con contenuto corrispondente all’immagine originale.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Numero di varianti]</td> 
   <td>Immettere un numero compreso tra 1 e 4. Il modulo genera questo numero di varianti di immagine riempite.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Formato immagine riempita]</td> 
   <td>Selezionate il formato di file con cui verrà salvata l'immagine riempita.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Image]</td> 
   <td>  <p> Clic <b>Aggiungi un'immagine</b>. Selezionare un file di origine da un modulo precedente o mappare il nome del file di origine e i dati immagine.</p> </td> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mask]</td> 
   <td>  <p> Clic <b>Aggiungi una maschera</b>. Selezionare un file di origine da un modulo precedente o mappare il nome del file di origine e i dati della maschera. Il file Maschera rappresenta la maschera personalizzata che verrà riempita con il contenuto generato.</p> </td> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Size]</td> 
   <td>Selezionate la dimensione desiderata per l'immagine riempita.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seed]</td> 
   <td>Inserisci o mappa un numero intero. Puoi utilizzare lo stesso valore di inizializzazione in un altro modulo Espandi un’immagine per generare un’immagine simile con stili diversi. </td> 
  </tr> 
 </tbody> 
</table>

## Generare un’immagine

Questo modulo di azione genera un’immagine e in base a un prompt fornito. È inoltre possibile fornire un&#39;immagine di riferimento facoltativa. L&#39;immagine generata corrisponderà allo stile dell&#39;immagine di riferimento.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Per istruzioni sulla creazione di una connessione a [!DNL Adobe Campaign], vedi <a href="#create-a-connection-to-adobe-firefly" class="MCXref xref" >Creare una connessione a [!DNL Adobe Firefly]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Prompt]</td> 
   <td>Immettete o mappate un prompt per l'immagine da creare. Un maggior numero di dettagli nel prompt consente un maggiore controllo su ciò che appare nell'immagine.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Numero di varianti]</td> 
   <td>Immettere un numero compreso tra 1 e 4. Il modulo genera questo numero di varianti di immagine.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Generated image format]</td> 
   <td>Selezionare il formato di file con cui verrà salvata l'immagine espansa. Se si seleziona predefinito, il formato del file sarà JPEG se non viene fornita alcuna immagine di riferimento. Se viene fornita un’immagine di riferimento, il formato del file dell’immagine generata sarà lo stesso dell’immagine di riferimento.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File di origine]</td> 
   <td>  <p>Selezionare un file di origine da un modulo precedente o mappare il nome del file di immagine di riferimento e il file di immagine di riferimento (dati) del file di origine. L’immagine generata viene creata in modo che corrisponda allo stile dell’immagine di riferimento.</p> </td> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Predefiniti]</td> 
   <td>Se si desidera utilizzare uno stile predefinito, fare clic su Aggiungi elemento e immettere o mappare lo stile che si desidera utilizzare.<p>Per un elenco degli stili predefiniti, consulta <a href="https://developer.adobe.com/firefly-services/docs/firefly-api/guides/concepts/styles/" >Stili modello immagine</a> nella documentazione per gli sviluppatori Adobe.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Negative prompt]</td> 
   <td>Immetti o mappa le parole da evitare nel contenuto generato. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Classe Content]</td> 
   <td>Seleziona se desideri che l'immagine generata sia più simile a una foto o più simile a un'immagine creata. <ul><li><b>Foto</b><p>Immettete i valori per l'apertura, la velocità dell'otturatore (in secondi) e il campo visivo (in millimetri).</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seed]</td> 
   <td>Inserisci o mappa un numero intero. Puoi utilizzare lo stesso valore di inizializzazione in un altro modulo Espandi un’immagine per generare un’immagine simile con stili diversi. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Size]</td> 
   <td>Seleziona la dimensione desiderata per l'immagine generata.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL]</td> 
   <td>Immettete o mappate un numero intero che rappresenta l'intensità con cui l'immagine generata corrisponderà allo stile dello stile predefinito o dell'immagine di riferimento. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Intensità visiva]</td> 
   <td>Immettere o mappare un numero intero che rappresenta l'intensità complessiva delle caratteristiche visive esistenti della foto. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Locale]</td> 
   <td>Se viene fornita una lingua, il modulo genera contenuto più pertinente alla lingua specificata. <p>Le impostazioni internazionali devono essere specificate nel codice della lingua ISO 639-1 e nell'area geografica ISO 3166-1.</p><p> Esempio: <code>en-US</code></p></td> 
  </tr> 
 </tbody> 
</table>
