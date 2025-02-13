---
product-area: resource-management
navigation-topic: resource-pools
title: Associa gruppi di risorse a progetti e modelli
description: I pool di risorse sono insiemi di utenti che consentono di gestire le risorse in Adobe Workfront.
author: Lisa
feature: Resource Management
exl-id: bbfe8257-ff02-4f06-9763-3f2ae4871c9d
source-git-commit: a3b2ac192e1f37e0c3d16d059ed96e8d5cadf8be
workflow-type: tm+mt
source-wordcount: '630'
ht-degree: 1%

---

# Associare i pool di risorse a progetti e modelli


<!-- drafted for bulk editing projects: keep this in yellow till this releases to ALL customers - May 1, 2023

Also - take out all the references to Preview and Prod at prod final
-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->


<!--
<p>The sections about how to add resource pools to templates, projects are duplicated from the articles listed in those sections (Editing Projects, Creating a Template, etc).</p>
<p>***I decided to keep these steps here, though, because it's hard to parse through those much lunger articles for just updating this one field.)</p>
-->

I pool di risorse sono insiemi di utenti che consentono di gestire le risorse in Adobe Workfront.

Dopo aver creato i pool di risorse, è possibile associarli ai progetti o ai modelli in modo da poter successivamente preventivare le risorse sui progetti.

È consigliabile creare in anticipo i pool di risorse, associarli ai progetti e preventivare le risorse prima dell&#39;inizio del progetto.

Per informazioni sui pool di risorse, vedere [Panoramica sui pool di risorse](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

Per informazioni sulla creazione di pool di risorse, vedere [Creare pool di risorse](../../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td><p>Nuovo: Qualsiasi</p>
       <p>oppure</p>
       <p>Corrente: Pro o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td><p>Nuovo: Standard</p>
       <p>oppure</p>
       <p>Corrente: Piano</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica l'accesso a Gestione risorse, incluso l'accesso a Gestisci gruppi di risorse</p> <p>Modificare l’accesso a progetti, modelli e utenti</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td>Gestisci le autorizzazioni per i progetti, i modelli e gli utenti a cui vuoi associare i Pool di Risorse</td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Associare i pool di risorse a un progetto o modello

È possibile associare i pool di risorse a un modello nello stesso modo in cui si associano i pool di risorse a un progetto. Questo articolo descrive come associare i pool di risorse ai progetti.

1. Vai a un progetto e fai clic sull&#39;icona **Altro** ![Altro](assets/more-icon.png)accanto al nome del progetto, quindi fai clic su **Modifica**.

1. Fare clic su **Impostazioni progetto**.

1. Inizia a digitare il nome di un pool di risorse nel campo **Pool di risorse**, quindi selezionalo dall&#39;elenco quando viene visualizzato.\
   È possibile associare più pool di risorse a un progetto o modello.

   ![Impostazioni progetto](assets/nwe-project-settings-in-edit-project-box-350x380.png)

1. Fai clic su **Salva**.

Per ulteriori informazioni su come modificare un progetto e associarlo ai pool di risorse, vedere [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md).

Per ulteriori informazioni su come modificare un modello e associarlo ai pool di risorse, vedere [Modifica modelli di progetto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

## Associare in blocco i pool di risorse a più progetti o modelli

È possibile modificare più progetti o modelli in blocco e associare gli stessi pool di risorse a tutti contemporaneamente.

È possibile associare i pool di risorse ai modelli nello stesso modo in cui si associano i pool di risorse ai progetti.

Per associare i pool di risorse a più progetti in blocco:

1. Consente di passare a un elenco di progetti.
1. Seleziona più progetti, quindi fai clic sull&#39;icona **Modifica** ![Modifica](assets/edit-icon.png) nella parte superiore dell&#39;elenco.

1. Fare clic su **Impostazioni**.
1. Inizia a digitare il nome di un pool di risorse nel campo **Pool di risorse**, quindi selezionalo dall&#39;elenco quando viene visualizzato.\
   È possibile associare più pool di risorse ai progetti o ai modelli.

   >[!NOTE]
   >
   >* Quando si modificano i modelli in blocco, in questo campo vengono visualizzati solo i pool di risorse comuni a tutti i modelli selezionati. Se i modelli selezionati non hanno pool di risorse condivisi, questo campo è vuoto. I pool di risorse specificati in questo campo sovrascrivono i singoli pool di risorse dei progetti o dei modelli.
   >
   >* Quando si modificano i progetti in blocco, viene visualizzato un indicatore &quot;Più valori&quot; se i progetti selezionati hanno pool di risorse diversi. Se si aggiungono in blocco gruppi di risorse per i progetti, tutti i gruppi vengono aggiunti al progetto selezionato, sovrascrivendo i gruppi di risorse originali.

   ![aggiungi_pool_di_risorse_a_più_progetti.png](assets/add-resource-pools-to-multiple-projects-350x358.png)

1. Fai clic su **Salva modifiche**.\
   Quando i pool di risorse sono associati ai progetti o ai modelli, è possibile preventivare le allocazioni utente per i progetti all&#39;interno della Programmazione delle risorse.\
   Per ulteriori informazioni sulla Programmazione delle risorse, vedere [Panoramica sulla programmazione delle risorse](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

Per ulteriori informazioni su come modificare i progetti in blocco, vedere la sezione &quot;Modifica progetti in blocco&quot; in [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md).

Per ulteriori informazioni su come modificare i modelli in blocco, vedere la sezione &quot;Modifica modelli in blocco&quot; in [Modifica modelli di progetto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).
