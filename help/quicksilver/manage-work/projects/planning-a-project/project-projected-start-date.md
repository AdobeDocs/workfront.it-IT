---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Panoramica della data di inizio prevista del progetto
description: La data di inizio prevista è una data in tempo reale in cui il progetto verrà avviato in base alla data di inizio prevista della prima attività del progetto.
author: Alina
feature: Work Management
exl-id: 6277e6cf-0a73-4ba8-a3fd-c0da473dc5d4
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 0%

---

# Panoramica della data di inizio prevista del progetto

## Panoramica della data di inizio prevista per progetti e attività

La data di inizio prevista è una data in tempo reale in cui il progetto verrà avviato in base alla data di inizio prevista della prima attività del progetto. 

Quando si pianifica un progetto per la prima volta, la data di inizio prevista e la data di inizio prevista delle attività e del progetto sono identiche. Poiché possono verificarsi ritardi o è possibile che le attività vengano completate in precedenza, la data di inizio prevista può diventare diversa dalla data di inizio prevista. 

Le modifiche apportate alla data di inizio prevista della prima attività del progetto attivano le modifiche nella data di inizio prevista del progetto. 

## Modificare la data di inizio prevista di un&#39;attività

La data di inizio prevista per un progetto o un&#39;attività è un calcolo eseguito da Adobe Workfront e non può essere modificato manualmente. 

Gli eventi seguenti possono attivare una modifica nella data di inizio prevista di un&#39;attività:

* Quando si inizia a lavorare su un&#39;attività, la data di inizio effettivo dell&#39;attività diventa la data di inizio prevista.
* Se la data di inizio prevista di un&#39;attività viene passata, la data di inizio prevista verrà spostata in futuro, indicando la data più breve disponibile per l&#39;inizio dell&#39;attività.\
   Quando si calcola la prima data disponibile per l’avvio dell’attività, Workfront tiene conto della quantità di ore pianificate sull’attività, nonché della pianificazione del progetto o dell’utente assegnato all’attività. 
* Le attività predecessori in esecuzione hanno un impatto sulla data di inizio prevista delle attività dipendenti. La data di inizio prevista delle attività dipendenti si sposta in base al tipo di dipendenza della relazione predecessore e alle date previste dei predecessori. 

Se una di queste attività è la prima di un progetto, la data di inizio prevista del progetto viene modificata in modo che corrisponda alla data di inizio prevista di questa attività. 

## Individuare la data di inizio prevista di un progetto o di un&#39;attività

È possibile individuare la data di inizio prevista di un progetto o di un&#39;attività nelle seguenti aree di Workfront:

* È possibile aggiungerlo a un progetto o a un report attività o a una visualizzazione.

   Per ulteriori informazioni sulla creazione di un rapporto, consulta l’articolo [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

* Nella sezione Dettagli progetto di un progetto o nella sezione Dettagli attività di un&#39;attività.
