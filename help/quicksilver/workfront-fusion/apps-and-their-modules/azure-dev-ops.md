---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli Azure DevOps
description: In un [!DNL Adobe Workfront Fusion] puoi automatizzare i flussi di lavoro che utilizzano [!DNL Azure DevOps], nonché collegarlo a più applicazioni e servizi di terze parti.
author: Becky
feature: Workfront Fusion
exl-id: ecaa93c9-47bb-4fe1-87b4-d2e117cc68ae
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1749'
ht-degree: 0%

---

# [!DNL Azure DevOps] moduli

In un [!DNL Adobe Workfront Fusion] puoi automatizzare i flussi di lavoro che utilizzano [!DNL Azure DevOps], nonché collegarlo a più applicazioni e servizi di terze parti.

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

Per utilizzare [!DNL Azure DevOps] moduli, è necessario disporre di un [!DNL Azure] Account DevOps.

## Connetti [!DNL Azure DevOps] a [!DNL Workfront Fusion] {#connect-azure-devops-to-workfront-fusion}

1. Aggiungi un [!DNL Azure DevOps] al tuo scenario.
1. Fai clic su **[!UICONTROL Aggiungi]** accanto al [!UICONTROL Connessione] campo .
1. In [!UICONTROL Tipo di connessione] campo , seleziona **[!DNL Azure DevOps]**.

   >[!IMPORTANT]
   >
   >La [!UICONTROL [!DNL Azure DevOps] (Richiedi tutti gli ambiti)] il tipo di connessione diventerà obsoleto in un prossimo futuro. Pertanto, si sconsiglia di utilizzarlo.

1. Compila i campi seguenti:

   <table style="table-layout:auto">
        <tr>
            <td>[!UICONTROL Nome connessione]</td>
            <td>Immettere un nome per la connessione che si sta creando.</td>
        </tr>
      <tr>
            <td>[!UICONTROL Organization]</td>
            <td>Immetti il nome dell'organizzazione in cui hai creato il tuo [!DNL Azure DevOps] applicazione.</td>
        </tr>
    </table>

1. Fai clic su **[!UICONTROL Continua]** per completare la configurazione della connessione e continuare a creare lo scenario.

## [!UICONTROL DevOps di Azure] moduli e relativi campi

Quando si configura [!DNL Azure DevOps] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL Azure DevOps] potrebbero essere visualizzati, a seconda di fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se trovi il pulsante mappa sopra un campo o una funzione, puoi utilizzarlo per impostare variabili e funzioni per quel campo. Per ulteriori informazioni, consulta [Mappare informazioni da un modulo a un altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Azioni](#actions)
* [Ricerche](#searches)

### Triggers

#### [!UICONTROL Controlla gli elementi di lavoro]

Questo modulo di attivazione immediata esegue uno scenario in cui un record viene aggiunto, aggiornato o eliminato in [!UICONTROL DevOps di Azure].

Il modulo restituisce tutti i campi standard associati al record, insieme a eventuali campi e valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>Selezionare o aggiungere un webhook per il modulo.</p> <p>Per ulteriori informazioni sui webhook nei moduli trigger, vedi <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">Trigger istantanei (webhook) in [!DNL Adobe Workfront Fusion]</a>.</p> <p>Per informazioni su come creare un webhook, vedi <a href="../../workfront-fusion/apps-and-their-modules/webhooks-updated.md" class="MCXref xref">Webhook</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Azioni

* [Chiamata API personalizzata](#custom-api-call)
* [Lettura record](#read-record)
* [Creare un record](#create-a-record)
* [Aggiornare un elemento di lavoro](#update-a-work-item)
* [[!UICONTROL Caricare un allegato]](#upload-an-attachment)
* [Scaricare un allegato](#download-an-attachment)
* [Collegamento di elementi di lavoro]([!UICONTROL #link-work-items])

#### [!UICONTROL Chiamata API personalizzata]

Questo modulo di azione ti consente di effettuare una chiamata autenticata personalizzata al [!DNL Azure DevOps] API. In questo modo, puoi creare un’automazione del flusso di dati che non può essere eseguita dall’altro [!DNL Azure DevOps] moduli.

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Azure DevOps] account a [!DNL Workfront Fusion], vedi <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Azure DevOps] a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL di base]</td> 
   <td> <p>Seleziona o mappa l’URL di base utilizzato per connettersi al [!DNL Azure DevOps] account</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL relativo]</td> 
   <td> <p>Immetti l’URL relativo a cui desideri connetterti per questa chiamata API.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span><code>{organization}/_apis[/{area}]/{resource}</code> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Versione API]</td> 
   <td>Seleziona o mappa la versione del [!DNL Azure DevOps] API a cui desideri connetterti per questa chiamata API. Se non è selezionata alcuna versione, [!DNL Workfront Fusion] si connette a [!DNL Azure DevOps] API versione 5.1.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL, Metodo]</td> 
   <td> <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Aggiungi le intestazioni della richiesta sotto forma di un oggetto JSON standard.</p> <p>Ad esempio: <code>{"Content-type":"application/json"}</code></p> </td> 
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

#### [!UICONTROL Lettura record]

Questo modulo di azione legge i dati da un singolo record in [!DNL Azure DevOps].

Specifica l&#39;ID del record.

Il modulo restituisce l’ID del record e di tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Azure DevOps] account a [!DNL Workfront Fusion], vedi <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Azure DevOps] a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td> <p>Selezionare se si desidera leggere un progetto o un elemento di lavoro</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Project]</strong>: Seleziona il progetto da leggere.</p> </li> 
     <li> <p><strong>[!UICONTROL Elemento di lavoro]</strong>: Selezionare il progetto contenente l'elemento di lavoro che si desidera leggere, quindi selezionare il tipo di elemento di lavoro.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Uscite]</td> 
   <td>Selezionare le informazioni che si desidera includere nel pacchetto di output per questo modulo. I campi disponibili dipendono dal tipo di elemento di lavoro.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Immettere o mappare l'ID del record che si desidera leggere.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Creare un record]

Questo modulo di azione crea un nuovo progetto o elemento di lavoro.

Il modulo genera l’ID oggetto per l’elemento di lavoro appena creato, oppure l’URL e il codice di stato di un progetto appena creato.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Azure DevOps] account a [!DNL Workfront Fusion], vedi <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Azure DevOps] a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td> <p>Selezionare se si desidera creare un elemento di lavoro o un progetto.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Project]</strong> </p> <p>Compila i campi seguenti:</p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Name]</strong>:immetti o mappa un nome per il nuovo progetto.</p> </li> 
       <li> <p><strong>[!UICONTROL Descrizione]</strong>:immetti o mappa una descrizione per il nuovo progetto. </p> </li> 
       <li> <p><strong>[!UICONTROL Visibility]</strong>: Seleziona se desideri che il progetto sia pubblico o privato. Per interagire con un progetto privato, gli utenti devono aver effettuato l’accesso all’organizzazione e devono disporre dell’accesso al progetto. I progetti pubblici sono visibili agli utenti che non hanno effettuato l’accesso alla tua organizzazione.</p> </li> 
       <li> <p><strong>[!UICONTROL Controllo versione]</strong>: Seleziona se desideri utilizzare il progetto [!DNL Git] o [!UICONTROL Team Foundation Version Control (TFCV)] per il controllo delle versioni.</p> </li> 
       <li> <p><strong>[!UICONTROL Processo elemento di lavoro]</strong>: Selezionare il processo di lavoro che si desidera utilizzare per il progetto. Le opzioni sono [!UICONTROL Basic], [!UICONTROL Scrum], [!UICONTROL Capability Maturity Model Integration (CMMI)] e [!UICONTROL Agile].</p> <p>Per ulteriori informazioni su [!DNL Azure DevOps] processi, vedi <a href="https://docs.microsoft.com/en-us/azure/devops/boards/work-items/guidance/choose-process?view=azure-devops&amp;tabs=basic-process">Scegliere un processo</a> in [!DNL Azure DevOps] Documentazione.</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Elemento di lavoro]</strong> </p> <p>Compila i campi seguenti:</p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Project]</strong>: Selezionare il progetto in cui si desidera creare l'elemento di lavoro.</p> </li> 
       <li> <p><strong>[!UICONTROL Tipo di elemento di lavoro]</strong>: Selezionare il tipo di elemento di lavoro che si desidera creare.</p> </li> 
       <li> <p><strong>[!UICONTROL Altri campi]</strong>:In questi campi, immettere il valore che si desidera che l'elemento di lavoro abbia per una determinata proprietà. I campi disponibili dipendono dal tipo di elemento di lavoro.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggiornare un elemento di lavoro]

Questo modulo di azione aggiorna un elemento di lavoro esistente utilizzando il relativo ID.

Il modulo restituisce l&#39;ID dell&#39;elemento di lavoro aggiornato.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Azure DevOps] account a [!DNL Workfront Fusion], vedi <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Azure DevOps] a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project]</td> 
   <td>Selezionare il progetto contenente l'elemento di lavoro che si desidera aggiornare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di elemento di lavoro]</td> 
   <td> <p>Selezionare il tipo di elemento di lavoro che si desidera aggiornare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Altri Campi]</td> 
   <td>In ciascuno di questi campi, immettere il valore che si desidera assegnare all'elemento di lavoro per una determinata proprietà. I campi disponibili dipendono dal tipo di elemento di lavoro.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID elemento di lavoro]</td> 
   <td>Immettere o mappare l'ID dell'elemento di lavoro che si desidera aggiornare.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Caricare un allegato]

Questo modulo di azione carica un file e lo allega a un elemento di lavoro.

Il modulo restituisce l&#39;ID allegato e un URL di download per l&#39;allegato.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Azure DevOps] account a [!DNL Workfront Fusion], vedi <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Azure DevOps] a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project] </td> 
   <td> <p>Seleziona il progetto in cui desideri caricare un allegato.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID elemento di lavoro]</td> 
   <td> <p>Immettere o mappare l'ID dell'elemento di lavoro in cui si desidera caricare un allegato.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Commento]</td> 
   <td>Inserisci il testo di un commento da aggiungere all’allegato caricato.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File di origine] </td> 
   <td>Selezionare un file di origine da un modulo precedente oppure immettere o mappare il nome e il contenuto del file di origine.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Scaricare un allegato]

Questo modulo di azione scarica un allegato.

Il modulo restituisce il contenuto del file dell&#39;allegato.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Azure DevOps] account a [!DNL Workfront Fusion], vedi <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Azure DevOps] a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Allegato URL]</td> 
   <td> <p>Immettere o mappare l'URL dell'allegato che si desidera scaricare.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Collegamento di elementi di lavoro]

Questo modulo di azione collega due elementi di lavoro e definisce la relazione tra di essi.

Il modulo restituisce l’ID dell’elemento di lavoro principale e di tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Azure DevOps] account a [!DNL Workfront Fusion], vedi <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Azure DevOps] a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID elemento di lavoro]</td> 
   <td>Immettere o mappare l'ID dell'elemento di lavoro principale a cui si desidera collegare un altro elemento di lavoro.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID elemento di lavoro collegato]</td> 
   <td>Immettere o mappare l'ID dell'elemento di lavoro che si desidera collegare all'elemento di lavoro principale.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Link Type]</td> 
   <td> <p>Definire la relazione tra gli elementi di lavoro che si desidera collegare.</p> <p>Per ulteriori informazioni, consulta <a href="https://docs.microsoft.com/en-us/azure/devops/boards/queries/link-type-reference?view=azure-devops">Riferimento per il tipo di collegamento</a> nella documentazione [!UICONTROL Azure DevOps].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Commento]</td> 
   <td>Inserisci o mappa il testo di un commento. Questo è utile per spiegare il ragionamento o l'intenzione del collegamento.</td> 
  </tr> 
 </tbody> 
</table>

### Ricerche

#### [!UICONTROL Elencare elementi di lavoro]

Questo modulo di azione recupera tutti gli elementi di lavoro di un tipo specifico in un [!DNL Azure DevOps] progetto.

Il modulo restituisce l’ID dell’elemento di lavoro principale e di tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Azure DevOps] account a [!DNL Workfront Fusion], vedi <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Azure DevOps] a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project]</td> 
   <td>Selezionare il progetto da cui si desidera recuperare gli elementi di lavoro.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di elemento di lavoro]</td> 
   <td> <p>Selezionare il tipo di elemento di lavoro che si desidera recuperare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Uscite]</td> 
   <td>Selezionare le proprietà che si desidera visualizzare nell'output del modulo. I campi disponibili dipendono dal tipo di elemento di lavoro che si desidera recuperare. È necessario selezionare almeno una proprietà.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Immettere o mappare il numero massimo di elementi di lavoro che [!DNL Workfront Fusion] restituisce durante un ciclo di esecuzione.</td> 
  </tr> 
 </tbody> 
</table>
