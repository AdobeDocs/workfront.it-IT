---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli Allocadia
description: In uno scenario  [!DNL Adobe Workfront Fusion] , puoi automatizzare i flussi di lavoro che utilizzano Allocadia e collegarlo a più applicazioni e servizi di terze parti.
author: Becky
feature: Workfront Fusion
exl-id: f1edefd1-9fe0-48fc-bea2-c3f9facf7363
source-git-commit: 2e91e9a4c691430f3c98e3cbddb30706ea57f84a
workflow-type: tm+mt
source-wordcount: '1415'
ht-degree: 0%

---

# [!DNL Allocadia] moduli

In uno scenario [!DNL Adobe Workfront Fusion], è possibile automatizzare i flussi di lavoro che utilizzano [!DNL Allocadia] e collegarlo a più applicazioni e servizi di terze parti.

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
   <p>Fabbisogno prodotto corrente: se si dispone del piano [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront], l'organizzazione deve acquistare [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo. [!DNL Workfront Fusion] è incluso nel piano [!UICONTROL Ultimate] [!DNL Workfront].</p>
   <p>Oppure</p>
   <p>Requisiti del prodotto legacy: la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Per conoscere il piano, il tipo di licenza o l&#39;accesso disponibili, contattare l&#39;amministratore [!DNL Workfront].

Per informazioni sulle [!DNL Adobe Workfront Fusion] licenze, vedere [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Prerequisiti

Per utilizzare i moduli [!DNL Allocadia], è necessario disporre di un account [!DNL Allocadia].

## Informazioni API di [!DNL Allocadia]

Il connettore Allocadia utilizza quanto segue:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Versione API</td> 
   <td> v1 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Tag API</td> 
   <td>v1.7.6</td> 
  </tr>
 </tbody> 
</table>

## Connetti [!DNL Allocadia] a [!DNL Workfront Fusion]

Puoi creare una connessione al tuo account [!DNL Allocadia] direttamente dall&#39;interno di un modulo [!DNL Allocadia].

1. In qualsiasi modulo [!DNL Allocadia], fai clic su **[!UICONTROL Aggiungi]** accanto al campo [!UICONTROL Connessione].
1. Selezionare se si desidera utilizzare il server Nord America o Europa.
1. Immettere il nome utente e la password.
1. Fai clic su **[!UICONTROL Continua]** per creare la connessione e tornare al modulo.

## [!DNL Allocadia] moduli e relativi campi

Quando configuri [!DNL Allocadia] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Insieme a questi, potrebbero essere visualizzati ulteriori campi di [!DNL Allocadia], a seconda di fattori quali il livello di accesso nell&#39;app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se viene visualizzato il pulsante Mappa sopra un campo o una funzione, è possibile utilizzarlo per impostare variabili e funzioni per tale campo. Per ulteriori informazioni, vedere [Mappare le informazioni da un modulo all&#39;altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Azioni](#actions)
* [Ricerche](#searches)

### Triggers

#### [!UICONTROL Osserva record]

Questo modulo trigger esegue uno scenario quando vengono aggiunti, aggiornati o entrambi gli oggetti di un tipo specifico. Il modulo restituisce tutti i campi standard associati al record o ai record, insieme a tutti i campi e i valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> <table style="table-layout:auto"> <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione dell'account Allocadia a [!DNL Workfront Fusion], vedere <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connect Allocadia] to Workfront Fusion</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Filtro</td> 
   <td> <p>Specificare se si desidera che lo scenario controlli Solo nuovi record, Solo [!UICONTROL Record aggiornati] o Record nuovi e aggiornati.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Tipo di entità</td> 
   <td>Selezionare il tipo di record Allocadia da controllare nel modulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Uscite</td> 
   <td> <p>Selezionare i campi da includere nell'output del modulo. I campi disponibili dipendono dal tipo di entità selezionato.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limite</td> 
   <td> <p>Immettere o mappare il numero massimo di record che il modulo deve controllare durante ogni ciclo di esecuzione dello scenario.</p> </td> 
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

Questo modulo di azione consente di effettuare una chiamata autenticata personalizzata all&#39;API [!DNL Allocadia]. In questo modo è possibile creare un&#39;automazione del flusso di dati che non può essere eseguita dagli altri moduli [!DNL Allocadia].

L’azione si basa sul tipo di entità (tipo di oggetto Allocadia) specificato.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Allocadia] a [!DNL Workfront Fusion], vedere <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connessione di [!DNL Allocadia] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Immettere un percorso relativo a <code>https://api-na.allocadia.com/{version}</code> o <code>https://api-eu.allocadia.com/{version}</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, vedere <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
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

#### [!UICONTROL Leggi record]

Questo modulo di azione legge i dati da un singolo record in [!DNL Allocadia].

Specifica l’ID del record.

Il modulo restituisce tutti i campi standard associati al record, insieme a tutti i campi e i valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Allocadia] a [!DNL Workfront Fusion], vedere <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connessione di [!DNL Allocadia] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di entità]</td> 
   <td>Selezionare il tipo di record [!DNL Allocadia] che si desidera venga letto dal modulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output]</td> 
   <td> <p>Selezionare i campi da includere nell'output del modulo. I campi disponibili dipendono dal tipo di entità [!UICONTROL] selezionato.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Immettere o mappare l'ID [!DNL Allocadia] univoco del record che si desidera venga letto dal modulo.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crea record]

Questo modulo di azione crea un record.

Il modulo restituisce l’ID del record ed eventuali campi associati, insieme a eventuali campi e valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Allocadia] a [!DNL Workfront Fusion], vedere <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connessione di [!DNL Allocadia] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di entità]</td> 
   <td>Specificare se si desidera creare un nuovo record in base alla voce di riga o alla scelta della colonna.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Budgets]</td> 
   <td> <p>Selezionare il budget in cui si desidera creare un record.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Column choices]</td> 
   <td>Selezionare la colonna da utilizzare per creare un nuovo record.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Label]</td> 
   <td>Immettere o mappare un'etichetta per il nuovo record</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Elimina record]

Questo modulo di azione elimina un record specifico.

Specifica l’ID del record.

Il modulo restituisce l’ID del record ed eventuali campi associati, insieme a eventuali campi e valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Allocadia] a [!DNL Workfront Fusion], vedere <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connessione di [!DNL Allocadia] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di entità]</td> 
   <td> <p>Selezionate il tipo di entità da eliminare.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL elemento riga]</strong> </p> <p>Inserire l'ID della riga</p> </li> 
     <li> <p><strong>[!UICONTROL Scelta colonna]</strong> </p> <p>Selezionare il budget dal quale si desidera eliminare un record, quindi immettere l'ID colonna e l'ID scelta.</p> </li> 
     <li> <p><strong>[!UICONTROL Tag previsioni]</strong> </p> <p>Selezionare il budget dal quale si desidera eliminare un record, quindi immettere l'ID tag.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggiorna record]

Questo modulo di azione aggiorna un record, ad esempio una voce di riga, un utente o una scelta di colonna.

Specifica l’ID del record.

Il modulo restituisce l’ID del record ed eventuali campi associati, insieme a eventuali campi e valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!UICONTROL Allocadia] a [!DNL Workfront Fusion], vedere <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connettere [!DNL Allocadia] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di entità]</td> 
   <td>Selezionare il tipo di record [!DNL Allocadia] da aggiornare nel modulo. Gli altri campi vengono visualizzati in base al tipo di entità selezionato.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Budgets]</td> 
   <td> <p>Selezionare il budget in cui si desidera aggiornare un record. </p> </td> 
  </tr> 
 </tbody> 
</table>

### Ricerche

#### [!UICONTROL Cerca record]

Questo modulo di ricerca cerca i record in un oggetto in [!DNL Allocadia] che corrispondono alla query di ricerca specificata.

Puoi mappare queste informazioni nei moduli successivi nello scenario.

Specificare il tipo di record desiderato.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Allocadia] a [!DNL Workfront Fusion], vedere <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connessione di [!DNL Allocadia] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di entità]</td> 
   <td>Selezionare il tipo di record [!DNL Allocadia] da cercare nel modulo. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Budgets]</td> 
   <td> <p>Selezionare il budget che si desidera cercare. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Set di risultati]</td> 
   <td>Selezionare se si desidera che il modulo restituisca tutti i record corrispondenti o solo il primo record corrispondente.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conteggio massimo dei record]</td> 
   <td> <p>Immettere o mappare il numero massimo di record che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Criteri di ricerca di [!UICONTROL]</td> 
   <td>Selezionare il campo che si desidera cercare, selezionare l'operazione e immettere o mappare il valore che si desidera cercare. Puoi aggiungere [!DNL AND] o [!DNL OR] regole per filtrare ulteriormente la ricerca.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output]</td> 
   <td> <p>Selezionare i campi da includere nell'output del modulo. I campi disponibili dipendono dal tipo di entità selezionato.</p> </td> 
  </tr> 
 </tbody> 
</table>
