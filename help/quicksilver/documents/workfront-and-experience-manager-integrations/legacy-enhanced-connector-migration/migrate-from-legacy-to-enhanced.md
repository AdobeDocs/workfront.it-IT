---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Migrare dal connettore legacy al connettore avanzato
description: Il processo seguente illustra le best practice per passare dal connettore legacy di Adobe Experience Manager al connettore avanzato per l’integrazione di Adobe Workfront con AEM Assets.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4a8d1e2b-9744-4f72-a337-5057448db4fb
TQID: https://experienceleague.adobe.com/px8ysyDqpwzajmCfRPJLclKOUSuIFacl99Uf6sRCKFQ
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 356
ht-degree: 5%

---

# Migrare dal connettore legacy al connettore avanzato

Il processo seguente illustra le best practice per passare dal connettore legacy di Adobe Experience Manager al connettore avanzato per l’integrazione di Adobe Workfront con AEM Assets.

>[!IMPORTANT]
>
>Questa documentazione è valida solo per i clienti che utilizzano ambienti Adobe Experience Manager Assets On-Premise o Managed Services.


Per i clienti che utilizzano Adobe Experience Manager Assets as a Cloud Service, il percorso di migrazione dal connettore legacy sarà alla nuova integrazione nativa all’interno di Workfront. Per ulteriori informazioni sul processo di migrazione, vedere [Migrare dal connettore legacy o avanzato a Workfront per l&#39;integrazione con Adobe Experience Manager as a Cloud Service](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/migrate-from-legacy-enhanced-connectors.md).

## Implementare il connettore avanzato

>[!IMPORTANT]
>
>Per l’implementazione del connettore avanzato sono necessari un partner certificato o i servizi Adobe Consulting.
>
> Per i partner che desiderano certificare sul connettore avanzato, leggere il seguente articolo: [Workfront per la serie Expert del connettore avanzato Experience Manager](https://experienceleague.adobe.com/it/docs/experience-manager-learn/assets/workfront/enhanced-connector/aem-experts-series/overview).

Per implementare il connettore avanzato, vedere [Configurare il connettore avanzato di Workfront per Experience Manager](https://experienceleague.adobe.com/it/docs/experience-manager-65/content/assets/integrations/workfront-connector-configure).


## Spostare le risorse esistenti

Dopo aver configurato l’ambiente, puoi spostare le risorse e le cartelle collegate esistenti in Adobe Experience Manager. Questo passaggio è facoltativo, ma assicurerà che le cartelle e le risorse collegate in precedenza tramite il connettore legacy siano ancora accessibili dopo la disinstallazione del connettore legacy.

Per ulteriori informazioni sullo spostamento delle risorse, consulta [Migrare cartelle e documenti collegati](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/workfront-document-link-updates.md).

## Convalidare tutti i casi d’uso critici che si intende utilizzare

Prima di disinstallare il connettore legacy, è importante convalidare tutti i casi d’uso critici che devono essere utilizzati tramite il connettore avanzato.

## Disinstalla il connettore legacy

Infine, devi disinstallare il connettore legacy. Il connettore legacy non deve essere eseguito in parallelo al connettore avanzato.

Per disinstallare, vedere [Disinstallare Workfront con il connettore legacy di Adobe Experience Manager](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-legacy-connector.md).
