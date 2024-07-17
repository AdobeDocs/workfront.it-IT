---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: Tipi di durata nei progetti Adobe Workfront e Microsoft
description: I Tipi di durata disponibili in Adobe Workfront sono diversi dai corrispondenti in Microsoft Project, denominati Tipi di attività. A volte questo può creare confusione durante l’esportazione o l’importazione di progetti tra Workfront e Microsoft Project.
author: Alina
feature: Work Management
exl-id: 986ecf91-693d-4ee1-bc56-355a2819ae41
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 2%

---

# Tipi di durata nei progetti Adobe Workfront e Microsoft

I Tipi di durata disponibili in Adobe Workfront sono diversi dai corrispondenti in Microsoft Project, denominati Tipi di attività. A volte questo può creare confusione durante l’esportazione o l’importazione di progetti tra Workfront e Microsoft Project.

Per informazioni sull&#39;importazione e l&#39;esportazione di progetti tra Workfront e Microsoft Project, vedere gli articoli seguenti:

* [Esporta un progetto in Microsoft Project](../../../manage-work/projects/manage-projects/export-project-to-ms-project.md)
* [Importare un progetto da Microsoft Project](../../../manage-work/projects/create-projects/import-project-from-ms-project.md)

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
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(drafting this because it is misleading)
</MadCap:conditionalText>
</note>
-->
