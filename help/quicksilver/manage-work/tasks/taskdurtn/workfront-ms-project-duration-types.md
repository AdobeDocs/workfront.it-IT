---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: Tipi di durata nei progetti Adobe Workfront e Microsoft
description: I tipi di durata disponibili in Adobe Workfront sono diversi dai loro omologhi in Progetto Microsoft, denominati Tipi di task. Questo può generare confusione durante l’esportazione o l’importazione di progetti tra Workfront e Microsoft Project.
author: Alina
feature: Work Management
exl-id: 986ecf91-693d-4ee1-bc56-355a2819ae41
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 2%

---

# Tipi di durata nei progetti Adobe Workfront e Microsoft

I tipi di durata disponibili in Adobe Workfront sono diversi dai loro omologhi in Progetto Microsoft, denominati Tipi di task. Questo può generare confusione durante l’esportazione o l’importazione di progetti tra Workfront e Microsoft Project.

Per informazioni sull’importazione e l’esportazione di progetti tra Workfront e Microsoft Project, consulta i seguenti articoli:

* [Esportare un progetto in un progetto Microsoft](../../../manage-work/projects/manage-projects/export-project-to-ms-project.md)
* [Importare un progetto da un progetto Microsoft](../../../manage-work/projects/create-projects/import-project-from-ms-project.md)

## Tipi di durata nei progetti Workfront e Microsoft

Workfront ha quattro tipi di durata delle attività:

* Semplice
* Impegno Aggiuntivo
* Lavoro Calcolato
* Incarico Calcolato

Per informazioni, consulta [Panoramica del tipo di durata e durata dell’attività](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

Questi tipi di durata non sono riconosciuti dal progetto Microsoft. Al momento, il progetto Microsoft dispone di tre tipi di attività simili a quelli di durata in Workfront:

* Unità fisse
* Lavoro fisso
* Durata fissa

## Il tipo di durata cambia quando si esporta da Workfront a MS Project

Quando si esportano progetti da Workfront a Microsoft Project, le attività basate su sforzo diventano lavoro fisso. Il lavoro semplice calcolato e l&#39;assegnazione calcolata diventano unità fisse.

## Il tipo di durata cambia quando si importa da MS Project a Workfront

Quando si importano progetti da Microsoft Project in Workfront, le unità fisse diventano basate sullo sforzo. Lavoro fisso e Durata fissa ricevono il tipo di durata predefinito selezionato dall&#39;amministratore Workfront per il sistema in uso. Per informazioni, consulta [Configurare le preferenze relative alle attività e ai problemi a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

<!--
<note type="warning">
When a task has Calculated Work as the Duration Type and the default Duration Type in Setup is set as Calculated Assignment, then MS Project assignment allocations will be lost during the import.
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(drafting this because it is misleading)
</MadCap:conditionalText>
</note>
-->
