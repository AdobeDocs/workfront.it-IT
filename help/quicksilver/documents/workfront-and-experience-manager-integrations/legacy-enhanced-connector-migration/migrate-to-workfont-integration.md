---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Migrare dal connettore legacy o avanzato a Workfront per l’integrazione con Adobe Experience Manager as a Cloud Service
description: Le informazioni contenute in questa pagina illustrano le best practice per passare da Workfront, ad Experience Cloud connettori avanzati o legacy, alla più recente integrazione nativa che collega Workfront e Adobe Experience Manager Assets as a Cloud Service.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: af14f408-df39-473c-9e18-bb88022c96ed
source-git-commit: 3a1bc4a56cba2fe224a1f0a21c8882c2d9d030de
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 0%

---

# Migrare dal connettore legacy o avanzato a Workfront per l’integrazione con Adobe Experience Manager as a Cloud Service

Le informazioni contenute in questa pagina illustrano le best practice per passare da Workfront, ad Experience Cloud connettori avanzati o legacy, alla più recente integrazione nativa che collega Workfront e Adobe Experience Manager Assets as a Cloud Service.

>[!IMPORTANT]
>
>Queste informazioni non sono applicabili ai clienti che utilizzano ambienti Adobe Experience Manager Assets On-Premise o Managed Services.

## Sposta l’istanza Workfront nell’Admin Console

I clienti che intendono utilizzare la nuova integrazione nativa tra Workfront e Adobe Experience Manager Assets as a Cloud Service devono assicurarsi che il proprio ambiente Workfront sia associato a un Adobe Admin Console. Per gli ambienti Workfront esistenti, questo richiederà probabilmente una migrazione dell’ambiente a un Adobe Admin Console connesso. Per ulteriori dettagli su questa migrazione e sull’elenco di controllo associato, consulta [Prepara l’onboarding della tua organizzazione in Adobe Admin Console](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md).

L&#39;Adobe deve contribuire a realizzare questa migrazione. Per richiedere assistenza, eseguire una delle operazioni seguenti:

* Se disponi dell’accesso a Workfront Hub, invia la richiesta al [Migrazione di Workfront a Adobe Admin Console](https://hub.workfront.com/requests/new?activeTab=tab-new-helpRequest&amp;projectID=629674d500054a38133cf26e01d06a97&amp;path=).
* Se non disponi dell’accesso a Workfront Hub, puoi inviare la richiesta a [Coda di richieste di migrazione anticipata da Workfront a Adobe Admin Console](https://workfront.az1.qualtrics.com/jfe/form/SV_9T5LuHf05JUOPAi).

## Configurare la nuova integrazione as a Cloud Service di Workfront for Adobe Experience Manager Assets

Dopo la migrazione dell’ambiente Workfront a un Adobe Admin Console, gli amministratori di Workfront possono configurare la nuova integrazione nativa. Per assistenza sulla configurazione, consulta [Configurare l’integrazione di Experience Manager Assets as a Cloud Service](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).

## Spostare le risorse esistenti nell’integrazione as a Cloud Service di Workfront for Adobe Experience Manager assets

Dopo aver configurato l’ambiente, puoi spostare le risorse e le cartelle collegate esistenti in Adobe Experience Manager. Questo passaggio è facoltativo, ma assicurerà che le cartelle e le risorse collegate in precedenza tramite il connettore legacy o avanzato siano ancora accessibili dopo la disinstallazione di tali connettori.

Per ulteriori informazioni sullo spostamento delle risorse, consulta [Eseguire la migrazione di cartelle e documenti collegati](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/workfront-document-link-updates.md).

## Convalidare tutti i casi d’uso critici che si intende utilizzare

Prima di disinstallare il connettore legacy o avanzato, è importante convalidare tutti i casi d’uso critici che devono essere utilizzati tramite l’integrazione nativa.

## Disinstallare il connettore legacy o avanzato

Infine, devi disinstallare il connettore legacy o avanzato. L’integrazione nativa non deve essere eseguita in parallelo con nessuno dei connettori.

Per disinstallare, vedi

* Istruzioni per la disinstallazione del connettore legacy: [Disinstallare Workfront con il connettore legacy di Adobe Experience Manager](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-legacy-connector.md).
* Istruzioni per la disinstallazione del connettore avanzato: [Disinstallare il Workfront con il connettore avanzato Adobe Experience Manager](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-enhanced-connector.md).
