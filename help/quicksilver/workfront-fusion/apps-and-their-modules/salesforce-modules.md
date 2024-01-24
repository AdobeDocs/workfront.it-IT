---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli Salesforce
description: In uno scenario Adobe Workfront Fusion, puoi automatizzare i flussi di lavoro che utilizzano Salesforce, nonché collegarla a più applicazioni e servizi di terze parti.
author: Becky
feature: Workfront Fusion
exl-id: 3c8adcd9-fb5f-400d-9edd-6d9fc30cc728
source-git-commit: c51169c18bef8ac8126a04c08deb88d830517b0b
workflow-type: tm+mt
source-wordcount: '2740'
ht-degree: 0%

---

# [!DNL Salesforce] moduli

In uno scenario Adobe Workfront Fusion, puoi automatizzare i flussi di lavoro che utilizzano [!DNL Salesforce], oltre a collegarlo a più applicazioni e servizi di terze parti.

Per un video introduttivo sul connettore Salesforce, vedi:

* [Salesforce](https://video.tv.adobe.com/v/3427027/){target=_blank}

Per istruzioni sulla creazione di uno scenario, consulta [Creare uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Per informazioni sui moduli, consulta [Moduli in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

>[!NOTE]
>
>* Non tutte le edizioni di [!DNL Salesforce] disporre dell’accesso API. Per ulteriori informazioni, vedere [!DNL Salesforce] edizioni con accesso API su [!DNL Salesforce] Sito della community.
>* Per informazioni su errori specifici restituiti dal [!DNL Salesforce] API, consulta [!DNL Salesforce] Documenti API. Puoi anche controllare lo stato del [!DNL Salesforce] API per eventuali interruzioni del servizio.
>

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

Da utilizzare [!DNL Salesforce] moduli, è necessario disporre di un [!DNL Salesforce] account.

## Informazioni sulla ricerca [!DNL Salesforce] oggetti

Durante la ricerca di oggetti, è possibile immettere singole parole di ricerca o creare una query più complessa utilizzando caratteri jolly e operatori:

* Utilizza il carattere jolly asterisco (\*) in sostituzione di zero o più caratteri. Ad esempio, la ricerca di Ca\* trova gli elementi che iniziano con Ca
* Utilizza un carattere jolly con punto interrogativo (?) come sostituto di un singolo carattere. Ad esempio, la ricerca di Jo?n consente di trovare elementi con il termine John o Joan ma non Jon
* Utilizza l’operatore tra virgolette (&quot;&quot;) per trovare una corrispondenza esatta della frase. Ad esempio: &quot;Riunione del lunedì&quot;

Per ulteriori informazioni sulle possibilità di ricerca, vedi [!DNL Salesforce] documentazione per gli sviluppatori su SOQL e SOSL.

## [!DNL Salesforce] moduli e relativi campi

* [Triggers](#triggers)
* [Azioni](#actions)
* [Ricerche](#searches)

### Triggers

* [[!UICONTROL Controlla i record]](#watch-for-records)
* [[!UICONTROL Osservare i messaggi in uscita]](#watch-outbound-messages)
* [[!UICONTROL Osserva un campo]](#watch-a-field)

#### [!UICONTROL Controlla i record]

Questo modulo trigger esegue uno scenario quando viene creato o aggiornato un record in un oggetto. Il modulo restituisce tutti i campi standard associati al record o ai record, insieme a tutti i campi e i valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Salesforce] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Type] </td> 
   <td> <p>Seleziona il tipo di [!DNL Salesforce] registrare che si desidera che il modulo controlli.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Campi Record]</td> 
   <td>Selezionare i campi che si desidera controllare nel modulo. I campi disponibili dipendono dal tipo di record.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Conteggio massimo dei record]</td> 
   <td> <p>Immettere o mappare il numero massimo di record che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td> <p>Determinare se si desidera che lo scenario controlli solo i nuovi record del tipo selezionato o i nuovi record del tipo selezionato e tutte le altre modifiche apportate ai record di tale tipo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Osservare i messaggi in uscita]

Questo modulo di attivazione esegue uno scenario quando un utente invia un messaggio. Il modulo restituisce tutti i campi standard associati al record o ai record, insieme a tutti i campi e i valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario.

Questo modulo richiede una configurazione aggiuntiva:

1. Vai a [!DNL Salesforce] pagina di impostazione.

   Per accedere alla pagina di impostazione, individuare e fare clic sul pulsante &quot;[!UICONTROL Configurazione]&quot; nell’angolo in alto a destra del [!DNL Salesforce] account. Dalla sezione [!DNL Salesforce] , individua la &quot;[!UICONTROL Ricerca rapida]&quot; barra a sinistra. Cerca &quot;[!UICONTROL Regole flusso di lavoro].&quot;

1. Clic **[!UICONTROL Regole flusso di lavoro]**.
1. Nella sezione [!UICONTROL Regole flusso di lavoro] pagina visualizzata, fai clic su **[!UICONTROL Nuova regola]** e seleziona il tipo di oggetto a cui applicare la regola (ad esempio &quot;[!UICONTROL opportunità]&quot; se stai monitorando gli aggiornamenti dei record Opportunità).
1. Clic **[!UICONTROL Successivo]**.
1. Imposta un nome di regola, criteri di valutazione e criteri di regola, quindi fai clic su **[!UICONTROL Salva]** e **[!UICONTROL Successivo]**.

1. Clic **[!UICONTROL Fine]**.
1. Dalla regola del flusso di lavoro appena creata, fai clic su **[!UICONTROL Modifica]**..
1. Dalla sezione **[!UICONTROL Azione Aggiungi flusso di lavoro]** elenco a discesa, seleziona **[!UICONTROL Nuovo messaggio in uscita]**.

1. Specifica nome, descrizione, URL endpoint e campi da includere nel nuovo messaggio in uscita, quindi fai clic su **[!UICONTROL Salva]**.

   Il **[!UICONTROL URL endpoint]** contiene l&#39;URL fornito sul [!DNL Salesforce] [!UICONTROL Messaggio in uscita] in [!DNL Workfront Fusion].

1. Configurare uno scenario che inizia con [!UICONTROL Messaggio in uscita] evento.

1. Fai clic su **&lt;/>** in basso a destra e copia l’URL fornito.
1. Torna a **[!UICONTROL Regole flusso di lavoro]** , individuare la regola appena creata, quindi fare clic su **[!UICONTROL Attiva]**.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Webhook]</td> 
   <td> <p>Seleziona il webhook che desideri utilizzare per guardare i messaggi in uscita. Per aggiungere un webhook, fai clic su <strong>[!UICONTROL Add]</strong> e inserisci il nome e la connessione del webhook.</p> <p>Per istruzioni sulla connessione [!DNL Salesforce] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!UICONTROL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo di record] </td> 
   <td> <p>Seleziona il tipo di [!DNL Salesforce] registrare che si desidera che il modulo controlli i messaggi in uscita.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fields]</td> 
   <td> <p>Seleziona i campi che desideri che il modulo controlli per i messaggi in uscita. I campi disponibili dipendono dal tipo di record.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### *[!UICONTROL Osserva un campo]*

Questo modulo trigger avvia uno scenario quando un campo viene aggiornato in [!DNL Salesforce].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Salesforce] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo di record] </td> 
   <td> <p>Selezionare il tipo di record contenente il campo che si desidera controllare nel modulo. È necessario scegliere un tipo di record in cui sia attivato [!UICONTROL Field History] [!DNL Salesforce] configurazione. Per ulteriori informazioni, consulta <a href="https://help.salesforce.com/articleView?id=tracking_field_history.htm&amp;type=5">Tracciamento cronologia campi</a> nel [!DNL Salesforce] documentazione. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Field]</td> 
   <td> <p>Selezionare i campi che si desidera che il modulo controlli per verificare le modifiche.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td> <p>Immettere o mappare il numero massimo di campi che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Azioni

* [[!UICONTROL Crea un record]](#create-a-record)
* [[!UICONTROL Leggi un record]](#read-a-record)
* [[!UICONTROL Eliminare un record]](#delete-a-record)
* [[!UICONTROL Chiamata API personalizzata]](#custom-api-call)
* [[!UICONTROL Carica allegato/documento]](#upload-attachmentdocument)
* [[!UICONTROL Scarica allegato/documento]](#download-attachmentdocument)

#### [!UICONTROL Crea un record]

Questo modulo di azione crea un nuovo record in un oggetto.

Il modulo consente di selezionare quale dei campi dell’oggetto è disponibile nel modulo. Questo riduce il numero di campi da scorrere durante la configurazione del modulo.

Il modulo restituisce l’ID del record ed eventuali campi associati, insieme a eventuali campi e valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Salesforce] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Tipo di record] </p> </td> 
   <td> <p>Seleziona il tipo di [!DNL Salesforce] che si desidera creare nel modulo. I campi diventano disponibili in base al tipo di record selezionato nel campo [!UICONTROL Tipo di record]. Questi campi si basano su [!DNL Salesforce] API.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Seleziona campi da mappare]</td> 
   <td> <p>Selezionare i campi che si desidera configurare nel modulo durante la creazione del nuovo record. I campi obbligatori si trovano all’inizio dell’elenco. </p> <p>I campi selezionati vengono aperti sotto questo campo. È ora possibile immettere valori in questi campi.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Leggi un record]

Questo modulo di azione legge i dati da un singolo oggetto in [!DNL Salesforce].

Specifica l’ID del record.

Il modulo restituisce l’ID del record ed eventuali campi associati, insieme a eventuali campi e valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr>
    <td>[!UICONTROL Connection]</td>
   <td> <p>Per istruzioni sulla connessione [!DNL Salesforce] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Tipo di record]</td>
    <td>Seleziona il tipo di [!DNL Salesforce] record che si desidera impostare come [action] per il modulo.leggi.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Campi Record]</td>
    <td>Seleziona i campi che desideri che il modulo legga. Selezionare almeno un campo.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL ID]</td>
    <td> <p>Inserisci o mappa l’univoco [!DNL Salesforce] ID del record che desideri che il modulo legga.</p> <p>Per ottenere l’ID, apri la [!DNL Salesforce] nel browser e copia il testo alla fine dell’URL dopo l’ultima barra (/). Ad esempio: <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminare un record]

Questo modulo di azione elimina un record esistente in un oggetto.

Specifica l’ID del record.

Il modulo restituisce l’ID del record ed eventuali campi associati, insieme a eventuali campi e valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Salesforce] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo di record] </td> 
   <td> <p>Seleziona il tipo di [!DNL Salesforce] che si desidera eliminare dal modulo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>Inserisci o mappa l’univoco [!DNL Salesforce] ID del record che desideri eliminare dal modulo.</p> <p>Per ottenere l’ID, apri la [!DNL Salesforce] nel browser e copia il testo alla fine dell’URL dopo l’ultima barra (/). Ad esempio: <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Chiamata API personalizzata]

Questo modulo di azione consente di effettuare una chiamata autenticata personalizzata al [!DNL Salesforce] API. In questo modo, puoi creare un’automazione del flusso di dati che non può essere eseguita dall’altro [!DNL Salesforce] moduli.

Il modulo restituisce quanto segue:

* **[!UICONTROL Codice di stato]** (numero): indica l’esito positivo o negativo della richiesta HTTP. Si tratta di codici standard che puoi cercare su Internet.
* **[!UICONTROL Intestazioni]** (oggetto): contesto più dettagliato per il codice di risposta/stato che non è correlato al corpo di output. Non tutte le intestazioni visualizzate in un’intestazione di risposta sono intestazioni di risposta, quindi alcune potrebbero non essere utili.

  Le intestazioni di risposta dipendono dalla richiesta HTTP scelta durante la configurazione del modulo.

* **[!UICONTROL Corpo]** (oggetto): a seconda della richiesta HTTP scelta durante la configurazione del modulo, alcuni dati potrebbero essere restituiti. Tali dati, come i dati provenienti da un [!UICONTROL GET] richiesta, è contenuto in questo oggetto.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Salesforce] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Inserisci un percorso relativo a<code> &lt;Instance URL&gt;/services/data/v46.0/</code>.</p> <p>Per l’elenco degli endpoint disponibili, consulta <a href="https://developer.salesforce.com/docs/atlas.en-us.api_rest.meta/api_rest/intro_what_is_rest_api.htm">Guida per gli sviluppatori API REST di Salesforce</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Method]</p> </td> 
   td&gt; <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Aggiungi le intestazioni della richiesta sotto forma di oggetto JSON standard. Ad esempio, <code>{"Content-type":"application/json"}</code>. Workfront Fusion aggiunge automaticamente le intestazioni di autorizzazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Stringa Di Query]</td> 
   <td> <p>Aggiungi la query per la chiamata API sotto forma di oggetto JSON standard. Ad esempio: <code>{"name":"something-urgent"}</code></p> </td> 
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

>[!INFO]
>
>**Esempio:** La seguente chiamata API restituisce l’elenco di tutti gli utenti nel tuo [!DNL Salesforce] account:
>
>* **URL**: `query`
>
>* **Metodo**: [!UICONTROL GET]
>
>* **Stringa di query**:
>
>* **Chiave**: `q`
>
>* **Valore**: `SELECT Id, Name, CreatedDate, LastModifiedDate FROM User LIMIT 10`
>
>Le corrispondenze della ricerca si trovano nell’Output del modulo in **[!UICONTROL Bundle] > [!UICONTROL Corpo] > [!UICONTROL record]**.
>
>Nel nostro esempio, sono stati restituiti 6 utenti:
>
>![](assets/matches-of-the-search-350x573.png)


#### [!UICONTROL Carica allegato/documento]

Questo modulo di azione carica un file e lo allega a un record specificato oppure carica un documento.

Il modulo restituisce l’ID dell’allegato o del documento e tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Salesforce] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo di caricamento]</td> 
   <td>Seleziona se vuoi che il modulo carichi un allegato o un documento.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td>Immettere o mappare l'ID dell'oggetto a cui si desidera caricare un allegato.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder]</td> 
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

Specificare l&#39;ID del record e il tipo di download desiderato.

Il modulo restituisce l’ID dell’allegato o del documento e tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr>
    <td>[!UICONTROL Connection]</td>
   <td> <p>Per istruzioni sulla connessione [!DNL Salesforce] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Tipo di download]</td>
    <td> <p>Specifica il tipo di file da scaricare da Salesforce.</p> 
     <ul> 
      <li>[!UICONTROL Attachment]</li> 
      <li>[!UICONTROL Documento]</li> 
      <li>[!UICONTROL ContentDocument] (documento caricato in una raccolta in [!DNL Saleforce CRM Content] o [!DNL Salesforce Files].)</li> 
     </ul> </td>
  </tr> 
  <tr>
    <td> <p>[!UICONTROL ID] / </p> <p>[!UICONTROL ID allegato] / </p> <p>[!UICONTROL ID ContentDocument]</p> </td>
    <td> <p>Inserisci o mappa l’univoco [!DNL Salesforce] ID del record che desideri scaricare dal modulo.</p> <p>Per ottenere l’ID, apri la [!DNL Salesforce] nel browser e copia il testo alla fine dell’URL dopo l’ultima barra (/). Ad esempio: <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td>
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL Aggiornare un record]

Questo modulo di azione modifica un record in un oggetto.

Il modulo consente di selezionare quale dei campi dell’oggetto è disponibile nel modulo. Questo riduce il numero di campi da scorrere durante la configurazione del modulo.

Il modulo restituisce l’ID del record ed eventuali campi associati, insieme a eventuali campi e valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Salesforce] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td>Immetti o mappa l’ID del record da aggiornare.</td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Tipo di record] </p> </td> 
   <td> <p>Seleziona il tipo di [!DNL Salesforce] che desideri aggiornare il modulo. I campi diventano disponibili in base al tipo di record selezionato nel campo Tipo di record. Questi campi si basano su [!DNL Salesforce] API.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Seleziona campi da mappare]</td> 
   <td> <p>Selezionare i campi che si desidera configurare nel modulo durante la creazione del nuovo record. I campi obbligatori si trovano all’inizio dell’elenco. </p> <p>I campi selezionati vengono aperti sotto questo campo. È ora possibile immettere valori in questi campi.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Ricerche

#### [!UICONTROL Cerca con query]

Questo modulo di ricerca cerca i record in un oggetto in [!DNL Salesforce] che corrispondono alla query di ricerca specificata. Puoi mappare queste informazioni nei moduli successivi nello scenario.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Salesforce] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>Tipo di ricerca [!UICONTROL]</td> 
   <td> <p>Selezionare il tipo di ricerca che si desidera venga eseguita dal modulo:</p> 
    <ul> 
     <li> <p>[!UICONTROL semplice]</p> </li> 
     <li> <p>[!UICONTROL Tramite SOSL (Salesforce Object Search Language)]</p> </li> 
     <li> <p>[!UICONTROL Tramite SOQL (Salesforce Object Query Language)]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Type] </p> </td> 
   <td> <p>Se è stato selezionato il tipo di ricerca Semplice, scegliere il tipo di [!DNL Salesforce] record che si desidera cercare nel modulo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Query] / [!UICONTROL SOSL Query] / [!UICONTROL SOQL Query]</td> 
   <td> <p>Immettere la query in base alla quale si desidera eseguire la ricerca.</p> <p>Per ulteriori informazioni su SOSL, vedere <a href="https://developer.salesforce.com/docs/atlas.en-us.soql_sosl.meta/soql_sosl/sforce_api_calls_sosl.htm">Linguaggio di ricerca oggetti Salesforce (SOSL)</a> nel [!DNL Salesforce] documentazione.</p> <p>Per ulteriori informazioni su SOQL, vedere <a href="https://developer.salesforce.com/docs/atlas.en-us.soql_sosl.meta/soql_sosl/sforce_api_calls_soql.htm">Salesforce Object Query Language (SOQL)</a> nel [!DNL Salesforce] documentazione.</p> <p>Nota: il valore del parametro <code>RETURNING </code>influenza l’output del modulo. Se usa <code>LIMIT</code>, [!DNL Fusion] ignorerà le impostazioni nel campo [!UICONTROL Conteggio massimo dei record]. Se non si imposta alcun limite, verrà inserito il valore [!UICONTROL LIMIT = Maximal count of records].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Conteggio massimo dei record]</td> 
   <td> <p>Immettere o mappare il numero massimo di record che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</p> </td> 
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
   <td>Per istruzioni sulla connessione [!DNL Salesforce] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a[!DNL  Adobe Workfront Fusion] - Istruzioni di base</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type]</td> 
   <td> <p>Selezionare il tipo di oggetto che si desidera cercare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Criteri di ricerca di [!UICONTROL]</td> 
   <td>Selezionare il campo in base al quale si desidera eseguire la ricerca, l'operatore che si desidera utilizzare nella query e il valore ricercato nel campo. È possibile connettere le query utilizzando AND o OR.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output]</td> 
   <td>Selezionare i campi da includere nell'output del modulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Set di risultati]</td> 
   <td>Selezionare se si desidera che il modulo restituisca tutti i record corrispondenti o solo il primo record corrispondente.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL max]</td> 
   <td>Immettere o mappare il numero massimo di record che il modulo deve recuperare durante ogni ciclo di esecuzione dello scenario.</td> 
  </tr> 
 </tbody> 
</table>
