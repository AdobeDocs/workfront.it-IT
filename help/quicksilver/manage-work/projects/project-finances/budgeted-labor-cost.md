---
content-type: reference
product-area: projects
navigation-topic: financials
title: Comprendere i costi del lavoro e le ore previste per i progetti
description: Comprendere i costi del lavoro e le ore previste per i progetti
author: Alina
feature: Work Management
exl-id: 01020bbb-7cf9-4461-b0b6-dcbbc537c616
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1128'
ht-degree: 0%

---

# Comprendere i costi del lavoro e le ore previste per i progetti

<!--
<(NOTE: Keep the structure of this article similar to Calculating Budgeted Cost)</p>
-->

È possibile eseguire il budget delle risorse per il lavoro utilizzando Adobe Workfront Resource Planner.

Man mano che si calcolano le risorse per il lavoro sui progetti, Workfront calcola il costo del lavoro a budget per ruoli, progetti e utenti in base ai valori del costo all&#39;ora.

Il costo del lavoro in budget del planner risorse di un progetto è un calcolo tra il costo associato ai ruoli del job assegnati per completare il lavoro sul progetto e la quantità di ore stimate (ore in budget del planner risorse) che potrebbero richiedere a ogni ruolo di completare il lavoro.

>[!IMPORTANT]
>
>Il costo del lavoro a budget del planner risorse per gli utenti non influisce su quello del progetto. Solo il costo della manodopera per i ruoli di lavoro influisce sul costo del progetto.

## Panoramica del costo del lavoro preventivato per i ruoli e il progetto

Per calcolare il costo del lavoro in budget del progetto, in Workfront viene utilizzato il costo del lavoro in budget dei ruoli del progetto.

>[!TIP]
>
>Il costo del lavoro a budget di un progetto nel Business Case viene visualizzato come Costo del lavoro a budget planner risorse nei report e negli elenchi.

La **Costo manodopera a budget** (o Costo manodopera a budget planner risorse) di un progetto viene calcolato con la seguente formula:

`Resource Planner Budgeted Labor Cost = SUM ( Resource Planner Budgeted Hours for each job role on the project * Cost per Hour rate of each job role on the project)`

I campi utilizzati nel calcolo di cui sopra fanno riferimento ai seguenti elementi:

* Le ore in budget per i ruoli di lavoro nell&#39;area Resource Budgeting del progetto o nel Planner risorse.

   Per ulteriori informazioni sulle risorse di budget nel Planner risorse, vedere la sezione &quot;Risorse di budget nel Planner risorse&quot; nell&#39;articolo [Panoramica di Resource Planner](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

   Per ulteriori informazioni sulle risorse di budget nell&#39;area Resource Budgeting del Business Case, vedere [Risorse di budget nel Business Case](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

* La **Costo per ora di un ruolo di lavoro** nel calcolo di cui sopra si fa riferimento al costo associato a ciascun ruolo di lavoro nel progetto.\
   Per ulteriori informazioni sulla creazione e la gestione dei ruoli di lavoro e sull&#39;associazione di questi con i tassi di costo, vedere l&#39;articolo [Creare e gestire ruoli di lavoro](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

>[!NOTE]
>
>Workfront calcola tutte le informazioni sui costi utilizzando la valuta del progetto. Se si specifica l&#39;orario previsto per le risorse nel Planner risorse, l&#39;opzione per modificare la valuta del progetto è disabilitata.\
>Per ulteriori informazioni sulla modifica della valuta di un progetto, consulta l’articolo [Modificare la valuta del progetto](../../../manage-work/projects/project-finances/change-project-currency.md).

## Panoramica del costo del lavoro preventivato per gli utenti

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Update the following section in the Create a Business Case article, as well, when you update it here.)</p>
-->

>[!IMPORTANT]
>
>Il costo del lavoro a budget utente non influisce sul costo del lavoro a budget del progetto. Solo il costo del lavoro dei ruoli di un progetto influisce sul costo del lavoro a budget del planner risorse del progetto.
> 
>Il totale di tutti i costi di manodopera di tutti gli utenti può corrispondere o meno al costo del lavoro a budget del planner risorse dei ruoli di lavoro associati agli utenti.
>
>Se si stimano gli orari in budget per gli utenti nel Planner risorse, i costi associati sono quelli dei ruoli di lavoro associati agli utenti. Non sono costi associati agli utenti o alle loro tariffe.

Se gli utenti sono associati ai ruoli del progetto e le loro ore sono iscritte in budget nel Planner risorse, il costo del lavoro a budget viene visualizzato con i seguenti nomi, a seconda della posizione in cui vengono visualizzate in Workfront:

* [!UICONTROL **Costo manodopera a budget**]: L&#39;area Resource Budgeting del Business Case sotto i rispettivi ruoli.

   ![](assets/budgeted-labor-cost-for-users-in-business-case-highlighted-350x73.png)

* [!UICONTROL **BDG**]: Planner risorse quando vengono visualizzate le informazioni nella visualizzazione Progetto e Ruolo in base al costo.

   ![](assets/budgeted-labor-cost-for-users-in-rp-project-view-cost--highlighted-350x115.png)

Gli utenti vengono visualizzati nell&#39;area Resource Budgeting del Business Case sotto i rispettivi ruoli o nel Resource Planner se soddisfano i seguenti requisiti:

* Sono associati a uno dei ruoli di lavoro del progetto.
* Sono specificate ore in budget nel planner risorse.
* Hanno un Costo per ora associato al loro profilo.

   Per ulteriori informazioni sull’aggiunta dei tassi di costo per ora agli utenti, consulta l’articolo [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* L’utente fa parte di uno dei pool di risorse associati al progetto.

Il costo del lavoro a budget di un utente viene calcolato dalla seguente formula:

`User Budgeted Labor Cost = Budgeted hours for the user on the project * Cost per Hour rate of the user`

## Individuare il costo del lavoro preventivato di un progetto

Il costo del lavoro a budget riportato nell&#39;area Budget risorse del Business Case o del Resource Planner viene visualizzato nelle seguenti aree di Workfront con i seguenti nomi:

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td><strong>Nome visualizzato Costo manodopera a budget</strong></td> 
     <td><strong>Area di Workfront</strong></td> 
    </tr> 
    <tr> 
     <td>Lav Bdg prv</td> 
     <td>Area Budget risorse del Business Case</td> 
    </tr> 
    <tr> 
     <td>Bdg prv</td> 
     <td><p>Rapporto Utilizzo Vista costo</p><p>Per ulteriori informazioni, consulta <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md">Visualizza informazioni sull'utilizzo</a> .</p></td> 
    </tr> 
    <tr> 
     <td>BDG </td> 
     <td>Visualizzazioni Progetto planner risorse o Ruolo, in base al costo</td> 
    </tr> 
    <tr> 
     <td>Costo manodopera in budget progetto planner risorse</td> 
     <td> <p>Rapporto sul progetto</p> <p>Rapporto Progetto (dati finanziari)</p> <p>Rapporto attività</p> <p>Report del problema</p> <p>Rapporto orario previsto</p> <p>Per informazioni sulla creazione di un rapporto, consulta l’articolo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Creare un rapporto personalizzato</a>.</p> </td> 
    </tr> 
   </tbody> 
  </table>

>[!NOTE]
>
>Se si utilizza Adobe Workfront Scenario Planner per preventivare le risorse del progetto, il costo del lavoro a budget nell&#39;area Resource Budgeting del Business Case corrisponde ai costi delle persone dell&#39;iniziativa collegata al progetto. Il planner scenario è disponibile solo nella nuova esperienza Adobe Workfront e richiede una licenza aggiuntiva. Per informazioni su Workfront Scenario Planner, vedi [Panoramica di Scenario Planner](../../../scenario-planner/scenario-planner-overview.md). Per informazioni sulle risorse di budget che utilizzano il Planner scenario, consulta [Risorse di budget nel caso aziendale utilizzando il Planner scenario](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

## Individua le ore previste di un progetto

<!--
(NOTE: Keep the structure of this article similar to Calculating Budgeted Cost)
-->

Le ore in budget influiscono sul valore del costo del lavoro in budget (o del costo budget planner risorse) del progetto.

Il costo del lavoro a budget di un progetto è il costo associato ai ruoli del processo assegnati per completare il lavoro sul progetto e la quantità di ore stimate (ore a budget) che potrebbero richiedere ogni ruolo per completare il lavoro.

È possibile visualizzare le ore previste in Workfront nei campi elencati nella tabella seguente.

>[!NOTE]
>
>Qualsiasi altro riferimento a &quot;Ore previste&quot; in Workfront fa riferimento alle ore inserite in budget utilizzando funzioni obsolete rimosse da Workfront. Si tratta di campi di sola visualizzazione e non vengono aggiornati con le informazioni correnti quando si utilizzano gli strumenti di budget delle risorse correnti.

Le ore inserite in budget nell&#39;area Resource Budgeting del Business Case o nel Resource Planner vengono visualizzate nelle seguenti aree di Workfront e con i seguenti nomi:

* **Ore**: Area Budget risorse del Business Case
* **BDG**:Planner risorse visualizzato in ore
* **Ore previste**: Rapporto Utilizzo Visualizzazione Ore Per informazioni, vedere [Visualizza informazioni sull’utilizzo delle risorse](../../../resource-mgmt/resource-utilization/view-utilization-information.md).
* **Bud. Ore**: Rapporto orario previsto

   L&#39;oggetto Ora a budget nel rapporto Ora a budget fa riferimento a informazioni relative a uno strumento di gestione delle risorse obsoleto. Solo il &quot;Bud&quot;. Il campo Ore in questo rapporto fa riferimento alle ore previste nel budget del Planner risorse o dell&#39;area Budget risorse del Business Case del progetto.

   Per ulteriori informazioni sulla creazione di un rapporto, consulta l’articolo **Creare un rapporto personalizzato**.
* **Orari in budget del planner risorse**: nelle seguenti relazioni:

   * Rapporto sul progetto
   * Rapporto Progetto (dati finanziari)
   * Rapporto attività
   * Report del problema
   * Rapporto orario previsto
