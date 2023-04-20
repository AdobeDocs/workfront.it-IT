---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli Allocadia
description: In un [!DNL Adobe Workfront Fusion] In questo caso, puoi automatizzare i flussi di lavoro che utilizzano Allocadia e collegarli a più applicazioni e servizi di terze parti.
author: Becky
feature: Workfront Fusion
exl-id: f1edefd1-9fe0-48fc-bea2-c3f9facf7363
source-git-commit: c88b00a086a9e1c5e44d481dde94f4244c7c959d
workflow-type: tm+mt
source-wordcount: '1353'
ht-degree: 0%

---

# [!DNL Allocadia] moduli

In un [!DNL Adobe Workfront Fusion] puoi automatizzare i flussi di lavoro che utilizzano [!DNL Allocadia], nonché collegarlo a più applicazioni e servizi di terze parti.

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

Per utilizzare [!DNL Allocadia] moduli, è necessario disporre di un [!DNL Allocadia] conto.

## Connetti [!DNL Allocadia] a [!DNL Workfront Fusion]

Puoi creare una connessione al tuo [!DNL Allocadia] account direttamente dall&#39;interno di un [!DNL Allocadia] modulo .

1. In qualsiasi [!DNL Allocadia] modulo, fai clic su **[!UICONTROL Aggiungi]** accanto al [!UICONTROL Connessione] campo .
1. Selezionare se si desidera utilizzare il server Nord America o il server Europa.
1. Immetti il tuo nome utente e la tua password.
1. Fai clic su **[!UICONTROL Continua]** per creare la connessione e tornare al modulo .

## [!DNL Allocadia] moduli e relativi campi

Quando si configura [!DNL Allocadia] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL Allocadia] potrebbero essere visualizzati, a seconda di fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se trovi il pulsante mappa sopra un campo o una funzione, puoi utilizzarlo per impostare variabili e funzioni per quel campo. Per ulteriori informazioni, consulta [Mappare informazioni da un modulo a un altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Azioni](#actions)
* [Ricerche](#searches)

### Triggers

#### [!UICONTROL Registra]

Questo modulo trigger esegue uno scenario in cui vengono aggiunti, aggiornati o entrambi oggetti di un tipo specifico. Il modulo restituisce tutti i campi standard associati al record o ai record, insieme a tutti i campi e i valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> <table style="table-layout:auto"> <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowhader"&gt; <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare il tuo account Allocadia a [!DNL Workfront Fusion], vedi <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connetti Allocadia a Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Filtro</td> 
   <td> <p>Selezionare se si desidera che lo scenario visualizzi solo nuovi record, solo record aggiornati o record nuovi e aggiornati.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Tipo di entità</td> 
   <td>Selezionare il tipo di record Allocadia che si desidera che il modulo guardi.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Uscite</td> 
   <td> <p>Seleziona i campi da includere nell’output del modulo. I campi disponibili dipendono dal tipo di entità selezionato.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limite</td> 
   <td> <p>Immettere o mappare il numero massimo di record che si desidera che il modulo visualizzi durante ogni ciclo di esecuzione degli scenari.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Azioni

* [Chiamata API personalizzata](#custom-api-call)
* [Leggi record](#read-record)
* [Crea record](#create-record)
* [Elimina record](#delete-record)
* [Aggiorna record](#update-record)

#### [!UICONTROL Chiamata API personalizzata]

Questo modulo di azione ti consente di effettuare una chiamata autenticata personalizzata al [!DNL Allocadia] API. In questo modo, puoi creare un’automazione del flusso di dati che non può essere eseguita dall’altro [!DNL Allocadia] moduli.

L&#39;azione si basa sul tipo di entità (tipo di oggetto Allocadia) specificato.

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Allocadia] account a [!DNL Workfront Fusion], vedi <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Allocadia] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Immettere un percorso relativo a <code>https://api-na.allocadia.com/{version}</code> o <code>https://api-eu.allocadia.com/{version}</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL, Metodo]</td> 
   <td> <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Aggiungi le intestazioni della richiesta sotto forma di un oggetto JSON standard.</p> <p>Ad esempio: <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] aggiunge le intestazioni di autorizzazione per te.</p> </td> 
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

#### [!UICONTROL Leggi record]

Questo modulo di azione legge i dati da un singolo record in [!DNL Allocadia].

Specifica l&#39;ID del record.

Il modulo restituisce tutti i campi standard associati al record, insieme a eventuali campi e valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowhader"&gt; <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Allocadia] account a [!DNL Workfront Fusion], vedi <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Allocadia] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entity Type]</td> 
   <td>Seleziona il tipo di [!DNL Allocadia] registrare che si desidera che il modulo legga.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Uscite]</td> 
   <td> <p>Seleziona i campi da includere nell’output del modulo. I campi disponibili dipendono dal [!UICONTROL Entity Type] selezionato.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Immetti o mappa l'univoco [!DNL Allocadia] ID del record che si desidera leggere nel modulo.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crea record]

Questo modulo di azione crea un record.

Il modulo restituisce l’ID del record e di tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowhader"&gt; <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Allocadia] account a [!DNL Workfront Fusion], vedi <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Allocadia] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entity Type]</td> 
   <td>Selezionare se si desidera creare un nuovo record in base all'elemento riga o alla scelta della colonna.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Budget]</td> 
   <td> <p>Selezionare il budget in cui si desidera creare un record.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Column choices]</td> 
   <td>Selezionare la colonna che si desidera utilizzare per creare un nuovo record.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Label]</td> 
   <td>Immettere o mappare un'etichetta per il nuovo record</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Elimina record]

Questo modulo di azione elimina un record specifico.

Specifica l&#39;ID del record.

Il modulo restituisce l’ID del record e di tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowhader"&gt; <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Allocadia] account a [!DNL Workfront Fusion], vedi <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Allocadia] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entity Type]</td> 
   <td> <p>Seleziona il tipo di entità da eliminare.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Riga elemento]</strong> </p> <p>Immettere l'ID dell'elemento riga</p> </li> 
     <li> <p><strong>[!UICONTROL Column Choice]</strong> </p> <p>Selezionare il budget da cui si desidera eliminare un record, quindi immettere l'ID colonna e l'ID scelta.</p> </li> 
     <li> <p><strong>[!UICONTROL Tags]</strong> </p> <p>Selezionare il budget da cui si desidera eliminare un record, quindi immettere l'ID tag.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggiorna record]

Questo modulo di azione aggiorna un record, ad esempio una scelta di riga, utente o colonna.

Specifica l&#39;ID del record.

Il modulo restituisce l’ID del record e di tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare il tuo account [!UICONTROL Allocadia] a [!DNL Workfront Fusion], vedi <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Allocadia] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entity Type]</td> 
   <td>Seleziona il tipo di [!DNL Allocadia] registrare che si desidera aggiornare il modulo. Altri campi vengono visualizzati in base al tipo di entità selezionato.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Budget]</td> 
   <td> <p>Selezionare il budget in cui si desidera aggiornare un record. </p> </td> 
  </tr> 
 </tbody> 
</table>

### Ricerche

#### [!UICONTROL Cerca record]

Questo modulo di ricerca cerca i record in un oggetto in [!DNL Allocadia] che corrispondono alla query di ricerca specificata.

Puoi mappare queste informazioni nei moduli successivi nello scenario .

Specificare il tipo di record desiderato.

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowhader"&gt; <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Allocadia] account a [!DNL Workfront Fusion], vedi <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Allocadia] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entity Type]</td> 
   <td>Seleziona il tipo di [!DNL Allocadia] registrare che si desidera cercare nel modulo. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Budget]</td> 
   <td> <p>Selezionare il budget da cercare. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Set di risultati]</td> 
   <td>Selezionare se si desidera che il modulo restituisca tutti i record corrispondenti o solo il record corrispondente.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conteggio massimo dei record]</td> 
   <td> <p>Immettere o mappare il numero massimo di record che si desidera restituire dal modulo durante ogni ciclo di esecuzione degli scenari.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Criteri di ricerca]</td> 
   <td>Selezionare il campo da cercare, selezionare l'operazione e immettere o mappare il valore da cercare. Puoi aggiungere [!DNL AND] o [!DNL OR] regole per filtrare ulteriormente la ricerca.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Uscite]</td> 
   <td> <p>Seleziona i campi da includere nell’output del modulo. I campi disponibili dipendono dal tipo di entità selezionato.</p> </td> 
  </tr> 
 </tbody> 
</table>
