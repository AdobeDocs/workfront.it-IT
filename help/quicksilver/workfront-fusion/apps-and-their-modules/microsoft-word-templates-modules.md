---
filename: microsoft-word-templates-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli modello di Microsoft Word
description: In uno scenario Adobe Workfront Fusion, è possibile automatizzare i flussi di lavoro che utilizzano modelli di Microsoft Word e collegarli a più applicazioni e servizi di terze parti.
author: Becky
feature: Workfront Fusion
exl-id: 889b417c-04a9-4dbf-9a34-0dab65f11f03
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '1286'
ht-degree: 0%

---

# [!DNL Microsoft Word Template] moduli

In un [!DNL Adobe Workfront Fusion] scenario, puoi automatizzare i flussi di lavoro che utilizzano [!DNL Microsoft Word Templates], oltre a collegarlo a più applicazioni e servizi di terze parti.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] per l'automazione e l'integrazione del lavoro] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare la funzionalità descritta in questo articolo.</td> 
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

Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, consulta [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Prerequisiti

Per utilizzare [!DNL Miscrosoft Word Templates] con [!DNL Adobe Workfront Fusion], è necessario disporre di un [!DNL Office 365] account. Puoi crearne uno all’indirizzo www.office.com.

## Utilizzo di [!DNL Microsoft Word Templates] moduli

È possibile utilizzare una [!DNL Microsoft Word Template] modulo per unire dati provenienti da più servizi web in un [!DNL Microsoft Word] documento.

Ad esempio, puoi utilizzare questo [!DNL Microsoft Word] modello:

![](assets/word-template-before-filled-350x62.png)

Per creare questo documento:

![](assets/word-template-exampled-filled-350x85.png)

## Informazioni sui tag dei valori

A [!DNL Microsoft Word] il modello è un normale [!DNL Microsoft Word] documento (file .docx) con tag speciali nel testo che determinano dove e come unire o compilare i dati. Esistono tre tipi di tag:

* [Tag valore semplice](#simple-value-tag)
* [Tag condizione](#condition-tag)
* [Tag loop](#loop-tag)

### Tag valore semplice {#simple-value-tag}

Un tag di valore semplice viene semplicemente sostituito con un valore corrispondente. Il nome del tag corrisponde a [!UICONTROL Chiave] il valore del campo, che viene posizionato all&#39;interno di doppie parentesi graffe; ad esempio,


<pre>&#123;&#123;name&#125;&#125;</pre>


.

**Esempio:** Per creare un documento con la dicitura &quot;Ciao, Petr!&quot;, puoi utilizzare un’ [!DNL Microsoft Word Template] per creare il seguente modello:

<pre>&gt; Ciao &#123;&#123;name&#125;&#125;!</pre>

A questo scopo, imposta il modulo come segue:

![](assets/word-template-simple-value-350x286.png)

### Tag condizione {#condition-tag}

È possibile utilizzare un tag condizione per racchiudere il testo di cui eseguire il rendering solo quando vengono soddisfatte determinate condizioni. Per racchiudere il testo, posizionalo tra i tag della condizione di apertura e chiusura, ad esempio &quot;hasPhone&quot; se la condizione è se i dati includono o meno un numero di telefono. Il nome di un tag di apertura è preceduto da un hash sign #, il nome di un tag di chiusura è preceduto da una barra /, come mostrato nell&#39;esempio seguente.

**Esempio:** Per produrre un documento che includa il numero di telefono di un cliente se i dati di input includono un numero di telefono, ma nessun indirizzo e-mail, puoi utilizzare un [!DNL Microsoft Word Template] e creare il seguente modello:
<pre>&gt; &#123;&#123;#hasPhone&#125;&#125;Telefono: &#123;&#123;phone&#125;&#125; &#123;&#123;/hasPhone&#125;&#125;</pre><pre>&gt; &#123;&#123;#hasEmail&#125;&#125;E-mail: &#123;&#123;email&#125;&#125; &#123;&#123;/hasEmail&#125;&#125;</pre>A questo scopo, imposta il modulo come segue:

![](assets/word-template-conditional-350x501.png)

Nel documento, il numero di telefono apparirà come segue:
<pre>&gt; Telefono: 4445551234</pre>

### Tag loop {#loop-tag}

Per ripetere una sezione di testo, è possibile utilizzare un tag loop, noto anche come tag di sezione. Racchiudi il testo posizionandolo tra i tag loop di apertura e chiusura. Il nome di un tag di apertura è preceduto da un hash sign #; il nome di un tag di chiusura è preceduto da una barra /.

* [Collega tag con Compila un modulo documento](#loop-tag-with-fill-out-a-document-module)
  <!-- [Loop tag with Fill a document with a batch of data module](#loop-tag-with-fill-a-document-with-a-batch-of-data-module)-->

#### Collega tag con Compila un modulo documento {#loop-tag-with-fill-out-a-document-module}

**Esempio:** Per produrre un documento in cui sono elencati il nome e il numero di telefono di ogni contatto in un elenco clienti, è possibile utilizzare una [!DNL Microsoft Word Template] e creare il seguente modello:

<pre>&gt; &#123;&#123;#contact&#125;&#125;</pre><pre>&gt;     &#123;&#123;name&#125;&#125;, &#123;&#123;phone&#125;&#125;</pre><pre>&gt; &#123;&#123;/contact&#125;&#125;</pre>

A questo scopo, imposta il modulo come segue:


![](assets/word-template-fill-out-a-document-350x732.png)

Il modulo crea il seguente documento:

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
* [Riempire un documento con un batch di dati](#fill-a-document-with-a-batch-of-data)

### [!UICONTROL Compilare un documento] {#fill-out-a-document}

Questo modulo di trasformazione consente di riempire un documento con i dati specificati. Può essere utilizzato con tag di valori semplici, tag condizionali o tag di loop.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Delimitatore iniziale del testo da sostituire]</td> 
   <td> <p>Immettere il carattere o i caratteri che si desidera contrassegnare come inizio del testo da sostituire. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span>Invio <code>[[</code> se si desidera sostituire un testo simile al seguente: <code>[[replace_me]]</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Delimitatore finale del testo da sostituire]</p> </td> 
   <td> <p>Immettere il carattere o i caratteri che si desidera contrassegnare come fine del testo da sostituire. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span>Invio <code>]]</code> se si desidera sostituire un testo simile al seguente: <code>[[replace_me]]</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File di origine]</td> 
   <td> <p> Mappa il file che desideri caricare dal modulo precedente (ad esempio, HTTP &gt; Ottieni un file o un Dropbox &gt; Ottieni un modulo file). In alternativa, immettere manualmente il file di dati.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome del file compilato]</td> 
   <td>Immettere un nome di file (con estensione) per il file di output di destinazione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Origine dati]</td> 
   <td> <p>Selezionare un'opzione per indicare se i dati utilizzati provengono da un modulo o da una raccolta di dati non elaborati (dati non elaborati del computer).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Values]</td> 
   <td> <p>Deve essere un array di raccolte, in cui:</p> 
    <ul> 
     <li>Ogni raccolta corrisponde a una voce di dati e contiene un elemento <code>entry</code></li> 
     <li>Elemento <code>entry </code>contiene una raccolta di <code>key </code>e <code>value</code></li> 
     <li>Elemento <code>key </code>contiene il nome del tag</li> 
     <li>elemento <code>value </code>contiene il valore del tag</li> 
    </ul> 
    <p>Per aggiungere una voce:</p>
    <ol> 
     <li> Clic <b>[!UICONTROL Add Item]</b>. </li> 
     <li>Selezionare il tipo di valore della voce.</li> 
     <li>Aggiungi nome e valore. Per ulteriori informazioni, consulta l’esempio per il tipo di valore scelto in questo articolo. 
      <ul> 
       <li><a href="#simple-value-tag" class="MCXref xref">Tag valore semplice</a></li> 
       <li><a href="#condition-tag" class="MCXref xref">Tag condizione</a></li> 
       <li><a href="#loop-tag" class="MCXref xref">Tag loop</a></li> 
      </ul></li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Riempire un documento con un batch di dati] {#fill-a-document-with-a-batch-of-data}

Questo modulo di aggregazione è utile se i dati inseriti vengono forniti come bundle separati. Con questo modulo, puoi facilmente impostare la struttura richiesta per il campo Valore e mappare gli elementi a ciascun elemento di valore. A differenza del modulo Compila un documento, il campo Valori del modulo Compila un documento con un batch di dati consente una sola voce contenente variabili.

Puoi anche utilizzare questo modulo se le voci di dati vengono fornite come array, utilizzando *Iteratore* per trasformare il contenuto dell’array in una serie di bundle.

I valori effettivi vengono creati e compilati per ogni bundle in ingresso. Il modello viene prodotto dopo l’elaborazione di tutti i bundle di input.

Questo modulo di aggregazione è particolarmente utile per la creazione di elenchi o rapporti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Module]</td> 
   <td>Selezionare il modulo che costituisce l'origine del testo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Delimitatore iniziale del testo da sostituire]</td> 
   <td> <p>Immettere il carattere o i caratteri che si desidera contrassegnare come inizio del testo da sostituire. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span>Invio <code>[[</code> se si desidera sostituire un testo simile al seguente: <code>[[replace_me]]</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Delimitatore finale del testo da sostituire]</p> </td> 
   <td> <p>Immettere il carattere o i caratteri che si desidera contrassegnare come fine del testo da sostituire. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span>Invio <code>]]</code> se si desidera sostituire un testo simile al seguente: <code>[[replace_me]]</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Raggruppa per]</td> 
   <td> Definisci un’espressione contenente uno o più elementi mappati. I dati aggregati vengono separati in Gruppi con il valore della stessa espressione. Ogni gruppo restituisce come bundle separato contenente una Chiave con l’espressione valutata e il testo aggregato. In questo modo, puoi utilizzare la Chiave come filtro nei moduli successivi.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Interrompi elaborazione dopo un'aggregazione vuota]</td> 
   <td>Abilita questa opzione per interrompere l’elaborazione quando un’aggregazione non contiene bundle.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File di origine]</td> 
   <td> <p> Mappa il file che desideri caricare dal modulo precedente (ad esempio, HTTP &gt; Ottieni un file o un Dropbox &gt; Ottieni un modulo file). In alternativa, immettere manualmente il file di dati.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome del file compilato]</td> 
   <td>Immettere un nome di file (con estensione) per il file di output di destinazione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Origine dati]</td> 
   <td> <p>Selezionare un'opzione per indicare se i dati utilizzati provengono da un modulo o da una raccolta di dati non elaborati (dati non elaborati del computer).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Values]</td> 
   <td> <p>Deve essere un array di raccolte, in cui:</p> 
    <ul> 
     <li>Ogni raccolta corrisponde a una voce di dati e contiene un elemento <code>entry</code></li> 
     <li>Elemento <code>entry </code>contiene una raccolta di <code>key </code>e <code>value</code></li> 
     <li>Elemento <code>key </code>contiene il nome del tag</li> 
     <li>elemento <code>value </code>contiene il valore del tag</li> 
    </ul> 
    <p>Per aggiungere una voce:</p>
    <ol> 
     <li> Clic <b>[!UICONTROL Add Item]</b>. </li> 
     <li>Selezionare il tipo di valore della voce.</li> 
     <li>Aggiungi nome e valore. Per ulteriori informazioni, consulta l’esempio per il tipo di valore scelto in questo articolo. 
      <ul> 
       <li><a href="#simple-value-tag" class="MCXref xref">Tag valore semplice</a></li> 
       <li><a href="#condition-tag" class="MCXref xref">Tag condizione</a></li> 
       <li><a href="#loop-tag" class="MCXref xref">Tag loop</a></li> 
      </ul></li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>
