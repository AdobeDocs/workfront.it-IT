---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Panoramica della data di inizio prevista del progetto
description: La data di inizio prevista è una data in tempo reale di inizio del progetto basata sulla data di inizio prevista della prima attività del progetto.
author: Alina
feature: Work Management
exl-id: 6277e6cf-0a73-4ba8-a3fd-c0da473dc5d4
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 0%

---

# Panoramica della data di inizio prevista del progetto

## Panoramica della data di inizio prevista per progetti e attività

La data di inizio prevista è una data in tempo reale di inizio del progetto basata sulla data di inizio prevista della prima attività del progetto.

Quando si pianifica un progetto per la prima volta, la data di inizio pianificata e la data di inizio prevista delle attività e del progetto sono identiche. Poiché si possono verificare ritardi o è possibile che le attività vengano completate prima, la Data inizio prevista può diventare diversa dalla Data inizio pianificata.

Le modifiche apportate alla data di inizio prevista della prima attività del progetto attivano le modifiche alla data di inizio prevista del progetto.

## Modificare la data di inizio prevista di un&#39;attività

La data di inizio prevista per un progetto o un’attività è un calcolo eseguito da Adobe Workfront e non può essere modificato manualmente.

I seguenti eventi possono attivare una modifica nella Data inizio prevista di un&#39;attività:

* Quando si inizia a lavorare su un&#39;attività, la data di inizio effettiva dell&#39;attività diventa la data di inizio prevista.
* Se la data di inizio pianificata di un&#39;attività viene superata, la data di inizio prevista si sposta nel futuro, indicando la data di inizio più vicina disponibile per l&#39;attività.\
  Quando si calcola la prima data disponibile per l&#39;inizio dell&#39;attività, Workfront tiene conto della quantità di ore pianificate per l&#39;attività e della pianificazione del progetto o dell&#39;utente assegnato all&#39;attività.
* Le attività predecessore in esecuzione in ritardo hanno un impatto sulla data di inizio prevista delle attività dipendenti. La data di inizio prevista delle attività dipendenti viene spostata in base al tipo di dipendenza della relazione predecessore e alle date previste dei predecessori.

Se una di queste attività è la prima attività di un progetto, la data di inizio prevista del progetto viene modificata in modo da corrispondere alla data di inizio prevista dell&#39;attività.

## Individuare la data di inizio prevista di un progetto o di un&#39;attività

È possibile individuare la data di inizio prevista di un progetto o di un&#39;attività nelle seguenti aree di Workfront:

* È possibile aggiungerlo a un progetto, a una relazione attività o a una visualizzazione.

  Per ulteriori informazioni sulla creazione di un report, vedere l&#39;articolo [Creare un report personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

* Nella sezione Project Details (Dettagli progetto) di un progetto o nella sezione Task Details (Dettagli attività) di un&#39;attività.
