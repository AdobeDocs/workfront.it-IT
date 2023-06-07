---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
navigation-topic: apps-and-their-modules
title: Parser testo
description: È possibile utilizzare lo strumento parser di testo per analizzare il testo da utilizzare in altri [!DNL Adobe Workfront Fusion] moduli di scenario. Il parser di testo non richiede una connessione.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 7d71cf64-4f86-42c5-81e7-8fc15333cbd7
source-git-commit: 54d1753b9062b6d4910e4478c1f072b7fedc87eb
workflow-type: tm+mt
source-wordcount: '996'
ht-degree: 0%

---

# [!UICONTROL Parser testo]

È possibile utilizzare [!UICONTROL Strumento parser testo] per analizzare il testo da utilizzare in altri [!DNL Adobe Workfront Fusion] moduli di scenario. Il [!UICONTROL Parser testo] non richiede una connessione.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] per l'automazione e l'integrazione del lavoro] </p> <p>[!UICONTROL [!DNL Workfront Fusion] per automazione lavoro]</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare la funzionalità descritta in questo articolo.</td> 
  </tr> 
 </tbody> 
</table>

Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, consulta [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL Parser testo] moduli e relativi campi

Quando si configura [!UICONTROL Parser testo] moduli, [!DNL Adobe Workfront Fusion] visualizza i campi elencati di seguito. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se viene visualizzato il pulsante Mappa sopra un campo o una funzione, è possibile utilizzarlo per impostare variabili e funzioni per tale campo. Per ulteriori informazioni, consulta [Mappare le informazioni da un modulo all’altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Trasformatori

* [[!UICONTROL Ottieni elementi da HTML]](#get-elements-from-html)
* [[!UICONTROL Ottieni elementi dal testo]](#get-elements-from-text)
* [[!UICONTROL HTML a testo]](#html-to-text)
* [[!UICONTROL Corrispondenza pattern]](#match-pattern)
* [[!UICONTROL Sostituisci]](#replace)

#### [!UICONTROL Ottieni elementi da HTML]

Recupera gli elementi desiderati dal codice HTML.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Continua l'esecuzione della route anche se il modulo non trova corrispondenze]</td> 
   <td> <p>Abilita questa opzione per garantire che il modulo non interrompa lo scenario se non restituisce alcun risultato.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo di elemento]</td> 
   <td> <p> Seleziona il tipo di elemento da recuperare dal codice HTML. </p> 
    <ul> 
     <li>[!UICONTROL Image]</li> 
     <li>[!UICONTROL Link]</li> 
     <li>[!UICONTROL elementi iFrame]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL HTML] </td> 
   <td> <p>Immettere o mappare il codice HTML da cui si desidera recuperare i tipi di elemento specificati.</p> </td> 
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
   <td> <p>Immettere o mappare il testo che si desidera analizzare.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pattern]</td> 
   <td> <p>Selezionate il motivo che riflette gli elementi da analizzare dal testo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ignora occorrenze duplicate]</td> 
   <td> <p>Selezionare questa casella per ignorare le occorrenze duplicate di un elemento di testo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL HTML a testo]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL HTML] </td> 
   <td> <p>Immettere il codice HTML che si desidera convertire in testo normale.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Interruzione di riga] </td> 
   <td> <p>Seleziona il tipo di nuova riga (interruzione di riga).</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Intestazioni in maiuscolo]</p> </td> 
   <td> <p>Abilita questa opzione per convertire il testo racchiuso nei tag di intestazione (ad esempio &lt;h2&gt; &lt;/h2&gt;) nel testo in maiuscolo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Corrispondenza pattern]

Il [!UICONTROL Corrispondenza pattern] Il modulo consente di trovare ed estrarre elementi stringa corrispondenti a un pattern di ricerca da un determinato testo. Questo modulo utilizza espressioni regolari (note anche come regex o regexp).

Un’espressione regolare è una sequenza di caratteri in cui ogni carattere è un metacarattere, con un significato speciale, o un carattere regolare con un significato letterale. Questi caratteri e metacaratteri identificano un pattern che può essere utilizzato per la ricerca di testo. Ad esempio, se si desidera cercare i nomi, è possibile impostare un&#39;espressione regolare per cercare un motivo costituito da due parole consecutive che iniziano con lettere maiuscole. Le espressioni regolari sono uno strumento utile per la ricerca e la manipolazione del testo.

Una discussione sulle espressioni regolari va oltre lo scopo di questo articolo. Si consiglia di utilizzare le risorse seguenti:

* Per l&#39;elenco completo dei metacaratteri, vedere [Espressioni regolari](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions) nei documenti web MDN.
* Per un tutorial su come creare espressioni regolari, si consiglia di [RegexOne](https://regexone.com/).
* Per la sperimentazione con espressioni regolari, si consiglia di [Espressioni regolari 101](https://regex101.com/) sito Web. Selezionare ECMAScript (JavaScript) FLAVOR nel pannello sinistro.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Pattern] </td> 
   <td> <p>Immettete il pattern di espressione regolare. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span> <code>[+-]?(\d+(\.\d+)?|\.\d+)([eE][+-]?\d+)?</code> estrae tutti i numeri nel testo specificato.</p> <p>Nota:  <p>Il modello deve contenere almeno un gruppo di acquisizione tra parentesi <code>()</code>. Se il modello non contiene gruppi di acquisizione, il bundle di output è vuoto.</p> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Corrispondenza globale]</td> 
   <td> <p>Abilita questa opzione per recuperare tutte le corrispondenze nel testo. Ogni corrispondenza viene generata in un bundle separato. Se questa opzione è disattivata, il modulo recupera solo la prima voce.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Distinzione maiuscole/minuscole]</td> 
   <td> <p> Abilita questa opzione per questo modulo per trattare il testo con distinzione tra maiuscole e minuscole.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Multiline] </td> 
   <td> <p>Abilita questa opzione per garantire che i metacaratteri iniziale e finale (<code>^</code> e <code>$</code>) corrisponde all'inizio o alla fine di ogni riga, non solo all'inizio o alla fine dell'intera stringa di input.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Singleline]</td> 
   <td>Abilita questa opzione per garantire che il periodo (.) corrisponde ai caratteri di nuova riga (<code>\n</code>).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Continua l'esecuzione della route anche se il modulo non restituisce alcun risultato]</td> 
   <td> <p>Abilita questa opzione per garantire che il modulo non interrompa lo scenario se non restituisce alcun risultato.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Text] </td> 
   <td> <p>Immettere o mappare il testo che si desidera associare al motivo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Sostituisci]

Cerca un valore o un&#39;espressione regolare specificata nel testo immesso e sostituisce il risultato con il nuovo valore.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Pattern] </td> 
   <td> <p>Immettere il termine di ricerca. È inoltre possibile utilizzare un'espressione regolare. Per ulteriori dettagli sull’espressione regolare, consulta <a href="#match-pattern" class="MCXref xref">[!UICONTROL Match Pattern]</a> modulo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nuovo valore]</td> 
   <td> <p> Immettere un valore che sostituisca il termine di ricerca.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Corrispondenza globale]</td> 
   <td> <p>Abilita questa opzione per recuperare tutte le corrispondenze nel testo. Ogni corrispondenza viene generata in un bundle separato. Se questa opzione è disattivata, il modulo recupera solo la prima voce.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Distinzione maiuscole/minuscole]</td> 
   <td> <p> Abilita questa opzione per questo modulo per trattare il testo con distinzione tra maiuscole e minuscole.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Multiline] </td> 
   <td> <p>Abilita questa opzione per garantire che i metacaratteri iniziale e finale (<code>^</code> e <code>$</code>) corrisponde all'inizio o alla fine di ogni riga, non solo all'inizio o alla fine dell'intera stringa di input.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Singleline]</td> 
   <td>Abilita questa opzione per garantire che il periodo (.) corrisponde ai caratteri di nuova riga (<code>\n</code>).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Text] </td> 
   <td> <p>Immettere il testo in cui eseguire la ricerca.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Scraping dei dati

Il raschiamento dei dati, a volte chiamato web scraping, estrazione dei dati o web harvesting, è il processo di raccolta dei dati dai siti web e di archiviazione nel database locale o nei fogli di calcolo. Se desideri estrarre i dati da un sito web e non hai familiarità con le espressioni regolari, puoi utilizzare uno strumento di raschiamento dei dati.

Se lo strumento di raschiamento dati fornisce un’API REST, puoi connetterti ad essa tramite il nostro universale [[!UICONTROL HTTP] moduli](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md) e [Webhook](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md) moduli.
