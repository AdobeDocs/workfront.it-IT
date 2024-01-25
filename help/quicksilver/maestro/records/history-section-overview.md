---
title: Panoramica della sezione Cronologia
description: È possibile esaminare le modifiche apportate al record e registrate dal sistema nel pannello destro di un record in Adobe Maestro.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 54c6adf51ab8ef4e7968e8fdeeb0025e42deecc5
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 2%

---


# Panoramica della sezione Cronologia

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--update the system updates articles when we release to open beta - check the long commenting stream article list and see articles that document where in the system we have system updates; "Maestro records" should be there-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. </span>

<span class="preview">For information about the current release schedule, see [First Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).</span> -->

Puoi collaborare ai record Adobe Maestro aggiungendo commenti o risposte nel pannello destro di un record. In quest&#39;area è inoltre possibile visualizzare altre modifiche apportate al record e registrate dal sistema.

Nel pannello destro di un record vengono visualizzate le sezioni riportate di seguito.

* **Commenti**: visualizza i commenti e le risposte aggiunte dagli utenti ai record. Per ulteriori informazioni sulla gestione dei commenti nei record Maestro, vedi [Gestisci commenti record](/help/quicksilver/maestro/records/manage-record-comments.md).
* **Cronologia**: visualizza le modifiche registrate dal sistema apportate dagli utenti ai campi record.

## Individuare la sezione Cronologia di un record

{{step1-to-maestro}}

Per impostazione predefinita, viene aperta l’ultima area di lavoro a cui si è effettuato l’accesso.

1. Scegliere una vista tabella dal menu **Visualizza** menu a discesa.
1. Fare clic sul nome di un record nella vista tabella.

   Il record **Dettagli** viene visualizzata la pagina. L’area Commenti (Comments) viene visualizzata per impostazione predefinita nel pannello di destra.
1. Fai clic su **Mostra cronologia** icona ![](assets/show-history-icon.png). Tutte le modifiche apportate ai campi del record vengono visualizzate nel pannello di destra, a partire da quello più recente.
1. (Facoltativo) Fai clic su **Nascondi cronologia** icona ![](assets/hide-history-icon.png) per chiudere il pannello destro.

## Considerazioni sulla sezione Cronologia

È possibile esaminare le modifiche apportate ai campi record nella sezione Cronologia del pannello di destra della pagina Dettagli di un record operativo o di una tassonomia.

![](assets/history-area-in-comments.png)

* Maestro registra le seguenti informazioni nella sezione Cronologia:

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
   * Campi collegati (ricerca)
   * Persone

  Se la modifica ha aggiunto solo valori al campo, il valore precedente non viene visualizzato e viene visualizzato solo il nuovo valore del campo.

* Nei campi di tipo casella di controllo non viene mai visualizzato il valore precedente in formato barrato. Se il campo viene modificato, viene visualizzato solo lo stato corrente al momento della modifica.

  Per ulteriori informazioni sui campi Maestro, consulta [Crea campi](/help/quicksilver/maestro/fields/create-fields.md).

* Se un campo viene rimosso dal sistema, gli aggiornamenti apportati a tale campo rimangono nella sezione Cronologia. Non vi è alcuna indicazione che il campo sia stato rimosso nella sezione Cronologia di un record.