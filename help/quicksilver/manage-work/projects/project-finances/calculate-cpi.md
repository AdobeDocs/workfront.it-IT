---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcola indice di prestazione dei costi (CPI)
description: L'indice delle prestazioni dei costi (CPI) descrive la relazione a livello di progetto o di task tra il costo pianificato e il costo effettivo. I project manager rivedono questa metrica per identificare le attività o i progetti attualmente monitorati sotto o sopra i costi in un determinato punto.
author: Alina
feature: Work Management
exl-id: 7f2efe26-7292-482d-986c-2d2077a7ca52
source-git-commit: a55041ad5a6cd41cd11ec3ade27bf5227ae0ac47
workflow-type: tm+mt
source-wordcount: '635'
ht-degree: 0%

---

# Calcola indice di prestazione dei costi (CPI)

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.)</p>
-->

L&#39;indice delle prestazioni dei costi (CPI) descrive la relazione a livello di progetto o di task tra il costo pianificato e il costo effettivo. I project manager rivedono questa metrica per identificare le attività o i progetti attualmente monitorati sotto o sopra i costi in un determinato punto. Il costo può essere misurato in ore o in dollari, a seconda del metodo Performance Index (PIM). Per ulteriori informazioni sull&#39;impostazione del metodo dell&#39;indice delle prestazioni, vedere [Impostare il metodo Performance Index (PIM)](../../../manage-work/projects/project-finances/set-pim.md).

Solo le organizzazioni che richiedono l’immissione di tempo possono utilizzare l’IPC. Inoltre, i valori PIM basati sui costi sono accurati solo nelle organizzazioni che hanno definito i tassi di costo per gli assegnatari delle attività (ruoli o utenti).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Revisione o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Accesso a progetti e dati finanziari</p> <p> Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizza o autorizzazioni superiori per il progetto con autorizzazioni per visualizzare Finanza</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Panoramica dell&#39;indice di prestazione dei costi (CPI)

* [Valore CPI](#the-cpi-value)
* [Calcolo dell&#39;IPC](#how-cpi-is-calculated)

### Valore CPI {#the-cpi-value}

I project manager comprendono che un valore CPI pari a 1 significa che il progetto è esattamente in budget. Valori superiori a 1 indicano che un progetto è in budget (sono state registrate meno ore o spese rispetto a quanto originariamente pianificato) e valori inferiori a 1 indicano che un progetto è in budget eccessivo (sono state registrate più ore o spese rispetto a quanto originariamente pianificato). Più lontano da 1, maggiore deviazione dal piano.

| **Valore CPI** | **Indicazione sul bilancio** |
|---|---|
| 1 | Piano o budget |
| > 1 (maggiore di 1) | In bilancio |
| &lt; 1 (inferiore a 1) | Eccesso di bilancio |


### Calcolo dell&#39;IPC {#how-cpi-is-calculated}

In Adobe Workfront, il calcolo per CPI dipende dal metodo di indice delle prestazioni selezionato per il progetto. Per ulteriori informazioni sull&#39;impostazione del metodo dell&#39;indice delle prestazioni, vedere [Impostare il metodo Performance Index (PIM)](../../../manage-work/projects/project-finances/set-pim.md).

* [Calcoli CPI quando si utilizza un PIM basato su ore](#cpi-calculations-when-using-hour-based-pim)
* [Calcoli CPI quando si utilizza un PIM basato sui costi](#cpi-calculations-when-using-cost-based-pim)

#### Calcoli CPI quando si utilizza un PIM basato su ore {#cpi-calculations-when-using-hour-based-pim}

Se

```
Actual Hours > 0 THEN CPI = Total Budgeted Cost Work Performed / Actual Hours
```

Diversamente

```
CPI = 1
```

* **Per un&#39;attività non padre:**

   ```
   Total Budgeted Cost Work Performed = Planned Hours * (Percent Complete / 100)
   ```

* **Per un&#39;attività padre:**
Lavoro costo totale in budget eseguito = la somma del campo Lavoro costo totale in budget eseguito per tutte le attività figlio dirette.

* **Per un progetto:**
Lavoro costo totale in budget eseguito = la somma del campo Lavoro costo totale in budget eseguito per tutte le attività di primo livello (attività principali e attività standalone).

Per informazioni sul lavoro di costo totale a budget eseguito (BCWP), vedere [Calcola il lavoro dei costi a budget eseguito (BCWP)](../../../manage-work/projects/project-finances/calculate-bcwp.md).

#### Calcoli CPI quando si utilizza un PIM basato sui costi {#cpi-calculations-when-using-cost-based-pim}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>CPI = (Planned Cost of Work Performed + Planned Cost of Incurred Expenses) / (Total Actual Cost + Actual Cost of Incurred Expenses) </code> </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>NOTE: this used to be here before - above - but Anna sent me the one below. I kept the other one, although she is still researching its validity - see this issue: https://hub.workfront.com/issue/5fc7b1cf00012aeebf9e822db8ea2513/overview)</code> </p>
-->

Se

```
Actual Labor Cost + Incurred Actual Expense Cost <> 0 THEN CPI = (Total Budgeted Cost Work Performed + Incurred Planned Expense Cost) / (Actual Labor Cost + Incurred Actual Expense Cost)
```



Diversamente

```
CPI = 1
```

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>(NOTE: above: this used to say: CPI = CPI Labor, but Anna had me fix it on July 21, 2021)</code> </p>
-->

I campi di questo calcolo sono descritti di seguito:

```
Total Actual Cost = Actual (logged) Hours * Hourly Rate of assignees
```

```
Incurred Actual Expense Cost = Actual Cost
```

Spese garantite è la spesa sulla quale il costo effettivo > 0

```
Planned Cost of Incurred Expenses = Total of Planned Cost of all incurred expenses
```



<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Old calculation - taken out by Lilit and replaced below: Planned Cost of Work Performed= (planned labor cost) * (percent complete) / 100 where planned labor cost is the planned hours allocated to assignees * their rates.)</p>
  -->

* Il costo pianificato del lavoro eseguito è calcolato dalla formula seguente:

   ```
   Planned Cost of Work Performed = Planned cost * Percent Complete / 100
   ```

Il lavoro di costo totale a budget eseguito viene calcolato per i seguenti elementi:

* **Per un&#39;attività non padre:**

   ```
   Total Budgeted Cost Work Performed = Planned Labor Cost * Percent Complete / 100
   ```

* **Per un&#39;attività padre:**

   ```
   Total Budgeted Cost Work Performed = SUM(Total Budgeted Cost Work Performed field from all direct child tasks)
   ```

* **Per un progetto:**

   ```
   Total Budgeted Cost Work Performed = SUM(Total Budgeted Cost Work Performed field for all top level tasks)
   ```



## Individuare CPI in un progetto o un&#39;attività

È possibile visualizzare l&#39;indice dei prezzi al consumo di un progetto o di un&#39;attività in un elenco di progetti o task o in un report. Inoltre, è possibile visualizzarlo a livello di progetto o task.

1. Passa al progetto o all’attività in cui desideri visualizzare l’indice dei prezzi al consumo.
1. Espandi **Dettagli progetto** o **Dettagli attività** nel pannello a sinistra, a seconda che visualizzi CPI per un progetto o un’attività.

1. Fai clic su **Finanza**.

   L&#39;IPC viene visualizzato nel **CPI/ SPI/ CSI** campo .

   ![](assets/cpi-on-project-nwe.png)
