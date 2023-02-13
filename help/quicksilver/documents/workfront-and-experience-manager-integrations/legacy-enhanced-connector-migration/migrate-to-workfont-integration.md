---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Migrazione dal connettore legacy o avanzato ad Workfront per l’integrazione con Adobe Experience Manager as a Cloud Service
description: Le informazioni presenti in questa pagina illustrano le best practice per passare da Workfront, ad Experience Cloud connettori avanzati o legacy, all’integrazione nativa più recente che collega Workfront e Adobe Experience Manager Assets as a Cloud Service.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: af14f408-df39-473c-9e18-bb88022c96ed
source-git-commit: 3a1bc4a56cba2fe224a1f0a21c8882c2d9d030de
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 0%

---

# Migrazione dal connettore legacy o avanzato ad Workfront per l’integrazione con Adobe Experience Manager as a Cloud Service

Le informazioni presenti in questa pagina illustrano le best practice per passare da Workfront, ad Experience Cloud connettori avanzati o legacy, all’integrazione nativa più recente che collega Workfront e Adobe Experience Manager Assets as a Cloud Service.

>[!IMPORTANT]
>
>Queste informazioni non si applicano ai clienti che utilizzano ambienti Adobe Experience Manager Assets On-Premise o Managed Services.

## Sposta l’istanza Workfront all’Admin Console

I clienti che intendono utilizzare la nuova integrazione nativa tra Workfront e Adobe Experience Manager Assets as a Cloud Service devono assicurarsi che il proprio ambiente Workfront sia associato a un Adobe Admin Console. Per gli ambienti Workfront esistenti, questo richiederà probabilmente una migrazione dell’ambiente a un Adobe Admin Console connesso. Per ulteriori dettagli su questa migrazione e sulla relativa lista di controllo, vedi [Preparati a integrare l’organizzazione in Adobe Admin Console](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md).

L&#39;Adobe deve contribuire a questa migrazione. Per richiedere assistenza, effettua una delle seguenti operazioni:

* Se disponi dell’accesso a Workfront Hub, invia la richiesta al [Migrazione Workfront a Adobe Admin Console](https://hub.workfront.com/requests/new?activeTab=tab-new-helpRequest&amp;projectID=629674d500054a38133cf26e01d06a97&amp;path=).
* Se non disponi dell’accesso a Workfront Hub, puoi inviare la richiesta al [Coda di richiesta di migrazione anticipata da Workfront a Adobe Admin Console](https://workfront.az1.qualtrics.com/jfe/form/SV_9T5LuHf05JUOPAi).

## Configurare il nuovo Workfront per l’integrazione as a Cloud Service delle risorse di Adobe Experience Manager

Dopo la migrazione dell’ambiente Workfront a un Adobe Admin Console, gli amministratori Workfront possono configurare la nuova integrazione nativa. Per assistenza sulla configurazione, consulta [Configurare l’integrazione as a Cloud Service di Experience Manager Assets](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).

## Sposta le risorse esistenti al tuo Workfront per l’integrazione as a Cloud Service delle risorse di Adobe Experience Manager

Dopo aver configurato l’ambiente, puoi spostare le risorse e le cartelle collegate esistenti in Adobe Experience Manager. Questo è un passaggio facoltativo, ma assicurerà che le cartelle e le risorse precedentemente collegate tramite il connettore legacy o avanzato siano ancora accessibili una volta che tali connettori sono stati disinstallati.

Per ulteriori informazioni sullo spostamento delle risorse, consulta [Migrazione di cartelle e documenti collegati](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/workfront-document-link-updates.md).

## Convalida tutti i casi d’uso critici destinati all’uso

Sarà importante convalidare tutti i casi d’uso critici destinati all’utilizzo tramite l’integrazione nativa prima di disinstallare il connettore legacy o avanzato.

## Disinstallare il connettore legacy o avanzato

Infine, devi disinstallare il connettore legacy o avanzato. L’integrazione nativa non deve essere eseguita in parallelo con entrambi i connettori.

Per disinstallare, vedi

* Istruzioni per la disinstallazione del connettore legacy: [Disinstallare Workfront con il connettore legacy Adobe Experience Manager](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-legacy-connector.md).
* Istruzioni per la disinstallazione del connettore avanzato: [Disinstallare Workfront con il connettore avanzato Adobe Experience Manager](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-enhanced-connector.md).
