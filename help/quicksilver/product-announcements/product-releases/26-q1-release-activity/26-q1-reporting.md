---
title: Miglioramenti al reporting per il primo trimestre 2026
description: Miglioramenti al reporting per il primo trimestre 2026
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 00483638948941c933e5f8bc8cb3edaf8e43fea1
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 0%

---

# Miglioramenti al reporting per il primo trimestre 2026

Questa pagina descrive i miglioramenti apportati all’ambiente di anteprima nella versione del primo trimestre 2026 per la generazione di rapporti. Questi miglioramenti saranno resi disponibili nell’ambiente di produzione come indicato.

Per un elenco di tutte le modifiche disponibili al momento nel ciclo di rilascio del primo trimestre 2026, consulta [Panoramica sulla versione del primo trimestre 2026](/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-release-overview.md).

## Duplicare un rapporto in un dashboard Canvas

>[!NOTE]
>
>Versione di anteprima: 23 ottobre 2025
>Produzione per tutti i clienti: 23 ottobre 2025
>[!BADGE Fuori programma]{type=Neutral}

È ora possibile duplicare un rapporto indicatore KPI, tabella o grafico in un dashboard di Canvas dopo averlo creato. Una volta duplicato, puoi modificare il rapporto in base alle esigenze prima di salvarlo.

## Rimozione delle opzioni dei campi dai filtri dei rapporti

>[!NOTE]
>
>Anteprima: 6 novembre 2025
>Versione rapida di produzione: 13 novembre 2025
>Produzione per tutti: 15 gennaio 2026

Sono state rimosse le seguenti opzioni di campo precedentemente disponibili durante l’applicazione di un filtro a un rapporto:

* ID di altri gruppi
* Altri ID Ruoli
* ID altri team

Questi sono stati rimossi a causa di problemi associati agli operatori Not Equal e Is Blank. Se disponi di un filtro esistente che utilizza uno di questi campi, questo continuerà a funzionare come previsto. In alternativa, è possibile continuare a utilizzare questi campi in <code>modalità testo</code>, ma si consiglia di evitare di utilizzare gli operatori Not Equal o Is Blank.

In alternativa, sono disponibili le seguenti opzioni di campo:

* Altri gruppi: ID
* Altri ruoli: ID
* Altri team: ID

## Visualizzazione migliorata del conteggio dei raggruppamenti nei dashboard di Canvas

>[!NOTE]
>
>Anteprima: 6 novembre 2025
>Versione rapida di produzione: 13 novembre 2025
>Produzione per tutti: 15 gennaio 2026

Quando un report tabella include più pagine di risultati e la tabella è configurata con raggruppamenti, la tabella visualizza ora sia la quantità di record per la pagina corrente che il conteggio di record complessivo per tutte le pagine. Ad esempio, se il rapporto di tabella ha 7 raggruppamenti e la prima pagina mostra 3, la tabella visualizzerà 3 di 7.


## Nuove protezioni per migliorare i tempi di caricamento nei dashboard di Canvas

>[!NOTE]
>
>Anteprima: 6 novembre 2025
>Versione rapida di produzione: 13 novembre 2025
>Produzione per tutti: 15 gennaio 2026

Per evitare ritardi nei tempi di caricamento e migliorare le prestazioni complessive nei dashboard di Canvas, sono stati applicati limiti al numero di componenti del dashboard che è possibile aggiungere a un dashboard:

* Report per dashboard: limite 25
* Raggruppamenti su viste tabella: limite 5
* Distanza dall&#39;oggetto di base del report: limite 10
* Colonne in una vista a tabella: limite 25
* Richieste filtro a livello di dashboard: limite 10