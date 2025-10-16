---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-tasks
title: La durata prevista non corrisponde alla durata pianificata
description: 'In questo articolo viene descritta la risoluzione dei problemi in Adobe Workfront quando potrebbe venire visualizzato il seguente messaggio: "La durata prevista di un''attività/problema è stata impostata su 0 e non corrisponde alla durata pianificata".'
author: Alina
feature: Work Management
exl-id: ef135d44-3138-457d-b54a-3f1102ce3116
source-git-commit: c1b8af0d8a95714bb597db7a429794773358cf05
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 0%

---

# La durata prevista non corrisponde alla durata pianificata

## Problema

Viene visualizzato il seguente messaggio di errore: &quot;La durata prevista di un&#39;attività/problema è stata impostata su 0 e non corrisponde alla durata pianificata&quot;.

## Causa

Ciò si verifica quando la data di inizio prevista corrisponde alla data di completamento prevista.

## Soluzione

Ci sono molti fattori che possono causare la corrispondenza tra le date di inizio previsto e di completamento. Questo problema è in gran parte legato alla distribuzione del tempo sull&#39;attività o sul problema in questione.

Nella maggior parte dei casi, a seconda del tipo di durata e del vincolo attività dell&#39;attività, l&#39;allocazione deve estendere la data di completamento prevista molto oltre il previsto. Tuttavia, in alcuni casi in base al modo in cui sono configurati Tipo di durata e Vincolo attività, è possibile che sia pari a zero.

Di seguito sono riportati gli elementi migliori da verificare in questi casi con collegamenti ai relativi articoli di supporto:

* Data di completamento prevista: [Panoramica della Data di completamento prevista per progetti, attività e problemi](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md)
* Vincolo attività: [Panoramica vincolo attività](../../../manage-work/tasks/task-constraints/task-constraint-overview.md)
* Tipo di durata: [Panoramica sulla durata dell&#39;attività e sul tipo di durata](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)

Se il tipo di data di completamento prevista, vincolo attività o durata funziona come previsto, contatta il supporto per una risoluzione più approfondita dei problemi.
