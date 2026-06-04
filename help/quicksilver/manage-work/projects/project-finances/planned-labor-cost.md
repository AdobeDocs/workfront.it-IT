---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcolare il costo manodopera pianificato
description: Quando si pianifica il lavoro sui progetti, Adobe Workfront calcola il costo manodopera pianificata per i ruoli e gli utenti assegnati a questo lavoro in base ai valori del costo orario.
author: Lisa
feature: Work Management
exl-id: af053e9a-09dc-4b4d-8ed4-f681ed611a59
TQID: https://experienceleague.adobe.com/xzjI7jrIuUBcwF7MpZ8fcWGuFgDrY-V2OUlAq95lDAw
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 309
ht-degree: 3%

---

# Calcolare il costo manodopera pianificato

Quando si pianifica il lavoro sui progetti, Adobe Workfront calcola il costo manodopera pianificata per i ruoli e gli utenti assegnati a questo lavoro in base ai valori del costo orario.

Il Costo manodopera pianificata di un progetto è un calcolo tra il costo associato alle mansioni o agli utenti assegnati per completare il lavoro sul progetto e la quantità di ore pianificate (Ore pianificate) che potrebbero richiedere a ciascun ruolo o utente di completare tale lavoro.

## Panoramica del costo della manodopera pianificata

Il **costo manodopera pianificata** di un progetto viene calcolato aggiungendo tutti i costi manodopera pianificata di tutte le attività del progetto.

>[!TIP]
>
>Non esiste alcun Costo di Lavoro Pianificato associato ai problemi o al progetto stesso.

Workfront calcola il costo manodopera pianificata di un progetto utilizzando la formula seguente:

```
Project Planned Labor Cost= SUM(Tasks Planned Labor Cost)
```

Il costo manodopera pianificata per l&#39;attività viene calcolato in base ai seguenti elementi:

* Numero di risorse sull&#39;attività e relativa allocazione individuale all&#39;attività
* Tipo di costo dell&#39;attività.

Il costo manodopera pianificata per l&#39;attività viene calcolato utilizzando la formula seguente:

```
Task Planned Cost = Planned Hours x User or Job Role Cost Per Hour
```

Per ulteriori informazioni sul modo in cui Workfront calcola il costo della manodopera pianificata per le attività, in base alle assegnazioni delle attività e al tipo di costo, vedere la sezione &quot;Modifica tipi di costo per singole attività&quot; nell&#39;articolo [Tracciare i costi](../../../manage-work/projects/project-finances/track-costs.md).

## Individuazione del costo manodopera pianificata

È possibile individuare il costo manodopera pianificata di un progetto nelle seguenti aree di Workfront:

* Un report di progetti
* Un elenco di progetti
* Un report di baseline in cui è possibile tracciarlo nel tempo
* Tramite l’API

Per informazioni sulla creazione di rapporti e sull’utilizzo dell’API Workfront, consulta i seguenti articoli:

* [Crea un report personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)
* [Nozioni di base sulle API](../../../wf-api/general/api-basics.md)
