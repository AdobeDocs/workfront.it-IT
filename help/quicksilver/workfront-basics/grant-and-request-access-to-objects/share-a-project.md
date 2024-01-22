---
title: Condividere un progetto in Adobe Workfront
product-area: projects
navigation-topic: grant-and-request-access-to-objects
description: Il tuo amministratore Adobe Workfront può concederti l’accesso per visualizzare o modificare progetti durante l’assegnazione del livello di accesso. Per ulteriori informazioni, consulta Concedere l’accesso ai progetti.
author: Alina
feature: Get Started with Workfront
exl-id: eaeedff8-9114-40d9-8cd4-56996edc7dad
source-git-commit: 71d5e15c38b26b9a833ac2418d5782afd249a24c
workflow-type: tm+mt
source-wordcount: '986'
ht-degree: 2%

---

# Condividere un progetto in Adobe Workfront

<!-- Audited: 1/2024 -->

Il tuo amministratore Adobe Workfront può concederti l’accesso per visualizzare o modificare progetti durante l’assegnazione del livello di accesso. Per ulteriori informazioni, consulta [Concedere l’accesso ai progetti](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

Oltre al livello di accesso concesso agli utenti, è possibile concedere loro le autorizzazioni per visualizzare, contribuire o gestire progetti specifici a cui si ha accesso per la condivisione.

Le autorizzazioni sono specifiche per un elemento in Workfront e definiscono quali azioni è possibile eseguire su tale elemento.

## Considerazioni sulla condivisione di progetti

Oltre alle considerazioni riportate di seguito, vedere anche [Panoramica delle autorizzazioni di condivisione sugli oggetti](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

* Per impostazione predefinita, il creatore di un progetto dispone delle autorizzazioni per gestire il progetto ed è anche designato come proprietario del progetto. Se il progetto è assegnato a un altro proprietario, anche tale utente dispone delle autorizzazioni necessarie per gestire il progetto. Quando il creatore del progetto (o il proprietario) condivide il progetto con altri utenti, concede a questi ultimi determinate autorizzazioni per controllare ciò che possono fare mentre lavorano sul progetto.

  Tuttavia, se un proprietario del progetto non dispone di una licenza Planner, non ha accesso completo alla gestione del progetto. Solo un utente con una licenza Pianificazione può disporre delle autorizzazioni per gestire un progetto. Per ulteriori informazioni, consulta [Funzionamento congiunto dei livelli di accesso e delle autorizzazioni](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

* Puoi condividere i progetti singolarmente, oppure puoi condividerne più di uno alla volta. La condivisione di progetti è identica alla condivisione di altri oggetti. Per ulteriori informazioni sulla condivisione di elementi in Workfront, vedi [Condividere un oggetto](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).
* Puoi concedere le seguenti autorizzazioni a un progetto:

   * Visualizza
   * Gestisci
   * Contribuisci

     ![](assets/view-on-projects-190x207.png) ![](assets/contribute-on-projects-159x243.png) ![](assets/manage-on-projects-178x230.png)

* Quando si condivide un progetto, tutte le attività, i problemi e i documenti ereditano le stesse autorizzazioni, se non diversamente specificato.

  Per informazioni sulla gestione dell’accesso alle attività e ai problemi del progetto in base alle autorizzazioni di un utente, consulta [](../../manage-work/projects/manage-projects/edit-projects.md#access) sezione nell’articolo [Modifica progetti](../../manage-work/projects/manage-projects/edit-projects.md).

  L&#39;amministratore di Workfront può specificare se i documenti devono ereditare le autorizzazioni da oggetti di livello superiore nel livello di accesso dell&#39;utente. Per ulteriori informazioni sulla limitazione delle autorizzazioni ereditate sui documenti, vedere [Creare o modificare livelli di accesso personalizzati](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* È possibile rimuovere le autorizzazioni ereditate da un progetto in modo che gli oggetti figlio non le ereditino. Per ulteriori informazioni sulla rimozione delle autorizzazioni ereditate dagli oggetti, vedere [Rimuovere le autorizzazioni dagli oggetti](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## Modi per condividere un progetto {#ways-to-share-a-project}

Puoi condividere un progetto nei seguenti modi:

* Manualmente, effettuando una delle seguenti operazioni:

   * Aggiunta di utenti al team del progetto. Quando aggiungi utenti al team di progetto, questi ottengono automaticamente le autorizzazioni di visualizzazione per il progetto.\
     Per ulteriori informazioni sull&#39;aggiunta di utenti a un team di progetto, vedere la sezione &quot;Aggiunta di utenti a un team di progetto&quot; in [Panoramica del team del progetto](../../manage-work/projects/planning-a-project/project-team-overview.md).
   * Condivisione individuale o in blocco dei progetti quando si utilizza **Condivisione** opzione.

     La condivisione di un progetto è simile alla condivisione di tutti gli altri oggetti in Adobe Workfront.

     Per informazioni sulla condivisione di oggetti in Workfront, consulta [Condividere un oggetto](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

* Automaticamente, effettuando una delle seguenti operazioni:

   * Posizionare un progetto in un **Portfolio** o **Programma** che è già condiviso con altri. Gli utenti ottengono le stesse autorizzazioni al progetto di cui dispongono per il portfolio o il programma.\
     Per informazioni sull’aggiunta di un progetto a un **Portfolio**, vedi [Aggiungere progetti a un portfolio](../../manage-work/portfolios/create-and-manage-portfolios/add-projects-to-portfolios.md).\
     Per informazioni sull’aggiunta di un progetto a un **Programma**, vedi [Aggiungere un progetto a un programma](../../manage-work/portfolios/create-and-manage-programs/add-project-to-program.md).

     Per informazioni sulla visualizzazione delle autorizzazioni ereditate su un oggetto, vedi [Visualizzare le autorizzazioni ereditate sugli oggetti](../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).

   * Aggiungere entità alla condivisione di progetti in un modello utilizzato per creare il progetto. Per informazioni sulla condivisione di progetti da modelli, consulta [Condividere un modello](../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).
   * Definire il modello di accesso al progetto.

     Per definire il modello di accesso al progetto, vedi [Condividere un oggetto](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

     >[!TIP]
     >
     >Quando si allega o si salva un modello, è possibile cancellare le regole di condivisione dei progetti dei modelli.

   * Modificare un progetto e definire **Quando a un utente viene dato l’accesso a questo progetto** impostazione. Per ulteriori informazioni, consulta [Modifica progetti](../../manage-work/projects/manage-projects/edit-projects.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: drafted because I created new article and linked it above) </p>
<p>To view what users have inherited the access on the project from a portfolio or a program, do the following:</p>
<ol style="list-style-type: lower-alpha;">
<li value="1">Go to a project whose sharing permissions you want to view. </li>
<li value="2"> Click the <strong>More</strong> menu <img src="assets/more-icon.png">, then click <strong>Sharing</strong>. </li>
<li value="3"> <p>Expand the <strong>Inherited Permissions</strong> list. </p> <p>This list displays the names of users that have access to either the portfolio or the program that the project belongs to and also have permissions to the project. </p>  </li>
</ol>
</div>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Go to a project whose sharing permissions you want for all projects you create from scratch. (NOTE: drafted because linked above)&nbsp;</li>
<li value="2"> Click the More menu, then click <strong>Sharing</strong>. </li>
<li value="3"> <p>In the Project Access box that displays, near the upper-right corner, click the gear icon <img src="assets/gear-icon-settings.png">, then click <strong>Set as my project access template</strong>.</p> <p>The entities that are granted permissions on the selected project have the same permissions for all the projects you create from scratch in the future.</p> <p> The project access template overrides the sharing defaults granted to you by the Workfront administrator in your Access Level.<br>For more information about specifying sharing defaults for projects in the Access Level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>.</p> </li>
<li value="4">Click <strong>Save</strong>.</li>
</ol>
-->

## Limitazioni per i diversi tipi di licenza

* Gli utenti con una licenza Worker non dispongono delle autorizzazioni necessarie per gestire i progetti. Per i lavoratori, l&#39;autorizzazione di condivisione più elevata è Contribute.
* Gli utenti con una licenza Request possono visualizzare le informazioni sul progetto, ma hanno accesso limitato al progetto.
* Un&#39;eccezione alla modifica dello stato di un progetto si verifica quando un utente con autorizzazioni Visualizza o Contribuisci è incluso anche in un processo di approvazione. Possono approvare il progetto, che modifica lo stato del progetto, ma lo stato è quello predefinito per l’approvazione o per il rifiuto.
* Per poter copiare un progetto, un utente deve anche avere accesso alla creazione di progetti nel proprio Livello di Accesso.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Configure default permissions for a project</h2>
<p>(NOTE: drafted because I added one more way to automatically share the project above in the bullet list and linked it to Edit Projects) </p>
<p>As a project owner, you can configure the default permissions for View, Manage, and Contribute access that are used when sharing&nbsp;the project with others. When users share a project, the default permissions are used. Users can then adjust the default permissions when sharing the project, as described in <a title="Project Permissions" href="#ways-to-share-a-project" class="MCXref xref">Ways to share a project</a>. </p>
<p>To configure the default permissions that are included with each access level:</p>
<ol>
<li value="1">Go to the project where you want to set the default permissions.</li>
<li value="2"> <p>Click the More menu <img src="assets/more-icon.png">, then click <strong>Edit</strong>. <img src="assets/edit-icon.png"></p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="3">Click <strong>Access</strong> in the list on the left.</li>
<li value="4"> <p>In the <strong>When someone is given access to this PROJECT</strong> section, select permissions that you want to be available when users are given access to the project via sharing.</p> <p>Ensure that any permissions that you want to include in the selected access level are selected and deselect any permissions that you do not want to include in the selected permissions level.</p> <p>To view which permissions are available for each level, see&nbsp;<a title="Project Permissions" href="#Understanding_Project_Permissions" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <note type="note">
The
<strong>Delete</strong> access in the
<strong>Manage</strong> permission level determines whether users can&nbsp;delete the project itself. Users with
<strong>Manage</strong> access to the project can delete tasks and issues within the project regardless of whether this option is selected, if they have
<strong>Manage</strong> permissions to the tasks and issues.&nbsp;
</note> </li>
<li value="5">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->

## Opzioni di autorizzazione del progetto

Nella tabella seguente sono elencate le autorizzazioni che gli utenti possono concedere quando condividono un progetto. Per ulteriori informazioni sugli utenti dell’accesso ottenuti in base alla propria licenza, consulta [Concedere l’accesso ai progetti](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Azioni</strong> </p> </th> 
   <th> <p><strong>Gestisci</strong> </p> </th> 
   <th> <p><strong>Contribuisci</strong> </p> </th> 
   <th> <p><strong>Visualizza</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Aggiungi modulo personalizzato</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aggiorna campi personalizzati</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aggiungere Un Processo Di Approvazione</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Approvare un progetto</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Approva ore</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓ </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Crea Un Progetto</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aggiungi documenti</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aggiungi problemi</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aggiungi attività</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Copia Progetto</p> </td> 
   <td> <p> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Cancella Progetto</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Modifica date pianificate</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Condividi progetto</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Condividi a livello di sistema</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Visualizza Progetto</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aggiornamenti/commenti</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Modifica stato</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Registra ore</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Modifica assegnazioni</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Gestisci Base Line</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Gestione dei rischi*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Gestisci dati finanziari*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aggiungi/Modifica spese*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Finanza*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Allega Modello</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Salva come modello</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aggiungi/Modifica Business Case</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Modifica dettagli progetto</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Modifica assegnazione personale</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Esporta in MS Project</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Ricalcola finanza/sequenza temporale*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Imposta proprietà coda</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Modificare un progetto in blocco in un elenco</p> </td> 
   <td> <p>✓</p> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Gli utenti che non hanno accesso ai dati finanziari non possono gestire i rischi e i finanziamenti per i progetti, anche se hanno accesso in modifica ai progetti. Per informazioni sull&#39;accesso ai dati finanziari, vedere [Concedere l’accesso ai dati finanziari](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
