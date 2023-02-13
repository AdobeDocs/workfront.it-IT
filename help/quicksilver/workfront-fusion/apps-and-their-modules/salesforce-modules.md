---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli Salesforce
description: In uno scenario Adobe Workfront Fusion, è possibile automatizzare i flussi di lavoro che utilizzano Salesforce, nonché collegarli a più applicazioni e servizi di terze parti.
author: Becky
feature: Workfront Fusion
exl-id: 3c8adcd9-fb5f-400d-9edd-6d9fc30cc728
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2720'
ht-degree: 0%

---

# [!DNL Salesforce] moduli

In uno scenario Adobe Workfront Fusion, è possibile automatizzare i flussi di lavoro che utilizzano [!DNL Salesforce], nonché collegarlo a più applicazioni e servizi di terze parti.

Se hai bisogno di istruzioni su come creare uno scenario, vedi [Crea uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Per informazioni sui moduli, consulta [Moduli in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

>[!NOTE]
>
>* Non tutte le edizioni di [!DNL Salesforce] avere accesso API. Per informazioni dettagliate, consulta [!DNL Salesforce] edizioni con accesso API nel [!DNL Salesforce] Sito della community.
>* Per informazioni su errori specifici restituiti dal [!DNL Salesforce] API, vedi [!DNL Salesforce] Documenti API. Puoi anche controllare lo stato del [!DNL Salesforce] API per eventuali interruzioni del servizio.
>


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

Per utilizzare [!DNL Salesforce] moduli, è necessario disporre di un [!DNL Salesforce] conto.

## Informazioni sulla ricerca [!DNL Salesforce] oggetti

Durante la ricerca di oggetti, è possibile immettere singole parole di ricerca o creare una query più complessa utilizzando caratteri jolly e operatori:

* Utilizzare l&#39;asterisco carattere jolly (\*) come sostituto di zero o più caratteri. Ad esempio, una ricerca per Ca\* trova gli elementi che iniziano con Ca
* Usa un punto interrogativo con carattere jolly (?) come sostituto di un singolo carattere. Ad esempio, una ricerca per Jo?n trova elementi con il termine John o Joan ma non Jon
* Utilizza l’operatore virgolette (&quot; &quot;) per trovare una corrispondenza esatta tra le frasi. Ad esempio: &quot;riunione di lunedì&quot;

Per ulteriori informazioni sulle possibilità di ricerca, consulta la sezione [!DNL Salesforce] documentazione per sviluppatori su SOQL e SOSL.

## [!DNL Salesforce] moduli e relativi campi

* [Triggers](#triggers)
* [Azioni](#actions)
* [Ricerche](#searches)

### Triggers

* [[!UICONTROL Cerca record]](#watch-for-records)
* [[!UICONTROL Visualizzare i messaggi in uscita]](#watch-outbound-messages)
* [[!UICONTROL Guarda un campo]](#watch-a-field)

#### [!UICONTROL Cerca record]

Questo modulo trigger esegue uno scenario quando viene creato o aggiornato un record in un oggetto. Il modulo restituisce tutti i campi standard associati al record o ai record, insieme a tutti i campi e i valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Salesforce] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Type] </td> 
   <td> <p>Seleziona il tipo di [!DNL Salesforce] registrare che si desidera che il modulo visualizzi.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Fields]</td> 
   <td>Selezionare i campi che si desidera controllare nel modulo. I campi disponibili dipendono dal tipo di record.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Conteggio massimo dei record]</td> 
   <td> <p>Immettere o mappare il numero massimo di record che si desidera restituire dal modulo durante ogni ciclo di esecuzione degli scenari.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td> <p>Determinare se si desidera che lo scenario visualizzi solo i nuovi record del tipo selezionato oppure i nuovi record del tipo selezionato e tutte le altre modifiche ai record di quel tipo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Visualizzare i messaggi in uscita]

Questo modulo di attivazione esegue uno scenario in cui un utente invia un messaggio. Il modulo restituisce tutti i campi standard associati al record o ai record, insieme a tutti i campi e i valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Questo modulo richiede una configurazione aggiuntiva:

1. Vai a [!DNL Salesforce] pagina di configurazione.

   Per accedere alla pagina di configurazione, individua e fai clic sul pulsante &quot;[!UICONTROL Configurazione]&quot; nell&#39;angolo superiore destro del [!DNL Salesforce] conto. Da [!DNL Salesforce] pagina di configurazione, individua il &quot;[!UICONTROL Ricerca rapida / Ricerca]&quot; barra sul lato sinistro. Cerca &quot;[!UICONTROL Regole del flusso di lavoro].&quot;

1. Fai clic su **[!UICONTROL Regole del flusso di lavoro]**.
1. Sulla [!UICONTROL Regole del flusso di lavoro] pagina visualizzata, fai clic su **[!UICONTROL Nuova regola]** e seleziona il tipo di oggetto a cui si applica la regola (ad esempio &quot;[!UICONTROL Opportunità]&quot; se stai monitorando gli aggiornamenti ai record Opportunità).
1. Fai clic su **[!UICONTROL Successivo]**.
1. Imposta un nome di regola, criteri di valutazione e criteri di regola, quindi fai clic su **[!UICONTROL Salva]** e **[!UICONTROL Successivo]**.

1. Fai clic su **[!UICONTROL Fine]**.
1. Dalla nuova regola del flusso di lavoro creata, fai clic su **[!UICONTROL Modifica]**.
1. Da **[!UICONTROL Aggiungi azione flusso di lavoro]** elenco a discesa, seleziona **[!UICONTROL Nuovo messaggio in uscita]**.

1. Specifica nome, descrizione, URL endpoint e campi da includere nel nuovo messaggio in uscita, quindi fai clic su **[!UICONTROL Salva]**.

   La **[!UICONTROL URL endpoint]** contiene l’URL fornito nella [!DNL Salesforce] [!UICONTROL Messaggio in uscita] in [!DNL Workfront Fusion].

1. Configurare uno scenario che inizia con [!UICONTROL Messaggio in uscita] evento.

1. Fai clic sul pulsante **&lt;/>** in basso a destra e copia l’URL fornito.
1. Torna a **[!UICONTROL Regole del flusso di lavoro]** , individua la regola appena creata, quindi fai clic su **[!UICONTROL Attiva]**.

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Webhook]</td> 
   <td> <p>Selezionare il webhook che si desidera utilizzare per guardare i messaggi in uscita. Per aggiungere un webhook, fai clic su <strong>[!UICONTROL Aggiungi]</strong> e inserire il nome e la connessione del webhook.</p> <p>Per istruzioni su come collegare le [!DNL Salesforce] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!UICONTROL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo di record] </td> 
   <td> <p>Seleziona il tipo di [!DNL Salesforce] registrare che si desidera che il modulo verifichi i messaggi in uscita.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fields]</td> 
   <td> <p>Seleziona i campi che desideri che il modulo verifichi per i messaggi in uscita. I campi disponibili dipendono dal tipo di record.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### *[!UICONTROL Guarda un campo]*

Questo modulo di attivazione avvia uno scenario in cui un campo viene aggiornato in [!DNL Salesforce].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Salesforce] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo di record] </td> 
   <td> <p>Selezionare il tipo di record che contiene il campo che si desidera controllare nel modulo. È necessario scegliere un tipo di record con [!UICONTROL Field History] attivato in [!DNL Salesforce] installazione. Per ulteriori informazioni, consulta <a href="https://help.salesforce.com/articleView?id=tracking_field_history.htm&amp;type=5">Tracciamento della cronologia dei campi</a> in [!DNL Salesforce] documentazione. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Field]</td> 
   <td> <p>Selezionare i campi che si desidera che il modulo verifichi le modifiche.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td> <p>Immettere o mappare il numero massimo di campi che si desidera che il modulo restituisca durante ogni ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Azioni

* [[!UICONTROL Creare un record]](#create-a-record)
* [[!UICONTROL Leggi un record]](#read-a-record)
* [[!UICONTROL Eliminare un record]](#delete-a-record)
* [[!UICONTROL Chiamata API personalizzata]](#custom-api-call)
* [[!UICONTROL Carica allegato/documento]](#upload-attachmentdocument)
* [[!UICONTROL Scarica allegato/documento]](#download-attachmentdocument)

#### [!UICONTROL Creare un record]

Questo modulo di azione crea un nuovo record in un oggetto.

Il modulo ti consente di selezionare i campi dell’oggetto disponibili nel modulo. Questo riduce il numero di campi da scorrere durante la configurazione del modulo.

Il modulo restituisce l’ID del record e di tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Salesforce] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Tipo di record] </p> </td> 
   <td> <p>Seleziona il tipo di [!DNL Salesforce] registrare che si desidera creare il modulo. I campi diventano disponibili in base al tipo di record selezionato nel campo [!UICONTROL Record Type]. Questi campi sono basati sulle [!DNL Salesforce] API.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Seleziona campi da mappare]</td> 
   <td> <p>Selezionare i campi che si desidera configurare dal modulo al momento della creazione del nuovo record. I campi obbligatori si trovano nella parte superiore dell’elenco. </p> <p>I campi selezionati vengono aperti sotto questo campo. È ora possibile immettere i valori in questi campi.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Leggi un record]

Questo modulo di azione legge i dati da un singolo oggetto in [!DNL Salesforce].

Specifica l&#39;ID del record.

Il modulo restituisce l’ID del record e di tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr>
    <td>[!UICONTROL Connection]</td>
   <td> <p>Per istruzioni su come collegare le [!DNL Salesforce] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Tipo di record]</td>
    <td>Seleziona il tipo di [!DNL Salesforce] registrare che si desidera che il modulo [action].read.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Record Fields]</td>
    <td>Selezionare i campi che si desidera leggere nel modulo. È necessario selezionare almeno un campo.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL ID]</td>
    <td> <p>Immetti o mappa l'univoco [!DNL Salesforce] ID del record che si desidera leggere nel modulo.</p> <p>Per ottenere l'ID, apri la [!DNL Salesforce] nel browser e copia il testo alla fine dell’URL dopo l’ultima barra (/). Ad esempio: <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminare un record]

Questo modulo di azione elimina un record esistente in un oggetto.

Specifica l&#39;ID del record.

Il modulo restituisce l’ID del record e di tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Salesforce] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo di record] </td> 
   <td> <p>Seleziona il tipo di [!DNL Salesforce] registrare che si desidera eliminare il modulo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>Immetti o mappa l'univoco [!DNL Salesforce] ID del record che si desidera eliminare dal modulo.</p> <p>Per ottenere l'ID, apri la [!DNL Salesforce] nel browser e copia il testo alla fine dell’URL dopo l’ultima barra (/). Ad esempio: <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Chiamata API personalizzata]

Questo modulo di azione ti consente di effettuare una chiamata autenticata personalizzata al [!DNL Salesforce] API. In questo modo, puoi creare un’automazione del flusso di dati che non può essere eseguita dall’altro [!DNL Salesforce] moduli.

Il modulo restituisce quanto segue:

* **[!UICONTROL Codice di stato]** (numero): Indica il successo o il fallimento della richiesta HTTP. Questi sono codici standard che puoi cercare su Internet.
* **[!UICONTROL Intestazioni]** (oggetto): Un contesto più dettagliato per il codice di risposta/stato che non si riferisce al corpo dell&#39;output. Non tutte le intestazioni che compaiono in un&#39;intestazione di risposta sono intestazioni di risposta, quindi alcune potrebbero non essere utili per te.

   Le intestazioni di risposta dipendono dalla richiesta HTTP scelta durante la configurazione del modulo.

* **[!UICONTROL Corpo]** (oggetto): A seconda della richiesta HTTP scelta durante la configurazione del modulo, è possibile che vengano restituiti alcuni dati. Tali dati, ad esempio i dati di un [!UICONTROL GET] è contenuto in questo oggetto.

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Salesforce] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Immettere un percorso relativo a<code> &lt;Instance URL&gt;/services/data/v46.0/</code>.</p> <p>Per l’elenco degli endpoint disponibili, consulta <a href="https://developer.salesforce.com/docs/atlas.en-us.api_rest.meta/api_rest/intro_what_is_rest_api.htm">Guida per gli sviluppatori dell’API REST di Salesforce</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL, Metodo]</p> </td> 
   td&gt; <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Aggiungi le intestazioni della richiesta sotto forma di un oggetto JSON standard. Ad esempio, <code>{"Content-type":"application/json"}</code>. Workfront Fusion aggiunge le intestazioni di autorizzazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>Aggiungi la query per la chiamata API sotto forma di un oggetto JSON standard. Ad esempio: <code>{"name":"something-urgent"}</code></p> </td> 
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

>[!INFO]
>
>**Esempio:** La seguente chiamata API restituisce l’elenco di tutti gli utenti nel tuo [!DNL Salesforce] account:
>
>* **URL**: `query`
>
>* **Metodo**: [!UICONTROL GET]
>
>* **Stringa query**:
>
>* **Chiave**: `q`
>
>* **Valore**: `SELECT Id, Name, CreatedDate, LastModifiedDate FROM User LIMIT 10`
>
>Le corrispondenze della ricerca si trovano nell&#39;Output del modulo in **[!UICONTROL Bundle] > [!UICONTROL Corpo] > [!UICONTROL record]**.
>
>Nel nostro esempio, sono stati restituiti 6 utenti:
>
>![](assets/matches-of-the-search-350x573.png)


#### [!UICONTROL Carica allegato/documento]

Questo modulo di azione carica un file e lo allega a un record specificato o carica un documento.

Il modulo restituisce l’ID dell’allegato o del documento e di tutti i campi associati, insieme a tutti i campi e valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Salesforce] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo di caricamento]</td> 
   <td>Seleziona se desideri che il modulo carichi un allegato o un documento.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td>Immettere o mappare l'ID dell'oggetto a cui si desidera caricare un allegato.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cartella]</td> 
   <td>Seleziona la cartella contenente il file da caricare nel modulo. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File di origine]</td> 
   <td>Selezionare un file di origine da un modulo precedente o mappare il nome e i dati del file di origine.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Scarica allegato/documento]

Questo modulo di azione scarica un documento o un allegato da un record.

Specifica l&#39;ID del record e il tipo di download desiderato.

Il modulo restituisce l’ID dell’allegato o del documento e di tutti i campi associati, insieme a tutti i campi e valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr>
    <td>[!UICONTROL Connection]</td>
   <td> <p>Per istruzioni su come collegare le [!DNL Salesforce] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Tipo di download]</td>
    <td> <p>Specifica il tipo di file da scaricare da Salesforce.</p> 
     <ul> 
      <li>Allegato [!UICONTROL]</li> 
      <li>[!UICONTROL Document]</li> 
      <li>[!UICONTROL ContentDocument] (documento caricato in una libreria in [!DNL Saleforce CRM Content] o [!DNL Salesforce Files].)</li> 
     </ul> </td>
  </tr> 
  <tr>
    <td> <p>[!UICONTROL ID] / </p> <p>[!UICONTROL Attachment ID] / </p> <p>[!UICONTROL ContentDocument ID]</p> </td>
    <td> <p>Immetti o mappa l'univoco [!DNL Salesforce] ID del record che si desidera scaricare dal modulo.</p> <p>Per ottenere l'ID, apri la [!DNL Salesforce] nel browser e copia il testo alla fine dell’URL dopo l’ultima barra (/). Ad esempio: <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td>
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL Aggiornare un record]

Questo modulo di azione modifica un record in un oggetto.

Il modulo ti consente di selezionare i campi dell’oggetto disponibili nel modulo. Questo riduce il numero di campi da scorrere durante la configurazione del modulo.

Il modulo restituisce l’ID del record e di tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Salesforce] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td>Immettere o mappare l'ID del record che si desidera aggiornare.</td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Tipo di record] </p> </td> 
   <td> <p>Seleziona il tipo di [!DNL Salesforce] registrare che si desidera aggiornare il modulo. I campi diventano disponibili in base al tipo di record selezionato nel campo Tipo di record . Questi campi sono basati sulle [!DNL Salesforce] API.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Seleziona campi da mappare]</td> 
   <td> <p>Selezionare i campi che si desidera configurare dal modulo al momento della creazione del nuovo record. I campi obbligatori si trovano nella parte superiore dell’elenco. </p> <p>I campi selezionati vengono aperti sotto questo campo. È ora possibile immettere i valori in questi campi.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Ricerche

#### [!UICONTROL Ricerca con query]

Questo modulo di ricerca cerca i record in un oggetto in [!DNL Salesforce] che corrispondono alla query di ricerca specificata. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Salesforce] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Search Type]</td> 
   <td> <p>Selezionare il tipo di ricerca che si desidera eseguire nel modulo:</p> 
    <ul> 
     <li> <p>[!UICONTROL Semplice]</p> </li> 
     <li> <p>[!UICONTROL Using SOSL (Salesforce Object Search Language)]</p> </li> 
     <li> <p>[!UICONTROL Using SOQL (Salesforce Object Query Language)]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Type] </p> </td> 
   <td> <p>Se hai selezionato il tipo di ricerca Semplice, scegli il tipo di [!DNL Salesforce] registrare che si desidera cercare nel modulo.</p> </td> 
  </tr> 
  <tr> 
   <td>Query [!UICONTROL] / Query SOSL] / Query SOQL [!UICONTROL]</td> 
   <td> <p>Immettere la query per la quale si desidera eseguire la ricerca.</p> <p>Per ulteriori informazioni su SOSL, vedi <a href="https://developer.salesforce.com/docs/atlas.en-us.soql_sosl.meta/soql_sosl/sforce_api_calls_sosl.htm">SOSL (Salesforce Object Search Language)</a> in [!DNL Salesforce] documentazione.</p> <p>Per ulteriori informazioni su SOQL, vedi <a href="https://developer.salesforce.com/docs/atlas.en-us.soql_sosl.meta/soql_sosl/sforce_api_calls_soql.htm">SOQL (Salesforce Object Query Language)</a> in [!DNL Salesforce] documentazione.</p> <p>Nota: Si prega di notare che il valore del parametro <code>RETURNING </code>influenza l’output del modulo. Se utilizzi <code>LIMIT</code>, [!DNL Fusion] ignora le impostazioni nel campo [!UICONTROL Numero massimo di record]. Se non si imposta alcun limite, Fusion inserirà il valore [!UICONTROL LIMIT = conteggio massimo dei record].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Conteggio massimo dei record]</td> 
   <td> <p>Immettere o mappare il numero massimo di record che si desidera restituire dal modulo durante ogni ciclo di esecuzione degli scenari.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ricerca]

Questo modulo di azione recupera tutti i record che soddisfano un determinato criterio.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Per istruzioni su come collegare le [!DNL Salesforce] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a[!DNL  Adobe Workfront Fusion] - Istruzioni di base</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type]</td> 
   <td> <p>Selezionare il tipo di oggetto da cercare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Criteri di ricerca]</td> 
   <td>Selezionare il campo di cui si desidera eseguire la ricerca, l’operatore da utilizzare nella query e il valore ricercato nel campo. È possibile collegare le query utilizzando AND o OR.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Uscite]</td> 
   <td>Seleziona i campi da includere nell’output del modulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Set di risultati]</td> 
   <td>Selezionare se si desidera che il modulo restituisca tutti i record corrispondenti o solo il record corrispondente.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Massimo [!UICONTROL]</td> 
   <td>Immettere o mappare il numero massimo di record che si desidera recuperare dal modulo durante ogni ciclo di esecuzione degli scenari.</td> 
  </tr> 
 </tbody> 
</table>
