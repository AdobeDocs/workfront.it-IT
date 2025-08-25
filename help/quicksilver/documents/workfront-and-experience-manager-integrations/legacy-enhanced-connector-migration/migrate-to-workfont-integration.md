---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Migrare dal connettore legacy o avanzato a Workfront per l’integrazione con Adobe Experience Manager as a Cloud Service
description: Le informazioni contenute in questa pagina illustrano le best practice per passare dai connettori avanzati o legacy di Workfront for Experience Cloud all’integrazione nativa più recente che collega Workfront e Adobe Experience Manager Assets as a Cloud Service.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: af14f408-df39-473c-9e18-bb88022c96ed
source-git-commit: a25eb28800ca8bbeeffedb521b3d72c8df71c697
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 0%

---

# Migrare dal connettore legacy o avanzato a Workfront per l’integrazione con Adobe Experience Manager as a Cloud Service

Le informazioni contenute in questa pagina illustrano le best practice per passare dai connettori avanzati o legacy di Workfront for Experience Cloud all’integrazione nativa più recente che collega Workfront e Adobe Experience Manager Assets as a Cloud Service.

>[!IMPORTANT]
>
>Queste informazioni non sono applicabili ai clienti che utilizzano ambienti Adobe Experience Manager Assets On-Premise o Managed Services.

## Spostare l’istanza Workfront in Admin Console

I clienti che intendono utilizzare la nuova integrazione nativa tra Workfront e Adobe Experience Manager Assets as a Cloud Service devono assicurarsi che il proprio ambiente Workfront sia associato a un Adobe Admin Console. Per gli ambienti Workfront esistenti, questo richiederà probabilmente una migrazione dell’ambiente a un Adobe Admin Console connesso. Per ulteriori dettagli su questa migrazione e sull&#39;elenco di controllo associato, vedere [Preparare l&#39;onboarding dell&#39;organizzazione in Adobe Admin Console](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md).

Adobe deve contribuire a eseguire questa migrazione. Per richiedere assistenza, eseguire una delle operazioni seguenti:

* Se disponi dell&#39;accesso Hub Workfront, invia la tua richiesta a [Migrazione Workfront a Adobe Admin Console](https://hub.workfront.com/requests/new?activeTab=tab-new-helpRequest&projectID=629674d500054a38133cf26e01d06a97&path=).
* Se non disponi dell&#39;accesso a Workfront Hub, puoi inviare la tua richiesta alla [Coda richieste di migrazione anticipata da Workfront a Adobe Admin Console](https://workfront.az1.qualtrics.com/jfe/form/SV_9T5LuHf05JUOPAi).

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
