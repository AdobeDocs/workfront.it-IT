---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Inviare un documento a Experience Manager Assets o Assets Essentials
description: Puoi inviare documenti da Workfront a Experience Manager Assets o Assets Essentials. I documenti caricati e inviati da Workfront ad Assets Essentials vengono comunque conteggiati nell’archiviazione complessiva dei documenti. I collegamenti Assets da Assets Essentials non vengono considerati ai fini dello storage complessivo.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 7942e77b-9466-4dff-9737-97b17647ac48
source-git-commit: 90eb99fa46e706a53427f995d484e2fb42e9c293
workflow-type: tm+mt
source-wordcount: '923'
ht-degree: 9%

---

# Inviare un documento a Experience Manager Assets o Assets Essentials

Puoi inviare documenti da Workfront a Experience Manager Assets o Assets Essentials. I documenti caricati e inviati da Workfront ad Assets Essentials vengono comunque conteggiati nell’archiviazione complessiva dei documenti. I collegamenti Assets da Assets Essentials non vengono considerati ai fini dello storage complessivo.

Assets inviato ad Experience Manager tramite questa integrazione ha un limite di dimensioni di **5 GB**.

Nell&#39;ambiente di anteprima, Assets inviato ad Experience Manager tramite questa integrazione ha un limite di dimensioni di **30 GB**.

>[!NOTE]
>
>Questa funzionalità non è disponibile nell&#39;area nuovi documenti.<br>
>Se l&#39;organizzazione utilizza l&#39;archiviazione aziendale, quando si accede ai documenti in Workfront verrà visualizzata la nuova area documenti. Da lì puoi inviare le risorse a Experience Manager Assets. Per ulteriori informazioni, consulta [Utilizzare Adobe Experience Manager con l’integrazione Frame.io](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/use-aem-with-frame.md).

## Metadati

I campi metadati vengono mappati per la prima volta quando invii una risorsa da Workfront a Experience Manager Assets o Assets Essentials. Vengono inviati anche tutti i metadati configurati per la mappatura degli oggetti principali. Per ulteriori informazioni sulla configurazione del mapping dei metadati, vedere [Configurare l&#39;integrazione Experience Manager Assets as a Cloud Service](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) o [Configurare l&#39;integrazione Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

>[!INFO]
>
>**Esempio** Quando invii una risorsa associata a un&#39;attività, i metadati dell&#39;attività vengono mappati su Experience Manager Assets o Assets Essentials, nonché i metadati mappati da oggetti principali come un progetto, un portfolio e un programma.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p> Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenze Adobe Workfront</td> 
   <td> 
   <p>Collaboratore o successiva</p> 
   <p>Richiedente o successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotti aggiuntivi</td> 
   <td>Devi disporre di Experience Manager as a Cloud Service o Assets Essentials e devi essere aggiunto al prodotto come utente in Admin Console.</td> 
  </tr> 
   <tr> 
    <td role="rowheader">Autorizzazioni Experience Manager</td> 
    <td>È necessario disporre dell'accesso in scrittura alla cartella.</td> 
   </tr>
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Accesso in modifica ai documenti</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
   <td> <p>Accesso di visualizzazione o versione successiva</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

Prima di iniziare,

* L’amministratore di Workfront deve configurare un’integrazione Experience Manager. Per ulteriori informazioni, consulta [Configurare l&#39;integrazione Experience Manager Assets as a Cloud Service](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) o [Configurare l&#39;integrazione Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).


## Invia un documento da Workfront

Quando un utente invia un documento da Workfront a Experience Manager Assets o Assets Essentials, i metadati mappati vengono trasferiti lungo il documento. Dopo l’invio del documento, le modifiche apportate ai metadati del documento in Workfront non vengono applicate in Assets o Assets Essentials. If a mapped field in Workfront is changed, you must send a new version of the document with the updated metadata to Assets or Assets Essentials. To set up or edit metadata, see [Configure the Experience Manager Assets as a Cloud Service integration](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) or [Configure the Experience Manager Assets Essentials integration](../../documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

To send a document:

1. Go to the **Documents** area in Workfront, and select the document you want to send.
1. Click **Send to**, then choose the Experience Manager integration your administrator set up.

   >[!NOTE]
   >
   >The Workfront administrator can choose any name for this integration, so it may not specifically mention Assets or Assets Essentials.

   ![Send to](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Choose where you want the asset to go, then click **Select Folder**.
1. When you find your desired destination, click **Save**.

## Send a new version

You can add a new version to a document you have previously uploaded to Workfront. For more information, see [Upload a new version of a document](../../documents/managing-documents/upload-new-document-version.md). After the latest version is uploaded, you can send it to Assets Essentials. If a mapped field in Workfront has changed, the new version updates the metadata in Assets Essentials when it sends.

>[!IMPORTANT]
>
>Before you upload a new version to Workfront, we recommend renaming the file. If you upload a new version with the exact same file name as a previous version, only the most recent version can be downloaded from Workfront. All versions can be downloaded from Experience Manager Assets or Assets Essentials regardless of the file name.

To send the most recent version:

1. Go to the **Documents** area in Workfront, and locate the document.
1. Select **Send to**, then choose the Experience Manager integration your administrator set up.

   >[!NOTE]
   >
   >The Workfront administrator can choose any name for this integration, so it might not specifically mention Assets or Assets Essentials.

   ![Send to](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Fai clic su **Salva**. The new version saves in the same location as the previous version.

## Move a document to a linked folder in Experience Manager Assets

>[!NOTE]
>
>This functionality is only available for Experience Manager Assets as a Cloud Service. It is not available for Experience Manager Assets Essentials.

You can move a document to a linked folder in Experience Manager Assets if both the document and the linked folder are in the same document list (such as the document area of a project).

1. Locate the document that you want to move.
1. Drag and drop the document onto the linked Experience Manager Assets folder that you want to move it to.

The document options are not available while the document is in the process of moving. After the document is moved to Experience Manager Assets, is no longer visible in the document list in Workfront.

>[!NOTE]
>
> Any actions or edits you make on the document while it is moving will not appear on the document in Experience Manager Assets, and will therefore be lost.

