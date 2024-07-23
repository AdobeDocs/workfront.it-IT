---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Creare una nuova versione di una bozza
description: Gestire il feedback tra più versioni o revisioni di un lavoro può essere una sfida enorme. Workfront semplifica questo processo consentendo la creazione e il confronto di più versioni di una bozza.
author: Courtney
feature: Digital Content and Documents
exl-id: ee0c859e-349b-4e7a-ac80-164740b950f0
source-git-commit: 7477b62cf0e2e61966f8e74cf268217e2ceb67ef
workflow-type: tm+mt
source-wordcount: '1734'
ht-degree: 0%

---

# Creare una nuova versione di una bozza

Gestire il feedback tra più versioni o revisioni di un lavoro può essere una sfida enorme. Workfront semplifica questo processo consentendo la creazione e il confronto di più versioni di una bozza.

Quando crei una nuova versione di una bozza, considera le seguenti informazioni:

* Puoi assegnare a un utente l’autorizzazione per visualizzare una versione, ma non un’altra. Al contrario, se condividi una versione successiva con un utente, quest’ultimo non può visualizzare le versioni precedenti a meno che tu non torni indietro e conceda esplicitamente all’utente l’accesso a tali versioni precedenti.
* Per creare una nuova versione di una bozza, è necessario disporre dei diritti di modifica per la bozza.

  Per ulteriori informazioni su chi dispone dei diritti di modifica su una bozza, consulta [Gestire i ruoli della bozza in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md) e [Profili delle autorizzazioni della bozza in Workfront Proof](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

  Per informazioni sulla condivisione delle versioni delle bozze, consulta  [Condividi bozza in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md).

>[!IMPORTANT]
>
>Se viene creata una bozza in Adobe Workfront, tutte le nuove versioni create per tale bozza devono essere create anche in Workfront. Non è possibile creare una nuova versione di una bozza in Workfront Proof se tale bozza è stata creata in Workfront.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Piano corrente: Pro o superiore</p> <p>oppure</p> <p>Piano legacy: Seleziona o Premium</p> <p>Per ulteriori informazioni sulla verifica dell'accesso con i diversi piani, vedere <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accesso alla funzionalità di verifica in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano corrente: Lavoro o Piano</p> <p>Piano legacy: qualsiasi (per l’utente deve essere abilitata la verifica)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Profilo autorizzazione bozza </td> 
   <td>Manager o superiore</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modifica accesso ai documenti</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, la mansione o il profilo di autorizzazione della bozza di cui si dispone, contattare l&#39;amministratore di Workfront o Workfront Proof.

+++

## Creare una nuova versione di una bozza in Workfront

Esistono diversi modi per caricare una nuova versione di bozza in Workfront. Le impostazioni di bozza predefinite possono essere o meno riportate dalla versione precedente, a seconda del metodo scelto:

* **Genera automaticamente le bozze durante il caricamento dei documenti**: le impostazioni di bozza predefinite non vengono riportate. Se questa impostazione è abilitata nel profilo utente, le impostazioni predefinite della bozza non vengono riportate quando si trascina e rilascia una nuova versione.
* **Crea bozza > Semplice**: le impostazioni di bozza predefinite non vengono riportate. Se selezioni Semplice durante la creazione di una nuova versione della bozza, le impostazioni predefinite della bozza non vengono riportate dalla versione precedente.
* **Aggiungi nuovo > Versione > Bozza**: le impostazioni di bozza predefinite vengono riportate dalla versione precedente.
* **Crea bozza > Avanzate**: le impostazioni predefinite della bozza vengono riportate dalla versione precedente.

  <table>
  <tbody>
  <tr>
  <td>Genera automaticamente delle bozze quando vengono caricati i documenti</td>
  <td>Le impostazioni di bozza predefinite non vengono riportate. Se questa impostazione è abilitata nel profilo utente, le impostazioni predefinite della bozza non vengono riportate quando si trascina e rilascia una nuova versione.</td>
  </tr>
  <tr>
  <td>Crea bozza &gt; Semplice</td>
  <td>Le impostazioni di bozza predefinite non vengono riportate. Se selezioni Semplice durante la creazione di una nuova versione della bozza, le impostazioni predefinite della bozza non vengono riportate dalla versione precedente.</td>
  </tr>
  <tr>
  <td>Aggiungi nuovo &gt; Versione &gt; Bozza</td>
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

   Seleziona la riga in cui è elencata la bozza, fai clic su **Aggiungi nuovo** > **Versione**, quindi fai clic sull&#39;opzione che desideri utilizzare per aggiungere la nuova versione della bozza.

   ![](assets/add-new-version-350x185.png)

## Creare una nuova versione di una bozza dal visualizzatore di bozze (solo Workfront Proof)

Se utilizzi il Workfront Proof autonomo, puoi creare una nuova versione di una bozza contenente un singolo file o una web capture. 

>[!NOTE]
>
>Se il tuo account fa parte di un piano Enterprise e carichi più file o clip web, questi verranno automaticamente combinati in un’unica nuova versione. Per ulteriori informazioni, consulta [Creare una bozza multipagina](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md).

Per creare una nuova versione di una bozza in Workfront Proof:

1. Apri la bozza.
1. Fai clic sul menu a discesa **Versione** nell&#39;angolo superiore sinistro, quindi fai clic su **+ Nuova versione** nella casella visualizzata.

   Nella pagina **Nuova versione bozza di** visualizzata è possibile visualizzare tutti i revisori della versione precedente, inclusi i ruoli e le impostazioni delle notifiche e-mail. Puoi modificare facilmente i ruoli e le notifiche dei revisori esistenti o rimuovere i revisori esistenti dalla nuova versione in questa pagina.

1. In **Aggiungi file**, carica un file come nuova versione della bozza trascinandolo dal computer o facendo clic su **sfoglia** e selezionando il file desiderato. È possibile digitare un **Nome bozza** per la versione oppure lasciare vuota questa casella per utilizzare lo stesso nome file con un numero di versione aggiunto alla fine.

   Oppure

   Acquisisci una pagina web come nuova versione della bozza digitando un URL.

   >[!NOTE]
   >
   >Il trascinamento della selezione è disponibile solo con i browser che supportano completamente HTML5. Sono esclusi Internet Explorer 7-9 e Safari.

1. In **Flusso di lavoro**, apporta una delle seguenti modifiche per specificare i revisori per questa versione della bozza.

   I revisori della versione precedente vengono sostituiti dai revisori aggiunti.

   * Modifica il **Proprietario** della versione con un altro utente nel tuo account.\
     Per informazioni sulle autorizzazioni del proprietario, vedere [Profili autorizzazioni bozza in Workfront Proof](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

   * Utilizzando **Digita il nome o l&#39;indirizzo di posta elettronica del contatto per aggiungere una casella del destinatario**, aggiungi i revisori alla versione. Puoi specificare un **Ruolo bozza** e un tipo **Avvisi e-mail** per ogni destinatario.

     Per informazioni sull’aggiunta di gruppi alla bozza, consulta  [Aggiungere gruppi a una bozza](../../../workfront-proof/wp-mnguserscontacts/groups/add-groups.md). Per informazioni sui ruoli, vedere [Gestione ruoli bozza in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

     >[!NOTE]
     >
     >Se il creatore o il proprietario di  la bozza ha [L&#39;e-mail bozza creata](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md) disabilitata per impostazione predefinita (nelle impostazioni personali), non riceverà alcuna e-mail bozza creata o nuova bozza anche se nella pagina Nuova bozza è selezionata la casella Notify people by email (Notifica persone per e-mail). Per informazioni sulle notifiche e-mail, vedere [Configurare le impostazioni delle notifiche e-mail in Workfront Proof](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md). Vedi anche [E-mail bozza creata](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md) e [E-mail nuova bozza](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md).

   * Imposta una scadenza per la bozza della versione.
   * Passa il puntatore del mouse sul nome di un revisore per vedere tutte le decisioni che ha preso su una versione precedente.

1. In **Notifica e-mail** eseguire una delle operazioni seguenti:

   * Specificare se si desidera notificare ai revisori la nuova versione.\
     La selezione verrà registrata nella sezione Attività della pagina Dettagli bozza. Per ulteriori informazioni, vedere [Gestire i dettagli della bozza in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

   * Aggiungi un oggetto e un messaggio personalizzati.

1. Nella sezione **Organizzazione** eseguire una delle operazioni seguenti: 

   * Applica uno o più tag alla bozza. Per ulteriori informazioni, vedere [Creare e gestire i tag in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-and-manage-tags.md).\
     I tag vengono ereditati anche dalla versione precedente della bozza. Se aggiungi un nuovo tag alla nuova versione, vengono taggate anche le versioni precedenti.

   * Aggiungi la versione a una cartella. Per ulteriori informazioni, vedere [Gestione cartelle in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md). La cartella verrà copiata dalla versione precedente della bozza. Se selezioni una cartella diversa, verrà spostata l’intera bozza (tutte le versioni).

   * Gli amministratori di fatturazione e gli amministratori possono rendere obbligatorio il campo della cartella in tutto l’account nella scheda Impostazioni. Per ulteriori informazioni, vedere.

1. In Impostazioni bozza apportare una delle modifiche seguenti:

   * Richiedi accesso alla bozza
   * Richiedi firme elettroniche nella bozza (solo per il piano Enterprise)
   * Blocca la bozza quando vengono prese tutte le decisioni
   * Consenti o blocca il download del file originale
   * Condivisione pubblica della bozza, incluse le impostazioni di condivisione pubbliche
   * Iscrizione alla bozza\
     Le selezioni effettuate in questa sezione vengono visualizzate nella pagina Dettagli bozza (dove è possibile modificare alcuni campi). Per ulteriori informazioni, vedere [Gestire i dettagli della bozza in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

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
* Deselezionare la casella Notify people by email (Notifica alle persone per posta elettronica), ovvero non verrà inviata alcuna e-mail ai revisori per notificare loro che dispongono di una nuova versione da rivedere.

  >[!NOTE]
  >
  >Nessun oggetto/messaggio personalizzato predefinito salvato nelle impostazioni personali influisce su questo valore.

Se nelle impostazioni personali sono salvati un oggetto e un messaggio predefiniti, questo influirà sul messaggio visualizzato per impostazione predefinita nella pagina Nuova versione:

* Se si sceglie di inviare una notifica ai revisori tramite e-mail per la versione precedente della bozza utilizzando l&#39;e-mail standard (ad esempio, nessun oggetto/messaggio personalizzato), l&#39;oggetto/messaggio personalizzato predefinito (le impostazioni personali) verrà visualizzato nella pagina Nuova versione. Puoi quindi modificare l’oggetto personalizzato e il messaggio o deselezionare la casella Notifica alle persone per e-mail (ovvero non verrà inviata alcuna e-mail ai revisori per comunicare loro che dispongono di una nuova versione da rivedere).
* Se hai scelto di non inviare ai revisori una notifica via e-mail per la versione precedente della bozza (ad esempio, senza inviare un’e-mail standard o personalizzata), la pagina Nuova versione non includerà alcun messaggio per impostazione predefinita. Per notificare ai revisori la nuova versione, fare clic sul collegamento Invia un messaggio, che consente di visualizzare l&#39;oggetto o il messaggio personalizzato predefinito (in base alle impostazioni personali). Se necessario, puoi quindi modificare l’oggetto personalizzato e il messaggio.

Se nelle impostazioni personali non vengono salvati un oggetto e un messaggio predefiniti, nella pagina Nuova versione verrà visualizzato quanto segue:

* Se si sceglie di inviare una notifica ai revisori tramite e-mail per la versione precedente della bozza utilizzando l&#39;e-mail standard (ad esempio, nessun oggetto/messaggio personalizzato), nella pagina Nuova versione verrà selezionata per impostazione predefinita l&#39;opzione Notifica persone per e-mail. Per aggiungere un messaggio personalizzato, fai clic sul collegamento.
* Se hai scelto di non inviare ai revisori una notifica via e-mail per la versione precedente della bozza (ad esempio, senza inviare un’e-mail standard o personalizzata), la pagina Nuova versione non includerà alcun messaggio per impostazione predefinita. Per notificare ai revisori la nuova versione, fare clic sul collegamento Invia un messaggio. È quindi possibile aggiungere un oggetto e un messaggio personalizzati facendo clic sul collegamento Aggiungi messaggio personalizzato.
