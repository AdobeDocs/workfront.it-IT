---
content-type: reference
product-area: projects
navigation-topic: financials
title: Comprendere il costo manodopera preventivato e le ore preventivate per i progetti
description: Comprendere il costo manodopera preventivato e le ore preventivate per i progetti
author: Lisa
feature: Work Management
exl-id: 01020bbb-7cf9-4461-b0b6-dcbbc537c616
source-git-commit: 6afa65f921864403c10541d283ef717dce81aed7
workflow-type: tm+mt
source-wordcount: '1128'
ht-degree: 0%

---

# Comprendere il costo manodopera preventivato e le ore preventivate per i progetti

<!--
<(NOTE: Keep the structure of this article similar to Calculating Budgeted Cost)</p>
-->

È possibile preventivare le risorse per il lavoro utilizzando Adobe Workfront Resource Planner.

Quando si preventivano le risorse per il lavoro sui progetti, Workfront calcola il costo preventivato della manodopera per i ruoli, i progetti e gli utenti in base ai valori del costo orario.

Il costo manodopera preventivata di un progetto per la programmazione delle risorse è un calcolo tra il costo associato alle mansioni assegnate per completare il lavoro sul progetto e la quantità di ore stimate (ore preventivate per la programmazione delle risorse) che possono assumere ogni ruolo per completare il lavoro.

>[!IMPORTANT]
>
>Il Costo manodopera preventivato di Programmazione risorse per gli utenti non influisce su quello del progetto. Solo il costo della manodopera per le mansioni influisce sul costo del progetto.

## Panoramica del costo manodopera preventivato per mansioni e progetto

Workfront utilizza il Costo manodopera preventivato delle mansioni del progetto per calcolare il Costo manodopera preventivato del progetto.

>[!TIP]
>
>Il Costo manodopera preventivato di un progetto nel caso aziendale viene visualizzato come Costo manodopera preventivato di Programmazione risorse nei rapporti e negli elenchi.

Il **Costo manodopera preventivato** (o Costo manodopera preventivato di programmazione risorse) di un progetto viene calcolato con la seguente formula:

`Resource Planner Budgeted Labor Cost = SUM ( Resource Planner Budgeted Hours for each job role on the project * Cost per Hour rate of each job role on the project)`

I campi utilizzati nel calcolo di cui sopra si riferiscono ai seguenti elementi:

* Le ore preventivate per le mansioni nell&#39;area Budget risorse del progetto o Pianificazione risorse.

  Per ulteriori informazioni sulla definizione del budget delle risorse nella Programmazione delle risorse, vedere la sezione &quot;Budgeting Resources in the Resource Planner&quot; nell&#39;articolo [Panoramica sulla programmazione delle risorse](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

  Per ulteriori informazioni sulle risorse budget nell&#39;area Budget risorse del caso aziendale, vedere [Risorse budget nel caso aziendale](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

* La **tariffa oraria di una mansione** nel calcolo precedente si riferisce al costo associato a ciascuna mansione nel progetto.\
  Per ulteriori informazioni sulla creazione e la gestione delle mansioni e sulla loro associazione alle tariffe, vedere l&#39;articolo [Creare e gestire le mansioni](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

>[!NOTE]
>
>Workfront calcola tutte le informazioni sui costi utilizzando la valuta del progetto. Se si specifica Ore preventivate per le risorse nella Programmazione risorse, l&#39;opzione per modificare la divisa del progetto è disabilitata.\
>Per ulteriori informazioni sulla modifica della valuta di un progetto, vedere l&#39;articolo [Modificare la valuta del progetto](../../../manage-work/projects/project-finances/change-project-currency.md).

## Panoramica del costo manodopera preventivato per gli utenti

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Update the following section in the Create a Business Case article, as well, when you update it here.)</p>
-->

>[!IMPORTANT]
>
>Il costo manodopera preventivato utente non influisce sul costo manodopera preventivato del progetto. Solo il costo manodopera delle mansioni di un progetto influisce sul costo manodopera preventivato di Programmazione risorse del progetto.
> 
>Il totale di tutti i costi manodopera di tutti gli utenti può essere uguale o diverso dal costo manodopera preventivato di Programmazione risorse delle mansioni associate agli utenti.
>
>Se si stimano le ore preventivate per gli utenti nella Programmazione risorse, i costi associati a tali ore sono quelli delle mansioni associate agli utenti. Non sono costi associati agli utenti o alle loro tariffe.

Se gli utenti sono associati alle mansioni del progetto e le loro ore sono preventivate nella Programmazione risorse, il Costo manodopera preventivato viene visualizzato con i seguenti nomi, a seconda della posizione in cui vengono visualizzati in Workfront:

* [!UICONTROL **Costo manodopera preventivato**]: area Budget risorse del caso aziendale con i rispettivi ruoli.

  ![](assets/budgeted-labor-cost-for-users-in-business-case-highlighted-350x73.png)

* [!UICONTROL **BDG**]: la pianificazione delle risorse quando vengono visualizzate le informazioni nella visualizzazione Progetto e Ruolo in base al costo.

  ![](assets/budgeted-labor-cost-for-users-in-rp-project-view-cost--highlighted-350x115.png)

Gli utenti vengono visualizzati nell&#39;area Budget risorse del caso aziendale sotto i rispettivi ruoli o nella Programmazione risorse se soddisfano i seguenti requisiti:

* Sono associati a una delle mansioni del progetto.
* Le ore preventivate sono specificate nella Programmazione delle risorse.
* Hanno una Tariffa Costo orario associata al loro profilo.

  Per ulteriori informazioni sull&#39;aggiunta di tariffe Costo orario agli utenti, vedere l&#39;articolo [Modifica profilo utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* L’utente fa parte di uno dei gruppi di risorse associati al progetto.

Il costo manodopera preventivato di un utente viene calcolato con la formula seguente:

`User Budgeted Labor Cost = Budgeted hours for the user on the project * Cost per Hour rate of the user`

## Individuazione del costo manodopera preventivato di un progetto

Il Costo manodopera preventivato riportato nell&#39;area Budget risorse del Business Case o del Programmatore risorse viene visualizzato nelle seguenti aree di Workfront con i seguenti nomi:

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td><strong>Nome visualizzato costo manodopera preventivato</strong></td> 
     <td><strong>Area di Workfront</strong></td> 
    </tr> 
    <tr> 
     <td>Lav Bdg prv</td> 
     <td>Area Budget risorse del Business Case</td> 
    </tr> 
    <tr> 
     <td>Bdg prv</td> 
     <td><p>Rapporto Utilizzo, vista Costo</p><p>Per ulteriori informazioni, vedere <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md">Visualizzare le informazioni sull'utilizzo</a>.</p></td> 
    </tr> 
    <tr> 
     <td>BDG </td> 
     <td>Visualizzazioni Progetto o Ruolo di Programmazione risorse, per Costo</td> 
    </tr> 
    <tr> 
     <td>Costo manodopera preventivato progetto di programmazione risorse</td> 
     <td> <p>Report del progetto</p> <p>Rapporto Progetto (Dati finanziari)</p> <p>Report attività</p> <p>Rapporto Issue</p> <p>Report ore preventivate</p> <p>Per informazioni sulla creazione di un report, vedere l'articolo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Creare un report personalizzato</a>.</p> </td> 
    </tr> 
   </tbody> 
  </table>

>[!NOTE]
>
>Se si utilizza Adobe Workfront Scenario Planner per preventivare le risorse del progetto, il Costo manodopera preventivato nell&#39;area Budget risorse del Business Case corrisponde ai Costi persone dell&#39;iniziativa collegata al progetto. La Pianificazione scenario è disponibile solo nella nuova esperienza Adobe Workfront e richiede una licenza aggiuntiva. Per informazioni su Workfront Scenario Planner, vedere [Panoramica di Scenario Planner](../../../scenario-planner/scenario-planner-overview.md). Per informazioni sull&#39;impostazione del budget delle risorse tramite Scenario Planner, vedere [Risorse budget nel Business Case mediante Scenario Planner](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

## Individuare le ore preventivate di un progetto

<!--
(NOTE: Keep the structure of this article similar to Calculating Budgeted Cost)
-->

Le ore preventivate influiscono sul valore del Costo manodopera preventivato (o Costo preventivato responsabile pianificazione risorse) del progetto.

Il costo manodopera preventivata di un progetto è il costo associato alle mansioni assegnate per completare il lavoro sul progetto e la quantità di ore stimate (ore preventivate) che possono assumere ciascun ruolo per completare il lavoro.

Puoi visualizzare le Ore preventivate in Workfront nei campi elencati nella tabella seguente.

>[!NOTE]
>
>Qualsiasi altra menzione di &quot;Ore preventivate&quot; in Workfront si riferisce alle ore preventivate utilizzando funzioni obsolete che sono state rimosse da Workfront. Si tratta di campi di sola visualizzazione che non vengono aggiornati con le informazioni correnti quando si utilizzano gli strumenti di budgeting delle risorse correnti.

Le ore preventivate nell&#39;area Budget risorse del Business Case o della Programmazione risorse vengono visualizzate nelle seguenti aree di Workfront e sotto i seguenti nomi:

* **Ore**: area Budget risorse del Business Case
* **BDG**:Pianificazione risorse visualizzata per ore
* **Ore preventivate**: visualizzazione ore report di utilizzo
Per informazioni, vedere [Visualizzare le informazioni sull&#39;utilizzo delle risorse](../../../resource-mgmt/resource-utilization/view-utilization-information.md).
* **Bud Ore**: rapporto Ore preventivate

  L&#39;oggetto Ora preventivata nel rapporto Ore preventivate fa riferimento a informazioni relative a uno strumento di gestione delle risorse obsoleto. Solo il &quot;Bud. Il campo &quot;Ore&quot; in questo rapporto si riferisce alle ore preventivate nella Programmazione delle risorse o nell&#39;area Budget risorse del Business Case del progetto.

  Per ulteriori informazioni sulla creazione di un report, vedere l&#39;articolo **Creare un report personalizzato**.
* **Ore preventivate programmazione risorse**: nei seguenti rapporti:

   * Report del progetto
   * Rapporto Progetto (Dati finanziari)
   * Report attività
   * Rapporto Issue
   * Report ore preventivate
