---
title: Panoramica della sezione Cronologia
description: È possibile esaminare le modifiche apportate al record e registrate dal sistema nel pannello destro di un record in Adobe Workfront Planning.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 8258589f-a7c3-4d77-9abe-c99e9184bd21
source-git-commit: cf42511263ec1cffd90d1e4bdcd43521b7fe6a30
workflow-type: tm+mt
source-wordcount: '462'
ht-degree: 3%

---

# Panoramica della sezione Cronologia

{{planning-important-intro}}

<!--update the system updates articles when we release to open beta - check the long commenting stream article list and see articles that document where in the system we have system updates; "Workfront Planning records" should be there-->

È possibile collaborare ai record di Adobe Workfront Planning aggiungendo commenti o risposte nel pannello destro di un record. In quest&#39;area è inoltre possibile visualizzare altre modifiche apportate al record e registrate dal sistema.

Nel pannello destro di un record vengono visualizzate le sezioni riportate di seguito.

* **Commenti**: visualizza i commenti e le risposte aggiunte dagli utenti ai record. Per ulteriori informazioni sulla gestione dei commenti nei record di Workfront Planning, vedere [Gestire i commenti ai record](/help/quicksilver/planning/records/manage-record-comments.md).
* **Cronologia**: visualizza le modifiche registrate dal sistema apportate dagli utenti ai campi record.

## Individuare la sezione Cronologia di un record

{{step1-to-planning}}

1. Fai clic sulla scheda di un’area di lavoro.

   L&#39;area di lavoro si apre e i tipi di record vengono visualizzati sulle schede.

1. Fare clic su una scheda del tipo di record.
Viene visualizzata la pagina del tipo di record e vengono visualizzati tutti i record di quel tipo.

1. In qualsiasi visualizzazione fare clic sul nome di un record.

   Viene visualizzata la pagina del record. L’area Commenti (Comments) viene visualizzata per impostazione predefinita nel pannello di destra.
1. Fai clic sull&#39;icona **Mostra cronologia** ![](assets/show-history-icon.png). Tutte le modifiche apportate ai campi del record vengono visualizzate nel pannello di destra, a partire da quello più recente.
1. (Facoltativo) Fai clic sull&#39;icona **Nascondi cronologia** ![](assets/hide-history-icon.png) per chiudere il pannello a destra.

## Considerazioni sulla sezione Cronologia

È possibile esaminare le modifiche apportate ai campi record nella sezione Cronologia del pannello di destra della pagina di un record.

![](assets/history-area-in-comments.png)

* Workfront Planning registra le seguenti informazioni nella sezione Cronologia:

   * Qualsiasi modifica apportata ai campi

   * I vecchi e i nuovi valori dei campi, quando i valori cambiano. I vecchi valori vengono visualizzati in formato barrato.

   * Nome completo dell&#39;utente che ha apportato la modifica

   * Indicatore di data e ora in cui è avvenuta la modifica.

* I campi dei tipi seguenti visualizzano sempre il valore precedente (in formato barrato) e il nuovo valore:

   * Testo
   * Paragrafo
   * Valuta
   * Data
   * Numero
   * Percentuale
   * Selezione singola

* I campi dei tipi seguenti mostrano il valore precedente in formato barrato solo se è stato rimosso almeno uno dei valori multipli:

   * Selezione multipla
   * Campi record collegati
   * Persone

  Se la modifica ha aggiunto solo valori al campo, il valore precedente non viene visualizzato e viene visualizzato solo il nuovo valore del campo.

* Nei campi di tipo casella di controllo non viene mai visualizzato il valore precedente in formato barrato. Se il campo viene modificato, viene visualizzato solo lo stato corrente al momento della modifica.

  Per ulteriori informazioni sui campi di Workfront Planning, vedere [Creare i campi](/help/quicksilver/planning/fields/create-fields.md).

* Le modifiche ai campi dei tipi seguenti non vengono visualizzate nella sezione Cronologia:

   * Campi collegati (ricerca)
   * Formula
   * Creato da
   * Data creazione
   * Ultima modifica eseguita da
   * Data ultima modifica

* Se un campo viene rimosso dal sistema, gli aggiornamenti apportati a tale campo rimangono nella sezione Cronologia. Non vi è alcuna indicazione che il campo sia stato rimosso nella sezione Cronologia di un record.
