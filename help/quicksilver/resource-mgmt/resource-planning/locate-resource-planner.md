---
product-area: resource-management
navigation-topic: resource-planning
title: Individua il planner risorse
description: '"(Questo è venuto fuori da questo articolo: crea il contenuto nell’articolo quando viene pubblicato: /Content/Resource Management/Resource Planning/get-started-resource-planner.html)'''
author: Alina
feature: Resource Management
exl-id: 0de749df-5af9-4124-8539-06b82dca2ec4
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 0%

---

# Individua il planner risorse

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(This came off this article: draft that content in the article when this comes live: /Content/Resource Mgmt/Resource Planning/get-started-resource-planner.html)</p>
-->

È possibile utilizzare il Planner risorse per gestire l&#39;allocazione delle risorse ai progetti. È possibile accedere al Planner risorse per più progetti contemporaneamente o per un progetto, dall&#39;area Business Case del progetto.

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
   <td> <p>Revisione o superiore<!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        (this seems to be the case in NWE only, not classic. Waiting on Vazgen's response for this)
      </MadCap:conditionalText>
     --></p> <p>Pianifica o superiore per individuare il Planner risorse nell'area globale</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Visualizza accesso o superiore a Gestione risorse</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizzare le autorizzazioni per progetti e utenti </p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Prerequisiti

Assicurati che tutti i prerequisiti per l&#39;accesso e l&#39;utilizzo con il Planner risorse siano soddisfatti prima di iniziare a utilizzarlo. In questo modo, è necessario assicurarsi che il Planner risorse visualizzi le informazioni corrette prima di iniziare a includere in budget le risorse.

Per informazioni sui prerequisiti di Resource Planner, consulta [Guida introduttiva alla pianificazione delle risorse](../../resource-mgmt/resource-planning/get-started-resource-planning.md).

## Individua il planner risorse

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(this was moved from the get-started-resource-planner article)</p>
-->

È possibile individuare il Planner risorse in due aree di Workfront, a seconda che si desideri assegnare il budget alle risorse per più progetti o per un solo progetto.

* [Utilizzare il planner risorse per più progetti](#use-the-resource-planner-for-multiple-projects)
* [Utilizzare il planner risorse per un progetto](#use-the-resource-planner-for-one-project)

### Utilizzare il planner risorse per più progetti {#use-the-resource-planner-for-multiple-projects}

Quando si utilizza il Planner risorse per più progetti, i numeri di allocazione delle risorse rappresentano numeri per più progetti.

Per accedere alla sezione Planner nell&#39;area Origine:

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront.

1. Fai clic su **Risorsa**. Il planner viene visualizzato per impostazione predefinita.  Per informazioni sulle risorse di budget nel Planner risorse, vedere l&#39;articolo [Risorse di budget nel planner risorse utilizzando le visualizzazioni Progetto e Ruolo](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

   ![](assets/qs-resource-management-area-with-planner-as-default-350x152.png)

1. Passa il cursore del mouse sul pannello di sinistra e fai clic su **Pool di risorse**.\
   Per informazioni sulla creazione di pool di risorse, consulta [Creare pool di risorse](../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

### Utilizzare il planner risorse per un progetto {#use-the-resource-planner-for-one-project}

Quando si utilizza il Planner risorse per un progetto, i numeri di allocazione delle risorse rappresentano i numeri per il progetto selezionato.

1. Passa a un progetto per il quale desideri assegnare un budget alle risorse.
1. Fai clic su **Business case** nel pannello a sinistra.
1. Scorri fino a **Budget risorse** sezione del Business Case.
1. Fai clic su **Modifica budget risorse** per aggiungere pool di risorse al progetto e iniziare a impostare il budget per le risorse.

   >[!TIP]
   >
   >È possibile aggiungere un pool di risorse solo nell&#39;area Budget risorse del Business Case quando il progetto non dispone di pool di risorse associati. Se il progetto dispone già di un pool di risorse, per impostazione predefinita gli utenti del pool e i relativi ruoli di lavoro vengono visualizzati nell&#39;area di budget risorse.

   ![](assets/resource-budgeting-area-on-project-350x70.png)

   Per informazioni sul budget delle risorse per un progetto, consulta l’articolo [Risorse di budget nel Business Case](../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).
