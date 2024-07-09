---
product-area: reporting
navigation-topic: reporting-elements
title: Modificatori di filtri e condizioni
description: I modificatori di filtri e condizioni ti consentono di creare filtri e stabilire condizioni per la formattazione dei risultati del rapporto.
author: Nolan
feature: Reports and Dashboards
exl-id: 13e9d926-8a89-490e-aa7a-e6e8baf2a36b
source-git-commit: c915c282c6258300b01600dd5b6247e96bf45185
workflow-type: tm+mt
source-wordcount: '1566'
ht-degree: 0%

---

# Modificatori di filtri e condizioni

<!-- Audited: 1/2024 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: This is temporary - Lilit is fixing this in a future story: NOTE If the field you are filtering for has multiple options, this filters out the results that contain only the choice you specify. If the field contains additional options including the one specified, those results are not filtered from the report. See this document and search for "not equal" for the link to the req doc: https://docs.google.com/document/d/1WA0zZ_wws-2qb908i53BFQ8zDwL3nPJHyIybtJvvnqU/edit) </p>
-->

I modificatori di filtri e condizioni ti consentono di creare filtri e stabilire condizioni per la formattazione dei risultati del rapporto.

Per ulteriori informazioni sulla creazione di filtri, consulta l’articolo [Panoramica sui filtri](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Per ulteriori informazioni sull&#39;utilizzo della formattazione condizionale nelle visualizzazioni, vedere l&#39;articolo [Utilizzare la formattazione condizionale nelle visualizzazioni](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

## Modificatori di filtri e condizioni

Alcuni modificatori sono incorporati e puoi sceglierli da un menu a discesa all’interno del filtro o dell’istruzione di formattazione condizionale. Altri modificatori possono essere utilizzati solo nei filtri in modalità testo.

Per ulteriori informazioni sulla modalità testo, consulta [Panoramica sulla modalità testo](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Per un elenco dei modificatori incorporati dell’intervallo di tempo, consulta l’articolo [Filtrare i rapporti per intervalli di tempo](../../../reports-and-dashboards/reports/creating-and-managing-reports/filter-reports-time-frames.md).

Puoi utilizzare i seguenti modificatori di condizioni nei filtri e nelle istruzioni di formattazione condizionale:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Modificatore incorporato</strong> </p> </th> 
   <th> <p><strong>Modificatore modalità testo</strong> </p> </th> 
   <th> <p><strong>Descrizione</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr valign="top"> 
   <td> <p><strong>È vuoto</strong> </p> </td> 
   <td> <p><strong>vuoto</strong> </p> </td> 
   <td> <p>Il campo esiste per l’oggetto, ma al momento non dispone di un valore.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Non è vuoto</strong> </p> </td> 
   <td> <p><strong>notblank</strong> </p> </td> 
   <td> <p>Il campo per il quale stai filtrando esiste ed è stato assegnato un valore.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>nulle</strong> </p> </td> 
   <td> <p>Il campo è vuoto o non esiste. Ad esempio, si desidera cercare elementi senza un ID attività padre. Ciò significa che si desidera visualizzare solo le attività autonome. Il qualificatore per l’"ID attività principale" è <strong>nulle</strong>, poiché un'attività senza un ID (in questo caso l'elemento padre) non esiste. </p> <p>Questo modificatore può essere utilizzato solo nei filtri in modalità testo. Per ulteriori informazioni sulla modalità testo nei filtri, consulta <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Modificare un filtro utilizzando la modalità testo</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notnull</strong> </p> </td> 
   <td> <p>Il campo per il quale si sta filtrando esiste e contiene un valore diverso da null.</p> <p>Questo modificatore può essere utilizzato solo nei filtri in modalità testo. Per ulteriori informazioni sulla modalità testo nei filtri, consulta <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Modificare un filtro utilizzando la modalità testo</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Contiene</strong> </p> </td> 
   <td> <p><strong>cicante</strong> </p> </td> 
   <td> <p>Questo è il <i>senza distinzione tra maiuscole e minuscole</i> versione di <strong>contiene</strong>. Ad esempio: <code>cicontains inf</code> acquisisce qualsiasi valore che contiene <code>Inf</code> o <code>inf</code>.</p> <p> <p>Nota: Adobe Workfront cerca la parola o la frase esatta specificata per ogni istruzione di filtro. Ad esempio, se stai cercando un progetto che contiene la frase <code>new project</code> nel nome, Workfront non mostra i progetti che hanno solo <code>new</code> o semplicemente <code>project</code>, o <code>new main project</code> nel nome. Il filtro trova solo i progetti con la frase esatta <code>new project</code> nel nome.</p> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Does Not Contain</strong> </p> </td> 
   <td> <p><strong>cinotcontains</strong> </p> </td> 
   <td> <p>Questo è il <i>senza distinzione tra maiuscole e minuscole</i> versione di <strong>notcontains</strong>.</p><p>Questo modificatore filtra gli elementi per i quali manca il valore specificato.</p> <p>Ad esempio: <code>does not contain inf</code> acquisisce qualsiasi cosa senza <code>Inf</code> o <code>inf</code> nel nome.</p> <p>Nota: <span>Se il campo per il quale si desidera filtrare dispone di più opzioni, verranno esclusi i risultati che contengono sia la scelta specificata, sia quella specificata ed eventuali altre scelte.</span> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td> <p><strong>contiene</strong> </p> </td> 
   <td> <p> Cerca il <i>distinzione maiuscole/minuscole</i> testo in un'intera stringa di testo.</p> <p>Ad esempio, utilizzando <code>contains Inf</code> acquisisce qualsiasi cosa con <code>Inf</code> in esso, ad esempio la parola <code>Infinity.</code></p> <p>Questo modificatore può essere utilizzato solo nei filtri in modalità testo.Per ulteriori informazioni sulla modalità testo nei filtri, consulta <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Modificare un filtro utilizzando la modalità testo</a>.</p> </td> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notcontains</strong> </p> </td> 
   <td> <p>Filtra gli elementi per i quali manca il <i>distinzione maiuscole/minuscole</i> valore specificato.</p> <p>Ad esempio: <code>notcontains inf</code> acquisisce qualsiasi cosa senza <code>inf</code>, ma visualizza valori che contengono <code>Inf</code>.</p> <p>Questo modificatore può essere utilizzato solo nei filtri in modalità testo. Per ulteriori informazioni sulla modalità testo nei filtri, consulta <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Modificare un filtro utilizzando la modalità testo</a>.</p> </td> 
  </tr> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cieq</strong> </p> </td> 
   <td> <p>Questo è il <i>senza distinzione tra maiuscole e minuscole</i> opzione di <strong>eq</strong>. Restituisce solo una corrispondenza esatta del valore cercato.</p> <p>Ad esempio, quando si cerca un’attività con un nome specifico, <code>task name cieq test</code> trova le attività in cui il nome è <code>Test</code>, <code>TEST</code>, o <code>Test</code>, ma non trova un'attività con il nome <code>test 123.</code></p> <p>Durante la ricerca di uno stato, il <strong>cieq</strong> modificatore non supportato. È necessario utilizzare il modificatore con distinzione tra maiuscole e minuscole, <strong>eq</strong>, per cercare uno stato.</p> <p>Questo modificatore può essere utilizzato solo nei filtri in modalità testo. Per ulteriori informazioni sulla modalità testo nei filtri, consulta <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Modificare un filtro utilizzando la modalità testo</a>.</p> </td>
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td><strong>cine</strong> </td> 
   <td> <p>Questo è il <i>senza distinzione tra maiuscole e minuscole</i> opzione di <strong>ne</strong>ed è l'opposto del <b>cieq</b> modificatore. Restituisce solo risultati che non corrispondono esattamente al valore cercato, senza considerare il caso del valore.</p> <p>Ad esempio: <b>cine</b> restituisce qualsiasi valore che non è uguale a "corrente" o "Corrente". </p> <p>Questo modificatore può essere utilizzato solo nei filtri in modalità testo. Per ulteriori informazioni sulla modalità testo nei filtri, consulta <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Modificare un filtro utilizzando la modalità testo</a>.</p> </td> 
  </tr>   <tr valign="top"> 
   <td> </td> 
   <td> <p><strong>eq</strong> </p> </td> 
   <td> <p>Questo modificatore restituisce solo un valore esatto, <i>distinzione maiuscole/minuscole</i> corrisponde al valore cercato.</p> <p>Ad esempio, quando cerchi progetti completi, <code>eq CPL</code> restituisce tutti i progetti nello stato Completato. <code>eq CPL, CUR</code> non restituisce un risultato perché un progetto non può essere completo e corrente allo stesso tempo.</p> <p>Questo modificatore può essere utilizzato solo nei filtri in modalità testo. Per ulteriori informazioni sulla modalità testo nei filtri, consulta <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Modificare un filtro utilizzando la modalità testo</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td><strong>ne</strong> </td> 
   <td> <p>Questo è il <i>distinzione maiuscole/minuscole</i> opposto di <strong>eq</strong>. Restituisce solo risultati che non corrispondono esattamente al valore ricercato, oltre alle maiuscole e minuscole.</p> <p>Ad esempio: <b>ne</b> restituisce qualsiasi valore che non è uguale a "Current", ma non restituisce alcun valore che non è uguale a "current". </p> <p>Questo modificatore può essere utilizzato solo nei filtri in modalità testo. Per ulteriori informazioni sulla modalità testo nei filtri, consulta <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Modificare un filtro utilizzando la modalità testo</a>.<br></p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>ciin</strong> </p> </td> 
   <td> <p> Questo è il <i>senza distinzione tra maiuscole e minuscole</i> versione di <strong>in</strong>.</p> <p>Questo modificatore può essere utilizzato solo nei filtri in modalità testo. Per ulteriori informazioni sulla modalità testo nei filtri, consulta <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Modificare un filtro utilizzando la modalità testo</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cinotina</strong> </p> </td> 
   <td> <p>Questo è il <i>senza distinzione tra maiuscole e minuscole</i> versione di <strong>notin</strong>.</p> <p>Questo modificatore può essere utilizzato solo nei filtri in modalità testo. Per ulteriori informazioni sulla modalità testo nei filtri, consulta <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Modificare un filtro utilizzando la modalità testo</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> <p> </p> <p> </p> <p><strong>Uguale</strong> </p> </td> 
   <td> <p><strong>in</strong> </p> </td> 
   <td> <p>Questo modificatore consente di creare un elenco separato da virgole <i>distinzione maiuscole/minuscole</i> variabili da confrontare con un singolo attributo valutato in un filtro. L’intero elenco viene trattato come un’istruzione OR e restituisce tutti i risultati che soddisfano i criteri di una o più variabili.</p> <p>Ad esempio, durante la ricerca di progetti, utilizzando <code>in CUR, PLN, CPL</code> restituisce tutti i progetti nello stato Corrente, O Pianificazione, O Completo.</p> <p>Il modificatore incorporato <strong>Uguale</strong> corrisponde al modificatore di modalità testo di <strong>in</strong>. Ciò significa che è possibile scegliere Uguale a più valori per il campo.</p> <p>Ad esempio, è possibile scegliere un rapporto "Stato è uguale a Corrente, Pianificazione, Inattivo" ed è possibile visualizzare i progetti in uno qualsiasi di questi stati.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Not Equal</strong> </p> </td> 
   <td> <p><strong>notin</strong> </p> </td> 
   <td> <p>Questo è il <i>distinzione maiuscole/minuscole</i> opposto di <strong>in</strong>. Restituisce solo i risultati non inclusi nell'elenco specificato.</p> <p>Questo modificatore può essere utilizzato solo nei filtri in modalità testo. Per ulteriori informazioni sulla modalità testo nei filtri, consulta <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Modificare un filtro utilizzando la modalità testo</a>.</p> <p>Nota: <span>Se il campo per il quale si desidera filtrare dispone di più opzioni, verranno esclusi i risultati che contengono sia la scelta specificata, sia quella specificata ed eventuali altre scelte.</span> </p> </td> 
  </tr>
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>mi piace</strong> </p> </td> 
   <td> <p>Questo modificatore cerca parti di una <i>distinzione maiuscole/minuscole</i> stringa di testo simile a <strong>contiene</strong>. Tuttavia, <strong>mi piace</strong> consente di inserire caratteri jolly per suddividere il testo.</p> <p>Ad esempio, durante la ricerca di note, utilizzando <code>like %Current% %Dead%</code> restituisce qualsiasi nota che contiene la frase "Current to Dead" (Da corrente a morto). Non include note che contengono "Dead to Current". Ogni valore viene ricercato nell’ordine in cui è elencato. % rappresenta un carattere jolly per sostituire caratteri o segmenti di testo. Un carattere di sottolineatura può essere utilizzato anche per un singolo carattere jolly, ad esempio <code>like Project_</code> che restituisce sia "Project" che "Projects". Se intendi utilizzare un’ <strong>mi piace</strong> o <strong>clike</strong> modificatore nel filtro, si consiglia di evitare i caratteri % o _ nei nomi dei campi dati personalizzati, nei valori delle opzioni dei parametri o in altri nomi di oggetto.</p><p>Questo modificatore può essere utilizzato solo nei filtri in modalità testo. Per ulteriori informazioni sulla modalità testo nei filtri, consulta <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Modificare un filtro utilizzando la modalità testo</a>.</p> </td> 
  </tr>  
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cilike</strong> </p> </td> 
   <td> <p>Questo è il <i>senza distinzione tra maiuscole e minuscole</i> versione di <strong>mi piace</strong>. Ad esempio: <code>cilike %Current% %Dead%</code> restituisce tutte le note che contengono <code>Current to Dead</code> o <code>current to dead</code>.</p> <p>Questo modificatore può essere utilizzato solo nei filtri in modalità testo. Per ulteriori informazioni sulla modalità testo nei filtri, consulta <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Modificare un filtro utilizzando la modalità testo</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td><strong>Non esiste</strong> </td> 
   <td><strong>NOTEXISTS</strong> </td> 
   <td> <p>Questo modificatore viene utilizzato solo con filtri complessi in un'istruzione EXISTS. Questi filtri si riferiscono solo ai seguenti oggetti: </p> 
    <ul> 
     <li>Oggetti che si estendono su più livelli nella gerarchia degli oggetti </li> 
     <li>Oggetti mancanti </li> 
    </ul> <p>Per informazioni sulla creazione di filtri complessi tramite istruzioni EXISTS, consulta l’articolo <a href="../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md">Creare filtri in modalità testo complessi utilizzando le istruzioni EXISTS</a>. Questo è l'unico modificatore utilizzato nelle istruzioni EXISTS.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Maggiore di</strong> </p> </td> 
   <td> <p><strong>gt</strong> </p> </td> 
   <td> <p>Questa opzione consente di cercare tutti i risultati con un valore maggiore di quello immesso, escluso il valore immesso.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Minore di</strong> </p> </td> 
   <td> <p><strong>lt</strong> </p> </td> 
   <td> <p>Consente di cercare tutti i risultati con un valore inferiore a quello immesso, escluso il valore immesso.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Maggiore di uguale</strong> </p> </td> 
   <td> <p><strong>gte</strong> </p> </td> 
   <td> <p>Consente di cercare tutti i risultati con valori maggiori o uguali al valore immesso.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Less Than Equal</strong> </p> </td> 
   <td> <p><strong>lte</strong> </p> </td> 
   <td> <p>Consente di cercare tutti i risultati con un valore minore o uguale al valore immesso.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Tra</strong> </p> </td> 
   <td> <p><strong>tra</strong> </p> </td> 
   <td> <p>Fornisce due valori di campo obbligatori e cerca tutti i risultati compresi nell'intervallo di entrambi i campi, inclusi i valori immessi.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notbetween</strong> </p> </td> 
   <td> <p>Questo è l'inverso di <strong>tra</strong>. Fornisce due campi valore obbligatori e cerca tutti i risultati al di fuori dell’intervallo di entrambi i campi, inclusi i valori immessi.</p> <p>Questo modificatore può essere utilizzato solo nei filtri in modalità testo. Per ulteriori informazioni sulla modalità testo nei filtri, consulta <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Modificare un filtro utilizzando la modalità testo</a>.</p> </td> 
  </tr>

</tbody> 
</table>
