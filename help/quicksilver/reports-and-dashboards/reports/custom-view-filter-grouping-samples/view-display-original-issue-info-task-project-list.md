---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Visualizzazione: visualizzazione delle informazioni originali sui problemi in elenchi di attività o progetti"
description: Dopo aver convertito il problema nelle attività e nei progetti dell’elenco, è possibile visualizzare le informazioni del problema originale in una visualizzazione degli elenchi di attività e progetti.
author: Nolan
feature: Reports and Dashboards
exl-id: 235156b6-a9b6-484e-b126-54874da705c8
source-git-commit: 6405c01c8b1d842a4175f9caa18a7ed31316a3a1
workflow-type: tm+mt
source-wordcount: '134'
ht-degree: 5%

---

# Visualizza: visualizza le informazioni originali sui problemi negli elenchi di attività o progetti

Dopo aver convertito il problema in attività e progetti dell’elenco, puoi visualizzare le seguenti informazioni del problema originale in una visualizzazione degli elenchi di attività e progetti:

* Nome problema convertito
* Data voce problema convertito
* Nome del mittente del problema convertito

Per informazioni sulla creazione di una visualizzazione mediante il generatore di report standard, vedere [Panoramica delle visualizzazioni in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

![task_and_project_list_with_original_issue_info.png](assets/task-and-project-list-with-original-issue-info-350x59.png)

Per ulteriori informazioni sull&#39;inserimento di informazioni aggiuntive sui problemi negli elenchi delle attività e dei progetti, vedere anche [Visualizza: dettagli problemi di origine per attività e progetti](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-originating-issue-details-tasks-projects.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: no longer needed - all fields are now in the UI</p>
<p>Applying this view is identical for tasks and projects.</p>
<p>To apply this view to a task list:</p>
<ol>
<li value="1">Go to a list of tasks which have been converted from issues</li>
<li value="2">From the <strong>View</strong> drop-down menu, select <strong>New View</strong>.</li>
<li value="3">In the<strong>Column Preview</strong> area, eliminate all columns except for one.</li>
<li value="4">Click the header of the remaining column, then click<strong>Switch to Text Mode</strong>.</li>
<li value="5">Mouse over the text mode area, and click <strong>Click to edit text</strong>.</li>
<li value="6"> <p>Remove the text you find in the <strong>Text Mode</strong> box, and replace it with the following code:</p>
<div class="codeSnippet">
<a class="codeSnippetCopyButton" role="button">Copy</a>
<div class="codeSnippetBody" data-mc-continue="False" data-mc-line-number-start="1" data-mc-use-line-numbers="False">
<pre><code>column.0.descriptionkey=name<br>column.0.isInlineEditable=false<br>column.0.link.linkproperty.20.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.querysort=name<br>column.0.section=0<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.displayname=Converted Issue Name<br>column.1.linkedname=convertedOpTask<br>column.1.textmode=true<br>column.1.valuefield=convertedOpTaskName<br>column.1.valueformat=HTML<br>column.2.displayname=Converted Issue Entry Date<br>column.2.textmode=true<br>column.2.valuefield=convertedOpTaskEntryDate<br>column.2.valueformat=HTML<br>column.3.displayname=Originator Name<br>column.3.textmode=true<br>column.3.valuefield=convertedOpTaskOriginator:name<br>column.3.valueformat=HTML</code></pre>
</div>
</div> </li>
<li value="7"> Click <strong>Save View</strong>. </li>
</ol>
</div>
-->
