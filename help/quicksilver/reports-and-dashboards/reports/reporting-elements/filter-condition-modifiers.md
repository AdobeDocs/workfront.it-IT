---
product-area: reporting
navigation-topic: reporting-elements
title: Modificatori di filtri e condizioni
description: I modificatori di filtri e condizioni ti consentono di creare filtri e stabilire condizioni per la formattazione dei risultati del rapporto.
author: Nolan
feature: Reports and Dashboards
exl-id: 13e9d926-8a89-490e-aa7a-e6e8baf2a36b
source-git-commit: 6bd9dc626befc4dfa4054760e7ec7d677f6da6e5
workflow-type: tm+mt
source-wordcount: '1593'
ht-degree: 0%

---

# Modificatori di filtri e condizioni

<!-- Audited: 11/2024 -->

<!--(NOTE: Alina: This is temporary - Lilit is fixing this in a future story: NOTE If the field you are filtering for has multiple options, this filters out the results that contain only the choice you specify. If the field contains additional options including the one specified, those results are not filtered from the report. See this document and search for "not equal" for the link to the req doc: https://docs.google.com/document/d/1WA0zZ_wws-2qb908i53BFQ8zDwL3nPJHyIybtJvvnqU/edit)-->

I modificatori di filtri e condizioni ti consentono di creare filtri e stabilire condizioni per la formattazione dei risultati del rapporto.

Per ulteriori informazioni sulla creazione di filtri, vedere l&#39;articolo [Panoramica sui filtri](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Per ulteriori informazioni sull&#39;utilizzo della formattazione condizionale nelle visualizzazioni, vedere l&#39;articolo [Utilizzare la formattazione condizionale nelle visualizzazioni](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

## Modificatori di filtri e condizioni

Alcuni modificatori sono incorporati e puoi sceglierli da un menu a discesa all’interno del filtro o dell’istruzione di formattazione condizionale. Altri modificatori possono essere utilizzati solo nei filtri in modalità testo.

Per ulteriori informazioni sulla modalità testo, vedere [Panoramica della modalità testo](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Per un elenco dei modificatori incorporati dell&#39;intervallo di tempo, consulta l&#39;articolo [Filtrare i rapporti per intervalli di tempo](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/filter-reports-time-frames.md).

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
   <td> <p><strong>È Vuoto</strong> </p> </td> 
   <td> <p><strong>vuoto</strong> </p> </td> 
   <td> <p>Il campo esiste per l’oggetto, ma al momento non dispone di un valore.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Non È Vuoto</strong> </p> </td> 
   <td> <p><strong>notblank</strong> </p> </td> 
   <td> <p>Il campo per il quale stai filtrando esiste ed è stato assegnato un valore.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>null</strong> </p> </td> 
   <td> <p>Il campo è vuoto o non esiste. Ad esempio, si desidera cercare elementi senza un ID attività padre. Ciò significa che si desidera visualizzare solo le attività autonome. Il qualificatore per l'"ID attività padre" sarebbe <strong>null</strong>, poiché un'attività senza un ID (in questo caso l'elemento padre) non esiste. </p> <p>Questo modificatore può essere utilizzato solo nei filtri in modalità testo. Per ulteriori informazioni sulla modalità testo nei filtri, vedere <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Modificare un filtro utilizzando la modalità testo</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notnull</strong> </p> </td> 
   <td> <p>Il campo per il quale si sta filtrando esiste e contiene un valore diverso da null.</p> <p>Questo modificatore può essere utilizzato solo nei filtri in modalità testo. Per ulteriori informazioni sulla modalità testo nei filtri, vedere <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Modificare un filtro utilizzando la modalità testo</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Contiene</strong> </p> </td> 
   <td> <p><strong>cicontains</strong> </p> </td> 
   <td> <p>Questa è la versione di <strong>contains</strong> senza distinzione tra maiuscole e minuscole</i>. <i> Ad esempio: <code>cicontains inf</code> acquisisce qualsiasi valore contenente <code>Inf</code> o <code>inf</code>.</p> <p> <p>Nota: Adobe Workfront cerca la parola o la frase esatta specificata per ogni istruzione di filtro. Se ad esempio si cerca un progetto che contiene la frase <code>new project</code> nel nome, in Workfront non verranno visualizzati i progetti che contengono solo <code>new</code> o solo <code>project</code> o <code>new main project</code> nel nome. Il filtro trova solo i progetti il cui nome contiene la frase esatta <code>new project</code>.</p> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Does Not Contain</strong> </p> </td> 
   <td> <p><strong>cinotcontains</strong> </p> </td> 
   <td> <p>Versione di <strong>notcontains</strong> senza distinzione tra maiuscole e minuscole</i>.<i></p><p>Questo modificatore filtra gli elementi per i quali manca il valore specificato.</p> <p>Ad esempio, <code>does not contain inf</code> acquisisce qualsiasi elemento senza <code>Inf</code> o <code>inf</code> nel nome.</p> <p>Nota: quando viene applicato a campi che contengono più valori (ad esempio, una raccolta di note all’interno di un progetto), il filtro determina l’esclusione come segue:
<ul>
    <li>Se tutti gli elementi di una raccolta contengono il testo specificato, l'intero record viene escluso dai risultati.</li>
    <li>Se almeno un elemento della raccolta non contiene il testo specificato, il record rimane nei risultati.</li>
</ul>
 </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td> <p><strong>contiene</strong> </p> </td> 
   <td> <p> Cerca il testo <i>con distinzione tra maiuscole e minuscole</i> specificato in un'intera stringa di testo.</p> <p>Ad esempio, l'utilizzo di <code>contains Inf</code> acquisisce qualsiasi elemento contenente <code>Inf</code>, ad esempio la parola <code>Infinity.</code></p> <p>Questo modificatore può essere utilizzato solo nei filtri in modalità testo.Per ulteriori informazioni sulla modalità testo nei filtri, vedere <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Modificare un filtro in modalità testo</a>.</p> </td> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notcontains</strong> </p> </td> 
   <td> <p>Filtra gli elementi per i quali manca il valore <i>con distinzione tra maiuscole e minuscole</i> specificato.</p> <p>Ad esempio, <code>notcontains inf</code> acquisisce qualsiasi elemento senza <code>inf</code>, ma visualizza valori che contengono <code>Inf</code>.</p> <p>Questo modificatore può essere utilizzato solo nei filtri in modalità testo. Per ulteriori informazioni sulla modalità testo nei filtri, vedere <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Modificare un filtro utilizzando la modalità testo</a>.</p> </td> 
  </tr> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cieq</strong> </p> </td> 
   <td> <p>Opzione <i>senza distinzione tra maiuscole e minuscole</i> di <strong>eq</strong>. Restituisce solo una corrispondenza esatta del valore cercato.</p> <p>Ad esempio, durante la ricerca di un'attività con un nome specifico, <code>task name cieq test</code> trova le attività il cui nome è <code>Test</code>, <code>TEST</code> o <code>Test</code>, ma non trova un'attività con il nome <code>test 123.</code></p> <p>Durante la ricerca di uno stato, il modificatore <strong>cieq</strong> non è supportato. Utilizza il modificatore con distinzione tra maiuscole e minuscole, <strong>eq</strong>, per cercare uno stato.</p> <p>Questo modificatore può essere utilizzato solo nei filtri in modalità testo. Per ulteriori informazioni sulla modalità testo nei filtri, vedere <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Modificare un filtro utilizzando la modalità testo</a>.</p> </td>
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td><strong>cine</strong> </td> 
   <td> <p>Questa è l'opzione <i>senza distinzione tra maiuscole e minuscole</i> di <strong>ne</strong> ed è l'opposto del modificatore <b>cieq</b>. Restituisce solo risultati che non corrispondono esattamente al valore cercato, senza considerare il caso del valore.</p> <p>Ad esempio, <b>cine</b> restituisce qualsiasi valore che non sia uguale a "current" o "Current". </p> <p>Questo modificatore può essere utilizzato solo nei filtri in modalità testo. Per ulteriori informazioni sulla modalità testo nei filtri, vedere <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Modificare un filtro utilizzando la modalità testo</a>.</p> </td> 
  </tr>   <tr valign="top"> 
   <td> </td> 
   <td> <p><strong>eq</strong> </p> </td> 
   <td> <p>Questo modificatore restituisce solo una corrispondenza esatta <i>con distinzione tra maiuscole e minuscole</i> del valore cercato.</p> <p>Ad esempio, durante la ricerca di progetti completi, <code>eq CPL</code> restituisce tutti i progetti nello stato Completato. <code>eq CPL, CUR</code> non restituisce un risultato perché un progetto non può essere completo e corrente allo stesso tempo.</p> <p>Questo modificatore può essere utilizzato solo nei filtri in modalità testo. Per ulteriori informazioni sulla modalità testo nei filtri, vedere <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Modificare un filtro utilizzando la modalità testo</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td><strong>ne</strong> </td> 
   <td> <p><i>distinzione maiuscole/minuscole</i> di fronte a <strong>eq</strong>. Restituisce solo risultati che non corrispondono esattamente al valore ricercato, oltre alle maiuscole e minuscole.</p> <p>Ad esempio, <b>ne</b> restituisce valori che non sono uguali a "Corrente", ma non restituisce valori che non sono uguali a "corrente". </p> <p>Questo modificatore può essere utilizzato solo nei filtri in modalità testo. Per ulteriori informazioni sulla modalità testo nei filtri, vedere <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Modificare un filtro utilizzando la modalità testo</a>.<br></p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cin</strong> </p> </td> 
   <td> <p> Questa è la versione di <strong>in</strong> di <i>senza distinzione tra maiuscole e minuscole</i>.</p> <p>Questo modificatore può essere utilizzato solo nei filtri in modalità testo. Per ulteriori informazioni sulla modalità testo nei filtri, vedere <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Modificare un filtro utilizzando la modalità testo</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cinotina</strong> </p> </td> 
   <td> <p>Versione di <strong>notin</strong> di <i>senza distinzione tra maiuscole e minuscole</i>.</p> <p>Questo modificatore può essere utilizzato solo nei filtri in modalità testo. Per ulteriori informazioni sulla modalità testo nei filtri, vedere <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Modificare un filtro utilizzando la modalità testo</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> <p> </p> <p> </p> <p><strong>Uguale</strong> </p> </td> 
   <td> <p><strong>in</strong> </p> </td> 
   <td> <p>Questo modificatore consente di creare un elenco separato da virgole di <i>variabili con distinzione tra maiuscole e minuscole</i> da confrontare con un singolo attributo valutato in un filtro. L’intero elenco viene trattato come un’istruzione OR e restituisce tutti i risultati che soddisfano i criteri di una o più variabili.</p> <p>Ad esempio, durante la ricerca di progetti, l'utilizzo di <code>in CUR, PLN, CPL</code> restituisce tutti i progetti nello stato Corrente, O Pianificazione, O Completo.</p> <p>Il modificatore incorporato <strong>Equal</strong> corrisponde al modificatore della modalità testo di <strong>in</strong>. Ciò significa che è possibile scegliere Uguale a più valori per il campo.</p> <p>Ad esempio, è possibile scegliere un rapporto "Stato è uguale a Corrente, Pianificazione, Inattivo" ed è possibile visualizzare i progetti in uno qualsiasi di questi stati.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Diverso</strong> </p> </td> 
   <td> <p><strong>notin</strong> </p> </td> 
   <td> <p><i>distinzione maiuscole/minuscole</i> di fronte a <strong>in</strong>. Restituisce solo i risultati non inclusi nell'elenco specificato.</p> <p>Questo modificatore può essere utilizzato solo nei filtri in modalità testo. Per ulteriori informazioni sulla modalità testo nei filtri, vedere <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Modificare un filtro utilizzando la modalità testo</a>.</p> <p>Nota: <span>Se il campo per il quale si sta eseguendo il filtro include più opzioni, verranno esclusi i risultati che contengono sia la scelta specificata, sia quella specificata ed eventuali altre scelte.</span> </p> </td> 
  </tr>
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>mi piace</strong> </p> </td> 
   <td> <p>Questo modificatore cerca parti di una stringa di testo <i>con distinzione tra maiuscole e minuscole</i> in modo simile a <strong>contains</strong>. Tuttavia, <strong>like</strong> consente di inserire caratteri jolly per interrompere il testo.</p> <p>Ad esempio, durante la ricerca di note, l'utilizzo di <code>like %Current% %Dead%</code> restituisce qualsiasi nota contenente la frase "Corrente in inattivo". Non include note che contengono "Dead to Current". Ogni valore viene ricercato nell’ordine in cui è elencato. % rappresenta un carattere jolly per sostituire caratteri o segmenti di testo. Un carattere di sottolineatura può essere utilizzato anche per un singolo carattere jolly, ad esempio in <code>like Project_</code> che restituisce sia "Progetto" che "Progetti". Se intendi utilizzare un modificatore <strong>like</strong> o <strong>clike</strong> nel filtro, ti consigliamo di evitare % o _ caratteri nei nomi dei campi dati personalizzati, nei valori delle opzioni dei parametri o in altri nomi di oggetto.</p><p>Questo modificatore può essere utilizzato solo nei filtri in modalità testo. Per ulteriori informazioni sulla modalità testo nei filtri, vedere <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Modificare un filtro utilizzando la modalità testo</a>.</p> </td> 
  </tr>  
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cilike</strong> </p> </td> 
   <td> <p>Questa è la versione di <strong>like</strong> di <i>senza distinzione tra maiuscole e minuscole</i>. Ad esempio: <code>cilike %Current% %Dead%</code> restituisce tutte le note che contengono <code>Current to Dead</code> o <code>current to dead</code>.</p> <p>Questo modificatore può essere utilizzato solo nei filtri in modalità testo. Per ulteriori informazioni sulla modalità testo nei filtri, vedere <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Modificare un filtro utilizzando la modalità testo</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td><strong>Non Esiste</strong> </td> 
   <td><strong>NOTEXISTS</strong> </td> 
   <td> <p>Questo modificatore viene utilizzato solo con filtri complessi in un'istruzione EXISTS. Questi filtri si riferiscono solo ai seguenti oggetti: </p> 
    <ul> 
     <li>Oggetti che si estendono su più livelli nella gerarchia degli oggetti </li> 
     <li>Oggetti mancanti </li> 
    </ul> <p>Per informazioni sulla creazione di filtri complessi tramite istruzioni EXISTS, vedere l'articolo <a href="../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md">Creare filtri in modalità testo complessi utilizzando istruzioni EXISTS</a>. Questo è l'unico modificatore utilizzato nelle istruzioni EXISTS.</p> </td> 
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
   <td> <p><strong>Minore di uguale</strong> </p> </td> 
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
   <td> <p>Si tratta dell'inverso di <strong>between</strong>. Fornisce due campi valore obbligatori e cerca tutti i risultati al di fuori dell’intervallo di entrambi i campi, inclusi i valori immessi.</p> <p>Questo modificatore può essere utilizzato solo nei filtri in modalità testo. Per ulteriori informazioni sulla modalità testo nei filtri, vedere <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Modificare un filtro utilizzando la modalità testo</a>.</p> </td> 
  </tr>

</tbody> 
</table>
