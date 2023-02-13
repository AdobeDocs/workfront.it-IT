---
content-type: overview
product-area: resource-management
navigation-topic: resource-planning
title: Panoramica di Resource Planner
description: È possibile stimare e preventivare l'allocazione delle risorse ai progetti a cui sono assegnate e prevedere la loro disponibilità per il lavoro futuro utilizzando il Resource Planner.
author: Alina
feature: Resource Management
exl-id: 06cd2226-f94d-4b6a-8692-6d35210782f2
source-git-commit: ec49a7d3adeb24c1b8df0ff5fafe650d18d92280
workflow-type: tm+mt
source-wordcount: '2077'
ht-degree: 0%

---

# Panoramica di Resource Planner

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Alina: this used to be the beginning of Planning in the Resource Planner - consider restructuring it further? Merging some of this information with information about Understanding Navigation in the RP?!)</p>
-->

È possibile stimare e preventivare l&#39;allocazione delle risorse ai progetti a cui sono assegnate e prevedere la loro disponibilità per il lavoro futuro utilizzando il Resource Planner.

Per una panoramica generale della pianificazione delle risorse in Adobe Workfront, consulta l’articolo [Guida introduttiva alla pianificazione delle risorse](../../resource-mgmt/resource-planning/get-started-resource-planning.md).

## Panoramica di Resource Planner

È possibile utilizzare il Planner risorse per comprendere facilmente la disponibilità di utenti e ruoli di lavoro, nonché il tempo pianificato necessario per completare il lavoro sui progetti. Puoi quindi decidere come allocare gli utenti e i loro ruoli di lavoro in base ai progetti a cui sono assegnati in base al tempo disponibile.

>[!IMPORTANT]
>
>Non è possibile utilizzare il Planner risorse per assegnare agli utenti il lavoro effettivo (attività e problemi). È possibile stimare solo il tempo necessario agli utenti o ai ruoli del lavoro per completare un progetto, indipendentemente dalle attività e dai problemi a cui sono assegnati.\
>Per assegnare il lavoro effettivo agli utenti è necessario utilizzare il servizio di bilanciamento del carico di lavoro. Per ulteriori informazioni sul servizio di bilanciamento del carico di lavoro, vedi [Panoramica del servizio di bilanciamento del carico di lavoro](../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

È possibile visualizzare le informazioni nel Planner risorse utilizzando tre viste separate. È possibile utilizzare ogni visualizzazione per soddisfare uno dei seguenti obiettivi:

* Per eseguire il budget del tempo o del costo delle risorse per il lavoro da eseguire utilizzando le visualizzazioni Progetto e Ruolo . Questo è lo scopo principale del Planner risorse.\
   Per ulteriori informazioni sull&#39;impostazione del budget in Resource Planner, vedere l&#39;articolo [Risorse di budget nel planner risorse utilizzando le visualizzazioni Progetto e Ruolo](../resource-planning/budget-resources-project-role-views-resource-planner.md).

* Per visualizzare le seguenti informazioni utilizzando la visualizzazione Utente:

   * la disponibilità degli utenti in base alla loro pianificazione
   * il tempo previsto necessario per completare il lavoro secondo il piano di progetto.
   * il tempo di accesso degli utenti agli elementi di lavoro effettivi.

   Per ulteriori informazioni sulla visualizzazione di Ore disponibili, pianificate e effettive o FTE per gli utenti nel Planner risorse, vedere l&#39;articolo [Visualizza Ore disponibili, pianificate e effettive o FTE nel planner risorse quando si utilizza la visualizzazione Utente](../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md#using).

## Considerazioni sul planner risorse

* Puoi assegnare priorità ai progetti su cui stai lavorando e assegnare le risorse in base alla loro priorità, per assicurarti di disporre delle risorse assegnate prima ai progetti più importanti.

   Per informazioni sulla priorità dei progetti nel Planner risorse, vedi [Assegnare priorità ai progetti nel planner risorse](../../resource-mgmt/resource-planning/prioritize-projects-resource-planner.md).

* È possibile visualizzare informazioni su ore, FTE e costi derivanti dalle attività e dai problemi dei progetti.

   >[!NOTE]
   >
   >Le attività e i problemi non vengono visualizzati nel Planner risorse. Tuttavia, le informazioni su ore, FTE e costi derivanti dalle allocazioni di risorse sulle attività vengono visualizzate nel Planner risorse come numero totale per il progetto.

* Le informazioni relative all&#39;ora, all&#39;FTE e ai costi delle attività principali sono escluse dai progetti visualizzati nel Planner risorse. È consigliabile assegnare le risorse solo alle attività secondarie se si desidera gestire il tempo o il costo di tali risorse nel Planner risorse.

   Per informazioni sulle attività principali, vedere i seguenti articoli:

   * [Panoramica delle attività](../../manage-work/tasks/task-information/tasks-overview.md)
   * [Creare sottoattività](../../manage-work/tasks/create-tasks/create-subtasks.md)

   >[!TIP]
   >
   >Le attività padre presentano un totale delle ore e dei costi delle attività figlio. Per questo motivo, il conteggio di ore, FTE e costi delle attività figlio e delle attività padre conteggiava questi importi due volte. Per questo motivo le informazioni sull&#39;attività padre vengono escluse dal Planner risorse.

* Non è possibile gestire l’allocazione dei team nei progetti per i quali hanno attività o problemi nel Planner risorse.
* È possibile allocare risorse per più progetti alla volta utilizzando il Planner risorse o per un singolo progetto utilizzando l&#39;area Budget risorse del Business Case. Le informazioni di budget per un progetto vengono visualizzate anche nel Planner risorse.

   Per informazioni sulle modalità di budget delle risorse per un singolo progetto, consulta l’articolo [Risorse di budget nel Business Case](../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

   Per informazioni sulle modalità di budget delle risorse nel Planner risorse per più progetti alla volta, vedere la sezione &quot;Risorse di budget nel Planner risorse&quot; nell&#39;articolo [Risorse di budget nel planner risorse utilizzando le visualizzazioni Progetto e Ruolo](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

## Prerequisiti per l’utilizzo del planner risorse {#prerequisites-for-working-in-the-resource-planner}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(<b>THIS SECTION IS LINKED TO ALL RES PLANNING ARTICLES. DO NOT RENAME OF DELETE THIS!</b> - do NOT ADD the variable here, because it might break this link!)</p>
-->

Per utilizzare correttamente il Planner risorse per l&#39;impostazione del budget delle risorse, è innanzitutto necessario assicurarsi che tu, i tuoi progetti e le tue attività soddisfino un insieme di prerequisiti. Questi prerequisiti sono obbligatori per visualizzare le informazioni corrette nel Planner risorse e per gestire con precisione le risorse.

>[!IMPORTANT]
>
>Se manca uno dei seguenti prerequisiti, è possibile che alcune informazioni sull&#39;allocazione o sulla disponibilità delle risorse siano mancanti o abbiano un valore zero.\
>Per ulteriori informazioni sui motivi per cui i campi mancano di dati o hanno valori zero, passa il cursore del mouse sui campi.

![](assets/no-users-with-this-role-in-the-res-pool-350x57.png)

>[!NOTE]
>
>I prerequisiti seguenti sono necessari solo quando si visualizza il Planner risorse per progetto o per ruolo di lavoro o quando si inseriscono risorse nel budget nel Business case di un progetto.

I seguenti tipi di prerequisiti sono necessari per la corretta funzionalità del Planner risorse quando lo si visualizza per progetto o per ruolo:

* [Prerequisiti utente](#user-prerequisites)
* [Prerequisiti per il progetto](#project-prerequisites)
* [Attività e problemi prerequisiti](#tasks-and-issues-prerequisites)
* [Prerequisiti a livello di sistema](#system-level-prerequisites)

### Prerequisiti utente {#user-prerequisites}

Verificare che esista la seguente configurazione utente prima di iniziare a utilizzare il Planner risorse:

* Accesso corretto alle risorse di budget.

   Per informazioni sull&#39;accesso necessario alle risorse di budget, consulta l&#39;articolo [Accesso necessario alle risorse di budget in Adobe Workfront](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).

* Gli utenti assegnati alle attività vengono aggiunti ai pool di risorse associati al progetto.

   Per informazioni sull’aggiunta di utenti ai pool di risorse, consulta [Associare pool di risorse con gli utenti](../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md).

   >[!NOTE]
   >
   >Quando gli utenti non vengono aggiunti ai pool di risorse, possono esistere i seguenti scenari:
   >
   >   
   >   
   >   * Gli utenti non vengono visualizzati nel Planner risorse anche se possono essere assegnati a attività sui progetti.
   >   * Se le attività a cui sono associate hanno orari pianificati, tali ore non vengono visualizzate nel Planner risorse per il progetto, a meno che l&#39;utente non sia associato anche a un ruolo di lavoro per tali attività.
   >   * Se gli utenti sono associati a un ruolo di lavoro in un&#39;attività del progetto, nel Planner risorse viene visualizzato l&#39;orario pianificato per il ruolo di lavoro, ma il ruolo di lavoro non può essere inserito in budget.


* Gli utenti assegnati a pool di lavoro e risorse devono disporre di Pianificazioni e Ruoli lavoro associati al loro profilo.

   Per informazioni sull&#39;associazione di Pianificazioni e Ruoli processo con gli utenti, consulta [Modificare il profilo di un utente](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

   >[!NOTE]
   >
   >Gli utenti che non sono associati a un programma ma che si trovano nel pool di risorse del progetto non possono essere inseriti in budget nel Planner risorse.

* Per informazioni precise sulle ore disponibili, assicurati che le pianificazioni associate agli utenti dispongano delle eccezioni di pianificazione e del tempo di inattività aggiornati.

   >[!NOTE]
   >
   >Se un utente non è associato a una pianificazione, la pianificazione predefinita del sistema Workfront è associata all&#39;utente per impostazione predefinita, ai fini del planner risorse.

   Per informazioni sulla creazione delle pianificazioni, consulta l’articolo [Creare una pianificazione](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* Se si desidera eseguire il budget delle risorse in base al costo, è necessario associare i ruoli processo a Costo/Ora. tariffe. Il costo associato ai ruoli di lavoro assegnati agli utenti nei pool di risorse viene utilizzato per calcolare il costo del lavoro in budget e il costo in budget del progetto.\
   Per informazioni sull&#39;associazione dei ruoli di lavoro con le tariffe, vedere l&#39;articolo [Creare e gestire ruoli di lavoro](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).\
   Per informazioni sul calcolo del costo del lavoro a budget, vedere l&#39;articolo [Comprendere i costi del lavoro e le ore previste per i progetti](../../manage-work/projects/project-finances/budgeted-labor-cost.md).\
   Per informazioni sul calcolo del costo preventivato, vedere l&#39;articolo [Calcola costo preventivato](../../manage-work/projects/project-finances/budgeted-cost.md).

### Prerequisiti per il progetto {#project-prerequisites}

Verificare che esista la seguente configurazione del progetto prima di iniziare a utilizzare il Planner risorse:

* I progetti sono associati a pool di risorse.\
   Per ulteriori informazioni sull’aggiunta di pool di risorse ai progetti, consulta [Associare pool di risorse a progetti e modelli](../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-projects-and-templates.md).

   >[!IMPORTANT]
   >
   >Nei progetti senza pool di risorse non vengono visualizzate le informazioni relative all&#39;ora pianificata o alle assegnazioni nel planner risorse.

### Attività e problemi prerequisiti {#tasks-and-issues-prerequisites}

Sebbene non sia possibile visualizzare attività e problemi nel Planner risorse, le relative informazioni vengono trasferite ai progetti visualizzati nel Planner risorse .

Prima di avviare le risorse di budget in Resource Planner, verificare che l&#39;attività e la configurazione del problema seguenti siano presenti:

* Le attività o i problemi relativi ai progetti per i quali vengono assegnate risorse di budget a una delle seguenti entità:

   * Utenti nei pool di risorse del progetto associati anche a Ruoli lavoro
   * Ruoli

   >[!NOTE]
   >
   >L&#39;orario pianificato delle attività e dei problemi assegnati ai ruoli del lavoro viene visualizzato nel Planner risorse, ma queste ore non possono essere iscritte in budget a meno che un utente associato al ruolo del lavoro non sia elencato in un pool di risorse associato al progetto.

* Non assegnare attività principali a utenti o ruoli.

   Per visualizzare le informazioni sulle ore nel Planner risorse per gli utenti o i ruoli associati alle attività principali, è necessario assegnarle anche alle attività secondarie. Il Planner risorse non visualizza informazioni relative alle attività principali.

* Le attività e i problemi hanno un valore per Orari pianificati maggiore di zero.
* Le attività e i problemi hanno un valore per la loro Durata maggiore di zero.
* Le date pianificate dei problemi si trovano nella timeline del progetto.

### Prerequisiti a livello di sistema {#system-level-prerequisites}

È necessario comprendere in che modo l’istanza di Workfront calcola la disponibilità dell’utente in base alle preferenze di gestione delle risorse nel sistema. Workfront può calcolare la disponibilità dell’utente utilizzando la pianificazione dell’utente definita nella pagina Profilo utente o nella pianificazione predefinita del sistema.

![](assets/resource-management-preferences-section-in-setup-350x89.png)

L&#39;amministratore Workfront configura le preferenze di gestione delle risorse.

Per ulteriori informazioni, consulta [Configurare le preferenze di Gestione risorse](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

## Individua il planner risorse

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(This became another standalone article; drfat this section here when article is live.)</p>
-->

È possibile individuare il Planner risorse in due aree di Workfront, a seconda che si desideri assegnare il budget alle risorse per più progetti o per un solo progetto.

Per informazioni su come individuare il planner risorse, vedere [Individua il planner risorse](../../resource-mgmt/resource-planning/locate-resource-planner.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(this is drafted and moved to its own article: locate-resource-planner) </p>
<p>Ensure that all prerequisites are met before starting to use the Resource Planner. This way, you ensure that the Resource Planner displays the correct information before you start budgeting your resources.<br>For information about the prerequisites that must be met before you can start using the Resource Planner, see the <a href="#prerequisites-for-working-in-the-resource-planner" class="MCXref xref">Prerequisites for working in the Resource Planner</a> section in this article. </p>
<p>You can locate the Resource Planner in two areas of Workfront, depending on whether you want to budget your resources for multiple projects, or for just one project.</p>
<ul>
<li><a href="#use-the-resource-planner-for-multiple-projects" class="MCXref xref">Use the Resource Planner for multiple projects</a> </li>
<li> <p><a href="#use-the-resource-planner-for-one-project" class="MCXref xref">Use the Resource Planner for one project</a> </p> </li>
</ul>
<p><strong>Use the Resource Planner for multiple projects</strong></p>
<p>When using the Resource Planner for multiple projects, the allocation numbers for your resources represent numbers across multiple projects. </p>
<p>To access the  Planner section  in the  Resourcing area: </p>
<ol>
<li value="1">  Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront.  </li>
<li value="2"> <p>  Click <strong>Resourcing</strong>. The Resource Planner displays by default.  For information about budgeting resources in the Resource Planner, see the article <a href="../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Budget resources in the Resource Planner using the Project and Role views</a>. </p> <p> <img src="assets/qs-resource-management-area-with-planner-as-default-350x152.png" style="width: 350;height: 152;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="3">  Hover over the left panel, and click <strong>Resource Pools</strong>. <br>For information about creating new resource pools, see <a href="../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md" class="MCXref xref">Create resource pools</a>.</li>
</ol>
<p><strong>Use the Resource Planner for one project</strong></p>
<p>When using the Resource Planner for one project, the allocation numbers for your resources represent numbers for the selected project. </p>
<ol>
<li value="1"> <p>Go to a project you want to budget resources for.</p> </li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Business Case</strong> in the left panel.</p> </li>
<li value="3"> <p>Scroll to the <strong>Resource Budgeting</strong> section of the Business Case.</p> </li>
<li value="4"> <p>Click <strong>Edit Resource Budgeting</strong> to add resource pools to your project and start budgeting your resources. </p> <note type="tip">
You can only add a resource pool in the Resource Budgeting area of the Business Case when the project has no resource pools associated with it. When the project already has a resource pool, the users in the pool and their job roles display in the Resource Budgeting area by default.
</note> <p> <img src="assets/resource-budgeting-area-on-project-350x70.png" style="width: 350;height: 70;"> </p> <p>For information about budgeting resources for one project, see the article <a href="../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md" class="MCXref xref">Budget resources in the Business Case</a>.</p> </li>
</ol>
</div>
-->

## Aree del planner risorse

È possibile visualizzare le informazioni seguenti o eseguire le azioni seguenti nel Planner risorse:

* Informazioni sulle risorse assegnate ai progetti nel Planner risorse in una cronologia generale.
* Sovrallocazione o sottoutilizzo delle risorse nel Planner risorse.
* Budget le risorse per lavorare manualmente o automaticamente.

Per ulteriori informazioni sulle aree da visualizzare nel Planner risorse e su come configurare le informazioni da visualizzare in queste aree, vedere l&#39;articolo [Panoramica sulla navigazione in planner risorse](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

## Limitazioni nella visualizzazione delle informazioni nel Planner risorse

Per migliorare le prestazioni, Workfront limita la quantità di elementi che è possibile visualizzare nel planner risorse.

Per ulteriori informazioni su queste limitazioni, consulta l’articolo [Limitazioni della visualizzazione di Resource Planner](../../resource-mgmt/resource-planning/resource-planner-display-limitations.md) .

## Calcola FTE nel planner risorse

È possibile visualizzare la disponibilità, l&#39;allocazione e i valori pianificati nel Planner risorse in ore, FTE o Costo.

Per ulteriori informazioni sulla modifica delle informazioni visualizzate nel Planner risorse, vedere la sezione [Visualizza le informazioni per ora, FTE o Costo](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md#display-by-hour-or-fte-menu) nell&#39;articolo [Verifica la disponibilità e l’allocazione delle risorse utilizzando Adobe Workfront Resource Planner](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md).

Per ulteriori informazioni sul calcolo delle ore e degli FTE per utenti e ruoli in Workfront, consulta l’articolo [Panoramica del calcolo delle ore e degli FTE per utenti e ruoli nel Planner risorse](../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md).

## Calcolare i costi nel planner risorse

Per visualizzare le informazioni in base al costo nel planner risorse, è necessario disporre dell&#39;accesso Visualizza dati finanziari e Visualizza autorizzazioni di finanziamento per i progetti.

Oltre a visualizzare la disponibilità, l&#39;allocazione e i valori pianificati nel Planner risorse in ore e FTE, puoi anche visualizzarli per costo.

>[!TIP]
>
>Per visualizzare le informazioni in base ai costi nel planner risorse, è necessario associare gli utenti e i ruoli lavoro ai tassi di costo per ora.

Per ulteriori informazioni sull&#39;associazione dei tassi di costo per ora con i ruoli di lavoro, consulta l&#39;articolo [Creare e gestire ruoli di lavoro](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).\
Per ulteriori informazioni sull&#39;associazione delle tariffe di costo per ora con gli utenti, consulta l&#39;articolo [Modificare il profilo di un utente](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Quando si visualizzano le informazioni in base al costo nel planner risorse, tenere presente quanto segue:

* Il costo di ogni tipo di ore (Pianificato, Disponibile, Preventivo, Effettivo per utenti, ruoli o progetti) viene calcolato utilizzando un diverso tasso di costo.
* Il costo pianificato è influenzato dal tipo di costo delle attività relative ai progetti.
* Quando si applica la visualizzazione utente al planner risorse, non è possibile visualizzare le informazioni di allocazione e disponibilità in base al costo.

Per ulteriori informazioni sul calcolo dei costi nel Planner risorse per utenti e ruoli, consulta l’articolo [Calcolare i costi nel planner risorse](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the User View to view Available, Planned, and Actual Hours or FTE </h2>
<p>(this information is repeated from above where it exists in shorter form. Drafted to simplify the amount of info of this article.) </p>
<p>You can use the User View of the Resource Planner to display information about the Planned, Available, and Actual Hours or FTE values for projects and resources. </p>
<p>For information about using the Resource Planner to review the Available, Planned, and Actual Hours and FTE for resources, see the article <a href="../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md" class="MCXref xref">View Available, Planned, and Actual Hours or FTE in the Resource Planner when using the User view</a>.</p>
<p><strong>Use the Project and Role Views to budget resources </strong></p>
<p> The main function of the Resource Planner is to budget your resources for the work that needs to be completed on the projects that you can manage. </p>
<p> You can budget your resources only if you apply the <strong>View by Project</strong> or <strong>View by Role</strong> views to the Resource Planner.</p>
<p>For information about budgeting resources using the Project and Role views in the Resource Planner, see the article <a href="../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md"><a href="../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Budget resources in the Resource Planner using the Project and Role views</a></a>.</p>
</div>
-->

## Filtrare le informazioni nel planner risorse

È possibile ridurre il numero di progetti, ruoli o utenti visualizzati nel Planner risorse creando un filtro.\
Per ulteriori informazioni, consulta l’articolo [Filtrare le informazioni nel planner risorse](../../resource-mgmt/resource-planning/filter-resource-planner.md).
