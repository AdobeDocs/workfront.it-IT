---
product-area: projects
navigation-topic: issue-information
title: Utilizza "opTask" e "issue" quando si fa riferimento a problemi
description: Il nome di un problema viene visualizzato come opTask nel database di Adobe Workfront. Anche se ci sono casi in cui è necessario utilizzare il nome del campo problema per fare riferimento a problemi, la maggior parte delle volte è necessario utilizzare il nome del campo opTask invece di problema quando si fa riferimento a problemi.
author: Alina
feature: Work Management
exl-id: 91107c04-616c-49b2-aa78-10e373d11f6b
source-git-commit: 813b97ee0979e29a90293d9ddaba12a33c99f64d
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 0%

---

# Utilizza &quot;opTask&quot; e &quot;issue&quot; quando si fa riferimento a problemi

Il nome di un problema viene visualizzato come `opTask` nel database di Adobe Workfront. Anche se in alcuni casi è necessario utilizzare il `issue` nome del campo per fare riferimento ai problemi, la maggior parte delle volte è necessario utilizzare il `opTask` nome campo invece di `issue` quando si fa riferimento a problemi.

Per ulteriori informazioni sull&#39;aspetto degli oggetti nel database di Workfront, vedere [API Explorer](https://developer.adobe.com/workfront/api-explorer/).

## `opTask` nome file

Utilizza il `opTask` nome del campo quando si fa riferimento a problemi nei seguenti contesti:

* Quando crei un rapporto personalizzato in modalità testo per i problemi e desideri fare riferimento ai problemi in viste, filtri, raggruppamenti o prompt.

   Per ulteriori informazioni sull’utilizzo della modalità testo in un rapporto, consulta [Panoramica sulla modalità testo](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

<!--* When you pull information about issues using our API.  
  For more information about the Workfront API, see [Adobe Workfront API](../../../wf-api/workfront-api.md)-->

* Quando aggiorni i campi del problema in un foglio di importazione dati Kick-Start.

   Per ulteriori informazioni sull’importazione di dati in Workfront tramite Kick-Start, consulta [Importare dati in Adobe Workfront utilizzando un modello di avvio](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

## `issue` nome campo

Utilizza il `issue` nome del campo per fare riferimento a problemi nei seguenti contesti:

* Quando si fa riferimento a problemi in una raccolta utilizzando la modalità testo in un rapporto.
* Quando si fa riferimento a una raccolta di problemi utilizzando l&#39;API Workfront.

Per informazioni sul reporting sulle raccolte, consulta [Fare riferimento alle raccolte in un rapporto](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

<!--
<note type="tip">
For information about how issues appear in a collection, see the
<a href="https://developer.adobe.com/workfront/api-explorer/" target="_blank">API Explorer</a> and select the API Unsupported option from the upper-right corner of the page.
<br>(NOTE: Drafted because this might not be needed.)
</note>
-->
