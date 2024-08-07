---
title: 23.3 Miglioramenti dell’integrazione
description: 23.3 Miglioramenti dell’integrazione
author: Lisa
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: d24ddc8a-fe96-4e9b-8186-0b54ab9ab213
source-git-commit: 84444753db0e5c496f013e0245988e62fddad585
workflow-type: tm+mt
source-wordcount: '740'
ht-degree: 0%

---

# 23.3 Miglioramenti dell’integrazione

Questa pagina descrive tutti i miglioramenti all’integrazione apportati con la versione 23.3 di. Questi miglioramenti sono stati resi disponibili nell’ambiente di produzione con la versione 23.3 del 20 e 21 luglio 2023.

Per un elenco di tutte le modifiche disponibili a questo punto del ciclo di rilascio 23.3, vedere [Panoramica sulla versione 23.3](/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-release-overview.md).

## È ora disponibile la nuova integrazione di Google Workspace

Una nuova integrazione di Google Workspace è ora disponibile nel marketplace Google. La nuova integrazione esegue l’autenticazione utilizzando OAuth2 e sostituisce l’integrazione precedente.

La precedente integrazione di Google Workspace è ora obsoleta e verrà disinstallata automaticamente.

Per istruzioni su come installare la nuova integrazione, vedi [Installa [!DNL Adobe Workfront for Google Workspace]](/help/quicksilver/workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

Per ulteriori informazioni su Workfront per Google Workspace, vedere [Workfront per Google Workspace](/help/quicksilver/workfront-integrations-and-apps/workfront-for-g-suite/workfront-for-gsuite.md).

## Le integrazioni Adobe Creative Cloud ora supportano più utenti assegnati

L’integrazione di Adobe Creative Cloud ora supporta la possibilità di scegliere tra &quot;Completato con la parte&quot; e &quot;Completo&quot; (o &quot;Risolto&quot;) quando a un’attività o a un problema sono assegnati più utenti.

In precedenza, l’integrazione consentiva agli utenti di contrassegnare un’attività come completata, senza specificare &quot;Fine con la parte&quot; o &quot;Completo&quot;/&quot;Risolto&quot;.

Per sfruttare questa funzionalità, scarica e installa i plug-in Workfront for Creative Cloud più recenti.

Per ulteriori informazioni sulla funzionalità, vedere [Contrassegnare gli elementi di lavoro come completati utilizzando il plug-in Adobe Workfront](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-complete.md).

Per informazioni sull&#39;installazione dei plug-in Workfront for Creative Cloud, vedere [Installare il plug-in Adobe Workfront for Creative Cloud Applications](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-toc.md).

## Visualizzare e gestire le notifiche Workfront da Workfront per i plug-in Creative Cloud

Per semplificare la ricezione delle notifiche necessarie, è possibile visualizzare e gestire le notifiche di Workfront senza uscire da Adobe Creative Cloud. Ora puoi visualizzare le notifiche, nonché accedere agli elementi di lavoro e ai commenti relativi a tali notifiche direttamente dalla finestra del plug-in Workfront all’interno dell’applicazione Creative Cloud.

In precedenza, le notifiche erano disponibili solo all’interno di Workfront e tramite e-mail.

Per sfruttare questa funzionalità, scarica e installa i plug-in Workfront for Creative Cloud più recenti.

Per ulteriori informazioni, vedere [Visualizzare e gestire [!DNL Adobe Workfront] le notifiche da Adobe Creative Cloud](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-notifications.md).

Per informazioni sull&#39;installazione dei plug-in Workfront for Creative Cloud, vedere [Installare il plug-in Adobe Workfront for Creative Cloud Applications](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-toc.md).

<!--

## Improved experience when moving a document to a linked folder with drag and drop

We've added some transparency to the process of dragging and dropping a document into a linked folder. Now, the document that you moved to a linked folder remains in the document list until it has fully moved. The document options are disabled, but you can still open the document for view while it is moving. When the document has completed the transfer, it disappears from the document list, because it is now fully located in the linked folder.

Previously, documents would immediately disappear from the document list, before they had finished moving to the linked folder.

For more information, see [Link documents from external applications](/help/quicksilver/documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

-->

## Creazione automatica di cartelle collegate in Adobe Experience Manager Assets durante la creazione di un progetto

Con il nuovo flusso di lavoro Crea cartella collegata per l’integrazione Adobe Experience Manager, puoi configurare l’integrazione con un percorso a una cartella Adobe Experience Manager Assets. Quando l’integrazione viene aggiunta a un modello di progetto, tutti i progetti creati dal modello creano automaticamente una sottocartella collegata in Experience Manager Assets nella cartella specificata.

In precedenza, la creazione di cartelle collegate richiedeva un’azione da parte dell’utente.

Questa funzionalità è disponibile solo con un’integrazione Adobe Experience Manager as a Cloud Service all’interno di Workfront. Questo non è disponibile nel connettore avanzato di Adobe Experience Manager.

Per ulteriori informazioni, vedere [Utilizzare i flussi di lavoro nell&#39;integrazione di Experience Manager Assets](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/use-aem-workflows.md).

## Mappare i valori dei campi di Workfront ai tag in Experience Manager Assets

Ora è possibile categorizzare e trovare rapidamente le risorse in base ai dati provenienti da Workfront. Puoi mappare questi dati come parte della configurazione dei metadati nell’integrazione di Workfront for Experience Manager Assets.

In precedenza, la mappatura dei dati di Workfront sui tag Experience Manager Assets non era disponibile.

Per ulteriori informazioni su questa funzionalità in Experience Manager Assets as a Cloud Service, vedere [Configurare l&#39;integrazione [!UICONTROL Experience Manager Assets as a Cloud Service]](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).
Per ulteriori informazioni su questa funzionalità in Experience Manager Assets Essentials, consulta [Configurare l&#39;integrazione di Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## Mappare i campi Workfront ai campi di metadati Experience Manager Assets personalizzati

Con l’integrazione nativa, ora puoi mappare i campi Workfront nativi e incorporati ai campi dello schema di metadati personalizzati in Experience Manager Assets as a Cloud Service.

Per ulteriori informazioni su questa funzionalità in Experience Manager Assets as a Cloud Service, vedere [Configurare l&#39;integrazione [!UICONTROL Experience Manager Assets as a Cloud Service]](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).
Per ulteriori informazioni su questa funzionalità in Experience Manager Assets Essentials, consulta [Configurare l&#39;integrazione di Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## Regolare le impostazioni del modello di flusso di lavoro per bozza automatizzata con Adobe Workfront for Creative Cloud

È ora possibile modificare le impostazioni del modello di workflow automatizzato esistente direttamente nella Creative Cloud. Dopo aver scelto un modello di workflow automatizzato esistente, è possibile:

* Disattiva fasi
* Aggiungi altri destinatari
* Modificare i ruoli della bozza
* Regolare la scadenza
* Aggiornare le notifiche e-mail
* E altro ancora!

Per ulteriori informazioni, consulta [Caricare documenti e bozze con il [!DNL Adobe Workfront] plug-in per [!DNL Creative Cloud] Applicazioni](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-docs-proofs-toc.md).

Questi miglioramenti sono disponibili per le seguenti app Creative Cloud:

* Photoshop
* XD
* InDesign
* Illustrator
