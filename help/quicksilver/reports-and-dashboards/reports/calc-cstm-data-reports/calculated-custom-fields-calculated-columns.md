---
content-type: overview
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Campi personalizzati calcolati e colonne calcolate
description: Scopri i dati personalizzati nei rapporti e nelle dashboard
author: Nolan
feature: Reports and Dashboards
exl-id: 17ac554d-0c90-4592-946e-a89f1784571d
source-git-commit: bcafa607da733b89747f6b448dd295d9b906d060
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 0%

---

# Campi personalizzati calcolati e colonne calcolate

Per aggregare diversi campi in Adobe Workfront e visualizzare tale valore aggregato in un nuovo campo, puoi effettuare le seguenti operazioni:

* Campo personalizzato calcolato in un modulo personalizzato\
  Per ulteriori informazioni sull’aggiunta di un campo personalizzato calcolato a un modulo personalizzato, consulta la sezione [Aggiungere un campo calcolato a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md#creating-calculated-custom-fields) nell’articolo [Aggiungere dati calcolati a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

* Una colonna calcolata in una visualizzazione\
  Per ulteriori informazioni sull&#39;utilizzo dei calcoli in una visualizzazione, vedere la sezione [Utilizzare la modalità testo nelle visualizzazioni](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md#using-text-mode-in-views) nell’articolo [Panoramica sugli usi comuni della modalità testo](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).

Sebbene si utilizzi la modalità testo per generare sia campi calcolati che colonne calcolate, la sintassi per la loro generazione è diversa. Per informazioni su come creare campi calcolati e colonne calcolate, consulta gli articoli elencati sopra. Per informazioni sulla diversa sintassi utilizzata nelle espressioni di dati calcolati, ad esempio campi e colonne personalizzati calcolati, vedere la sezione [Sintassi dei campi personalizzati calcolati rispetto alle colonne personalizzate calcolate](#syntax-of-calculated-custom-fields-vs-calculated-custom-columns-syntax) in questo articolo.

È possibile utilizzare gli stessi calcoli sia nei campi calcolati che in una colonna calcolata. Tuttavia, a seconda dello scopo di questi calcoli, potresti voler considerare la creazione di uno rispetto all’altro.

## Sintassi dei campi personalizzati calcolati rispetto alle colonne personalizzate calcolate

Anche se le funzioni utilizzate sono le stesse, la sintassi per la creazione di un&#39;espressione in un campo personalizzato calcolato può essere diversa da quella per la creazione di una colonna personalizzata calcolata.

Ad esempio:

* In un campo personalizzato, in un modulo personalizzato per le attività, puoi utilizzare quanto segue per generare il nome del progetto principale dell’attività a cui è allegato il modulo personalizzato:

  ```
  {project}.{name}
  ```

* In una colonna personalizzata di un report, utilizzare quanto segue per aggiungere una colonna personalizzata Nome progetto a un report attività:

  ```
  valuefield=project:name
  ```

  Oppure

  ```
  valueexpression={project}.{name}
  ```

  >[!TIP]
  >
  >La stessa sintassi si applica a tutti gli elementi di reporting in modalità testo in cui vengono utilizzate espressioni calcolate: viste, filtri, raggruppamenti, prompt.

Le differenze tra le due sintassi sono:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Campo personalizzato calcolato</td> 
   <td>Elemento di reporting personalizzato calcolato</td> 
  </tr> 
  <tr> 
   <td> <p>Utilizza il nome dei campi così come sono visualizzati nell’interfaccia di Workfront.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span>Esempio di nome di campo utilizzato in un campo personalizzato calcolato: <code>Planned Completion Date</code>.</p> </td> 
   <td> <p>Utilizzare il nome degli oggetti o dei campi così come sono visualizzati nel database di Workfront. I nomi degli oggetti e dei campi vengono scritti in lettere minuscole o camel, se sono nomi composti. </p> <p>Per un inventario di tutti gli oggetti e i campi di Workfront visualizzati nel database, vedere <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span>Esempio di nome del campo utilizzato in un elemento di reporting personalizzato calcolato: <code>plannedCompletionDate</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>Racchiudere i nomi dei campi tra parentesi graffe</td> 
   <td> <p>Non racchiudere i nomi dei campi tra parentesi quadre o parentesi quando li si utilizza in un <code>valuefield </code>linea.</p> <p>Racchiudi i nomi dei campi tra parentesi graffe quando li utilizzi in una <code>valueexpression</code> linea.</p> </td> 
  </tr> 
  <tr> 
   <td>Separa i campi per periodi</td> 
   <td> <p>Separa i campi con due punti quando li utilizzi in una <code>valuefield </code>linea</p> <p>Separa i campi per punti quando li utilizzi in una <code>valueexpression </code>linea. </p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori informazioni sulla sintassi da utilizzare in una colonna personalizzata calcolata, consulta [Panoramica sulla modalità testo](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Quando utilizzare i campi personalizzati calcolati

* Quando si desidera raggruppare i risultati aggregati in un report o visualizzare queste informazioni in un grafico
* Quando desideri aggregare i dati oltre l’aggregazione calcolata nel campo
* Se non sei preoccupato della tempestività dei dati, poiché i dati non vengono aggiornati e potrebbero cambiare nel tempo

## Azioni che attivano l’aggiornamento di un campo personalizzato calcolato

* Nella pagina principale di un oggetto, fare clic sull&#39;icona Altro ![](assets/more-icon.png), quindi clic su **Ricalcola espressioni**

* Modifica in blocco di più oggetti quando **Ricalcolare Espressioni Personalizzate** è abilitato
* Modifica di un modulo personalizzato durante **Aggiorna calcoli precedenti** è abilitato per il campo personalizzato calcolato

## Quando utilizzare le colonne calcolate in una visualizzazione

* Quando desideri che i dati in tempo reale siano disponibili in un rapporto.

  Le viste calcolate sono sempre nuove perché il calcolo viene effettuato quando il rapporto viene eseguito o la vista viene applicata.

* Quando non si prevede di raggruppare i risultati aggregati né di utilizzare queste informazioni in un grafico.
* Quando non prevedi di aggregare i dati oltre l’aggregazione calcolata nella colonna (i dati possono essere aggregati una sola volta).
* Se si desidera che il calcolo includa un riferimento alla data corrente utilizzando i caratteri jolly $$TODAY o $$NOW.

  >[!TIP]
  >
  >Non utilizzare questo riferimento nei campi personalizzati calcolati perché vengono ricalcolati solo quando l&#39;oggetto associato viene modificato. Questi tipi di calcoli non sono più aggiornati.

## Esempi di campi e colonne personalizzati calcolati

Per esempi di campi personalizzati calcolati, consulta [Dati personalizzati calcolati nei rapporti](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-data-reports.md).

Per esempi di colonne personalizzate calcolate nelle visualizzazioni, consulta i seguenti articoli:

* [Panoramica sugli usi comuni della modalità testo](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md)
* [Esempi di visualizzazione, filtro e raggruppamento personalizzati](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)
