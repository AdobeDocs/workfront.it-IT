---
title: Miglioramenti alla comunicazione del quarto trimestre 2026
description: Miglioramenti alla comunicazione del quarto trimestre 2026
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: c34c4f351010980098b3efece8643a5f5620917f
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 5%

---

# Miglioramenti alla comunicazione del quarto trimestre 2026

Questa pagina descrive i miglioramenti apportati all’ambiente di anteprima nella versione del quarto trimestre 2026 per la generazione di rapporti. Tali miglioramenti saranno resi disponibili nell’ambiente di produzione come indicato.

Per un elenco di tutte le modifiche disponibili a questo punto del ciclo di rilascio del quarto trimestre 2026, consulta [Panoramica sulla versione del quarto trimestre 2026](/help/quicksilver/product-announcements/product-releases/26-q4-release-activity/26-q4-release-overview.md).

## Applicazione delle date di fine per i rapporti pianificati

>[!NOTE]
>
>Anteprima: 13 agosto 2026
>Versione rapida di produzione: 17 settembre 2026
>Produzione per tutti: 15 ottobre 2026

I rapporti pianificati ora richiedono una data di fine per impedire la consegna indefinita. Le pianificazioni che superano la data di fine vengono disattivate automaticamente.

Le pianificazioni esistenti sono state aggiornate con le date di fine per migliorare l’affidabilità e ridurre l’utilizzo non necessario del sistema. Workfront offre inoltre visibilità e avvisi aggiuntivi per aiutarti a gestire i cicli di vita della pianificazione dei rapporti in vista della data di fine.

Per ulteriori informazioni, consulta [Pianificare la consegna automatica di un report](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md).

<!--

## Updated column headers for dependent connected record fields

>[!NOTE]
>
>Preview: August 13, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

We've made visual improvements to the column headers for a dependent connected record field in the table view.

For information, see [Manage dependent connections](/help/quicksilver/planning/architecture/manage-dependent-connections.md).

-->

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
