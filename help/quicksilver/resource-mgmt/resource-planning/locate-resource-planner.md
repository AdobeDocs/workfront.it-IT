---
product-area: resource-management
navigation-topic: resource-planning
title: Individuare la pianificazione risorse
description: È possibile utilizzare la Programmazione delle risorse per gestire l'allocazione delle risorse ai progetti. È possibile accedere alla pianificazione risorse per più progetti contemporaneamente o per un progetto dall'area Caso di business del progetto.
author: Lisa
feature: Resource Management
exl-id: 0de749df-5af9-4124-8539-06b82dca2ec4
TQID: https://experienceleague.adobe.com/-p17GWsoDlmbZtZW3T47YGxOmgSOsMddnFfFXpW36C4
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2:
  - id: d1573eb8-a2e8-4a06-9526-9c3410bf4914
  - id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 461
ht-degree: 9%

---

# Individuare la pianificazione risorse

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(This came off this article: draft that content in the article when this comes live: /Content/Resource Mgmt/Resource Planning/get-started-resource-planner.html)</p>
-->

È possibile utilizzare la Programmazione delle risorse per gestire l&#39;allocazione delle risorse ai progetti. È possibile accedere alla pianificazione risorse per più progetti contemporaneamente o per un progetto dall&#39;area Caso di business del progetto.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacchetto Adobe Workfront</td> 
   <td><p>Qualsiasi</p></td>
  </tr> 
  <tr> 
   <td>Licenza di Adobe Workfront</td> 
   <td><p>Leggero o superiore per un progetto; standard per più progetti</p>
       <p>Revisione o successiva per un progetto; pianificazione per più progetti</p></td>
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td> <p>Accesso di visualizzazione o superiore a Gestione risorse</p> </td> 
  </tr> 
  <tr> 
   <td>Autorizzazioni sugli oggetti</td> 
   <td> <p>Visualizzare le autorizzazioni per progetti e utenti </p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

Prima di iniziare a utilizzare la pianificazione risorse, assicurati che siano soddisfatti tutti i prerequisiti per accedere e lavorare con essa. In questo modo, è possibile assicurarsi che la Programmazione delle risorse visualizzi le informazioni corrette prima di iniziare a definire il budget delle risorse.

Per informazioni sui prerequisiti di Pianificazione risorse, vedere [Introduzione alla pianificazione risorse](../../resource-mgmt/resource-planning/get-started-resource-planning.md).

## Individuare la pianificazione risorse

È possibile individuare la Programmazione delle risorse in due aree di Workfront, a seconda che si desideri preventivare le risorse per più progetti o per un solo progetto.

* [Utilizza la pianificazione risorse per più progetti](#use-the-resource-planner-for-multiple-projects)
* [Utilizzare la Programmazione delle risorse per un progetto](#use-the-resource-planner-for-one-project)

### Utilizzare la programmazione delle risorse per più progetti {#use-the-resource-planner-for-multiple-projects}

Quando si utilizza la pianificazione risorse per più progetti, i numeri di allocazione per le risorse rappresentano i numeri per più progetti.

Per accedere alla sezione Planner nell&#39;area Risorse:

{{step1-to-resourcing}}

Il Planner viene visualizzato per impostazione predefinita.  Per informazioni sulla definizione del budget delle risorse nella Programmazione delle risorse, vedere l&#39;articolo [Risorse preventivo nella Programmazione delle risorse utilizzando le visualizzazioni Progetto e Ruolo](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

![Pianificazione risorse predefinita](assets/qs-resource-management-area-with-planner-as-default-350x152.png)

1. Fai clic su **Pool di Risorse** nel pannello a sinistra.
Per informazioni sulla creazione dei pool di risorse, vedere [Creare i pool di risorse](../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

### Utilizzare la Programmazione delle risorse per un progetto {#use-the-resource-planner-for-one-project}

Quando si utilizza la pianificazione risorse per un progetto, i numeri di allocazione per le risorse rappresentano i numeri per il progetto selezionato.

1. Vai a un progetto per il quale vuoi preventivare le risorse.
1. Fai clic su **Business Case** nel pannello a sinistra.
1. Scorri fino alla sezione **Budget risorse** del Business Case.
1. Fai clic su **Modifica budget risorse** per aggiungere gruppi di risorse al progetto e iniziare a pianificare le risorse.

   >[!TIP]
   >
   >È possibile aggiungere un gruppo di risorse nell&#39;area Budget risorse del Business Case solo se al progetto non è associato alcun gruppo di risorse. Quando il progetto ha già un Pool di Risorse, gli utenti nel pool e le loro mansioni vengono visualizzati nell&#39;area Budget risorse per impostazione predefinita.

   ![Impostazione budget risorse](assets/resource-budgeting-area-on-project-350x70.png)

   Per informazioni sulla definizione del budget delle risorse per un progetto, vedere l&#39;articolo [Risorse budget nel caso aziendale](../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).
