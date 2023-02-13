---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcola costo lavoro pianificato
description: Quando si pianifica il lavoro sui progetti, Adobe Workfront calcola il costo del lavoro pianificato per i ruoli e gli utenti assegnati a questo lavoro in base ai valori di Costo per ora.
author: Alina
feature: Work Management
exl-id: af053e9a-09dc-4b4d-8ed4-f681ed611a59
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 0%

---

# Calcola costo lavoro pianificato

Quando si pianifica il lavoro sui progetti, Adobe Workfront calcola il costo del lavoro pianificato per i ruoli e gli utenti assegnati a questo lavoro in base ai valori di Costo per ora.

Il costo del lavoro pianificato di un progetto è un calcolo tra il costo associato ai ruoli del lavoro o agli utenti assegnati per completare il lavoro sul progetto e la quantità di ore pianificate (ore pianificate) che potrebbero richiedere a ciascun ruolo o utente di completare il lavoro.

## Panoramica del costo del lavoro pianificato

La **Costo del lavoro pianificato** di un progetto viene calcolato aggiungendo tutti i costi di manodopera pianificati di tutte le attività del progetto.

>[!TIP]
>
>Non esiste un costo del lavoro pianificato associato a problemi o al progetto stesso.

Workfront calcola il costo del lavoro pianificato di un progetto utilizzando la formula seguente:

```
Project Planned Labor Cost= SUM(Tasks Planned Labor Cost)
```

Il costo del lavoro pianificato dell&#39;attività viene calcolato in base ai seguenti criteri:

* Numero di risorse sull&#39;attività e relativa allocazione individuale all&#39;attività
* Tipo di costo dell&#39;attività.

Il costo del lavoro pianificato task viene calcolato utilizzando la formula seguente:

```
Task Planned Cost = Planned Hours x User or Job Role Cost Per Hour
```

Per ulteriori informazioni sul modo in cui Workfront calcola il costo del lavoro pianificato per le attività, a seconda delle assegnazioni delle attività e del tipo di costo, vedere la sezione &quot;Modifica tipi di costo per le singole attività&quot; nell&#39;articolo [Costi di tracciamento](../../../manage-work/projects/project-finances/track-costs.md).

## Individuare il costo del lavoro pianificato

È possibile individuare il costo del lavoro pianificato per un progetto nelle seguenti aree di Workfront:

* Rapporto Progetto
* Elenco dei progetti
* Un rapporto della linea di base in cui è possibile tenerlo traccia nel tempo
* Tramite l’API

Per informazioni sulla creazione di rapporti e sull’utilizzo dell’API Workfront, consulta i seguenti articoli:

* [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)
* [Nozioni di base sulle API](../../../wf-api/general/api-basics.md)
