---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: Impedire che l’azione Ricalcola dati finanziari influisca sulle ore storiche quando le tariffe cambiano
description: È necessario aggiornare il costo orario per un utente o una mansione (a causa di un aumento o di un’altra circostanza), ma non si desidera che questa modifica influisca sulle ore precedentemente registrate nei progetti o che influisca solo su una parte delle ore storiche.
author: Lisa
feature: Timesheets
exl-id: 29d3124b-cf7a-4a47-95c4-cd5379489810
TQID: https://experienceleague.adobe.com/TBeLp0FaUmlRk2uk5SdCqntrUWeAAVucox6Dyx5M0Uw
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 188
ht-degree: 13%

---

# Impedire che l’azione Ricalcola dati finanziari influisca sulle ore storiche quando le tariffe cambiano

## Problema

È necessario aggiornare il costo orario per un utente o una mansione (a causa di un aumento o di un’altra circostanza), ma non si desidera che questa modifica influisca sulle ore precedentemente registrate nei progetti o che influisca solo su una parte delle ore storiche.

## Soluzione

Aggiungi le ore che non vuoi cambiare in una Fatturazione sul progetto e imposta lo stato della fatturazione su Fatturato.  Questa operazione blocca il tasso precedente e verrà ignorata dall&#39;azione Ricalcola dati finanziari.  Le ore che non appartengono a un record Fatturazione fatturata vengono calcolate alla nuova tariffa. Per ulteriori informazioni, vedere [Ricalcolare i dati finanziari del progetto](../../manage-work/projects/project-finances/recalculate-project-finances.md).
