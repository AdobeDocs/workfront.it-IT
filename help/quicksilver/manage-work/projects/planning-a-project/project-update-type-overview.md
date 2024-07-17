---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Panoramica del tipo di aggiornamento del progetto
description: Il tipo di aggiornamento di un progetto indica il modo in cui Adobe Workfront calcola la timeline di un progetto. Le modifiche apportate al piano di progetto potrebbero determinare modifiche nella sequenza temporale del progetto. La timeline del progetto deve essere ricalcolata automaticamente o manualmente per garantire che sia aggiornata con queste modifiche.
author: Alina
feature: Work Management
exl-id: a6394961-2ac8-4b95-aa1b-dba8108c612f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '515'
ht-degree: 0%

---

# Panoramica del tipo di aggiornamento del progetto

Il tipo di aggiornamento di un progetto indica il modo in cui Adobe Workfront calcola la timeline di un progetto. Le modifiche apportate al piano di progetto potrebbero determinare modifiche nella sequenza temporale del progetto. La timeline del progetto deve essere ricalcolata automaticamente o manualmente per garantire che sia aggiornata con queste modifiche.

Per informazioni sul ricalcolo della sequenza temporale del progetto, vedere [Ricalcolare le sequenze temporali del progetto](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

## Tipi di aggiornamento del progetto

Esistono quattro tipi di aggiornamento per un progetto, a seconda di quando si desidera che Workfront ricalcoli la sequenza temporale del progetto. Selezionate un tipo di aggiornamento dall&#39;elenco seguente.

Per informazioni su come aggiornare il tipo di aggiornamento del progetto, vedere [Selezionare il tipo di aggiornamento del progetto](../../../manage-work/projects/manage-projects/select-project-update-type.md).

>[!IMPORTANT]
>
>Se la timeline di un progetto è più lunga di 15 anni, Workfront non la calcola automaticamente o in caso di modifica. Il tipo di aggiornamento di un progetto di durata superiore a 15 anni è sempre Manuale.

* **Automatico e alla modifica:** Questa è l&#39;impostazione predefinita. La timeline del progetto viene aggiornata ogni volta che si verifica una modifica nel progetto o in un altro progetto da cui dipende. Anche la timeline del progetto viene aggiornata ogni notte. \
  Si tratta dell’impostazione consigliata in quanto garantisce che la timeline del progetto sia sempre aggiornata.

  Quando si aggiorna un&#39;attività o un progetto e si attiva un ricalcolo della sequenza temporale, tutte le date disponibili vengono visualizzate immediatamente, consentendo di continuare a lavorare. Nei progetti con più di 100 attività, le date che richiedono calcoli più lunghi vengono disattivate.

  ![](assets/dates-dimmed-when-insline-editing-350x146.png)

  Questo indica che il ricalcolo non è ancora terminato e che le date sono soggette a modifiche.

* **Solo modifica:** la sequenza temporale del progetto viene aggiornata ogni volta che si verifica una modifica nel progetto o in un altro progetto da cui dipende la sequenza temporale. Gli aggiornamenti pianificati non vengono eseguiti.\
  È possibile selezionare questa opzione se si è preoccupati delle prestazioni del sistema e se raramente si verificano modifiche nel progetto o in altri progetti da cui dipende la sequenza temporale.

* **Solo automatico:** La sequenza temporale del progetto viene aggiornata ogni notte e non viene aggiornata immediatamente dopo le modifiche apportate.\
  È possibile selezionare questa opzione se si è preoccupati delle prestazioni del sistema e se si verificano molte modifiche ogni giorno nel progetto o in altri progetti da cui dipende la sequenza temporale.

  >[!NOTE]
  >
  >Un progetto non viene ricalcolato automaticamente ogni notte se si trova nello stato Pianificazione. Viene ricalcolato solo in seguito a modifica.

* **Solo manuale:** la sequenza temporale del progetto viene aggiornata solo quando si seleziona l&#39;opzione **Ricalcola sequenze temporali**, come descritto nella sezione &quot;Ricalcolo manuale&quot; nell&#39;articolo [Ricalcola sequenze temporali del progetto](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).\
  È possibile selezionare questa opzione se si apportano contemporaneamente molte modifiche al progetto e si desidera che il ricalcolo della sequenza temporale venga eseguito dopo che tutte le modifiche sono state apportate (anziché dopo ogni singola modifica).
