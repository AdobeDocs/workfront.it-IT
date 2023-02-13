---
content-type: overview
product-area: documents
keywords: prova,autorizzazione
navigation-topic: proofing-overview
title: Panoramica del profilo di autorizzazione della bozza
description: I profili delle autorizzazioni di prova determinano le autorizzazioni generali degli utenti rispetto a tutte le bozze del tuo account. I profili delle autorizzazioni di prova sono assegnati agli utenti nel loro profilo utente. I profili delle autorizzazioni di prova sono diversi dai ruoli di bozza. Per ulteriori informazioni sui ruoli di bozza, consulta Panoramica sui ruoli di prova .
author: Courtney
feature: Digital Content and Documents
exl-id: fb6faa48-d97b-4b7b-83ae-fe39d40b3963
source-git-commit: 9b60133c4cc20deb410f507854597f44d0607228
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 2%

---

# Panoramica del profilo di autorizzazione della bozza

I profili delle autorizzazioni di prova determinano le autorizzazioni generali degli utenti rispetto a tutte le bozze del tuo account. I profili delle autorizzazioni di prova sono assegnati agli utenti nel loro profilo utente. I profili delle autorizzazioni di prova sono diversi dai ruoli di bozza. Per ulteriori informazioni sui ruoli di bozza, consulta [Panoramica sulla bozza dei ruoli](../../../review-and-approve-work/proofing/proofing-overview/proof-roles.md).

>[!NOTE]
>
>Se sei un amministratore, puoi creare profili personalizzati per gli utenti della tua organizzazione. Per ulteriori informazioni, consulta [Configurare profili personalizzati in Workfront Proof](../../../workfront-proof/wp-acct-admin/account-settings/configure-custom-profiles.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Consider the following about roles and permissions:</p>
-->

<!--
<ul data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li> <p>Assigned profile permissions relate only to the users and items in your own account. The exception is in the case of Satellite accounts, where the Administrator and Billing Administrator for the main (hub) accounts can access and manage the&nbsp;account settings&nbsp;and billing of those accounts from the hub account level.</p> </li>
<li> <p>Billing Administrators and Administrators can delete users. This can only be done in&nbsp;Account settings.</p> </li>
<li>When Billing Administrators and Administrators view proofs that are owned by other users in their account, they view them with the role of a Reviewer.</li>
<li>Using the Read Only role, Billing Administrators and Administrators can access proofs in folders shared with them or in folders created by them.&nbsp;</li>
</ul>
-->

## Profili delle autorizzazioni di prova

Nella tabella seguente sono visualizzate le autorizzazioni disponibili per ogni profilo di autorizzazione della bozza.

<table>
  <tr>
   <td colspan="5" ><strong>Elementi propri</strong>
   </td>
   <td colspan="3" ><strong>Altri elementi utente</strong>
   </td>
   <td><strong>Amministrazione</strong>
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td><strong>Aggiungi</strong>
   </td>
   <td><strong>Visualizza</strong>
   </td>
   <td><strong>Modifica</strong>
   </td>
   <td><strong>Elimina</strong>
   </td>
   <td><strong>Visualizza</strong>
   </td>
   <td><strong>Modifica</strong>
   </td>
   <td><strong>Elimina</strong>
   </td>
   <td><strong>Modifica ed Elimina</strong>
   </td>
  </tr>
  <tr>
   <td>Amministrazione
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
  </tr>
  <tr>
   <td>Supervisore
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>Manager
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>Osservatore
   </td>
   <td>
   </td>
   <td>x
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
</table>

### Amministratore

Gli amministratori hanno accesso a [Impostazioni account](https://support.workfront.com/hc/en-us/sections/115000912147-Account-Settings) e dispongono delle seguenti autorizzazioni:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Gli amministratori possono:</td> 
   <td>Gli amministratori non possono:</td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li> <p>Creazione di bozze, caricamento di file e creazione di cartelle</p> </li> 
     <li> <p>Visualizza, modifica ed elimina le bozze e i file creati</p> </li> 
     <li> <p>Visualizza, modifica ed elimina le bozze e i file creati da tutti gli utenti dell’organizzazione</p> </li> 
     <li> <p>Elimina le cartelle pubbliche di altri utenti</p> </li> 
     <li> <p>Modificare tutte le bozze create nell’account</p> </li> 
     <li> <p>Imposta come proprietario della zona di rilascio*</p> </li> 
     <li> <p>Accedi alla pagina Impostazioni account e modifica i dettagli dell'account</p> </li> 
     <li> <p>Svuotare il cestino</p> </li> 
     <li> <p>Aggiungere, modificare ed eliminare utenti</p> </li> 
     <li> <p>Crea gruppi e aggiungi nuovi contatti</p> </li> 
     <li> <p>Elimina contatti</p> </li> 
     <li> <p>Modifica le bozze se non sono presenti risposte</p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>Modifica le risposte della bozza.</p> </li> 
     <li> <p>Elimina le cartelle private di altri utenti</p> </li> 
     <li> <p>Accedi alla pagina Fatturazione o modifica i dettagli di fatturazione</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Disponibile solo nel prodotto standalone Workfront Proof.

### Supervisore

Le autorità di vigilanza dispongono delle seguenti autorizzazioni:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Le autorità di vigilanza possono:</td> 
   <td>I supervisori non possono:</td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li> <p>Creazione di bozze, caricamento di file e creazione di cartelle</p> </li> 
     <li> <p>Visualizza, modifica ed elimina le bozze e i file creati</p> </li> 
     <li> <p>Visualizza, modifica ed elimina le bozze e i file creati da tutti gli utenti dell’organizzazione</p> </li> 
     <li> <p>Elimina le cartelle pubbliche di altri utenti</p> </li> 
     <li> <p>Modificare tutte le bozze create nell’account</p> </li> 
     <li> <p>Crea gruppi e aggiungi nuovi contatti</p> </li> 
     <li> <p>Elimina contatti</p> </li> 
     <li> <p>Modifica le bozze se non sono presenti risposte</p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>Modifica le risposte della bozza.</p> </li> 
     <li> <p>Elimina le cartelle private di altri utenti</p> </li> 
     <li> <p>Accedi alla pagina Fatturazione o modifica i dettagli di fatturazione</p> </li> 
     <li> <p>Aggiungere, modificare o eliminare utenti</p> </li> 
     <li> <p>Svuotare il cestino</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Manager

I manager dispongono delle seguenti autorizzazioni:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>I manager possono:</td> 
   <td>I manager non possono:</td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li> <p>Creazione di bozze, caricamento di file e creazione di cartelle</p> </li> 
     <li> <p>Visualizza, modifica ed elimina le bozze e i file creati</p> </li> 
     <li> <p>Visualizzare, esaminare e approvare le bozze di altri utenti che sono esplicitamente condivisi con loro (diritti di sola lettura per tutto ciò che si trova in una cartella condivisa)</p> </li> 
     <li> <p>Modificare tutte le bozze create nell’account</p> </li> 
     <li> <p>Crea gruppi e aggiungi nuovi contatti</p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>Visualizza, modifica o elimina le bozze e i file creati da altri utenti dell’organizzazione. </p> <p>Modifica le risposte della bozza.</p> </li> 
     <li> <p>Elimina le cartelle private o pubbliche di altri utenti</p> </li> 
     <li> <p>Accedi alla pagina Fatturazione o modifica i dettagli di fatturazione</p> </li> 
     <li> <p>Aggiungere, modificare o eliminare utenti</p> </li> 
     <li> <p> Elimina contatti</p> </li> 
     <li> <p>Svuotare il cestino</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode">Observer</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Observers have the following permissions:</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/cleaner2.png">Can see, review, and approve proofs of other users that are explicitly shared with them (Read-only&nbsp;rights to everything in a shared folder). For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md" class="MCXref xref">Manage Proof Roles in Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/cleaner2.png">Can view files that are explicitly shared with them.&nbsp;</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot&nbsp;create proofs, upload files, and create folders. For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md" class="MCXref xref">Upload Files and Web Content to Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot view, edit, or delete proofs and files created by other users in the organization.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot edit proofs&nbsp;or replies.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot delete any items created in the organization.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot access&nbsp;the Billing page or Account settings. For more information, see <a href="../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md" class="MCXref xref">The Workfront Proof Billing Page</a>&nbsp;and&nbsp;<a href="../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md" class="MCXref xref">Account settings in Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot be set as the Dropzone owner. For more information, see <a href="../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md" class="MCXref xref">Configure the dropzone in Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot empty the&nbsp;trash. For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md" class="MCXref xref">Restore and Empty the Trash in Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot add, edit, or delete users.&nbsp;</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot create groups or add new contacts.&nbsp;</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot delete contacts.&nbsp;</p>
-->


><!--
><p data-mc-conditions="QuicksilverOrClassic.Draft mode">Menus and functions available to Observers are limited.&nbsp;</p>>
>-->
>  <!--
>  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Observers do not see the Header menu or the green New menu in their Dashboard</li>>
>  -->
>  <!--
>  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Observers do not see the following links in their Settings:&nbsp;Account settings,&nbsp;Billing </li>>
>  -->


<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode">Guest</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Guest profile is used to give access to proofs for reviewers who do not have their own Workfront Proof account. Guests can access proofs shared with them directly via their personal email notifications.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/cleaner2.png">Can view, review, and approve proofs that are explicitly shared with them.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/cleaner2.png">Can view files that are explicitly shared with them.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot access the Dashboard.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot have folders shared with them. For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md" class="MCXref xref">Manage Folders in Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot be added as Authors or Moderators to the proofs. For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md" class="MCXref xref">Manage Proof Roles in Workfront Proof</a>.</p>
-->

<!--
<note type="note">
&nbsp;Guests are not Workfront Proof users, so they cannot see all the proofs shared with them in their own Dashboard.
</note>
-->
