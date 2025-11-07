---
title: Condivisione di un modello
product-area: templates
navigation-topic: grant-and-request-access-to-objects
description: In qualità di amministratore di Adobe Workfront, puoi assegnare un livello di accesso agli utenti per autorizzarli a visualizzare o modificare i modelli. Per poter accedere a Modifica modelli, l’utente deve disporre di una licenza per uno dei piani disponibili.
author: Courtney
feature: Get Started with Workfront
exl-id: 19fb0de5-7db5-42a9-9f33-a4570acfeef8
source-git-commit: 883ec4eaa2258de2e464acf14b6b4083db05b99a
workflow-type: tm+mt
source-wordcount: '584'
ht-degree: 15%

---

# Condividere un modello

In qualità di amministratore di Adobe Workfront, puoi assegnare un livello di accesso agli utenti per autorizzarli a visualizzare o modificare i modelli. Per poter accedere a Modifica modelli, l’utente deve disporre di una licenza per uno dei piani disponibili.

Per ulteriori informazioni sulla concessione dell&#39;accesso ai modelli, vedere [Concedere l&#39;accesso ai modelli](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md).

Oltre al livello di accesso concesso, un utente può anche ricevere le autorizzazioni per visualizzare o gestire modelli specifici da altri utenti che li condividono.

>[!NOTE]
>
>I livelli di autorizzazione funzionano all’interno dei livelli di accesso. Ad esempio, un utente non può ricevere le autorizzazioni per gestire un modello, se il suo livello di accesso consente solo di visualizzare i modelli.

Le autorizzazioni sono specifiche per un elemento in Workfront e definiscono quali azioni è possibile eseguire su tale elemento.

## Considerazioni durante la condivisione di un modello

* Oltre alle considerazioni riportate di seguito, vedere anche [Panoramica sulle autorizzazioni di condivisione per gli oggetti](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).
* Per impostazione predefinita, il creatore di un modello e il proprietario del modello dispongono delle autorizzazioni di gestione per il modello. Per informazioni sulla designazione di un utente come proprietario del modello, vedere [Modifica modelli di progetto](../../manage-work/projects/create-and-manage-templates/edit-templates.md).
* Quando condividi un modello, puoi condividere quanto segue:

   * Il modello

     Per ulteriori informazioni su come condividere un modello, vedere [Condividere modelli di progetto](../../manage-work/projects/create-and-manage-templates/share-project-template.md).

     Puoi concedere le seguenti autorizzazioni a un modello:

      * Visualizzazione
      * Gestione

   * I progetti futuri creati utilizzando il modello. Puoi assegnare ai progetti creati da un modello gli stessi livelli di autorizzazione di un singolo progetto. 

     Per informazioni su come condividere un progetto da un modello a livello di modello, vedere [Condividere modelli di progetto](../../manage-work/projects/create-and-manage-templates/share-project-template.md).

* Quando si condivide un modello o un progetto creato dal modello, per impostazione predefinita gli utenti ereditano le stesse autorizzazioni per tutti gli oggetti figlio associati al modello o al progetto.

  Per ulteriori informazioni sulla gerarchia degli oggetti in Workfront, consulta  [Informazioni sugli oggetti in Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

* Quando si condivide un modello, tutte le attività e i documenti modello, nonché i problemi relativi al progetto futuro creato dal modello, ereditano le stesse autorizzazioni, se non diversamente specificato.

  Per informazioni sulla gestione dell&#39;accesso alle attività modello e sui problemi relativi al progetto in base alle autorizzazioni di un utente per il progetto, vedere la sezione [Accesso](../../manage-work/projects/create-and-manage-templates/edit-templates.md#access) nell&#39;articolo [Modifica modelli di progetto](../../manage-work/projects/create-and-manage-templates/edit-templates.md).

* L&#39;amministratore di Workfront può specificare se i documenti devono ereditare le autorizzazioni da oggetti di livello superiore nel livello di accesso dell&#39;utente. Per ulteriori informazioni sulla limitazione delle autorizzazioni ereditate sui documenti, vedere [Creare o modificare livelli di accesso personalizzati](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Non è possibile condividere le attività modello singolarmente. La condivisione di un modello consente di condividere anche le attività del modello. La condivisione del progetto dal modello consente di condividere anche le attività future del progetto.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Share a template</h2>
<p>(NOTE: drafted because this is also linked above: Share project templates >> which is an article in the Manage Work section>> Templates)&nbsp;</p>
<ol>
<li value="1"> <p>Go to the template you want to share with other entities, click <strong>Template Actions</strong>, then <strong>Template Sharing</strong>.<br>Or</p> <p>Navigate to a list of templates, and select multiple templates from the list, then click <strong>Share Template</strong>.</p> <note type="note">
If you select multiple templates, you cannot view who already has permissions to the individual templates.
</note> </li>
<li value="2"> <p>Start typing the name of a user, group, team, job role, or company that you want to share the template with in the <strong>Give template access to</strong> or <strong>Edit template access for</strong> fields.</p> <p>Select them when they appear in the list.</p> <note type="tip">
You can share an object only with active users, teams,
<span>roles,</span> or companies.
</note> </li>
<li value="3">From the drop-down menu, select which level of permissions you want to grant:<br>
<ul>
<li><p><strong>View it</strong>: Users with these permissions are able to view the template and create a project using it, or attach it to an existing project.</p><p><img src="assets/template-permissions-350x197.png" alt="template_permissions.png" style="width: 350;height: 197;"></p></li>
<li><strong>Manage it</strong>: Users with these permissions are able to edit or delete the template.</li>
</ul></li>
<li value="4">(Optional) Click <strong>Advanced Settings</strong> to fine-tune your settings for each level of permissions.</li>
<li value="5">Click <strong>Save</strong>.</li>
</ol>
<h2>Share a project at the template level</h2>
<p>You can share the future projects that are created using a template with users at the template level.</p>
<ol>
<li value="1"> <p>Go to the template whose future projects you want to share with other entities, click <strong>Template Actions</strong>, then <strong>Project Sharing</strong>.</p> <p>Or</p> <p>Navigate to a list of templates, and select multiple templates from the list, then click <strong>Share Project</strong>.</p> <note type="note">
If you select multiple templates, you cannot view who already has project permissions to the individual templates.
</note> </li>
<li value="2"> <p>Start typing and then select the name of a user, group, team, job role, or company with whom you want to share future projects created from the template in the <strong>Give project access to</strong> or <strong>Edit template access for</strong> fields.</p> <note type="tip">
You can share an object only with active users, teams,
<span>roles,</span> or companies.
</note> </li>
<li value="3">From the drop-down menu, select which level of permissions you want to grant.<br>Select from the following:<br>
<ul>
<li><strong>No access</strong>: You can specify which users will not have any access to the template.<br>This option is available only when bulk sharing projects from templates.&nbsp;</li>
<li><strong>View</strong>: Users with these permissions can view projects created from the template.</li>
<li><strong>Contribute</strong>: Users with these permissions can contribute to projects created from the template&nbsp;</li>
<li><strong>Manage</strong>: Users with these permissions can manage or delete projects created from this template.<br><img src="assets/share-project-from-template-350x268.png" alt="share_project_from_template.png" style="width: 350;height: 268;"></li>
</ul></li>
<li value="4">(Optional) Click <strong>Advanced Settings</strong> to fine-tune your settings for each level of permissions. </li>
<li value="5">Click <strong>Save</strong>.</li>
</ol>
</div>
-->

## Impostazioni avanzate per la condivisione dei modelli

Nella tabella seguente vengono visualizzate le autorizzazioni che è possibile concedere agli utenti quando si consente loro di visualizzare o gestire un modello. Per le istruzioni sulla condivisione di un modello, vedere la sezione [Condividere un modello](../../manage-work/projects/create-and-manage-templates/share-project-template.md#share) nell&#39;articolo [Condividere modelli di progetto](../../manage-work/projects/create-and-manage-templates/share-project-template.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Azioni</th> 
   <th>Gestione</th> 
   <th>Visualizzazione</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Copia</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Elimina</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Modifica dettagli modello</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Visualizza Modello</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Condividi</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Condividi a livello di sistema</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Aggiungi documenti</p> <p>Suggerimento: a volte gli utenti aggiungono documenti a un modello di progetto pensando di aggiungerli a un progetto. Disabilitando questa impostazione è possibile evitare che ciò si verifichi per i destinatari.</p> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

Per informazioni sulle autorizzazioni concesse agli utenti per i progetti creati da un modello, vedere [Condividere un progetto in Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).
