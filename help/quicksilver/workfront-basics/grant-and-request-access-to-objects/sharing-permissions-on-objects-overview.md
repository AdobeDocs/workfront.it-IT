---
content-type: overview
navigation-topic: grant-and-request-access-to-objects
title: Panoramica della condivisione delle autorizzazioni sugli oggetti
description: È possibile condividere o rimuovere le autorizzazioni per un oggetto creato o condiviso con l'utente.
author: Alina
feature: Get Started with Workfront
exl-id: 7c14702e-ac55-4266-88a7-f31618f84218
source-git-commit: c566eb094e96abca6073554433434822c567bc34
workflow-type: tm+mt
source-wordcount: '1167'
ht-degree: 1%

---

# Panoramica della condivisione delle autorizzazioni sugli oggetti

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Redundancy here with the article Permissions for shared objects?</p>
-->

Non è necessario essere un amministratore di Adobe Workfront per condividere le autorizzazioni sugli oggetti a cui si ha accesso, ma le autorizzazioni sugli oggetti funzionano entro i livelli di accesso impostati dall’amministratore di Workfront.

Per ulteriori informazioni sui livelli di accesso e le autorizzazioni, consulta [Funzionamento congiunto dei livelli di accesso e delle autorizzazioni](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

È possibile condividere o rimuovere le autorizzazioni per un oggetto creato o condiviso con l&#39;utente. Se non sei l&#39;autore dell&#39;oggetto, devi disporre dell&#39;accesso Condividi sull&#39;oggetto che desideri condividere nel livello di accesso, oltre alle autorizzazioni Condividi sull&#39;oggetto. Per informazioni sui livelli di accesso, vedi [Panoramica dei livelli di accesso](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

>[!NOTE]
>
>Un amministratore Workfront può aggiungere o rimuovere autorizzazioni per qualsiasi elemento del sistema, per tutti gli utenti, senza esserne il proprietario.

## Oggetti condivisibili in Workfront

In Workfront puoi condividere i seguenti oggetti con altri utenti:

* **Progetti**: Per ulteriori informazioni, consulta [Condivisione di un progetto in Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

* **Modelli**: Per ulteriori informazioni, consulta [Condividere i modelli di progetto](../../manage-work/projects/create-and-manage-templates/share-project-template.md).

* **Portfoli**: Per ulteriori informazioni, consulta [Condividere un portfolio](../../workfront-basics/grant-and-request-access-to-objects/share-a-portfolio..md).

* **Programmi**: Per informazioni, consulta [Condividere un programma](../../workfront-basics/grant-and-request-access-to-objects/share-a-program.md) .

* **Attività**: Per informazioni, consulta [Condividere un’attività](../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md).

* **Problemi**: Per informazioni, consulta [Condividere un problema](../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md).

* **Documenti**: Per informazioni, consulta [Condividere un documento](../../workfront-basics/grant-and-request-access-to-objects/document-permissions.md).

* **Cartelle documenti**: Per informazioni, consulta [Condivisione di una cartella di documenti](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

* **Bozze**: Per informazioni, consulta [Condividi una bozza in Workfront Proof](../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md).

* **Report, dashboard e calendari**: Per informazioni, consulta [Condividere rapporti, dashboard e calendari](../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md). Inoltre, consulta i seguenti articoli:

   * [Condivisione di un rapporto in Adobe Workfront](../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md)
   * [Condivisione di un dashboard](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md)
   * [Condivisione di un rapporto calendario](../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md)

* **Filtri, visualizzazioni e raggruppamenti**: Per informazioni, consulta [Condividere un filtro, una visualizzazione o un raggruppamento](../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).

* **Piani**: Per informazioni, consulta [Condividere un piano in Planner scenario](../../scenario-planner/share-a-plan.md).

   Questo richiede una licenza aggiuntiva.

* **Obiettivi**: Per informazioni, consulta [Condividere un obiettivo in Obiettivi di Workfront](../../workfront-goals/workfront-goals-settings/share-a-goal.md).

   Questo richiede una licenza aggiuntiva.

## Considerazioni sulla condivisione di oggetti

* È possibile condividere solo lo stesso livello o un livello inferiore di autorizzazioni sull&#39;oggetto.

   Ad esempio, se si dispone delle autorizzazioni di Contribute per l&#39;oggetto, non è possibile concedere a un altro utente autorizzazioni di gestione per quell&#39;oggetto.

* Non è possibile condividere un oggetto con un livello di autorizzazione superiore al livello di accesso di un utente. Ad esempio, se un utente dispone dell’accesso Visualizza a progetti nel proprio livello di accesso, non è possibile concedere loro le autorizzazioni Gestione a un progetto.
* Un utente con autorizzazioni per visualizzare almeno un oggetto può condividere tale oggetto con un altro utente.
* È possibile condividere oggetti con utenti attivi, ruoli di lavoro, team, gruppi o aziende.

   >[!NOTE]
   >
   >Puoi condividere un piano o un obiettivo solo con altri utenti attivi. Ciò richiede licenze aggiuntive.
   >
   >
   >Per ulteriori informazioni, consulta:
   >
   >* [Condividere un piano in Planner scenario](../../scenario-planner/share-a-plan.md)
   >* [Condividere un obiettivo in Obiettivi di Workfront](../../workfront-goals/workfront-goals-settings/share-a-goal.md)


## Limiti di condivisione

È possibile condividere un oggetto con un massimo di 100 entità (utenti, team, gruppi, ruoli di lavoro, aziende). È consigliabile condividere gli oggetti con gruppi, team o aziende anziché con singoli utenti, per evitare questa limitazione.

## Condividere le autorizzazioni per gli oggetti

La tabella seguente illustra il livello di autorizzazioni che è possibile selezionare durante la condivisione di un oggetto. Non tutti gli oggetti dispongono di tutte queste impostazioni. È possibile concedere a un&#39;altra entità autorizzazioni per visualizzare o gestire un oggetto. Se condividete un progetto, un&#39;attività o un problema, potete anche concedere le autorizzazioni per Contribute.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Visualizza</td> 
   <td> <p>È possibile eseguire le azioni seguenti sull’oggetto:</p> 
    <ul> 
     <li>Visualizza l’oggetto</li> 
     <li>Aggiungere documenti all’oggetto</li> 
     <li>Visualizza informazioni finanziarie sull'oggetto</li> 
     <li> <p>Condividere l’oggetto<br></p> <p>Quando si condivide l’oggetto, è possibile concedere ad altri utenti lo stesso livello di autorizzazione disponibile solo sull’oggetto, non un livello superiore.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">contribuire</td> 
   <td> <p>È possibile eseguire le azioni seguenti sull’oggetto:</p> 
    <ul> 
     <li>Visualizzare</li> 
     <li>Tutte le azioni incluse nell’autorizzazione Visualizza.</li> 
     <li>Aggiungi spese</li> 
     <li>Aggiungi i problemi (se si tratta di un’attività o di un progetto)</li> 
     <li>Aggiungi attività (se si tratta di un progetto)</li> 
     <li>Modifica Forms personalizzato su di esso</li> 
     <li>Orari di log sull’oggetto</li> 
     <li>Assegna assegnazioni</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Gestisci</td> 
   <td> <p>È possibile eseguire le azioni seguenti sull’oggetto:</p> 
    <ul> 
     <li>Visualizzare</li> 
     <li>Tutte le azioni incluse nelle autorizzazioni Visualizza e Contribute</li> 
     <li>Elimina</li> 
     <li>Gestire le informazioni finanziarie</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Rendi pubblico agli utenti esterni</td> 
   <td> <p>Chiunque non disponga di un account Workfront può visualizzare l’oggetto facendo clic su un collegamento ad esso. Questa funzione non è disponibile per tutti gli oggetti.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Rendi visibile a livello di sistema</td> 
   <td> <p>L’oggetto può essere trovato nelle ricerche e visualizzato da chiunque disponga di un account Workfront.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Comprendere le autorizzazioni ereditate e la gerarchia degli oggetti

* [Autorizzazioni ereditate dagli oggetti principali](#permissions-inherited-from-parent-objects)
* [Autorizzazioni acquisite tramite appartenenze organizzative](#permissions-acquired-through-organizational-memberships) 

### Autorizzazioni ereditate dagli oggetti principali {#permissions-inherited-from-parent-objects}

Le autorizzazioni in Workfront vengono ereditate gerarchicamente. Ciò significa che se si concedono autorizzazioni a un utente su un oggetto principale, per impostazione predefinita ottengono le stesse autorizzazioni sugli oggetti secondari associati ad esso.

Ad esempio, se assegnate a un utente le autorizzazioni Contribute a un progetto, l&#39;utente dispone delle autorizzazioni Contribute per tutte le attività e i problemi (oggetti secondari) associati al progetto.

Continuando con l’esempio precedente, non è possibile limitare le autorizzazioni agli oggetti secondari. Se non si desidera che l&#39;utente disponga delle autorizzazioni di Contribute per gli oggetti secondari associati al progetto, è necessario rimuovere manualmente le Autorizzazioni ereditate dagli oggetti e quindi regolare le autorizzazioni per il singolo utente, incluse le impostazioni avanzate. 

Per ulteriori informazioni sulla gerarchia e l’interdipendenza degli oggetti in Workfront, consulta la sezione [Interdipendenza e gerarchia degli oggetti](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) nell&#39;articolo [Comprendere gli oggetti in Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

>[!NOTE]
>
>L’amministratore Workfront può disattivare le autorizzazioni ereditate per i documenti nel livello di accesso. Per ulteriori informazioni sulla disattivazione delle autorizzazioni ereditate per i documenti a livello di accesso, vedere [Creare o modificare livelli di accesso personalizzati](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

### Autorizzazioni acquisite tramite appartenenze organizzative  {#permissions-acquired-through-organizational-memberships}

Se si concedono le autorizzazioni di gestione a un gruppo di utenti su un oggetto e si concedono le autorizzazioni di visualizzazione a un singolo utente del gruppo sullo stesso oggetto, l&#39;utente dispone del livello più alto di autorizzazioni (Manage) concesse tramite l&#39;appartenenza al gruppo sull&#39;oggetto. 

Se desideri concedere autorizzazioni inferiori a un utente che fa già parte di un’unità organizzativa (Gruppo, Team, Ruolo lavoro o Società) con un livello di autorizzazione superiore, devi rimuovere le autorizzazioni dall’unità organizzativa e aggiungere singolarmente utenti con un livello di autorizzazioni inferiore.

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

Per informazioni sulla condivisione degli oggetti, vedere [Condividere un oggetto](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

## Rimuovere le autorizzazioni dagli oggetti

Per informazioni su come rimuovere le autorizzazioni dagli oggetti, vedere [Rimuovere le autorizzazioni dagli oggetti](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## Richiedere autorizzazioni agli oggetti

Quando un utente invia un collegamento a un oggetto che non dispone delle autorizzazioni di visualizzazione o se si dispone di autorizzazioni inferiori per un oggetto e si desidera richiedere un livello di autorizzazioni superiore, è possibile richiedere le autorizzazioni per l&#39;oggetto. 

È possibile richiedere l’accesso a un oggetto a chiunque disponga dell’autorizzazione Condividi per l’oggetto. 

Per ulteriori informazioni sulla richiesta di autorizzazioni agli oggetti, consulta [Richiedere l’accesso agli oggetti](../../workfront-basics/grant-and-request-access-to-objects/request-access.md).
