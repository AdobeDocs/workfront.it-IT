---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli di Microsoft Dynamics 365
description: In un [!DNL Adobe Workfront Fusion] In questo caso, è possibile automatizzare i flussi di lavoro che utilizzano Microsoft Dynamics 365 e collegarli a più applicazioni e servizi di terze parti.
author: Becky
feature: Workfront Fusion
exl-id: 116df088-20a7-40a8-8880-9f422dc37632
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1541'
ht-degree: 0%

---

# [!DNL Microsoft Dynamics 365 modules]

In un [!DNL Adobe Workfront Fusion] puoi automatizzare i flussi di lavoro che utilizzano [!DNL Microsoft Dynamics 365], nonché collegarlo a più applicazioni e servizi di terze parti.

>[!NOTE]
>
>La [!DNL Microsoft Dynamics 365] connettore non supportato [!DNL Dynamics Finance and Operations].

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

Per utilizzare [!DNL Microsoft Dynamics] 365, devi avere un [!DNL Microsoft Dynamics 365] conto.

## Collegare Microsoft Dynamics 365 a Workfront Fusion

Puoi creare una connessione al tuo [!DNL Microsoft Dynamics 365] account direttamente dall&#39;interno di un [!DNL Microsoft Dynamics 365] modulo .

1. In qualsiasi [!DNL Microsoft Dynamics 365] modulo, fai clic su **[!UICONTROL Aggiungi]** accanto al [!UICONTROL Connessione] campo .
1. Immettere un nome per la connessione.
1. In **[!UICONTROL Risorsa]** campo , inserisci l&#39;indirizzo del [!DNL Dynamics 365] conto, senza `https://`.
1. Fai clic su **[!UICONTROL Continua]** per creare la connessione e tornare al modulo .

>[!NOTE]
>
>Durante la registrazione [!DNL Workfront Fusion] nel tuo [!DNL Microsoft Azure] portale, utilizza il seguente URI di reindirizzamento:
>
>* `https://app.workfrontfusion.com/oauth/cb/workfront-microsoft-dynamics2`



## [!DNL Microsoft Dynamics 365] moduli e relativi campi

Quando si configura [!DNL Microsoft Dynamics 365] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL Microsoft Dynamics 365] potrebbero essere visualizzati, a seconda di fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se trovi il pulsante mappa sopra un campo o una funzione, puoi utilizzarlo per impostare variabili e funzioni per quel campo. Per ulteriori informazioni, consulta [Mappare informazioni da un modulo a un altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [[!UICONTROL Guarda i record (pianificati)]](#watch-records-scheduled)
* [[!UICONTROL Guarda i record (in tempo reale)]](#watch-records-real-time)
* [[!UICONTROL Crea record]](#create-record)
* [[!UICONTROL Effettuare una chiamata API]](#make-an-api-call)
* [[!UICONTROL Elimina record]](#delete-record)
* [[!UICONTROL Leggi record]](#read-records)
* [[!UICONTROL Aggiorna record]](#update-record)
* [[!UICONTROL Cerca record]](#search-records)

### [!UICONTROL Guarda i record (pianificati)]

Questo modulo trigger pianificato esegue uno scenario in cui viene creato o aggiornato un record nell’oggetto specificato dopo l’ultima esecuzione pianificata in [!DNL Dynamics 365].

L&#39;output del modulo indica se il record trovato è nuovo o aggiornato (se è stato aggiunto e aggiornato nel periodo di tempo, viene contrassegnato come nuovo). Puoi mappare queste informazioni nei moduli successivi nello scenario .

Questo accade in un intervallo regolarmente programmato specificato.

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Per istruzioni su come collegare le [!DNL Microsoft Dynamics 365] account a [!DNL Workfront Fusion], vedi <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Microsoft Dynamics 365] a [!DNL Workfront Fusion]</a> in questo articolo. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Include]</td> 
   <td>Seleziona se desideri che il modulo guardi <strong>[!UICONTROL Solo nuovi record]</strong>, <strong>[!UICONTROL Solo record aggiornati]</strong>oppure <strong>[!UICONTROL Nuovi record e tutte le modifiche]</strong>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entity Type]</td> 
   <td>Scegli il tipo di record [!UICONTROL Microsoft Dynamics 365] che desideri che lo scenario visualizzi.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Uscite]</td> 
   <td> <p>Selezionare le informazioni che si desidera includere nel pacchetto di output per questo modulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Max Records]</td> 
   <td> <p>Immettere o mappare il numero massimo di record che si desidera restituire dal modulo durante ogni ciclo di esecuzione degli scenari.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Guarda i record (in tempo reale)]

Questo modulo di attivazione immediata esegue uno scenario in cui viene creato o aggiornato un record (oggetto) specificato [!DNL Dynamics 365].

In questo modulo è richiesto un webhook.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>Selezionare il webhook che si desidera utilizzare per questo modulo. </p> <p>Per aggiungere un nuovo webhook:</p> 
    <ol> 
     <li value="1"> <p>Fai clic su <strong>[!UICONTROL Aggiungi]</strong> a destra del campo Webhook</p> </li> 
     <li value="2"> <p>In <strong>[!UICONTROL Webhook]</strong> campo name, digitare un nome descrittivo per il webhook.</p> </li> 
     <li value="3"> <p>In <strong>[!UICONTROL Connection]</strong> selezionare la connessione che si desidera utilizzare selezionata</p> <p>Per istruzioni su come collegare le [!DNL Microsoft Dynamics 365] account a [!DNL Workfront Fusion], vedi <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Microsoft Dynamics 365] a [!DNL Workfront Fusion]</a> in questo articolo. </p> </li> 
     <li value="4"> <p>Fai clic su <strong>[!UICONTROL Save]</strong> per salvare il webhook e tornare al modulo.</p> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Crea record]

Questo modulo di azione crea un&#39;entità, ad esempio un appuntamento o un&#39;attività.

Puoi specificare le informazioni sull’entità da creare.

Il modulo restituisce l’ID della nuova entità e di tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Microsoft Dynamics 365] account a [!DNL Workfront Fusion], vedi <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Microsoft Dynamics 365] a [!DNL Workfront Fusion]</a> in questo articolo. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entity Type]</td> 
   <td>Seleziona il tipo di entità che desideri creare nel modulo.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Property fields]</td> 
   <td>In questi campi, immettere il valore che si desidera che l'elemento di lavoro abbia per una determinata proprietà. I campi disponibili dipendono dal tipo di entità.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Effettuare una chiamata API]

Questo modulo di azione ti consente di effettuare una chiamata autenticata personalizzata al [!DNL Microsoft Dynamics 365] API. In questo modo, puoi creare un’automazione del flusso di dati che non può essere eseguita dall’altro [!DNL Microsoft Dynamics 365] moduli.

Il modulo restituisce informazioni sul codice di stato, sulle intestazioni e sul corpo. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Per ulteriori informazioni, consulta la sezione [!DNL Microsoft] documentazione sull&#39;utilizzo [!DNL Dynamics 365 Customer Engagement Web API].

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Per istruzioni su come collegare le [!DNL Microsoft Dynamics 365] account a [!DNL Workfront Fusion], vedi <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Microsoft Dynamics 365] a [!DNL Workfront Fusion]</a> in questo articolo. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> <p>Immettere un percorso relativo a <code>&lt;Instance URL>/api/data/v9.1/</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL, Metodo]</td> 
   <td> <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> <p>Per ulteriori informazioni in</p> </td> 
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

### [!UICONTROL Elimina record]

Questo modulo di azione elimina un’entità.

Specifica l’ID dell’entità.

Il modulo restituisce l’ID dell’entità e di tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Per istruzioni su come collegare le [!DNL Microsoft Dynamics 365] account a [!DNL Workfront Fusion], vedi <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Microsoft Dynamics 365] a [!DNL Workfront Fusion]</a> in questo articolo. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entity Type]</td> 
   <td> <p>Seleziona il tipo di entità da eliminare dal modulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td> <p>Immetti o mappa l'univoco [!DNL Microsoft Dynamics 365] ID del record che si desidera eliminare dal modulo.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Leggi record]

Questo modulo di azione legge i dati di una singola entità in [!DNL Microsoft Dynamics 365].

Specifica l’ID dell’entità.

Il modulo restituisce l’ID dell’entità e di tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Per istruzioni su come collegare le [!DNL Microsoft Dynamics 365] account a [!DNL Workfront Fusion], vedi <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Microsoft Dynamics 365] a [!DNL Workfront Fusion]</a> in questo articolo. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entity Type]</td> 
   <td>Selezionare il tipo di entità che si desidera leggere nel modulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Uscite]</td> 
   <td> <p>Selezionare le informazioni che si desidera includere nel pacchetto di output per questo modulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Immetti o mappa l'univoco [!DNL Microsoft Dynamics 365] ID del record che si desidera leggere nel modulo.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Aggiorna record]

Questo modulo di azione aggiorna un’entità.

Specifica l’ID dell’entità.

Il modulo restituisce l’ID del record aggiornato e di tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Per istruzioni su come collegare le [!DNL Microsoft Dynamics 365] account a [!DNL Workfront Fusion], vedi <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Microsoft Dynamics 365] a [!DNL Workfront Fusion]</a> in questo articolo. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Entity Type]</td> 
   <td>Seleziona il tipo di entità da aggiornare nel modulo.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Property fields]</td> 
   <td>In questi campi, immettere il valore che si desidera che l'elemento di lavoro abbia per una determinata proprietà. I campi disponibili dipendono dal tipo di entità.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Immetti o mappa l'univoco [!DNL Microsoft Dynamics] ID 365 del record che si desidera aggiornare nel modulo.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Cerca record]

Questo modulo di ricerca cerca i record in un oggetto in [!DNL Microsoft Dynamics 365] che corrispondono alla query di ricerca specificata. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Per istruzioni su come collegare le [!DNL Microsoft Dynamics 365] account a [!DNL Workfront Fusion], vedi <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Microsoft Dynamics 365] a [!DNL Workfront Fusion]</a> in questo articolo. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entity Type]</td> 
   <td>Seleziona il tipo di entità da aggiornare nel modulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filters]</td> 
   <td> <p>Selezionare il filtro da utilizzare per la ricerca.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Standard Filters]</strong> </p> <p>Imposta il filtro selezionando un campo e un operatore e immettendo o mappando il valore da cercare. Puoi utilizzare le regole AND o OR per il filtro.</p> </li> 
     <li> <p><strong>[!UICONTROL Query Functions]</strong> </p> <p>Inserisci il [!DNL Dynamics 365] funzione di query API web che si desidera utilizzare per la ricerca. </p> <p>Per ulteriori informazioni sulle funzioni di query, consulta <a href="https://docs.microsoft.com/en-us/dynamics365/customer-engagement/web-api/queryfunctions?view=dynamics-ce-odata-9">Riferimento per la funzione di query API web</a> in [!DNL Microsoft] documentazione.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sort]</td> 
   <td> <p>Specifica l'ordine in cui gli elementi vengono restituiti. Puoi aggiungere più ordinamenti.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Field]</strong> </p> <p>Specifica il campo in base al quale vuoi ordinare i risultati.</p> </li> 
     <li> <p><strong>[!UICONTROL Direction]</strong> </p> <p>Specifica la direzione dell’ordinamento (crescente o decrescente).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Max Records]</td> 
   <td> <p>Immettere o mappare il numero massimo di record che si desidera restituire dal modulo durante ogni ciclo di esecuzione degli scenari.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Uscite]</td> 
   <td> <p>Selezionare le informazioni che si desidera includere nel pacchetto di output per questo modulo.</p> </td> 
  </tr> 
 </tbody> 
</table>
