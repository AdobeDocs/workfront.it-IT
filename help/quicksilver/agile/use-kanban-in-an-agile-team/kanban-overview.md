---
content-type: overview
product-area: agile-and-teams
navigation-topic: use-kanban-in-an-agile-team
title: Panoramica Kanban
description: Leggi questo articolo per comprendere meglio come funziona la bacheca Kanban.
author: Lisa
feature: Agile
exl-id: d7daa6c1-dae2-4e5c-a765-6a6ebdfaa331
source-git-commit: fa499d74df891441e729c32188e9b2f74e4ef5c0
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---

# Panoramica Kanban

<!-- Audited: 01/2024 -->

Le sezioni seguenti consentono di comprendere meglio come [!UICONTROL Kanban] funzioni della scheda.

Per una descrizione della K[!UICONTROL anban] metodologia, vedi [Creare un team agile](/help/quicksilver/agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

Se ti interessa migrare da un team agile [!UICONTROL Kanban] bacheca a [!DNL Workfront] [!UICONTROL Schede], vedi [Migra agile team [!UICONTROL Kanban] schede a [!DNL Workfront] schede madri](/help/quicksilver/agile/use-boards-agile-planning-tools/migrate-kanban-cards-to-boards.md).

## [!UICONTROL Kanban] layout e funzioni della scheda

Il [!UICONTROL Kanban] La bacheca è costituita dai seguenti elementi:

**Colonna backlog**: visualizza tutte le attività attualmente nel backlog. Questa colonna non viene visualizzata per impostazione predefinita. Per ulteriori informazioni sul backlog, tra cui come visualizzarlo sul [!UICONTROL Kanban] bacheca, vedi [Gestire il backlog agile](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

**Stati storia**: indica lo stato di avanzamento di un brano in base alla colonna di stato in cui si trova.

Per ulteriori informazioni, consulta [Aggiornare lo stato delle storie su [!UICONTROL Kanban] scheda](../../agile/use-kanban-in-an-agile-team/update-the-status-of-stories.md).

Gli stati delle storie possono essere personalizzati per il progetto modificando la vista agile, come descritto nella sezione [[!UICONTROL Creare o personalizzare una visualizzazione Agile]](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md#create-or-customize-an-agile-view) in [Creare o modificare le viste in [!DNL Adobe Workfront]](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

>[!NOTE]
>
>Per impostazione predefinita, nel Kanban Board vengono visualizzate un massimo di cinquanta schede, ma puoi fare clic su **[!UICONTROL Mostra altro]** per visualizzare schede aggiuntive.

## Relazione tra le sottoattività e i brani

Se un brano contiene sottoattività, non è possibile aggiornare alcuna informazione sul brano principale stesso, ad esempio punti/ore o percentuale di completamento. Inoltre, non è possibile spostare la storia attraverso [!UICONTROL Kanban] per aggiornarne lo stato. Piuttosto, qualsiasi modifica apportata alle sottoattività del brano viene riflessa sul brano. I punti o le ore del brano combinato per tutte le sottoattività determinano i punti o le ore del brano principale.

Ad esempio, se una storia ha una sola sottoattività valutata in 4 punti, anche la storia stessa ha 4 punti. Se modificate il valore del punto della sottoattività in 3, il valore del punto del brano padre viene modificato in 3. Se create un&#39;altra sottoattività sullo stesso brano e impostate il valore del punto per tale sottoattività su 4, il valore del punto del brano viene modificato su 7 in modo da riflettere il valore del punto combinato per entrambe le sottoattività.

La stessa logica si applica alle sottoattività di secondo livello (sottoattività delle sottoattività). Se una sottoattività include una o più sottoattività di secondo livello, la sottoattività viene calcolata in base alle sottoattività di secondo livello.

## Funzioni supportate

Quando utilizzi la bacheca Kanban, puoi effettuare le seguenti operazioni:

* [Aggiungere una sottoattività a un brano esistente in [!UICONTROL Kanban] scheda](../../agile/use-kanban-in-an-agile-team/add-a-subtask-to-an-existing-story.md)
* [Aggiungi attività o problemi esistenti al [!UICONTROL Kanban] scheda](../../agile/use-kanban-in-an-agile-team/add-existing-tasks-or-issues-to-the-kanban-board.md)
* [Assegnare utenti a un brano in [!UICONTROL Kanban] scheda](../../agile/use-kanban-in-an-agile-team/assign-users-to-a-story.md)
* [Aggiungi storie e problemi da [!UICONTROL Kanban] scheda](../../agile/use-kanban-in-an-agile-team/add-story-from-kanban-board.md)
* [Elimina storie o problemi da [!UICONTROL Kanban] scheda](../../agile/use-kanban-in-an-agile-team/delete-story-from-kanban-board.md)
* [Modifica informazioni brano](../../agile/use-kanban-in-an-agile-team/edit-story-information.md)
* [Filtra per utente sulla [!UICONTROL Kanban] scheda](../../agile/use-kanban-in-an-agile-team/filter-by-user.md)
* [Gestire il limite WIP (Work In Progress) per [!UICONTROL Kanban] scheda](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md)
* [Riordina le storie su [!UICONTROL Kanban] scheda](../../agile/use-kanban-in-an-agile-team/reorder-stories-on-the-kanban-board.md)
* [Aggiornare lo stato delle storie su [!UICONTROL Kanban] scheda](../../agile/use-kanban-in-an-agile-team/update-the-status-of-stories.md)
* [Utilizza i flag sulle storie in [!UICONTROL Kanban] scheda](../../agile/use-kanban-in-an-agile-team/use-flags-on-stories.md)
* [Aggiungi il backlog al [!UICONTROL Kanban] scheda](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md)
