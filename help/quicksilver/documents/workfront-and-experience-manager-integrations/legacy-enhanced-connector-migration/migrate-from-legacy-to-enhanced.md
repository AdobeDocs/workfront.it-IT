---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Migrare dal connettore legacy al connettore avanzato
description: Il seguente processo illustra le best practice per lo spostamento dal connettore legacy di Adobe Experience Manager al connettore avanzato per l’integrazione di Adobe Workfront con AEM Assets.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4a8d1e2b-9744-4f72-a337-5057448db4fb
source-git-commit: 3a1bc4a56cba2fe224a1f0a21c8882c2d9d030de
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---

# Migrare dal connettore legacy al connettore avanzato

Il seguente processo illustra le best practice per lo spostamento dal connettore legacy di Adobe Experience Manager al connettore avanzato per l’integrazione di Adobe Workfront con AEM Assets.

>[!IMPORTANT]
>
>Questa documentazione si applica solo ai clienti che utilizzano ambienti Adobe Experience Manager Assets On-Premise o Managed Services.


Per i clienti che utilizzano Adobe Experience Manager Assets as a Cloud Service, il percorso di migrazione dal connettore legacy sarà alla nuova integrazione nativa all’interno di Workfront. Per ulteriori informazioni su questo processo di migrazione, consulta [Migrazione dal connettore legacy o avanzato ad Workfront per l’integrazione con Adobe Experience Manager as a Cloud Service](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/migrate-from-legacy-enhanced-connectors.md).

## Implementare il connettore avanzato

>[!IMPORTANT]
>
>Per l’implementazione del connettore avanzato è necessario un partner certificato o un servizio di consulenza Adobe.
>
> Per i partner che desiderano certificare il connettore avanzato, consulta il seguente articolo: [Workfront per Experience Manager connettore avanzato serie Expert](https://experienceleague.adobe.com/docs/experience-manager-learn/assets/workfront/enhanced-connector/aem-experts-series/overview.html?lang=en).

Per implementare il connettore avanzato, vedi [Configurazione di Workfront per un connettore migliorato ad Experience Manager](https://experienceleague.adobe.com/docs/experience-manager-65/assets/integrations/workfront-connector-configure.html?lang=en).


## Spostare le risorse esistenti

Dopo aver configurato l’ambiente, puoi spostare le risorse e le cartelle collegate esistenti in Adobe Experience Manager. Questo è un passaggio facoltativo, ma assicurerà che le cartelle e le risorse precedentemente collegate tramite il connettore legacy siano ancora accessibili dopo la disinstallazione del connettore legacy.

Per ulteriori informazioni sullo spostamento delle risorse, consulta [Migrazione di cartelle e documenti collegati](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/workfront-document-link-updates.md).

## Convalida tutti i casi d’uso critici destinati all’uso

È importante convalidare tutti i casi d’uso critici destinati all’uso tramite il connettore avanzato prima di disinstallare il connettore legacy.

## Disinstallare il connettore legacy

Infine, devi disinstallare il connettore legacy. Il connettore legacy non deve essere eseguito in parallelo con il connettore avanzato.

Per disinstallare, vedi [Disinstallare Workfront con il connettore legacy Adobe Experience Manager](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-legacy-connector.md).
