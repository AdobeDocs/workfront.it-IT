---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Creare una nuova versione di una bozza
description: Gestire il feedback tra più versioni o revisioni di un lavoro può essere una sfida enorme. Workfront semplifica questo processo consentendo la creazione e il confronto di più versioni di una bozza.
author: Courtney
feature: Digital Content and Documents
exl-id: ee0c859e-349b-4e7a-ac80-164740b950f0
source-git-commit: ac714bd5a5259d6f995ac445efbd0125e07022cb
workflow-type: tm+mt
source-wordcount: '1454'
ht-degree: 0%

---

# Creare una nuova versione di una bozza

<!-- Audited: 4/2025 -->

Gestire il feedback tra più versioni o revisioni di un lavoro può essere una sfida. Adobe Workfront semplifica questo processo consentendoti di creare e confrontare più versioni di una bozza.

Quando crei una nuova versione di una bozza, considera le seguenti informazioni:

* Puoi assegnare a un utente l’autorizzazione per visualizzare una versione, ma non un’altra. Al contrario, se condividi una versione successiva con un utente, quest’ultimo non può visualizzare le versioni precedenti a meno che tu non torni indietro e conceda loro l’accesso alle versioni precedenti.
* Per creare una nuova versione è necessario disporre dei diritti di modifica sulla bozza.

  Per ulteriori informazioni, vedere [Gestione dei ruoli di bozza in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md) e [Profili di autorizzazioni di bozza in Workfront Proof](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

  Per informazioni sulla condivisione delle versioni delle bozze, consulta  [Condividi bozza in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md).

>[!IMPORTANT]
>
>Se viene creata una bozza in Adobe Workfront, è necessario creare anche le nuove versioni di tale bozza in Workfront. Non è possibile creare una nuova versione di una bozza in Workfront Proof se tale bozza è stata creata in Workfront.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> <p>Standard</p> 
   <p>Lavoro o piano</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Profilo autorizzazione bozza </td> 
   <td>Manager o superiore</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica accesso ai documenti</p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creare una nuova versione di bozza in Workfront

Esistono diversi modi per caricare una nuova versione di bozza in Workfront. A seconda del metodo selezionato, le impostazioni di bozza predefinite possono essere o meno riportate dalla versione precedente:

* **Genera automaticamente le bozze durante il caricamento dei documenti**: se questa impostazione è abilitata nel tuo profilo utente, le impostazioni predefinite della bozza non vengono riportate quando trascini e rilasci una nuova versione.
* **Crea bozza > Semplice**: se selezioni questa opzione, le impostazioni di bozza predefinite non verranno riportate dalla versione precedente.
* **Aggiungi nuovo > Versione > Bozza**: se si seleziona questa opzione, le impostazioni predefinite della bozza vengono riportate dalla versione precedente.
* **Crea bozza > Avanzate**: se selezioni questa opzione, le impostazioni di bozza predefinite verranno riportate dalla versione precedente.

Per creare una nuova versione di una bozza:

1. Aprire l&#39;elenco di documenti contenente la bozza.
1. Dal file system del computer, trascinare un nuovo file sulla bozza.

   Oppure

   Seleziona la riga in cui è elencata la bozza, fai clic su **Aggiungi nuovo** > **Versione**, quindi fai clic sull&#39;opzione che desideri utilizzare per aggiungere la nuova versione della bozza.

   ![Aggiungi nuova versione](assets/add-new-proof-version.png)

## Crea una nuova versione di bozza dal visualizzatore di bozze (solo Workfront Proof)

Se utilizzi il Workfront Proof autonomo, puoi creare una nuova versione di una bozza contenente un singolo file o una web capture. 

>[!NOTE]
>
>Se il tuo account fa parte di un piano Enterprise e carichi più file o clip web, questi verranno automaticamente combinati in un’unica nuova versione. Per ulteriori informazioni, consulta [Creare una bozza multipagina](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md).

Per creare una nuova versione di una bozza in Workfront Proof:

1. Apri la bozza.
1. Nell&#39;angolo in alto a sinistra, fare clic sul menu a discesa **Versione**, quindi fare clic su **+ Nuova versione** nella casella visualizzata. Viene visualizzata la pagina Nuova versione bozza.

   ![Aggiungi nuova versione](assets/new-version-button.png)

1. Nella sezione **Aggiungi file**, carica un file come nuova versione della bozza trascinandolo dal computer o facendo clic su **sfoglia** e selezionando un file.

   Oppure

   Acquisisci una pagina web come nuova versione della bozza immettendo un URL.

   >[!NOTE]
   >
   >Il trascinamento della selezione è disponibile solo con i browser che supportano completamente HTML5. Sono esclusi Internet Explorer 7-9 e Safari.

1. (Facoltativo) Seleziona il titolo della bozza e immetti un nuovo **Nome bozza** per la versione.

1. Nella sezione **Flusso di lavoro**, apporta una delle seguenti modifiche per aggiungere revisori per questa versione della bozza (sostituirà i revisori della versione precedente):

   * (Facoltativo) Modifica il **Proprietario** della versione in un altro utente nel tuo account.

     Per informazioni, vedere [Profili autorizzazioni bozza in Workfront Proof](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

   * (Facoltativo) Se si utilizza il nome o l&#39;indirizzo e-mail del contatto **Digitare per aggiungere un destinatario**, aggiungere i revisori alla versione. Puoi quindi selezionare un tipo di **Ruolo bozza** e **Avvisi e-mail** per ogni destinatario.

     Per informazioni, vedere [Aggiungere gruppi a una bozza](../../../workfront-proof/wp-mnguserscontacts/groups/add-groups.md) e [Gestire i ruoli di bozza in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

     >[!NOTE]
     >
     >Se il creatore o il proprietario della bozza ha disabilitato l&#39;e-mail Proof Made per impostazione predefinita nelle proprie impostazioni personali, non riceverà alcuna e-mail Proof Made o New proof anche se la casella **Notify recipients about this proof** (Notifica ai destinatari questa bozza) è selezionata nella pagina New proof (Nuova bozza). Per informazioni, vedere [Configurare le impostazioni delle notifiche e-mail in Workfront Proof](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md), [E-mail bozza creata](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md) e [E-mail nuova bozza](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md).

   * (Facoltativo) Imposta una scadenza per la bozza.

   * (Facoltativo e Condizionale) Selezionare un nuovo responsabile delle decisioni principale nel menu a discesa **Trasferisci diritti di decisione principali a**.

   * (Facoltativo) Seleziona la casella **Richiedi una sola decisione per questa fase** per rimuovere l&#39;opzione di impostare un utente come nuovo decision maker primario.

1. Nella sezione **Notifica e-mail**, selezionare una delle impostazioni seguenti:

   * (Facoltativo) **Notifica ai destinatari questa bozza**: seleziona questa opzione per notificare ai revisori la nuova versione. La selezione verrà registrata nella sezione **Attività** della pagina **Dettagli bozza**. Per ulteriori informazioni, vedere [Gestire i dettagli della bozza in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

   * (Condizionale e facoltativo) **Aggiungi oggetto e messaggio personalizzati**: seleziona questa opzione per aggiungere un oggetto e un messaggio personalizzati alla notifica e-mail.

1. Nella sezione **Organizzazione** selezionare una delle impostazioni seguenti:

   * Applica uno o più tag alla bozza. Per ulteriori informazioni, vedere [Creare e gestire i tag in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-and-manage-tags.md).

   * Aggiungi la versione a una cartella. La cartella verrà copiata dalla versione precedente della bozza. Se selezioni una cartella diversa, verrà spostata l’intera bozza, che include tutte le versioni. Per ulteriori informazioni, vedere [Gestione cartelle in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

   * Gli amministratori di fatturazione e gli amministratori possono rendere obbligatorio il campo della cartella in tutto l&#39;account nella scheda **Impostazioni**.

1. Nella sezione **Impostazioni bozza**, selezionare una delle impostazioni seguenti:

   * Richiedi a un utente di accedere per visualizzare la bozza.
   * Richiedi firme elettroniche nella bozza (solo per il piano Enterprise).
   * Blocca la bozza quando vengono prese tutte le decisioni.
   * Consenti il download del file originale.
   * Consenti la condivisione pubblica della bozza.
   * Consenti la sottoscrizione alla bozza.

     Le selezioni effettuate in questa sezione verranno visualizzate nella pagina **Dettagli bozza** (in cui è possibile modificare alcuni campi). Per ulteriori informazioni, vedere [Gestire i dettagli della bozza in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

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

Se nella versione precedente della bozza era incluso un oggetto/messaggio personalizzato, questo verrà visualizzato per impostazione predefinita nella pagina Nuova versione. Puoi eseguire le seguenti operazioni:

* Modifica l’oggetto e il messaggio.
* Deselezionare la casella Notify people by email (Notifica alle persone per posta elettronica), ovvero non verrà inviata alcuna e-mail ai revisori per notificare loro che dispongono di una nuova versione da rivedere.

  >[!NOTE]
  >
  >Nessun oggetto/messaggio personalizzato predefinito salvato nelle impostazioni personali influisce su questo valore.

Se nelle impostazioni personali sono stati salvati un oggetto e un messaggio predefiniti, questo determinerà quale messaggio verrà visualizzato per impostazione predefinita nella pagina Nuova versione:

* Se hai informato i tuoi revisori della versione della bozza precedente utilizzando l’e-mail standard (ad esempio, nessun oggetto/messaggio personalizzato), l’oggetto/messaggio personalizzato predefinito (le tue impostazioni personali) verrà visualizzato nella pagina Nuova versione. È quindi possibile modificare l&#39;oggetto e il messaggio personalizzato oppure deselezionare la casella Notify people by email (Notifica alle persone per e-mail), ovvero non verrà inviata alcuna e-mail ai revisori per comunicare loro che dispongono di una nuova versione da rivedere.
* Se non hai notificato ai revisori la versione della bozza precedente (ad esempio, nessuna e-mail standard o personalizzata), la pagina Nuova versione non includerà un messaggio per impostazione predefinita. Per notificare ai revisori la nuova versione, fare clic sul collegamento Invia un messaggio, che consente di visualizzare l&#39;oggetto o il messaggio personalizzato predefinito (in base alle impostazioni personali). Puoi quindi modificare l’oggetto personalizzato e il messaggio, in base alle esigenze.

Se nelle impostazioni personali non vengono salvati un oggetto e un messaggio predefiniti, nella pagina Nuova versione verrà visualizzato quanto segue:

* Se hai informato i tuoi revisori della versione della bozza precedente utilizzando l’e-mail standard (ad esempio, nessun oggetto/messaggio personalizzato), l’opzione Notifica alle persone per e-mail sarà selezionata per impostazione predefinita nella pagina Nuova versione. Per aggiungere un messaggio personalizzato, fai clic sul collegamento.
* Se non hai notificato ai revisori la versione della bozza precedente (ad esempio, nessuna e-mail standard o personalizzata), la pagina Nuova versione non includerà alcun messaggio per impostazione predefinita. Per notificare ai revisori la nuova versione, fare clic sul collegamento Invia un messaggio. È quindi possibile aggiungere un oggetto e un messaggio personalizzati facendo clic sul collegamento Aggiungi messaggio personalizzato.
