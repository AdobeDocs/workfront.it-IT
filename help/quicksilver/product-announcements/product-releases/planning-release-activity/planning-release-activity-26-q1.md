---
content-type: release-notes
title: Attività della versione del primo trimestre 2026 per Adobe Workfront Planning
description: Questa è l’attività di rilascio per il prodotto Adobe Workfront Planning per il primo trimestre 2026.
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: 7fb12a3fbdad661baf2d0ad472ce8017e178ddef
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 0%

---

# Attività della versione del primo trimestre 2026 per Adobe Workfront Planning

Questo articolo descrive le funzioni rilasciate per Workfront Planning durante la versione del primo trimestre 2026.

<!--keep the sentence below for all future quarterly release pages-->

Per un elenco di tutte le funzionalità rilasciate per Adobe Workfront Planning, vedere [Attività di rilascio di Adobe Workfront Planning: indice articolo](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).


<!--## New field search box in the Filters, Fields, and Row colors icons in Planning views

>[!NOTE]
>
>Preview: October 30, 2025 
>Production fast release: November 13, 2025 
>Production for everyone:  January 15, 2026 


You can now search for a specific field when building a view element in record type view. The new search boxes have been added when you build a filter, sort, grouping, or when you configure your fields or row colors. Prior to this enhancement, you could simply scroll through the list of available fields.
This improvement is available in all views.

For information, see [Manage the table view](/help/quicksilver/planning/views/manage-the-table-view.md).-->


## Tipi di record globali e la possibilità di aggiungerli come tipi di record esistenti ad altre aree di lavoro

>[!NOTE]
>
>Anteprima: 16 ottobre 2025
>&#x200B;>Versione rapida di produzione: 13 novembre 2025
>&#x200B;>Produzione per tutti: 15 gennaio 2026

Quando si implementa Workfront Planning per un’organizzazione con più team e flussi di lavoro comuni, potrebbe essere necessario definire una struttura coesa e i metadati per i tipi di record chiave (come Campagne o Deliverable) che possono essere aggiunti alle aree di lavoro di ciascun team per acquisire e gestire il proprio lavoro.

Inoltre, potrebbe essere necessario il lavoro di ogni team per raggiungere un livello centrale.

Con un flusso di lavoro di questo tipo, puoi fare in modo che i team acquisiscano in modo coerente il proprio lavoro e allo stesso tempo sblocchino la visibilità tra i team, senza dover aggiungere tutti gli utenti dell’organizzazione a ogni area di lavoro. A tale scopo, è possibile utilizzare i tipi di record globali.

È ora possibile designare un tipo di record come globale e utilizzarlo in più aree di lavoro. Gli utenti possono utilizzare la stessa struttura di campi e le stesse connessioni già configurate in un’area di lavoro centrale.

Per ulteriori informazioni, consulta i seguenti articoli:

* [Panoramica del tipo di record tra aree di lavoro](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md)

* [Configurare le funzionalità tra aree di lavoro diverse per il tipo di record](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)

* [Aggiungere tipi di record esistenti da un&#39;altra area di lavoro](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md)

## Nuovo limite per i campi di connessione per un tipo di record

>[!NOTE]
>
>Anteprima: 16 ottobre 2025
>&#x200B;>Versione rapida di produzione: 13 novembre 2025
>&#x200B;>Produzione per tutti: 15 gennaio 2026

È stato introdotto un limite di 30 campi di connessione per ogni tipo di record.

NOTA: se l&#39;organizzazione dispone attualmente di più di 30 campi di connessione per un tipo di record, è possibile mantenere i campi aggiuntivi che superano il limite di 30. Non è tuttavia possibile aggiungere altri campi di connessione ai tipi di record che superano il limite. In futuro, verrà applicato il nuovo limite di 30 campi di connessione.

Per ulteriori informazioni, vedere [Panoramica sui tipi di record connessi](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

## Impostare valori descrittivi per le scelte dei campi di tipo selezionato

>[!NOTE]
>
>Anteprima: 16 ottobre 2025
>&#x200B;>Versione rapida di produzione: 13 novembre 2025
>&#x200B;>Produzione per tutti: 15 gennaio 2026

Quando si aggiungono scelte di campo a un campo a selezione singola o multipla, Workfront assegnerà valori univoci di facile utilizzo a ciascuna scelta. Prima di questo miglioramento, Workfront generava un ID alfanumerico difficile da comprendere e utilizzare nelle chiamate API e in altre integrazioni.

Considera quanto segue con questo miglioramento:

* I nuovi valori verranno aggiunti alle nuove scelte di campo. Le scelte di campo esistenti manterranno i loro ID alfanumerici.

* I valori di scelta sono univoci per un campo, ma possono essere ripetuti tra campi diversi.

* La ridenominazione di una scelta non ne aggiorna il valore originale.

* I valori di scelta vengono visualizzati in minuscolo e sono separati da trattini bassi nel caso di scelte tra più parole. Se utilizzi un’etichetta già utilizzata come altro nome di scelta per lo stesso campo, Workfront aggiunge al valore un numero sequenziale.

Per informazioni, vedere [Creare i campi](/help/quicksilver/planning/fields/create-fields.md).