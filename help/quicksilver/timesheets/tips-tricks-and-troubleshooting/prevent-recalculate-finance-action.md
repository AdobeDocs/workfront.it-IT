---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: Impedisci che l'azione Ricalcola finanze influisca sugli orari storici in caso di modifica dei tassi
description: È necessario aggiornare il costo orario per un utente o un ruolo di lavoro (a causa di un aumento o di un'altra circostanza), ma non si desidera che questa modifica influisca sulle ore in cui è stato eseguito l'accesso a progetti in precedenza o si desidera che influisca solo su una parte delle ore storiche.
author: Alina
feature: Timesheets
exl-id: 29d3124b-cf7a-4a47-95c4-cd5379489810
source-git-commit: 7786d899841cb82cc4d3832fb083c6e2bda2e197
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---

# Impedisci che l&#39;azione Ricalcola finanze influisca sugli orari storici in caso di modifica dei tassi

## Problema

È necessario aggiornare il costo orario per un utente o un ruolo di lavoro (a causa di un aumento o di un&#39;altra circostanza), ma non si desidera che questa modifica influisca sulle ore in cui è stato eseguito l&#39;accesso a progetti in precedenza o si desidera che influisca solo su una parte delle ore storiche.

## Soluzione

Aggiungere le ore che non si desidera modificare in un record di fatturazione nel progetto e impostare lo stato del record di fatturazione su Fatturato.  Questo blocca il vecchio tasso e verrà ignorato dall&#39;azione Ricalcola finanze.  Tutte le ore che non appartengono a un record di fatturazione fatturata vengono calcolate al nuovo tasso. Per ulteriori informazioni, consulta [Ricalcolare le finanze del progetto](../../manage-work/projects/project-finances/recalculate-project-finances.md).
