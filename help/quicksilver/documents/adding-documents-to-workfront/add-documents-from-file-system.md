---
product-area: documents
navigation-topic: add-documents-to-workfront
title: Aggiungere documenti ad Adobe Workfront dal file system
description: È possibile aggiungere documenti a progetti, attività o problemi in più aree in Adobe Workfront.
author: Courtney
feature: Digital Content and Documents
exl-id: 0a5f82b2-f86e-4ffa-b3a6-18221dd0e158
source-git-commit: 430751f0e38c6c45145c965398990ee3652f36fe
workflow-type: tm+mt
source-wordcount: '715'
ht-degree: 1%

---

# Aggiungere documenti ad Adobe Workfront dal file system

È possibile aggiungere documenti a progetti, attività o problemi nelle seguenti aree in Adobe Workfront:

* Area Documenti globale
* Area Documenti per un oggetto Workfront
* Una scheda collegata su una scheda Workfront

È inoltre possibile caricare nuove versioni di documenti e aggiungere collegamenti a documenti di fornitori di cloud di terze parti, ad esempio Google Drive, Dropbox e Microsoft OneDrive. Per informazioni sull&#39;aggiunta di nuove versioni di documenti, vedere [Caricare una nuova versione di un documento](../../documents/managing-documents/upload-new-document-version.md). Per informazioni sull&#39;aggiunta di documenti da fornitori di cloud di terze parti, vedere [Collegare documenti da applicazioni esterne](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

Non esistono restrizioni sui tipi e sulle dimensioni dei file che è possibile caricare in Workfront. Tuttavia, per avere successo, il caricamento deve essere completato entro cinque minuti e devi disporre di spazio di archiviazione sufficiente.

Se hai bisogno di informazioni sul caricamento di nuove versioni di un documento in Workfront, consulta [Caricare una nuova versione di un documento](../../documents/managing-documents/upload-new-document-version.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p> Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenze Adobe Workfront*</td> 
   <td> 
   <p>Collaboratore o versione successiva</p> 
   <p>Richiedi o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica accesso ai documenti</p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Aggiungi documenti a Workfront

È possibile aggiungere nuovi documenti a Workfront dal file system della workstation. È inoltre possibile collegare documenti da applicazioni di terze parti, ad esempio Google Drive e SharePoint.

>[!IMPORTANT]
>
>* È possibile caricare fino a 150 documenti alla volta.
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
      <td role="rowheader">Caricare documenti dal file system sulla workstation</td> 
      <td> 
       <ol> 
        <li value="1">Dal menu a discesa <strong>Aggiungi nuovo</strong>, seleziona <strong>Documento.</strong></li> 
        <li value="2"> <p>Individuare e selezionare il documento che si desidera aggiungere dal file system della workstation.<br></p> <p>È possibile selezionare più documenti premendo il tasto Maiusc mentre si selezionano altri file.</p> </li> 
        <li value="3">Fai clic su <strong>Apri</strong>.</li> 
       </ol> 
       <p><b>NOTA</b>: è inoltre possibile trascinare i file direttamente dal file manager nell'elenco dei documenti.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Caricare documenti da un'applicazione di terze parti come Google Drive o SharePoint</td> 
      <td> 
       <ol> 
        <li value="1"> <p>Dal menu a discesa <strong>Aggiungi nuovo</strong>, seleziona <strong>Da &lt;name_of_third-party_application&gt;</strong>.</p> <p>Ad esempio, per caricare un documento da Google Drive, fare clic su <strong>Da Google Drive</strong>.</p> </li> 
        <li value="2"> <p>Seguire le istruzioni per selezionare il documento nell'applicazione di terze parti.<br></p> <p>Per ulteriori informazioni sui documenti collegati, vedere <a href="../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md" class="MCXref xref">Collegare documenti da applicazioni esterne</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Richiedere un documento a un altro utente di Workfront</td> 
      <td> 
       <ol> 
        <li value="1">Dal menu a discesa <strong>Aggiungi nuovo</strong>, selezionare <strong>Richiedi documento</strong>.</li> 
        <li value="2">Nella casella <strong>Chi richiede il documento</strong> digitare il nome dell'utente al quale si richiede il documento.</li> 
        <li value="3">Nella casella <strong>Informazioni</strong> digitare il nome del documento.</li> 
        <li value="4"> <p>Fai clic su <strong>Invia richiesta</strong>.</p> <p>La richiesta viene visualizzata nella scheda Documenti.</p> <p>Per ulteriori informazioni sulla richiesta di documenti, vedere <a href="../../documents/adding-documents-to-workfront/request-a-document.md" class="MCXref xref">Richiedere un documento</a>.</p> </li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

## Sicurezza dei documenti

Il sito Workfront impedisce ai virus e ad altri contenuti dannosi di accedere al sito tramite i documenti nei seguenti modi:

* [Rilevamento dei file danneggiati in Workfront](#how-workfront-detects-corrupted-files)
* [Limitazioni per i nomi dei file](#file-name-restrictions)

### Rilevamento dei file danneggiati in Workfront {#how-workfront-detects-corrupted-files}

La scansione dei documenti è abilitata per la tua organizzazione solo su richiesta.

Se è abilitata la scansione dei documenti, i file di dimensioni inferiori a 25 MB vengono analizzati al momento del caricamento. I file superiori a 25 MB non vengono analizzati.

Se Workfront rileva un documento danneggiato, viene visualizzato un messaggio che indica che il file è danneggiato. Ricevi inoltre una notifica e-mail quando Workfront rileva contenuti potenzialmente dannosi e il file è pianificato per la rimozione.

I file danneggiati vengono rimossi entro 24 ore dal rilevamento, a meno che non vengano rimossi manualmente. Se elimini un file danneggiato, Workfront tiene traccia di questa azione come aggiornamento. Se consenti a Workfront di rimuoverlo, non vengono registrati aggiornamenti.

### Limitazioni per i nomi dei file {#file-name-restrictions}

I file caricati in Workfront non possono contenere determinati caratteri nei nomi dei file. Se un file contiene uno dei seguenti caratteri nel nome del file, i caratteri vengono rimossi dal nome del file al caricamento: `! # % * \ | ' " / ? < > { } [ ]`.
