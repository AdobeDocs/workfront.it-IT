---
content-type: release-notes
navigation-topic: 2019-4-release-activity
title: 2019.4 altri miglioramenti
description: Questa pagina descrive vari miglioramenti apportati alla versione 2019.4 di. Sarà reso disponibile nell’ambiente di produzione la settimana dell’11 novembre 2019.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: ed7488f1-2076-4160-97f3-a3da25cccd0f
source-git-commit: e1bf5fbc7dc25bf8ce472b21b9a0906530f82cf0
workflow-type: tm+mt
source-wordcount: '627'
ht-degree: 0%

---

# 2019.4 altri miglioramenti

Questa pagina descrive vari miglioramenti apportati alla versione 2019.4 di. Sarà reso disponibile nell’ambiente di produzione la settimana dell’11 novembre 2019.

Per un elenco di tutte le modifiche apportate in 2019.4, consulta [Panoramica sulla versione 2019.4](../../../../product-announcements/product-releases/quarterly-release-archive/2019.4-release-activity/2019-4-release-activity-overview.md).

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td> <strong>Avvia un flusso di lavoro di verifica automatizzata da un Adobe documento CC</strong> <p>Senza uscire da Adobe CC, è possibile avviare un flusso di lavoro di verifica automatizzato per un documento Adobe CC creato. Per ulteriori informazioni, vedere la sezione <a href="../../../../documents/workfront-for-adobe-creative-cloud/use-wf-adobe-cc.md#generate" class="MCXref xref" xrefformat="{para}">Generare una bozza da Illustrator o InDesign</a> nell'articolo <a href="../../../../documents/workfront-for-adobe-creative-cloud/use-wf-adobe-cc.md" class="MCXref xref" xrefformat="{para}">Utilizzare l'estensione Workfront per Illustrator e InDesign</a>.</p> </td> 
  </tr> 
  <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td><strong>Workfront G Suite add-on</strong> <p>Now you can manage Workfront objects directly from Gmail, Google Calendar, and Google Drive.</p> <p>When you open a Workfront notification email, instantly view all information about the associated object and take actions, such as reviewing content or updating a status, without leaving your Inbox.</p> <p>When you open a non-Workfront email:</p> 
     <ul> 
      <li>Convert it into a task or issue.</li> 
      <li>Associate it with a project.</li> 
      <li>Assign it as a work item.</li> 
      <li>Add it to a work item as an update.</li> 
      <li>Upload its attachments to Workfront.</li> 
     </ul> <p>Manage Workfront objects without leaving G Suite:</p> 
     <ul> 
      <li>Post updates and replies to comments.</li> 
      <li>View and manage documents associated with a task or issue.</li> 
     </ul> <p>Access and work with object details:</p> 
     <ul> 
      <li>Read the description</li> 
      <li>View the parent object</li> 
      <li>Change the status</li> 
      <li>Access custom data</li> 
      <li>Mark it as complete.</li> 
     </ul> <p>And access your Workfront Home content, including tasks, issues, approvals, and access requests, without leaving G Suite.</p> <p>For more information, see <a href="../../../../workfront-integrations-and-apps/workfront-for-g-suite/workfront-for-gsuite.md" class="MCXref xref" xrefformat="{para}">Adobe Workfront for G Suite</a>.</p> </td> 
   </tr>
  --> 
  <tr> 
   <td> <strong>Impedisci indirizzi e-mail duplicati</strong> <p>Non è più possibile utilizzare lo stesso indirizzo e-mail quando si creano più utenti in Workfront, anche se tali indirizzi variano a seconda dei casi. Ad esempio, non puoi creare un utente con l’indirizzo e-mail JohnDoe@example.com e un altro utente con l’indirizzo e-mail johndoe@example.com. </p> <p>Prima di questa modifica, era supportata la creazione di utenti con indirizzi e-mail corrispondenti che si differenziavano solo per maiuscole e minuscole. </p> <p>Nota: gli utenti esistenti con indirizzi e-mail corrispondenti che differiscono solo per caso dovranno essere aggiornati in una data futura. Se in un’istanza di Workfront sono presenti utenti con indirizzi e-mail corrispondenti che si differenziano solo per maiuscole e minuscole, Workfront ti contatterà con informazioni aggiuntive e una timeline quando è necessario aggiornarli.</p> </td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <strong>Ulteriori tipi di oggetto disponibili per i campi Typeahead in un modulo personalizzato</strong> 
     <p>Ora, quando si crea un campo personalizzato Automatico, è possibile associare al campo i seguenti tipi di oggetto: Utente, Società, Gruppo, Mansione, Portfolio, Programma, Progetto e Modello.</p> 
     <p>In precedenza era possibile associare solo il tipo di oggetto User a un campo personalizzato Typeahead.</p> 
     <p>Per ulteriori informazioni, vedere la sezione <a href="../../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#create" class="MCXref xref" xrefformat="{para}">Creare o modificare un modulo personalizzato</a> nell'articolo <a href="../../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref" xrefformat="{para}">Creare o modificare un modulo personalizzato</a>.</p> 
    </div> </td> 
  </tr> 
  <tr> 
   <td> <strong>Nome file della versione più recente di un documento visualizzato</strong> <p>Ora, quando si carica una versione del documento con un nome di file diverso da quello della versione esistente, il nuovo nome di file viene visualizzato in Workfront.</p> <p>In precedenza, quando si aggiungeva una nuova versione con un nome di file diverso, il nome del file della versione precedente continuava a essere visualizzato in Workfront.</p> <p>Per ulteriori informazioni, vedere <a href="../../../../documents/managing-documents/upload-new-document-version.md" class="MCXref xref" xrefformat="{para}">Caricare una nuova versione di un documento</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <strong>Aggiungere un filtro a un campo automatico in un modulo personalizzato</strong> <p>Ora, quando si aggiunge un campo automatico a un modulo personalizzato, è possibile aggiungere un filtro per limitare gli oggetti disponibili quando un utente utilizza il campo. Ad esempio, puoi limitare il campo in modo che l’utente possa selezionare solo i membri del team Marketing e Vendite della tua organizzazione.</p> <p>Per ulteriori informazioni, consulta la sezione Creare e aggiungere un nuovo campo nell’articolo Creazione di un Forms personalizzato.</p> </td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <strong>Modifica il tipo di visualizzazione di un campo in un modulo personalizzato</strong> 
     <p>Ora è possibile modificare il tipo di visualizzazione di un campo in un modulo personalizzato.</p> 
     <p>Se ad esempio è stato creato un campo Caselle di controllo, è possibile modificarlo in un campo a discesa o in un campo Pulsanti di scelta. Questi tre tipi di visualizzazione dei campi sono intercambiabili.</p> 
     <p>In alternativa, se è stato creato un campo di testo a riga singola, è possibile modificarlo in un campo di testo paragrafo. Questi due tipi di visualizzazione dei campi sono intercambiabili.</p> 
     <p>In precedenza, per modificare il tipo di visualizzazione di un campo personalizzato, era necessario creare un nuovo campo ed eliminare quello precedente. Questo richiedeva il trasferimento dei dati, operazione che spesso richiedeva molto tempo.</p> 
     <p>Per ulteriori informazioni, vedere <a href="../../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#create" class="MCXref xref" xrefformat="{para}">Creare o modificare un modulo personalizzato</a> nell'articolo <a href="../../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref" xrefformat="{para}">Creare o modificare un modulo personalizzato</a></p> 
    </div> </td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <strong>Creazione di calendari e report dell'indisponibilità</strong> 
     <p>Ora puoi vedere il tempo libero dell’utente per una migliore pianificazione ed esecuzione. Puoi anche aggiungere ai dashboard nuovi rapporti e calendari di ferie per una visualizzazione in tempo reale della disponibilità degli utenti.</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>
