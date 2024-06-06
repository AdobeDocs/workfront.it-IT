---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli Microsoft Dynamics 365
description: In un [!DNL Adobe Workfront Fusion] scenario, puoi automatizzare i flussi di lavoro che utilizzano Microsoft Dynamics 365 e collegarlo a più applicazioni e servizi di terze parti.
author: Becky
feature: Workfront Fusion
exl-id: 116df088-20a7-40a8-8880-9f422dc37632
source-git-commit: 46c282062ed737be860aeb4af96ac5f5efe9360d
workflow-type: tm+mt
source-wordcount: '1633'
ht-degree: 0%

---

# [!DNL Microsoft Dynamics 365 modules]

In un [!DNL Adobe Workfront Fusion] scenario, puoi automatizzare i flussi di lavoro che utilizzano [!DNL Microsoft Dynamics 365], oltre a collegarlo a più applicazioni e servizi di terze parti.

>[!NOTE]
>
>Il [!DNL Microsoft Dynamics 365] il connettore non supporta [!DNL Dynamics Finance and Operations].

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

Da utilizzare [!DNL Microsoft Dynamics] 365, è necessario disporre di un [!DNL Microsoft Dynamics 365] account.

## Connettere Microsoft Dynamics 365 a Workfront Fusion

Puoi creare una connessione al tuo [!DNL Microsoft Dynamics 365] account direttamente da un [!DNL Microsoft Dynamics 365] modulo.

1. In qualsiasi [!DNL Microsoft Dynamics 365] modulo, fai clic su **[!UICONTROL Aggiungi]** accanto al [!UICONTROL Connessione] campo.
1. Immettere un nome per la connessione.
1. In **[!UICONTROL Risorsa]** , immettere l&#39;indirizzo del [!DNL Dynamics 365] account, senza `https://`.
1. Clic **[!UICONTROL Continua]** per creare la connessione e tornare al modulo.

>[!NOTE]
>
>Durante la registrazione [!DNL Workfront Fusion] nel tuo [!DNL Microsoft Azure] , utilizza il seguente URI di reindirizzamento:
>
>* `https://app.workfrontfusion.com/oauth/cb/workfront-microsoft-dynamics2`


## [!DNL Microsoft Dynamics 365] moduli e relativi campi

Quando si configura [!DNL Microsoft Dynamics 365] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL Microsoft Dynamics 365] I campi potrebbero essere visualizzati in base a fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se viene visualizzato il pulsante Mappa sopra un campo o una funzione, è possibile utilizzarlo per impostare variabili e funzioni per tale campo. Per ulteriori informazioni, consulta [Mappare le informazioni da un modulo all’altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [[!UICONTROL Osserva record (pianificato)]](#watch-records-scheduled)
* [[!UICONTROL Record di controllo (tempo reale)]](#watch-records-real-time)
* [[!UICONTROL Crea record]](#create-record)
* [[!UICONTROL Effettuare una chiamata API]](#make-an-api-call)
* [[!UICONTROL Elimina record]](#delete-record)
* [[!UICONTROL Leggi record]](#read-records)
* [[!UICONTROL Aggiorna record]](#update-record)
* [[!UICONTROL Cerca record]](#search-records)

### [!UICONTROL Osserva record (pianificato)]

Questo modulo trigger pianificato esegue uno scenario quando un record nell&#39;oggetto specificato viene creato o aggiornato dopo l&#39;ultima esecuzione pianificata in [!DNL Dynamics 365].

L’output del modulo indica se il record trovato è nuovo o aggiornato (se è stato aggiunto e aggiornato nel periodo di tempo, viene contrassegnato come nuovo). Puoi mappare queste informazioni nei moduli successivi nello scenario.

Questo si verifica in un intervallo pianificato regolare specificato.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Per istruzioni sulla connessione [!DNL Microsoft Dynamics 365] account a [!DNL Workfront Fusion], vedi <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Microsoft Dynamics 365] a [!DNL Workfront Fusion]</a> in questo articolo. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Include]</td> 
   <td>Seleziona se desideri che il modulo venga controllato <strong>[!UICONTROL Solo nuovi record]</strong>, <strong>[!UICONTROL Solo record aggiornati]</strong>, o <strong>[!UICONTROL Nuovi record e tutte le modifiche]</strong>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di entità]</td> 
   <td>Scegliere il tipo di record [!UICONTROL Microsoft Dynamics 365] che si desidera controllare nello scenario.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output]</td> 
   <td> <p>Seleziona le informazioni da includere nel bundle di output per questo modulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Max record]</td> 
   <td> <p>Immettere o mappare il numero massimo di record che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Record di controllo (tempo reale)]

Questo modulo di attivazione immediata esegue uno scenario quando un record (oggetto) specificato viene creato o aggiornato in [!DNL Dynamics 365].

In questo modulo è necessario un webhook.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>Seleziona il webhook da utilizzare per questo modulo. </p> <p>Per aggiungere un nuovo webhook:</p> 
    <ol> 
     <li value="1"> <p>Clic <strong>[!UICONTROL Add]</strong> a destra del campo Webhook</p> </li> 
     <li value="2"> <p>In <strong>[!UICONTROL Webhook]</strong> nome, digita un nome descrittivo per il webhook.</p> </li> 
     <li value="3"> <p>In <strong>[!UICONTROL Connection]</strong> , selezionare la connessione che si desidera utilizzare selezionata</p> <p>Per istruzioni sulla connessione [!DNL Microsoft Dynamics 365] account a [!DNL Workfront Fusion], vedi <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Microsoft Dynamics 365] a [!DNL Workfront Fusion]</a> in questo articolo. </p> </li> 
     <li value="4"> <p>Clic <strong>[!UICONTROL Salva]</strong> per salvare il webhook e tornare al modulo.</p> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Crea record]

Questo modulo di azione crea un&#39;entità, ad esempio un appuntamento o un task.

È possibile specificare informazioni sull&#39;entità da creare.

Il modulo restituisce l’ID della nuova entità e dei campi associati, insieme a eventuali campi e valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Microsoft Dynamics 365] account a [!DNL Workfront Fusion], vedi <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Microsoft Dynamics 365] a [!DNL Workfront Fusion]</a> in questo articolo. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di entità]</td> 
   <td>Selezionare il tipo di entità che si desidera creare nel modulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seleziona campi da mappare]</td> 
   <td>Selezionare i campi per i quali si desidera includere i valori al momento della creazione del record. I campi disponibili dipendono dal tipo di entità.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Campi proprietà [!UICONTROL]</td> 
   <td> Questi sono i campi selezionati. Immettere il valore desiderato per il record per una determinata proprietà. </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Effettuare una chiamata API]

Questo modulo di azione consente di effettuare una chiamata autenticata personalizzata al [!DNL Microsoft Dynamics 365] API. In questo modo, puoi creare un’automazione del flusso di dati che non può essere eseguita dall’altro [!DNL Microsoft Dynamics 365] moduli.

Il modulo restituisce informazioni sul codice di stato, le intestazioni e il corpo. Puoi mappare queste informazioni nei moduli successivi nello scenario.

Per ulteriori informazioni, consulta [!DNL Microsoft] documentazione sull’utilizzo di [!DNL Dynamics 365 Customer Engagement Web API].

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Per istruzioni sulla connessione [!DNL Microsoft Dynamics 365] account a [!DNL Workfront Fusion], vedi <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Microsoft Dynamics 365] a [!DNL Workfront Fusion]</a> in questo articolo. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> <p>Inserisci un percorso relativo a <code>&lt;Instance URL>/api/data/v9.1/</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> <p>Per ulteriori informazioni in</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Aggiungi le intestazioni della richiesta sotto forma di oggetto JSON standard.</p> <p>Ad esempio: <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] aggiunge le intestazioni di autorizzazione.</p> </td> 
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

### [!UICONTROL Elimina record]

Questo modulo di azione elimina un’entità.

Specifica l’ID dell’entità.

Il modulo restituisce l’ID dell’entità e degli eventuali campi associati, insieme a eventuali campi e valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Per istruzioni sulla connessione [!DNL Microsoft Dynamics 365] account a [!DNL Workfront Fusion], vedi <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Microsoft Dynamics 365] a [!DNL Workfront Fusion]</a> in questo articolo. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di entità]</td> 
   <td> <p>Selezionare il tipo di entità che si desidera eliminare dal modulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td> <p>Inserisci o mappa l’univoco [!DNL Microsoft Dynamics 365] ID del record che desideri eliminare dal modulo.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Leggi record]

Questo modulo di azione legge i dati da una singola entità in [!DNL Microsoft Dynamics 365].

Specifica l’ID dell’entità.

Il modulo restituisce l’ID dell’entità e degli eventuali campi associati, insieme a eventuali campi e valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Per istruzioni sulla connessione [!DNL Microsoft Dynamics 365] account a [!DNL Workfront Fusion], vedi <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Microsoft Dynamics 365] a [!DNL Workfront Fusion]</a> in questo articolo. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di entità]</td> 
   <td>Selezionate il tipo di entità che desiderate che venga letta dal modulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output]</td> 
   <td> <p>Seleziona le informazioni da includere nel bundle di output per questo modulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Inserisci o mappa l’univoco [!DNL Microsoft Dynamics 365] ID del record che desideri che il modulo legga.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Aggiorna record]

Questo modulo di azione aggiorna un’entità.

Specifica l’ID dell’entità.

Il modulo restituisce l’ID del record aggiornato e di tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Per istruzioni sulla connessione [!DNL Microsoft Dynamics 365] account a [!DNL Workfront Fusion], vedi <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Microsoft Dynamics 365] a [!DNL Workfront Fusion]</a> in questo articolo. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Tipo di entità]</td> 
   <td>Selezionare il tipo di entità che si desidera aggiornare nel modulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seleziona campi da mappare]</td> 
   <td>Selezionare i campi per i quali si desidera includere i valori al momento della creazione del record. I campi disponibili dipendono dal tipo di entità.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Campi proprietà [!UICONTROL]</td> 
   <td>Questi sono i campi selezionati. Immettere il valore desiderato per il record per una determinata proprietà.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Inserisci o mappa l’univoco [!DNL Microsoft Dynamics] ID 365 del record che si desidera aggiornare con il modulo.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Cerca record]

Questo modulo di ricerca cerca i record in un oggetto in [!DNL Microsoft Dynamics 365] che corrispondono alla query di ricerca specificata. Puoi mappare queste informazioni nei moduli successivi nello scenario.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Per istruzioni sulla connessione [!DNL Microsoft Dynamics 365] account a [!DNL Workfront Fusion], vedi <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Microsoft Dynamics 365] a [!DNL Workfront Fusion]</a> in questo articolo. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di entità]</td> 
   <td>Selezionare il tipo di entità che si desidera aggiornare nel modulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filters]</td> 
   <td> <p>Selezionare il filtro che si desidera utilizzare per la ricerca.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Filtri standard]</strong> </p> <p>Imposta il filtro selezionando un campo e un operatore e immettendo o mappando il valore che desideri cercare. Puoi utilizzare le regole AND o OR per il filtro.</p> </li> 
     <li> <p><strong>Funzioni query [!UICONTROL]</strong> </p> <p>Inserisci il [!DNL Dynamics 365] funzione di query API web che desideri utilizzare per eseguire ricerche. </p> <p>Per ulteriori informazioni sulle funzioni di query, consulta <a href="https://docs.microsoft.com/en-us/dynamics365/customer-engagement/web-api/queryfunctions?view=dynamics-ce-odata-9">Riferimento funzione query API Web</a> nel [!DNL Microsoft] documentazione.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sort]</td> 
   <td> <p>Specificare l'ordine di restituzione degli elementi. È possibile aggiungere più ordinamenti.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Field]</strong> </p> <p>Specificare il campo in base al quale ordinare i risultati.</p> </li> 
     <li> <p><strong>[!UICONTROL Direction]</strong> </p> <p>Specifica la direzione dell’ordinamento (crescente o decrescente).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Max record]</td> 
   <td> <p>Immettere o mappare il numero massimo di record che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output]</td> 
   <td> <p>Seleziona le informazioni da includere nel bundle di output per questo modulo.</p> </td> 
  </tr> 
 </tbody> 
</table>
