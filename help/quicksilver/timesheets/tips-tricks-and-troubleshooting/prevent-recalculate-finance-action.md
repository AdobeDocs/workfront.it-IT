---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: Impedisci che l'azione Ricalcola dati finanziari influisca sulle ore storiche quando i tassi cambiano
description: È necessario aggiornare il costo orario per un utente o una mansione (a causa di un aumento o di un’altra circostanza), ma non si desidera che questa modifica influisca sulle ore precedentemente registrate nei progetti o che influisca solo su una parte delle ore storiche.
author: Alina
feature: Timesheets
exl-id: 29d3124b-cf7a-4a47-95c4-cd5379489810
source-git-commit: 7786d899841cb82cc4d3832fb083c6e2bda2e197
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---

# Impedisci che l&#39;azione Ricalcola dati finanziari influisca sulle ore storiche quando i tassi cambiano

## Problema

È necessario aggiornare il costo orario per un utente o una mansione (a causa di un aumento o di un’altra circostanza), ma non si desidera che questa modifica influisca sulle ore precedentemente registrate nei progetti o che influisca solo su una parte delle ore storiche.

## Soluzione

Aggiungi le ore che non vuoi cambiare in una Fatturazione sul progetto e imposta lo stato della fatturazione su Fatturato.  Questa operazione blocca il tasso precedente e verrà ignorata dall&#39;azione Ricalcola dati finanziari.  Le ore che non appartengono a un record Fatturazione fatturata vengono calcolate alla nuova tariffa. Per ulteriori informazioni, vedere [Ricalcolare i dati finanziari del progetto](../../manage-work/projects/project-finances/recalculate-project-finances.md).
