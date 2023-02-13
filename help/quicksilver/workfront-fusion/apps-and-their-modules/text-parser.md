---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
navigation-topic: apps-and-their-modules
title: Analizzatore di testo
description: È possibile utilizzare lo strumento di analisi del testo per analizzare il testo da utilizzare in altri [!DNL Adobe Workfront Fusion] moduli di scenario. Il parser Testo non richiede una connessione.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 7d71cf64-4f86-42c5-81e7-8fc15333cbd7
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1010'
ht-degree: 0%

---

# [!UICONTROL Analizzatore di testo]

È possibile utilizzare [!UICONTROL Strumento di analisi del testo] per analizzare il testo da utilizzare in altri [!DNL Adobe Workfront Fusion] moduli di scenario. La [!UICONTROL Analizzatore di testo] non richiede una connessione.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p> <p>[!UICONTROL [!DNL Workfront Fusion] per automazione del lavoro</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</td> 
  </tr> 
 </tbody> 
</table>

Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, vedi [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL Analizzatore di testo] moduli e relativi campi

Quando si configura [!UICONTROL Analizzatore di testo] moduli, [!DNL Adobe Workfront Fusion] visualizza i campi elencati di seguito. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se trovi il pulsante mappa sopra un campo o una funzione, puoi utilizzarlo per impostare variabili e funzioni per quel campo. Per ulteriori informazioni, consulta [Mappare informazioni da un modulo a un altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Trasformatori

* [[!UICONTROL Ottenere elementi da HTML]](#get-elements-from-html)
* [[!UICONTROL Ottieni elementi dal testo]](#get-elements-from-text)
* [[!UICONTROL HTML al testo]](#html-to-text)
* [[!UICONTROL Pattern di corrispondenza]](#match-pattern)
* [[!UICONTROL Sostituisci]](#replace)

#### [!UICONTROL Ottenere elementi da HTML]

Recupera gli elementi desiderati dal codice HTML.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Continua l’esecuzione del percorso anche se il modulo non trova corrispondenze]</td> 
   <td> <p>Abilita questa opzione per garantire che il modulo non interrompa lo scenario se non restituisce risultati.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo di elemento]</td> 
   <td> <p> Seleziona il tipo di elemento da recuperare dal codice HTML. </p> 
    <ul> 
     <li>[!UICONTROL Immagine]</li> 
     <li>[!UICONTROL Link]</li> 
     <li>[!UICONTROL elemento/iFrame]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL HTML] </td> 
   <td> <p>Immetti o mappa il codice HTML da cui desideri recuperare i tipi di elementi specificati.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottieni elementi dal testo]

Analizza gli elementi dal testo in base al pattern specificato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Testo di input]</td> 
   <td> <p>Immettere o mappare il testo da analizzare.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pattern]</td> 
   <td> <p>Selezionare il pattern che riflette gli elementi che si desidera analizzare dal testo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ignora occorrenze duplicate]</td> 
   <td> <p>Seleziona questa casella per ignorare le occorrenze duplicate di un elemento di testo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL HTML al testo]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL HTML] </td> 
   <td> <p>Immetti il codice HTML da convertire in testo normale.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Interruzione di riga] </td> 
   <td> <p>Selezionare il tipo di nuova riga (interruzione di riga).</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Intestazioni maiuscole]</p> </td> 
   <td> <p>Abilita questa opzione per convertire il testo racchiuso tra i tag di intestazione (ad esempio &lt;h2&gt; &lt;/h2&gt;) nel testo in maiuscolo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Pattern di corrispondenza]

La [!UICONTROL Pattern di corrispondenza] Il modulo ti consente di trovare ed estrarre elementi stringa che corrispondono a un pattern di ricerca da un determinato testo. Questo modulo utilizza espressioni regolari (note anche come regex o regexp).

Un&#39;espressione regolare è una sequenza di caratteri in cui ogni carattere è un metacarattero, con un significato speciale, o un carattere regolare con un significato letterale. Questi caratteri e metacaratteri identificano un pattern che può essere utilizzato per la ricerca di testo. Ad esempio, se si desidera cercare i nomi, è possibile impostare un&#39;espressione regolare per cercare un pattern composto da due parole consecutive che iniziano con lettere maiuscole. Le espressioni regolari sono uno strumento potente per la ricerca e la manipolazione del testo.

Una discussione sulle espressioni regolari va oltre l&#39;ambito di applicazione di questo articolo. Consigliamo le seguenti risorse:

* Per l&#39;elenco completo dei metacaratteri, vedi [Espressioni regolari](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions) nei documenti web MDN.
* Per un&#39;esercitazione su come creare espressioni regolari, si consiglia di [RegexOne](https://regexone.com/).
* Per la sperimentazione con espressioni regolari, si consiglia l’ [Espressioni regolari 101](https://regex101.com/) sito web. Selezionare ECMAScript (JavaScript) FLAVOR nel pannello a sinistra.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Pattern] </td> 
   <td> <p>Immettere il pattern di espressione regolare. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span> <code>[+-]?(\d+(\.\d+)?|\.\d+)([eE][+-]?\d+)?</code> estrae tutti i numeri nel testo fornito.</p> <p>Nota:  <p>Il modello deve contenere almeno un gruppo di cattura tra parentesi <code>()</code>. Se il pattern non contiene gruppi di acquisizione, il bundle di output è vuoto.</p> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Global match]</td> 
   <td> <p>Abilita questa opzione per recuperare tutte le corrispondenze nel testo. Ogni corrispondenza viene trasmessa in un bundle separato. Se questa opzione è disabilitata, il modulo recupera solo la prima voce.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maiuscole/minuscole]</td> 
   <td> <p> Attiva questa opzione per questo modulo per trattare il testo con distinzione tra maiuscole e minuscole.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Multiline] </td> 
   <td> <p>Abilita questa opzione per garantire che i metacaratteri di inizio e di fine (<code>^</code> e <code>$</code>) corrisponde all’inizio o alla fine di ogni riga, non solo all’inizio o alla fine dell’intera stringa di input.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Singleline]</td> 
   <td>Abilita questa opzione per garantire che il punto (.) corrisponde ai caratteri di nuova riga (<code>\n</code>).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Continua l’esecuzione del percorso anche se il modulo non restituisce risultati]</td> 
   <td> <p>Abilita questa opzione per garantire che il modulo non interrompa lo scenario se non restituisce risultati.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Testo] </td> 
   <td> <p>Immettere o mappare il testo che si desidera associare al pattern.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Sostituisci]

Cerca nel testo immesso un valore o un&#39;espressione regolare specificati e sostituisce il risultato con il nuovo valore.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Pattern] </td> 
   <td> <p>Inserisci il termine di ricerca. È inoltre possibile utilizzare un’espressione regolare. Per ulteriori dettagli sull’espressione regolare, consulta la sezione <a href="#match-pattern" class="MCXref xref">[!UICONTROL Pattern di corrispondenza]</a> modulo .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nuovo valore]</td> 
   <td> <p> Immettere un valore che sostituisca il termine di ricerca.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Global match]</td> 
   <td> <p>Abilita questa opzione per recuperare tutte le corrispondenze nel testo. Ogni corrispondenza viene trasmessa in un bundle separato. Se questa opzione è disabilitata, il modulo recupera solo la prima voce.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maiuscole/minuscole]</td> 
   <td> <p> Attiva questa opzione per questo modulo per trattare il testo con distinzione tra maiuscole e minuscole.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Multiline] </td> 
   <td> <p>Abilita questa opzione per garantire che i metacaratteri di inizio e di fine (<code>^</code> e <code>$</code>) corrisponde all’inizio o alla fine di ogni riga, non solo all’inizio o alla fine dell’intera stringa di input.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Singleline]</td> 
   <td>Abilita questa opzione per garantire che il punto (.) corrisponde ai caratteri di nuova riga (<code>\n</code>).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Testo] </td> 
   <td> <p>Immettere il testo da cercare.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Scraping dei dati

Lo scraping dei dati, talvolta chiamato web scraping, estrazione dei dati o raccolta web, è il processo di raccolta dei dati dai siti web e di memorizzazione nel database o nei fogli di calcolo locali. Se desideri estrarre dati da un sito web e non hai familiarità con le espressioni regolari, puoi utilizzare uno strumento di scraping dei dati:

* [Apificare](https://apify.com/)
* [Migliori strumenti di scansione dei dati per il 2019](https://www.octoparse.com/blog/best-data-scraping-tools-for-2019-top-10-reviews)

Se lo strumento di scraping dei dati fornisce un’API REST, puoi connetterti a essa tramite il nostro universale [[!UICONTROL HTTP] moduli](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md) e [Webhook](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md) moduli.
