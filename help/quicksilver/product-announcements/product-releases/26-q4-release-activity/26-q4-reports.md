---
title: Miglioramenti alla comunicazione del quarto trimestre 2026
description: Miglioramenti alla comunicazione del quarto trimestre 2026
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: ee1fceee828c97db535ccc03c8b428940d6f7eed
workflow-type: tm+mt
source-wordcount: '611'
ht-degree: 8%

---

# Miglioramenti alla comunicazione del quarto trimestre 2026

Questa pagina descrive i miglioramenti apportati all’ambiente di anteprima nella versione del quarto trimestre 2026 per la generazione di rapporti. Tali miglioramenti saranno resi disponibili nell’ambiente di produzione come indicato.

Per un elenco di tutte le modifiche disponibili a questo punto del ciclo di rilascio del quarto trimestre 2026, consulta [Panoramica sulla versione del quarto trimestre 2026](/help/quicksilver/product-announcements/product-releases/26-q4-release-activity/26-q4-release-overview.md).

<!--

## Duplicate dashboards in Canvas Dashboards

>[!NOTE]
>
>Preview: September 3, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

You can now duplicate a Canvas Dashboard using the new **Duplicate dashboard** action. This action is available to any user whose access level grants edit or create rights to Dashboards, even if they only have view access to the specific dashboard being copied. Users without edit or create rights to Dashboards do not see this action.

When you duplicate a dashboard, you can rename it, update its description and currency, and choose which widgets, dashboard filters, and dashboard prompts to carry over to the copy.

Run as user configurations on widgets are only preserved if you are the designated user or a system administrator. Sharing preferences are not copied to the new dashboard, and a confirmation message with a link to the new dashboard displays once the copy is complete.

Previously, there was no way to duplicate a dashboard; users had to rebuild dashboards from scratch to create audience-specific variations.

For more information, see 

-->

## Campo Tipo di approvazione nei dashboard di Canvas

>[!NOTE]
>
>Produzione per tutti: 28 agosto 2026
>[!BADGE Fuori pianificazione]{type=Neutral}

L&#39;entità Approvazione ora include un campo **Tipo di approvazione** che consente agli utenti di distinguere tra approvazioni di bozze, approvazioni di versioni di documenti, approvazioni di assunzioni e altri tipi di approvazione.

## Aggiornamento della terminologia di approvazione nei dashboard di Canvas

>[!NOTE]
>
>Produzione per tutti: 28 agosto 2026
>[!BADGE Fuori pianificazione]{type=Neutral}

I seguenti nomi di campo utilizzati nei dashboard di Canvas per le approvazioni di documenti e lavori sono stati rinominati per maggiore chiarezza:

| Nome precedente | Nuovo nome |
| --- | --- |
| Approvazione documento | Approvazione |
| Fase di approvazione documento | Fase di approvazione |
| Partecipante alla fase di approvazione documento | Fase di approvazione del partecipante |
| Processo di approvazione | Processo di approvazione lavoro |
| Fase di approvazione | Fase di approvazione lavoro |
| Stato approvatore | Stato approvatore lavoro |
| In attesa di Approvazione | In attesa di approvazione lavoro |

Questa modifica non influisce sul funzionamento dei rapporti correnti.

## Rapporti di tabella pivot nei dashboard di Canvas

>[!NOTE]
>
>Anteprima: 27 agosto 2026
>Versione rapida di produzione: 17 settembre 2026
>Produzione per tutti: 15 ottobre 2026

Il nuovo tipo di rapporto per tabella pivot nei dashboard di Canvas aggrega i dati con aggregazioni dati precise e complete. Puoi creare metriche quali conteggi, somme e medie direttamente sul dashboard, quindi eseguire il drill-through nei record sottostanti dietro qualsiasi totale.

Per ulteriori informazioni, vedere [Creare un report di tabella pivot in un dashboard di Canvas](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-pivot-table-report.md).

## Applicazione delle date di fine per i rapporti pianificati

>[!NOTE]
>
>Anteprima: 13 agosto 2026
>Versione rapida di produzione: 17 settembre 2026
>Produzione per tutti: 15 ottobre 2026

I rapporti pianificati ora richiedono una data di fine per impedire la consegna indefinita. Le pianificazioni che superano la data di fine vengono disattivate automaticamente.

Le pianificazioni esistenti sono state aggiornate con le date di fine per migliorare l’affidabilità e ridurre l’utilizzo non necessario del sistema. Workfront offre inoltre visibilità e avvisi aggiuntivi per aiutarti a gestire i cicli di vita della pianificazione dei rapporti in vista della data di fine.

Per ulteriori informazioni, consulta [Pianificare la consegna automatica di un report](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md).

## I campi di riferimento nativi sono disponibili per gli elenchi e i report

>[!NOTE]
>
>Anteprima: 30 luglio 2026
>Versione rapida di produzione: 13 agosto 2026
>Produzione per tutti: 15 ottobre 2026

È ora possibile aggiungere campi di riferimento nativi a elenchi e rapporti in Workfront.

Un campo di riferimento nativo è un campo personalizzato. Quando il campo si trova in un modulo personalizzato allegato a un oggetto, il campo viene popolato dai dati dell’oggetto. Ad esempio, se il campo fa riferimento al campo Descrizione e si trova in un modulo personalizzato allegato a un progetto, estrae la descrizione del progetto. Il campo può mostrare “N/D” se non sono disponibili dati.

Per informazioni sulla creazione di campi di riferimento nativi, incluso l&#39;elenco dei campi nativi supportati, vedere [Creare un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
Per informazioni sull&#39;aggiunta di campi ai report, vedere [Creare un report personalizzato](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Ordinamento coerente dei valori dei campi a selezione multipla negli elenchi e nei rapporti legacy

>[!NOTE]
>
>Anteprima: 30 luglio 2026
>Versione rapida di produzione: 13 agosto 2026
>Produzione per tutti: 15 ottobre 2026

Le opzioni selezionate per i campi personalizzati a selezione multipla vengono ora visualizzate in un ordine coerente e prevedibile negli elenchi e nei rapporti precedenti. L’ordine dei campi è determinato dalla disposizione dei campi nel modulo personalizzato.

![L&#39;ordine dei campi modulo personalizzato corrisponde all&#39;ordine dei valori selezionati in un elenco o report](assets/new-field-order-multi-select.png)

In precedenza, le opzioni selezionate venivano visualizzate nell’ordine in cui erano state scelte o in un ordine incoerente, rendendo più difficile la scansione e il confronto delle righe.

Nota: il nuovo ordinamento non è applicabile se il campo utilizza la modalità testo.
