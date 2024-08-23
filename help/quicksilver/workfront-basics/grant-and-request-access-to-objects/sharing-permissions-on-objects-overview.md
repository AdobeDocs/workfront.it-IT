---
content-type: overview
navigation-topic: grant-and-request-access-to-objects
title: Panoramica delle autorizzazioni di condivisione sugli oggetti
description: È possibile condividere o rimuovere le autorizzazioni per un oggetto creato o condiviso con l'utente.
author: Alina
feature: Get Started with Workfront
exl-id: 7c14702e-ac55-4266-88a7-f31618f84218
source-git-commit: e1ac95e8be0f6059700ddacb120b08c7c7b683b1
workflow-type: tm+mt
source-wordcount: '1181'
ht-degree: 1%

---

# Panoramica delle autorizzazioni di condivisione sugli oggetti

<!-- Audited: 12/2023 -->

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Redundancy here with the article Permissions for shared objects?</p>
-->
Quando condividi un oggetto con qualcuno nel sistema, puoi concedere al destinatario una delle seguenti autorizzazioni: visualizza, contribuisce e gestisci.

Non è necessario essere amministratori di Adobe Workfront per condividere le autorizzazioni sugli oggetti a cui hai accesso, ma le autorizzazioni sugli oggetti funzionano all’interno dei livelli di accesso impostati dall’amministratore di Workfront.

È possibile condividere o rimuovere le autorizzazioni per un oggetto creato o condiviso con l&#39;utente. Se non si è il creatore dell&#39;oggetto, è necessario disporre dell&#39;accesso Condivisione sull&#39;oggetto che si desidera condividere nel proprio livello di accesso oltre alle autorizzazioni Condivisione sull&#39;oggetto. Per informazioni sui livelli di accesso, vedere [Panoramica sui nuovi livelli di accesso](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md) o [Panoramica sui livelli di accesso](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

>[!NOTE]
>
>Un amministratore di Workfront può aggiungere o rimuovere autorizzazioni per qualsiasi elemento del sistema, per tutti gli utenti, senza esserne il proprietario.

## Oggetti che puoi condividere in Workfront

In Workfront è possibile condividere i seguenti oggetti con altri utenti:

* **Progetti**: per ulteriori informazioni, vedere [Condividere un progetto in Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

* **Modelli**: per ulteriori informazioni, vedere [Condividere modelli di progetto](../../manage-work/projects/create-and-manage-templates/share-project-template.md).

* **Portfoli**: per ulteriori informazioni, vedere [Condividere un portfolio](../../workfront-basics/grant-and-request-access-to-objects/share-a-portfolio.md).

* **Programmi**: per informazioni, vedere [Condividere un programma](../../workfront-basics/grant-and-request-access-to-objects/share-a-program.md).

* **Attività**: per informazioni, vedere [Condividere un&#39;attività](../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md).

* **Problemi**: per informazioni, vedere [Condividere un problema](../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md).

* **Documenti**: per informazioni, vedere [Condividi documento](../../workfront-basics/grant-and-request-access-to-objects/document-permissions.md).

* **Cartelle documenti**: per informazioni, vedere [Condividere una cartella documenti](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

* **Bozze**: per informazioni, vedere [Condividi bozza in Workfront](/help/quicksilver/review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

* **Report, dashboard e calendari**: per informazioni, vedere [Condividere report, dashboard e calendari](../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md). Inoltre, vedi i seguenti articoli:

   * [Condividere un rapporto in Adobe Workfront](../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md)
   * [Condividere un dashboard](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md)
   * [Condivisione di un report calendario](../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md)

* **Filtri, visualizzazioni e raggruppamenti**: per informazioni, vedere [Condividere un filtro, una visualizzazione o un raggruppamento](../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).

* **Piani**: per informazioni, vedere [Condividere un piano nella Pianificazione scenario](../../scenario-planner/share-a-plan.md).

  È necessaria una licenza aggiuntiva.

* **Obiettivi**: per informazioni, vedere [Condividere un obiettivo in Obiettivi Workfront](../../workfront-goals/workfront-goals-settings/share-a-goal.md).

  È necessaria una licenza aggiuntiva.

## Considerazioni sulla condivisione degli oggetti

* Puoi condividere solo lo stesso livello o un livello inferiore di autorizzazioni disponibili per l’oggetto.

  Se ad esempio si dispone delle autorizzazioni Contribute per l&#39;oggetto, non è possibile concedere a un altro utente le autorizzazioni Manage per tale oggetto.

* Impossibile condividere un oggetto con un livello di autorizzazione superiore al livello di accesso di un utente.

  Ad esempio, se un utente ha accesso in visualizzazione ai progetti nel suo livello di accesso, non puoi assegnare loro le autorizzazioni di gestione per un progetto.
* Un utente che dispone almeno delle autorizzazioni per visualizzare un oggetto può condividerlo con un altro utente.
* Puoi condividere oggetti con utenti attivi, mansioni, team, gruppi o aziende.

  >[!NOTE]
  >
  >Puoi condividere un piano o un obiettivo solo con altri utenti attivi. A tal fine sono necessarie licenze aggiuntive.
  >
  >
  >Per ulteriori informazioni, consulta:
  >
  >* [Condivisione di un piano nella Pianificazione scenario](../../scenario-planner/share-a-plan.md)
  >* [Condividi un obiettivo negli Obiettivi di Workfront](../../workfront-goals/workfront-goals-settings/share-a-goal.md)

## Limiti di condivisione

Puoi condividere un oggetto con un massimo di 100 entità (utenti, team, gruppi, mansioni, aziende). Per evitare questo limite, è consigliabile condividere gli oggetti con gruppi, team o aziende anziché con i singoli utenti.

## Autorizzazioni di condivisione per gli oggetti

Nella tabella seguente viene illustrato il livello di autorizzazioni che è possibile selezionare quando si condivide un oggetto. Non tutti gli oggetti dispongono di tutte queste impostazioni. È possibile concedere a un&#39;altra entità le autorizzazioni per visualizzare o gestire un oggetto. Se condividi un progetto, un’attività o un problema, puoi anche concedere autorizzazioni a Contribute.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Visualizza</strong></td> 
   <td> <p>È possibile eseguire le azioni seguenti sull'oggetto:</p> 
    <ul> 
     <li><p>Visualizza l'oggetto</p></li> 
     <li><p>Aggiungere documenti all'oggetto</p></li> 
     <li><p>Visualizza informazioni finanziarie sull'oggetto</p></li> 
     <li> <p>Condividere l’oggetto<br></p> <p>Quando si condivide l'oggetto, è possibile concedere ad altri utenti lo stesso livello di autorizzazione disponibile solo per l'oggetto e non per un livello superiore.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Contribuisci</strong></td> 
   <td> <p>È possibile eseguire le azioni seguenti sull'oggetto:</p> 
    <ul> 
     <li>Tutte le azioni incluse nell’autorizzazione Visualizzazione.</li> 
     <li>Aggiungi spese</li> 
     <li>Aggiungi problemi (se si tratta di un'attività o di un progetto)</li> 
     <li>Aggiungi attività (se si tratta di un progetto)</li> 
     <li>Modifica Forms personalizzato</li> 
     <li>Registra le ore sull'oggetto</li> 
     <li>Effettua assegnazioni</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Gestire</strong></td> 
   <td> <p>È possibile eseguire le azioni seguenti sull'oggetto:</p> 
    <ul> 
     <li>Tutte le azioni incluse nelle autorizzazioni Visualizza e Contribute</li> 
     <li>Elimina</li> 
     <li>Gestire le informazioni finanziarie</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Rendi pubblico agli utenti esterni</strong></td> 
   <td> <p>Chiunque non disponga di un account Workfront può visualizzare l’oggetto facendo clic su un collegamento ad esso. Non disponibile per tutti gli oggetti.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Rendi visibile a livello di sistema</strong></td> 
   <td> <p>L’oggetto si trova nelle ricerche e viene visualizzato dagli utenti con un account Workfront.</p><p><b>Nota</b>: gli utenti con licenze Collaboratore o Richiedente non possono visualizzare i progetti, anche se questa impostazione è abilitata. </td> 
  </tr> 
 </tbody> 
</table>

## Comprendere le autorizzazioni ereditate e la gerarchia di oggetti

### Autorizzazioni ereditate dagli oggetti padre {#permissions-inherited-from-parent-objects}

Le autorizzazioni in Workfront vengono ereditate gerarchicamente. Ciò significa che se si concedono le autorizzazioni a un utente su un oggetto padre, per impostazione predefinita queste ottengono le stesse autorizzazioni sugli oggetti figlio a esso associati.

Se ad esempio si assegnano a un utente le autorizzazioni Contribute per un progetto, l&#39;utente disporrà delle autorizzazioni Contribute per tutte le attività e i problemi (oggetti figlio) associati a tale progetto.

Continuando con l&#39;esempio precedente, non è possibile limitare le autorizzazioni agli oggetti figlio. Se non si desidera che l&#39;utente disponga delle autorizzazioni di Contribute per gli oggetti figlio associati al progetto, è necessario rimuovere manualmente le autorizzazioni ereditate dagli oggetti e quindi modificare le autorizzazioni per il singolo utente, incluse eventuali impostazioni avanzate. 

Per ulteriori informazioni sulla gerarchia e l&#39;interdipendenza degli oggetti in Workfront, vedere la sezione [Interdipendenza e gerarchia degli oggetti](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#interdependency-and-hierarchy-of-objects) nell&#39;articolo [Panoramica sugli oggetti di Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

>[!NOTE]
>
>L&#39;amministratore di Workfront può disabilitare le autorizzazioni ereditate per i documenti nel proprio livello di accesso. Per ulteriori informazioni sulla disattivazione delle autorizzazioni ereditate per i documenti nel livello di accesso, vedere [Creare o modificare livelli di accesso personalizzati](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

### Autorizzazioni acquisite tramite appartenenze a organizzazioni  {#permissions-acquired-through-organizational-memberships}

Se si concedono le autorizzazioni di gestione a un gruppo di utenti su un oggetto e si concedono le autorizzazioni di visualizzazione a un singolo utente di tale gruppo sullo stesso oggetto, l&#39;utente disporrà del livello più alto di autorizzazioni (Gestisci) concesso tramite l&#39;appartenenza al gruppo sull&#39;oggetto. 

Se desideri concedere autorizzazioni inferiori a un utente che fa già parte di un’unità organizzativa (Gruppo, Team, Mansione o Società) con un livello di autorizzazione più alto, devi rimuovere le autorizzazioni dall’unità organizzativa e aggiungere gli utenti singolarmente con un livello di autorizzazione più basso.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Remove permissions from objects</h2>
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">AL: draft/ hide this div when Becky makes Remove permissions from objects live and replace with the drafted content with the link at the top of this section</p>
<p>You can remove permissions from objects you have access to Share. Removing permissions from objects is identical for all objects that can be shared.&nbsp;</p> <note type="note">
&nbsp;You cannot remove permissions when you share items in bulk. You can remove permissions only when selecting individual items.&nbsp;
</note>
<p>To remove permissions from objects consider the following:&nbsp;</p>
<ul>
<li><a href="#remove-entities-from-the-sharing-list-of-an-object" class="MCXref xref">Remove entities from the sharing list of an object</a> </li>
<li><a href="#remove-inherited-permissions" class="MCXref xref">Remove inherited permissions</a> </li>
<li><a href="#make-an-object-private" class="MCXref xref">Make an object private</a> </li>
</ul>
<p><strong>Remove entities from the sharing list of an object</strong></p>
<p>You can remove entities from the sharing list of an object to remove their permissions from the object.</p>
<p>To remove permissions from objects:&nbsp;</p>
<ol>
<li value="1">Navigate to an object on which you want to modify the permissions.</li>
<li value="2">Click the <strong>Actions</strong> menu, then click <strong>Sharing</strong>.<br>For example, on a project, click <strong>Project Actions</strong>, then <strong>Sharing</strong>.&nbsp;</li>
<li value="3">Click the <strong>x</strong> next to the name of a user, team, group, company, job role to remove them.<br></li>
<li value="4">In the <strong><User Name>'s Workfront access will be removed from this</strong> drop-down menu, select whether you want their access to be removed just from the object you have selected, or from all children objects associated with it.<br>The following scenarios exist:
<ul>
<li>If you remove the entity only from the object, that entity loses their permissions on the object, and their inherited permissions to the children objects. If they are granted permissions to the children items individually, they retain the same permissions on all children objects associated with it when you select this option.&nbsp;</li>
<li>If you remove the entity from the object and all the children objects, that entity loses their permissions to the object as well as all children objects, even when they have been given individual permission on each child object.&nbsp;</li>
</ul></li>
<li value="5">Click <strong>Save</strong>.</li>
</ol>
<p> <p><strong>Remove inherited permissions</strong></p> </p>
<p>Inherited permissions can be removed from objects allowing for owners to specifically&nbsp;identify who will get access to children objects regardless of the access of a user to a parent object. Only users with Manage permission are able to remove inherited permissions.</p>
<p>To remove inherited permissions:</p>
<ol>
<li value="1">Navigate to an object to which you have Manage permissions. <br>For example, navigate to a task.</li>
<li value="2">Go to the sharing list as described in the <a href="#Share" class="MCXref xref">Overview of sharing permissions on objects</a> section in this article. </li>
<li value="3">Select the <strong>X</strong>&nbsp;mark next to <strong>Inherited Permission</strong>&nbsp;on the sharing box to remove&nbsp;anyone listed there.<br><br>This ensures that no one who is granted permissions to the parent object (for example, the project) has permissions to this task by default. You must list&nbsp; individual entities in the sharing list of the task to grant permissions on the task.<br><note type="note">
You cannot remove individual entities from the Inherited Permissions list. You can only disable the Inherited Permissions for all entities listed.
</note></li>
<li value="4">Click <strong>Save</strong>.&nbsp;</li>
</ol>
<p><strong>Make an object private</strong></p>
<p>If you have shared an object system-wide, or you have shared it with external uses by making it public, you can make it private again by removing the system-wide or public permissions.&nbsp;</p>
<p>For more information about making an object available system-wide, or publicly, see the section <a href="#Share" class="MCXref xref">Overview of sharing permissions on objects</a> in this article.</p>
<p>To make an object private:</p>
<ol>
<li value="1">Go to the object you want to make private.<br>For example, navigate to a report.</li>
<li value="2">Click <strong>Report Actions</strong>, then <strong>Sharing</strong>.<br><br></li>
<li value="3">Click <strong>Remove public access</strong> to remove the access of external users to viewing the report.</li>
<li value="4">Click <strong>Remove system-wide access</strong> to stop sharing it with all Workfront users.&nbsp;</li>
<li value="5">Click <strong>Save</strong>.</li>
</ol>
</div>
-->

## Condividere un oggetto

Per informazioni su come condividere gli oggetti, vedere [Condividere un oggetto](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

## Rimuovere le autorizzazioni dagli oggetti

Per informazioni su come rimuovere le autorizzazioni dagli oggetti, vedere [Rimuovere le autorizzazioni dagli oggetti](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## Richiedi autorizzazioni per gli oggetti

Quando qualcuno ti invia un collegamento a un oggetto per il quale non disponi di autorizzazioni di visualizzazione, o quando disponi di autorizzazioni inferiori per un oggetto e desideri richiedere un livello di autorizzazioni superiore, puoi richiedere le autorizzazioni per l’oggetto. 

È possibile richiedere l&#39;accesso a un oggetto a chiunque disponga dell&#39;autorizzazione di condivisione per l&#39;oggetto. 

Per ulteriori informazioni sulla richiesta di autorizzazioni agli oggetti, vedere [Richiedere l&#39;accesso agli oggetti](../../workfront-basics/grant-and-request-access-to-objects/request-access.md).
