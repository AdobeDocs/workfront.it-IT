---
product-area: projects
navigation-topic: issue-information
title: Utilizza "opTask" e "issue" quando si fa riferimento a Issues
description: Il nome di un problema viene visualizzato come opTask nel database di Adobe Workfront. Anche se ci sono casi in cui è necessario utilizzare il nome del campo problema per fare riferimento a problemi, la maggior parte delle volte è necessario utilizzare il nome del campo opTask invece di problema quando si fa riferimento a problemi.
author: Alina
feature: Work Management
exl-id: 91107c04-616c-49b2-aa78-10e373d11f6b
source-git-commit: 0542587bb3254dec5664de493c1c321528cf7f3e
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 0%

---

# Utilizza &quot;opTask&quot; e &quot;issue&quot; quando si fa riferimento a problemi

<!--Audited: 08/2025-->

Il nome di un problema viene visualizzato come `opTask` nel database di Adobe Workfront. Sebbene in alcuni casi sia necessario utilizzare il nome del campo `issue` per fare riferimento a problemi, nella maggior parte dei casi è necessario utilizzare il nome del campo `opTask` invece di `issue` quando si fa riferimento a problemi.

Per ulteriori informazioni sull&#39;aspetto degli oggetti nel database di Workfront, vedere [API Explorer](https://developer.adobe.com/workfront/api-explorer/).

## Nome campo `opTask`

Utilizza il nome del campo `opTask` quando si fa riferimento a problemi nei seguenti contesti:

* Quando crei un rapporto personalizzato in modalità testo per i problemi e desideri fare riferimento ai problemi in viste, filtri, raggruppamenti o prompt.

  Per ulteriori informazioni sull&#39;utilizzo della modalità testo in un report, vedere [Cenni preliminari sulla modalità testo](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

<!--* When you pull information about issues using our API.  
  For more information about the Workfront API, see [Adobe Workfront API](../../../wf-api/workfront-api.md)-->

* Quando aggiorni i campi del problema in un foglio di importazione dati Kick-Start.

  Per ulteriori informazioni sull&#39;importazione di dati in Workfront tramite Kick-Start, vedere [Importare dati in Adobe Workfront utilizzando un modello Kick-Start](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

## Nome campo `issue`

Utilizza il nome del campo `issue` per fare riferimento ai problemi nei seguenti contesti:

* Quando si fa riferimento a problemi in una raccolta utilizzando la modalità testo in un rapporto.
* Quando si fa riferimento a una raccolta di problemi utilizzando l&#39;API Workfront.

Per informazioni sul reporting sulle raccolte, vedere [Riferimento alle raccolte in un report](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

<!--
<note type="tip">
For information about how issues appear in a collection, see the
<a href="https://developer.adobe.com/workfront/api-explorer/" target="_blank">API Explorer</a> and select the API Unsupported option from the upper-right corner of the page.
<br>(NOTE: Drafted because this might not be needed.)
</note>
-->
