---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli Bynder
description: In un [!DNL Adobe Workfront Fusion] scenario, puoi automatizzare i flussi di lavoro che utilizzano [!DNL Bynder], oltre a collegarlo a più applicazioni e servizi di terze parti.
author: Becky
feature: Workfront Fusion
exl-id: e4dc9588-334a-41a3-85d1-996cb819c3fa
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1664'
ht-degree: 0%

---

# [!DNL Bynder] moduli

In un [!DNL Adobe Workfront Fusion] scenario, puoi automatizzare i flussi di lavoro che utilizzano [!DNL Bynder], oltre a collegarlo a più applicazioni e servizi di terze parti.

Per istruzioni sulla creazione di uno scenario, consulta [Creare uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Per informazioni sui moduli, consulta [Moduli in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

## Prerequisiti

Da utilizzare [!DNL Bynder] moduli, è necessario disporre di un [!DNL Bynder] account.

## Connetti [!DNL Bynder] a Workfront Fusion  {#connect-bynder-to-workfront-fusion}

* [Creare una connessione a [!DNL Bynder] da [!DNL Workfront Fusion]](#create-a-connection-to-bynder-from-workfront-fusion)
* [Genera un [!UICONTROL ID client] e [!UICONTROL Segreto client] in [!DNL Bynder] (Facoltativo)](#generate-a-client-id-and-client-secret-in-bynder-optional)

### Creare una connessione a [!DNL Bynder] da [!DNL Workfront Fusion]

Puoi creare una connessione da [!DNL Workfront Fusion] al tuo [!DNL Bynder] account direttamente dall&#39;interno di un [!DNL Bynder] modulo.

1. In qualsiasi [!DNL Bynder] modulo, fai clic su **[!UICONTROL Aggiungi]** accanto al [!UICONTROL Connessione] campo.
1. Seleziona la [!DNL Bynder] dominio a cui desideri connetterti.
1. (Facoltativo) Fai clic su **[!UICONTROL Impostazioni avanzate]**, quindi immetti il [!UICONTROL ID client] e [!UICONTROL Segreto client].

   Per istruzioni sulla generazione dell&#39;ID client e del segreto client, consulta [Generare un ID client e un segreto client in [!DNL Bynder] (Facoltativo)](#generate-a-client-id-and-client-secret-in-bynder-optional) in questo articolo.

1. In [!UICONTROL accesso] immettere il nome utente (indirizzo e-mail) e la password.
1. Clic **[!UICONTROL Continua]** per creare la connessione e tornare al modulo.

### Genera un [!UICONTROL ID client] e [!UICONTROL Segreto client] in [!DNL Bynder] (Facoltativo)

Se desideri creare una connessione utilizzando l’ID client e il segreto client, puoi generarli dal tuo [!DNL Bynder] account. L&#39;ID client e il Segreto client vengono generati quando crei un&#39;app in [!DNL Bynder].

Per istruzioni su come creare un’app in [!DNL Bynder], vedi [App Oauth 2.0](https://developer-docs.bynder.com/api/authentication-oauth2-oauth-apps/) nel [!DNL Bynder] documentazione.

>[!NOTE]
>
>Durante la creazione dell’app in [!DNL Bynder], immetti quanto segue come `redirect uri`:
>
>`https://app.workfrontfusion.com/oauth/cb/workfront-bynder`

## [!DNL Bynder] moduli e relativi campi

Quando si configura [!DNL Bynder] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL Bynder] I campi potrebbero essere visualizzati in base a fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se viene visualizzato il pulsante Mappa sopra un campo o una funzione, è possibile utilizzarlo per impostare variabili e funzioni per tale campo. Per ulteriori informazioni, consulta [Mappare le informazioni da un modulo all’altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Azioni](#actions)
* [Ricerche](#searches)
* [Triggers](#triggers)

### Azioni

* [[!UICONTROL Chiamata API personalizzata]](#custom-api-call)
* [[!UICONTROL Leggi metadati risorsa]](#read-asset-metadata)
* [[!UICONTROL Aggiornare i metadati delle risorse]](#update-asset-metadata)
* [[!UICONTROL Aggiungere risorse a una raccolta]](#add-assets-to-a-collection)
* [[!UICONTROL Rimuovere risorse dalla raccolta]](#remove-assets-from-collection)
* [[!UICONTROL Aggiungere un tag alle risorse]](#add-a-tag-to-assets)
* [[!UICONTROL Rimuovere un tag] da risorse](#remove-a-tag-from-assets)
* [[!UICONTROL Scarica risorsa]](#download-asset)
* [[!UICONTROL Carica risorsa]](#upload-asset)

#### [!UICONTROL Chiamata API personalizzata]

Questo modulo di azione consente di effettuare una chiamata autenticata personalizzata al [!DNL Bynder] API. In questo modo, puoi creare un’automazione del flusso di dati che non può essere eseguita dall’altro [!DNL Bynder] moduli.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

Il modulo restituisce un codice di stato, insieme alle intestazioni e al corpo della chiamata API.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Bynder] account a [!DNL Workfront Fusion], vedi <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Bynder] a [!DNL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td>Inserisci un percorso relativo a <code>https://{your-bynder-domain}/api/{api-version}/</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   td&gt; <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Aggiungi le intestazioni della richiesta sotto forma di oggetto JSON standard.</p> <p>Ad esempio: <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion aggiunge automaticamente le intestazioni di autorizzazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Stringa Di Query]</td> 
   <td> <p>Aggiungi la query per la chiamata API sotto forma di oggetto JSON standard.</p> <p>Ad esempio: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Aggiungi il contenuto body per la chiamata API sotto forma di oggetto JSON standard.</p> <p>Nota:  <p>Quando si utilizzano istruzioni condizionali quali <code>if</code> nel JSON, inserisci le virgolette al di fuori dell’istruzione condizionale.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Leggi metadati risorsa]

Questo modulo di azione legge i metadati di una risorsa.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Bynder] account a [!DNL Workfront Fusion], vedi <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Bynder] a [!DNL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID risorsa]</td> 
   <td>Immetti o mappa l’ID della risorsa per la quale desideri recuperare i metadati.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output]</td> 
   <td> <p>Seleziona le informazioni da includere nel bundle di output per questo modulo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggiornare i metadati delle risorse]

Questo modulo di azione aggiorna i metadati di una risorsa esistente.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Bynder] account a [!DNL Workfront Fusion], vedi <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Bynder] a [!DNL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID risorsa]</td> 
   <td>Immetti o mappa l’ID della risorsa per la quale desideri aggiornare i metadati.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fields]</td> 
   <td> <p>Selezionare i campi per i quali si desidera immettere le informazioni, quindi immettere o mappare in tali campi le informazioni con le quali si desidera aggiornare i metadati. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Metaproperties]</p> </td> 
   <td>Seleziona le opzioni da aggiornare, quindi immetti o mappa le informazioni in tali proprietà. Le metaproprietà sono informazioni sulla risorsa che non rappresentano campi specifici della risorsa.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggiungere risorse a una raccolta]

Questo modulo di azione aggiunge una o più risorse a una raccolta.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Bynder] account a [!DNL Workfront Fusion], vedi <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Bynder] a [!DNL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID raccolta]</td> 
   <td> <p>Inserisci o mappa l’ID della raccolta in cui desideri aggiungere le risorse.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID risorsa]</td> 
   <td> <p>Per ogni risorsa da aggiungere alla raccolta, fai clic su <strong>[!UICONTROL Add item]</strong>, quindi immetti o mappa l’ID della risorsa.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Rimuovere risorse dalla raccolta]

Questo modulo di azione rimuove una o più risorse da una raccolta.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Bynder] account a [!DNL Workfront Fusion], vedi <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Bynder] a [!DNL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID raccolta]</td> 
   <td> <p>Inserisci o mappa l’ID della raccolta in cui desideri rimuovere le risorse.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID risorsa]</td> 
   <td> <p>Per ogni risorsa da rimuovere dalla raccolta, fai clic su <strong>[!UICONTROL Add item]</strong>, quindi immetti o mappa l’ID della risorsa.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggiungere un tag alle risorse]

Aggiungere un tag a una o più risorse

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Bynder] account a [!DNL Workfront Fusion], vedi <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Bynder] a [!DNL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID tag]</td> 
   <td> <p>Inserisci o mappa l’ID del tag da aggiungere alle risorse.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID risorsa]</td> 
   <td> <p>Per ogni risorsa a cui vuoi assegnare i tag, fai clic su <strong>[!UICONTROL Add item]</strong>, quindi immetti o mappa l’ID della risorsa.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Rimuovere un tag dalle risorse]

Rimuovere un tag da una o più risorse

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Bynder] account a [!DNL Workfront Fusion], vedi <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Bynder] a [!DNL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID tag]</td> 
   <td> <p>Immetti o mappa l’ID del tag da rimuovere dalle risorse.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID risorsa]</td> 
   <td> <p>Per ogni risorsa da cui vuoi rimuovere un tag, fai clic su <strong>[!UICONTROL Add item]</strong>, quindi immetti o mappa l’ID della risorsa.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Scarica risorsa]

Questo modulo di azione scarica una singola risorsa.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Bynder] account a [!DNL Workfront Fusion], vedi <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Bynder] a [!DNL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID risorsa]</td> 
   <td>Inserisci o mappa l’ID della risorsa da scaricare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL versione risorsa]</td> 
   <td> <p>Immetti o mappa la versione della risorsa da scaricare. Per scaricare la versione più recente della risorsa, lascia vuoto il campo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Carica risorsa]

Questo modulo di azione carica una singola risorsa.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Bynder] account a [!DNL Workfront Fusion], vedi <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Bynder] a [!DNL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Salva con nome]</td> 
   <td> <p>Seleziona la modalità di salvataggio del file che stai caricando.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nuova risorsa]</strong> </p> <p>Selezionare i campi e le metaproprietà per i quali si desidera immettere le informazioni, quindi immettere le informazioni in tali campi.</p> <p>Inserisci o mappa l’ID del marchio che desideri utilizzare per la risorsa caricata.</p> </li> 
     <li> <p><strong>[!UICONTROL Nuova versione risorsa]</strong> </p> <p>Immetti l’ID della risorsa per la quale stai caricando una nuova versione.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File di origine]</td> 
   <td>Selezionare un file di origine da un modulo precedente o mappare il nome e i dati del file di origine.</td> 
  </tr> 
 </tbody> 
</table>

### Ricerche

* [[!UICONTROL Record elenco]](#list-record)
* [[!UICONTROL Cercare le risorse]](#search-for-assets)

#### [!UICONTROL Record elenco]

Questo modulo di ricerca recupera tutti gli elementi di un tipo specifico.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Bynder] account a [!DNL Workfront Fusion], vedi <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Bynder] a [!DNL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td> <p>Selezionare il tipo di record da elencare.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Leggi tutte le raccolte]</strong> </p> </li> 
     <li> <p><strong>[!UICONTROL Leggi informazioni su tutti i tag]</strong> </p> </li> 
     <li> <p><strong>[!UICONTROL Leggi tutte le risorse di una raccolta]</strong> </p> <p>Inserisci o mappa l’ID della raccolta di cui desideri elencare le risorse.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output]</td> 
   <td> <p>Selezionare i campi da includere nell'output del modulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Immettere o mappare il numero massimo di risorse che il modulo deve restituire durante ciascun ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Cercare le risorse]

Questo modulo di ricerca cerca le risorse in base ai criteri specificati.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Bynder] account a [!DNL Workfront Fusion], vedi <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Bynder] a [!DNL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Criteria]</td> 
   <td> <p>Inserire i criteri di ricerca. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Field]</strong> </p> <p>Selezionare il campo da utilizzare nella ricerca</p> </li> 
     <li> <p><strong>[!UICONTROL Operatore Logico]</strong> </p> <p>Seleziona l’operatore da utilizzare nella ricerca.</p> </li> 
     <li> <p><strong>Valore [!UICONTROL]</strong> </p> <p>Immetti o mappa il valore da cercare nel campo selezionato. Il tipo di valore deve essere uguale al tipo di dati del campo selezionato. </p> <p>Per ulteriori informazioni sui tipi di dati, consulta <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">Tipi di dati degli elementi in [!DNL Adobe Workfront Fusion]</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Set di risultati]</td> 
   <td>Seleziona se desideri restituire la prima risorsa corrispondente o tutte le risorse corrispondenti.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordina per]</td> 
   <td> <p>Selezionare il campo in base al quale si desidera eseguire l'ordinamento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL - Direzione di ordinamento]</td> 
   <td> <p>Seleziona se desideri ordinare in modo crescente o decrescente.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output]</td> 
   <td> <p>Selezionare i campi da includere nell'output del modulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Immettere o mappare il numero massimo di risorse che il modulo deve restituire durante ciascun ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Triggers

#### [!UICONTROL Visualizzare le risorse]

Questo modulo di attivazione avvia uno scenario quando una risorsa viene creata o aggiornata.

<table style="table-layout:auto">
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Bynder] account a [!DNL Workfront Fusion], vedi <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Bynder] a [!DNL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> <!--
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Event type</td>
   --> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Select whether you want to start the scenario when a new asset is created or when an existing asset is updated.</td>
   --> 
  </tr> 
  <tr>
     <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">[!UICONTROL Raccolte]</td>
   <td> <p>Seleziona la raccolta da controllare per le nuove risorse. Per controllare tutte le raccolte, lascia vuoto questo campo.</p> </td> 
  </tr> 
  <tr> <!--
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Outputs</td>
   --> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Select the fields that you want to include in the output.</td>
   --> 
  </tr> 
  <tr> 
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">[!UICONTROL Limit]</td>

<td> <p>Immettere il numero massimo di record che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>
