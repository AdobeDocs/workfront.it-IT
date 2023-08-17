---
product-area: documents
navigation-topic: add-documents-to-workfront
title: Aggiungere documenti ad Adobe Workfront dal file system
description: È possibile aggiungere documenti a progetti, attività o problemi nelle seguenti aree in Adobe Workfront - MODIFICA.
author: Courtney
feature: Digital Content and Documents
exl-id: 0a5f82b2-f86e-4ffa-b3a6-18221dd0e158
source-git-commit: 55ba26b65cf046806f5a198e4de1b5eed2e08384
workflow-type: tm+mt
source-wordcount: '751'
ht-degree: 1%

---

# Aggiungere documenti ad Adobe Workfront dal file system

{{preview-and-fast-release}}

È possibile aggiungere documenti a progetti, attività o problemi nelle seguenti aree in Adobe Workfront:

* Area Documenti globale
* Area Documenti per un oggetto Workfront
* <span class="preview">Una scheda collegata su una scheda Workfront</span>

È inoltre possibile caricare nuove versioni di documenti e aggiungere collegamenti a documenti di fornitori di cloud di terze parti, ad esempio Google Drive, Dropbox e Microsoft OneDrive. Per informazioni sull&#39;aggiunta di nuove versioni di documenti, vedere [Carica una nuova versione di un documento](../../documents/managing-documents/upload-new-document-version.md). Per informazioni sull’aggiunta di documenti di fornitori cloud di terze parti, consulta [Collegare documenti da applicazioni esterne](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

Non esistono restrizioni sui tipi e sulle dimensioni dei file che è possibile caricare in Workfront. Tuttavia, per avere successo, il caricamento deve essere completato entro cinque minuti e devi disporre di spazio di archiviazione sufficiente.

Per informazioni sul caricamento di nuove versioni di un documento in Workfront, consulta [Carica una nuova versione di un documento](../../documents/managing-documents/upload-new-document-version.md).

## Requisiti di accesso

Devi avere i seguenti:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p> Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenze Adobe Workfront*</td> 
   <td> <p>Richiedi o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modifica accesso ai documenti</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

## Aggiungi documenti a Workfront

È possibile aggiungere nuovi documenti a Workfront dal file system della workstation. È inoltre possibile collegare documenti da applicazioni di terze parti, ad esempio Google Drive e SharePoint.

>[!NOTE]
>
>Anche se non esiste un limite di dimensione per il caricamento dei documenti, il download dei documenti è limitato a 4 GB.

Per aggiungere un documento:

1. Passare al progetto, all&#39;attività o al problema in cui si desidera aggiungere un nuovo documento.
1. Fai clic su **Documenti** , quindi fare clic sulla scheda **Aggiungi nuovo** menu a discesa.

   ![](assets/add-new-350x138.png)

1. A seconda del tipo di documento che si desidera aggiungere, eseguire una delle operazioni seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Caricare documenti dal file system sulla workstation</td> 
      <td> 
       <ol> 
        <li value="1">Dalla sezione <strong>Aggiungi nuovo</strong> menu a discesa, seleziona <strong>Documento.</strong></li> 
        <li value="2"> <p>Individuare e selezionare il documento che si desidera aggiungere dal file system della workstation.<br></p> <p>È possibile selezionare più documenti premendo il tasto Maiusc mentre si selezionano altri file.</p> </li> 
        <li value="3">Clic <strong>Apri</strong>.</li> 
       </ol> 
       <p><b>NOTA</b>: è anche possibile trascinare i file direttamente dal file manager nell’elenco dei documenti.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Caricare documenti da un'applicazione di terze parti come Google Drive o SharePoint</td> 
      <td> 
       <ol> 
        <li value="1"> <p>Dalla sezione <strong>Aggiungi nuovo</strong> menu a discesa, seleziona <strong>Da &lt;name_of_third-party_application&gt;</strong>.</p> <p>Ad esempio, per caricare un documento da Google Drive, fare clic su <strong>Da Google Drive</strong>.</p> </li> 
        <li value="2"> <p>Seguire le istruzioni per selezionare il documento nell'applicazione di terze parti.<br></p> <p>Per ulteriori informazioni sui documenti collegati, vedere <a href="../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md" class="MCXref xref">Collegare documenti da applicazioni esterne</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Richiedere un documento a un altro utente di Workfront</td> 
      <td> 
       <ol> 
        <li value="1">Dalla sezione <strong>Aggiungi nuovo</strong> menu a discesa, seleziona <strong>Richiedi un documento</strong>.</li> 
        <li value="2">In <strong>A chi lo stai richiedendo?</strong> digitare il nome dell'utente che richiede il documento.</li> 
        <li value="3">In <strong>Informali sulla tua richiesta</strong> digitare il nome del documento.</li> 
        <li value="4"> <p>Clic <strong>Invia richiesta</strong>.</p> <p>La richiesta viene visualizzata nella scheda Documenti.</p> <p> <img src="assets/request-a-document-350x110.png" style="width: 350;height: 110;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> <p>Per ulteriori informazioni sulla richiesta di documenti, consulta <a href="../../documents/adding-documents-to-workfront/request-a-document.md" class="MCXref xref">Richiedi un documento</a>.</p> </li> 
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

Se Workfront rileva un documento danneggiato, Workfront interrompe il processo di caricamento e viene visualizzato un messaggio che indica che il file è danneggiato. Ricevi inoltre una notifica e-mail quando Workfront rileva contenuti potenzialmente dannosi e il file è pianificato per la rimozione.

I file danneggiati vengono rimossi entro 24 ore dal rilevamento, a meno che non vengano rimossi manualmente. Se elimini un file danneggiato, Workfront tiene traccia di questa azione come aggiornamento. Se consenti a Workfront di rimuoverlo, non vengono registrati aggiornamenti.

### Limitazioni per i nomi dei file {#file-name-restrictions}

I file caricati in Workfront non possono contenere determinati caratteri nei nomi dei file. Se un file contiene uno dei seguenti caratteri nel nome del file, questi vengono rimossi dal nome al momento del caricamento del file: `< > { }`.
