---
content-type: reference
product-area: projects
navigation-topic: task-information
title: Differenza tra durata pianificata e durata per le attività
description: Durata è il tempo che intercorre tra l'inizio pianificato e la data di completamento pianificata di un elemento di lavoro. Le attività hanno una Durata e una Durata Pianificata in Adobe Workfront, a seconda del Tipo di Durata dell’attività.
author: Alina
feature: Work Management
exl-id: 183a3334-b4af-4f45-8e72-9e82ff3862a0
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---

# Differenza tra durata pianificata e durata per le attività

Durata è il tempo che intercorre tra l&#39;inizio pianificato e la data di completamento pianificata di un elemento di lavoro. Le attività hanno una Durata e una Durata Pianificata in Adobe Workfront, a seconda del Tipo di Durata dell’attività.

I problemi e i progetti non possono essere associati a un Tipo di durata e hanno solo una Durata.

## Durata attività

Per le attività, la Durata e la Durata pianificata in genere mostrano lo stesso valore: l&#39;intervallo di tempo tra la Data inizio pianificata e la Data completamento pianificata di un&#39;attività.

Quando il tipo di durata dell&#39;attività è Basato sull&#39;impegno, la durata pianificata diminuisce man mano che si aggiungono risorse all&#39;attività.

**Esempio:** se un&#39;attività con un tipo di durata impostato su Impegno ha una durata di 3 giorni e si assegna all&#39;attività una risorsa con una pianificazione a tempo pieno, anche la durata pianificata è di 3 giorni.

Se si assegnano tre risorse con una programmazione a tempo pieno alla stessa attività, la Durata rimane 3 giorni, ma la Durata pianificata diventa 1 giorno. Con Durata pianificata vengono modificate anche le date di Inizio pianificato e Completamento pianificato dell&#39;attività, in modo da riflettere la nuova Durata pianificata. Di conseguenza, anche la timeline del progetto ne risente.
È possibile utilizzare il Tipo di durata basata sulle risorse quando si assegna un&#39;attività a più risorse. In questo modo si riduce il tempo necessario per il completamento del lavoro sull&#39;attività.

Per ulteriori informazioni sul tipo di durata basata sulle risorse, vedere [Panoramica sul tipo di durata: basata sulle risorse](../../../manage-work/tasks/taskdurtn/effort-driven.md).

## Problema e durata del progetto

I problemi e i progetti hanno un solo valore Durata, che è la differenza tra la Data inizio pianificata e la Data completamento pianificata del problema e del progetto, rispettivamente.
