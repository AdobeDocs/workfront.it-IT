---
title: Miglioramenti al reporting per il terzo trimestre 2026
description: Miglioramenti al reporting per il terzo trimestre 2026
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 9a86968cf8fff2c7c930aa6c8408ab8566905cb8
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 6%

---

# Miglioramenti al reporting per il terzo trimestre 2026

Questa pagina descrive i miglioramenti apportati all’ambiente di anteprima nella versione del terzo trimestre 2026 per la generazione di rapporti. Tali miglioramenti saranno resi disponibili nell’ambiente di produzione come indicato.

Per un elenco di tutte le modifiche disponibili al momento nel ciclo di rilascio del terzo trimestre 2026, consulta [Panoramica sulla versione del terzo trimestre 2026](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-release-overview.md).

## Miglioramento della precisione dei dati nei rapporti del dashboard di Canvas

>[!NOTE]
>
>Anteprima: 14 maggio 2026>Versione rapida di produzione: 11 giugno 2026>Produzione per tutti: 16 luglio 2026
>
>Canvas Dashboards è attualmente in versione beta.

I dashboard dell’area di lavoro ora strutturano le query dei rapporti in modo da evitare righe duplicate quando i filtri o i campi attraversano record correlati, in modo che i conteggi, le somme e altri aggregati restituiscano valori precisi.

In precedenza, un join tra record correlati poteva ripetere i record padre una volta per ogni record correlato. Ad esempio, in un report di progetto filtrato per le attività assegnate a un utente specifico, ogni progetto viene ripetuto una volta per ogni attività corrispondente. Un indicatore KPI con il budget del progetto sommato potrebbe mostrare 6.000 dollari invece dei 1.250 dollari corretti.

Non sono state apportate modifiche all’interfaccia del dashboard di Canvas. I rapporti esistenti restituiscono automaticamente dati precisi dopo questa versione.
