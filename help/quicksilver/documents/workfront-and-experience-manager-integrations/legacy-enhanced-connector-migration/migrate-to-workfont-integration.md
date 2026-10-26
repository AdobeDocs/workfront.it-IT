---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Migrare dal connettore legacy o avanzato a Workfront per l’integrazione con Adobe Experience Manager as a Cloud Service
description: Le informazioni contenute in questa pagina illustrano le best practice per passare dai connettori avanzati o legacy di Workfront for Experience Cloud all’integrazione nativa più recente che collega Workfront e Adobe Experience Manager Assets as a Cloud Service.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: af14f408-df39-473c-9e18-bb88022c96ed
TQID: 'https://experienceleague.adobe.com/0pAHfS7cDqv1tV4TBdx9WqvJA1-zySGsPHVXI8EG7Hc'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
    internal-label: Integrations
  - id: a1f87682-0525-5459-aa06-3560bb4c3b2a
    internal-label: Workfront Integrations and Apps
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: e7123179a59cd7ed9c76f4718b3b8019854cbfe1
workflow-type: tm+mt
source-wordcount: '344'
ht-degree: 0%
---
# Migrare dal connettore legacy o avanzato a Workfront per l’integrazione con Adobe Experience Manager as a Cloud Service

Le informazioni contenute in questa pagina illustrano le best practice per passare dai connettori avanzati o legacy di Workfront for Experience Cloud all’integrazione nativa più recente che collega Workfront e Adobe Experience Manager Assets as a Cloud Service.

>[!IMPORTANT]
>
>Queste informazioni non sono applicabili ai clienti che utilizzano ambienti Adobe Experience Manager Assets On-Premise o Managed Services.

<!--

## Move your Workfront instance to the Admin Console

Customers that intend to use the new native integration between Workfront and Adobe Experience Manager Assets as a Cloud Service must ensure their Workfront environment is tied to an Adobe Admin Console. For existing Workfront environments, this will likely require a migration of the environment to a connected Adobe Admin Console. For more details regarding this migration and the associated checklist, see [Prepare to onboard your organization to the Adobe Admin Console](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md). 

 Adobe must help carry out this migration. To request help, do one of the following:

* If you have Workfront Hub access, submit your request to the [Workfront Migration to Adobe Admin Console](https://hub.workfront.com/requests/new?activeTab=tab-new-helpRequest&projectID=629674d500054a38133cf26e01d06a97&path=).
* If you do not have Workfront Hub access, you can submit your request to the [Workfront to Adobe Admin Console Early Migration Request Queue](https://workfront.az1.qualtrics.com/jfe/form/SV_9T5LuHf05JUOPAi).

-->

## Configurare la nuova integrazione Workfront for Adobe Experience Manager assets as a Cloud Service

Dopo la migrazione dell’ambiente Workfront a un Adobe Admin Console, gli amministratori di Workfront possono configurare la nuova integrazione nativa. Per informazioni sulla configurazione, vedere [Configurare l&#39;integrazione Experience Manager Assets as a Cloud Service](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).

## Spostare le risorse esistenti nell’integrazione Workfront for Adobe Experience Manager assets as a Cloud Service

Dopo aver configurato l’ambiente, puoi spostare le risorse e le cartelle collegate esistenti in Adobe Experience Manager. Questo passaggio è facoltativo, ma assicurerà che le cartelle e le risorse collegate in precedenza tramite il connettore legacy o avanzato siano ancora accessibili dopo la disinstallazione di tali connettori.

Per ulteriori informazioni sullo spostamento delle risorse, consulta [Migrare cartelle e documenti collegati](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/workfront-document-link-updates.md).

## Convalidare tutti i casi d’uso critici che si intende utilizzare

Prima di disinstallare il connettore legacy o avanzato, è importante convalidare tutti i casi d’uso critici che devono essere utilizzati tramite l’integrazione nativa.

## Disinstallare il connettore legacy o avanzato

Infine, devi disinstallare il connettore legacy o avanzato. L’integrazione nativa non deve essere eseguita in parallelo con nessuno dei connettori.

Per disinstallare, vedi

* Istruzioni per la disinstallazione del connettore legacy: [Disinstallare Workfront con il connettore legacy di Adobe Experience Manager](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-legacy-connector.md).
* Istruzioni per la disinstallazione del connettore avanzato: [Disinstallare Workfront con il connettore avanzato di Adobe Experience Manager](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-enhanced-connector.md).
