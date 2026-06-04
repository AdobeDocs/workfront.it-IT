---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: Tipi di durata in Adobe Workfront e progetto di Microsoft
description: I Tipi di durata disponibili in Adobe Workfront sono diversi dai corrispondenti in Microsoft Project, denominati Tipi di attività. A volte questo può creare confusione durante l’esportazione o l’importazione di progetti tra Workfront e Microsoft Project.
author: Alina
feature: Work Management
exl-id: 986ecf91-693d-4ee1-bc56-355a2819ae41
TQID: https://experienceleague.adobe.com/avh0ZuYJpsf7Ed5HiWuLkxEA-0PD-1iFvzHmWvpDZiI
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b91c0848-76c4-4da4-8b81-3aade0518dd0id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 257
ht-degree: 11%

---

# Tipi di durata in Adobe Workfront e progetto di Microsoft

I Tipi di durata disponibili in Adobe Workfront sono diversi dai corrispondenti in Microsoft Project, denominati Tipi di attività. A volte questo può creare confusione durante l’esportazione o l’importazione di progetti tra Workfront e Microsoft Project.

Per informazioni sull&#39;importazione e l&#39;esportazione di progetti tra Workfront e Microsoft Project, vedere gli articoli seguenti:

* [Esporta un progetto in Microsoft Project](../../../manage-work/projects/manage-projects/export-project-to-ms-project.md)
* [Importare un progetto da progetto di Microsoft](../../../manage-work/projects/create-projects/import-project-from-ms-project.md)

## Tipi di durata nei progetti Workfront e Microsoft

In Workfront sono disponibili quattro tipi di durata attività:

* Semplice
* Impegno Aggiuntivo
* Lavoro Calcolato
* Incarico Calcolato

Per informazioni, vedere [Panoramica sulla durata e sul tipo di durata dell&#39;attività](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

Questi tipi di durata non sono riconosciuti da Microsoft Project. Attualmente, Microsoft Project dispone di tre tipi di attività simili ai tipi di durata in Workfront:

* Unità fisse
* Lavoro fisso
* Durata fissa

## Modifica del Tipo di Durata durante l’esportazione da Workfront a MS Project

Quando si esportano progetti da Workfront a Microsoft Project, le attività basate sulle risorse diventano lavoro fisso. Il lavoro semplice, il lavoro calcolato e l&#39;assegnazione calcolata diventano unità fisse.

## Modifica del Tipo di Durata durante l’importazione da MS Project a Workfront

Quando si importano progetti da Microsoft Project in Workfront, le Fixed Unit diventano Effort Driven. Lavoro fisso e Durata fissa ricevono il tipo di durata predefinito selezionato dall&#39;amministratore di Workfront per il sistema. Per informazioni, consulta [Configurare le preferenze per attività e problemi a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

<!--
<note type="warning">
When a task has Calculated Work as the Duration Type and the default Duration Type in Setup is set as Calculated Assignment, then MS Project assignment allocations will be lost during the import.
 
(drafting this because it is misleading)
 
</note>
-->
