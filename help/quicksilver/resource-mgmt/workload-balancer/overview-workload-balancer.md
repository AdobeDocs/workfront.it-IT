---
content-type: overview
product-area: resource-management
navigation-topic: the-workload-balancer
title: Panoramica del Bilanciatore dei carichi di lavoro
description: Dopo che i project manager hanno pianificato il lavoro sui progetti creando attività e dopo aver allocato le risorse dei ruoli ai progetti nella Programmazione risorse, i project manager e i team manager possono utilizzare il Bilanciatore dei carichi di lavoro per assegnare gli elementi di lavoro agli utenti.
author: Lisa
feature: Resource Management
exl-id: 9398bd04-9df7-4b77-8361-fdb5bdce6829
source-git-commit: 3c5bcb85080a882a8b69bffcd01563a0479f98a5
workflow-type: tm+mt
source-wordcount: '1180'
ht-degree: 0%

---

# Panoramica del Bilanciatore dei carichi di lavoro

<!--
<p>(NOTE: this is linked from the UI for the Workload Balancer page. DO NOT CHANGE TITLE OR LINK) </p>
-->

Dopo che i project manager hanno pianificato il lavoro sui progetti creando attività e dopo aver allocato le risorse dei ruoli ai progetti nella Programmazione risorse, i project manager e i team manager possono utilizzare il Bilanciatore dei carichi di lavoro per assegnare gli elementi di lavoro agli utenti.

>[!IMPORTANT]
>
>È possibile utilizzare il Bilanciatore dei carichi di lavoro per assegnare il lavoro effettivo (attività e problemi) agli utenti.
>
>È necessario utilizzare la pianificazione delle risorse e non il bilanciatore dei carichi di lavoro per stimare le allocazioni dei ruoli per i progetti, a un livello elevato. Per ulteriori informazioni sulla Programmazione delle risorse, consulta [Panoramica di Programmazione delle risorse](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

Questo articolo descrive lo scopo generale del Bilanciatore dei carichi di lavoro e alcune delle best practice per configurare progetti e risorse per utilizzarlo con successo.

Per rivedere i video tutorial sul Bilanciatore dei carichi di lavoro, vai al [Tutorials Workfront](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html) pagina. Nel menu a sinistra, seleziona **Gestire le risorse** > **Bilanciatore dei carichi di lavoro** e scegli un tutorial.

## Individuare il Bilanciatore dei carichi di lavoro

<!--
<p>(NOTE: This will be taken out when all we will have is one tool - should be replaced by a blurb that says you can add this tool anywhere, in any custom tab, etc (long term dev promise)) </p>
-->

È consigliabile utilizzare il Bilanciatore dei carichi di lavoro nelle seguenti aree per pianificare le risorse:

* A livello di sistema, nell&#39;area Risorse.
* A livello di progetto, nella sezione Bilanciatore dei carichi di lavoro di un progetto.
* A livello di team, nella sezione Bilanciatore dei carichi di lavoro di un team.

Per ulteriori informazioni sull’individuazione del Bilanciatore dei carichi di lavoro, consulta [Individuare il Bilanciatore dei carichi di lavoro](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

## Vantaggi del Bilanciatore dei carichi di lavoro

Quando utilizzi il Bilanciatore dei carichi di lavoro, considera i seguenti vantaggi:

<!--
<p> Add about the what-if scenarios as a benefit when they become available </p>
-->

* Accedi a una chiara mappatura visiva della sovrassegnazione e del sottoutilizzo delle risorse, che sia trasparente per tutte le parti interessate.
* In qualità di responsabile del personale, puoi proteggere il tuo personale dall’esaurimento e metterlo in grado di svolgere il suo lavoro al meglio con maggiore attenzione, qualità e coinvolgimento. Puoi garantirne l’utilizzo completo, suddividere i silos e consentire l’allineamento del lavoro tra i team.
* Quando si assegna il lavoro a livello di attività o di problema, non si ha visibilità di quanto occupato un utente. Quando utilizzi il Bilanciatore dei carichi di lavoro, puoi visualizzare quali utenti dispongono di disponibilità nel loro carico di lavoro per completare l’attività o il problema in tempo. Questo include i dettagli relativi alle ferie e alle eccezioni alla pianificazione.

  Per ulteriori informazioni, consulta [Panoramica sull’assegnazione del lavoro nel Bilanciatore dei carichi di lavoro](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

  È inoltre possibile assegnare elementi di lavoro in blocco, semplificando così la distribuzione di più elementi di lavoro contemporaneamente in più progetti. Per ulteriori informazioni, consulta [Assegnare il lavoro in blocco utilizzando il Bilanciatore dei carichi di lavoro](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md).

* I dirigenti possono prendere decisioni tempestive in materia di assegnazione del personale attraverso la trasparenza delle modalità di utilizzo delle persone all&#39;interno dell&#39;organizzazione.
* I membri del team traggono vantaggio da una migliore collaborazione, in quanto possono tutti visualizzare su cosa stanno lavorando i loro colleghi in un dato momento. Per informazioni sull’accesso necessario per visualizzare o gestire le risorse nel Bilanciatore dei carichi di lavoro, consulta [Accesso necessario per gestire le risorse nel Bilanciatore dei carichi di lavoro](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).
* Per condividerlo con utenti che non hanno accesso all&#39;area Risorse, incorpora un collegamento in una scheda personalizzata. Per informazioni, consulta [Condividere il Bilanciatore dei carichi di lavoro con un collegamento](../../resource-mgmt/workload-balancer/share-link-for-workload-balancer.md)
* Visualizza e gestisci i carichi di lavoro e la domanda delle persone in un’unica vista a livello globale, di progetto o di team, a seconda del ruolo. Durante la gestione dei progetti, questo include non solo l’allocazione delle risorse per il progetto, ma anche la visualizzazione dell’allocazione delle risorse da Adobe Workfront Scenario Planner. I responsabili delle persone utilizzano Workfront Scenario Planner per gestire le competenze professionali in tutta l’organizzazione. La funzione Pianificazione scenario è disponibile solo nella nuova esperienza Adobe Workfront.

  >[!NOTE]
  >
  >  Scenario Planner richiede una licenza aggiuntiva. Per informazioni su Workfront Scenario Planner, consulta [Panoramica sulla pianificazione degli scenari](../../scenario-planner/scenario-planner-overview.md).


## Best practice per l’utilizzo del Bilanciatore dei carichi di lavoro

Per la pianificazione dei progetti, la configurazione degli utenti e l’utilizzo dei filtri, consigliamo le seguenti best practice prima di iniziare a pianificare le risorse utilizzando il Bilanciatore dei carichi di lavoro.

* [Best practice per la visualizzazione delle informazioni nel Bilanciatore dei carichi di lavoro](#best-practices-for-displaying-information-in-the-workload-balancer)
* [Best practice per la configurazione degli utenti](#best-practices-for-setting-up-users)
* [Best practice per l’impostazione di attività e problemi](#best-practices-for-setting-up-tasks-and-issues)

### Best practice per la visualizzazione delle informazioni nel Bilanciatore dei carichi di lavoro {#best-practices-for-displaying-information-in-the-workload-balancer}

È consigliabile utilizzare i filtri in modo da poter visualizzare solo le informazioni pertinenti per gli elementi di lavoro non assegnati e assegnati.

Per informazioni sulla creazione e l’utilizzo dei filtri nel Bilanciatore dei carichi di lavoro, consulta [Filtrare le informazioni nel Bilanciatore dei carichi di lavoro](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

### Best practice per la configurazione degli utenti

* L&#39;utente che pianifica il lavoro per gli altri deve disporre dell&#39;accesso e delle autorizzazioni corretti per pianificare le risorse per il lavoro.

  Per informazioni sull’accesso necessario per gestire il carico di lavoro delle risorse nel Bilanciatore dei carichi di lavoro, consulta [Accesso necessario per gestire le risorse nel Bilanciatore dei carichi di lavoro](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).

* Gli utenti il cui carico di lavoro si desidera gestire devono soddisfare i seguenti criteri in modo che le informazioni sulla loro disponibilità e sulle loro competenze siano accurate:

   * Hanno Schedules e Ruoli associati al loro profilo.

     Per ulteriori informazioni sull&#39;associazione di pianificazioni e mansioni agli utenti, vedere [Aggiungi utenti](../../administration-and-setup/add-users/create-and-manage-users/add-users.md)
   * Se un utente non è associato a una pianificazione, la pianificazione predefinita del sistema Workfront viene associata all&#39;utente per impostazione predefinita, ai fini della gestione delle risorse.
   * Richiedere l&#39;aggiornamento delle eccezioni di pianificazione nelle proprie pianificazioni.

     Per ulteriori informazioni sulla creazione di pianificazioni, vedere [Creare una pianificazione](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)

   * Aggiornare il calendario Time Off (Ferie) nel profilo.

     Per informazioni sull&#39;aggiornamento del calendario Time Off (Ferie) di un utente, vedere [Configurare l’indisponibilità personale](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

     <!--   
     <div data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     <p>(NOTE: Add another bullet for Costs, when this becomes available:</p>   
     <p>If you want to budget your resources by Cost, you must associate Job Roles with Cost/ Hr. rates. The cost associated with Job Roles assigned to users in your Resource Pools is used to calculate the Budgeted Labor Cost and the Budgeted Cost of the project.For more information about associating job roles with rates, see the article Creating and Managing Job Roles in the new Adobe Workfront experience.For more information about calculating Budgeted Labor Cost, see the article Calculating Budgeted Labor Cost in the new Adobe Workfront experience.For more information about calculating Budgeted Cost, see the article Calculating Budgeted Cost in .) </p>   
     </div>   
     -->

* L&#39;amministratore di Workfront deve determinare il modo in cui Workfront calcola la disponibilità degli utenti. Possono decidere se Workfront utilizza la pianificazione predefinita del sistema o la pianificazione dell&#39;utente per calcolare il tempo in cui l&#39;utente è disponibile a lavorare modificando le preferenze di Gestione risorse nell&#39;area Configurazione di Workfront.

  Per ulteriori informazioni, consulta [Configurare le preferenze di Gestione risorse](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

### Best practice per l’impostazione di attività e problemi {#best-practices-for-setting-up-tasks-and-issues}

Prima di iniziare a assegnare il lavoro agli utenti nel Bilanciatore dei carichi di lavoro, assicurati che siano presenti le seguenti impostazioni di attività e problemi:

* Le attività padre non vengono assegnate a utenti o ruoli. Le attività padre non vengono visualizzate nel Bilanciatore dei carichi di lavoro.
* Le attività e i problemi hanno un valore per Ore pianificate maggiore di zero.

* Le attività e i problemi hanno un valore per la durata maggiore di zero.
* Le Date Pianificate dei problemi rientrano nella timeline del progetto.

## Prima di iniziare a utilizzare il Bilanciatore dei carichi di lavoro

* Rivedi i seguenti articoli prima di iniziare a utilizzare il Bilanciatore dei carichi di lavoro:

   * Questo articolo illustra come navigare nel Bilanciatore dei carichi di lavoro per eseguire le azioni seguenti: [Navigare nel Bilanciatore dei carichi di lavoro](../workload-balancer/navigate-the-workload-balancer.md).

   * I seguenti articoli descrivono come assegnare lavoro e gestire le allocazioni utente:

      * [Panoramica sull’assegnazione del lavoro nel Bilanciatore dei carichi di lavoro](../workload-balancer/assign-work-in-workload-balancer.md).
      * [Gestire le allocazioni utente nel Bilanciatore dei carichi di lavoro](../workload-balancer/manage-user-allocations-workload-balancer.md).

* Il Bilanciatore dei carichi di lavoro si trova in diverse aree di Workfront. Per informazioni su dove è possibile trovare il Bilanciatore dei carichi di lavoro, vedi [Individuare il Bilanciatore dei carichi di lavoro](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

## Accesso necessario per utilizzare il Bilanciatore dei carichi di lavoro

Per poter visualizzare e utilizzare il Bilanciatore dei carichi di lavoro in Workfront, è necessario disporre dell’accesso e delle autorizzazioni Workfront corretti per progetti specifici. Per informazioni sull’accesso necessario per utilizzare il Bilanciatore dei carichi di lavoro, consulta l’articolo [Accesso necessario per gestire le risorse nel Bilanciatore dei carichi di lavoro](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).
