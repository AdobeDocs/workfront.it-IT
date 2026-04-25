---
product-area: documents
navigation-topic: add-documents-to-workfront
title: Aggiungere documenti ad Adobe Workfront dal file system
description: È possibile aggiungere documenti a progetti, attività o problemi in più aree in Adobe Workfront.
author: Courtney
feature: Digital Content and Documents
exl-id: 0a5f82b2-f86e-4ffa-b3a6-18221dd0e158
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 90eb99fa46e706a53427f995d484e2fb42e9c293
workflow-type: tm+mt
source-wordcount: '1271'
ht-degree: 5%

---

# Aggiungere documenti ad Adobe Workfront dal file system

In Workfront sono attualmente disponibili due versioni dell&#39;area Documenti: l&#39;area documenti legacy e l&#39;area nuovi documenti. La versione utilizzata dall&#39;organizzazione dipende dal fatto che l&#39;organizzazione si basi su sistemi di storage Workfront o aziendali legacy. Per ulteriori informazioni su questi tipi di archiviazione, vedere [Panoramica sullo storage aziendale di Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

L’aggiunta di documenti a Workfront varia a seconda della versione dell’area documenti utilizzata dall’organizzazione.

* [Aggiungere documenti a dal file system nell&#39;area dei documenti legacy](#add-documents-from-your-file-system-in-the-legacy-documents-area)
* [Aggiungere documenti a Workfront nell’area dei nuovi documenti](#add-documents-to-workfront-in-the-new-documents-area)



## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi pacchetto Workfront per gestire i documenti utilizzando lo storage Workfront legacy</p>
<p>Qualsiasi pacchetto di flusso di lavoro per gestire i documenti utilizzando lo storage aziendale Adobe</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenze Adobe Workfront*</td> 
   <td> 
   <p>Collaboratore o successiva</p> 
   <p>Richiedente o successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Archiviazione Workfront legacy: modifica accesso ai documenti</p> 
   <p>Archiviazione aziendale: l'accesso di modifica ai documenti è abilitato per impostazione predefinita e non può essere modificato</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Aggiungere documenti dal file system nell&#39;area dei documenti legacy

Se la tua organizzazione utilizza un sistema di archiviazione Workfront legacy, quando accedi ai documenti in Workfront visualizzerai l’area documenti legacy. Per ulteriori informazioni sull&#39;archiviazione Workfront, vedere [Differenze tra l&#39;archiviazione aziendale Adobe e l&#39;archiviazione Workfront legacy](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-enterprise-storage-and-legacy-workfront-storage).

È possibile aggiungere documenti a progetti, attività o problemi nelle seguenti aree in Adobe Workfront:

* Area Documenti globale
* Area Documenti per un oggetto Workfront
* Una scheda collegata su una scheda Workfront

È inoltre possibile caricare nuove versioni di documenti e aggiungere collegamenti a documenti di fornitori di cloud di terze parti, ad esempio Google Drive, Dropbox e Microsoft OneDrive. Per informazioni sull&#39;aggiunta di nuove versioni di documenti, vedere [Caricare una nuova versione di un documento](../../documents/managing-documents/upload-new-document-version.md). Per informazioni sull&#39;aggiunta di documenti da fornitori di cloud di terze parti, vedere [Collegare documenti da applicazioni esterne](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

Non esistono restrizioni sui tipi e sulle dimensioni dei file che è possibile caricare in Workfront. Tuttavia, per avere successo, il caricamento deve essere completato entro cinque minuti e devi disporre di spazio di archiviazione sufficiente.

Se hai bisogno di informazioni sul caricamento di nuove versioni di un documento in Workfront, consulta [Caricare una nuova versione di un documento](../../documents/managing-documents/upload-new-document-version.md).


### Aggiungere documenti a Workfront nell’area documenti legacy

È possibile aggiungere nuovi documenti a Workfront dal file system della workstation. È inoltre possibile collegare documenti da applicazioni di terze parti, ad esempio Google Drive e SharePoint.

>[!IMPORTANT]
>
>* You can upload up to 150 documents at one time.
>* Non esiste alcun limite alla dimensione del file.
>* I download dei documenti sono limitati a 4 GB.

Per aggiungere un documento:

1. Passare al progetto, all&#39;attività o al problema in cui si desidera aggiungere un nuovo documento.
1. Fai clic sulla scheda **Documenti**, quindi sul menu a discesa **Aggiungi nuovo**.

   ![Aggiungi nuovo documento](assets/add-new-doc.png)

1. A seconda del tipo di documento che si desidera aggiungere, eseguire una delle operazioni seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Upload documents from your file system on your workstation</td> 
      <td> 
       <ol> 
        <li value="1">Dal menu a discesa <strong>Aggiungi nuovo</strong>, seleziona <strong>Documento.</strong></li> 
        <li value="2"> <p>Browse to and select the document that you want to add from the file system on your workstation.<br></p> <p>You can select multiple documents by pressing the Shift key as you select additional files.</p> </li> 
        <li value="3">Fai clic su <strong>Apri</strong>.</li> 
       </ol> 
       <p><b>NOTA</b>: è inoltre possibile trascinare i file direttamente dal file manager nell'elenco dei documenti.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Upload documents from a third-party application such as Google Drive or SharePoint</td> 
      <td> 
       <ol> 
        <li value="1"> <p>Dal menu a discesa <strong>Aggiungi nuovo</strong>, seleziona <strong>Da &lt;name_of_third-party_application&gt;</strong>.</p> <p>Ad esempio, per caricare un documento da Google Drive, fare clic su <strong>Da Google Drive</strong>.</p> </li> 
        <li value="2"> <p>Follow the prompts to select the document in the third-party application.<br></p> <p>Per ulteriori informazioni sui documenti collegati, vedere <a href="../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md" class="MCXref xref">Collegare documenti da applicazioni esterne</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Request a document from another Workfront user</td> 
      <td> 
       <ol> 
        <li value="1">Dal menu a discesa <strong>Aggiungi nuovo</strong>, selezionare <strong>Richiedi documento</strong>.</li> 
        <li value="2">Nella casella <strong>Chi richiede il documento</strong> digitare il nome dell'utente al quale si richiede il documento.</li> 
        <li value="3">In the <strong>Tell them what you're requesting</strong> box, type the name of the document.</li> 
        <li value="4"> <p>Fai clic su <strong>Invia richiesta</strong>.</p> <p>La richiesta viene visualizzata nella scheda Documenti.</p> <p>Per ulteriori informazioni sulla richiesta di documenti, vedere <a href="../../documents/adding-documents-to-workfront/request-a-document.md" class="MCXref xref">Richiedere un documento</a>.</p> </li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>


## Aggiungere documenti a Workfront nell’area dei nuovi documenti

È possibile aggiungere documenti a progetti, attività o problemi utilizzando il modello di storage aziendale. Per ulteriori informazioni sull&#39;archiviazione aziendale, vedere [Panoramica sull&#39;archiviazione aziendale di Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

Funzionalità non attualmente supportata nell&#39;area dei nuovi documenti:

* Caricamento di documenti nell&#39;area globale Documenti
* Aggiunta di collegamenti a documenti di fornitori di cloud di terze parti, ad esempio Google Drive, Dropbox e Microsoft OneDrive.
* Richiesta di documenti
* Copiare un collegamento in una cartella
* Estrazione di documenti
* Incollare immagini dagli Appunti
* Aggiunta di cartelle avanzate


### Aggiungere documenti a Workfront nell’area dei nuovi documenti

Se l&#39;organizzazione utilizza l&#39;archiviazione aziendale, quando si accede ai documenti in Workfront verrà visualizzata la nuova area documenti. Per ulteriori informazioni sull&#39;archiviazione aziendale, vedere [Panoramica sull&#39;archiviazione aziendale di Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

<!--
>[!IMPORTANT]
>
>* You can upload up to 150 documents at one time.
>* There is no limit on the file size. 
>* Document downloads are limited to 4GB.
-->

Per aggiungere un documento:

1. Passare al progetto, all&#39;attività o al problema in cui si desidera aggiungere un nuovo documento.
1. Fai clic su **Documenti** nel pannello a sinistra.
1. Fai clic su **Nuovo** sul lato destro della pagina oppure trascina e rilascia il file nella zona di rilascio visualizzata. È possibile aggiungere più documenti contemporaneamente.

   ![Aggiungi un nuovo documento](assets/add-new-doc-new-doc.png)

Se hai bisogno di informazioni sul caricamento di nuove versioni di un documento in Workfront, consulta [Caricare una nuova versione di un documento](../../documents/managing-documents/upload-new-document-version.md).

## Sicurezza dei documenti per lo storage aziendale

Workfront impedisce ai virus e ad altri contenuti dannosi di accedere al sito tramite i documenti nei seguenti modi:

**How Workfront detects corrupted files**

Document scanning is automatically enabled for objects using the enterprise storage model.

All files under 500 MB are scanned when they are uploaded. Files over 500 MB are not scanned. If Workfront detects a corrupted document, it is automatically removed.

**File name restrictions**

Because this integration is built using Adobe enterprise storage, there are some enforced structure and naming conventions to be aware of when managing projects and documents.

* Object names must be unique and can&#39;t be duplicated
* Adobe enterprise storage requires unique names for peer objects with the same parent in the hierarchy tree
* Documents can&#39;t have the same name if they belong to the same project
* Document names can&#39;t contain any of the following special characters: `\ / : * ? " | < >`
* Document names are limited to 255 characters maximum

With these limitations in mind, Workfront automatically renames objects or documents as needed to prevent conflicts.


## Document security for legacy Workfront storage

Workfront site prevents viruses and other malicious content from entering the site via documents in the following ways:

**How Workfront detects corrupted files**

Document scanning is enabled for your organization only upon request.

If document scanning is enabled, files under 25 MB are scanned when they are uploaded. Files over 25 MB are not scanned.

If Workfront detects a corrupted document, a message appears indicating that the file is corrupt. You also receive an email notification when Workfront detects potentially malicious content and the file is slated for removal.

Corrupted files are removed within 24 hours of detection unless you remove it manually. If you delete a corrupted file, Workfront tracks this action as an update. If you allow Workfront to remove it, then no updates are recorded.

**File name restrictions**

I file caricati in Workfront non possono contenere determinati caratteri nei nomi dei file. Se un file contiene uno dei seguenti caratteri nel nome del file, i caratteri vengono rimossi dal nome del file al caricamento: `! # % * \ | ' " / ? < > { } [ ]`.
