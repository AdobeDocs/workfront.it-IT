---
content-type: reference
product-area: projects
navigation-topic: task-information
title: Differenza tra la durata prevista e la durata delle attività
description: La durata è la quantità di tempo tra la data di inizio pianificata e la data di completamento pianificata di un elemento di lavoro. Le attività hanno una Durata e una Durata pianificata in Adobe Workfront, a seconda del Tipo di durata dell’attività.
author: Alina
feature: Work Management
exl-id: 183a3334-b4af-4f45-8e72-9e82ff3862a0
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---

# Differenza tra la durata prevista e la durata delle attività

La durata è la quantità di tempo tra la data di inizio pianificata e la data di completamento pianificata di un elemento di lavoro. Le attività hanno una Durata e una Durata pianificata in Adobe Workfront, a seconda del Tipo di durata dell’attività.

I problemi e i progetti non possono essere associati a un tipo di durata e hanno solo una durata.

## Durata attività

Per le attività, in genere vengono visualizzati lo stesso valore in Durata e Durata pianificata: il periodo di tempo tra la data di inizio pianificata e la data di completamento pianificata di un&#39;attività.

Quando il tipo di durata dell&#39;attività è Basato su sforzo, la durata pianificata diminuisce man mano che si aggiungono risorse all&#39;attività.

**Esempio:** Se un&#39;attività con un tipo di sforzo di durata ha una durata di 3 giorni e si assegna all&#39;attività una risorsa con una pianificazione a tempo pieno, anche la durata prevista è di 3 giorni.

Se si assegnano tre risorse con una pianificazione a tempo pieno alla stessa attività, la Durata rimane di 3 giorni, ma la Durata pianificata diventa di 1 giorno. La durata pianificata cambia anche le date di inizio e completamento pianificato dell&#39;attività, in modo da riflettere la nuova durata pianificata. Di conseguenza, viene interessata anche la timeline del progetto.
È possibile utilizzare il tipo di durata guidata sforzo quando si assegna un&#39;attività a più risorse. Questo riduce il tempo necessario per completare il lavoro sull’attività.

Per ulteriori informazioni sul tipo di durata guidata sforzo, consulta [Panoramica sul tipo di durata: Guida allo sforzo](../../../manage-work/tasks/taskdurtn/effort-driven.md).

## Problema e durata del progetto

I problemi e i progetti hanno un solo valore di Durata, corrispondente alla differenza tra la Data inizio prevista e la Data completamento pianificato rispettivamente del problema e del progetto.
