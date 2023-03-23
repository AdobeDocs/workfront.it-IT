---
product-area: resource-management
navigation-topic: resource-pools
title: Associare pool di risorse a progetti e modelli
description: I pool di risorse sono raccolte di utenti che consentono di gestire le risorse in Adobe Workfront.
author: Alina
feature: Resource Management
exl-id: bbfe8257-ff02-4f06-9763-3f2ae4871c9d
source-git-commit: addcff71ff067be22e9ee80f997af545293fa5db
workflow-type: tm+mt
source-wordcount: '696'
ht-degree: 0%

---

# Associare pool di risorse a progetti e modelli


<!-- drafted for bulk editing projects: keep this in yellow till this releases to ALL customers - May 1, 2023

Also - take out all the references to Preview and Prod at prod final
-->

<span class="preview">Le informazioni evidenziate in questa pagina fanno riferimento a funzionalità non ancora disponibili al pubblico. È disponibile per tutti i clienti nell’ambiente Anteprima e per un gruppo selezionato di clienti nell’ambiente Produzione.</span>


<!--
<p>The sections about how to add resource pools to templates, projects are duplicated from the articles listed in those sections (Editing Projects, Creating a Template, etc).</p>
<p>***I decided to keep these steps here, though, because it's hard to parse through those much lunger articles for just updating this one field.)</p>
-->

I pool di risorse sono raccolte di utenti che consentono di gestire le risorse in Adobe Workfront.

Dopo aver creato i pool di risorse, è possibile associarli a progetti o modelli in modo da poter in un secondo momento eseguire il budget delle risorse sui progetti.

È consigliabile creare in anticipo i pool di risorse, associarli ai progetti e assegnare un budget alle risorse prima dell’avvio del progetto.

Per informazioni sui pool di risorse, consulta [Panoramica dei pool di risorse](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

Per informazioni sulla creazione di pool di risorse, consulta [Creare pool di risorse](../../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

## Requisiti di accesso

Devi disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Pro e superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica l'accesso a Gestione risorse che include l'accesso a Gestione pool di risorse</p> <p>Accesso a progetti, modelli e utenti</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Consente di gestire le autorizzazioni per i progetti, i modelli e gli utenti a cui si associano i pool di risorse</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Associa pool di risorse a un progetto o a un modello

È possibile associare i pool di risorse a un modello nello stesso modo in cui si associano i pool di risorse a un progetto. Questo articolo descrive come associare i pool di risorse ai progetti.

1. Passa a un progetto e fai clic sul pulsante **Altro** icona ![](assets/more-icon.png)accanto al nome del progetto, fai clic su **Modifica**.

1. Fai clic su **Impostazioni progetto**.

1. Inizia a digitare il nome di un pool di risorse nel **Pool di risorse** , quindi selezionalo dall’elenco quando viene visualizzato.\
   È possibile associare più pool di risorse a un progetto o modello.

   ![](assets/nwe-project-settings-in-edit-project-box-350x380.png)

1. Fai clic su **Salva**.

Per ulteriori informazioni su come modificare un progetto e associarlo ai pool di risorse, consulta [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md).

Per ulteriori informazioni su come modificare un modello e associarlo ai pool di risorse, consulta [Modificare i modelli di progetto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

## Associa pool di risorse a diversi progetti o modelli in blocco

È possibile modificare più progetti o modelli in blocco e associare contemporaneamente gli stessi pool di risorse a tutti i progetti.

È possibile associare i pool di risorse ai modelli nello stesso modo in cui si associano i pool di risorse ai progetti.

Per associare pool di risorse a diversi progetti in blocco:

1. Vai a un elenco di progetti.
1. Seleziona più progetti, quindi fai clic sul pulsante **Modifica** icona ![](assets/edit-icon.png) in cima all&#39;elenco.

1. Fai clic su **Impostazioni**.
1. Inizia a digitare il nome di un pool di risorse nel **Pool di risorse** , quindi selezionalo dall’elenco quando viene visualizzato.\
   È possibile associare più pool di risorse a progetti o modelli.

   >[!NOTE]
   >
   >* Nell’ambiente Produzione, quando si modificano in blocco progetti o modelli, in questo campo vengono visualizzati solo i pool di risorse comuni a tutti i progetti o modelli selezionati. Se i progetti selezionati non dispongono di pool di risorse condivise, questo campo sarà vuoto. I pool di risorse qui specificati sovrascriveranno i singoli pool di risorse dei progetti o modelli.
   >
   >* <span class="preview">Nell’ambiente Anteprima, quando si modificano progetti in blocco, è presente un indicatore di &quot;Valori multipli&quot; se i progetti selezionati hanno pool di risorse diversi. Se si aggiungono pool di risorse in blocco, tutti i pool verranno aggiunti al progetto selezionato, sovrascrivendo i pool di risorse originali.</span>


   <span class="preview">![add_resource_pool_to_multiple_projects.png](assets/add-resource-pools-to-multiple-projects-350x358.png)</span>

1. Fai clic su **Salva modifiche**.\
   Quando i pool di risorse sono associati ai progetti o ai modelli, è possibile allocare gli utenti a budget per i progetti all&#39;interno del Planner risorse.\
   Per ulteriori informazioni sul planner risorse, vedere [Panoramica di Resource Planner](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

Per ulteriori informazioni su come modificare progetti in blocco, consulta la sezione &quot;Modifica progetti in blocco&quot; in [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md).

Per ulteriori informazioni su come modificare i modelli in blocco, consulta la sezione &quot;Modificare i modelli in blocco&quot; in [Modificare i modelli di progetto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).
