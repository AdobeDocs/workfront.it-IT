---
content-type: overview
product-area: resource-management
navigation-topic: the-workload-balancer
title: Panoramica sul bilanciamento dei carichi di lavoro
description: Dopo che i project manager hanno pianificato il lavoro sui progetti creando attività e dopo che i manager delle risorse hanno allocato le risorse delle mansioni ai progetti nella pianificazione risorse, i manager del team e i proprietari dei progetti possono utilizzare il bilanciamento dei carichi di lavoro per assegnare gli elementi di lavoro agli utenti.
author: Lisa
feature: Resource Management
exl-id: 9398bd04-9df7-4b77-8361-fdb5bdce6829
TQID: https://experienceleague.adobe.com/fMt1jY5l7jMYTHUeKNyCE-HJdDEH89xmLqG2UacvU7c
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2:
  - id: c33d85a1-be85-4290-854c-87408c10aa80
  - id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
  - id: d1573eb8-a2e8-4a06-9526-9c3410bf4914
  - id: d3382524-5489-431b-bde9-271ab257bc37
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 1202
ht-degree: 100%

---

# Panoramica sul bilanciamento dei carichi di lavoro {#workload-balancer-overview}

>[!CONTEXTUALHELP]
>id="wf-resourcing-workload-balancer"
>title="Bilanciatore dei carichi di lavoro"
>abstract="I proprietari dei progetti e i manager del team possono utilizzare il bilanciamento del carico di lavoro per assegnare elementi di lavoro agli utenti."

<!--
<p>(NOTE: this is linked from the UI for the Workload Balancer page. DO NOT CHANGE TITLE OR LINK) </p>
-->

Dopo che i project manager hanno pianificato il lavoro sui progetti creando attività e dopo che i manager delle risorse hanno allocato le risorse delle mansioni ai progetti nella pianificazione risorse, i manager del team e i proprietari dei progetti possono utilizzare il bilanciamento dei carichi di lavoro per assegnare gli elementi di lavoro agli utenti.

>[!IMPORTANT]
>
>Puoi utilizzare il bilanciamento dei carichi di lavoro per assegnare il lavoro effettivo (attività e problemi) agli utenti.
>
>Devi utilizzare la pianificazione risorse e non il bilanciamento dei carichi di lavoro per stimare le allocazioni delle mansioni per i progetti, a un alto livello. Per ulteriori informazioni sulla pianificazione risorse, consulta [Panoramica sulla pianificazione risorse](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

Questo articolo descrive lo scopo generale del bilanciamento dei carichi di lavoro e alcune delle best practice per configurare progetti e risorse per utilizzarli correttamente.

Per rivedere i video tutorial del bilanciamento dei carichi di lavoro, passa alla pagina [Tutorial di Workfront](https://experienceleague.adobe.com/it/docs/workfront-learn/tutorials-workfront/home). Nel menu a sinistra, seleziona **Gestisci le risorse** > **Bilanciamento dei carichi di lavoro** e scegli un tutorial.

## Individuare il bilanciamento dei carichi di lavoro

<!--
<p>(NOTE: This will be taken out when all we will have is one tool - should be replaced by a blurb that says you can add this tool anywhere, in any custom tab, etc (long term dev promise)) </p>
-->

È consigliabile utilizzare il bilanciamento dei carichi di lavoro nelle seguenti aree per pianificare le risorse:

* A livello di sistema, nell’area Gestione risorse.
* A livello di progetto, nella sezione Bilanciamento dei carichi di lavoro di un progetto.
* A livello di team, nella sezione Bilanciamento dei carichi di lavoro di un team.

Per ulteriori informazioni sull’individuazione del bilanciamento dei carichi di lavoro, consulta [Individuare il bilanciamento dei carichi di lavoro](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

## Vantaggi del bilanciamento dei carichi di lavoro

Quando utilizzi il bilanciamento dei carichi di lavoro, considera i seguenti vantaggi:

<!--
<p> Add about the what-if scenarios as a benefit when they become available </p>
-->

* Accedere a una chiara mappatura visiva dell’allocazione eccessiva e del sottoutilizzo delle risorse che sia trasparente per tutti gli stakeholder.
* In qualità di people manager, puoi proteggere le persone dal burnout e consentire loro di svolgere il proprio lavoro al meglio con maggiore concentrazione, qualità e coinvolgimento. Puoi garantirne l’utilizzo completo, suddividere i silos e consentire l’allineamento del lavoro tra i team.
* Quando assegni il lavoro a livello di attività o di problema, non puoi vedere quanto un utente è occupato. Quando utilizzi il bilanciamento dei carichi di lavoro, puoi visualizzare quali utenti hanno disponibilità nel loro carico di lavoro per completare l’attività o il problema in tempo. Questo include i dettagli relativi alla non disponibilità e alle eccezioni di pianificazione.

  Per ulteriori informazioni, consulta [Panoramica sull’assegnazione del lavoro nel bilanciamento dei carichi di lavoro](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

  Inoltre, è possibile assegnare elementi di lavoro in blocco, semplificando così la distribuzione di più elementi di lavoro contemporaneamente in più progetti. Per ulteriori informazioni, consulta [Assegnare il lavoro in blocco utilizzando il bilanciamento dei carichi di lavoro](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md).

* I dirigenti possono prendere decisioni tempestive in materia di gestione del personale attraverso la trasparenza delle modalità di utilizzo delle persone all’interno dell’organizzazione.
* I membri del team traggono vantaggio da una migliore collaborazione, in quanto possono tutti visualizzare su cosa stanno lavorando i colleghi in un determinato momento. Per informazioni sull’accesso necessario per visualizzare o gestire risorse nel bilanciamento dei carichi di lavoro, consulta [Accesso necessario per gestire le risorse nel bilanciamento dei carichi di lavoro](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).
* Per condividerlo con altri utenti che non dispongono di Gestione risorse nel menu principale, incorpora un collegamento in una scheda personalizzata. Per informazioni, consulta [Condividere il bilanciamento dei carichi di lavoro tramite un collegamento](../../resource-mgmt/workload-balancer/share-link-for-workload-balancer.md).
* Visualizza e gestisci i carichi di lavoro e la richiesta delle persone in un’unica vista a livello globale, di progetto o di team, a seconda del ruolo. Durante la gestione dei progetti, questo include non solo l’allocazione delle risorse per il progetto, ma anche la visualizzazione dell’allocazione delle risorse da Pianificazione scenari di Adobe Workfront. I people manager utilizzano Pianificazione scenari di Workfront per gestire le competenze professionali in tutta l’organizzazione. La funzione Pianificazione scenari è disponibile solo nella nuova esperienza Adobe Workfront.

  >[!NOTE]
  >
  >  Pianificazione scanari richiede una licenza aggiuntiva. Per informazioni su Pianificazione scenari di Workfront, consulta [Panoramica su Pianificazione scenari](../../scenario-planner/scenario-planner-overview.md).


## Best practice per l’utilizzo del bilanciamento dei carichi di lavoro

Per la pianificazione dei progetti, la configurazione degli utenti e l’utilizzo dei filtri, consigliamo le seguenti best practice prima di iniziare a pianificare le risorse utilizzando il bilanciamento dei carichi di lavoro.

* [Best practice per la visualizzazione delle informazioni nel bilanciamento dei carichi di lavoro](#best-practices-for-displaying-information-in-the-workload-balancer)
* [Best practice per la configurazione degli utenti](#best-practices-for-setting-up-users)
* [Best practice per la configurazione di attività e problemi](#best-practices-for-setting-up-tasks-and-issues)

### Best practice per la visualizzazione delle informazioni nel bilanciamento dei carichi di lavoro {#best-practices-for-displaying-information-in-the-workload-balancer}

È consigliabile utilizzare i filtri in modo da poter visualizzare solo le informazioni pertinenti sia per gli elementi di lavoro non assegnati che per quelli assegnati.

Per informazioni sulla creazione e l’utilizzo dei filtri nel bilanciamento dei carichi di lavoro, consulta [Informazioni sui filtri nel bilanciamento dei carichi di lavoro](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

### Best practice per la configurazione degli utenti

* In qualità di utente che pianifica il lavoro per altri, devi disporre dell’accesso e delle autorizzazioni corrette per pianificare le risorse per il lavoro.

  Per informazioni sull’accesso necessario per gestire il carico di lavoro delle risorse nel Bilanciatore dei carichi di lavoro, consulta [Accesso necessario per gestire le risorse nel Bilanciatore dei carichi di lavoro](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).

* Gli utenti di cui desideri gestire il carico di lavoro devono soddisfare i seguenti criteri in modo che le informazioni sulla loro disponibilità e sulle loro competenze siano accurate:

   * Disporre di pianificazioni e mansioni associate al loro profilo.

     Per ulteriori informazioni sull’associazione di pianificazioni e mansioni agli utenti, consulta [Aggiungere utenti](../../administration-and-setup/add-users/create-and-manage-users/add-users.md)
   * Se un utente non è associato a una pianificazione, la pianificazione predefinita del sistema Workfront viene associata all’utente per impostazione predefinita, ai fini della gestione delle risorse.
   * Avere le eccezioni di pianificazione aggiornate nelle loro pianificazioni.

     Per ulteriori informazioni sulla creazione di pianificazioni, consulta [Creare una pianificazione](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)

   * Avere il calendario delle indisponibilità aggiornato nel loro profilo.

     Per informazioni sull’aggiornamento del calendario delle indisponibilità di un utente, consulta [Configurare l’indisponibilità personale](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

     <!--   
     <div data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     <p>(NOTE: Add another bullet for Costs, when this becomes available:</p>   
     <p>If you want to budget your resources by Cost, you must associate Job Roles with Cost/ Hr. rates. The cost associated with Job Roles assigned to users in your Resource Pools is used to calculate the Budgeted Labor Cost and the Budgeted Cost of the project.For more information about associating job roles with rates, see the article Creating and Managing Job Roles in the new Adobe Workfront experience.For more information about calculating Budgeted Labor Cost, see the article Calculating Budgeted Labor Cost in the new Adobe Workfront experience.For more information about calculating Budgeted Cost, see the article Calculating Budgeted Cost in .) </p>   
     </div>   
     -->

* L’amministratore di Workfront deve determinare il modo in cui Workfront calcola la disponibilità degli utenti. Può decidere se Workfront utilizza la pianificazione predefinita del sistema o la pianificazione dell’utente per calcolare il tempo in cui l’utente è disponibile a lavorare modificando le preferenze di Gestione risorse nell’area Configurazione di Workfront.

  Per ulteriori informazioni, consulta [Configurare le preferenze di gestione delle risorse](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

### Best practice per la configurazione di attività e problemi {#best-practices-for-setting-up-tasks-and-issues}

Prima di iniziare ad assegnare il lavoro agli utenti nel Bilanciatore dei carichi di lavoro, assicurati che sia presente la seguente configurazione per attività e problemi:

* Le attività principali non sono assegnate a utenti o ruoli. Le attività principali non vengono visualizzate nel Bilanciatore dei carichi di lavoro.
* Le attività e i problemi hanno un valore per Ore pianificate maggiore di zero.

* Le attività e i problemi hanno un valore per Durata maggiore di zero.
* Le Date pianificate dei problemi rientrano nella timeline del progetto.

## Prima di iniziare a utilizzare il Bilanciatore dei carichi di lavoro

* Rivedi i seguenti articoli prima di iniziare a utilizzare il Bilanciatore dei carichi di lavoro:

   * Questo articolo illustra come navigare nel Bilanciatore dei carichi di lavoro per eseguire le seguenti azioni: [Navigare nel Bilanciatore dei carichi di lavoro](../workload-balancer/navigate-the-workload-balancer.md).

   * I seguenti articoli descrivono come assegnare lavoro e gestire le allocazioni utente:

      * [Panoramica sull’assegnazione del lavoro nel Bilanciatore dei carichi di lavoro](../workload-balancer/assign-work-in-workload-balancer.md).
      * [Gestire le allocazioni degli utenti nel Bilanciatore dei carichi di lavoro](../workload-balancer/manage-user-allocations-workload-balancer.md).

* Il Bilanciatore dei carichi di lavoro è disponibile in diverse aree di Workfront. Per informazioni su dove trovare il Bilanciatore dei carichi di lavoro, consulta [Individuare il Bilanciatore dei carichi di lavoro](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

## Accesso necessario per utilizzare il Bilanciatore dei carichi di lavoro

Per poter visualizzare e utilizzare il Bilanciatore dei carichi di lavoro in Workfront, devi disporre dell’accesso e delle autorizzazioni Workfront corrette per progetti specifici. Per informazioni sull’accesso necessario per utilizzare il Bilanciatore dei carichi di lavoro, consulta l’articolo [Accesso necessario per gestire le risorse nel Bilanciatore dei carichi di lavoro](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).
