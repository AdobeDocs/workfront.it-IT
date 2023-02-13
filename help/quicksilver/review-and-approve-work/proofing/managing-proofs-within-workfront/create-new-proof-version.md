---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Creare una nuova versione di una bozza
description: La gestione del feedback in più versioni o revisioni di un pezzo di lavoro può essere una sfida enorme. Workfront semplifica questo processo consentendo di creare e confrontare più versioni di una bozza.
author: Courtney
feature: Digital Content and Documents
exl-id: ee0c859e-349b-4e7a-ac80-164740b950f0
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '1721'
ht-degree: 0%

---

# Creare una nuova versione di una bozza

La gestione del feedback in più versioni o revisioni di un pezzo di lavoro può essere una sfida enorme. Workfront semplifica questo processo consentendo di creare e confrontare più versioni di una bozza.

Quando crei una nuova versione di una bozza, considera quanto segue:

* Puoi concedere a un utente l’autorizzazione per vedere una versione ma non un’altra. Al contrario, se condividi una versione successiva con un utente, quest’ultimo non può vedere le versioni precedenti a meno che tu non torni indietro e conceda esplicitamente all’utente l’accesso a tali versioni precedenti.
* Per creare una nuova versione di una bozza, è necessario disporre dei diritti di modifica sulla bozza.

   Vedi [Gestire i ruoli delle prove in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md) e [Profili delle autorizzazioni di prova in Workfront Proof](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) per ottenere ulteriori informazioni su chi dispone di diritti di modifica su una bozza.

   Per informazioni sulla condivisione delle versioni a prova, vedi  [Condividi una bozza in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md).

>[!IMPORTANT]
>
>Se una bozza viene creata in Adobe Workfront, è necessario creare anche tutte le nuove versioni create per tale bozza all’interno di Workfront. Non è possibile creare una nuova versione di una bozza all’interno di Workfront Proof se la bozza è stata creata in Workfront.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Piano attuale: Pro o superiore</p> <p>oppure</p> <p>Piano legacy: Seleziona o Premium</p> <p>Per ulteriori informazioni sulla verifica dell’accesso con i diversi piani, consulta <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accesso alle funzionalità di correzione in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano attuale: Lavoro o piano</p> <p>Piano legacy: Qualsiasi (è necessario che la correzione sia attivata per l’utente)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Profilo autorizzazione bozza </td> 
   <td>Manager o superiore</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica accesso ai documenti</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il ruolo o il profilo delle autorizzazioni di prova, contattare l&#39;amministratore Workfront o Workfront Proof.

## Creare una nuova versione di una bozza in Workfront

Esistono diversi modi per caricare una nuova versione di prova in Workfront. Le impostazioni predefinite della bozza possono essere riportate o meno dalla versione precedente a seconda del metodo scelto:

* **Generazione automatica di bozze durante il caricamento di documenti**: Le impostazioni di bozza predefinite non vengono riportate. Se questa impostazione è abilitata nel profilo utente, le impostazioni di bozza predefinite non vengono mantenute quando trascini e rilasci una nuova versione.
* **Crea bozza > Semplice**: Le impostazioni di bozza predefinite non vengono riportate. Se scegli Semplice durante la creazione di una nuova versione di bozza, le impostazioni di bozza predefinite non vengono riportate dalla versione precedente.
* **Aggiungi nuovo > Versione > Prova**: Le impostazioni di bozza predefinite vengono riportate dalla versione precedente.
* **Crea bozza > Avanzate**: Le impostazioni di bozza predefinite vengono riportate dalla versione precedente.

   <table>
  <tbody>
  <tr>
  <td>Genera automaticamente delle bozze quando vengono caricati i documenti</td>
  <td>Le impostazioni di bozza predefinite non vengono riportate. Se questa impostazione è abilitata nel profilo utente, le impostazioni di bozza predefinite non vengono mantenute quando trascini e rilasci una nuova versione.</td>
  </tr>
  <tr>
  <td>Crea bozza &gt; Semplice</td>
  <td>Le impostazioni di bozza predefinite non vengono riportate. Se scegli Semplice durante la creazione di una nuova versione di bozza, le impostazioni di bozza predefinite non vengono riportate dalla versione precedente.</td>
  </tr>
  <tr>
  <td>Aggiungi nuovo &gt; Versione &gt; Prova</td>
  <td>Le impostazioni di bozza predefinite vengono riportate dalla versione precedente.</td>
  </tr>
  <tr>
  <td>Crea bozza &gt; Avanzate</td>
  <td>Le impostazioni di bozza predefinite vengono riportate dalla versione precedente.</td>
  </tr>
  </tbody>
  </table>




Per creare una nuova versione di una bozza:

1. Aprire l&#39;elenco di documenti contenente la bozza.
1. Dal file system del computer, trascinare un nuovo file sulla bozza.

   Oppure

   Seleziona la riga in cui è elencata la bozza, fai clic su **Aggiungi nuovo** > **Versione**, quindi fai clic sull’opzione da utilizzare per aggiungere la nuova versione della bozza.

   ![](assets/add-new-version-350x185.png)

## Creare una nuova versione di una bozza dal visualizzatore di correzione (solo per Workfront Proof)

Se utilizzi Workfront Proof autonomo, puoi creare una nuova versione di una bozza contenente un singolo file o un’acquisizione Web. 

>[!NOTE]
>
>Se il tuo account è su un piano Enterprise e carichi più file o acquisizioni web, verranno automaticamente combinati in una singola nuova versione. Vedi [Creare una bozza a più pagine](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md) per ulteriori informazioni.

Per creare una nuova versione di una bozza in Workfront Proof:

1. Apri la bozza.
1. Fai clic sul pulsante **Versione** menu a discesa nell&#39;angolo in alto a sinistra, quindi fai clic su **+ Nuova versione** nella casella visualizzata.

   Sulla **Nuova versione a prova di** viene visualizzata una pagina che mostra tutti i revisori della versione precedente, inclusi i relativi ruoli e le impostazioni di notifica via e-mail. Puoi modificare facilmente i ruoli e le notifiche dei revisori esistenti o rimuovere i revisori esistenti dalla nuova versione di questa pagina.

1. Sotto **Aggiungi file**, carica un file come nuova versione della bozza trascinandolo dal computer o facendo clic su **navigare** e selezionare il file desiderato. È possibile digitare un **Nome della bozza** per la versione o lasciare vuota questa casella per utilizzare lo stesso nome file con un numero di versione aggiunto alla fine.

   Oppure

   Acquisisci una pagina web come nuova versione della bozza digitando un URL.

   >[!NOTE]
   >
   >La funzione di trascinamento è disponibile solo con i browser che supportano completamente HTML5. Ciò esclude Internet Explorer da 7 a 9 e Safari.

1. Sotto **Flusso di lavoro**, apporta una delle seguenti modifiche per specificare i revisori per questa versione della bozza.

   I revisori della versione precedente vengono sostituiti dai revisori aggiunti.

   * Modificare la **Proprietario** della versione a un altro utente del tuo account.\
      Per informazioni sulle autorizzazioni del proprietario, consulta [Profili delle autorizzazioni di prova in Workfront Proof](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

   * Utilizzo della **Digitare il nome del contatto o l&#39;indirizzo e-mail per aggiungere una casella del destinatario**, aggiungi i revisori alla versione. Puoi specificare un **Ruolo di prova** e **Avvisi e-mail** digita per ogni destinatario.

      Per informazioni sull’aggiunta di gruppi alla bozza, consulta  [Aggiungi gruppi a una bozza](../../../workfront-proof/wp-mnguserscontacts/groups/add-groups.md). Per informazioni sui ruoli, consulta [Gestire i ruoli delle prove in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

      >[!NOTE]
      >
      >Se il creatore o il proprietario della prova ha [E-mail di bozza creata](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md) disattivato per impostazione predefinita (nelle impostazioni personali), non riceverà alcun messaggio e-mail Proof made o New proof nemmeno se la casella Notifica le persone tramite e-mail è selezionata nella pagina Nuova bozza . Per informazioni sulle notifiche e-mail, vedi [Configurare le impostazioni di notifica e-mail in Workfront Proof](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md). Vedi anche [E-mail di bozza creata](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md) e [Nuova e-mail a prova di](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md).

   * Imposta una scadenza della bozza per la versione.
   * Passa il puntatore del mouse sul nome di un revisore per vedere tutte le decisioni prese in merito a una versione precedente.

1. Sotto **Notifica e-mail**, effettua una delle seguenti operazioni:

   * Specifica se desideri avvisare i revisori della nuova versione.\
      La selezione verrà registrata nella sezione Attività della pagina Dettagli bozza. Per ulteriori informazioni, consulta [Gestire i dettagli delle prove in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

   * Aggiungi un oggetto e un messaggio personalizzati.

1. In **Organizzazione** eseguire una delle operazioni seguenti: 

   * Applica uno o più tag alla bozza. Per ulteriori informazioni, consulta [Creare e gestire tag in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-and-manage-tags.md).\
      I tag vengono ereditati anche dalla versione precedente della bozza. Se aggiungi un nuovo tag alla nuova versione, vengono assegnati tag anche alle versioni precedenti.

   * Aggiungi la versione a una cartella. Vedi [Gestione cartelle in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md) per ulteriori informazioni. La cartella verrà copiata dalla versione precedente della bozza. Se selezioni una cartella diversa, l’intera bozza (tutte le versioni) verrà spostata.

   * Gli amministratori e gli amministratori di fatturazione possono rendere obbligatorio il campo della cartella per l’intero account nella scheda Impostazioni. Per ulteriori informazioni, consulta .

1. In Impostazioni bozza, apporta una delle seguenti modifiche:

   * Richiedi accesso alla bozza
   * Richiedi firme elettroniche sulla bozza (solo piano aziendale)
   * Blocca la prova quando vengono prese tutte le decisioni
   * Consenti o blocca il download del file originale
   * Condivisione pubblica delle prove, comprese le impostazioni di condivisione pubbliche
   * Iscrizione alla bozza\
      Le selezioni effettuate in questa sezione vengono visualizzate nella pagina dei dettagli Prova (dove è possibile modificare alcuni campi). Per ulteriori informazioni, consulta [Gestire i dettagli delle prove in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Create a new version of a proof from the proofing viewer</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To create a new version from the proofing viewer</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Open the proof.</li>
<li value="2"> <p>Click the <strong>Version</strong> drop-down menu in the upper-left corner, then click <strong>+ New version</strong> in the box that appears.</p> <p>On the <strong>New proof version of</strong> page that appears, you can see all the reviewers from the previous version, including their roles and email notification settings. You can easily edit the roles and notifications of existing reviewers or remove existing reviewers from the new version on this page.</p> </li>
<li value="3"> <p>Under <strong>Add files</strong>, upload a file as a new version of the proof by dragging and dropping from your computer or by clicking <strong>browse</strong> and selecting the file you want. You can type a&nbsp;<strong>Proof name</strong>&nbsp;for the version or leave this box blank to&nbsp;use the same filename with a version number added on the end.</p> <p>Or<br></p> <p>Capture a web page as a new version of the proof by typing a URL</p> <note type="note">
Drag and drop is available only with browsers that fully support HTML5. This excludes Internet Explorer 7 through 9 and Safari.
<br>
</note> </li>
<li value="4"> <p>Under <strong>Workflow</strong>, make any of the following changes to specify the reviewers for this version of the proof.</p> <p>Reviewers from the previous version are replaced by the reviewers you add.</p>
<ul>
<li>Change the <strong>Owner</strong> of the version to another user in your account.<br>For information about owner permissions, see <a href="../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md" class="MCXref xref">Proof Permissions Profiles in Workfront Proof</a>.</li>
<li> <p>Using the <strong>Type contact name or email address to add a recipient box</strong>, add reviewers to the version. You can specify a <strong>Proof role</strong> and an <strong>Email alerts</strong> type for each recipient.</p> <p>For information about adding groups to the proof, see&nbsp;<a href="../../../workfront-proof/wp-mnguserscontacts/groups/add-groups.md" class="MCXref xref">Add Groups to a Proof</a>.&nbsp;For information about roles, see <a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md" class="MCXref xref">Manage Proof Roles in Workfront Proof</a>.</p> <note type="note">
If the creator or owner of&nbsp;&nbsp;the proof has
<a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">The Proof Made email</a> disabled by default (in their personal settings), they won't receive any Proof made or New proof emails even if the Notify people by email box is checked on the New proof page. For information about email notifications, see
<a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md" class="MCXref xref">Configure email notification settings in Workfront Proof</a>.&nbsp;See also
<a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">The Proof Made email</a> and
<a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md" class="MCXref xref">New proof email</a>.
<br>
</note> </li>
<li>Set a proof deadline for the version.</li>
<li>Hover over a reviewer's name to see any decisions he or she made on a previous version.</li>
</ul> </li>
<li value="5">Under <strong>Email notification</strong>, do any of the following:
<ul>
<li>Specify whether you want to notify the reviewers of the new version.<br>Your selection will be logged in the Proof activity section on the Proof details page.</li>
<li>Add a custom subject and message.</li>
</ul></li>
<li value="6">Under Proof settings, make any of the changes below:
<ul>
<li>Require login on the proof</li>
<li>Require electronic signatures on the proof (Enterprise plan only)</li>
<li>Lock the proof when all decisions are made</li>
<li>Allow or block download of original file</li>
<li>Public sharing of the proof,&nbsp;including public sharing settings</li>
<li>Subscription to the proof<br>The selections made in this section will be shown in the Proof details page.</li>
</ul></li>
</ol>
-->

## Informazioni sul messaggio Nuova versione

Se nella versione precedente della bozza era incluso un oggetto/messaggio personalizzato, questo verrà visualizzato per impostazione predefinita nella pagina Nuova versione. È possibile:

* Modifica l’oggetto e il messaggio.
* Deseleziona la casella Notifica le persone per e-mail, il che significa che nessun messaggio e-mail verrà inviato ai tuoi revisori per avvisarli di avere una nuova versione da rivedere.

   >[!NOTE]
    Questo non è influenzato da alcun oggetto/messaggio personalizzato predefinito salvato nelle impostazioni personali.

Se nelle impostazioni personali sono stati salvati un oggetto e un messaggio predefiniti, questo influisce sul messaggio visualizzato per impostazione predefinita nella pagina Nuova versione:

* Se hai scelto di inviare una notifica via e-mail ai revisori per la versione precedente della bozza utilizzando l’e-mail standard (ad esempio, nessun oggetto/messaggio personalizzato), l’oggetto/messaggio personalizzato predefinito (impostazioni personali) verrà visualizzato nella pagina Nuova versione . Puoi quindi modificare l’oggetto e il messaggio personalizzati o deselezionare la casella Notifica le persone per e-mail (ovvero non verrà inviata alcuna e-mail ai revisori per avvisarli di avere una nuova versione da rivedere).
* Se si sceglie di non inviare una notifica tramite e-mail ai revisori per la versione precedente della bozza (ad esempio, nessuna e-mail standard o personalizzata), la pagina Nuova versione non includerà alcun messaggio per impostazione predefinita. Per informare i revisori della nuova versione, fai clic sul collegamento Invia un messaggio, che mostrerà l’oggetto/messaggio personalizzato predefinito (in base alle impostazioni personali). Puoi quindi modificare l’oggetto personalizzato e il messaggio, se necessario.

Se nelle impostazioni personali non è stato salvato un oggetto e un messaggio predefiniti, nella pagina Nuova versione verrà visualizzato quanto segue:

* Se hai scelto di inviare una notifica via e-mail ai revisori per la versione precedente della bozza utilizzando l’e-mail standard (ad esempio, nessun oggetto/messaggio personalizzato), l’opzione Notifica le persone per e-mail sarà selezionata per impostazione predefinita nella pagina Nuova versione . Per aggiungere un messaggio personalizzato, fai clic sul collegamento .
* Se si sceglie di non inviare una notifica tramite e-mail ai revisori per la versione precedente della bozza (ad esempio, nessuna e-mail standard o personalizzata), la pagina Nuova versione non includerà alcun messaggio per impostazione predefinita. Per informare i revisori della nuova versione, fai clic sul collegamento Invia un messaggio . Puoi quindi aggiungere un oggetto e un messaggio personalizzati facendo clic sul collegamento Aggiungi messaggio personalizzato .
