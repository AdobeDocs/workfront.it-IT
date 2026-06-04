---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Panoramica sulla data di completamento effettiva del progetto
description: I progetti, le attività e i problemi hanno una Data di completamento effettiva in Adobe Workfront. Si tratta della data in cui il progetto, l’attività o il problema sono stati contrassegnati come completati.
author: Alina
feature: Work Management
exl-id: 0baba359-a61d-43d7-8336-1f45c7f34374
TQID: https://experienceleague.adobe.com/MoATj74YM1zoW2SsIGrpKY0gc9dHRKjlDvnPfT-kk2s
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 490
ht-degree: 2%

---

# Panoramica sulla data di completamento effettiva del progetto

I progetti, le attività e i problemi hanno una Data di completamento effettiva in Adobe Workfront. Si tratta della data in cui il progetto, l’attività o il problema sono stati contrassegnati come completati.

## Date di completamento effettive

La data di completamento effettiva rappresenta la data e l&#39;ora effettive in cui il lavoro viene completato. Quando un’attività o un problema è contrassegnato come completato o completato, Workfront imposta automaticamente la data della modifica dello stato dell’elemento come data di completamento effettiva dell’attività o del problema. Se tale data non riflette in modo accurato il momento in cui l’attività o il problema è stato effettivamente completato, puoi modificare manualmente la Data di completamento effettiva.

Ad esempio, puoi contrassegnare un’attività o un problema come completato il lunedì, ma sai che il lavoro è stato completato il venerdì precedente. Dopo aver contrassegnato l’attività o il problema come completato, puoi aggiornare manualmente la Data di completamento effettiva dell’attività o del problema alla data del venerdì precedente per riflettere il completamento effettivo.

Non è possibile modificare manualmente la Data di completamento effettiva di un progetto, ma è possibile modificare manualmente lo stato di un progetto che può attivare una modifica alla relativa Data di completamento effettiva.

La data di completamento effettiva di un progetto è impostata nei modi seguenti:

* Aggiornando manualmente lo stato del progetto: se la modalità di completamento del progetto è impostata su Manuale e lo stato del progetto viene modificato manualmente su Completo, la data di completamento effettiva del progetto viene aggiornata alla data e all&#39;ora dell&#39;ultima attività completata.
* Automaticamente, quando l&#39;ultima attività del progetto viene completata: se la Modalità di completamento del progetto è impostata su Automatico e l&#39;ultima attività viene contrassegnata come Completa o se si aggiorna la Data di completamento effettiva dell&#39;ultima attività, anche la Data di completamento effettiva del progetto viene aggiornata con tale data.

  Per informazioni sull&#39;impostazione della modalità di completamento di un progetto, vedere l&#39;articolo [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md).

  >[!NOTE]
  >
  >Workfront utilizza come data di completamento effettiva per l&#39;intero progetto la data di completamento effettiva dell&#39;ultima attività del progetto completata.

Un amministratore di Workfront o di gruppo determina se Workfront utilizza la data odierna o la data di completamento pianificata di un’attività o un problema quando questi sono impostati su Completo o Chiuso. Per informazioni sull&#39;impostazione delle preferenze per attività e problemi, vedere [Configurare le preferenze per attività e problemi a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

<!--this statement is confusing, not sure what it is referring to, so I am drafting this for now: The value for the Actual Completion Date is always what is considered the current date and time.-->



## Individua le date di completamento effettive

La data di completamento effettiva si trova nelle seguenti aree di Workfront:

* Aree Dettagli progetto, Attività e Problema
* Caselle Modifica progetto, attività e problema
* Aggiornamenti di progetti, attività e problemi come aggiornamento del sistema.
* Elenchi o report di progetti, attività o problemi.

Per ulteriori informazioni sulla creazione di report, vedere l&#39;articolo [Creare un report personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
