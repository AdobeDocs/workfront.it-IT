---
title: Le assegnazioni in un oggetto eliminato appaiono in modo imprevisto nei report degli assegnatari
description: Le assegnazioni in un oggetto eliminato appaiono in modo imprevisto nei report degli assegnatari
author: Courtney
draft: Probably
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '146'
ht-degree: 0%

---

# Le assegnazioni in un oggetto eliminato appaiono in modo imprevisto nei report degli assegnatari

## Problema

Dopo aver eliminato un oggetto con un&#39;assegnazione, vengono eliminati sia l&#39;oggetto che l&#39;assegnazione. Tuttavia, l&#39;assegnazione potrebbe essere ancora visualizzata in alcuni rapporti.

Se ad esempio si elimina un&#39;attività assegnata a un utente, viene eliminata anche l&#39;assegnazione all&#39;utente. Tuttavia, se in seguito si esegue un report di attività filtrato per assegnatario, con l&#39;utente specificato, il report elenca ancora l&#39;attività eliminata se l&#39;attività si trova ancora nel Cestino.

## Causa

Ciò è dovuto a limitazioni architetturali del Cestino. Attualmente non sono previsti piani per affrontare questo problema a causa della portata della riprogettazione architettonica che sarebbe necessaria.
