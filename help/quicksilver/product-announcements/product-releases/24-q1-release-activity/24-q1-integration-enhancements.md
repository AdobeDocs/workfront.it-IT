---
title: Miglioramenti all’integrazione per il primo trimestre 2024
description: Miglioramenti all’integrazione per il primo trimestre 2024
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 0d581f3c-2aaf-4ac1-97a5-df1b01627080
TQID: https://experienceleague.adobe.com/ZPt9H-R2eSNNha-gjfwkgnUOQqvU5tzAQPE5fMA-9uA
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aadid: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dcid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 385
ht-degree: 0%

---

# Miglioramenti all’integrazione per il primo trimestre 2024

Questa pagina descrive tutti i miglioramenti all’integrazione apportati con la versione del primo trimestre 2024 all’ambiente di anteprima. Questi miglioramenti saranno resi disponibili nell’ambiente di produzione con la versione del primo trimestre 2024.

Per un elenco di tutte le modifiche disponibili al momento nel ciclo di rilascio del primo trimestre 2024, consulta [Panoramica sulla versione del primo trimestre 2024](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).

## La mappatura dei metadati in Experience Manager Assets Essentials ora utilizza `xcm:keywords` invece di `dc:subject`

Abbiamo aggiornato l’integrazione di Experience Manager Assets Essentials per adattarla all’esperienza nell’integrazione di Experience Manager Assets as a Cloud Service. Ora, quando si mappano più campi di testo a riga singola a un singolo campo in Experience Manager Assets, entrambi i servizi utilizzano il campo `xcm:keywords`.

In precedenza, questi campi venivano mappati al campo `dc:subject` in Experience Manager Assets Essentials. La funzionalità as a Cloud Service di Experience Manager Assets è invariata.

Eventuali metadati di Experience Manager Assets Essentials attualmente mappati a `dc:subject` devono essere rimappati a `xcm:keywords`.

Per informazioni sulla mappatura dei metadati su Experience Manager Assets Essentials, vedi [Parola chiave AEM](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md#aem-keyword).

## I campi typeahead sono ora disponibili nell’integrazione di Adobe Experience Manager

Per semplificare il collegamento dei campi tra Workfront e Adobe Experience Manager, è stato aggiunto il supporto dei campi typeahead nella mappatura dei metadati. Ora è possibile mappare i campi typeahead ai campi corrispondenti in Adobe Experience Manager.

Se un utente seleziona un valore diverso per un campo in Workfront, tale modifica si riflette immediatamente in Adobe Experience Manager. Inoltre, se l’opzione del valore di un campo cambia (ad esempio, se un team ne cambia il nome in un nuovo nome), la modifica si riflette anche in Adobe Experience Manager.

Per informazioni e istruzioni sulla mappatura dei metadati nell&#39;integrazione di Adobe Experience Manager, vedere [Configurare i metadati](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-metadata-optional).

## Pubblicare automaticamente le risorse in Adobe Experience Manager

È stato aggiunto un altro flusso di lavoro all’integrazione Adobe Experience Manager. Ora puoi impostare la pubblicazione automatica delle risorse quando vengono inviate a Adobe Experience Manager. L’integrazione può essere configurata per la pubblicazione nel servizio di pubblicazione Adobe Experience Manager o in un Portale marchio Adobe Experience Manager.

Il flusso di lavoro Pubblicazione automatica può essere abilitato e configurato nell’integrazione di Adobe Experience Manager. Quando è attivata, il flusso di lavoro può essere modificato a livello di modello di progetto o di progetto.

Per ulteriori informazioni, consulta [Pubblicazione delle risorse](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/use-aem-workflows.md#publishing-assets) in [Utilizzare i flussi di lavoro nell&#39;integrazione di Experience Manager Assets](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/use-aem-workflows.md).
