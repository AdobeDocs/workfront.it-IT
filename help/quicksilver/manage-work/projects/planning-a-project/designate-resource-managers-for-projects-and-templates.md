---
product-area: projects;templates
navigation-topic: plan-a-project
title: Designare Responsabili risorse per un progetto o un modello
description: È possibile designare Responsabili risorse per un progetto per indicare chi è responsabile della gestione delle risorse del progetto.
author: Alina
feature: Work Management
exl-id: ae2a89e7-8049-4ee6-9b28-ce247d3f2a6f
source-git-commit: 59c3a57e334d1660e3e59da480a90060b1ba81b7
workflow-type: tm+mt
source-wordcount: '826'
ht-degree: 1%

---

# Designare Responsabili risorse per un progetto o un modello

<!--
<p This article might have to be deleted when the Resource Manager field/ requirement will be forever removed from the system; right now it's still a requirement for Scheduler - January 2023/p>
-->

<!-- remove Prod and Prev references with Prod release - Jan 2023-->

È possibile designare Responsabili risorse per un progetto per indicare chi è responsabile della gestione delle risorse del progetto. Questo è un campo informativo e non è connesso ad alcun strumento di gestione delle risorse.

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
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modificare l’accesso a progetti e modelli</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni sul progetto o sul modello</p>

<p><b>NOTA</b>

Gli utenti che vengono aggiunti come Responsabili risorse a un progetto o a un modello ottengono immediatamente le autorizzazioni di gestione sul progetto o sul modello</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l&#39;accesso agli oggetti </a>.</p> </td>
</tr> 
 </tbody> 
</table>

*Per informazioni sulla pianificazione, il tipo di licenza o l&#39;accesso disponibili, contattare l&#39;amministratore Workfront.

## Considerazioni sui Responsabili risorse

>[!NOTE]
>
>Gestione risorse DITA non è una mansione, ma un campo disponibile in un progetto o in un modello che è possibile aggiornare manualmente.

* È possibile designare fino a 30 utenti come Responsabili risorse per un singolo progetto o modello.

<!--
* In the Production environment,designating Resource Managers on projects is a prerequisite to allowing users to schedule resources for work on the project when using the Scheduling tools.

  For information about resource scheduling, see [Resource Scheduling](../../../resource-mgmt/resource-scheduling/resource-scheduling-overview.md). 

  <span class="preview">Scheduling tools have been removed from the Preview environment.</span>

* Designating Resource Managers on projects is not a prerequisite to allowing users to schedule resources for work using the Workload Balancer.

  For information about the Workload Balancer, see [Workload Balancer overview](../../../resource-mgmt/workload-balancer/overview-workload-balancer.md). 

 -->

* Non è possibile designare team o gruppi come responsabili delle risorse. È possibile designare gli utenti solo come responsabili delle risorse.

* Gli utenti designati come Responsabili risorse in un progetto o modello non entrano automaticamente a far parte del team di progetto.

  Per informazioni sui team di progetto, vedere [Gestione del team di progetto](../../../manage-work/projects/planning-a-project/manage-project-team.md).

* Puoi designare i Responsabili risorse per i progetti o per i modelli di progetto. Quando si designano i Responsabili risorse in un modello di progetto, tutti gli utenti designati come Responsabili risorse nel modello diventano automaticamente Responsabili risorse in tutti i progetti creati utilizzando tale modello.
* È possibile visualizzare il campo Responsabile risorse nelle aree seguenti:

   * Durante la modifica di un progetto, come descritto in questo articolo.
   * Durante la modifica di un modello, come descritto in questo articolo.
   * Durante la creazione di report di progetti o modelli. Per informazioni sulla creazione di report, vedere [Creare un report personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
   * Durante la creazione o la personalizzazione di un progetto o di una vista modello per un elenco. Per ulteriori informazioni, vedere [Panoramica delle visualizzazioni in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

* È possibile aggiungere o rimuovere rapidamente Responsabili risorse in più progetti o modelli aggiungendo il campo Responsabile risorse a una visualizzazione di un elenco o di un progetto e modificando il campo tramite la modifica in linea.

## Designare Responsabili risorse per un progetto

1. Effettua una delle seguenti operazioni:

   * Per aggiungere Responsabili risorse a un singolo progetto, passa al progetto in cui desideri designare uno o più responsabili delle risorse, quindi fai clic sul **Altro menu** accanto al nome del progetto, quindi su **Modifica .**

   * Per aggiungere i responsabili risorse a più progetti contemporaneamente, passare a un elenco di progetti, selezionare i progetti in cui si desidera designare uno o più responsabili risorse, quindi fare clic su **Modifica**.

     I Responsabili risorse esistenti non vengono rimossi dai progetti che si stanno modificando; tutti gli utenti aggiunti in questo modo vengono aggiunti come Responsabili risorse nel progetto oltre a eventuali Responsabili risorse esistenti.

   * Per aggiungere Responsabili risorse a un nuovo progetto, inizia a crearne uno nuovo.

     Per informazioni sulla creazione di un progetto, vedere [Creare un progetto](../../../manage-work/projects/create-projects/create-project.md).

1. Nella sezione **Panoramica** della finestra di dialogo Modifica progetto, fare clic nel campo **Gestione risorse DITA**.
1. Inizia a digitare il nome dell’utente che desideri aggiungere come responsabile delle risorse per il progetto, quindi fai clic sul nome quando viene visualizzato nell’elenco.

   Ripeti questo passaggio per aggiungere più gestori di risorse per il progetto.

1. Fai clic su **Salva modifiche**.

## Designare Responsabili risorse per un modello

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **menu principale** nell&#39;angolo superiore destro di Adobe Workfront.

1. Fare clic su **Modelli**.

1. Effettua una delle seguenti operazioni:

   * Per aggiungere Resource Manager a un singolo modello, passare al modello in cui si desidera designare uno o più Resource Manager, quindi fare clic sul **Altro menu** accanto al nome del modello, quindi **Modifica .**

   * Per aggiungere i responsabili risorse a più modelli contemporaneamente, passare a un elenco di modelli e selezionare i modelli in cui si desidera designare uno o più responsabili risorse, quindi fare clic su **Modifica**.

     I Responsabili risorse esistenti non vengono rimossi dai modelli che si stanno modificando; tutti gli utenti aggiunti in questo modo vengono aggiunti come Responsabili risorse nel modello, oltre a eventuali Responsabili risorse esistenti.

   * Per aggiungere i Resource Manager a un nuovo modello, fai clic su **Nuovo modello**, quindi fai clic sul **Altro menu** accanto al nome del modello, quindi su **Modifica .**

1. Nella sezione **Panoramica**, fai clic nel campo **Gestione risorse DITA**.
1. Inizia a digitare il nome dell’utente che desideri aggiungere come responsabile risorse per il modello, quindi fai clic sul nome quando viene visualizzato nell’elenco.

   Ripetere questo passaggio per aggiungere più gestori di risorse al modello.

1. Fai clic su **Salva modifiche**.
