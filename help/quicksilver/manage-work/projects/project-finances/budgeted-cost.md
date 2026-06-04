---
content-type: reference
product-area: projects
navigation-topic: financials
title: Calcolare il costo preventivato
description: Calcola lo stato di avanzamento del progetto di registrazione dei costi preventivati con un report Utilizzo
author: Lisa
feature: Work Management
exl-id: e96fe38f-58c2-4938-9d2d-81d1109123fa
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/20gQnapiR9T6hm3WCv6-8ymhphOOEcZWqUi-05a4CUU
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 395
ht-degree: 7%

---

# Calcolare il costo preventivato

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
     <td> <p>Portfolio Optimizer</p> <p>Suggerimento: il totale di tutti i valori di Costo preventivato progetto è il Costo preventivato del portfolio.</p> </td> 
    </tr> 
    <tr> 
     <td>Costo preventivato progetto</td> 
     <td>
     <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report (NOTE: this was removed with flash)</p>
      -->
      <p>Report del progetto</p> <p>Rapporto Progetto (Dati finanziari)</p> <p>Report attività</p> <p>Rapporto Issue</p> <p>Report ore preventivate</p> <p>Per ulteriori informazioni sulla creazione di un rapporto, consulta l’articolo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Creare un rapporto personalizzato</a>.</p> </td>
    </tr> 
   </tbody> 
  </table>
