---
content-type: release-notes
title: Attività della versione del primo trimestre 2026 per Adobe Workfront Planning
description: Questa è l’attività di rilascio per il prodotto Adobe Workfront Planning per il primo trimestre 2026.
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: 1e830ccb4e87c231f57ae39e59988bb261737188
workflow-type: tm+mt
source-wordcount: '979'
ht-degree: 0%

---

# Attività della versione del primo trimestre 2026 per Adobe Workfront Planning

Questo articolo descrive le funzioni rilasciate per Workfront Planning durante la versione del primo trimestre 2026.

<!--keep the sentence below for all future quarterly release pages-->

Per un elenco di tutte le funzionalità rilasciate per Adobe Workfront Planning, vedere [Attività di rilascio di Adobe Workfront Planning: indice articolo](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).

## Aggiunta del campo Connessione marchio a Prodotti e utenti tipo per impostazione predefinita nell’area di lavoro di GenStudio

>[!NOTE]
>
>Anteprima: 11 dicembre 2025
>Versione rapida di produzione: 11 dicembre 2025
>Produzione per tutti: 11 dicembre 2025

Il campo di connessione con il marchio GenStudio for Performance Marketing viene ora aggiunto per impostazione predefinita ai tipi di record Prodotti e utenti tipo nell’area di lavoro GenStudio di Workfront Planning.

La tua organizzazione deve avere sia Workfront Planning che Adobe GenStudio for Performance Marketing.

Prima di questo miglioramento, era possibile aggiungere il campo di connessione al marchio solo manualmente a qualsiasi tipo di record, inclusi Prodotti e utenti tipo. È comunque possibile collegare manualmente il tipo di record di Brand GenStudio ad altri tipi di record in Workfront Planning.

Per informazioni, vedere [Introduzione all&#39;integrazione di Adobe Workfront Planning e Adobe GenStudio for Performance Marketing](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md).

## Limita la rimozione delle autorizzazioni degli utenti di GenStudio for Performance Marketing da Planning

>[!NOTE]
>
>Anteprima: 11 dicembre 2025
>Versione rapida di produzione: 11 dicembre 2025
>Produzione per tutti: 11 dicembre 2025

È stato aggiunto un guardrail che impedisce la rimozione delle autorizzazioni degli utenti di GenStudio for Performance Marketing dagli oggetti di Workfront Planning. Grazie a questo miglioramento, non sarà più possibile rimuovere gli utenti di GenStudio dall&#39;area di lavoro di GenStudio in Planning, né disabilitare le autorizzazioni ereditate per i tipi di record nell&#39;area di lavoro di GenStudio, se tali autorizzazioni includono gli utenti di GenStudio. Prima di questo miglioramento, se rimuovessi questi utenti dall’area di lavoro di GenStudio in Planning, perderebbero le autorizzazioni per i tipi di record anche in GenStudio.

La tua organizzazione deve avere sia Workfront Planning che Adobe GenStudio for Performance Marketing.

Per informazioni, vedere [Introduzione all&#39;integrazione di Adobe Workfront Planning e Adobe GenStudio for Performance Marketing](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md).


## È stata rimossa la condivisione pubblica delle viste su un tipo di record globale in un’area di lavoro secondaria


>[!NOTE]
>
>Anteprima: 3 dicembre 2025
>Versione rapida di produzione: 4 dicembre 2025
>Produzione per tutti: 15 gennaio 2026


È stata rimossa la scheda Condivisione pubblica quando si condivideva una vista per un record globale in un’area di lavoro secondaria. Non è possibile condividere una visualizzazione pubblicamente da un tipo di record globale aggiunto a un&#39;altra area di lavoro da un tipo di record globale esistente. È possibile condividere una visualizzazione del tipo di record globale pubblicamente dalla relativa area di lavoro originale.

Per informazioni, vedere [Condividi visualizzazioni](/help/quicksilver/planning/access/share-views.md).


## Collegare i marchi GenStudio for Performance Marketing ai tipi di record di Workfront Planning

>[!NOTE]
>
>Anteprima: 13 novembre 2025
>Versione rapida di produzione: 13 novembre 2025
>Produzione per tutti: 13 novembre 2025

È ora possibile collegare i tipi di record di Workfront Planning ai Marchi di Adobe GenStudio for Performance Marketing. La tua organizzazione deve avere sia Workfront Planning che Adobe GenStudio for Performance Marketing.

Per ulteriori informazioni, vedere [Connetti tipi di record](/help/quicksilver/planning/architecture/connect-record-types.md).


## Nuova casella di ricerca dei campi nelle icone Filtri, Campi e Colori riga nelle visualizzazioni di Planning

>[!NOTE]
>
>Anteprima: 6 novembre 2025
>Versione rapida di produzione: 11 dicembre 2025
>Produzione per tutti: 15 gennaio 2026

È ora possibile cercare un campo specifico durante la creazione di un elemento di visualizzazione in una visualizzazione del tipo di record. Sono state aggiunte caselle di ricerca quando si crea un filtro, si ordina, si raggruppa o quando si configurano i campi o i colori delle righe. Prima di questo miglioramento, era sufficiente scorrere l’elenco dei campi disponibili.

Questo miglioramento è disponibile in tutte le visualizzazioni dei tipi di record.

Per informazioni, vedere [Gestire la visualizzazione della tabella](/help/quicksilver/planning/views/manage-the-table-view.md).


## Tipi di record globali e la possibilità di aggiungerli come tipi di record esistenti ad altre aree di lavoro

>[!NOTE]
>
>Anteprima: 16 ottobre 2025
>Versione rapida di produzione: 13 novembre 2025
>Produzione per tutti: 15 gennaio 2026

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
>Versione rapida di produzione: 13 novembre 2025
>Produzione per tutti: 15 gennaio 2026

È stato introdotto un limite di 30 campi di connessione per ogni tipo di record.

NOTA: se l&#39;organizzazione dispone attualmente di più di 30 campi di connessione per un tipo di record, è possibile mantenere i campi aggiuntivi che superano il limite di 30. Non è tuttavia possibile aggiungere altri campi di connessione ai tipi di record che superano il limite. In futuro, verrà applicato il nuovo limite di 30 campi di connessione.

Per ulteriori informazioni, vedere [Panoramica sui tipi di record connessi](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

## Impostare valori descrittivi per le scelte dei campi di tipo selezionato

>[!NOTE]
>
>Anteprima: 16 ottobre 2025
>Versione rapida di produzione: 13 novembre 2025
>Produzione per tutti: 15 gennaio 2026

Quando si aggiungono scelte di campo a un campo a selezione singola o multipla, Workfront assegnerà valori univoci di facile utilizzo a ciascuna scelta. Prima di questo miglioramento, Workfront generava un ID alfanumerico difficile da comprendere e utilizzare nelle chiamate API e in altre integrazioni.

Considera quanto segue con questo miglioramento:

* I nuovi valori verranno aggiunti alle nuove scelte di campo. Le scelte di campo esistenti manterranno i loro ID alfanumerici.

* I valori di scelta sono univoci per un campo, ma possono essere ripetuti tra campi diversi.

* La ridenominazione di una scelta non ne aggiorna il valore originale.

* I valori di scelta vengono visualizzati in minuscolo e sono separati da trattini bassi nel caso di scelte tra più parole. Se utilizzi un’etichetta già utilizzata come altro nome di scelta per lo stesso campo, Workfront aggiunge al valore un numero sequenziale.

Per informazioni, vedere [Creare i campi](/help/quicksilver/planning/fields/create-fields.md).