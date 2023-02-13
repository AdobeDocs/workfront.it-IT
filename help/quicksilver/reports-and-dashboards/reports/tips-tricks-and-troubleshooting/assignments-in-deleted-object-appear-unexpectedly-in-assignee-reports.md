---
title: Le assegnazioni in un oggetto eliminato vengono visualizzate in modo imprevisto nei rapporti relativi agli assegnatari
description: Le assegnazioni in un oggetto eliminato vengono visualizzate in modo imprevisto nei rapporti relativi agli assegnatari
author: Nolan
draft: Probably
source-git-commit: de30bd970bda06c706e5156d5195e8568558e593
workflow-type: tm+mt
source-wordcount: '146'
ht-degree: 0%

---

# Le assegnazioni in un oggetto eliminato vengono visualizzate in modo imprevisto nei rapporti relativi agli assegnatari

## Problema

Dopo aver eliminato un oggetto con un&#39;assegnazione, vengono eliminati sia l&#39;oggetto che l&#39;assegnazione. Ma l&#39;incarico potrebbe ancora apparire in alcuni rapporti.

Ad esempio, se si elimina un&#39;attività assegnata a un utente, viene eliminata anche l&#39;assegnazione all&#39;utente. Tuttavia, se in seguito si esegue un report attività filtrato per assegnatario, con tale utente specificato, il report elenca comunque l&#39;attività eliminata se l&#39;attività è ancora nel Cestino.

## Causa

Ciò è dovuto alle limitazioni architettoniche del Cestino. Attualmente non vi sono piani per affrontare questo problema a causa della portata della riprogettazione architettonica che sarebbe necessaria.
