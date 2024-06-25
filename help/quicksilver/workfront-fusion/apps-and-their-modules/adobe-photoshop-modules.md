---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli Adobe Photoshop
description: Con i moduli di Adobe Photoshop, puoi avviare uno scenario Adobe Workfront Fusion basato sugli eventi nell’account Adobe Photoshop, creare, leggere o aggiornare contratti e altri record, cercare i record utilizzando i criteri impostati e caricare i documenti.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: f20192ea-e363-4fba-8bd2-b1d50443918d
source-git-commit: 6bcf404432129a812b5e4d840b59e72f036ec723
workflow-type: tm+mt
source-wordcount: '1547'
ht-degree: 0%

---

# [!DNL Adobe Photoshop] moduli

In un [!DNL Adobe Workfront Fusion] scenario, puoi automatizzare i flussi di lavoro che utilizzano [!DNL Adobe Photoshop], oltre a collegarlo a più applicazioni e servizi di terze parti.


Per istruzioni sulla creazione di uno scenario, consulta [Creare uno scenario](../../workfront-fusion/scenarios/create-a-scenario.md).

Per informazioni sui moduli, consulta [Moduli in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Requisiti di accesso

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] piano*</td>
      <td>
        <p>[!UICONTROL Pro] o versione successiva</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] licenza*</td>
      <td>
        <p>[!UICONTROL Plan], [!UICONTROL Work]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront Fusion] licenza**</td>
      <td >
        <p>[!UICONTROL Workfront Fusion per l'automazione e l'integrazione del lavoro]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Prodotto</td>
      <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare la funzionalità descritta in questo articolo.</td>
    </tr>
    </tr>
  </tbody>
</table>


&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.

&#42;&#42;Per informazioni su [!DNL Adobe Workfront Fusion] licenze, consulta [!DNL [Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Prerequisiti

Prima di utilizzare il [!DNL Adobe Photoshop] connettore, è necessario assicurarsi che siano soddisfatti i seguenti prerequisiti:

* È necessario disporre di un [!DNL Adobe Photoshop] account.

## Creare una connessione a [!DNL Adobe Photoshop]

Per creare una connessione per [!DNL Adobe Photoshop] moduli:

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
        <td role="rowheader">[!UICONTROL ID client]</td>
        <td>Immetti il [!UICONTROL Adobe] [!UICONTROL ID client]. Questo si trova nella sezione dei dettagli [!UICONTROL Credentials] del [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Segreto client]</td>
        <td>Immetti il [!DNL Adobe] [!UICONTROL Segreto Client]. Questo si trova nella sezione dei dettagli [!UICONTROL Credentials] del [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL ID account tecnico]</td>
        <td>Immetti il [!DNL Adobe] [!UICONTROL ID account tecnico]. Questo si trova nella sezione dei dettagli [!UICONTROL Credentials] del [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL ID organizzazione]</td>
        <td>Immetti il [!DNL Adobe] [!UICONTROL ID organizzazione]. Questo si trova nella sezione dei dettagli [!UICONTROL Credentials] del [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Chiave privata]</td>
        <td>
          <p>Immetti la chiave privata generata al momento della creazione delle credenziali in [!DNL Adobe Developer Console]. </p>
          <p>Per estrarre la chiave privata o il certificato:</p>
          <ol>
            <li value="1">
              <p>Clic <b>[!UICONTROL Extract]</b>.</p>
            </li>
            <li value="2">
              <p>Selezionare il tipo di file da estrarre.</p>
            </li>
            <li value="3">
              <p>Seleziona il file che contiene la chiave privata o il certificato.</p>
            </li>
            <li value="4">
              <p>Immettere la password per il file.</p>
            </li>
            <li value="5">
              <p>Clic <b>Salva</b> per estrarre il file e tornare alla configurazione della connessione [!UICONTROL ]e.</p>
            </li>
          </ol>
        </td>
        </tr>
      </tbody>
    </table>

1. Clic **[!UICONTROL Continua]** per salvare la connessione e tornare al modulo.

## [!DNL Adobe Photoshop] moduli e relativi campi

Quando si configura [!DNL Adobe Photoshop] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL Adobe Photoshop] I campi potrebbero essere visualizzati in base a fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se viene visualizzato il pulsante Mappa sopra un campo o una funzione, è possibile utilizzarlo per impostare variabili e funzioni per tale campo. Per ulteriori informazioni, consulta [Mappare le informazioni da un modulo all’altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)


### Azioni

* [Crea un nuovo PSD](#create-a-new-psd)
* [Modificare i livelli di testo](#edit-text-layers)
* [Esegui sfocatura profondità](#execute-depth-blur)
* [Eseguire azioni Photoshop](#execute-photoshop-actions)
* [Esegui ritaglio prodotto](#execute-product-crop)
* [Ottieni informazioni livello](#get-layer-info)
* [Effettuare una chiamata API personalizzata](#make-a-custom-api-call)

#### Crea un nuovo PSD

Questo modulo di azione crea un nuovo PSD con livelli facoltativi e genera rappresentazioni o salva come PSD.

Per i campi relativi a questo modulo, consulta [Crea un nuovo PSD](https://developer.adobe.com/photoshop/photoshop-api-docs/api/#tag/Photoshop/operation/documentCreate) nella documentazione di Adobe Photoshop.

#### Modificare i livelli di testo

Questo modulo di azione modifica i livelli di testo in un file Photoshop.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Per istruzioni sulla creazione di una connessione a [!DNL Adobe Photoshop], vedi <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Creare una connessione a [!DNL Adobe Photoshop]</a> in questo articolo.</td>
    </tr>
    <tr>
      <td role="rowheader">Archiviazione file di input [!UICONTROL]</td>
      <td>
        <p>Selezionare il servizio file in cui è memorizzato il file che si desidera modificare.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL file di input]</p>
      </td>
   <td> Immetti o mappa l’URL o il percorso del file da modificare. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Gestisci tipi di carattere mancanti]</td>
      <td>
        <p>Selezionare l'azione da eseguire se nel documento mancano uno o più tipi di carattere. Se il font non viene fornito, il modulo utilizza il font predefinito.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Default font]  </td>
      <td>
        <p>Immettere il nome postscript completo del tipo di carattere da utilizzare come predefinito globale per il documento. Questo tipo di carattere verrà utilizzato per qualsiasi livello di testo con un tipo di carattere mancante e nessun altro tipo di carattere è stato specificato per tale livello. Se questo tipo di carattere non è presente, verrà applicata l'opzione specificata in Gestione tipi di carattere mancanti.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Livelli]</td>
   <td> <p>Per informazioni dettagliate sulle opzioni dei livelli, consultate <a href="https://developer.adobe.com/photoshop/photoshop-api-docs/api/#tag/Photoshop/operation/text">Modifica livello testo</a> nella documentazione di Adobe Photoshop.</p>  </td>     </tr>
    <tr>
      <td role="rowheader">Archiviazione file di output di [!UICONTROL]</td>
      <td>
        <p>Selezionare il servizio file in cui si desidera memorizzare il file modificato.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL file di output]</p>
      </td>
   <td> Inserisci o mappa l’URL o il percorso in cui verrà memorizzato il file modificato. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Tipo di file di output]</p>
      </td>
   <td> Selezionare il tipo di file per il file modificato. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Overwrite]</td>
      <td>
        <p>Seleziona se il file appena modificato sovrascriverà eventuali file di output già esistenti.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Compression]</p>
      </td>
   <td> Selezionare il livello di compressione per il file di output. </td> 
    </tr>
  </tbody>
</table>

#### Esegui sfocatura profondità

Questo modulo di azione esegue Sfocatura profondità sul file selezionato.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Per istruzioni sulla creazione di una connessione a [!DNL Adobe Photoshop], vedi <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Creare una connessione a [!DNL Adobe Photoshop]</a> in questo articolo.</td>
    </tr>
    <tr>
      <td role="rowheader">Archiviazione file di input [!UICONTROL]</td>
      <td>
        <p>Selezionare il servizio file in cui è memorizzato il file che si desidera modificare.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL file di input]</p>
      </td>
   <td> Immetti o mappa l’URL o il percorso del file da modificare. </td> 
    </tr>
    <tr>
      <td role="rowheader">Archiviazione file di output di [!UICONTROL]</td>
      <td>
        <p>Selezionare il servizio file in cui si desidera memorizzare il file modificato.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL file di output]</p>
      </td>
   <td> Inserisci o mappa l’URL o il percorso in cui verrà memorizzato il file modificato. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Tipo di file di output]</p>
      </td>
   <td> Selezionare il tipo di file per il file modificato. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Altri campi]</td>
      <td>
        <p>Per informazioni dettagliate sulle altre opzioni di Sfocatura profondità, consultate <a href="https://developer.adobe.com/photoshop/photoshop-api-docs/api/#tag/Photoshop/operation/depthBlur">Esegui sfocatura profondità </a>nella documentazione API di Adobe Photoshop.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Overwrite]</td>
      <td>
        <p>Seleziona se il file appena modificato sovrascriverà eventuali file di output già esistenti.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Compression]</p>
      </td>
   <td> Selezionare il livello di compressione per il file di output. </td> 
    </tr>
  </tbody>
</table>

#### Esegui azioni Photoshop

Questo modulo di azione esegue un’azione Photoshop sull’immagine selezionata.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Per istruzioni sulla creazione di una connessione a [!DNL Adobe Photoshop], vedi <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Creare una connessione a [!DNL Adobe Photoshop]</a> in questo articolo.</td>
    </tr>
    <tr>
      <td role="rowheader">Archiviazione file di input [!UICONTROL]</td>
      <td>
        <p>Selezionare il servizio file in cui è memorizzato il file che si desidera modificare.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL file di input]</p>
      </td>
   <td> Immetti o mappa l’URL o il percorso del file da modificare. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Archiviazione file azioni]</td>
      <td>
        <p>Selezionare il file service in cui è memorizzato il file di azioni.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL file azioni]</p>
      </td>
   <td> Inserisci o mappa l’URL o il percorso del file delle azioni. </td> 
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Nome azione]</p>
      </td>
   <td> Se si desidera eseguire solo una determinata azione, è possibile specificare l'azione da eseguire dal set di azioni. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Font / Pattern / Archiviazione pennello]</td>
      <td>
        <p>Selezionare il servizio file in cui è memorizzato il file che si desidera utilizzare.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Font / Pattern / URL file pennello]</p>
      </td>
   <td> Inserisci o mappa l’URL o il percorso del file che desideri utilizzare. </td> 
    </tr>
    <tr>
      <td role="rowheader">Archiviazione file di output di [!UICONTROL]</td>
      <td>
        <p>Selezionare il servizio file in cui si desidera memorizzare il file modificato.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL file di output]</p>
      </td>
   <td> Inserisci o mappa l’URL o il percorso in cui verrà memorizzato il file modificato. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Tipo di file di output]</p>
      </td>
   <td> Selezionare il tipo di file per il file modificato. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Overwrite]</td>
      <td>
        <p>Seleziona se il file appena modificato sovrascriverà eventuali file di output già esistenti.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Compression]</p>
      </td>
   <td> Selezionare il livello di compressione per il file di output. </td> 
    </tr>
  </tbody>
</table>

#### Esegui ritaglio prodotto

Questo modulo di azione esegue il ritaglio prodotto sull’immagine selezionata.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Per istruzioni sulla creazione di una connessione a [!DNL Adobe Photoshop], vedi <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Creare una connessione a [!DNL Adobe Photoshop]</a> in questo articolo.</td>
    </tr>
    <tr>
      <td role="rowheader">Archiviazione file di input [!UICONTROL]</td>
      <td>
        <p>Selezionare il servizio file in cui è memorizzato il file da ritagliare.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL file di input]</p>
      </td>
   <td> Inserisci o mappa l’URL o il percorso del file da ritagliare. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Unit]</p>
      </td>
   <td> Selezionate se desiderate descrivere la regolazione di altezza e larghezza in pixel o come percentuale. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Width]</p>
      </td>
   <td> Immettete o mappate la spaziatura che desiderate aggiungere. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Height]</p>
      </td>
   <td> Immettete o mappate la quantità di spazio per l'altezza che desiderate aggiungere. </td> 
    </tr>
    <tr>
      <td role="rowheader">Archiviazione file di output di [!UICONTROL]</td>
      <td>
        <p>Selezionare il servizio file in cui si desidera memorizzare il file modificato.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL file di output]</p>
      </td>
   <td> Inserisci o mappa l’URL o il percorso in cui verrà memorizzato il file modificato. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Tipo di file di output]</p>
      </td>
   <td> Selezionare il tipo di file per il file modificato. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Overwrite]</td>
      <td>
        <p>Seleziona se il file appena modificato sovrascriverà eventuali file di output già esistenti.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Compression]</p>
      </td>
   <td> Selezionare il livello di compressione per il file di output. </td> 
    </tr>
  </tbody>
</table>

#### Ottieni informazioni livello

Questo modulo di azione recupera le informazioni sui livelli dal file PSD specificato.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Per istruzioni sulla creazione di una connessione a [!DNL Adobe Photoshop], vedi <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Creare una connessione a [!DNL Adobe Photoshop]</a> in questo articolo.</td>
    </tr>
    <tr>
      <td role="rowheader">Archiviazione file di input [!UICONTROL]</td>
      <td>
        <p>Selezionate il servizio file da cui memorizzare il file da cui desiderate recuperare le informazioni sui livelli.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL file di input]</p>
      </td>
   <td> Immettete o mappate l'URL o il percorso del file da cui desiderate recuperare le informazioni sui livelli. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL miniature]</p>
      </td>
   <td> </td> 
    </tr>
  </tbody>
</table>

#### Effettuare una chiamata API personalizzata

Questo modulo di azione effettua una chiamata personalizzata all’API Photoshop.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Per istruzioni sulla creazione di una connessione a [!DNL Adobe Photoshop], vedi <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Creare una connessione a [!DNL Adobe Photoshop]</a> in questo articolo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]</td>
      <td>
        <p>Inserisci un percorso relativo a <code>https://image.adobe.io/pie/psdService</code>. Esempio: <code>/photoshopActions</code></p>
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
      <td role="rowheader">[!UICONTROL Stringa Di Query]  </td>
      <td>
        <p>Immettere la stringa di query richiesta.</p>
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
