---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: Raggruppare un report per un campo personalizzato a selezione multipla
description: Puoi eseguire il raggruppamento in base al valore in un campo personalizzato a selezione multipla in un rapporto di Adobe Workfront solo utilizzando la modalità testo.
author: Nolan
feature: Reports and Dashboards
exl-id: 530dff59-0d4c-490e-b464-1d3bb1d0f36f
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '518'
ht-degree: 0%

---

# Raggruppare un rapporto per un campo personalizzato a selezione multipla

<!--Audited: 10/2024-->

Puoi eseguire il raggruppamento in base al valore in un campo personalizzato a selezione multipla in un rapporto di Adobe Workfront solo utilizzando la modalità testo.

Di seguito sono riportati alcuni esempi di campi personalizzati a selezione multipla:

* Checkboxe
* Menu a discesa a selezione multipla

Per informazioni sull&#39;utilizzo della modalità testo, vedere l&#39;articolo [Panoramica della modalità testo](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Considerazioni durante il raggruppamento per un campo personalizzato a selezione multipla

* Non è possibile tracciare un report che utilizza un raggruppamento in modalità testo. È necessario creare un campo calcolato aggiuntivo che faccia riferimento al campo personalizzato a selezione multipla per tracciare il rapporto anche in base al valore del campo personalizzato a selezione multipla.

  Per ulteriori informazioni, vedere [Tracciare un report in base a un campo personalizzato a selezione multipla](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/chart-report-by-multi-select-custom-field.md).
* Gli elementi con una delle scelte selezionate vengono conteggiati una sola volta.

  Ad esempio, se si dispone di un campo personalizzato Casella di controllo con le opzioni Scelta 1 e Scelta 2 e si allega il modulo alle attività, le attività con le opzioni Scelta 1 e Scelta 2 selezionate vengono raggruppate separatamente dalle attività con la sola scelta 1 o Scelta 2 selezionate.


## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> 
    <p>Nuovo:</p>
   <ul><li><p>Collaboratore per modificare un filtro </p></li>
   <li><p>Standard per modificare un rapporto</p></li> </ul>

<p>Corrente:</p>
   <ul><li><p>Richiesta di modifica di un filtro </p></li>
   <li><p>Pianificare la modifica di un rapporto</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari per modificare un rapporto</p> <p>Modificare l’accesso a Filtri, Viste, Raggruppamenti per modificare un filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Raggruppare un rapporto per più campi personalizzati selezionati

Per poter raggruppare in base a un campo personalizzato a selezione multipla, è necessario disporre dei seguenti prerequisiti:

* Crea il campo personalizzato a selezione multipla in un modulo personalizzato.\
  Per informazioni sulla creazione di moduli personalizzati e sull&#39;aggiunta di campi personalizzati, vedere l&#39;articolo [Creare un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

* Allegare il modulo personalizzato agli oggetti.
* Compila il campo personalizzato a selezione multipla con un valore su ciascun oggetto.

Per raggruppare in base a un campo personalizzato a selezione multipla in un rapporto:

1. Crea un rapporto o modificane uno esistente in cui desideri aggiungere un raggruppamento per un campo personalizzato a selezione multipla.\
   Per informazioni sulla creazione di report, vedere l&#39;articolo [Creare un report personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Fai clic su **Azioni report**, quindi su **Modifica**.
1. Selezionare la scheda **Raggruppamenti**.
1. Fare clic su **Passa alla modalità testo**.

1. Selezionare il testo nella casella **Raggruppa per** e sostituirlo con il seguente codice:

   <pre>
   group.0.displayname=Nome campo personalizzato a selezione multipla
   group.0.valueexpression={DE:Nome campo personalizzato a selezione multipla}
   group.0.valueformat=HTML
   group.0.textmode=true
   </pre>

1. Sostituisci &quot;Nome campo personalizzato a selezione multipla&quot; con il nome effettivo del campo personalizzato a selezione multipla, come visualizzato nell’istanza di Workfront.
1. Fare clic su **Salva e chiudi**.

   Gli oggetti nel report sono raggruppati in base ai valori del campo personalizzato a selezione multipla.

   ![Raggruppamento del campo a selezione multipla](assets/grouping-by-multi-select-field-text-mode-ui-example.png)

   I nomi dei raggruppamenti del rapporto sono i nomi del campo personalizzato a selezione multipla seguiti dai valori selezionati nel campo.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Chart a report by multi-select Custom Fields</h2>
<p>(NOTE: this moved to its own article, linked in the Note above!)</p>
<p>You cannot build a chart in a report by referencing a multi-select custom field. Instead, you can create a calculated field that records the values of the multi-select custom field on a given object and group by the calculated field.&nbsp;</p>
<ul>
<li><a href="#build-a-calculated-custom-field-that-references-a-multi-select-custom-field" class="MCXref xref">Build a calculated custom field that references a multi-select custom field</a> </li>
<li><a href="#build-a-chart-that-references-a-calculated-custom-field" class="MCXref xref">Build a chart that references a calculated custom field</a> </li>
</ul>
<p><strong>Build a calculated custom field that references a multi-select custom field</strong></p>
<p>To be able to build a calculated field that references a multi-select custom field, you must have the following prerequisites:</p>
<ul>
<li>Build the multi-select custom field in a custom form.<br>.</li>
<li>Attach the custom form to objects.</li>
<li>Populate the multi-select custom field with a value on each object.</li>
</ul>
<p>To build the calculated custom field that references the multi-select custom field:</p>
<ol>
<li value="1">Create a custom form, or edit an existing one.<br>.</li>
<li value="2">Click<strong>Add a Field</strong>, then <strong>Calculated</strong> to add the multi-select custom field to the form.</li>
<li value="3">In the <strong>Label</strong> box, name the new calculated field to indicate that it references the multi-select custom field.<br>For example: "Calculated Multi-select Field."</li>
<li value="4"> <p>In the <strong>Calculation</strong> box, enter the following code:</p><pre>{DE:Multi-select Custom Field}</pre> <p> <img src="assets/calculated-multi-select-custom-field-350x201.png" style="width: 350;height: 201;"> <br> </p> </li>
<li value="5">Replace "Multi-select Custom Field" with the actual name of your multi-select custom field, as it appears in Workfront.</li>
<li value="6"> <p>(Optional) If the multi-select custom field is already on this form and if this form is already attached to objects, enable the <strong>Update previous calculations</strong>&nbsp;option.</p> <p>This ensures that the new field is automatically populated with the value from the multi-select custom field as it is added to the forms attached to the objects already.</p> </li>
<li value="7">Click <strong>Done</strong>.</li>
<li value="8">Click <strong>Save +Close</strong>.</li>
</ol>
<p><strong>Build a chart that references a calculated custom field</strong></p>
<ol>
<li value="1"> Go to the report where you want to add the chart for the calculated field that references the multi-select custom field. </li>
<li value="2"> (Optional) To ensure that all the calculated fields that you want to chart by are populated with values, select all the objects in your report, then click <strong>Edit</strong>. </li>
<li value="3"> <p> (Optional and conditional) Enable the <strong>Recalculate Custom Expressions</strong> field, then click <strong>Save Changes</strong>.</p> <p> <img src="assets/recalculate-custom-expressions-350x259.png" style="width: 350;height: 259;"> <br> </p> </li>
<li value="4"> Click <strong>Report Actions</strong>, then <strong>Edit</strong>. </li>
<li value="5">Select the <strong>Groupings</strong> tab, then click <strong>Add Grouping</strong>. </li>
<li value="6">Add the<strong>Calculated Multi-select Field</strong> you created as your grouping. </li>
<li value="7"> <p>Select the <strong>Chart</strong> tab, and add a chart to your report.</p> <p>For information about adding a chart to a report, see the section <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md#add-a-chart" class="MCXref xref">Add a chart to a report</a> in the article <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Create a custom report</a>. </p> </li>
<li value="8">Select the <strong>Calculated Multi-select Field</strong> as one of the fields to display in the chart. </li>
<li value="9"> <p>Click <strong>Save + Close</strong>.</p> <p>The report displays the results grouped by the Calculated Multi-select Field in a chart. </p> </li>
</ol>
</div>
-->
