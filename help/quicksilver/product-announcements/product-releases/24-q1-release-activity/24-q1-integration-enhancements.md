---
title: Miglioramenti all’integrazione per il primo trimestre 2024
description: Miglioramenti all’integrazione per il primo trimestre 2024
author: Becky
feature: Product Announcements
exl-id: 0d581f3c-2aaf-4ac1-97a5-df1b01627080
source-git-commit: 44dd48b72e798b8967c4a4e3dc7d523fe9b130d2
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 0%

---

# Miglioramenti all’integrazione per il primo trimestre 2024

Questa pagina descrive tutti i miglioramenti all’integrazione apportati con la versione del primo trimestre 2024 all’ambiente di anteprima. Questi miglioramenti saranno resi disponibili nell’ambiente di produzione con la versione del primo trimestre 2024.

Per un elenco di tutte le modifiche disponibili a questo punto nel ciclo di rilascio del primo trimestre 2024, consulta [Panoramica sulla versione del primo trimestre 2024](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).

## La mappatura dei metadati in Experience Manager Assets Essentials ora utilizza `xcm:keywords` invece di `dc:subject`

Abbiamo aggiornato l’integrazione di Experience Manager Assets Essentials per adattarla all’esperienza nell’integrazione di Experience Manager Assets as a Cloud Service. Ora, quando si mappano più campi di testo a riga singola a un singolo campo in Experience Manager Assets, entrambi i servizi utilizzano `xcm:keywords` campo.

In precedenza, questi campi venivano mappati su `dc:subject` in Experience Manager Assets Essentials. La funzionalità as a Cloud Service di Experience Manager Assets è invariata.

Qualsiasi metadati di Experience Manager Assets Essentials attualmente mappati su `dc:subject` deve essere rimappato a `xcm:keywords`.

Per informazioni sulla mappatura dei metadati su Experience Manager Assets Essentials, consulta [Parola chiave AEM](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md#aem-keyword).

## I campi typeahead sono ora disponibili nell’integrazione di Adobe Experience Manager

Per semplificare il collegamento dei campi tra Workfront e Adobe Experience Manager, è stato aggiunto il supporto dei campi typeahead nella mappatura dei metadati. Ora è possibile mappare i campi typeahead ai campi corrispondenti in Adobe Experience Manager.

Se un utente seleziona un valore diverso per un campo in Workfront, tale modifica si riflette immediatamente in Adobe Experience Manager. Inoltre, se l’opzione del valore di un campo cambia (ad esempio, se un team ne cambia il nome in un nuovo nome), la modifica si riflette anche in Adobe Experience Manager.

Per informazioni e istruzioni sulla mappatura dei metadati nell’integrazione di Adobe Experience Manager, consulta [Configurare i metadati](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-metadata-optional).

## Pubblicare automaticamente le risorse in Adobe Experience Manager

È stato aggiunto un altro flusso di lavoro all’integrazione Adobe Experience Manager. Ora puoi impostare la pubblicazione automatica delle risorse quando vengono inviate a Adobe Experience Manager. L’integrazione può essere configurata per la pubblicazione nel servizio di pubblicazione Adobe Experience Manager o in un Portale marchio Adobe Experience Manager.

Il flusso di lavoro Pubblicazione automatica può essere abilitato e configurato nell’integrazione di Adobe Experience Manager. Quando è attivata, il flusso di lavoro può essere modificato a livello di modello di progetto o di progetto.

Per ulteriori informazioni, consulta [Pubblicazione delle risorse](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/use-aem-workflows.md#publishing-assets) in [Utilizzare i flussi di lavoro nell’integrazione di Experience Manager Assets](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/use-aem-workflows.md).
