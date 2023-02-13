---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Panoramica della data di completamento effettivo del progetto
description: I progetti, le attività e i problemi hanno una data di completamento effettiva in Adobe Workfront. Data in cui il progetto, l’attività o il problema sono stati contrassegnati come completati.
author: Alina
feature: Work Management
exl-id: 0baba359-a61d-43d7-8336-1f45c7f34374
source-git-commit: 3a3dc541219706e3f6a4700889db344c110838bb
workflow-type: tm+mt
source-wordcount: '489'
ht-degree: 0%

---

# Panoramica della data di completamento effettivo del progetto

I progetti, le attività e i problemi hanno una data di completamento effettiva in Adobe Workfront. Data in cui il progetto, l’attività o il problema sono stati contrassegnati come completati.

## Date di completamento effettive

La data di completamento effettivo rappresenta la data e l&#39;ora effettive al completamento del lavoro. Quando un&#39;attività o un problema viene contrassegnato come Fine o Completa, Workfront imposta automaticamente la data della modifica dello stato dell&#39;elemento come Data di completamento effettiva dell&#39;attività o del problema. Se tale data non riflette in modo accurato quando l&#39;attività o il problema è stato effettivamente completato, è possibile modificare manualmente la data di completamento effettivo.

Ad esempio, è possibile contrassegnare un’attività o un problema Fine lunedì, ma si sa che il lavoro è stato completato il venerdì precedente. Dopo aver contrassegnato l&#39;attività o il problema come Fine, è possibile quindi aggiornare manualmente la data di completamento effettivo dell&#39;attività o del problema alla data del venerdì precedente per riflettere il completamento effettivo.

Non è possibile modificare manualmente la data di completamento effettivo di un progetto, ma è possibile modificare manualmente lo stato di un progetto che può attivare una modifica alla data di completamento effettivo.

La data di completamento effettivo di un progetto viene impostata nei seguenti modi:

* Aggiornando manualmente lo stato del progetto: se la modalità di completamento del progetto è impostata su Manuale e lo stato del progetto viene modificato manualmente in Completato, viene attivata la data di completamento effettivo del progetto da aggiornare alla data e all&#39;ora in cui viene modificato lo stato.
* Automaticamente, al completamento dell&#39;ultima attività del progetto: se la modalità di completamento del progetto è impostata su Automatico e si contrassegna l&#39;ultima attività come Completa o si aggiorna la data di completamento effettivo dell&#39;ultima attività, viene aggiornata anche la data di completamento effettivo del progetto.

   Per informazioni sull&#39;impostazione della modalità di completamento di un progetto, vedere l&#39;articolo [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md).

   >[!NOTE]
   >
   >Workfront utilizza la data di completamento effettivo dell&#39;attività del progetto che è stata completata per ultima come data di completamento effettivo per l&#39;intero progetto.

Un amministratore di Workfront o di gruppo determina se Workfront utilizza la data odierna o la data di completamento pianificata di un&#39;attività o un problema quando questi sono impostati su Completa o Chiuso. Per informazioni sull&#39;impostazione delle preferenze per le attività e i problemi, consulta [Configurare le preferenze relative alle attività e ai problemi a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

<!--this statement is confusing, not sure what it is referring to, so I am drafting this for now: The value for the Actual Completion Date is always what is considered the current date and time.-->



## Individua date di completamento effettive

La data di completamento effettiva si trova nelle seguenti aree di Workfront:

* Aree Dettagli progetto, attività e problema
* Modificare le caselle Progetto, Attività e Problema
* Area Aggiornamenti di progetto, task e problemi come aggiornamento del sistema.
* Elenchi di progetti, attività o problemi o rapporti.

Per ulteriori informazioni sulla creazione di rapporti, consulta l’articolo [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
