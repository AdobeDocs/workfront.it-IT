---
content-type: api
navigation-topic: general-api
title: Campi di testo RTF nell’API di Adobe Workfront
description: Campi di testo RTF nell’API di Adobe Workfront
author: John
feature: Workfront API
exl-id: 67fc34dc-0722-4419-8254-0371ad5abfc3
source-git-commit: 40698643b0fa530b38da465f3bc1e4d841fcc190
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 0%

---


# Campi di testo RTF nell’API di Adobe Workfront

Alcuni oggetti in Adobe Workfront consentono l’archiviazione di testo con formattazione RTF. Nell’API Workfront il testo RTF viene memorizzato come JSON utilizzando il framework open source Draft.js.

## Esempio di panoramica

Viene chiamato un campo personalizzato con formattazione RTF **Campo con testo RTF** e può avere i seguenti valori associati:

![](assets/rich-text-example-350x158.png)

**Esempio:** Richiesta di base di GET per recuperare il valore del campo modulo personalizzato **Campo con testo RTF**:

<!-- [Copy](javascript:void(0);) -->
<pre><OBJ Code><OBJ ID><OBJ Code><OBJ ID></pre>

**Esempio:** Questa richiesta restituirà il valore di **Campo con testo RTF** in JSON memorizzato in **parameterValue** **DE:Campo con testo RTF**

<!-- [Copy](javascript:void(0);) -->
<pre></pre>

**Esempio:** Questa è una versione formattata della risposta che compare nella figura direttamente sopra

<!-- [Copy](javascript:void(0);) -->
<pre></pre>

## Blocchi

Gli oggetti JSON che memorizzano il contenuto RTF sono composti da due parti principali: **blocchi** e **entityMaps**.

Un blocco è un oggetto JSON che rappresenta una singola riga di testo formattato. Poiché un singolo campo personalizzato può contenere più di una riga di testo, ogni riga di testo ha un proprio blocco e ogni blocco è rappresentato come un elemento in una matrice principale denominata **blocchi**.

**Esempio:** In questo caso, ogni riga di testo da un campo personalizzato viene mappata su un elemento blocco nei blocchi array

![](assets/copy-of-rich-text-mapping-350x159.png)

Poiché ogni elemento di blocco è anche un oggetto JSON, ogni blocco è composto dagli elementi: **key**, **text**, **type**, **profondità**, **inlineStyleRanges**, **entityRanges** e **dati**. Ognuno di questi elementi funziona come segue:

* **Chiave** è l&#39;identificatore univoco per quel blocco. La chiave viene utilizzata per mappare una riga di testo tramite entityMaps. I dettagli su entityMaps si trovano nella sezione entityMaps di questo documento.
* **Testo** è la riga del contenuto di testo memorizzata dal campo personalizzato.
* **Tipo** descrive il tipo di testo rappresentato. Ad esempio, una riga di testo memorizzata in un blocco potrebbe far parte di un elenco. Se tale riga di testo fa parte di un elenco non ordinato, il relativo tipo viene definito come: unordered-list-item.
* Gli elenchi non sono attualmente supportati, ma dovrebbero essere disponibili a breve.
* **Profondità** Questo parametro definisce la profondità della linea quando la linea è una parte nidificata di un elenco ordinato o non ordinato.
* **inlineStyleRanges** Matrice che descrive i tipi di formattazione applicati alla riga di testo rappresentata dal blocco corrente.

**Esempio:** Ecco un array inlineStyleRanges che descrive ogni stile a livello di carattere. In questo caso: 9 caratteri (lunghezza: 9) a partire dall&#39;indice 0 (offset: 0) aveva lo stile **Grassetto** applicata:

![](assets/copy-of-rich-text-mapping-2-350x136.png)

Nel caso in cui siano stati applicati più tipi di formattazione a una singola riga, gli stili verranno mappati su elementi aggiuntivi nell’array** inlineStyleRanges**.

**Esempio:** Esempio di un blocco quando si memorizza una riga di testo contenente formattazione mista: **Testo in grassetto e corsivo**

<!-- [Copy](javascript:void(0);) -->
<pre></pre>

>[!NOTE]
>
>Tutte le versioni successive alla versione 20.3 supportano le opzioni di formattazione grassetto, corsivo e sottolineato.

## entityMaps e entityRanges

Un blocco di dati può contenere potenzialmente entità quali collegamenti ipertestuali o altri tipi di formattazione stilizzata collegati a origini dati situate al di fuori del campo di testo personalizzato.

## Esempi

### Recupero di testo normale da JSON

Quando viene inviato un campo personalizzato con formattazione RTF, tutto il testo viene memorizzato nell&#39;array **blocchi**. Tuttavia, ogni riga del testo completo viene memorizzata nella **parametro di testo** all&#39;interno di ciascuno degli elementi di blocco separati che compongono l&#39;array principale **blocchi**. Quindi, per recuperare il testo completo, ogni riga di testo separata deve essere estratta e rimessa insieme. A tal fine, è possibile eseguire il ciclo su tutti gli elementi nei blocchi e concatenare insieme ogni parametro di testo con un delimitatore di riga (\n).

**Esempio:** Ecco come potrebbe essere il tuo JS:

<!-- [Copy](javascript:void(0);) -->
<pre></pre>

### Salvataggio di un valore di campo RTF tramite API Workfront

Per salvare i seguenti valori di un campo RTF utilizzando l’API Workfront:
<pre>
		Ciao <strong>World</strong>!
		Questa è la mia prima <strong>Rich Text</strong></pre>

1. Crea JSON che rappresenta il valore del campo RTF che stai tentando di acquisire organizzando ogni riga di testo in un elemento blocco, nell’array **blocchi**

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

1. Acquisire la formattazione RTF utilizzando **inlineStyleRanges** parameter

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

1. Per acquisire la seconda riga, il testo &quot;Rich Text&quot; deve essere formattato in grassetto e corsivo.

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

   >[!NOTE]
   >
   >La funzionalità entityMap non è supportata durante la versione iniziale, ma rimane comunque un campo obbligatorio per il passaggio di questo JSON in una richiesta

1. Utilizza la **stringiare** sul JSON descritto sopra per creare un **PUT** richiedi e invia aggiornamenti

   <!-- [Copy](javascript:void(0);) -->
   <pre><OBJ Code><OBJ ID></pre>
