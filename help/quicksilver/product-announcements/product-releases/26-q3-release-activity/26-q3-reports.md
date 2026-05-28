---
title: Miglioramenti al reporting per il terzo trimestre 2026
description: Miglioramenti al reporting per il terzo trimestre 2026
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: a177e2887c2b8b281b19cda45ce59c6f8149cefb
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 4%

---

# Miglioramenti al reporting per il terzo trimestre 2026

Questa pagina descrive i miglioramenti apportati all’ambiente di anteprima nella versione del terzo trimestre 2026 per la generazione di rapporti. Tali miglioramenti saranno resi disponibili nell’ambiente di produzione come indicato.

Per un elenco di tutte le modifiche disponibili al momento nel ciclo di rilascio del terzo trimestre 2026, consulta [Panoramica sulla versione del terzo trimestre 2026](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-release-overview.md).

## Campi di dati valuta personalizzati nei rapporti del dashboard Area di lavoro

>[!NOTE]
>
>Anteprima: 28 maggio 2026>Rilascio rapido produzione: 11 giugno 2026>Produzione per tutti: 16 luglio 2026

I rapporti del dashboard Canvas ora supportano campi di dati valuta personalizzati come colonne, filtri, raggruppamenti e aggregazioni, anche quando nella configurazione del sistema sono configurati più tassi di cambio. Quando un campo dati valuta personalizzato viene visualizzato come colonna o aggregazione, i valori vengono convertiti nella valuta selezionata nell’interruttore del tasso di cambio del dashboard, a meno che il campo non sia bloccato a livello di report.

Vengono ora visualizzati i rapporti che in precedenza non riuscivano con un messaggio di &quot;campo limitato&quot; dopo l’aggiunta di una seconda valuta del tasso di cambio. I campi della valuta di pianificazione rimangono limitati quando vengono definiti più tassi di cambio.

Per ulteriori informazioni, vedere [Utilizzare i campi di valuta nei dashboard di Canvas](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-canvas-dashboards/switch-currencies.md).

## Miglioramento della precisione dei dati nei rapporti del dashboard di Canvas

>[!NOTE]
>
>Anteprima: 14 maggio 2026>Rilascio rapido produzione: 11 giugno 2026>Produzione per tutti: 16 luglio 2026
>
>Canvas Dashboards è attualmente in versione beta.

I dashboard dell’area di lavoro ora strutturano le query dei rapporti in modo da evitare righe duplicate quando i filtri o i campi attraversano record correlati, in modo che i conteggi, le somme e altri aggregati restituiscano valori precisi.

In precedenza, un join tra record correlati poteva ripetere i record padre una volta per ogni record correlato. Ad esempio, in un report di progetto filtrato per le attività assegnate a un utente specifico, ogni progetto viene ripetuto una volta per ogni attività corrispondente. Un indicatore KPI con il budget del progetto sommato potrebbe mostrare 6.000 dollari invece dei 1.250 dollari corretti.

Non sono state apportate modifiche all’interfaccia del dashboard di Canvas. I rapporti esistenti restituiscono automaticamente dati precisi dopo questa versione.
