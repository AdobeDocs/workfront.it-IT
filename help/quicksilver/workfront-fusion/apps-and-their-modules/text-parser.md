---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
navigation-topic: apps-and-their-modules
title: Parser testo
description: È possibile utilizzare lo strumento parser di testo per analizzare il testo da utilizzare in altri [!DNL Adobe Workfront Fusion]  moduli scenario. Il parser di testo non richiede una connessione.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 7d71cf64-4f86-42c5-81e7-8fc15333cbd7
source-git-commit: 27fb07b7b19bab25bb7ee925e722ccace3bea628
workflow-type: tm+mt
source-wordcount: '1048'
ht-degree: 0%

---

# [!UICONTROL Parser di testo]

È possibile utilizzare lo strumento [!UICONTROL parser di testo] per analizzare il testo da utilizzare in altri moduli di scenario [!DNL Adobe Workfront Fusion]. Il parser [!UICONTROL Text] non richiede una connessione.

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
   <p>Requisito licenza legacy: [!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione lavoro], [!UICONTROL [!DNL Workfront Fusion] per automazione lavoro]</p>
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

## Informazioni API parser di testo

Il connettore parser di testo utilizza quanto segue:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Tag API</td> 
   <td>v2</td> 
  </tr>
 </tbody> 
 </table>

## [!UICONTROL Moduli parser di testo] e relativi campi

Quando configuri i moduli [!UICONTROL Parser di testo], [!DNL Adobe Workfront Fusion] visualizza i campi elencati di seguito. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se viene visualizzato il pulsante Mappa sopra un campo o una funzione, è possibile utilizzarlo per impostare variabili e funzioni per tale campo. Per ulteriori informazioni, vedere [Mappare le informazioni da un modulo all&#39;altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Trasformatori

* [[!UICONTROL Ottieni elementi da HTML]](#get-elements-from-html)
* [[!UICONTROL Ottieni elementi dal testo]](#get-elements-from-text)
* [[!UICONTROL HTML al testo]](#html-to-text)
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

#### [!UICONTROL HTML al testo]

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
   <td> <p>Abilita questa opzione per convertire in testo maiuscolo il testo racchiuso nei tag di intestazione (ad esempio &lt;h2&gt; &lt;/h2&gt;).</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Corrispondenza pattern]

Il modulo [!UICONTROL Match pattern] consente di trovare ed estrarre elementi stringa che corrispondono a un pattern di ricerca da un determinato testo. Questo modulo utilizza espressioni regolari (note anche come regex o regexp).

Un’espressione regolare è una sequenza di caratteri in cui ogni carattere è un metacarattere, con un significato speciale, o un carattere regolare con un significato letterale. Questi caratteri e metacaratteri identificano un pattern che può essere utilizzato per la ricerca di testo. Ad esempio, se si desidera cercare i nomi, è possibile impostare un&#39;espressione regolare per cercare un motivo costituito da due parole consecutive che iniziano con lettere maiuscole. Le espressioni regolari sono uno strumento utile per la ricerca e la manipolazione del testo.

Una discussione sulle espressioni regolari va oltre lo scopo di questo articolo. Si consiglia di utilizzare le risorse seguenti:

* Per l&#39;elenco completo dei metacaratteri, vedere [Espressioni regolari](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions) nei documenti Web MDN.
* Per un&#39;esercitazione sulla creazione di espressioni regolari, consigliamo [RegexOne](https://regexone.com/).
* Per la sperimentazione con espressioni regolari, consigliamo il sito Web [Espressioni regolari 101](https://regex101.com/). Selezionare ECMAScript (JavaScript) FLAVOR nel pannello sinistro.

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
   <td> <p>Abilitare questa opzione per assicurarsi che i metacaratteri iniziale e finale (<code>^</code> e <code>$</code>) corrispondano all'inizio o alla fine di ogni riga, non solo all'inizio o alla fine dell'intera stringa di input.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Singleline]</td> 
   <td>Abilitare questa opzione per assicurarsi che il punto (.) corrisponda ai caratteri di nuova riga (<code>\n</code>).</td> 
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
   <td> <p>Immettere il termine di ricerca. È inoltre possibile utilizzare un'espressione regolare. Per ulteriori dettagli sull'espressione regolare, fare riferimento al modulo <a href="#match-pattern" class="MCXref xref">[!UICONTROL Match Pattern]</a>.</p> </td> 
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
   <td> <p>Abilitare questa opzione per assicurarsi che i metacaratteri iniziale e finale (<code>^</code> e <code>$</code>) corrispondano all'inizio o alla fine di ogni riga, non solo all'inizio o alla fine dell'intera stringa di input.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Singleline]</td> 
   <td>Abilitare questa opzione per assicurarsi che il punto (.) corrisponda ai caratteri di nuova riga (<code>\n</code>).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Text] </td> 
   <td> <p>Immettere il testo in cui eseguire la ricerca.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Scraping dei dati

Il raschiamento dei dati, a volte chiamato web scraping, estrazione dei dati o web harvesting, è il processo di raccolta dei dati dai siti web e di archiviazione nel database locale o nei fogli di calcolo. Se desideri estrarre i dati da un sito web e non hai familiarità con le espressioni regolari, puoi utilizzare uno strumento di raschiamento dei dati.

Se lo strumento di scarto dati fornisce un&#39;API REST, puoi connetterti tramite i nostri moduli universali [[!UICONTROL HTTP]](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md) e [Webhook](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md).
