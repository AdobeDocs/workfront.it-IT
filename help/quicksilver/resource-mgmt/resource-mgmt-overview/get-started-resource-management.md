---
content-type: overview
product-area: resource-management
navigation-topic: resource-management-overview
title: Introduzione alla gestione delle risorse
description: Gestione risorse consente di configurare il sistema per prevedere con precisione l'utilizzo delle risorse in base alla disponibilità, in modo che il lavoro da eseguire venga completato in tempo e nel preventivo.
author: Alina
feature: Resource Management
exl-id: b10ef503-60ea-4450-b63e-b2918e9bcc11
source-git-commit: ca4da5302198d8fffc8b706baa3b3aeaa1f738e3
workflow-type: tm+mt
source-wordcount: '1171'
ht-degree: 0%

---

# Introduzione alla gestione delle risorse

<!-- Audited: 12/2023 -->

<!--
<p>(NOTE: DO NOT DELETE THIS ARTICLE. MANY ARTICLES MENTIONING RES MANAGEMENT ARE AND STILL SHOULD / WILL BE LINKED TO IT.) </p>
<p>(NOTE: Alina: ***As functionality is removed from Legacy and added to Res Planning - this will be continually updated: remove the Legacy Res Planning when that functionality is removed from the system.) </p>
</div>
-->

Gestione risorse consente di configurare il sistema per prevedere con precisione l&#39;utilizzo delle risorse in base alla disponibilità, in modo che il lavoro da eseguire venga completato in tempo e nel preventivo.

## Panoramica sulla gestione delle risorse in Adobe Workfront

Gestione risorse si riferisce a tutte le attività eseguite dall&#39;amministratore di Adobe Workfront, dal responsabile delle risorse e dal proprietario del progetto per pianificare (Pianificazione risorse o Scenario) e programmare (Bilanciatore dei carichi di lavoro) le risorse di un&#39;organizzazione e assegnarle al lavoro da eseguire, tenendo conto della loro disponibilità. Inoltre, la gestione delle risorse si riferisce anche alla visualizzazione delle informazioni sulle allocazioni di risorse pianificate ed effettive in una visualizzazione rapporto (rapporto Utilizzo).

Workfront dispone di diversi set di strumenti utilizzati per gestire le risorse. Ogni strumento ha un ambito individuale. Attualmente, puoi utilizzare i seguenti strumenti di gestione delle risorse in Workfront, a seconda della fase di gestione delle risorse in cui ti trovi:

* Per pianificare il modo in cui le risorse vengono allocate a un livello superiore, prima dell&#39;inizio del lavoro effettivo sui progetti, utilizzare i seguenti strumenti:

   * **Pianificazione risorse**: è possibile utilizzare la Pianificazione risorse nella prima fase della gestione delle risorse per calcolare il tempo del progetto per le risorse in base alla disponibilità programmata. Durante la fase di pianificazione delle risorse, è possibile organizzare gli utenti in pool di risorse e assegnare più pool di risorse a un progetto.

     Per ulteriori informazioni sulla pianificazione delle risorse, vedere [Pianificazione delle risorse in Adobe Workfront](../../resource-mgmt/resource-planning/resource-planning-overview.md).

   * **Pianificazione scenario**: si tratta di una pianificazione di livello superiore delle risorse che consente di gestirle in più iniziative che possono estendersi su un piano di uno, tre o cinque anni e includere più progetti. È possibile utilizzare lo scenario migliore per sfruttare al massimo la disponibilità e il budget.

     La Pianificazione scenario richiede una licenza separata, oltre alla licenza Workfront. Per informazioni su Workfront Scenario Planner, consulta [Panoramica sulla pianificazione degli scenari](../../scenario-planner/scenario-planner-overview.md).

     <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: when more functionality is added, maybe we add that we recommend to start here if this is available for them?!) </p>   
     -->

* Per programmare o assegnare risorse al lavoro effettivo (attività e problemi), utilizzare lo strumento seguente:

   * **Il Bilanciatore dei carichi di lavoro**: appartiene a una fase di livello inferiore della gestione delle risorse, in cui è possibile assegnare le risorse al lavoro effettivo (attività e problemi) che devono completare, in base alla quantità di ore necessarie per completarle e alla loro disponibilità. Utilizzando il Bilanciatore dei carichi di lavoro è possibile assegnare gli utenti al lavoro effettivo attualmente non assegnato o assegnato a mansioni.

     Per informazioni sul Bilanciatore di Workfront, consulta [L’indice del Bilanciatore dei carichi di lavoro: articolo](../../resource-mgmt/workload-balancer/workload-balancer.md).

<!--

  * **Scheduling** (deprecated <span class="preview">and removed from the Preview environment</span>): Refers to assigning actual work to users by matching the job roles assigned to the tasks and issues with the job roles they can fulfill, or assigning actual work to users on tasks and issues which are currently unassigned. This happens at a lower-level in the process of managing resources, where you can assign your resources to the actual work (tasks and issues) that they must fulfill, according to the hours needed in the project plan to fulfill them.  

     For more information about resource scheduling, see the section [Resource Scheduling](../../resource-mgmt/resource-scheduling/resource-scheduling-overview.md).

    >[!CAUTION]
    >
    >
    >We are no longer supporting the Resource Scheduling tools and they will be removed from Workfront in **January 2023**. We recommend that you use the Workload Balancer for scheduling your resources. 
    >
    >
    >* For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).
    >
    >
    >* For more information about the timeline for removing the Resource Scheduling tools and replacing them with the Workload Balancer, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).

-->
* Per analizzare le allocazioni preventivate, pianificate ed effettive per più progetti, utilizzare lo strumento seguente:

   * **Rapporto utilizzo**: utilizza questo rapporto per visualizzare l’utilizzo delle risorse per i progetti. È possibile confrontare le allocazioni preventivate, pianificate ed effettive per i progetti e il relativo impatto sui costi e sui ricavi dei progetti.

     Per informazioni sul rapporto Utilizzo, vedere [Visualizza informazioni sull&#39;utilizzo delle risorse](../../resource-mgmt/resource-utilization/view-utilization-information.md).

## Componenti del processo Gestione risorse

>[!NOTE]
>
>La gestione delle risorse non è mai un processo stagnante in Workfront. Man mano che cambiano le pianificazioni dei progetti, la disponibilità degli utenti o i loro ruoli, è necessario modificare continuamente le informazioni relative alle risorse, alle assegnazioni e alle assegnazioni a progetti, attività e problemi.

Il processo di gestione delle risorse in Workfront prevede le seguenti fasi:

* **Configurazione**: in qualità di amministratore di sistema, manager delle risorse o proprietario del progetto, è necessario configurare alcuni campi e oggetti nell’istanza di Workfront prima di gestire le risorse. Per ulteriori informazioni sui prerequisiti necessari per iniziare a gestire le risorse in Workfront, vedi [Prerequisiti per una gestione accurata delle risorse](#prerequisites-for-accurate-resource-management) in questo articolo.\
  Oltre a disporre di progetti con elementi di lavoro, è necessario configurare i seguenti elementi in Workfront:

   * Utenti\
     Per ulteriori informazioni sulla creazione di utenti, consulta l’articolo [Aggiungi utenti](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

   * Ruoli\
     Per ulteriori informazioni sulla creazione di ruoli, consulta l’articolo [Creare e gestire le mansioni](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

   * Schedule\
     Per ulteriori informazioni sulla creazione di pianificazioni, vedere l&#39;articolo [Creare una pianificazione](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

   * Preferenze progetto

     >[!TIP]
     >
     >Solo un amministratore di sistema o di gruppo può modificare le preferenze di progetto per il sistema o per il gruppo.

     Per ulteriori informazioni sulla definizione delle preferenze di progetto, consulta l’articolo [Configurare le preferenze di progetto a livello di sistema](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   * Gruppi di risorse

     Per ulteriori informazioni sulla creazione di pool di risorse, consulta [Creare i pool di risorse](../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

   * Preferenze di Gestione risorse

     In qualità di sistema, è necessario decidere in che modo Workfront calcola la disponibilità dell&#39;utente a livello di sistema, utilizzando la pianificazione dell&#39;utente o la pianificazione predefinita del sistema.

     Per ulteriori informazioni, consulta [Configurare le preferenze di Gestione risorse](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

* **Allocazione delle risorse**: in qualità di responsabile delle risorse o proprietario di un progetto, puoi definire l’allocazione delle risorse per i tuoi progetti e assegnare lavoro. Per questo passaggio è possibile gestire la stima dell&#39;allocazione delle risorse utilizzando la Programmazione delle risorse o la Pianificazione scenario e assegnare il lavoro effettivo agli utenti nel Bilanciatore dei carichi di lavoro.

  Per ulteriori informazioni sulla pianificazione delle risorse e sull&#39;assegnazione del lavoro, vedere le sezioni seguenti:

   * [Pianificazione delle risorse in Adobe Workfront](../../resource-mgmt/resource-planning/resource-planning-overview.md)
   * [Pianificazione scenario Adobe Workfront](../../scenario-planner/scenario-planning.md)
   * [L’indice del Bilanciatore dei carichi di lavoro: articolo](../../resource-mgmt/workload-balancer/workload-balancer.md)

<!--
* **Resource scheduling**: After generally planning for resources to use on your projects at a high level, you can start assigning work items (tasks and issues) to users based on their job roles using the Workload Balancer.

  For more information, see [Overview of the Workload Balancer](../workload-balancer/overview-workload-balancer.md). 
-->

* **Analisi**: in qualità di responsabile delle risorse, proprietario del progetto o responsabile del personale, esaminare il rapporto Utilizzo per comprendere il confronto tra le allocazioni pianificate e preventivate delle risorse e quelle effettive. Esaminare le informazioni in base a ore, costi o ricavi. Per informazioni sul rapporto Utilizzo, vedere [Visualizza informazioni sull&#39;utilizzo delle risorse](../../resource-mgmt/resource-utilization/view-utilization-information.md).

## Accesso necessario per visualizzare e gestire le risorse utilizzando gli strumenti di gestione delle risorse in Workfront

I seguenti utenti hanno accesso agli strumenti di gestione delle risorse in Workfront:

Devi essere uno dei seguenti utenti e disporre dei seguenti diritti di accesso e autorizzazioni per accedere agli strumenti di gestione delle risorse:

* L&#39;amministratore di sistema.
* Utente con una licenza Pianificazione.

  Un utente con una licenza Lavoro può utilizzare il Bilanciatore dei carichi di lavoro di un progetto e gestire assegnazioni e allocazioni.

  Oltre a disporre di una licenza Lavoro o superiore, per utilizzare strumenti specifici di gestione delle risorse è necessario disporre dei seguenti elementi:

   * Accesso di modifica alla gestione delle risorse (non necessario per effettuare assegnazioni nel Bilanciatore dei carichi di lavoro)
   * Modifica l&#39;accesso ai dati finanziari per visualizzare le informazioni sui costi nella Programmazione delle risorse
   * Visualizzare l&#39;accesso ai dati finanziari per visualizzare le informazioni su costi e ricavi nel rapporto Utilizzo (solo utenti con una licenza Pianificazione)

* Autorizzazioni di Contribute o superiori che includono Make Assignments (Crea assegnazioni) per i progetti per i quali si desidera gestire le risorse.

<!--
* Designated as a Resource Manager for projects to use the Scheduling tool (the Scheduling tool is deprecated).

  >[!TIP]
  >
  >You do not have to be a Resource Manager to use the Resource Planner, Scenario Planner, or the Workload Balancer. 
-->

Per informazioni sull&#39;accesso necessario alle risorse del budget, vedere l&#39;articolo [Accesso necessario alle risorse del budget](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).

Per informazioni sull’accesso necessario per gestire le risorse nel Bilanciatore dei carichi di lavoro, consulta [Accesso necessario per gestire le risorse nel Bilanciatore dei carichi di lavoro](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).

## Prerequisiti per una gestione accurata delle risorse  {#prerequisites-for-accurate-resource-management}

Prima di poter utilizzare in modo efficiente gli strumenti di gestione delle risorse in Workfront, è necessario soddisfare una serie di requisiti.

Per informazioni sui requisiti di ogni strumento di gestione delle risorse in Workfront, vedere:

* La sezione [Prerequisiti per lavorare nella Programmazione delle risorse](../../resource-mgmt/resource-planning/get-started-resource-planner.md#prerequisites-for-working-in-the-resource-planner) nell’articolo [Panoramica di Programmazione delle risorse](../../resource-mgmt/resource-planning/get-started-resource-planner.md).
  <!--remove this at production: * The section "Prerequisites" in the article [Get started with Resource Scheduling](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).-->
* La sezione [Best practice per l’utilizzo del Bilanciatore dei carichi di lavoro](../../resource-mgmt/workload-balancer/overview-workload-balancer.md#best-practices-for-using-the-workload-balancer) nell’articolo [Panoramica del Bilanciatore dei carichi di lavoro](../../resource-mgmt/workload-balancer/overview-workload-balancer.md).
* [Accesso necessario per preventivare le risorse in Adobe Workfront](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).
* [Accesso necessario per gestire le risorse nel Bilanciatore dei carichi di lavoro](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: drafted and replaced with the links to each prerequisites instead) </p>
<p> We recommend that the following settings exist before starting to manage resources for your organization: </p>
<ul>
<li> You must have users in the system who have active accounts. </li>
<li> You must assign a Plan or a Worker license to the users whose work allocation you want to manage. <note type="note">
Although you can assign work to a Reviewer or a Requestor, they cannot complete it.
<br>We recommend against assigning work to Reviewers or Requestors. For information about access levels in Workfront, see
<a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md" class="MCXref xref" xrefformat="{para}">Access levels overview</a>.
</note></li>
<li> You must have job roles configured in the system.<br>For information about adding job roles to Workfront, see the article <a href="../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref" xrefformat="{para}">Create and manage job roles</a>.</li>
<li> (Optional) If you want to budget cost for your work, your job roles and your users must also have rates associated with them.<br></li>
<li> You must associate at least one job role with your users. </li>
<li> You must specify a valid value for the FTE field of all users when you use the User's Schedule instead of The Default Schedule in your Resource Management system preferences. <br>For information about editing users to ensure they have a job role, FTE, or cost associated with them, see the article <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref" xrefformat="{para}">Edit a user's profile</a>. For information about editing the Resource Management preferences in your system, see <a href="../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref" xrefformat="{para}">Configure Resource Management preferences</a>.</li>
<li>You must associate accurate schedules with your users and they should include schedule exceptions.<br>For information about creating and editing schedules, see the article <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" xrefformat="{para}">Create a schedule</a>.</li>
<li>The Time Off calendar of the users must be up to date. </li>
<li> <p>The following is recommended for the Resource Planner when applying the Project and Role views: </p>
<ul>
<li> <p>You must associate projects with Resource Pools.<br>For information about associating projects with Resource Pools, see <a href="../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-projects-and-templates.md" class="MCXref xref" xrefformat="{para}">Associate resource pools with projects and templates</a>.</p> </li>
</ul> </li>
<li> <p>Your must designate a Resource Manager on your projects and they must have the correct access to budget resources when using the Scheduling tools. </p> <p>For information about the access needed to budget resources, see the article <a href="../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md" class="MCXref xref" xrefformat="{para}">Access needed to budget resources in&nbsp;Adobe Workfront</a>.</p> </li>
<li> <p>You must assign the tasks and issues in your system to job roles, teams, or users.</p> </li>
<li>You must specify a valid value for Planned Hours and Duration for all tasks in your system.<br>For information about Planned Hours, see the article <a href="../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref" xrefformat="{para}">Planned Hours overview</a>.<br>For information about Duration, see the article <a href="../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref" xrefformat="{para}">Overview of Task Duration and Duration Type</a>.</li>
</ul>
</div>
-->
