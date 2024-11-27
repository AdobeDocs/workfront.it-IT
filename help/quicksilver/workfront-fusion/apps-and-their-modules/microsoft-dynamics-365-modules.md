---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli Microsoft Dynamics 365
description: In uno scenario  [!DNL Adobe Workfront Fusion] , puoi automatizzare i flussi di lavoro che utilizzano Microsoft Dynamics 365 e collegarlo a più applicazioni e servizi di terze parti.
author: Becky
feature: Workfront Fusion
exl-id: 116df088-20a7-40a8-8880-9f422dc37632
source-git-commit: f6b00b98d3375e5660d684f1fad682fa721517aa
workflow-type: tm+mt
source-wordcount: '1733'
ht-degree: 0%

---

# [!DNL Microsoft Dynamics 365 modules]

In uno scenario [!DNL Adobe Workfront Fusion], è possibile automatizzare i flussi di lavoro che utilizzano [!DNL Microsoft Dynamics 365] e collegarlo a più applicazioni e servizi di terze parti.

>[!NOTE]
>
>Il connettore [!DNL Microsoft Dynamics 365] non supporta [!DNL Dynamics Finance and Operations].
>
>Per i moduli Finanza e Operazioni di Microsoft Dynamics 365, vedere [[!DNL Microsoft Dynamics 365 Finance and Operations modules]](/help/quicksilver/workfront-fusion/apps-and-their-modules/dynamics-finance-operations-modules.md).

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

Per usare [!DNL Microsoft Dynamics] 365, devi avere un account [!DNL Microsoft Dynamics 365].

## Collegare Microsoft Dynamics 365 a Workfront Fusion

Puoi creare una connessione al tuo account [!DNL Microsoft Dynamics 365] direttamente dall&#39;interno di un modulo [!DNL Microsoft Dynamics 365].

>[!NOTE]
>
>Alcune app Microsoft utilizzano la stessa connessione, che è associata alle autorizzazioni dei singoli utenti. Pertanto, durante la creazione di una connessione, nella schermata di consenso delle autorizzazioni vengono visualizzate tutte le autorizzazioni concesse in precedenza alla connessione dell’utente, oltre alle nuove autorizzazioni necessarie per l’applicazione corrente.
>
>Ad esempio, se un utente dispone delle autorizzazioni &quot;Leggi tabella&quot; concesse tramite il connettore Excel e quindi crea una connessione nel connettore Outlook per leggere le e-mail, nella schermata di consenso delle autorizzazioni verranno visualizzate sia l’autorizzazione &quot;Leggi tabella&quot; già concessa che l’autorizzazione &quot;Scrivi e-mail&quot; appena richiesta.

1. In qualsiasi modulo [!DNL Microsoft Dynamics 365], fai clic su **[!UICONTROL Aggiungi]** accanto al campo [!UICONTROL Connessione].
1. Immettere un nome per la connessione.
1. Nel campo **[!UICONTROL Risorsa]** immettere l&#39;indirizzo dell&#39;account [!DNL Dynamics 365], senza `https://`.
1. Fai clic su **[!UICONTROL Continua]** per creare la connessione e tornare al modulo.

>[!NOTE]
>
>Durante la registrazione di [!DNL Workfront Fusion] nel portale [!DNL Microsoft Azure], utilizza il seguente URI di reindirizzamento:
>
>* `https://app.workfrontfusion.com/oauth/cb/workfront-microsoft-dynamics2`


## [!DNL Microsoft Dynamics 365] moduli e relativi campi

Quando configuri [!DNL Microsoft Dynamics 365] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Insieme a questi, potrebbero essere visualizzati ulteriori campi di [!DNL Microsoft Dynamics 365], a seconda di fattori quali il livello di accesso nell&#39;app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se viene visualizzato il pulsante Mappa sopra un campo o una funzione, è possibile utilizzarlo per impostare variabili e funzioni per tale campo. Per ulteriori informazioni, vedere [Mappare le informazioni da un modulo all&#39;altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [[!UICONTROL Osserva record (pianificati)]](#watch-records-scheduled)
* [[!UICONTROL Osserva record (tempo reale)]](#watch-records-real-time)
* [[!UICONTROL Crea record]](#create-record)
* [[!UICONTROL Effettuare una chiamata API]](#make-an-api-call)
* [[!UICONTROL Elimina record]](#delete-record)
* [[!UICONTROL Leggi record]](#read-records)
* [[!UICONTROL Aggiorna record]](#update-record)
* [[!UICONTROL Cerca record]](#search-records)

### [!UICONTROL Osserva record (pianificati)]

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
  <td> <p>Per istruzioni sulla connessione dell'account [!DNL Microsoft Dynamics 365] a [!DNL Workfront Fusion], vedere <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connessione di [!DNL Microsoft Dynamics 365] a [!DNL Workfront Fusion]</a> in questo articolo. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Include]</td> 
   <td>Specificare se si desidera che il modulo controlli <strong>[!UICONTROL Solo nuovi record]</strong>, <strong>[!UICONTROL Solo record aggiornati]</strong> o <strong>[!UICONTROL Nuovi record e tutte le modifiche]</strong>.</td> 
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

### [!UICONTROL Osserva record (tempo reale)]

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
     <li value="1"> <p>Fai clic su <strong>[!UICONTROL Add]</strong> a destra del campo Webhook</p> </li> 
     <li value="2"> <p>Nel campo del nome <strong>[!UICONTROL Webhook]</strong> digitare un nome descrittivo per il webhook.</p> </li> 
     <li value="3"> <p>Nel campo <strong>[!UICONTROL Connection]</strong>, selezionare la connessione che si desidera utilizzare selezionata</p> <p>Per istruzioni sulla connessione dell'account [!DNL Microsoft Dynamics 365] a [!DNL Workfront Fusion], vedere <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connessione di [!DNL Microsoft Dynamics 365] a [!DNL Workfront Fusion]</a> in questo articolo. </p> </li> 
     <li value="4"> <p>Fai clic su <strong>[!UICONTROL Salva]</strong> per salvare il webhook e tornare al modulo.</p> </li> 
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
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Microsoft Dynamics 365] a [!DNL Workfront Fusion], vedere <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connessione di [!DNL Microsoft Dynamics 365] a [!DNL Workfront Fusion]</a> in questo articolo. </p> </td> 
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

Questo modulo di azione consente di effettuare una chiamata autenticata personalizzata all&#39;API [!DNL Microsoft Dynamics 365]. In questo modo è possibile creare un&#39;automazione del flusso di dati che non può essere eseguita dagli altri moduli [!DNL Microsoft Dynamics 365].

Il modulo restituisce informazioni sul codice di stato, le intestazioni e il corpo. Puoi mappare queste informazioni nei moduli successivi nello scenario.

Per ulteriori informazioni, vedere la documentazione di [!DNL Microsoft] sull&#39;utilizzo di [!DNL Dynamics 365 Customer Engagement Web API].

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Per istruzioni sulla connessione dell'account [!DNL Microsoft Dynamics 365] a [!DNL Workfront Fusion], vedere <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connessione di [!DNL Microsoft Dynamics 365] a [!DNL Workfront Fusion]</a> in questo articolo. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> <p>Immettere un percorso relativo a <code>&lt;Instance URL>/api/data/v9.1/</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, vedere <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> <p>Per ulteriori informazioni in</p> </td> 
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
   <td> <p>Aggiungi il contenuto body per la chiamata API sotto forma di oggetto JSON standard.</p> <p>Nota:  <p>Quando si utilizzano istruzioni condizionali come <code>if</code> nel JSON, inserire le virgolette al di fuori dell'istruzione condizionale.</p> 
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
  <td> <p>Per istruzioni sulla connessione dell'account [!DNL Microsoft Dynamics 365] a [!DNL Workfront Fusion], vedere <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connessione di [!DNL Microsoft Dynamics 365] a [!DNL Workfront Fusion]</a> in questo articolo. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di entità]</td> 
   <td> <p>Selezionare il tipo di entità che si desidera eliminare dal modulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td> <p>Immettere o mappare l'ID [!DNL Microsoft Dynamics 365] univoco del record che si desidera eliminare dal modulo.</p> </td> 
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
  <td> <p>Per istruzioni sulla connessione dell'account [!DNL Microsoft Dynamics 365] a [!DNL Workfront Fusion], vedere <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connessione di [!DNL Microsoft Dynamics 365] a [!DNL Workfront Fusion]</a> in questo articolo. </p> </td> 
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
   <td>Immettere o mappare l'ID [!DNL Microsoft Dynamics 365] univoco del record che si desidera venga letto dal modulo.</td> 
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
  <td> <p>Per istruzioni sulla connessione dell'account [!DNL Microsoft Dynamics 365] a [!DNL Workfront Fusion], vedere <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connessione di [!DNL Microsoft Dynamics 365] a [!DNL Workfront Fusion]</a> in questo articolo. </p> </td> 
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
   <td>Immettere o mappare l'ID [!DNL Microsoft Dynamics] 365 univoco del record che si desidera aggiornare nel modulo.</td> 
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
  <td> <p>Per istruzioni sulla connessione dell'account [!DNL Microsoft Dynamics 365] a [!DNL Workfront Fusion], vedere <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connessione di [!DNL Microsoft Dynamics 365] a [!DNL Workfront Fusion]</a> in questo articolo. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di entità]</td> 
   <td>Selezionare il tipo di entità che si desidera aggiornare nel modulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filters]</td> 
   <td> <p>Selezionare il filtro che si desidera utilizzare per la ricerca.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Filtri Standard]</strong> </p> <p>Imposta il filtro selezionando un campo e un operatore e immettendo o mappando il valore che desideri cercare. Puoi utilizzare le regole AND o OR per il filtro.</p> </li> 
     <li> <p><strong>[!UICONTROL Funzioni query]</strong> </p> <p>Immettere la funzione di query API Web [!DNL Dynamics 365] che si desidera utilizzare per la ricerca. </p> <p>Per ulteriori informazioni sulle funzioni di query, vedere <a href="https://docs.microsoft.com/en-us/dynamics365/customer-engagement/web-api/queryfunctions?view=dynamics-ce-odata-9">Riferimento funzione query API Web</a> nella documentazione di [!DNL Microsoft].</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sort]</td> 
   <td> <p>Specificare l'ordine di restituzione degli elementi. È possibile aggiungere più ordinamenti.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Campo]</strong> </p> <p>Specificare il campo in base al quale ordinare i risultati.</p> </li> 
     <li> <p><strong>[!UICONTROL Direzione]</strong> </p> <p>Specifica la direzione dell’ordinamento (crescente o decrescente).</p> </li> 
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
