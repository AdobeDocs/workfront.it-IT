---
product-area: reporting
navigation-topic: text-mode-reporting
title: Utilizzare la formattazione condizionale in modalità testo
description: Utilizzare la formattazione condizionale in modalità testo
author: Nolan
feature: Reports and Dashboards
exl-id: 48fc8450-35c6-4d59-89d3-0feffe662b25
source-git-commit: 9b6552fe496a1602786cdc6b6050d02cd367a531
workflow-type: tm+mt
source-wordcount: '1743'
ht-degree: 1%

---

# Utilizzare la formattazione condizionale in modalità testo

<!--
(NOTE: Alina: this article might need to be split in its sections. Tony asked that numbers and dates should be in separate articles (??))
-->

Il generatore di interfacce standard offre un’ampia gamma di flessibilità nella creazione di elementi di reporting per soddisfare le esigenze della tua organizzazione.

È possibile applicare la formattazione condizionale a una visualizzazione utilizzando l&#39;interfaccia standard.\
Per ulteriori informazioni sull&#39;applicazione della formattazione condizionale a una visualizzazione, vedere [Utilizzare la formattazione condizionale nelle visualizzazioni](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modifica accesso a Filtri, Viste, Raggruppamenti</p> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari per modificare le visualizzazioni in un rapporto</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un report per modificare le visualizzazioni in un report</p> <p>Gestire le autorizzazioni per una visualizzazione per modificarla</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

## Formattazione condizionale in modalità testo

La modalità testo consente di creare visualizzazioni, filtri, raggruppamenti e prompt più complessi, consentendo di utilizzare campi non disponibili nell&#39;interfaccia standard.

Per un elenco completo di tutti i campi da segnalare, vedi  [API Explorer](../../../wf-api/general/api-explorer.md).

Per ulteriori informazioni sull&#39;utilizzo della sintassi in modalità testo, vedere [Panoramica sulla sintassi della modalità testo](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md).

È inoltre possibile utilizzare la modalità testo per formattare le visualizzazioni nei report e negli elenchi. Utilizzando la formattazione condizionale, è possibile modificare le visualizzazioni dei rapporti modificando il tipo di carattere e lo sfondo dei risultati, nonché le icone e i contrassegni. È consigliabile creare sempre le visualizzazioni utilizzando prima l’interfaccia standard e passare all’interfaccia in modalità testo solo quando assolutamente necessario.

>[!NOTE]
>
> L’utilizzo dello stile CSS per personalizzare la formattazione condizionale non è supportato. Utilizza invece le opzioni di formattazione predefinite disponibili in Adobe Workfront.

## Aggiungere la formattazione condizionale alle visualizzazioni

Per ulteriori informazioni sull&#39;applicazione della formattazione condizionale a una visualizzazione nell&#39;interfaccia standard del generatore, vedere [Utilizzare la formattazione condizionale nelle visualizzazioni](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

Per aggiungere la formattazione condizionale a una visualizzazione nell&#39;interfaccia della modalità testo:

1. Consente di passare a un elenco di oggetti.
1. Espandere il menu a discesa di una visualizzazione a cui si desidera aggiungere la formattazione condizionale.
1. Clic **Personalizza visualizzazione**.
1. Fare clic sulla colonna della visualizzazione alla quale si desidera applicare la formattazione condizionale.
1. Clic **Passa alla modalità testo**.
1. In **Mostra in questa colonna:** , fare clic su **Fare clic per modificare il testo**.
1. Aggiungi gli esempi di codice forniti in [Formattare le visualizzazioni utilizzando la modalità testo](#format-views-using-text-mode) nella parte inferiore del testo nella colonna selezionata.
1. Clic **Salva**, quindi fai clic su **Salva visualizzazione**.

## Formattare le visualizzazioni utilizzando la modalità testo {#format-views-using-text-mode}

È possibile aggiungere i seguenti componenti a una colonna in una vista per formattarla in modo condizionale in modalità testo:

* [Impostazioni colonna](#column-settings)
* [Regole colonna](#column-rules)
* [Formattare un&#39;espressione di valore in modo condizionale](#conditionally-format-a-valueexpression)

### Impostazioni colonna {#column-settings}

È necessario avere familiarità con l&#39;interfaccia in modalità testo prima di poter aggiungere la formattazione condizionale alle visualizzazioni.

Quando si utilizza la formattazione condizionale in una visualizzazione, è possibile personalizzare i seguenti elementi di una colonna:

* [Intestazioni di colonna](#column-headers)
* [Formato date](#format-dates)
* [Formato numeri](#format-numbers)

#### Intestazioni di colonna {#column-headers}

Per modificare l’intestazione di colonna visualizzata, aggiungi il seguente codice alla colonna: `displayname= [Name of column]`. Ad esempio, per nominare una colonna Proprietario progetto, il codice di testo sarà simile al seguente:

```
displayname=Project Owner
```

#### Formato date {#format-dates}

Le date possono essere configurate per la visualizzazione in diversi formati.

Per ulteriori informazioni, consulta [Formattare le date nei report in modalità testo](../../../reports-and-dashboards/reports/text-mode/format-dates-in-text-mode-reports.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this is drafted and replaced by the article linked above)</p>
<p>To establish a date format, you must modify the <code>valueformat</code> line of the text mode code in the column.</p>
<pre>valueformat= [new date format]</pre>
<p>For example, if you wanted the Projected Completion Date to be displayed as MM/DD/YY the code would look like:</p>
<pre>valueformat=atDate<br>valuefield=projectedCompletionDate </pre>
<p>If you wanted to show the Planned Completion Date as <em>Mth, DD, Year</em>, the code would look like:</p>
<pre>valueformat=mediumAtdate<br>valuefield=plannedCompletionDate</pre>
<p>You can format dates using the following <code>valueformat</code> text mode values:</p>
<table style="table-layout:auto">
<col>
<col>
<col>
<thead>
<tr>
<th scope="col"><strong>Format</strong> </th>
<th scope="col">Example </th>
<th scope="col"><em><strong>valueformat=</strong></em> </th>
</tr>
</thead>
<tbody>
<tr>
<td>MM/DD/YY</td>
<td>10/11/18</td>
<td><pre>atDate</pre> </td>
</tr>
<tr>
<td>MM/DD/YY Time</td>
<td>10/11/18 12:00pm</td>
<td><pre>longAtDate</pre> </td>
</tr>
<tr>
<td>MM/DD/YY</td>
<td>10/11/18</td>
<td><pre>shortAtDate</pre> </td>
</tr>
<tr>
<td>Mth, DD, YR</td>
<td>Oct, 11, 2018</td>
<td><pre>mediumAtDate</pre> </td>
</tr>
<tr>
<td>DW, Mth, Day, YR</td>
<td>Mon, Oct, 11, 2018</td>
<td><pre>partialAtDate</pre> </td>
</tr>
<tr>
<td>DW, Mth, Day, YR Time</td>
<td>Mon, Oct, 11, 2018 12:00 pm</td>
<td><pre>fullAtDate</pre> </td>
</tr>
</tbody>
</table>
</div>
-->

#### Formato numeri {#format-numbers}

È possibile formattare i valori numerici per visualizzare le informazioni più adatte alle proprie esigenze di reporting.

Per ulteriori informazioni, consulta [Formattare numeri, valuta e valori percentuali nei report in modalità testo](../../../reports-and-dashboards/reports/text-mode/format-numbers-in-text-mode-reports.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>To modify the format of a numeric value, you must edit the <strong>valueformat</strong> line of your column.</p> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this is drafted and replaced by the article linked above) </p>
<p>For example, if you wanted to display the Budget column as $1000, the value format line would look like:</p>
<pre>valueformat=currencyStringCurrencyRounded<br>valuefield=budget</pre>
<p>You can format numbers using the following values for the <code>valueformat</code> line of your column:</p>
<table border="2" cellspacing="15" cellpadding="1">
<col>
<col>
<thead>
<tr>
<th scope="col"><strong>Example</strong> </th>
<th scope="col"><em><code>valueformat=</code></em> </th>
</tr>
</thead>
<tbody>
<tr>
<td>1234</td>
<td><pre>doubleAsString</pre> or <pre>int</pre></td>
</tr>
<tr>
<td>1,234</td>
<td><pre>doubleAsInt</pre> </td>
</tr>
<tr>
<td>$1,234</td>
<td><pre>currencyStringCurrencyRounded</pre> </td>
</tr>
<tr>
<td>1234.56</td>
<td><pre>doubleAsDouble</pre> </td>
</tr>
<tr>
<td>$1,234.56</td>
<td><pre>currencyStringCurrency</pre> </td>
</tr>
<tr>
<td>12%</td>
<td><pre>doubleAsPercentRounded</pre> </td>
</tr>
<tr>
<td>12.34%</td>
<td><pre>doubleAsPercent</pre> </td>
</tr>
<tr>
<td>(1,234.56)</td>
<td><pre>doubleAsFinancial</pre> </td>
</tr>
<tr>
<td>(1,234)</td>
<td><pre>doubleAsFiancialRounded</pre> </td>
</tr>
</tbody>
</table>
</div>
-->

### Regole colonna {#column-rules}

Le regole di colonna consentono di aggiungere immagini, colore, formattazione e sostituzioni di testo all’interno di una visualizzazione. Le regole di colonna possono essere stabilite in modo indipendente o possono contenere più condizioni per una colonna.

* [Formattazione condizionale](#conditional-formatting)
* [Più formati condizionali](#multiple-conditional-formats)
* [Applica testo](#apply-text)
* [Applicare formati di riga](#apply-row-formats)
* [Applicare le immagini](#apply-images)

#### Formattazione condizionale {#conditional-formatting}

Quando si incorpora un colore o si formatta un testo, è necessario applicare un’istruzione specifica per la modalità testo.

>[!NOTE]
>
>La formattazione condizionale potrebbe non essere supportata nelle colonne unite.\
>Per ulteriori informazioni sull&#39;unione di colonne con la modalità testo, vedere [Vista: unire le informazioni provenienti da più colonne in una colonna condivisa](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md).

Inserisci il seguente codice in qualsiasi colonna in cui desideri aggiungere la formattazione condizionale:

```
styledef.case.0.comparison.leftmethod= [field name]
styledef.case.0.comparison.lefttext= [field name]
styledef.case.0.comparison.righttext= [field value]
styledef.case.0.comparison.operator= [qualifier]
styledef.case.0.comparison.operatortype= [data type]
styledef.case.0.comparison.icon=false
styledef.case.0.comparison.truetext= 
styledef.case.0.comparison.trueproperty.0.name= [format option]
styledef.case.0.comparison.trueproperty.0.value= [format style]
```

>[!NOTE]
>
>Il *styledef.case.0.comparison.icon* La riga è sempre false a meno che non si utilizzino le icone.
>
>Il *styledef.case.0.comparison.truetext* La riga viene sempre lasciata vuota fino a quando non si utilizza la sovrascrittura del testo.
>
>Il *styledef.case.0.comparison.righttext* la riga è vuota quando il qualificatore non è vuoto.

Ad esempio, se desideri visualizzare il Nome azienda in verde in un report di progetto, puoi utilizzare il seguente codice:

```
styledef.case.0.comparison.leftmethod=company:name
styledef.case.0.comparison.lefttext=company:name ;
styledef.case.0.comparison.righttext= 
styledef.case.0.comparison.operator=notblank
styledef.case.0.comparison.operatortype=string
styledef.case.0.comparison.icon=false
styledef.case.0.comparison.truetext=
styledef.case.0.comparison.trueproperty.0.name=textcolor
styledef.case.0.comparison.trueproperty.0.value=03a219
```

>[!NOTE]
>
>* Questa istruzione può essere applicata a una colonna Nome società, ma può anche essere applicata a qualsiasi altra colonna del report. Il testo verde viene visualizzato solo se al progetto è associata una società. Ricorda la `[field name]`, `[value]`, e `[qualifier]` guida, a prescindere dal fatto che il condizionamento venga visualizzato sulla colonna.
>* Quando si lavora con i qualificatori, si consiglia di utilizzare `cicontains` anziché `equal`. Per impostazione predefinita, `equal` cerca i numeri ID. Utilizzo di `cicontains` qualificatore, puoi accedere agli elementi in base al loro nome.

![](assets/screen-shot-2013-08-15-at-2.53.51-pm-350x199.png)

![](assets/screen-shot-2013-08-15-at-2.54.08-pm-350x185.png)

Se a una modalità testo vengono applicati il colore del testo, l&#39;allineamento, lo stile del carattere o il colore di sfondo, viene utilizzata la stessa istruzione (illustrata sopra).

Le righe seguenti devono essere modificate per riflettere la formattazione corrispondente necessaria per la colonna:

```
styledef.case.0.comparison.trueproperty.0.name= [format option]
styledef.case.0.comparison.trueproperty.0.value= [format style]
```

Utilizzare le tabelle seguenti per identificare le righe da modificare e i valori da specificare per definire lo stile di formato della colonna:

| **Colore testo** | **Line: textcolor=** |
|---|---|
| Nero | `000000` |
| Blu scuro | `0c6aca` |
| Verde acqua | `1b878c` |
| Verde | `03a219` |
| Viola | `6408c4` |
| Grigio | `767676` |
| Rosso | `d30519` |
| Giallo | `e19503` |

{style="table-layout:auto"}

| **Allineamento** | **Line: align=** |
|---|---|
| Allineamento a sinistra | `left` |
| Allineamento a destra | `right` |
| Allineamento al centro | `center` |

{style="table-layout:auto"}

| Font | Riga: ***fontstyle=*** |
|---|---|
| Bold | `bold` |
| Italic | `italic` |

{style="table-layout:auto"}

| **Colore di fondo** | **Line: bgcolor=** |
|---|---|
| Verde acqua | `dcf6f7` |
| Verde | `def6e2` |
| Grigio | `e8e8e8` |
| Blu | `e8f1ff` |
| Viola | `e9def4` |
| Rosso | `eac6c9` |
| Giallo | `feecc8` |
| Bianco | `ffffff` |

{style="table-layout:auto"}

#### Più formati condizionali {#multiple-conditional-formats}

È possibile applicare più stili di formattazione a un&#39;istruzione. L’istruzione core rimarrà invariata e tutte le espressioni di formattazione aggiuntive verranno aggiunte all’istruzione.

Ad esempio, utilizzando l’istruzione precedente per includere Nome azienda nel testo in grassetto verde. L’istruzione viene scritta con il seguente codice:

```
styledef.case.0.comparison.leftmethod=company:name
styledef.case.0.comparison.lefttext=company:name
styledef.case.0.comparison.righttext=
styledef.case.0.comparison.operator=notblank
styledef.case.0.comparison.operatortype=string
styledef.case.0.comparison.icon=false
styledef.case.0.comparison.truetext= 
styledef.case.0.comparison.trueproperty.0.name=textcolor
styledef.case.0.comparison.trueproperty.0.value=03a219
styledef.case.0.comparison.trueproperty.1.name=fontstyle
styledef.case.0.comparison.trueproperty.1.value=bold
```

>[!NOTE]
>
>Quando si includono più espressioni di formattazione condizionale, è necessario identificare numericamente ogni espressione nell&#39;istruzione. Sono state identificate l’espressione 0 e l’espressione 1.

#### Applica testo {#apply-text}

Se si desidera sostituire i valori predefiniti che vengono inseriti in una colonna con un valore scelto, è possibile applicare del testo alla colonna.

Ad esempio, in un rapporto di progetto, imposta il valore della colonna Data inizio pianificata in modo da non visualizzare la data di inizio pianificata per il progetto, ma il testo &quot;Non oggi&quot;. Utilizza il seguente codice per la colonna Data inizio pianificata:

```
case.0.comparison.leftmethod=plannedStartDate
case.0.comparison.lefttext=plannedStartDate
case.0.comparison.righttext=2013-04-10T10:45:00:000
case.0.comparison.operator=ne
case.0.comparison.operatortype=date
case.0.comparison.icon=false
case.0.comparison.truetext=not today
styledef.case.0.comparison.leftmethod=plannedStartDate
styledef.case.0.comparison.lefttext=plannedStartDate
styledef.case.0.comparison.righttext=2013-04-10T10:45:00:000 
styledef.case.0.comparison.operator=ne
styledef.case.0.comparison.operatortype=date&
styledef.case.0.comparison.icon=false
styledef.case.0.comparison.truetext=not today
```

>[!NOTE]
>
>Le righe che iniziano con `case.0.` confronti tra casi d’uso per identificare l’utilizzo del testo. Le righe che iniziano con **styledef.case.0.** sono le prime istruzioni di formattazione condizionale in cui viene identificato l’utilizzo del testo tramite `truetext` espressione. Assicurati di impostare `truetext` a un valore, anziché lasciarlo vuoto.

![](assets/screen-shot-2013-08-15-at-3.22.02-pm-350x196.png)

![](assets/screen-shot-2013-08-15-at-3.22.16-pm-350x151.png)

#### Applicare formati di riga {#apply-row-formats}

Se desideri applicare una condizione all’intera riga, utilizza il seguente codice con il codice di colonna:

```
styledef.case.0.comparison.icon=false
```

```
styledef.case.0.comparison.isrowcase=true
```

```
styledef.case.0.comparison.leftmethod= [field name]
```

```
styledef.case.0.comparison.lefttext= [field name]
```

```
styledef.case.0.comparison.operator= [qualifier]
```

```
styledef.case.0.comparison.operatortype= [data type]
```

```
styledef.case.0.comparison.righttext= [field value]
```

```
styledef.case.0.comparison.trueproperty.0.name= [format option]
```

```
styledef.case.0.comparison.trueproperty.0.value= [format style]
```

```
styledef.case.0.comparison.truetext=
```

```
row.0.styledef.applyallcases=true
```

```
row.0.styledef.case.0.comparison.icon=false
```

```
row.0.styledef.case.0.comparison.isrowcase=true
```

```
row.0.styledef.case.0.comparison.leftmethod= [field name]
```

```
row.0.styledef.case.0.comparison.lefttext= [field name]
```

```
row.0.styledef.case.0.comparison.operator= [qualifier]
```

```
row.0.styledef.case.0.comparison.operatortype= [data type]
```

```
row.0.styledef.case.0.comparison.righttext= [field value]
```

```
row.0.styledef.case.0.comparison.trueproperty.0.name= [format option]
```

```
row.0.styledef.case.0.comparison.trueproperty.0.value= [format style]
```

```
row.0.styledef.case.0.comparison.truetext=
```


#### Applicare le immagini {#apply-images}

Analogamente alla formattazione con il testo, le immagini possono essere utilizzate per visualizzare informazioni nei rapporti. Workfront dispone di diverse immagini incorporate per trasmettere informazioni visive in un&#39;impostazione di rapporto. Per utilizzare le immagini nell’impostazione della formattazione condizionale è necessaria l’istruzione seguente:

```
image.case.0.comparison.leftmethod= [field name]
image.case.0.comparison.lefttext= [field name]
image.case.0.comparison.righttext= [field value]
image.case.0.comparison.operator= [qualifier]
image.case.0.comparison.operatortype= [data type]
image.case.0.comparison.icon=true
image.case.0.comparison.truetext=
```

Ad esempio, in un rapporto di progetto, desideri creare una colonna in cui visualizzare un volto disordinato per ogni Data di completamento pianificata che non sia uguale alla data odierna. Utilizza il seguente codice in modalità testo per aggiungere l’icona alla colonna:

```
image.case.0.comparison.leftmethod=plannedCompletionDate
image.case.0.comparison.lefttext=plannedCompletionDate
image.case.0.comparison.righttext=2013-04-10T13:00:00:000 
image.case.0.comparison.operator=ne 
image.case.0.comparison.operatortype=date
image.case.0.comparison.icon=true
image.case.0.comparison.truetext=/interface/images/v4_redux/icons/casebuilder/emoticon_frown.gif
```

>[!NOTE]
>
>Si noti che l&#39;istruzione utilizza `icon=true` espressione. Questa istruzione è diversa anche da altre istruzioni di formattazione condizionale in quanto non utilizza `style.def` ma piuttosto un formato immagine univoco.

![](assets/screen-shot-2013-08-15-at-3.35.08-pm-350x199.png)

![](assets/screen-shot-2013-08-15-at-3.35.22-pm-1-350x167.png)

Per utilizzare le immagini disponibili, applica il codice e i valori seguenti:

| **Icona** | **Riga: image.case.0.comparison.truetext=** |
|---|---|
| Faccia accigliata ![](assets/face-sad.png) | =`/interface/images/v4_redux/icons/casebuilder/emoticon_frown.gif` |
| Volto felice ![](assets/face-happy.png) | =`/interface/images/v4_redux/icons/casebuilder/emoticon_smile.gif` |
| Flag blu  ![](assets/flag-blue-large.png) | =`/interface/images/v4_redux/icons/casebuilder/flag_blue.gif` |
| Flag verde  ![](assets/flag-green-large.png) | =`/interface/images/v4_redux/icons/casebuilder/flag_green.gif` |
| Segnalazione rossa  ![](assets/flag-red-style2.png) | =`/interface/images/v4_redux/icons/casebuilder/flag_red.gif` |
| Flag giallo  ![](assets/flag-yellow-style2.png) | =`/interface/images/v4_redux/icons/casebuilder/flag_yellow.gif` |
| Cerchio nero  ![](assets/dot-black.png) | =`/interface/images/v4_redux/icons/casebuilder/light_black.gif` |
| Cerchio blu ![](assets/dot-blue.png) | =`/interface/images/v4_redux/icons/casebuilder/light_blue.gif` |
| Cerchio grigio ![](assets/dot-gray.png) | =`/interface/images/v4_redux/icons/casebuilder/light_grey.gif` |
| Cerchio verde ![](assets/dot-green.png) | =`/interface/images/v4_redux/icons/casebuilder/light_green.gif` |
| Cerchio arancione ![](assets/dot-orange.png) | =`/interface/images/v4_redux/icons/casebuilder/light_orange.gif` |
| Cerchio rosa ![](assets/dot-pink.png) | =`/interface/images/v4_redux/icons/casebuilder/light_pink.gif` |
| Cerchio viola ![](assets/dot-purple.png) | =`/interface/images/v4_redux/icons/casebuilder/light_purple.gif` |
| Cerchio rosso ![](assets/dot-red.png) | =`/interface/images/v4_redux/icons/casebuilder/light_red.gif` |
| Cerchio bianco ![](assets/dot-white.png) | =`/interface/images/v4_redux/icons/casebuilder/light_white.gif` |
| Cerchio giallo ![](assets/dot-yellow.png) | =`/interface/images/v4_redux/icons/casebuilder/light_yellow.gif` |

{style="table-layout:auto"}

### Formattare in modo condizionale una `valueexpression` {#conditionally-format-a-valueexpression}

Per visualizzare un valore calcolato in una colonna, è possibile sostituire il `valuefield` riga di codice nella colonna con una `valueexpression`. Un valore calcolato consente di visualizzare un nuovo valore per un oggetto in base al calcolo tra due campi esistenti sullo stesso oggetto.

Per ulteriori informazioni su come formattare `valueexpression line`, vedi [Panoramica sulla sintassi della modalità testo](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md).

Non è possibile formattare in modo condizionale una colonna che contiene `valueexpression` riga di codice. È invece possibile aggiungere un campo personalizzato calcolato a un modulo personalizzato e associarlo agli oggetti visualizzati nel report. È quindi possibile formattare in modo condizionale le colonne che visualizzano questo campo.

Per ulteriori informazioni sui campi personalizzati calcolati, vedi [Aggiungere dati calcolati a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## Aggiungere un valore aggregatore in una colonna Modalità testo

È consigliabile innanzitutto creare la colonna nell’interfaccia del generatore di, aggiungere il valore dell’aggregatore e quindi modificare la colonna in modalità testo.

Quando si aggiungono aggregatori a una colonna in modalità testo, tenere presente quanto segue:

* I valori nella colonna devono avere un formato riepilogabile. Ad esempio, devono avere uno dei seguenti formati:

   * Numero
   * Data
   * Valuta

* È possibile aggiungere un aggregatore a una colonna che visualizza un calcolo. Il valore aggregato viene visualizzato nel raggruppamento della visualizzazione o del report. Per ulteriori informazioni, consulta [Raggruppamento: visualizza il risultato dell’aggregazione di più valori calcolati in un raggruppamento](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-calculation-between-two-fields-aggregated-in-grouping.md).
* Le righe di codice per la definizione della colonna devono essere identiche alle righe di codice che introducono l&#39;aggregatore e precedute da &quot;aggregatore&quot;. Ad esempio, in una colonna in cui vengono visualizzate le ore pianificate in un progetto, la modalità testo delle righe principali della colonna è:

  ```
  valuefield=workRequired
  valueformat=compound
  ```

  Quando desideri aggregare il valore di tutte le righe nel raggruppamento della vista, puoi aggiungere il seguente codice per aggiungere i valori dell’aggregatore: `aggregator.valuefield=workRequired` (il `aggregator.valuefield` la riga deve essere uguale alla `valuefield` che descrive la colonna) `aggregator.valueformat=compound` (il `aggregator.valueformat` la riga deve avere lo stesso valore della `valueformat` che descrive la colonna) `aggregator.function=SUM` (questa è una riga obbligatoria che indica come aggregare la colonna; in questo caso, si desidera aggiungere tutte le singole ore pianificate in un unico numero nella riga di raggruppamento) `aggregator.displayformat=minutesAsHoursString` (poiché le ore sono memorizzate in Workfront in pochi minuti, è necessario indicare `displayformat` per le ore in cui sono conservati in minuti)
