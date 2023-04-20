---
filename: airtable-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli aerei
description: Adobe Workfront Fusion richiede una licenza Adobe Workfront Fusion oltre a una licenza Adobe Workfront.
author: Becky
hidefromtoc: true
source-git-commit: 6955c979d504adb6514ae64bf5108174d7a90ce4
workflow-type: tm+mt
source-wordcount: '1863'
ht-degree: 2%

---


# Moduli aerei


Con la [!DNL Airtable] connettore per [!DNL Adobe Workfront Fusion], puoi avviare uno scenario basato sugli eventi nel [!DNL Airtable] account, creazione, caricamento e aggiornamento di record, record di ricerca e creazione di chiamate API personalizzate all&#39;API Airtable.

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

Devi disporre di un account Airtable per utilizzare la funzionalità di questo articolo.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information, see the tutorial .</p>
-->

## Connetti Airtable a Workfront Fusion {#connect-airtable-to-workfront-fusion}

<!--

1. Log in to your Airtable account.
1. Open your account overview and generate the API key.
-->
1. Aprire Workfront Fusion e **Creare una connessione** finestra di dialogo del modulo desiderato.
1. Immettere un nome per la connessione.
1. (Facoltativo) Fai clic su Mostra impostazioni avanzate e immetti il tuo ID client Airtable e il tuo segreto client.
1. Fai clic sul pulsante **Continua** per creare la connessione e tornare al modulo.

## Moduli e relativi campi

### Record

* [Creare un record](#create-a-record)
* [Eliminare un record](#delete-a-record)
* [Ottieni un record](#get-a-record)
* [Cerca record](#search-records)
* [Aggiornare un record](#update-a-record)
* [Aggiornare un record](#upsert-a-record)
* [Registra record](#watch-records)
* [Risposte di controllo](#watch-responses)
* [Effettuare una chiamata API](#make-an-api-call)

#### Creare un record {#create-a-record}

Questo modulo di azione crea un nuovo record.

È possibile specificare i dati desiderati nel record e la posizione in cui si desidera memorizzarli.

Il modulo restituisce tutti i campi standard associati al record, insieme a eventuali campi e valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connessione </td> 
   <td> <p>Per istruzioni su come collegare il tuo account Airtable a Workfront Fusion, vedi <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Connetti Airtable a Workfront Fusion</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>Base </td> 
   <td> <p>Selezionare la base a cui apparterrà il nuovo record.</p> </td> 
  </tr> 
  <tr> 
   <td>Tabella </td> 
   <td> <p>Selezionare la tabella a cui appartiene il nuovo record.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Inserimento</p> </td> 
   <td> <p>Immettere i valori per il nuovo record. I campi disponibili si basano sulla tabella selezionata.</p> <!--<p>For more information on field types, search for "Supported field types" in the Airtable documentation.</p> 
    <ul> 
     <li> <p><strong>Text</strong>: string</p> <p>A single line of text.</p> </li> 
     <li> <p><strong>Long text</strong>: string</p> <p>Multiple lines of text, which may contain "mention tokens", for example:</p><pre>&lt;airtable:mention id="menE1i9oBaGX3DseR"&gt;@Alex&lt;/airtable:mention&gt;</pre> </li> 
     <li><strong>Attachment</strong> : Add the attachment. Airtable will download the file from the provided <code>url</code> and keep its own copy of it. If the File name field is left empty, Airtable generates the name automatically.</li> 
     <li><strong>Checkbox</strong>: Select one of the options.</li> 
     <li><strong>Multiple select</strong>: Select multiple options in the checklist.</li> 
     <li><strong>Single select</strong>: Select one option from the drop-down menu.</li> 
     <li><strong>Collaborator</strong>: Enter the email that uniquely identifies a user in Airtable who this base is shared with.</li> 
     <li><strong>Date</strong>: UTC date, for example, 2019-09-05 (ISO 8601 formatted date)</li> 
     <li>Phone number:</li> 
     <li><strong>Emails</strong>: A valid email address.</li> 
     <li><strong>URL</strong>: A valid URL (for example, airtable.com or https://airtable.com/universe).</li> 
     <li><strong>Number</strong>: Enter a number.</li> 
     <li><strong>Currency</strong>: Currency value.</li> 
     <li><strong>Percent</strong>: A percentage value. Must be higher than or equal to 0.</li> 
     <li><strong>Duration</strong>: Enter the duration time. If you need help, see the information about the duration field type in the Airtable support documentation. </li> 
     <li><strong>Rating</strong>: Enter the number. For example, "3 stars" is 3. A rating cannot be 0.</li> 
     <li><strong>Link</strong>: Enter the linked records IDs from the table. The order of record IDs will be reversed compared to what you see in the app.</li> 
     <li><strong>Rollup</strong>: Computed value: COUNT(values)</li> 
     <li><strong>Lookup</strong>: Array of long text fields</li> 
     <li><strong>Autonumber</strong>: Automatically incremented unique counter for each record.</li> 
     <li> <p><strong>Barcode</strong>: The barcode object may contain the following two properties, both of which are optional.</p> <p>Barcode data (text)</p> <p>Barcode symbology, for example, "upce" or "code39" (type)</p> </li> 
    </ul> --></td> 
  </tr> 
  <tr> 
   <td>Collegamenti intelligenti</td> 
   <td> <p>Abilitare questa opzione per immettere nomi invece degli ID record nei campi che si collegano a un’altra tabella. Il record viene creato automaticamente nella tabella collegata in assenza di corrispondenza.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Eliminare un record {#delete-a-record}

Questo modulo di azione elimina un record specifico.

Puoi specificare l’ID e le posizioni del record.

Il modulo restituisce l’ID del record e di tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connessione </td> 
   <td> <p>Per istruzioni su come collegare il tuo account Airtable a Workfront Fusion, vedi <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Connetti Airtable a Workfront Fusion</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>Base </td> 
   <td> <p>Selezionare la base contenente il record da eliminare.</p> </td> 
  </tr> 
  <tr> 
   <td>Tabella </td> 
   <td> <p>Selezionare la tabella contenente il record da eliminare.</p> </td> 
  </tr> 
  <tr> 
   <td>ID record</td> 
   <td> <p>Immettere o mappare l'ID Airtable univoco del record che si desidera eliminare dal modulo. Ad esempio, puoi recuperare l’ID utilizzando il modulo Cerca record .</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Ottieni un record {#get-a-record}

Questo modulo di azione recupera i dettagli dei record.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connessione </td> 
   <td> <p>Per istruzioni su come collegare il tuo account Airtable a Workfront Fusion, vedi <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Connetti Airtable a Workfront Fusion</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>Base </td> 
   <td> <p>Selezionare la base che contiene la tabella con il record che si desidera recuperare.</p> </td> 
  </tr> 
  <tr> 
   <td>Tabella</td> 
   <td> <p> Selezionare la tabella contenente il record per il quale si desidera recuperare i dettagli.</p> </td> 
  </tr> 
  <tr> 
   <td>ID record</td> 
   <td> <p> Immettere o mappare l'ID del record per il quale si desidera recuperare i dettagli.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Cerca record {#search-records}

Questo modulo di ricerca cerca i record di un oggetto in Airtable che corrispondono alla query di ricerca specificata.

Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connessione </td> 
   <td> <p>Per istruzioni su come collegare il tuo account Airtable a Workfront Fusion, vedi <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Connetti Airtable a Workfront Fusion</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>Base </td> 
   <td> <p>Selezionare la base in cui si desidera cercare i record.</p> </td> 
  </tr> 
  <tr> 
   <td>Tabella </td> 
   <td> <p>Selezionare la tabella che si desidera cercare.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Formula</p> </td> 
   <td> <p>Formula utilizzata per filtrare i record. La formula viene valutata per ogni record e se il risultato non è <code>0</code>, <code>false</code>, <code>""</code>, <code>NaN</code>, <code>[]</code>oppure <code>#Error!</code> il record viene incluso nella risposta.</p> <p>Se combinato con <code>view</code>, vengono restituiti solo i record che soddisfano la formula.</p> <p>Ad esempio, per includere solo i record in cui Nome non è vuoto, passa:<code> NOT({Name} = '')</code></p> <p>Per ulteriori informazioni, cercare informazioni sui riferimenti ai campi formula nella documentazione relativa al supporto Airtable.</p> </td> 
  </tr> 
  <tr> 
   <td>Ordina </td> 
   <td> <p>Selezionare la direzione di ordinamento e il campo in base al quale si desidera ordinare i risultati.</p> </td> 
  </tr> 
  <tr> 
   <td>Visualizza </td> 
   <td> <p>Selezionare la visualizzazione in cui si desidera cercare i record.</p> </td> 
  </tr> 
  <tr> 
   <td>Limite</td> 
   <td> <p>Immettere o mappare il numero massimo di record che si desidera restituire dal modulo durante ogni ciclo di esecuzione degli scenari.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Aggiornare un record {#update-a-record}

Questo modulo di azione aggiorna un record specifico.

Specificare l&#39;ID del record e i nuovi dati che si desidera contenere.

Il modulo restituisce tutti i campi standard associati al record, insieme a eventuali campi e valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connessione </td> 
   <td> <p>Per istruzioni su come collegare il tuo account Airtable a Workfront Fusion, vedi <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Connetti Airtable a Workfront Fusion</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>Base </td> 
   <td> <p>Selezionare la base contenente il record da aggiornare.</p> </td> 
  </tr> 
  <tr> 
   <td>Tabella </td> 
   <td> <p>Selezionare la tabella contenente il record da aggiornare.</p> </td> 
  </tr> 
  <tr> 
   <td>ID record </td> 
   <td> <p>Immettere o mappare l'ID Airtable univoco del record che si desidera aggiornare nel modulo. Ad esempio, puoi recuperare l’ID utilizzando il modulo Cerca record .</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Inserimento</p> </td> 
   <td> <p>Immettere i valori per il nuovo record. I campi disponibili dipendono dalla tabella selezionata.</p> <!--<p>In order to delete the content of the field, use the erase function. </p>  <p>Field types (via airtable.com/api):</p> 
    <ul> 
     <li> <p><strong>Text</strong>: string</p> <p>A single line of text.</p> </li> 
     <li> <p><strong>Long text</strong>: string</p> <p>The string can contain multiple lines of text with "mention tokens." For example:</p><pre>&lt;airtable:mention id="menE1i9oBaGX3DseR"&gt;@Alex&lt;/airtable:mention&gt;</pre> </li> 
     <li><strong>Attachment</strong>: Add the attachment. Airtable will download the file from the provided url and keep its own copy of it. If the File name field is left empty, Airtable will generate the name automatically.</li> 
     <li><strong>Checkbox</strong>: Select one of the options.</li> 
     <li><strong>Multiple select</strong>: Select multiple options in the checklist.</li> 
     <li><strong>Single select</strong>: Select one option from the drop-down menu.</li> 
     <li><strong>Collaborator</strong>: Enter the email that uniquely identifies a user in Airtable who this base is shared with.</li> 
     <li><strong>Date</strong>: UTC date, for example, 2019-09-05. (ISO 8601 formatted date)</li> 
     <li><strong>Phone number</strong>: A telephone number, for example, (415) 555-9876.</li> 
     <li><strong>Email</strong>valid email address.</li> 
     <li><strong>URL</strong>: lid URL such as airtable.com or https://airtable.coiverse.</li> 
     <li><strong>Number</strongnter a number.</li> 
     <li><strong>Currency</stro Currency value.</li> 
     <li><strong>Percent</stronA percentage value; must be equal to or more than 0i> 
     <li><strong>Duration</strong>: Enter the duration time. If you need help, see the information about the duration field type in the Airtable support documentation.</li> 
     <li><strong>Rating</strong>: Enter the number. For example, "3 stars" is 3. A rating cannot be 0.</li> 
     <li><strong>Link</strong>: Enter the linked records IDs from the table. The order of record IDs is reversed compared to what you see in the app.</li> 
     <li><strong>Rollup</strong>: Computed value: COUNT(values)</li> 
     <li><strong>Lookup</strong>: Array of long text fields</li> 
     <li><strong>Autonumber</strong>: Automatically incremented unique counter for each record.</li> 
     <li> <p><strong>Barcode</strong>: The barcode object may contain the following two properties, both of which are optional.</p> <p>Barcode data (text)</p> <p>Barcode symbology, for example, "upce" or "code39" (type)</p> </li> 
    </ul> --></td> 
  </tr> 
  <tr> 
   <td>Collegamenti intelligenti</td> 
   <td> <p>Immettere i nomi invece degli ID dei record nei campi collegati a un’altra tabella. Il record viene creato automaticamente nella tabella collegata in assenza di corrispondenza.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Aggiornare un record

Questo modulo di azione aggiorna o inserisce un record specifico.

Specificare l&#39;ID del record e i nuovi dati che si desidera contenere.

Il modulo restituisce tutti i campi standard associati al record, insieme a eventuali campi e valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connessione </td> 
   <td> <p>Per istruzioni su come collegare il tuo account Airtable a Workfront Fusion, vedi <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Connetti Airtable a Workfront Fusion</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>Base </td> 
   <td> <p>Selezionare la base contenente il record da aggiornare.</p> </td> 
  </tr> 
  <tr> 
   <td>Tabella </td> 
   <td> <p>Selezionare la tabella contenente il record da aggiornare.</p> </td> 
  </tr> 
  <tr> 
   <td>ID record </td> 
   <td> <p>Se si aggiorna un record, immettere o mappare l'ID univoco della tabella aerea del record che si desidera aggiornare nel modulo. Ad esempio, puoi recuperare l’ID utilizzando il modulo Cerca record .</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Inserimento</p> </td> 
   <td> <p>Immettere i valori per il nuovo record. I campi disponibili dipendono dalla tabella selezionata.</p> <!-- <p>In order to delete the content of the field, use the erase function. </p>  <p>Field types (via airtable.com/api):</p> 
    <ul> 
     <li> <p><strong>Text</strong>: string</p> <p>A single line of text.</p> </li> 
     <li> <p><strong>Long text</strong>: string</p> <p>The string can contain multiple lines of text with "mention tokens." For example:</p><pre>&lt;airtable:mention id="menE1i9oBaGX3DseR"&gt;@Alex&lt;/airtable:mention&gt;</pre> </li> 
     <li><strong>Attachment</strong>: Add the attachment. Airtable will download the file from the provided url and keep its own copy of it. If the File name field is left empty, Airtable will generate the name automatically.</li> 
     <li><strong>Checkbox</strong>: Select one of the options.</li> 
     <li><strong>Multiple select</strong>: Select multiple options in the checklist.</li> 
     <li><strong>Single select</strong>: Select one option from the drop-down menu.</li> 
     <li><strong>Collaborator</strong>: Enter the email that uniquely identifies a user in Airtable who this base is shared with.</li> 
     <li><strong>Date</strong>: UTC date, for example, 2019-09-05. (ISO 8601 formatted date)</li> 
     <li><strong>Phone number</strong>: A telephone number, for example, (415) 555-9876.</li> 
     <li><strong>Email</strong>valid email address.</li> 
     <li><strong>URL</strong>: lid URL such as airtable.com or https://airtable.coiverse.</li> 
     <li><strong>Number</strongnter a number.</li> 
     <li><strong>Currency</stro Currency value.</li> 
     <li><strong>Percent</stronA percentage value; must be equal to or more than 0i> 
     <li><strong>Duration</strong>: Enter the duration time. If you need help, see the information about the duration field type in the Airtable support documentation.</li> 
     <li><strong>Rating</strong>: Enter the number. For example, "3 stars" is 3. A rating cannot be 0.</li> 
     <li><strong>Link</strong>: Enter the linked records IDs from the table. The order of record IDs is reversed compared to what you see in the app.</li> 
     <li><strong>Rollup</strong>: Computed value: COUNT(values)</li> 
     <li><strong>Lookup</strong>: Array of long text fields</li> 
     <li><strong>Autonumber</strong>: Automatically incremented unique counter for each record.</li> 
     <li> <p><strong>Barcode</strong>: The barcode object may contain the following two properties, both of which are optional.</p> <p>Barcode data (text)</p> <p>Barcode symbology, for example, "upce" or "code39" (type)</p> </li> 
    </ul> --></td> 
  </tr> 
  <tr> 
   <td>Collegamenti intelligenti</td> 
   <td> <p>Immettere i nomi invece degli ID dei record nei campi collegati a un’altra tabella. Il record viene creato automaticamente nella tabella collegata in assenza di corrispondenza.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Registra record {#watch-records}

Questo modulo di attivazione avvia uno scenario quando un record viene creato o aggiornato nella tabella specificata.

>[!NOTE]
>
>Per utilizzare questo modulo, è necessario creare nella tabella il campo Ora creazione o Ora ultima modifica.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connessione </td> 
   <td> <p>Per istruzioni su come collegare il tuo account Airtable a Workfront Fusion, vedi <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Connetti Airtable a Workfront Fusion</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>Base </td> 
   <td> <p>Selezionare la base che si desidera controllare per i nuovi record.</p> </td> 
  </tr> 
  <tr> 
   <td>Tabella </td> 
   <td> <p>Selezionare la tabella che si desidera controllare per i nuovi record.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Configurazione del trigger</p> </td> 
   <td> <p>Campo trigger</p> <p>A <code>Created Time</code> o <code>Last Modified Time</code> campo utilizzato per ordinare i record. Se non hai una <code>Created Time</code> o <code>Last Modified Time</code> nel tuo schema, devi crearne uno. </p> <p>Campo etichetta</p> <p>Campo utilizzato come etichetta per un record, ad esempio nella finestra di dialogo Scegli dove iniziare.</p> </td> 
  </tr> 
  <tr> 
   <td>Limite</td> 
   <td> <p>Immettere o mappare il numero massimo di record che si desidera che il modulo visualizzi durante ogni ciclo di esecuzione degli scenari.</p> </td> 
  </tr> 
  <tr> 
   <td>Visualizza</td> 
   <td> <p>Selezionare la visualizzazione da utilizzare.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Formula</p> </td> 
   <td> <p>Formula utilizzata per filtrare i record. La formula viene valutata per ogni record e se il risultato non è <code>0</code>, <code>false</code>, <code>""</code>, <code>NaN</code>, <code>[]</code>oppure <code>#Error!</code> il record viene incluso nella risposta.</p> <p>Se combinato con <code>view</code>, vengono restituiti solo i record che soddisfano la formula.</p> <p>Ad esempio, per includere solo i record in cui Nome non è vuoto, passa:<code> NOT({Name} = '')</code></p> <p>Per ulteriori informazioni, vedere le informazioni sui riferimenti ai campi formula nella documentazione relativa al supporto Airtable.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Risposte di controllo

Questo modulo di attivazione avvia uno scenario in cui viene inviato un modulo.

>[!NOTE]
>
>Questa funzionalità è disponibile solo per i piani Airtable Pro a pagamento.

L’URL del webhook deve essere generato in Workfront Fusion e quindi aggiunto alla configurazione del modulo in Airtable.

1. Aggiungi il modulo Nuove risposte allo scenario Workfront Fusion.
1. Genera e copia l’URL del webhook.

   Per istruzioni, consulta [Trigger istantanei (webhook) in Adobe Workfront Fusion](../../workfront-fusion/webhooks/instant-triggers-webhooks.md).

1. Accedi al tuo account Airtable.
1. Aprire la base e la tabella che si desidera utilizzare per il modulo e creare una visualizzazione Modulo.
1. Impostare il modulo come necessario, scorrere il modulo verso il basso e abilitare l’opzione Reindirizza a URL dopo l’invio del modulo.
1. Inserisci l&#39;URL Webhook generato al passaggio 2 nella finestra di dialogo visualizzata e aggiungi la ?record_id={record_id} subito dopo l&#39;URL del webhook per includere l&#39;ID record nell&#39;output del modulo, quindi fai clic su Salva. L’URL risultante, ad esempio, sarà simile al seguente:
1. Torna al tuo scenario Workfront Fusion ed esegui il modulo Watch Responses solo per caricare i campi da Airtable e per essere in grado di mappare tali campi negli altri moduli.
1. Invia il modulo in Airtable dove l’opzione Reindirizza all’URL dopo l’invio del modulo è abilitata e viene aggiunto l’URL Webhook (passaggio 6 sopra).

   Viene attivato il modulo Risposte di controllo e vengono caricati i dati desiderati.

1. Aggiungi il modulo Airtable > Get a Record (Ottieni un record) subito dopo il modulo Airtable > Watch Responses (Tabella volo) e mappa il record_id al campo Record ID (ID record).

Ora, ogni volta che il modulo viene inviato, viene attivato il modulo Risposte di controllo nello scenario Workfront Fusion e il modulo Ottieni un record restituisce i dettagli del modulo inviato.

#### Effettuare una chiamata API

#### Chiamata API personalizzata

Questo modulo di azione ti consente di effettuare una chiamata autenticata personalizzata al [!DNL Airtable] API. In questo modo, puoi creare un’automazione del flusso di dati che non può essere eseguita dall’altro [!DNL Airtable] moduli.

L&#39;azione si basa sul tipo di entità (tipo di oggetto Allocadia) specificato.

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connessione</p> </td> 
   <td> <p>Per istruzioni su come collegare il tuo account Airtable a Workfront Fusion, vedi <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Connetti Airtable a Workfront Fusion</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td>Immettere un percorso relativo a <code>https://api.airtable.com/}</code>. Esempio: <code>v0/{base}/{table}</code> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Metodo</td> 
   <td> <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Intestazioni</td> 
   <td> <p>Aggiungi le intestazioni della richiesta sotto forma di un oggetto JSON standard.</p> <p>Ad esempio: <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] aggiunge le intestazioni di autorizzazione per te.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Stringa query</td> 
   <td> <p>Aggiungi la query per la chiamata API sotto forma di chiave e valore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Corpo</td> 
   <td> <p>Aggiungi il contenuto del corpo per la chiamata API sotto forma di un oggetto JSON standard.</p> <p>Nota:  <p>Quando si utilizzano istruzioni condizionali come <code>if</code> nel JSON, inserisci le virgolette al di fuori dell’istruzione condizionale.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>
