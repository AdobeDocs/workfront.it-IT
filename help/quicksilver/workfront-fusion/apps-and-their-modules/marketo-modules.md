---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli Marketo
description: In un [!DNL Adobe Workfront Fusion] puoi automatizzare i flussi di lavoro che utilizzano [!DNL Marketo], nonché collegarlo a più applicazioni e servizi di terze parti.
author: Becky
feature: Workfront Fusion
exl-id: 7f6dace5-ab50-45da-a926-1a8919057f7b
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2014'
ht-degree: 0%

---

# [!DNL Marketo] moduli

In un [!DNL Adobe Workfront Fusion] puoi automatizzare i flussi di lavoro che utilizzano [!DNL Marketo], nonché collegarlo a più applicazioni e servizi di terze parti.

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

Per utilizzare [!DNL Marketo] moduli, è necessario disporre di un [!DNL Marketo] conto.

## Connetti [!DNL Marketo] a Workfront Fusion {#connect-marketo-to-workfront-fusion}

Puoi creare una connessione al tuo [!DNL Marketo] account direttamente dall&#39;interno [!DNL Marketo] modulo .

1. In qualsiasi [!DNL Marketo] modulo, fai clic su **[!UICONTROL Aggiungi]** accanto al [!UICONTROL Connessione] campo .
1. Inserisci il tuo [!DNL Marketo] conto o [!DNL Marketo] [!UICONTROL Munchkin] ID. Questa è la parte univoca dell&#39;URL di base o dell&#39;endpoint assegnato al tuo account, a cui puoi accedere [!DNL Marketo] tramite [!UICONTROL REST] API. Per istruzioni su come individuare questo, consulta [URL di base](https://developers.marketo.com/rest-api/base-url/) in [!DNL Marketo] documentazione.
1. Inserisci il tuo [!UICONTROL ID client] e [!UICONTROL Segreto client]. Per istruzioni su come individuarle, vedi [Autenticazione](https://developers.marketo.com/rest-api/authentication/) in [!DNL Marketo] documentazione.
1. Fai clic su **[!UICONTROL Continua]** per creare la connessione e tornare al modulo .

## [!DNL Marketo] Moduli e relativi campi

Quando si configura [!DNL Marketo] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL Marketo] potrebbero essere visualizzati, a seconda di fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se trovi il pulsante mappa sopra un campo o una funzione, puoi utilizzarlo per impostare variabili e funzioni per quel campo. Per ulteriori informazioni, consulta [Mappare informazioni da un modulo a un altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Azioni](#actions)
* [Ricerche](#searches)

### Triggers

* [[!UICONTROL Registri di controllo]](#watch-records)
* [[!UICONTROL Eventi di controllo (Instant)]](#watch-events-instant)

#### [!UICONTROL Registri di controllo]

Questo modulo di attivazione avvia uno scenario quando un record viene creato o aggiornato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Marketo] account a [!DNL Workfront Fusion], vedi <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Marketo] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td> <p>Selezionare il tipo di record che si desidera creare.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Activity]</strong> </p> <p>Seleziona il tipo di attività da visualizzare. </p> <p>Il modulo controlla solo le nuove attività.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Lead]</strong> </p> <p>Seleziona se desideri controllare i nuovi record, i record aggiornati, sia nuovi che aggiornati o gli aggiornamenti specifici dei campi. Se si sceglie di controllare gli aggiornamenti specifici dei campi, selezionare il campo che si desidera che il modulo controlli.</p> </li> 
     <li> <p><strong>[!UICONTROL Program]</strong> </p> <p>Seleziona se desideri controllare i nuovi record, i record aggiornati o i record nuovi e aggiornati.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Uscite]</td> 
   <td> <p>Selezionare le informazioni che si desidera includere nel pacchetto di output per questo modulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Immettere o mappare il numero massimo di record che si desidera restituire dal modulo durante ogni ciclo di esecuzione degli scenari.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eventi di controllo (Instant)]

Questo modulo di attivazione avvia uno scenario quando un record viene creato o aggiornato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Webhook]</p> </td> 
   <td> <p>Immettere il webhook che si desidera utilizzare nel modulo.</p> <p>Per ulteriori informazioni sui webhook, vedi <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">Trigger istantanei (webhook) in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Immettere o mappare il numero massimo di record che si desidera restituire dal modulo durante ogni ciclo di esecuzione degli scenari.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Azioni

* [[!UICONTROL Chiamata API personalizzata]](#custom-api-call)
* [[!UICONTROL Creare un record]](#create-a-record)
* [[!UICONTROL Aggiornare un record]](#update-a-record)
* [[!UICONTROL Scaricare un file]](#download-a-file)
* [[!UICONTROL Caricare un file]](#upload-a-file)
* [[!UICONTROL Leggi un record]](#read-a-record)
* [[!UICONTROL Aggiungere lead a un elenco]](#add-leads-to-a-list)
* [[!UICONTROL Rimuovere i lead da un elenco]](#remove-leads-from-a-list)
* [[!UICONTROL Pianificare una campagna]](#schedule-a-campaign)
* [[!UICONTROL Copiare un programma]](#copy-a-program)

#### [!UICONTROL Chiamata API personalizzata]

Questo modulo di azione ti consente di effettuare una chiamata autenticata personalizzata al [!DNL Marketo] API. In questo modo, puoi creare un’automazione del flusso di dati che non può essere eseguita dall’altro [!DNL Marketo] moduli.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Marketo] account a [!DNL Workfront Fusion], vedi <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Marketo] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Immettere un percorso relativo a <code>https://{your-base-url}.mktorest.com/</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL, Metodo]</td> 
   <td> <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Aggiungi le intestazioni della richiesta sotto forma di un oggetto JSON standard.</p> <p>Ad esempio: <code>{"Content-type":"application/json"}</code></p> <p>[!UICONTROL Workfront Fusion] aggiunge le intestazioni di autorizzazione.</p> </td> 
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
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Immettere o mappare il numero massimo di record con cui si desidera che il modulo funzioni durante ogni ciclo di esecuzione degli scenari.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Creare un record]

Questo modulo di azione crea un nuovo record in [!DNL Marketo]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Marketo] account a [!DNL Workfront Fusion], vedi <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Marketo] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td> <p>Selezionare il tipo di record che si desidera creare.</p> 
    <ul> 
     <li> <p>[!UICONTROL Company]</p> </li> 
     <li> <p>[!UICONTROL Cartella]</p> </li> 
     <li> <p>[!UICONTROL Lead]</p> </li> 
     <li> <p>[!UICONTROL Program]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seleziona campi da mappare]</td> 
   <td>Se si sta creando una società o un lead, selezionare i campi per i quali si desidera impostare i valori al momento della creazione del nuovo record, quindi immettere i valori per questi campi.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Program Type]</td> 
   <td>Se si sta creando un programma, selezionare il tipo di programma che si desidera creare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Program Channel] </td> 
   <td>Se si sta creando un programma, selezionare il canale del programma in cui si desidera creare il programma.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder] / [!UICONTROL Program Name]</td> 
   <td>Se si sta creando una cartella o un programma, immettere o mappare un nome per il nuovo record.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Descrizione]</td> 
   <td> <p>Se si sta creando una cartella o un programma, immettere o mappare una descrizione per il nuovo record.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID cartella padre]</td> 
   <td>Se si sta creando una cartella o un programma, immettere o mappare l'ID della cartella padre in cui si desidera creare il nuovo record.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cost]</td> 
   <td>Se stai creando un programma, aggiungi eventuali costi.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tags]</td> 
   <td>Se stai creando un programma, aggiungi eventuali tag</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggiornare un record]

Questo modulo di azione aggiorna un record esistente utilizzando il relativo ID.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Marketo] account a [!DNL Workfront Fusion], vedi <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Marketo] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td> <p>Selezionare il tipo di record che si desidera creare.</p> 
    <ul> 
     <li> <p>[!UICONTROL Company]</p> </li> 
     <li> <p>[!UICONTROL Lead]</p> </li> 
     <li> <p>[!UICONTROL Program]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Company] / [!UICONTROL Lead] / [!UICONTROL Program ID]</td> 
   <td>Immettere o mappare l'ID del record che si desidera aggiornare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seleziona campi da mappare]</td> 
   <td>Se si aggiorna una società o un lead, selezionare i campi per i quali si desidera aggiornare i valori, quindi immettere i valori per questi campi.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Program Name]</td> 
   <td>Se si aggiorna un programma, immettere o mappare un nuovo nome per il programma.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Descrizione]</td> 
   <td> <p>Se si aggiorna un programma, immettere o mappare una nuova descrizione del programma.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data di inizio]</td> 
   <td>Se si aggiorna un programma, immettere o mappare una nuova data di inizio per il programma.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data di fine]</td> 
   <td>Se si aggiorna un programma, immettere o mappare una nuova data di fine per il programma.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cost]</td> 
   <td>Se stai aggiornando un programma, aggiungi eventuali costi.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tags]</td> 
   <td>Se stai aggiornando un programma, aggiungi eventuali tag</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Scaricare un file]

Questo modulo di azione scarica un file utilizzando l’ID file.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Marketo] account a [!DNL Workfront Fusion], vedi <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Marketo] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File ID]</td> 
   <td>Mappa l'ID del file da scaricare.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Caricare un file]

Questo modulo di azione carica un nuovo file in [!UICONTROL Marketo].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Marketo] account a [!DNL Workfront Fusion], vedi <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Marketo] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File di origine]</td> 
   <td>Selezionare un file di origine da un modulo precedente o mappare il nome e i dati del file di origine.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID cartella [!UICONTROL]</td> 
   <td>Immettere o mappare l'ID della cartella in cui si desidera individuare il nuovo file.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Descrizione]</td> 
   <td>Immetti una descrizione per il file caricato.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Leggi un record]

Questo modulo di azione legge le informazioni su un record utilizzando il relativo ID.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Marketo] account a [!DNL Workfront Fusion], vedi <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Marketo] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td> <p>Selezionare il tipo di record che si desidera creare.</p> 
    <ul> 
     <li> <p>[!UICONTROL Campaign]</p> </li> 
     <li> <p>[!UICONTROL Company]</p> </li> 
     <li> <p>[!UICONTROL Lead]</p> </li> 
     <li> <p>[!UICONTROL List]</p> </li> 
     <li> <p>[!UICONTROL Program]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Uscite]</td> 
   <td>Selezionare le informazioni che si desidera includere nel pacchetto di output per questo modulo. I campi sono disponibili in base al [!UICONTROL Record Type] selezionato.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL &lt;object&gt; ID]</td> 
   <td>Immettere o mappare l'ID dell'oggetto di cui si desidera recuperare le informazioni.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggiungere lead a un elenco]

Questo modulo di azione aggiunge uno o più lead a un elenco, utilizzando l’ID lead.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Marketo] account a [!DNL Workfront Fusion], vedi <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Marketo] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List ID]</td> 
   <td>Immetti o mappa l’ID dell’elenco in cui desideri aggiungere i lead.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Lead ID]</td> 
   <td> <p>Per ogni lead da aggiungere all’elenco, fai clic su <b>[!UICONTROL Aggiungi]</b>, quindi immetti o mappa l’ID del lead che desideri aggiungere. Puoi aggiungere fino a 300 lead all’elenco per il modulo .</p> <p>Fai clic sull’opzione mappa per mappare una raccolta di lead esistente da aggiungere all’elenco.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Rimuovere i lead da un elenco]

Questo modulo di azione rimuove uno o più lead da un elenco, utilizzando l’ID lead.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Marketo] account a [!DNL Workfront Fusion], vedi <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Marketo] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List ID]</td> 
   <td>Immetti o mappa l’ID dell’elenco in cui desideri rimuovere i lead.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Lead ID]</td> 
   <td> <p>Per ogni lead che si desidera rimuovere dall’elenco, fare clic su <b>[!UICONTROL Aggiungi]</b>, quindi immetti o mappa l’ID del lead da rimuovere. Puoi aggiungere fino a 300 lead per il modulo da rimuovere dall’elenco. </p> <p>Fai clic sull’opzione mappa per mappare una raccolta di lead esistente da rimuovere dall’elenco.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Pianificare una campagna]

Questo modulo di azione pianifica una campagna esistente per una data specifica.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Marketo] account a [!DNL Workfront Fusion], vedi <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Marketo] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campaign ID]</td> 
   <td>Immetti o mappa l’ID della campagna da pianificare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Pianificazione della data]</p> </td> 
   <td>Seleziona la data in cui desideri eseguire la campagna. Se questo campo viene lasciato vuoto, la campagna viene eseguita cinque minuti dopo l’inizio dello scenario.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Copiare un programma]

Questo modulo di azione crea una copia di un programma utilizzando l’ID del programma esistente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Marketo] account a [!DNL Workfront Fusion], vedi <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Marketo] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID programma esistente]</td> 
   <td>Immettere o mappare l'ID del programma da copiare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Nuovo Nome Programma]</p> </td> 
   <td> <p>Immettere o mappare un nome per il nuovo programma</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID cartella [!UICONTROL]</td> 
   <td>Immettere o mappare l'ID della cartella in cui si desidera individuare il nuovo programma.</td> 
  </tr> 
 </tbody> 
</table>

### Ricerche

* [[!UICONTROL Elencare record]](#list-records)
* [[!UICONTROL Cerca record]](#update-a-record)

#### [!UICONTROL Elencare record]

Questo modulo di azione recupera tutti i record di un tipo specifico.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Marketo] account a [!DNL Workfront Fusion], vedi <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Marketo] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td> <p>Selezionare il tipo di record da elencare.</p> 
    <ul> 
     <li> <p>[!UICONTROL Leggi tutte le campagne]</p> </li> 
     <li> <p>[!UICONTROL Leggi tutti i programmi]</p> </li> 
     <li> <p>[!UICONTROL Leggi tutti i lead] </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Field]</td> 
   <td>Se hai selezionato per recuperare i lead, seleziona se desideri recuperare i lead da un elenco o da un programma.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Uscite]</td> 
   <td>Selezionare le informazioni che si desidera includere nel pacchetto di output per questo modulo. I campi sono disponibili in base al [!UICONTROL Record Type] selezionato.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Immettere o mappare il numero massimo di record che si desidera restituire dal modulo durante ogni ciclo di esecuzione degli scenari.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Cerca record]

Questo modulo di ricerca recupera un elenco di record che corrispondono a criteri di ricerca specifici.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Marketo] account a [!DNL Workfront Fusion], vedi <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Marketo] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td> <p>Selezionare il tipo di record da cercare.</p> 
    <ul> 
     <li> <p>Campagne</p> </li> 
     <li> <p>[!UICONTROL Lead]</p> </li> 
     <li> <p>[!UICONTROL Programmi]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Field]</p> </td> 
   <td> <p>Selezionare se si desidera eseguire la ricerca per nome, nome del programma o nome dell'area di lavoro.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Values]</td> 
   <td>Per ogni valore che si desidera cercare, fare clic su <b>[!UICONTROL Aggiungi elemento]</b> e immetti il valore .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output]</td> 
   <td> <p>Selezionare le informazioni che si desidera includere nel pacchetto di output per questo modulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Immettere o mappare il numero massimo di record che si desidera restituire dal modulo durante ogni ciclo di esecuzione degli scenari.</p> </td> 
  </tr> 
 </tbody> 
</table>
