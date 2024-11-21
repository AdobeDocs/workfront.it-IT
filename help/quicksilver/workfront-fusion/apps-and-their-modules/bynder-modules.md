---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli Bynder
description: In uno scenario  [!DNL Adobe Workfront Fusion] , puoi automatizzare i flussi di lavoro che utilizzano  [!DNL Bynder], nonché collegarli a più applicazioni e servizi di terze parti.
author: Becky
feature: Workfront Fusion
exl-id: e4dc9588-334a-41a3-85d1-996cb819c3fa
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '1676'
ht-degree: 0%

---

# [!DNL Bynder] moduli

In uno scenario [!DNL Adobe Workfront Fusion], è possibile automatizzare i flussi di lavoro che utilizzano [!DNL Bynder] e collegarlo a più applicazioni e servizi di terze parti.

Se hai bisogno di istruzioni per la creazione di uno scenario, consulta [Creare uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Per informazioni sui moduli, vedere [Moduli in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <p>Requisito licenza legacy: [!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>
   <p>Fabbisogno prodotto corrente: se disponi del piano [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront], la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo. [!DNL Workfront Fusion] è incluso nel piano [!UICONTROL Ultimate] [!DNL Workfront].</p>
   <p>Oppure</p>
   <p>Requisiti del prodotto legacy: la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Per conoscere il piano, il tipo di licenza o l&#39;accesso disponibili, contattare l&#39;amministratore [!DNL Workfront].

Per informazioni sulle [!DNL Adobe Workfront Fusion] licenze, vedere [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Prerequisiti

Per utilizzare i moduli [!DNL Bynder], è necessario disporre di un account [!DNL Bynder].

## Informazioni API di Bynder

Il connettore Bynder utilizza quanto segue:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Versione API</td> 
   <td> v4 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Tag API</td> 
   <td>v1.25.21</td> 
  </tr>
 </tbody> 
 </table>

## Connetti [!DNL Bynder] a Workfront Fusion  {#connect-bynder-to-workfront-fusion}

* [Crea una connessione a  [!DNL Bynder] da [!DNL Workfront Fusion]](#create-a-connection-to-bynder-from-workfront-fusion)
* [Genera un [!UICONTROL ID client] e un [!UICONTROL Segreto client] in [!DNL Bynder] (facoltativo)](#generate-a-client-id-and-client-secret-in-bynder-optional)

### Crea una connessione a [!DNL Bynder] da [!DNL Workfront Fusion]

È possibile creare una connessione da [!DNL Workfront Fusion] all&#39;account [!DNL Bynder] direttamente dall&#39;interno di un modulo [!DNL Bynder].

1. In qualsiasi modulo [!DNL Bynder], fai clic su **[!UICONTROL Aggiungi]** accanto al campo [!UICONTROL Connessione].
1. Selezionare il dominio [!DNL Bynder] a cui connettersi.
1. (Facoltativo) Fai clic su **[!UICONTROL Impostazioni avanzate]**, quindi immetti il tuo [!UICONTROL ID client] e [!UICONTROL Segreto client].

   Per istruzioni sulla generazione dell&#39;ID client e del segreto client, vedere [Generare un ID client e un segreto client in [!DNL Bynder] (facoltativo)](#generate-a-client-id-and-client-secret-in-bynder-optional) in questo articolo.

1. Nella finestra [!UICONTROL accesso], immetti il tuo nome utente (indirizzo e-mail) e la tua password.
1. Fai clic su **[!UICONTROL Continua]** per creare la connessione e tornare al modulo.

### Genera un [!UICONTROL ID client] e un [!UICONTROL Segreto client] in [!DNL Bynder] (facoltativo)

Se desideri creare una connessione utilizzando l&#39;ID client e il segreto client, puoi generarli dal tuo account [!DNL Bynder]. L&#39;ID client e il segreto client vengono generati quando si crea un&#39;app in [!DNL Bynder].

Per istruzioni sulla creazione di un&#39;app in [!DNL Bynder], vedere [App Oauth 2.0](https://developer-docs.bynder.com/api/authentication-oauth2-oauth-apps/) nella documentazione di [!DNL Bynder].

>[!NOTE]
>
>Durante la creazione dell&#39;app in [!DNL Bynder], immetti `redirect uri` come segue:
>
>`https://app.workfrontfusion.com/oauth/cb/workfront-bynder`

## [!DNL Bynder] moduli e relativi campi

Quando configuri [!DNL Bynder] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Insieme a questi, potrebbero essere visualizzati ulteriori campi di [!DNL Bynder], a seconda di fattori quali il livello di accesso nell&#39;app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se viene visualizzato il pulsante Mappa sopra un campo o una funzione, è possibile utilizzarlo per impostare variabili e funzioni per tale campo. Per ulteriori informazioni, vedere [Mappare le informazioni da un modulo all&#39;altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Azioni](#actions)
* [Ricerche](#searches)
* [Triggers](#triggers)

### Azioni

* [[!UICONTROL Chiamata API personalizzata]](#custom-api-call)
* [[!UICONTROL Leggi metadati risorsa]](#read-asset-metadata)
* [[!UICONTROL Aggiorna metadati risorsa]](#update-asset-metadata)
* [[!UICONTROL Aggiungere risorse a una raccolta]](#add-assets-to-a-collection)
* [[!UICONTROL Rimuovi risorse dalla raccolta]](#remove-assets-from-collection)
* [[!UICONTROL Aggiungi un tag alle risorse]](#add-a-tag-to-assets)
* [[!UICONTROL Rimuovi un tag] dalle risorse](#remove-a-tag-from-assets)
* [[!UICONTROL Scarica risorsa]](#download-asset)
* [[!UICONTROL Carica risorsa]](#upload-asset)

#### [!UICONTROL Chiamata API personalizzata]

Questo modulo di azione consente di effettuare una chiamata autenticata personalizzata all&#39;API [!DNL Bynder]. In questo modo è possibile creare un&#39;automazione del flusso di dati che non può essere eseguita dagli altri moduli [!DNL Bynder].

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

Il modulo restituisce un codice di stato, insieme alle intestazioni e al corpo della chiamata API.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Bynder] a [!DNL Workfront Fusion], vedere <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connessione di [!DNL Bynder] a [!DNL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td>Immettere un percorso relativo a <code>https://{your-bynder-domain}/api/{api-version}/</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   td&gt; <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, vedere <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
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
   <td> <p>Aggiungi il contenuto body per la chiamata API sotto forma di oggetto JSON standard.</p> <p>Nota:  <p>Quando si utilizzano istruzioni condizionali come <code>if</code> nel JSON, inserire le virgolette al di fuori dell'istruzione condizionale.</p> 
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
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Bynder] a [!DNL Workfront Fusion], vedere <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connessione di [!DNL Bynder] a [!DNL Workfront Fusion] </a> in questo articolo.</p> </td> 
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

#### [!UICONTROL Aggiorna metadati risorsa]

Questo modulo di azione aggiorna i metadati di una risorsa esistente.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Bynder] a [!DNL Workfront Fusion], vedere <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connessione di [!DNL Bynder] a [!DNL Workfront Fusion] </a> in questo articolo.</p> </td> 
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
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Bynder] a [!DNL Workfront Fusion], vedere <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connessione di [!DNL Bynder] a [!DNL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID raccolta]</td> 
   <td> <p>Inserisci o mappa l’ID della raccolta in cui desideri aggiungere le risorse.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID risorsa]</td> 
   <td> <p>Per ogni risorsa da aggiungere alla raccolta, fai clic su <strong>[!UICONTROL Add item]</strong>, quindi immetti o mappa l'ID della risorsa.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Rimuovi risorse dalla raccolta]

Questo modulo di azione rimuove una o più risorse da una raccolta.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Bynder] a [!DNL Workfront Fusion], vedere <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connessione di [!DNL Bynder] a [!DNL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID raccolta]</td> 
   <td> <p>Inserisci o mappa l’ID della raccolta in cui desideri rimuovere le risorse.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID risorsa]</td> 
   <td> <p>Per ogni risorsa da rimuovere dalla raccolta, fai clic su <strong>[!UICONTROL Add item]</strong>, quindi immetti o mappa l'ID della risorsa.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggiungi un tag alle risorse]

Aggiungere un tag a una o più risorse

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Bynder] a [!DNL Workfront Fusion], vedere <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connessione di [!DNL Bynder] a [!DNL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID tag]</td> 
   <td> <p>Inserisci o mappa l’ID del tag da aggiungere alle risorse.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID risorsa]</td> 
   <td> <p>Per ogni risorsa a cui si desidera assegnare il tag, fare clic su <strong>[!UICONTROL Add item]</strong>, quindi immettere o mappare l'ID della risorsa.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Rimuovi un tag dalle risorse]

Rimuovere un tag da una o più risorse

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Bynder] a [!DNL Workfront Fusion], vedere <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connessione di [!DNL Bynder] a [!DNL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID tag]</td> 
   <td> <p>Immetti o mappa l’ID del tag da rimuovere dalle risorse.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID risorsa]</td> 
   <td> <p>Per ogni risorsa da cui vuoi rimuovere un tag, fai clic su <strong>[!UICONTROL Aggiungi elemento]</strong>, quindi immetti o mappa l'ID della risorsa.</p> </td> 
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
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Bynder] a [!DNL Workfront Fusion], vedere <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connessione di [!DNL Bynder] a [!DNL Workfront Fusion] </a> in questo articolo.</p> </td> 
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
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Bynder] a [!DNL Workfront Fusion], vedere <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connessione di [!DNL Bynder] a [!DNL Workfront Fusion] </a> in questo articolo.</p> </td> 
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
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td>Selezionare un file di origine da un modulo precedente o mappare il nome e i dati del file di origine.</td> 
  </tr> 
 </tbody> 
</table>

### Ricerche

* [[!UICONTROL Elenca record]](#list-record)
* [[!UICONTROL Cerca risorse]](#search-for-assets)

#### [!UICONTROL Elenca record]

Questo modulo di ricerca recupera tutti gli elementi di un tipo specifico.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Bynder] a [!DNL Workfront Fusion], vedere <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connessione di [!DNL Bynder] a [!DNL Workfront Fusion] </a> in questo articolo.</p> </td> 
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

#### [!UICONTROL Cerca risorse]

Questo modulo di ricerca cerca le risorse in base ai criteri specificati.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Bynder] a [!DNL Workfront Fusion], vedere <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connessione di [!DNL Bynder] a [!DNL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Criteria]</td> 
   <td> <p>Inserire i criteri di ricerca. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Campo]</strong> </p> <p>Selezionare il campo da utilizzare nella ricerca</p> </li> 
     <li> <p><strong>[!UICONTROL Operatore Logico]</strong> </p> <p>Seleziona l’operatore da utilizzare nella ricerca.</p> </li> 
     <li> <p><strong>[!UICONTROL Valore]</strong> </p> <p>Immetti o mappa il valore da cercare nel campo selezionato. Il tipo di valore deve essere uguale al tipo di dati del campo selezionato. </p> <p>Per ulteriori informazioni sui tipi di dati, vedere <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">Tipi di dati elemento in [!DNL Adobe Workfront Fusion]</a>.</p> </li> 
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

#### [!UICONTROL Risorse da controllare]

Questo modulo di attivazione avvia uno scenario quando una risorsa viene creata o aggiornata.

<table style="table-layout:auto">
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Bynder] a [!DNL Workfront Fusion], vedere <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connessione di [!DNL Bynder] a [!DNL Workfront Fusion] </a> in questo articolo.</p> </td> 
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
