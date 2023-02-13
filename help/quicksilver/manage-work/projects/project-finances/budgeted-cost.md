---
content-type: reference
product-area: projects
navigation-topic: financials
title: Calcola costo preventivato
description: Calcola l'avanzamento del progetto CostTracking a budget con un rapporto di utilizzo""
author: Alina
feature: Work Management
exl-id: e96fe38f-58c2-4938-9d2d-81d1109123fa
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 2%

---

# Calcola costo preventivato

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: This article is linked from "Tracking Project Progress with a Utilization Report"</p>
<p>Keep the structure of this article similar to Calculating Budgeted Labor Cost)</p>
</div>
-->

Il costo preventivato di un progetto è il costo totale associato al progetto come stimato al momento della pianificazione del progetto.

## Panoramica del costo preventivato in un progetto

Non è possibile modificare manualmente il costo preventivato di un progetto. Adobe Workfront calcola il costo in budget utilizzando la seguente formula:

`Budgeted Cost = Resource Planner Budgeted Labor Cost + Budgeted Expenses Cost + Fixed Cost of the project`

* La **Costo manodopera a budget planner risorse** nel calcolo di cui sopra è il costo associato ai ruoli del lavoro nel progetto.

   È possibile tenere traccia del costo del lavoro preventivato di un progetto nell&#39;area Budget risorse del Business Case o del Resource Planner.

   >[!TIP]
   >
   >  Il costo del lavoro a budget di un progetto nel Business Case viene visualizzato come Costo del lavoro a budget planner risorse nei report e negli elenchi.

   Per informazioni sui costi del lavoro a budget, vedere l&#39;articolo [Comprendere i costi del lavoro e le ore previste per i progetti](../../../manage-work/projects/project-finances/budgeted-labor-cost.md).

* La **Costo spese in budget** nel calcolo di cui sopra è riportato il costo pianificato associato alle spese del progetto, come calcolato nell&#39;area Spese del Business Case o nella scheda Spese del progetto.\
   Per ulteriori informazioni sulle spese per un progetto, consulta l’articolo [Gestione delle spese di progetto](../../../manage-work/projects/project-finances/manage-project-expenses.md).

* La **Costo fisso** nel calcolo di cui sopra è l&#39;importo fisso associato al costo del progetto, come definito nell&#39;area Finanze della sezione Dettagli del progetto.\
   Per ulteriori informazioni sulla sottoscheda Finanza di un progetto, consulta l’articolo [Gestire le informazioni nell&#39;area di finanziamento del progetto](../../../manage-work/projects/project-finances/manage-project-finance-area.md).

>[!NOTE]
>
>Workfront calcola tutte le informazioni sui costi utilizzando la valuta del progetto. Se si specifica l&#39;orario previsto per le risorse nel Planner risorse, l&#39;opzione per modificare la valuta del progetto è disabilitata.
>
>Per ulteriori informazioni sulla modifica della valuta di un progetto, consulta l’articolo [Modificare la valuta del progetto](../../../manage-work/projects/project-finances/change-project-currency.md).

## Individuare il costo preventivato di un progetto

Il costo preventivato riportato nell&#39;area Budget risorse del Business Case o del Resource Planner viene visualizzato nelle seguenti aree di Workfront con i seguenti nomi:

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td><strong>Nome visualizzato Costo preventivato</strong></td> 
     <td><strong>Area di Workfront</strong></td> 
    </tr> 
    <tr> 
     <td>Bdg prv</td> 
     <td> <p>Riassunto del Business Case</p> <p> <img src="assets/business-case-summary-qs-350x453.png" style="width: 350;height: 453;"> </p> </td> 
    </tr> 
    <tr> 
     <td>Costo</td> 
     <td> <p>Ottimizzatore Portfolio</p> <p>Suggerimento: Il totale di tutti i valori di Costo preventivato del progetto è il Costo preventivato del portafoglio.</p> </td> 
    </tr> 
    <tr> 
     <td>Costo preventivato progetto</td> 
     <td> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report (NOTE: this was removed with flash)</p>
      --> <p>Rapporto sul progetto</p> <p>Rapporto Progetto (dati finanziari)</p> <p>Rapporto attività</p> <p>Report del problema</p> <p>Rapporto orario previsto</p> <p>Per ulteriori informazioni sulla creazione di un rapporto, consulta l’articolo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Creare un rapporto personalizzato</a>.</p> </td> 
    </tr> 
   </tbody> 
  </table>
