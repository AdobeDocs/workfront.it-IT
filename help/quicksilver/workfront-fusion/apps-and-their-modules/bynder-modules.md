---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli Bynder
description: In un [!DNL Adobe Workfront Fusion] puoi automatizzare i flussi di lavoro che utilizzano [!DNL Bynder], nonché collegarlo a più applicazioni e servizi di terze parti.
author: Becky
feature: Workfront Fusion
exl-id: e4dc9588-334a-41a3-85d1-996cb819c3fa
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1616'
ht-degree: 0%

---

# [!DNL Bynder] moduli

In un [!DNL Adobe Workfront Fusion] puoi automatizzare i flussi di lavoro che utilizzano [!DNL Bynder], nonché collegarlo a più applicazioni e servizi di terze parti.

Se hai bisogno di istruzioni su come creare uno scenario, vedi [Crea uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Per informazioni sui moduli, consulta [Moduli in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Requisiti di accesso

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td>
  <td> <p>[!UICONTROL Pro] o superiore</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licenza**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</td> 
  </tr> 
 </tbody> 
</table>

Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, vedi [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Prerequisiti

Per utilizzare [!DNL Bynder] moduli, è necessario disporre di un [!DNL Bynder] conto.

## Connetti [!DNL Bynder] a Workfront Fusion  {#connect-bynder-to-workfront-fusion}

* [Creare una connessione a [!DNL Bynder] da [!DNL Workfront Fusion]](#create-a-connection-to-bynder-from-workfront-fusion)
* [Genera un [!UICONTROL ID client] e [!UICONTROL Segreto client] in [!DNL Bynder] (Facoltativo)](#generate-a-client-id-and-client-secret-in-bynder-optional)

### Creare una connessione a [!DNL Bynder] da [!DNL Workfront Fusion]

Puoi creare una connessione da [!DNL Workfront Fusion] al tuo [!DNL Bynder] account direttamente dall&#39;interno di un [!DNL Bynder] modulo .

1. In qualsiasi [!DNL Bynder] modulo, fai clic su **[!UICONTROL Aggiungi]** accanto al [!UICONTROL Connessione] campo .
1. Seleziona la [!DNL Bynder] dominio a cui si desidera connettersi.
1. (Facoltativo) Fai clic su **[!UICONTROL Impostazioni avanzate]**, quindi inserisci il [!UICONTROL ID client] e [!UICONTROL Segreto client].

   Per istruzioni su come generare l’ID client e il segreto client, consulta [Generare un ID client e un segreto client in [!DNL Bynder] (Facoltativo)](#generate-a-client-id-and-client-secret-in-bynder-optional) in questo articolo.

1. In [!UICONTROL login] finestra, inserisci il tuo nome utente (indirizzo e-mail) e la password.
1. Fai clic su **[!UICONTROL Continua]** per creare la connessione e tornare al modulo .

### Genera un [!UICONTROL ID client] e [!UICONTROL Segreto client] in [!DNL Bynder] (Facoltativo)

Se desideri creare una connessione utilizzando l’ID client e il segreto client, puoi generarle dal tuo [!DNL Bynder] conto. L’ID client e il segreto client vengono generati quando crei un’app in [!DNL Bynder].

Per istruzioni su come creare un’app in [!DNL Bynder], vedi [App Oauth 2.0](https://developer-docs.bynder.com/api/authentication-oauth2-oauth-apps/) in [!DNL Bynder] documentazione.

>[!NOTE]
>
>Quando crei l’app in [!DNL Bynder], immetti quanto segue come `redirect uri`:
>
>`https://app.workfrontfusion.com/oauth/cb/workfront-bynder`

## [!DNL Bynder] moduli e relativi campi

Quando si configura [!DNL Bynder] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL Bynder] potrebbero essere visualizzati, a seconda di fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se trovi il pulsante mappa sopra un campo o una funzione, puoi utilizzarlo per impostare variabili e funzioni per quel campo. Per ulteriori informazioni, consulta [Mappare informazioni da un modulo a un altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Azioni](#actions)
* [Ricerche](#searches)
* [Triggers](#triggers)

### Azioni

* [[!UICONTROL Chiamata API personalizzata]](#custom-api-call)
* [[!UICONTROL Leggere i metadati delle risorse]](#read-asset-metadata)
* [[!UICONTROL Aggiornare i metadati delle risorse]](#update-asset-metadata)
* [[!UICONTROL Aggiungere risorse a una raccolta]](#add-assets-to-a-collection)
* [[!UICONTROL Rimuovere risorse dalla raccolta]](#remove-assets-from-collection)
* [[!UICONTROL Aggiungere un tag alle risorse]](#add-a-tag-to-assets)
* [[!UICONTROL Rimuovere un tag] da risorse](#remove-a-tag-from-assets)
* [[!UICONTROL Scarica risorsa]](#download-asset)
* [[!UICONTROL Caricare risorse]](#upload-asset)

#### [!UICONTROL Chiamata API personalizzata]

Questo modulo di azione ti consente di effettuare una chiamata autenticata personalizzata al [!DNL Bynder] API. In questo modo, puoi creare un’automazione del flusso di dati che non può essere eseguita dall’altro [!DNL Bynder] moduli.

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

Il modulo restituisce un codice di stato, insieme alle intestazioni e al corpo della chiamata API.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Bynder] account a [!DNL Workfront Fusion], vedi <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Bynder] a [!DNL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td>Immettere un percorso relativo a <code>https://{your-bynder-domain}/api/{api-version}/</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL, Metodo]</td> 
   td&gt; <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Aggiungi le intestazioni della richiesta sotto forma di un oggetto JSON standard.</p> <p>Ad esempio: <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion aggiunge le intestazioni di autorizzazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>Aggiungi la query per la chiamata API sotto forma di un oggetto JSON standard.</p> <p>Ad esempio: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Aggiungi il contenuto del corpo per la chiamata API sotto forma di un oggetto JSON standard.</p> <p>Nota:  <p>Quando si utilizzano istruzioni condizionali come <code>if</code> nel JSON, inserisci le virgolette al di fuori dell’istruzione condizionale.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Leggere i metadati delle risorse]

Questo modulo di azione legge i metadati di una risorsa.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Bynder] account a [!DNL Workfront Fusion], vedi <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Bynder] a [!DNL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID]</td> 
   <td>Immetti o mappa l’ID della risorsa per la quale desideri recuperare i metadati.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Uscite]</td> 
   <td> <p>Selezionare le informazioni che si desidera includere nel pacchetto di output per questo modulo.</p> </td> 
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
   <td> <p>Per istruzioni su come collegare le [!DNL Bynder] account a [!DNL Workfront Fusion], vedi <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Bynder] a [!DNL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID]</td> 
   <td>Immetti o mappa l’ID della risorsa per la quale vuoi aggiornare i metadati.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fields]</td> 
   <td> <p>Selezionare i campi per i quali si desidera immettere le informazioni, quindi immettere o mappare le informazioni con cui si desidera aggiornare i metadati in tali campi. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Metaproprietà [!UICONTROL]</p> </td> 
   <td>Seleziona le opzioni che desideri aggiornare, quindi immetti o mappa le informazioni in tali proprietà. Le proprietà sono informazioni sulla risorsa che non rappresentano campi specifici della risorsa.</td> 
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
   <td> <p>Per istruzioni su come collegare le [!DNL Bynder] account a [!DNL Workfront Fusion], vedi <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Bynder] a [!DNL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID raccolta [!UICONTROL]</td> 
   <td> <p>Immetti o mappa l’ID della raccolta in cui desideri aggiungere le risorse.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset IDs]</td> 
   <td> <p>Per ogni risorsa da aggiungere alla raccolta, fai clic su <strong>[!UICONTROL Aggiungi elemento]</strong>, quindi immetti o mappa l’ID risorsa.</p> </td> 
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
   <td> <p>Per istruzioni su come collegare le [!DNL Bynder] account a [!DNL Workfront Fusion], vedi <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Bynder] a [!DNL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID raccolta [!UICONTROL]</td> 
   <td> <p>Immetti o mappa l’ID della raccolta in cui desideri rimuovere le risorse.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset IDs]</td> 
   <td> <p>Per ogni risorsa da rimuovere dalla raccolta, fai clic su <strong>[!UICONTROL Aggiungi elemento]</strong>, quindi immetti o mappa l’ID risorsa.</p> </td> 
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
   <td> <p>Per istruzioni su come collegare le [!DNL Bynder] account a [!DNL Workfront Fusion], vedi <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Bynder] a [!DNL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tag ID]</td> 
   <td> <p>Immetti o mappa l’ID del tag da aggiungere alle risorse.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset IDs]</td> 
   <td> <p>Per ogni risorsa a cui desideri assegnare un tag, fai clic su <strong>[!UICONTROL Aggiungi elemento]</strong>, quindi immetti o mappa l’ID risorsa.</p> </td> 
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
   <td> <p>Per istruzioni su come collegare le [!DNL Bynder] account a [!DNL Workfront Fusion], vedi <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Bynder] a [!DNL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tag ID]</td> 
   <td> <p>Immetti o mappa l’ID del tag da rimuovere dalle risorse.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset IDs]</td> 
   <td> <p>Per ogni risorsa da cui vuoi rimuovere un tag, fai clic su <strong>[!UICONTROL Aggiungi elemento]</strong>, quindi immetti o mappa l’ID risorsa.</p> </td> 
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
   <td> <p>Per istruzioni su come collegare le [!DNL Bynder] account a [!DNL Workfront Fusion], vedi <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Bynder] a [!DNL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID]</td> 
   <td>Immetti o mappa l’ID della risorsa da scaricare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Versione risorsa]</td> 
   <td> <p>Immetti o mappa la versione della risorsa da scaricare. Per scaricare la versione più recente della risorsa, lascia vuoto il campo .</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Caricare risorse]

Questo modulo di azione carica una singola risorsa.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Bynder] account a [!DNL Workfront Fusion], vedi <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Bynder] a [!DNL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Salva con nome]</td> 
   <td> <p>Seleziona la modalità di salvataggio del file che stai caricando.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nuova risorsa]</strong> </p> <p>Selezionare i campi e le proprietà delle metriche per i quali si desidera immettere le informazioni, quindi immettere le informazioni in tali campi.</p> <p>Immetti o mappa l’ID del marchio da utilizzare per la risorsa caricata.</p> </li> 
     <li> <p><strong>[!UICONTROL Nuova versione della risorsa]</strong> </p> <p>Immetti l’ID della risorsa per la quale stai caricando una nuova versione.</p> </li> 
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
* [[!UICONTROL Cercare risorse]](#search-for-assets)

#### [!UICONTROL Record elenco]

Questo modulo di ricerca recupera tutti gli elementi di un tipo specifico.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Bynder] account a [!DNL Workfront Fusion], vedi <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Bynder] a [!DNL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td> <p>Selezionare il tipo di record da elencare.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Leggi tutte le raccolte]</strong> </p> </li> 
     <li> <p><strong>[!UICONTROL Leggi informazioni su tutti i tag]</strong> </p> </li> 
     <li> <p><strong>[!UICONTROL Leggi tutte le risorse di una raccolta]</strong> </p> <p>Immetti o mappa l’ID della raccolta di cui desideri elencare le risorse.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Uscite]</td> 
   <td> <p>Seleziona i campi da includere nell’output del modulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Immetti o mappa il numero massimo di risorse che desideri che il modulo restituisca durante ogni ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Cercare risorse]

Questo modulo di ricerca cerca le risorse in base ai criteri forniti.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Bynder] account a [!DNL Workfront Fusion], vedi <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Bynder] a [!DNL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Criteri di [!UICONTROL]</td> 
   <td> <p>Immetti i criteri di ricerca. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Field]</strong> </p> <p>Selezionare il campo da utilizzare nella ricerca</p> </li> 
     <li> <p><strong>[!UICONTROL Operatore logico]</strong> </p> <p>Seleziona l’operatore da utilizzare nella ricerca.</p> </li> 
     <li> <p><strong>[!UICONTROL Value]</strong> </p> <p>Immetti o mappa il valore da cercare nel campo selezionato. Il tipo di valore deve corrispondere al tipo di dati del campo selezionato. </p> <p>Per ulteriori informazioni sui tipi di dati, consulta <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">Tipi di dati degli elementi in [!DNL Adobe Workfront Fusion]</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Set di risultati]</td> 
   <td>Seleziona se restituire la prima risorsa corrispondente o tutte le risorse corrispondenti.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordina per]</td> 
   <td> <p>Selezionare il campo in base al quale si desidera eseguire l’ordinamento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordina Direzione]</td> 
   <td> <p>Seleziona se desideri ordinare in ordine crescente o decrescente.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Uscite]</td> 
   <td> <p>Seleziona i campi da includere nell’output del modulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Immetti o mappa il numero massimo di risorse che desideri che il modulo restituisca durante ogni ciclo di esecuzione dello scenario.</p> </td> 
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
   <td> <p>Per istruzioni su come collegare le [!DNL Bynder] account a [!DNL Workfront Fusion], vedi <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Bynder] a [!DNL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> <!--
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Event type</td>
   --> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Select whether you want to start the scenario when a new asset is created or when an existing asset is updated.</td>
   --> 
  </tr> 
  <tr>
     <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">[!UICONTROL Raccolte]</td>
   <td> <p>Seleziona la raccolta da controllare per le nuove risorse. Per guardare tutte le raccolte, lasciare vuoto questo campo.</p> </td> 
  </tr> 
  <tr> <!--
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Outputs</td>
   --> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Select the fields that you want to include in the output.</td>
   --> 
  </tr> 
  <tr> 
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">[!UICONTROL Limit]</td>

<td> <p>Immettere il numero massimo di record che si desidera restituire dal modulo durante ogni ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>
