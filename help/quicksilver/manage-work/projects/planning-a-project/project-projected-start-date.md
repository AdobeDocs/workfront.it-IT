---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Panoramica sulla data di inizio prevista del progetto
description: La data di inizio prevista è una data in tempo reale di inizio del progetto basata sulla data di inizio prevista della prima attività del progetto.
author: Alina
feature: Work Management
exl-id: 6277e6cf-0a73-4ba8-a3fd-c0da473dc5d4
TQID: https://experienceleague.adobe.com/2rcx201EGt4cqRpqfXws6P-NbRnXyVlFoTbJrQJBipg
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 430
ht-degree: 6%

---

# Panoramica sulla data di inizio prevista del progetto

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

  Per ulteriori informazioni sulla creazione di un rapporto, consulta l’articolo [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

* Nella sezione Project Details (Dettagli progetto) di un progetto o nella sezione Task Details (Dettagli attività) di un&#39;attività.
