---
product-area: projects;templates
navigation-topic: plan-a-project
title: Designare i responsabili delle risorse per un progetto o un modello
description: È possibile designare Manager risorse per un progetto per indicare chi è responsabile della gestione delle risorse del progetto.
author: Alina
feature: Work Management
exl-id: ae2a89e7-8049-4ee6-9b28-ce247d3f2a6f
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '825'
ht-degree: 0%

---

# Designare i responsabili delle risorse per un progetto o un modello

<!--
<p This article might have to be deleted when the Resource Manager field/ requirement will be forever removed from the system; right now it's still a requirement for Scheduler - January 2023/p>
-->

<!-- remove Prod and Prev references with Prod release - Jan 2023-->

È possibile designare Manager risorse per un progetto per indicare chi è responsabile della gestione delle risorse del progetto. Si tratta di un campo informativo e non è connesso ad alcun strumento di gestione delle risorse.

<!-- drafted for res scheduling deprecation blurb for preview release
Designating Resource Managers for a project is a prerequisite for using the Scheduling tools in Adobe Workfront, in the Production environment.
  
>[!CAUTION]  
>  
>  
> <span class="preview">Some of the information in this article refers to the Adobe Workfront's Scheduling tools. The Scheduling areas have been removed from the Preview environment and will be removed from the Production environment in **January 2023**. </span>  
> <span class="preview"> Instead, you can schedule resources in the Workload Balancer. </span>  
>  
>* <span class="preview"> For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../../resource-mgmt/workload-balancer/workload-balancer.md).</span>  
>  
>* <span class="preview"> For more information about the deprecation and removal of the Scheduling tools, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).</span> 
-->

## Requisiti di accesso

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects and Templates</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions on the project or template</p> 
   
   <p><b>NOTE</b>
   
   Users who are added as Resource Managers to a project or a template immediately gain Manage permissions on the project or the template</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica l’accesso a progetti e modelli</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestisci le autorizzazioni per il progetto o il modello</p>

<p><b>NOTA</b>

Gli utenti che vengono aggiunti come Resource Manager a un progetto o a un modello ottengono immediatamente le autorizzazioni di gestione per il progetto o il modello</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td>
</tr> 
 </tbody> 
</table>

*Per sapere quale piano, tipo di licenza o accesso si dispone, contattare l&#39;amministratore Workfront.

## Considerazioni sui responsabili risorse

>[!NOTE]
>
>Gestione risorse non è un ruolo di lavoro; si tratta di un campo disponibile in un progetto o in un modello che è possibile aggiornare manualmente.

* Puoi designare fino a 30 utenti come responsabili risorse per un singolo progetto o modello.

<!--
* In the Production environment,designating Resource Managers on projects is a prerequisite to allowing users to schedule resources for work on the project when using the Scheduling tools.

  For information about resource scheduling, see [Resource Scheduling](../../../resource-mgmt/resource-scheduling/resource-scheduling-overview.md). 

  <span class="preview">Scheduling tools have been removed from the Preview environment.</span>

* Designating Resource Managers on projects is not a prerequisite to allowing users to schedule resources for work using the Workload Balancer.

  For information about the Workload Balancer, see [Overview of the Workload Balancer](../../../resource-mgmt/workload-balancer/overview-workload-balancer.md). 

 -->

* Non è possibile designare team o gruppi come gestori di risorse. Puoi designare solo gli utenti come gestori di risorse.

* Gli utenti designati come Gestione risorse in un progetto o modello non diventano automaticamente parte del team di progetto.

   Per informazioni sui team di progetto, consulta [Gestione del team del progetto](../../../manage-work/projects/planning-a-project/manage-project-team.md).

* È possibile designare i responsabili risorse per i progetti o per i modelli di progetto. Quando si designano i responsabili risorse in un modello di progetto, tutti gli utenti designati come responsabili risorse nel modello diventano automaticamente responsabili risorse in tutti i progetti creati utilizzando tale modello.
* È possibile visualizzare il campo Gestione risorse nelle aree seguenti:

   * Durante la modifica di un progetto, come descritto in questo articolo.
   * Durante la modifica di un modello, come descritto in questo articolo.
   * Durante la creazione di rapporti di progetto o modello. Per informazioni sulla creazione dei rapporti, vedi [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
   * Durante la creazione o la personalizzazione di una visualizzazione di progetto o modello per un elenco. Per ulteriori informazioni, consulta [Panoramica delle visualizzazioni in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

* È possibile aggiungere o rimuovere rapidamente Gestione risorse su più progetti o modelli aggiungendo il campo Gestione risorse a una visualizzazione di un elenco o di un progetto e modificando il campo utilizzando la modifica in linea.

## Designare i responsabili delle risorse per un progetto

1. Effettua una delle seguenti operazioni:

   * Per aggiungere Gestione risorse a un singolo progetto, passare al progetto in cui si desidera designare uno o più gestori risorse, quindi fare clic sul pulsante **Menu Altro** accanto al nome del progetto, quindi **Modifica .**

   * Per aggiungere Gestione risorse a più progetti contemporaneamente, passare a un elenco di progetti, selezionare i progetti in cui si desidera designare uno o più gestori risorse, quindi fare clic su **Modifica**.

      I gestori risorse esistenti non vengono rimossi dai progetti che si stanno modificando; tutti gli utenti aggiunti in questo modo vengono aggiunti come responsabili risorse al progetto, oltre a tutti i responsabili risorse esistenti.

   * Per aggiungere Gestione risorse a un nuovo progetto, inizia a creare un nuovo progetto.

      Per informazioni sulla creazione di un progetto, consulta [Creare un progetto](../../../manage-work/projects/create-projects/create-project.md).

1. In **Panoramica** nella sezione della finestra di dialogo Modifica progetto fare clic su nella **Gestione risorse** campo .
1. Inizia a digitare il nome dell’utente che desideri aggiungere come gestore delle risorse per il progetto, quindi fai clic sul nome quando viene visualizzato nell’elenco.

   Ripeti questo passaggio per aggiungere più gestori di risorse per il progetto.

1. Fai clic su **Salva modifiche**.

## Designare i responsabili delle risorse per un modello

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront.

1. Fai clic su **Modelli**.

1. Effettua una delle seguenti operazioni:

   * Per aggiungere Gestione risorse a un singolo modello, passare al modello in cui si desidera designare uno o più gestori risorse, quindi fare clic sul pulsante **Menu Altro** accanto al nome del modello, quindi **Modifica .**

   * Per aggiungere contemporaneamente i Resource Manager a più modelli, passare a un elenco di modelli e selezionare i modelli in cui si desidera designare uno o più Resource Manager, quindi fare clic su **Modifica**.

      I gestori di risorse esistenti non vengono rimossi dai modelli che si stanno modificando; tutti gli utenti aggiunti in questo modo vengono aggiunti come responsabili risorse sul modello, oltre a tutti i responsabili risorse esistenti.

   * Per aggiungere Gestione risorse a un nuovo modello, fare clic su **Nuovo modello**, quindi fai clic sul pulsante **Menu Altro** accanto al nome del modello, quindi **Modifica .**

1. In **Panoramica** fai clic su nella sezione **Gestione risorse** campo .
1. Inizia a digitare il nome dell’utente che desideri aggiungere come gestore delle risorse per il modello, quindi fai clic sul nome quando viene visualizzato nell’elenco.

   Ripeti questo passaggio per aggiungere più gestori di risorse al modello.

1. Fai clic su **Salva modifiche**.
