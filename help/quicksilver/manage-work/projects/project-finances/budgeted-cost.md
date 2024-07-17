---
content-type: reference
product-area: projects
navigation-topic: financials
title: Calcola costo preventivato
description: Calcola lo stato di avanzamento del progetto di traccia dei costi preventivati con un rapporto Utilizzo""
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

Il costo preventivato di un progetto è il costo totale associato al progetto, stimato al momento della pianificazione del progetto.

## Panoramica sui costi preventivati in un progetto

Non è possibile modificare manualmente il Costo preventivato di un progetto. Adobe Workfront calcola il costo preventivato utilizzando la formula seguente:

`Budgeted Cost = Resource Planner Budgeted Labor Cost + Budgeted Expenses Cost + Fixed Cost of the project`

* Il **Costo manodopera preventivato per la programmazione delle risorse** nel calcolo di cui sopra è il costo associato alle mansioni nel progetto.

  È possibile tenere traccia del Costo manodopera preventivato di un progetto nell&#39;area Budget risorse del Business Case o della Programmazione risorse.

  >[!TIP]
  >
  >  Il Costo manodopera preventivato di un progetto nel caso aziendale viene visualizzato come Costo manodopera preventivato di Programmazione risorse nei rapporti e negli elenchi.

  Per informazioni sui costi manodopera preventivati, vedere l&#39;articolo [Comprendere il costo manodopera preventivato e le ore preventivate per i progetti](../../../manage-work/projects/project-finances/budgeted-labor-cost.md).

* Il **Costo spese preventivate** nel calcolo riportato sopra è il Costo pianificato associato alle spese del progetto, in quanto vengono calcolate nell&#39;area Spese del Business Case o nella scheda Spese del progetto.\
  Per ulteriori informazioni sulle spese di un progetto, vedere l&#39;articolo [Gestione delle spese del progetto](../../../manage-work/projects/project-finances/manage-project-expenses.md).

* Il **Costo fisso** nel calcolo di cui sopra è l&#39;importo fisso associato al Costo del progetto, come definito nell&#39;area Finanze della sezione Dettagli del progetto.\
  Per ulteriori informazioni sulla scheda secondaria Finanza di un progetto, vedere l&#39;articolo [Gestire le informazioni nell&#39;area Finanza del progetto](../../../manage-work/projects/project-finances/manage-project-finance-area.md).

>[!NOTE]
>
>Workfront calcola tutte le informazioni sui costi utilizzando la valuta del progetto. Se si specifica Ore preventivate per le risorse nella Programmazione risorse, l&#39;opzione per modificare la divisa del progetto è disabilitata.
>
>Per ulteriori informazioni sulla modifica della valuta di un progetto, vedere l&#39;articolo [Modificare la valuta del progetto](../../../manage-work/projects/project-finances/change-project-currency.md).

## Individuazione del costo preventivato di un progetto

Il Costo preventivato riportato nell&#39;area Budget risorse del Business Case o della Programmazione risorse viene visualizzato nelle seguenti aree di Workfront con i seguenti nomi:

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td><strong>Nome visualizzato costo preventivato</strong></td> 
     <td><strong>Area di Workfront</strong></td> 
    </tr> 
    <tr> 
     <td>Bdg prv</td> 
     <td> <p>Riassunto del Business Case</p> <p> <img src="assets/business-case-summary-qs-350x453.png" style="width: 350;height: 453;"> </p> </td> 
    </tr> 
    <tr> 
     <td>Costo</td> 
     <td> <p>Ottimizzatore Portfolio</p> <p>Suggerimento: il totale di tutti i valori di Costo preventivato progetto è il Costo preventivato del portfolio.</p> </td> 
    </tr> 
    <tr> 
     <td>Costo preventivato progetto</td> 
     <td> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report (NOTE: this was removed with flash)</p>
      --> <p>Report del progetto</p> <p>Rapporto Progetto (Dati finanziari)</p> <p>Report attività</p> <p>Rapporto Issue</p> <p>Report ore preventivate</p> <p>Per ulteriori informazioni sulla creazione di un report, vedere l'articolo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Creare un report personalizzato</a>.</p> </td> 
    </tr> 
   </tbody> 
  </table>
