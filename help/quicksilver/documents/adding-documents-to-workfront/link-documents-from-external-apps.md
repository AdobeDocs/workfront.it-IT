---
product-area: documents
navigation-topic: add-documents-to-workfront
title: Collegare documenti da applicazioni esterne
description: You can link documents and folders to Adobe Workfront from external sources.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 97823f70-6544-445a-9a81-abe1e2f3de55
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 90eb99fa46e706a53427f995d484e2fb42e9c293
workflow-type: tm+mt
source-wordcount: '2592'
ht-degree: 3%

---

# Collegare documenti da applicazioni esterne

<!-- Audited: 01/2024 -->

You can link documents and folders to Adobe Workfront from the following sources:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Existing third party cloud document providers</td> 
   <td>These include the following: 
    <ul> 
     <li>Box</li> 
     <li>Dropbox</li> 
     <li>Dropbox Business</li> 
     <li>WebDAM</li> 
     <li>Microsoft OneDrive</li> 
     <li>Microsoft SharePoint</li> 
     <li>Google Drive</li> 
     <li>Quip</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront Proof </td> 
   <td>You can make proofs that were originally created within Workfront Proof available within Workfront.</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td role="rowheader">Experience Manager Assets Essentials </td> 
   <td>You can link documents to Workfront from Experience Manager Assets Essentials. For more information, see <a href="../../documents/adobe-workfront-for-experience-manager-assets-essentials/workfront-for-aem-asset-essentials.md" class="MCXref xref"> Adobe Workfront for Experience Manager Assets Essentials</a>.</td> 
  </tr>

<tr> 
   <td role="rowheader">Other document providers (through custom document integrations)</td> 
   <td> <p class="workfront_plans">These integrations can be configured in the Setup area.</p> </td>
  </tr> 
 </tbody> 
</table>

Before you link documents or folders, your Workfront administrator must enable this functionality for each document provider, or for a custom document integration, as described in [Configure document integrations](../../administration-and-setup/configure-integrations/configure-document-integrations.md).

You can proof and approve documents linked to an external cloud provider the same way you do so with documents uploaded directly to Workfront.

>[!NOTE]
>
>Questa funzionalità non è disponibile nell&#39;area nuovi documenti.<br>
>Se l&#39;organizzazione utilizza l&#39;archiviazione aziendale, quando si accede ai documenti in Workfront verrà visualizzata la nuova area documenti. Per ulteriori informazioni sull&#39;archiviazione aziendale, vedere [Panoramica sull&#39;archiviazione aziendale di Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td>
   <td> <p>Qualsiasi</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td>
   <td><p>Collaboratore o successiva</p>
    <p>Richiedente o successiva</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Accesso in modifica ai documenti</p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Document storage

Documents that are linked to Workfront from an external application are stored with the external cloud provider, not within Workfront.

The following exceptions apply:

* When provided by the document service, thumbnails and preview images might be stored on Workfront servers.
* When you use proofing in Workfront, the document is copied and added to the proofing servers.

## Limiti di dimensione del file

Third-party cloud providers:

* Single file: 5 GB or less
* Multiple file: 1 GB or less (total of all files)

## Link a document from an external application to Workfront

You can link existing documents with an external cloud provider. Ciò include tutti i documenti condivisi.

### Prerequisiti {#prerequisites}

Prima di collegare documenti o cartelle, l&#39;amministratore di Workfront deve abilitare questa funzionalità per ogni provider di documenti o per un&#39;integrazione di documenti personalizzata, come descritto in [Configurare le integrazioni di documenti](../../administration-and-setup/configure-integrations/configure-document-integrations.md).

### Collegare un documento esterno a Workfront {#link-an-external-document-to-workfront}

È possibile collegare documenti a Workfront da un&#39;applicazione esterna come Google e Microsoft OneDrive.

>[!IMPORTANT]
>
>Dropbox memorizza i documenti in base al percorso del file. Per questo motivo, se un file collegato da Dropbox viene spostato, rinominato o eliminato, diventa inaccessibile in Workfront.

1. Vai all&#39;area **Documenti** in Workfront in cui desideri inserire il documento.
1. Fare clic su **Aggiungi nuovo**, quindi sul provider di documenti esterno in cui si desidera collegare i documenti a Workfront.

   Ad esempio, per collegare documenti da Dropbox, fare clic su **Da Dropbox**.

   I provider esterni che hai già autorizzato vengono visualizzati nella parte superiore dell’elenco.

1. (Condizionale) Se viene richiesto di accedere al servizio esterno, digitare le credenziali di accesso per il servizio nella casella visualizzata, quindi fare clic su **Accedi**.
1. (Condizionale) Se viene richiesto di autorizzare l&#39;applicazione esterna, fare clic sul pulsante **Autorizza**.

   Devi fare questo solo una volta.

1. Nella casella di ricerca della casella **Collega file e cartelle esterni** visualizzata, digitare il nome dell&#39;elemento che si desidera cercare, quindi premere **Invio** per visualizzare tutti i risultati dell&#39;applicazione esterna, indipendentemente dalla cartella in cui sono archiviati.

   Oppure

   Individuare e selezionare i documenti da collegare.

   Sebbene sia possibile selezionare più documenti, vengono collegati solo i documenti selezionati nella visualizzazione corrente. Se ad esempio si seleziona un documento e quindi si accede a una cartella, il documento selezionato in origine non verrà collegato.

1. (Condizionale) Se sei un cliente Workfront DAM, fai clic sull&#39;icona **Miniatura** per visualizzare i file come immagini di miniatura.

   >[!NOTE]
   >
   >I clienti di Workfront DAM possono visualizzare le miniature quando collegano documenti da Workfront DAM. Le miniature potrebbero essere visualizzate anche per i clienti di Workfront DAM per altri servizi come Dropbox e Box. Tuttavia, la visualizzazione delle miniature per servizi diversi da Workfront DAM in Workfront non è supportata e le miniature non vengono mai visualizzate quando si collegano documenti da SharePoint o Google Drive.

1. Fai clic su **Collegamento**.

   In Workfront, accanto ai documenti viene visualizzata l’icona del provider di cloud.

   >[!NOTE]
   >
   >* Se l&#39;URL di download utilizzato per collegare il documento supera i 2048 caratteri, il file non può essere collegato.
   >* Per i documenti collegati a Box, il collegamento al documento in Box viene visualizzato solo dopo l&#39;aggiornamento della pagina.

### Add a new version of a linked document {#add-a-new-version-of-a-linked-document}

You can add a new version of a document linked to Workfront from an external application.

1. Go to the **Documents** area where the document is linked, then select the linked document.

   >[!IMPORTANT]
   >
   >The document must be outside of a linked folder to create a new version.

1. Click **Add New** > **Version**, then click the external document provider.

   For example, to link a new version of a document from Dropbox, click **From Dropbox**.

   I provider esterni che hai già autorizzato vengono visualizzati nella parte superiore dell’elenco.

1. (Condizionale) Se viene richiesto di accedere al servizio esterno, digitare le credenziali di accesso per il servizio nella casella visualizzata, quindi fare clic su **Accedi**.
1. (Conditional) If you are prompted to authorize the external application, click **Authorize**.

   Devi fare questo solo una volta.

1. In the search box of the **Link External Files and Folders** box that appears, type the name of the item you want to search for, then press **Enter** to see all results from the external application, regardless of which folder they are stored in.

   Oppure

   Individuare e selezionare i documenti da collegare.

   You can select multiple documents; however, only documents that are selected in the current view are linked. Se ad esempio si seleziona un documento e quindi si accede a una cartella, il documento selezionato in origine non verrà collegato.

1. (Condizionale) Se sei un cliente Workfront DAM, fai clic sull&#39;icona **Miniatura** per visualizzare i file come immagini di miniatura.

   >[!NOTE]
   >
   >I clienti di Workfront DAM possono visualizzare le miniature quando collegano documenti da Workfront DAM. Le miniature potrebbero essere visualizzate anche per i clienti di Workfront DAM per altri servizi come Dropbox e Box. Tuttavia, la visualizzazione delle miniature per servizi diversi da Workfront DAM in Workfront non è supportata e le miniature non vengono mai visualizzate quando si collegano documenti da SharePoint o Google Drive.

1. Fai clic su **Collegamento**.

   In Workfront, the cloud provider&#39;s icon appears next to the documents, indicating that they are linked to the external cloud provider.

   >[!NOTE]
   >
   >Per i documenti collegati a Box, il collegamento al documento in Box viene visualizzato solo dopo l&#39;aggiornamento della pagina.

For information about adding new version of a document you have uploaded to Workfront from your file system, see [Add documents to Adobe Workfront](../../documents/adding-documents-to-workfront/add-documents-from-file-system.md#add-documents-to-workfront) in [Add documents to Adobe Workfront from your file system](../../documents/adding-documents-to-workfront/add-documents-from-file-system.md).

### Link Workfront Proof documents {#link-workfront-proof-documents}

You can link proofs to Workfront that originally existed in Workfront Proof. When you link a proof from Workfront Proof, all comments and other metadata associated with the proof are available in Workfront.

Puoi collegare solo le bozze per le quali disponi dell’accesso di visualizzazione in Workfront Proof.

1. Vai all&#39;area **Documenti** in Workfront in cui desideri inserire il documento.
1. Fai clic su **Aggiungi nuovo**, quindi su **Da Workfront Proof**.

   >[!NOTE]
   >
   >Le opzioni di questo menu possono variare a seconda dei provider di terze parti configurati nel tuo ambiente.

1. Nella casella **Collega bozze da Workfront Proof** visualizzata, inizia a digitare il nome della bozza che desideri rendere disponibile in Workfront.

   L&#39;elenco viene filtrato durante la digitazione.

1. Seleziona fino a 10 bozze da collegare.

   Qualsiasi nome di bozza oscurato non è disponibile per il collegamento, perché la bozza è già associata a un documento in Workfront.

1. Fai clic su **Collegamento**.

   La versione più recente della bozza è collegata a Workfront. Quando apri la bozza, nel visualizzatore di bozze sono disponibili tutte le versioni.

### Creazione di un documento Google da Workfront {#create-a-google-document-from-within-workfront}

È possibile creare un nuovo documento Google da Workfront. Non è possibile creare nuovi documenti da Workfront per altri provider cloud.

1. Vai all&#39;area **Documenti** in Workfront in cui desideri inserire il documento.
1. Fai clic su **Aggiungi nuovo** > **File Google**, quindi seleziona il tipo di documento Google che desideri creare.
1. Se viene visualizzata la casella **Aggiungi account Google Drive**, fare clic su **Autorizza Google Drive**.

   Un documento Google è stato aggiunto alla scheda **Documenti**.

   >[!NOTE]
   >
   > Le opzioni Unità e Condiviso con me visualizzano due risultati diversi. Se non si riesce a individuare un file nella cartella Unità, archiviare la cartella Condiviso con me.

## Caricare e collegare un documento da Workfront a un provider cloud esterno

Puoi caricare e collegare un documento da Workfront a un provider cloud esterno. In questo modo l’archiviazione del documento viene spostata da Workfront al provider cloud esterno. Quando il documento viene modificato nell&#39;applicazione esterna, viene aggiornato automaticamente in Workfront.

>[!NOTE]
>
>Quando si invia una risorsa a un provider di documenti esterno, viene creata una nuova versione della risorsa.

Users without Workfront access can see the document in the external application if they have access to the application.

1. Select a document that is uploaded in Workfront.
1. Click **More** >**Send to**, then select the cloud provider that you want to store the linked document.

   You can also use the More menu ![More menu](assets/more-icon.png) on the Document Details page to do this.

1. Select the folder in the provider&#39;s application where you want to store the document.

   This can be any folder in the provider&#39;s application, including a shared folder.

1. Fai clic su **Salva**.

   The external provider&#39;s logo appears next to the document name to indicate that the document is now linked to Workfront and stored by the external cloud provider.

   ![doc_with_google_drive_link_highlight__1_.png](assets/doc-with-google-drive-link-highlight--1--350x66.png)

## Link folders

When you link a folder between Workfront and an external cloud provider, the folder and all of its contents are linked. If users without Workfront access add, remove, and modify files from the external document application, their changes are synchronized to Workfront.

### Folder access rights {#folder-access-rights}

When synchronizing folder content from an external document application, Workfront uses the credentials of the user who originally linked the folder. This results in the following user experience:

* If users do not have access to view files and folders in the external application, but do have access to view the linked folder via Workfront, they can view only the names of the files and folders in Workfront, not their contents.
* When someone accesses content inside a linked folder in Workfront (such as a subfolder in a linked folder) that was linked to Workfront by another user, the content synchronizes to Workfront using the Workfront login credentials of the user who originally linked the folder, not the credentials of the user accessing the content.

>[!IMPORTANT]
>
>* If the user who originally linked the folder is removed from the Workfront system, users are no longer able to access content on the linked folder via Workfront. In this case, the folder must be relinked by an active Workfront user who has rights to the folder in the external application.
>* If the user who linked a folder no longer has access to the external application, Workfront can no longer access the contents of the folder. This may happen, for example, if the user who originally linked the folder leaves the company. To ensure continued access, a user with access to the folder must re-link the folder.

### Link one or more external folders {#link-one-or-more-external-folders}

1. Go to the area in Workfront where you want the folder, then click  **Documents** ![Documents icon](assets/document-icon.png) in the left panel .

1. Click **Add New**, then click the external document provider from which you want to link a folder to Workfront.
1. (Conditional) If you have not yet authorized the external service, specify your login credentials for the external provider, then click **Sign in**.

   I provider esterni che hai già autorizzato vengono visualizzati nella parte superiore dell’elenco.

1. Nella casella **Collega file e cartelle esterni** visualizzata, individuare e selezionare le cartelle che si desidera collegare.

   Oppure

   Digitare il nome della cartella da cercare, quindi premere **Invio**.

   È possibile selezionare più cartelle; tuttavia, solo le cartelle selezionate nella visualizzazione corrente sono collegate. Ad esempio, se selezioni una cartella e successivamente la inserisci in una cartella, la cartella selezionata originariamente non viene collegata.

   >[!NOTE]
   >
   >Quando si collegano cartelle da Google Drive, è possibile collegare solo le cartelle che si trovano nell&#39;unità personale (My Drive) e in Team Drive. Non è possibile collegare cartelle dall&#39;area Condiviso con me.

1. Fai clic su **Collegamento**.

   In Workfront, accanto alla cartella viene visualizzato il logo del provider di cloud, che indica che è collegato al provider di cloud esterno.

1. (Facoltativo) Per rinominare la cartella in modo che il nome della cartella in Workfront sia diverso dal nome della cartella nell&#39;applicazione per documenti esterni, selezionare la cartella nella sezione **Cartelle**, fare clic sul menu Altro ![Menu Altro](assets/more-icon.png) visualizzato accanto al nome della cartella, quindi fare clic su **Rinomina**.

   ![Rinomina cartella](assets/documents-folderlink-rename-nwe-350x154.png)

La cartella non verrà rinominata nell&#39;applicazione esterna.

### Aggiungere sottocartelle a una cartella collegata  {#add-subfolders-to-a-linked-folder}

È possibile creare una nuova cartella all&#39;interno di una cartella collegata esistente. Puoi anche trascinare un’altra cartella in una cartella collegata esistente.

1. Per creare una nuova cartella all&#39;interno di una cartella collegata esistente, passare alla cartella esistente, quindi creare la nuova cartella come descritto in [Crea cartelle di documenti](../../documents/organizing-documents/create-documents-folder.md).

   Oppure

   Per trascinare una cartella esistente in una cartella collegata esistente, passare all&#39;area Documenti in cui si desidera inserire la sottocartella, quindi trascinarla nella cartella collegata.

   ![Trascina nella cartella collegata](assets/documents-link-folder-move-nwe-350x113.png)

   >[!NOTE]
   >
   >Quando si trascina una cartella Workfront esistente in una cartella collegata, si applicano le seguenti limitazioni:
   >
   >* La cartella che stai trascinando non può essere già collegata e non può contenere alcun contenuto già collegato.
   >* La cartella (compreso il suo contenuto) che stai trascinando non può superare i 50 MB.

## Aggiungere un documento a una cartella collegata

Quando si aggiunge un documento a una cartella collegata tramite Workfront, questo viene aggiunto automaticamente come documento collegato.

1. Selezionare la cartella collegata in cui si desidera inserire il documento, fare clic su **Aggiungi nuovo > Documento**, quindi individuare il documento e aggiungerlo alla cartella.

   Oppure

   Nell&#39;area **Documenti** in cui si desidera inserire il documento, trascinare il documento in una cartella collegata.

   Una nuova versione del documento viene creata automaticamente nell&#39;applicazione esterna e collegata a Workfront.

>[!NOTE]
>
> * Le opzioni del documento non sono disponibili mentre è in corso lo spostamento del documento.
>
> * Dopo lo spostamento di un documento in Experience Manager Assets, non sarà più visibile nell&#39;elenco dei documenti in Workfront.
>
> * Qualsiasi azione o modifica eseguita su un documento durante lo spostamento non verrà visualizzata sul documento in Experience Manager Assets e andrà quindi persa.

## Eliminare un documento o una cartella collegata

Quando si elimina un documento o una cartella collegata dall&#39;applicazione esterna, il documento o la cartella rimane nel sistema Workfront fino a quando non viene eliminato anche da Workfront.

1. Selezionare il documento o la cartella collegata, quindi fare clic su **Elimina**.
1. Nella casella di conferma visualizzata fare clic su **Sì, scollega**.

   Il documento è scollegato dal sito Workfront. Non viene influenzato nell’applicazione esterna.

## Informazioni sulla ridenominazione di documenti e cartelle collegati

Quando si rinomina un documento o una cartella collegata, la modifica è visibile solo nell&#39;applicazione in cui viene creata. Se ad esempio si rinomina un documento collegato in Workfront, il nuovo nome sarà visibile solo in Workfront.

Se si desidera che il nome corrisponda in Workfront e nell&#39;applicazione esterna, è necessario rinominarlo in entrambe le posizioni.

>[!IMPORTANT]
>
>Non rinominare un documento in Workfront collegato a Dropbox; in questo modo il file in Workfront non è accessibile. Rinomina il file in Dropbox, quindi sincronizza nuovamente il file.
