---
product-area: projects
navigation-topic: issue-information
title: Usa "opTask" e "issue" quando si fa riferimento a problemi
description: Il nome di un problema viene visualizzato come opTask nel database Adobe Workfront. Anche se in alcuni casi è necessario utilizzare il nome del campo del problema per fare riferimento a problemi, la maggior parte delle volte è necessario utilizzare il nome del campo opTask invece del problema quando si fa riferimento a problemi.
author: Alina
feature: Work Management
exl-id: 91107c04-616c-49b2-aa78-10e373d11f6b
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 0%

---

# Usa &quot;opTask&quot; e &quot;issue&quot; quando si fa riferimento a problemi

Il nome di un problema viene visualizzato come `opTask` nel database Adobe Workfront. Anche se in alcuni casi è necessario utilizzare il `issue` nome del campo per fare riferimento ai problemi, la maggior parte delle volte è necessario utilizzare il `opTask` nome campo anziché `issue` quando si fa riferimento a problemi.

Per ulteriori informazioni sulla modalità di visualizzazione degli oggetti nel database Workfront, consulta la [Esplora API](https://one.workfront.com/s/api-explorer).

## `opTask` nomefile

Utilizza la `opTask` nome del campo quando si fa riferimento a problemi nei seguenti contesti:

* Quando crei un rapporto personalizzato in modalità testo per i problemi e desideri fare riferimento a problemi relativi a viste, filtri, raggruppamenti o prompt.

   Per ulteriori informazioni sull’utilizzo della modalità testo in un rapporto, consulta [Panoramica della modalità testo](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

<!--* When you pull information about issues using our API.  
  For more information about the Workfront API, see [Adobe Workfront API](../../../wf-api/workfront-api.md)-->

* Quando si aggiornano i campi del problema in un foglio di importazione di dati Click-Start.

   Per ulteriori informazioni sull&#39;importazione di dati in Workfront tramite un avvio rapido, vedi [Importare dati in Adobe Workfront utilizzando un modello Click-Start](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

## `issue` nome campo

Utilizza la `issue` nome del campo per fare riferimento ai problemi nei seguenti contesti:

* Quando si fa riferimento a problemi in una raccolta utilizzando la modalità testo in un rapporto.
* Quando fai riferimento a una raccolta di problemi utilizzando l&#39;API Workfront.

Per informazioni sul reporting sulle raccolte, vedi [Riferimento alle raccolte in un rapporto](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

<!--
<note type="tip">
For information about how issues appear in a collection, see the
<a href="https://one.workfront.com/s/api-explorer" target="_blank">API Explorer</a> and select the API Unsupported option from the upper-right corner of the page.
<br>(NOTE: Drafted because this might not be needed.)
</note>
-->
