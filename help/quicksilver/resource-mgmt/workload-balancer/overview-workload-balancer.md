---
content-type: overview
product-area: resource-management
navigation-topic: the-workload-balancer
title: Panoramica del servizio di bilanciamento del carico di lavoro
description: Dopo che i project manager pianificano il lavoro sui progetti e creano attività, puoi utilizzare il servizio di bilanciamento del carico di lavoro per assegnare il lavoro agli utenti dei team.
author: Alina
feature: Resource Management
exl-id: 9398bd04-9df7-4b77-8361-fdb5bdce6829
source-git-commit: 11c87d8a97261c24d063fbc824f2e907d07f8217
workflow-type: tm+mt
source-wordcount: '1122'
ht-degree: 0%

---

# Panoramica del servizio di bilanciamento del carico di lavoro

<!--
<p>(NOTE: this is linked from the UI for the Workload Balancer page. DO NOT CHANGE TITLE OR LINK) </p>
-->

Dopo aver pianificato il lavoro sui progetti e creato le attività, è possibile utilizzare il servizio di bilanciamento del carico di lavoro per assegnare il lavoro agli utenti.

>[!IMPORTANT]
>
>È possibile utilizzare il servizio di bilanciamento del carico di lavoro per assegnare agli utenti il lavoro effettivo (attività e problemi).
>
>Per stimare le allocazioni dei ruoli di lavoro per i progetti, è necessario utilizzare il planner risorse e non il servizio di bilanciamento del carico di lavoro. Per ulteriori informazioni sul planner risorse, vedere [Panoramica di Resource Planner](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

Questo articolo descrive lo scopo generale del servizio di bilanciamento del carico di lavoro e alcune delle best practice per configurare i progetti e le risorse per un utilizzo corretto.

## Individua il servizio di bilanciamento del carico di lavoro

<!--
<p>(NOTE: This will be taken out when all we will have is one tool - should be replaced by a blurb that says you can add this tool anywhere, in any custom tab, etc (long term dev promise)) </p>
-->

Per la pianificazione delle risorse è consigliabile utilizzare il servizio di bilanciamento del carico di lavoro nelle seguenti aree:

* A livello di sistema, nell&#39;area Risorse.
* A livello di progetto, nella sezione del servizio di bilanciamento del carico di lavoro di un progetto.
* A livello di team, nella sezione del servizio di bilanciamento del carico di lavoro di un team.

Per ulteriori informazioni su come individuare il servizio di bilanciamento del carico di lavoro, vedi [Individua il servizio di bilanciamento del carico di lavoro](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

## Vantaggi del bilanciamento del carico di lavoro

Quando utilizzi il servizio di bilanciamento del carico di lavoro, considera i seguenti vantaggi:

<!--
<p> Add about the what-if scenarios as a benefit when they become available </p>
-->

* Accedi a una chiara mappatura visiva della sovrallocazione delle risorse e del sottoutilizzo, trasparente per tutti i soggetti interessati.
* In qualità di responsabile delle persone, puoi proteggere la tua gente dal burnout e permettergli di lavorare al meglio con una migliore concentrazione, qualità e coinvolgimento. Puoi assicurarne il pieno utilizzo, interrompere i silos e abilitare l’allineamento del lavoro tra i team.
* Quando si assegna il lavoro a livello di attività o di problema, non si ha visibilità sulla disponibilità di un utente. Quando si utilizza il servizio di bilanciamento del carico di lavoro, è possibile visualizzare gli utenti disponibili nel carico di lavoro per completare l&#39;attività o il problema in tempo. Questo include i dettagli delle eccezioni di orario e pianificazione.

   Per ulteriori informazioni, consulta [Panoramica dell’assegnazione del lavoro nel servizio di bilanciamento del carico di lavoro](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

   È inoltre possibile assegnare elementi di lavoro in blocco, facilitando la distribuzione simultanea di un gran numero di elementi di lavoro in più progetti. Per ulteriori informazioni, consulta [Assegnare il lavoro in blocco utilizzando il bilanciamento del carico di lavoro](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md).

* I dirigenti possono prendere decisioni tempestive sul personale attraverso la trasparenza nel modo in cui le persone nella loro organizzazione vengono utilizzate.
* I membri del team beneficiano di una migliore collaborazione, in quanto possono tutti vedere su cosa stanno lavorando i loro colleghi in un dato momento. Per informazioni sull&#39;accesso necessario per visualizzare o gestire le risorse nel servizio di bilanciamento del carico di lavoro, vedi [Accesso necessario per gestire le risorse nel servizio di bilanciamento del carico di lavoro](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).
* Condividerlo con chiunque non abbia accesso all&#39;area Origine incorporando un collegamento ad essa in una scheda personalizzata. Per informazioni, consulta [Condivisione del bilanciamento del carico di lavoro con un collegamento](../../resource-mgmt/workload-balancer/share-link-for-workload-balancer.md)
* Visualizza e gestisci i carichi di lavoro e le richieste delle persone in una sola visualizzazione a livello globale, di progetto o di team, a seconda del tuo ruolo. Durante la gestione dei progetti, questo include non solo l&#39;allocazione delle risorse per il progetto, ma anche la visualizzazione dell&#39;allocazione delle risorse da Adobe Workfront Scenario Planner. I responsabili del personale utilizzano Workfront Scenario Planner per gestire le competenze professionali in tutta l’organizzazione. Il planner scenario è disponibile solo nella nuova esperienza Adobe Workfront.

   >[!NOTE]
   >
   >  Il planner scenario richiede una licenza aggiuntiva. Per informazioni su Workfront Scenario Planner, vedi [Panoramica di Scenario Planner](../../scenario-planner/scenario-planner-overview.md).


## Best practice per l’utilizzo del load balancer

È consigliabile seguire le best practice per la pianificazione dei progetti, la configurazione degli utenti e l’utilizzo dei filtri prima di iniziare a pianificare le risorse utilizzando il servizio di bilanciamento del carico di lavoro.

* [Best practice per la visualizzazione delle informazioni nel servizio di bilanciamento del carico di lavoro](#best-practices-for-displaying-information-in-the-workload-balancer)
* [Best practice per l’impostazione degli utenti](#best-practices-for-setting-up-users)
* [Best practice per l’impostazione di attività e problemi](#best-practices-for-setting-up-tasks-and-issues)

### Best practice per la visualizzazione delle informazioni nel servizio di bilanciamento del carico di lavoro {#best-practices-for-displaying-information-in-the-workload-balancer}

È consigliabile utilizzare i filtri in modo da visualizzare solo le informazioni pertinenti per gli elementi di lavoro non assegnati e per quelli assegnati.

Per informazioni sulla creazione e l’utilizzo dei filtri nel servizio di bilanciamento del carico di lavoro, consulta [Filtrare le informazioni nel servizio di bilanciamento del carico di lavoro](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

### Best practice per l’impostazione degli utenti

* Poiché l&#39;utente che pianifica il lavoro per altri, è necessario disporre dell&#39;accesso e delle autorizzazioni corrette per pianificare le risorse per il lavoro.

   Per informazioni sull&#39;accesso necessario per gestire il carico di lavoro delle risorse nel servizio di bilanciamento del carico di lavoro, vedi [Accesso necessario per gestire le risorse nel servizio di bilanciamento del carico di lavoro](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).

* Gli utenti il cui carico di lavoro si desidera gestire devono soddisfare i seguenti criteri in modo che le informazioni sulla loro disponibilità e le loro competenze siano accurate:

   * Avere le pianificazioni e i ruoli del lavoro associati al loro profilo.
   * Per ulteriori informazioni sull&#39;associazione di Pianificazioni e Ruoli processo con gli utenti, vedi [Aggiungi utenti](../../administration-and-setup/add-users/create-and-manage-users/add-users.md)
   * Se un utente non è associato a una pianificazione, la pianificazione predefinita del sistema Workfront è associata all’utente per impostazione predefinita, ai fini della gestione delle risorse.
   * Avere aggiornato le eccezioni di pianificazione nelle relative pianificazioni.\
      Per ulteriori informazioni sulla creazione delle pianificazioni, consulta [Creare una pianificazione](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)

   * Aggiorna il loro calendario Time Off nel loro profilo.\
      Per informazioni sull&#39;aggiornamento del calendario Time Off di un utente, vedi [Configurare l’ora personale di inattività in Adobe Workfront](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

      <!--   
     <div data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     <p>(NOTE: Add another bullet for Costs, when this becomes available:</p>   
     <p>If you want to budget your resources by Cost, you must associate Job Roles with Cost/ Hr. rates. The cost associated with Job Roles assigned to users in your Resource Pools is used to calculate the Budgeted Labor Cost and the Budgeted Cost of the project.For more information about associating job roles with rates, see the article Creating and Managing Job Roles in the new Adobe Workfront experience.For more information about calculating Budgeted Labor Cost, see the article Calculating Budgeted Labor Cost in the new Adobe Workfront experience.For more information about calculating Budgeted Cost, see the article Calculating Budgeted Cost in .) </p>   
     </div>   
     -->

* L’amministratore di Workfront deve determinare in che modo Workfront calcola la disponibilità degli utenti. Possono decidere se Workfront utilizza la pianificazione predefinita del sistema o la pianificazione dell&#39;utente per calcolare l&#39;ora in cui l&#39;utente è disponibile a lavorare. Per ulteriori informazioni, consulta [Configurare le preferenze di Gestione risorse](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

### Best practice per l’impostazione di attività e problemi {#best-practices-for-setting-up-tasks-and-issues}

Assicurati che esista la seguente attività e configurazione del problema prima di iniziare ad assegnare il lavoro agli utenti nel workload Balancer:

* Le attività principali non sono assegnate a utenti o ruoli. Non vengono visualizzati nel bilanciamento del carico di lavoro.
* Le attività e i problemi hanno un valore per Orari pianificati maggiore di zero.

* Le attività e i problemi hanno un valore per la loro Durata maggiore di zero.
* Le date pianificate dei problemi si trovano nella timeline del progetto.

## Prima di iniziare a utilizzare il servizio di bilanciamento del carico di lavoro

* È possibile utilizzare il servizio di bilanciamento del carico di lavoro per assegnare il lavoro e gestire le allocazioni giornaliere per gli utenti dell&#39;organizzazione.

   Questo articolo illustra come navigare nel servizio di bilanciamento del carico di lavoro per eseguire queste azioni: [Naviga nel bilanciamento del carico di lavoro](../workload-balancer/navigate-the-workload-balancer.md).

   Gli articoli seguenti illustrano come assegnare il lavoro e gestire le allocazioni degli utenti:

   * [Panoramica dell’assegnazione del lavoro nel servizio di bilanciamento del carico di lavoro](../workload-balancer/assign-work-in-workload-balancer.md).
   * [Gestire le allocazioni di utenti nel load balancer](../workload-balancer/manage-user-allocations-workload-balancer.md).

* Il servizio di bilanciamento del carico di lavoro può trovarsi in diverse aree di Workfront. Per informazioni su dove è possibile trovare il servizio di bilanciamento del carico di lavoro, vedi [Individua il servizio di bilanciamento del carico di lavoro](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

## Accesso necessario per utilizzare il servizio di bilanciamento del carico di lavoro

Per poter visualizzare e utilizzare il servizio di bilanciamento del carico di lavoro in Workfront, è necessario disporre dell’accesso e delle autorizzazioni Workfront corretti per progetti specifici. Per informazioni sull&#39;accesso necessario per utilizzare il servizio di bilanciamento del carico di lavoro, consulta l&#39;articolo [Accesso necessario per gestire le risorse nel servizio di bilanciamento del carico di lavoro](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).
