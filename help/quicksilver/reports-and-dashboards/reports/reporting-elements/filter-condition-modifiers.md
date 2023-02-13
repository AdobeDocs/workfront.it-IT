---
product-area: reporting
navigation-topic: reporting-elements
title: Modificatori di filtri e condizioni
description: I modificatori di filtro e condizione consentono di creare filtri e stabilire le condizioni per la formattazione dei risultati del rapporto.
author: Lisa
feature: Reports and Dashboards
exl-id: 13e9d926-8a89-490e-aa7a-e6e8baf2a36b
source-git-commit: 442e0b8fde9e4acaa2686ccd292fb003f72be623
workflow-type: tm+mt
source-wordcount: '1556'
ht-degree: 1%

---

# Modificatori di filtri e condizioni

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: This is temporary - Lilit is fixing this in a future story: NOTE If the field you are filtering for has multiple options, this filters out the results that contain only the choice you specify. If the field contains additional options including the one specified, those results are not filtered from the report. See this document and search for "not equal" for the link to the req doc: https://docs.google.com/document/d/1WA0zZ_wws-2qb908i53BFQ8zDwL3nPJHyIybtJvvnqU/edit) </p>
-->

I modificatori di filtro e condizione consentono di creare filtri e stabilire le condizioni per la formattazione dei risultati del rapporto.

Per ulteriori informazioni sulla creazione dei filtri, consulta l’articolo [Panoramica sui filtri in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Per ulteriori informazioni sull&#39;utilizzo della formattazione condizionale nelle visualizzazioni, consulta l&#39;articolo [Utilizzare la formattazione condizionale nelle visualizzazioni](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

## Modificatori di filtri e condizioni

Per un elenco dei modificatori di intervalli di tempo incorporati, consulta l’articolo [Filtrare i rapporti per intervalli di tempo](../../../reports-and-dashboards/reports/creating-and-managing-reports/filter-reports-time-frames.md).

Alcuni modificatori sono incorporati e puoi sceglierli da un menu a discesa all’interno del filtro o dell’istruzione di formattazione condizionale. Altri modificatori possono essere utilizzati solo nei filtri in modalità testo. Per ulteriori informazioni sulla modalità testo, consulta [Panoramica della modalità testo](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

È possibile utilizzare i seguenti modificatori di condizioni nei filtri e nelle istruzioni di formattazione condizionale:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Modificatore incorporato</strong> </p> </th> 
   <th> <p><strong>Modificatore della modalità testo</strong> </p> </th> 
   <th> <p><strong>Descrizione</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr valign="top"> 
   <td> <p><strong>Blank</strong> </p> </td> 
   <td> <p><strong>Vuoto</strong> </p> </td> 
   <td> <p>Il campo esiste per l’oggetto ma al campo non è stato ancora assegnato un valore.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Not Blank</strong> </p> </td> 
   <td> <p><strong>non vuoto</strong> </p> </td> 
   <td> <p>Il campo a cui si sta filtrando esiste ed è stato assegnato un valore.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>null</strong> </p> </td> 
   <td> <p>Il campo è vuoto o non esiste. Ad esempio, per cercare gli elementi senza un ID attività padre. Ciò significa che desideri visualizzare solo le attività autonome. Il qualificatore per l'"ID attività padre" sarebbe <strong>null</strong>, poiché non esiste un’attività senza un ID (in questo caso l’elemento padre). </p> <p>Questo modificatore può essere utilizzato solo nei filtri in modalità testo. Per ulteriori informazioni sulla modalità testo nei filtri, consulta <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Modificare un filtro utilizzando la modalità testo</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notnull</strong> </p> </td> 
   <td> <p>Il campo a cui si sta filtrando esiste e contiene un valore diverso da null.</p> <p>Questo modificatore può essere utilizzato solo nei filtri in modalità testo. Per ulteriori informazioni sulla modalità testo nei filtri, consulta <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Modificare un filtro utilizzando la modalità testo</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Contiene</strong> </p> </td> 
   <td> <p><strong>cicontani</strong> </p> </td> 
   <td> <p>(Senza distinzione tra maiuscole e minuscole) Si tratta della versione senza distinzione tra maiuscole e minuscole di <strong>contiene</strong>. Ad esempio: "cicontains inf" acquisisce qualsiasi valore che contiene "Inf" o "inf".</p> <p> <p>Nota: Adobe Workfront cerca la parola o la frase esatta che si sta specificando per ogni istruzione di filtro. Ad esempio, se cerchi un progetto contenente la frase "nuovo progetto" nel nome, Workfront non visualizza i progetti il cui nome contiene solo "nuovo" o semplicemente "progetto" o "nuovo progetto principale". Il filtro trova solo i progetti con la frase esatta "nuovo progetto" nel nome.</p> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cieq</strong> </p> </td> 
   <td> <p>(Senza distinzione tra maiuscole e minuscole) Questa è l’opzione senza distinzione tra maiuscole e minuscole di <strong>eq</strong>. Restituisce solo una corrispondenza esatta del valore ricercato.</p> <p>Ad esempio, quando si cerca un'attività con un nome specifico, "task name cieq test" trova attività in cui il nome è "Test", "TEST" o "Test", ma non trova un'attività con il nome "test 123".</p> <p>Questo modificatore può essere utilizzato solo nei filtri in modalità testo. Per ulteriori informazioni sulla modalità testo nei filtri, consulta <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Modificare un filtro utilizzando la modalità testo</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>ciine</strong> </p> </td> 
   <td> <p>(Senza distinzione tra maiuscole e minuscole) Si tratta della versione senza distinzione tra maiuscole e minuscole di <strong>in</strong>.</p> <p>Questo modificatore può essere utilizzato solo nei filtri in modalità testo. Per ulteriori informazioni sulla modalità testo nei filtri, consulta <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Modificare un filtro utilizzando la modalità testo</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>ciliegina</strong> </p> </td> 
   <td> <p>Questa è la versione senza distinzione tra maiuscole e minuscole di <strong>like</strong>. Ad esempio: "cilike %Current% %Dead%" restituisce tutte le note che contengono "Current to Dead" o "current to Dead".</p> <p>Questo modificatore può essere utilizzato solo nei filtri in modalità testo. Per ulteriori informazioni sulla modalità testo nei filtri, consulta <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Modificare un filtro utilizzando la modalità testo</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cinotina</strong> </p> </td> 
   <td> <p>(Senza distinzione tra maiuscole e minuscole) Si tratta della versione senza distinzione tra maiuscole e minuscole di <strong>notina</strong>.</p> <p>Questo modificatore può essere utilizzato solo nei filtri in modalità testo. Per ulteriori informazioni sulla creazione di filtri utilizzando la modalità testo, consulta <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Modificare un filtro utilizzando la modalità testo</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td> <p><strong>contiene</strong> </p> </td> 
   <td> <p>(distinzione maiuscole/minuscole) Cerca il testo specificato in un'intera stringa di testo.</p> <p>Ad esempio, l’utilizzo di "contiene Inf" acquisisce qualsiasi elemento con "Inf", come la parola "Infinity".</p> <p>Questo modificatore può essere utilizzato solo nei filtri in modalità testo. Per ulteriori informazioni sulla modalità testo nei filtri, vedere <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Modificare un filtro utilizzando la modalità testo</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Non contiene</strong> </p> </td> 
   <td> <p><strong>cinotcontiene</strong> </p> </td> 
   <td> <p>(Senza distinzione tra maiuscole e minuscole) filtra gli elementi per i quali manca il valore specificato.</p> <p>Ad esempio, "non contiene inf" acquisisce nulla senza "Inf" o "inf" nel nome.</p> <p>Nota: <span>Se il campo a cui si sta filtrando dispone di più opzioni, vengono filtrati i risultati che contengono sia la scelta specificata, sia la scelta specificata ed eventuali opzioni aggiuntive.</span> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td><strong>Non esiste</strong> </td> 
   <td><strong>NOTESSISTI</strong> </td> 
   <td> <p>Questo modificatore viene utilizzato solo con filtri complessi in un'istruzione EXISTS. Questi filtri si riferiscono solo ai seguenti oggetti: </p> 
    <ul> 
     <li>Oggetti che si estendono su più livelli nella gerarchia degli oggetti </li> 
     <li>Oggetti mancanti </li> 
    </ul> <p>Per informazioni sulla creazione di filtri complessi utilizzando le istruzioni EXISTS, consulta l’articolo <a href="../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md">Creare filtri in modalità testo complessi utilizzando le istruzioni EXISTS</a>. Questo è l’unico modificatore utilizzato nelle istruzioni EXISTS.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> <p> </p> <p> </p> <p><strong>Equal (Case Insensitive)</strong> </p> </td> 
   <td> <p><strong>in</strong> </p> </td> 
   <td> <p>(Con distinzione tra maiuscole e minuscole) Questo modificatore consente di creare un elenco di variabili separate da virgola da confrontare con un singolo attributo valutato in un filtro. L’intero elenco viene trattato come un’istruzione OR e restituisce tutti i risultati che soddisfano i criteri di una o più variabili.</p> <p>Ad esempio, quando si cercano progetti, utilizzando "in CUR, PLN, CPL" vengono restituiti tutti i progetti che si trovano nello stato Current, OR Planning, OR Complete.</p> <p>Modificatore incorporato <strong>Uguale</strong> corrisponde al modificatore di modalità testo di <strong>in</strong>. Ciò significa che è possibile scegliere Uguale a più valori per il campo.</p> <p>Ad esempio, puoi scegliere "Stato uguale a corrente, pianificazione, morto" in un rapporto di progetto e visualizzare i progetti in uno qualsiasi di questi stati.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td> <p><strong>eq</strong> </p> </td> 
   <td> <p>(Con distinzione tra maiuscole e minuscole) restituisce solo una corrispondenza esatta del valore ricercato.</p> <p>Ad esempio, quando cerchi progetti completi, "eq CPL" restituisce tutti i progetti nello stato completo. "eq CPL, CUR" non restituisce un risultato perché un progetto non può essere completo e attuale allo stesso tempo.</p> <p>Questo modificatore può essere utilizzato solo nei filtri in modalità testo. Per ulteriori informazioni sull’utilizzo della modalità testo per creare i filtri, consulta <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Modificare un filtro utilizzando la modalità testo</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Maggiore di</strong> </p> </td> 
   <td> <p><strong>gt</strong> </p> </td> 
   <td> <p>Cerca tutti i risultati con un valore maggiore del valore inserito, senza includere il valore inserito.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>like</strong> </p> </td> 
   <td> <p>(distinzione maiuscole/minuscole) Cerca parti di una stringa di testo in modo simile a <strong>contiene</strong>. Tuttavia, <strong>like</strong> consente di inserire caratteri jolly per suddividere il testo.</p> <p>Ad esempio, quando si cercano le note, utilizzando "come %Current% %Dead%" viene restituita qualsiasi nota contenente la frase "Current to Dead". Non include le note contenenti "Dead to Current" (Morto a corrente). Ogni valore viene ricercato nell’ordine in cui è elencato. % rappresenta un carattere jolly per sostituire caratteri o segmenti di testo.</p> <p>Questo modificatore può essere utilizzato solo nei filtri in modalità testo. Per ulteriori informazioni sulla modalità testo nei filtri, consulta <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Modificare un filtro utilizzando la modalità testo</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Minore di</strong> </p> </td> 
   <td> <p><strong>lt</strong> </p> </td> 
   <td> <p>Cerca tutti i risultati con un valore inferiore a quello immesso, senza includere il valore inserito.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Greater Than Equal</strong> </p> </td> 
   <td> <p><strong>get</strong> </p> </td> 
   <td> <p>Cerca tutti i risultati con valori maggiori o uguali al valore inserito.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Less Than Equal</strong> </p> </td> 
   <td> <p><strong>lite</strong> </p> </td> 
   <td> <p>Cerca tutti i risultati con un valore minore o uguale al valore inserito.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Tra</strong> </p> </td> 
   <td> <p><strong>tra</strong> </p> </td> 
   <td> <p>Fornisce due valori di campo obbligatori e cerca tutti i risultati entro l’intervallo di entrambi i campi, inclusi i valori immessi.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>non contiene</strong> </p> </td> 
   <td> <p>Fa distinzione tra maiuscole e minuscole e filtra gli elementi per i quali manca il valore specificato.</p> <p>Ad esempio, "non contiene inf" acquisisce qualsiasi cosa con senza "inf", ma visualizza valori che contengono "Inf".</p> <p>Questo modificatore può essere utilizzato solo nei filtri in modalità testo. Per ulteriori informazioni sulla modalità testo nei filtri, consulta <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Modificare un filtro utilizzando la modalità testo</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>non</strong> </p> </td> 
   <td> <p>Questo è l'inverso di <strong>tra</strong>. Fornisce due campi di valori obbligatori e cerca tutti i risultati al di fuori dell’intervallo di entrambi i campi, inclusi i valori immessi.</p> <p>Questo modificatore può essere utilizzato solo nei filtri in modalità testo. Per ulteriori informazioni sulla modalità testo nei filtri, consulta <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Modificare un filtro utilizzando la modalità testo</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Not Equal</strong> </p> </td> 
   <td> <p><strong>notina</strong> </p> </td> 
   <td> <p>(Caso sensibile) Questo è l'opposto di <strong>in</strong>. Restituisce solo i risultati non inclusi nell'elenco specificato.</p> <p>Questo modificatore può essere utilizzato solo nei filtri in modalità testo. Per ulteriori informazioni sulla modalità testo nei filtri, consulta <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Modificare un filtro utilizzando la modalità testo</a>.</p> <p>Nota: <span>Se il campo a cui si sta filtrando dispone di più opzioni, vengono filtrati i risultati che contengono sia la scelta specificata, sia la scelta specificata ed eventuali opzioni aggiuntive.</span> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td><strong>ne</strong> </td> 
   <td> <p>(Caso sensibile) Questo è l'opposto di <strong>eq</strong>. Restituisce solo i risultati che non corrispondono esattamente al valore ricercato e corrisponde anche al caso del valore .</p> <p>Ad esempio: <b>ne</b> restituisce qualsiasi valore che non sia uguale a "Current" (Corrente), ma non restituisce alcun valore che non sia uguale a "current" (corrente). </p> <p>Questo modificatore può essere utilizzato solo nei filtri in modalità testo. Per ulteriori informazioni sulla modalità testo nei filtri, consulta <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Modificare un filtro utilizzando la modalità testo</a>.<br></p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td><strong>cina</strong> </td> 
   <td> <p>(Senza distinzione tra maiuscole e minuscole) Questa è l’opzione senza distinzione tra maiuscole e minuscole di <strong>ne</strong> ed è l'opposto del <b>cieq</b> modificatore. Restituisce solo risultati che non corrispondono esattamente al valore ricercato, senza tenere conto del caso del valore.</p> <p>Ad esempio: <b>cina</b> restituisce tutti i valori che non sono uguali a "current" o "Current". </p> <p>Questo modificatore può essere utilizzato solo nei filtri in modalità testo. Per ulteriori informazioni sulla modalità testo nei filtri, consulta <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Modificare un filtro utilizzando la modalità testo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
