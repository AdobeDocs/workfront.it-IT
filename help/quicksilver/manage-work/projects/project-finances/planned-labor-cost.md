---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcola costo manodopera pianificata
description: Quando si pianifica il lavoro sui progetti, Adobe Workfront calcola il costo manodopera pianificata per i ruoli e gli utenti assegnati a questo lavoro in base ai valori del costo orario.
author: Lisa
feature: Work Management
exl-id: af053e9a-09dc-4b4d-8ed4-f681ed611a59
source-git-commit: 6afa65f921864403c10541d283ef717dce81aed7
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 0%

---

# Calcola costo manodopera pianificata

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
