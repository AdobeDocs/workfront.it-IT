---
product-area: projects
navigation-topic: issue-information
title: Utilizza "opTask" e "issue" quando si fa riferimento a Issues
description: Il nome di un problema viene visualizzato come opTask nel database di Adobe Workfront. Anche se ci sono casi in cui è necessario utilizzare il nome del campo problema per fare riferimento a problemi, la maggior parte delle volte è necessario utilizzare il nome del campo opTask invece di problema quando si fa riferimento a problemi.
author: Alina
feature: Work Management
exl-id: 91107c04-616c-49b2-aa78-10e373d11f6b
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/jrNMdSfyMO3MgzcxxKSNtrgzuY3e4ZNJpJ-JdvylJN4
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 257
ht-degree: 4%

---

# Utilizzare “opTask” e “problema” quando si fa riferimento ai problemi

<!--Audited: 08/2025-->

Il nome di un problema viene visualizzato come `opTask` nel database di Adobe Workfront. Sebbene in alcuni casi sia necessario utilizzare il nome del campo `issue` per fare riferimento a problemi, nella maggior parte dei casi è necessario utilizzare il nome del campo `opTask` invece di `issue` quando si fa riferimento a problemi.

Per ulteriori informazioni sull&#39;aspetto degli oggetti nel database di Workfront, vedere [API Explorer](https://developer.adobe.com/workfront/api-explorer/).

## Nome campo `opTask`

Utilizza il nome del campo `opTask` quando si fa riferimento a problemi nei seguenti contesti:

* Quando crei un rapporto personalizzato in modalità testo per i problemi e desideri fare riferimento ai problemi in viste, filtri, raggruppamenti o prompt.

  Per ulteriori informazioni sull&#39;utilizzo della modalità testo in un report, vedere [Cenni preliminari sulla modalità testo](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

<!--
* When you pull information about issues using our API.  
  For more information about the Workfront API, see [Adobe Workfront API](../../../wf-api/workfront-api.md)
  -->

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
