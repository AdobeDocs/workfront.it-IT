---
filename: microsoft-word-templates-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli modello di Microsoft Word
description: In uno scenario Adobe Workfront Fusion, è possibile automatizzare i flussi di lavoro che utilizzano i modelli di Microsoft Word, nonché collegarli a più applicazioni e servizi di terze parti.
author: Becky
source-git-commit: 43b64d1371438909063d2ac81cccb90b97179dfc
workflow-type: tm+mt
source-wordcount: '1286'
ht-degree: 0%

---


# [!DNL Microsoft Word Template] moduli

In un [!DNL Adobe Workfront Fusion] puoi automatizzare i flussi di lavoro che utilizzano [!DNL Microsoft Word Templates], nonché collegarlo a più applicazioni e servizi di terze parti.

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
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Access level configurations*</td> 
    <td> 
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a Workfront Fusion administrator for your organization.</p>
     --> <!--
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a Workfront Fusion administrator for your team.</p>
     --> </td> 
   </tr>
 </tbody> 
</table>

Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, vedi [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Prerequisiti

Per utilizzare [!DNL Miscrosoft Word Templates] con [!DNL Adobe Workfront Fusion], è necessario disporre di un [!DNL Office 365] conto. Puoi crearne uno all’indirizzo www.office.com.

## Utilizzo [!DNL Microsoft Word Templates] moduli

Puoi utilizzare un [!DNL Microsoft Word Template] modulo per unire dati da più servizi Web in un [!DNL Microsoft Word] documento.

Ad esempio, puoi utilizzare [!DNL Microsoft Word] modello:

![](assets/word-template-before-filled-350x62.png)

Per creare questo documento:

![](assets/word-template-exampled-filled-350x85.png)

## Informazioni sui tag valore

A [!DNL Microsoft Word] modello è regolare [!DNL Microsoft Word] documento (file .docx) con tag speciali nel relativo testo che determinano dove e come unire o compilare i dati. Esistono tre tipi di tag:

* [Tag di valore semplice](#simple-value-tag)
* [Tag condizione](#condition-tag)
* [Tag loop](#loop-tag)

### Tag di valore semplice {#simple-value-tag}

Un tag valore semplice viene semplicemente sostituito con un valore corrispondente. Il nome del tag corrisponde al [!UICONTROL Chiave] il valore del campo, posto all&#39;interno di doppie parentesi graffe; ad esempio,


<pre>{{name}}</pre>


.

**Esempio:** Per creare un documento che dice &quot;Ciao Petr!&quot;, potresti usare un [!DNL Microsoft Word Template] modulo per creare il seguente modello:

<pre>&gt; Ciao {{name}}!</pre>

A questo scopo, imposterai il modulo come segue:

![](assets/word-template-simple-value-350x286.png)

### Tag condizione {#condition-tag}

È possibile utilizzare un tag di condizione per racchiudere il testo di cui è necessario eseguire il rendering solo quando sono soddisfatte determinate condizioni. Per racchiudere il testo, posizionarlo tra i tag di condizione di apertura e chiusura, ad esempio &quot;hasPhone&quot;, se la condizione è se i dati includono o meno un numero di telefono. Il nome di un tag di apertura viene preceduto dal simbolo cancelletto #, il nome di un tag di chiusura viene preceduto da una barra /, come mostrato nell’esempio seguente.

**Esempio:** Per produrre un documento che include il numero di telefono di un cliente se i dati di input includono un numero di telefono, ma nessun indirizzo e-mail, è possibile utilizzare un [!DNL Microsoft Word Template] e crea il seguente modello:
<pre>&gt; {{#hasPhone}}Telefono: {{phone}} {{/hasPhone}}</pre><pre>&gt; {{#hasEmail}}Email: {{email}} {{/hasEmail}}</pre>A questo scopo, imposterai il modulo come segue:

![](assets/word-template-conditional-350x501.png)

Nel documento, il numero di telefono appare come segue:
<pre>&gt; Telefono: 4445551234</pre>

### Tag loop {#loop-tag}

È possibile utilizzare un tag di ciclo, noto anche come tag di sezione, per ripetere una sezione di testo. Racchiudi il testo posizionandolo tra i tag di ciclo di apertura e chiusura. Il nome di un tag di apertura è preceduto dal simbolo cancelletto #; il nome di un tag di chiusura viene preceduto da una barra /.

* [Tag Loop con Compilare un modulo di documento](#loop-tag-with-fill-out-a-document-module)

<!-- [Loop tag with Fill a document with a batch of data module](#loop-tag-with-fill-a-document-with-a-batch-of-data-module)-->

#### Tag Loop con Compilare un modulo di documento {#loop-tag-with-fill-out-a-document-module}

**Esempio:** Per produrre un documento in cui siano elencati il nome e il numero di telefono di ogni contatto in un elenco di clienti, è possibile utilizzare un [!DNL Microsoft Word Template] e crea il seguente modello:

<pre>&gt; {{#contact}}</pre><pre>&gt; {{name}}, {{phone}}</pre><pre>&gt; {{/contact}}</pre>

A questo scopo, imposterai il modulo come segue:


![](assets/word-template-fill-out-a-document-350x732.png)

Il modulo creerà il seguente documento:

```
> Jan Toman, 4445551234
> Eduard Salo, 4445552345
```

<!--

#### Loop tag with Fill a document with a batch of data module {#loop-tag-with-fill-a-document-with-a-batch-of-data-module}

**Example:** You can export Google contacts into a table that you create using loop tags.

The first module loads the template. The next module retrieves all contacts from the group you specify in [!DNL Google Contacts]. The aggregator module aggregates all values retrieved from Google Contacts and merges them into the template. And the last module saves the filled template to the desired location.

![](assets/word-template-batch-scenario-350x124.png)

You could use this scenario with the following template:

![](assets/word-template-batch-template-350x26.png)

To do this, you would set up the module as follows:

![](assets/word-template-batch-module-setup-350x323.png)

The module would create the following document:

![](assets/word-template-batch-document-350x46.png)
-->

## [!DNL Microsoft Word Template] moduli

Questi moduli non richiedono una connessione.

* [Compilare un documento](#fill-out-a-document)
* [Compilare un documento con un batch di dati](#fill-a-document-with-a-batch-of-data)

### [!UICONTROL Compilare un documento] {#fill-out-a-document}

Questo modulo di trasformazione consente di compilare un documento con i dati specificati. Può essere utilizzato con valori semplici tag, tag condizionali o tag loop.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Carattere di delimitazione iniziale del testo da sostituire]</td> 
   <td> <p>Immettere i caratteri che si desidera contrassegnare come inizio il testo da sostituire. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span>Invio <code>[[</code> se si desidera sostituire un testo simile a questo: <code>[[replace_me]]</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Fine delimitatore del testo da sostituire]</p> </td> 
   <td> <p>Immettere i caratteri che si desidera contrassegnare come fine del testo da sostituire. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span>Invio <code>]]</code> se si desidera sostituire un testo simile a questo: <code>[[replace_me]]</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File di origine]</td> 
   <td> <p> Mappa il file da caricare dal modulo precedente (ad esempio, HTTP &gt; Ottieni un file o un Dropbox &gt; Ottieni un modulo file). Oppure inserisci manualmente il file di dati.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome del file compilato]</td> 
   <td>Immetti un nome file (inclusa l’estensione) per il file di output di destinazione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Origine dati]</td> 
   <td> <p>Selezionare un'opzione per indicare se i dati utilizzati provengono da un modulo o da una raccolta dati non elaborati (dati di computer non elaborati).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Values]</td> 
   <td> <p>Deve essere una matrice di raccolte, dove:</p> 
    <ul> 
     <li>Ogni raccolta corrisponde a una voce di dati e contiene un elemento <code>entry</code></li> 
     <li>Elemento <code>entry </code>contiene una raccolta di <code>key </code>e <code>value</code></li> 
     <li>Elemento <code>key </code>contiene il nome del tag</li> 
     <li>item <code>value </code>contiene il valore del tag</li> 
    </ul> 
    <p>Per aggiungere una voce:</p>
    <ol> 
     <li> Fai clic su <b>[!UICONTROL Aggiungi elemento]</b>. </li> 
     <li>Selezionare il tipo di valore della voce.</li> 
     <li>Aggiungi nome e valore. Per ulteriori informazioni, consulta l’esempio per il tipo di valore scelto in questo articolo. 
      <ul> 
       <li><a href="#simple-value-tag" class="MCXref xref">Tag di valore semplice</a></li> 
       <li><a href="#condition-tag" class="MCXref xref">Tag condizione</a></li> 
       <li><a href="#loop-tag" class="MCXref xref">Tag loop</a></li> 
      </ul></li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Compilare un documento con un batch di dati] {#fill-a-document-with-a-batch-of-data}

Questo modulo aggregatore è utile se le voci di dati vengono come bundle separati. Con questo modulo, puoi facilmente impostare la struttura richiesta per il campo Valore e mappare gli elementi a ogni elemento valore. A differenza del modulo Compilare un documento, il campo Valori nel Compila un documento con un batch di moduli dati consente solo una singola voce contenente variabili.

È inoltre possibile utilizzare questo modulo anche se le voci di dati sono come una matrice, utilizzando *Iteratore* modulo per trasformare il contenuto dell’array in una serie di bundle.

I valori effettivi vengono creati e compilati per ogni bundle in entrata. Il modello viene prodotto dopo l’elaborazione di tutti i bundle di input.

Questo modulo aggregatore è particolarmente utile per la creazione di elenchi o rapporti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Module]</td> 
   <td>Selezionare il modulo che rappresenta l'origine del testo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Carattere di delimitazione iniziale del testo da sostituire]</td> 
   <td> <p>Immettere i caratteri che si desidera contrassegnare come inizio il testo da sostituire. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span>Invio <code>[[</code> se si desidera sostituire un testo simile a questo: <code>[[replace_me]]</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Fine delimitatore del testo da sostituire]</p> </td> 
   <td> <p>Immettere i caratteri che si desidera contrassegnare come fine del testo da sostituire. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span>Invio <code>]]</code> se si desidera sostituire un testo simile a questo: <code>[[replace_me]]</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Group by]</td> 
   <td> Definisci un'espressione contenente uno o più elementi mappati. I dati aggregati sono separati in Gruppi con lo stesso valore dell'espressione. Ogni gruppo produce come bundle separato contenente una Chiave con l'espressione valutata e il testo aggregato. In questo modo, puoi utilizzare la Chiave come filtro nei moduli successivi.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Interrompe l'elaborazione dopo un'aggregazione vuota]</td> 
   <td>Abilita questa opzione per interrompere l’elaborazione quando un’aggregazione non contiene bundle.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File di origine]</td> 
   <td> <p> Mappa il file da caricare dal modulo precedente (ad esempio, HTTP &gt; Ottieni un file o un Dropbox &gt; Ottieni un modulo file). Oppure inserisci manualmente il file di dati.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome del file compilato]</td> 
   <td>Immetti un nome file (inclusa l’estensione) per il file di output di destinazione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Origine dati]</td> 
   <td> <p>Selezionare un'opzione per indicare se i dati utilizzati provengono da un modulo o da una raccolta dati non elaborati (dati di computer non elaborati).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Values]</td> 
   <td> <p>Deve essere una matrice di raccolte, dove:</p> 
    <ul> 
     <li>Ogni raccolta corrisponde a una voce di dati e contiene un elemento <code>entry</code></li> 
     <li>Elemento <code>entry </code>contiene una raccolta di <code>key </code>e <code>value</code></li> 
     <li>Elemento <code>key </code>contiene il nome del tag</li> 
     <li>item <code>value </code>contiene il valore del tag</li> 
    </ul> 
    <p>Per aggiungere una voce:</p>
    <ol> 
     <li> Fai clic su <b>[!UICONTROL Aggiungi elemento]</b>. </li> 
     <li>Selezionare il tipo di valore della voce.</li> 
     <li>Aggiungi nome e valore. Per ulteriori informazioni, consulta l’esempio per il tipo di valore scelto in questo articolo. 
      <ul> 
       <li><a href="#simple-value-tag" class="MCXref xref">Tag di valore semplice</a></li> 
       <li><a href="#condition-tag" class="MCXref xref">Tag condizione</a></li> 
       <li><a href="#loop-tag" class="MCXref xref">Tag loop</a></li> 
      </ul></li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

