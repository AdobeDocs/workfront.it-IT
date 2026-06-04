---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcola l’Indice prestazioni pianificazione costi (CSI)
description: Il CSI (Cost Schedule Performance Index) è un calcolo automatico che combina l'IPC (Cost Performance Index) e l'IPP (Schedule Performance Index) in un'unica metrica generale che bilancia i costi e la programmazione.
author: Lisa
feature: Work Management
exl-id: 38a8c5e0-b812-499d-8fe7-a71ddccb3aad
TQID: https://experienceleague.adobe.com/USODdaQOyE-D76BVmLLVUS1WxUMrK6Q05xZU1Xg9Gjc
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 332
ht-degree: 16%

---

# Calcola l’Indice prestazioni pianificazione costi (CSI)

<!-- Audited: 6/2025 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.) </p>
-->

## Panoramica dell&#39;indice delle prestazioni del programma di costo (CSI)

Il CSI (Cost Schedule Performance Index) è un calcolo automatico che combina l&#39;IPC (Cost Performance Index) e l&#39;IPP (Schedule Performance Index) in un&#39;unica metrica generale che bilancia i costi e la programmazione. Moltiplicando insieme questi valori, una singola metrica può rappresentare una pianificazione prolungata con un budget inferiore o viceversa. I project manager possono utilizzarla per determinare lo stato generale del progetto o dell’attività quando il costo viene sacrificato per prouovere alla pianificazione di metà progetto.

>[!TIP]
>
>Adobe Workfront calcola CSI sia per le attività che per i progetti, ma non per i problemi.

Puoi trarre vantaggio dalle informazioni fornite da questa metrica solo se nell’organizzazione sono presenti i seguenti scenari:

* Gli utenti registrano il tempo necessario per completare il lavoro. Questo calcola il CSI in base alle ore.
* Agli utenti o alle mansioni sono associati tassi Costo orario. Questo calcola il CSI in base ai costi.

## Modalità di calcolo dell&#39;indice di prestazioni del programma di costo (CSI, Cost Schedule Performance Index) in Workfront

Workfront calcola l&#39;indice di prestazioni dei costi (CSI, Cost Performance Index) di un progetto o di un task utilizzando la formula seguente:

`CSI = CPI x SPI`

Per informazioni sull&#39;indice dei prezzi al consumo, vedere l&#39;articolo [Calcolare l&#39;indice delle prestazioni dei costi (IPC)](../../../manage-work/projects/project-finances/calculate-cpi.md).

Per informazioni su SPI, vedere l&#39;articolo [Calcolare l&#39;indice delle prestazioni della pianificazione (SPI)](../../../manage-work/projects/project-finances/calculate-spi.md).

CSI ha i seguenti tre valori possibili:

* 1 = segue il piano generale
* \>1 = Combinazione programmazione sotto budget
* &lt;1 = Combinazione di programmi fuori budget

![CSI](assets/csi-highlighted.png)

## Individuare l&#39;indice CSI (Cost Schedule Performance Index)

>[!CAUTION]
>
>Per visualizzare il valore CSI di un progetto o di un task, è necessario disporre dell&#39;accesso Visualizzazione dati finanziari nel proprio livello di accesso e delle autorizzazioni per visualizzare il progetto o il task.

È possibile individuare CSI nelle seguenti aree di Workfront:

* Area Finanza nella sezione Dettagli progetto.
* Area Contabilità nella sezione Dettagli attività.
* Visualizzazione di un progetto o di un&#39;attività.
* Un report di progetto o attività.
