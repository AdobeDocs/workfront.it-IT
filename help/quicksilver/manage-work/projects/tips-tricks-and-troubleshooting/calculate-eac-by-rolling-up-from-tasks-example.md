---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: 'Esempio di calcolo: calcolare EAC come rollup dalle attività'
description: Questo articolo fornisce un esempio di calcolo della stima al completamento (CES) di un progetto sotto forma di riepilogo da tutte le attività del progetto in Adobe Workfront.
author: Lisa
feature: Work Management
exl-id: 68b582c9-f72a-4000-9d28-f7dafa23541f
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '1134'
ht-degree: 2%

---

# Esempio di calcolo: calcolare EAC come rollup dalle attività

## Metodo EAC: eseguire il rollup da attività o sottoattività

* [PIM= Basato su Ore](#pim-hour-based)
* [PIM= Basato su Costo](#pim-cost-based)

### PIM= Basato su Ore {#pim-hour-based}

* [Esempio semplice: il progetto non ha attività secondarie](#simple-example-project-has-no-children-tasks)
* [Esempio complicato: il progetto ha attività figlio](#complicated-example-project-has-children-tasks)

#### Esempio semplice: il progetto non ha attività secondarie {#simple-example-project-has-no-children-tasks}

PIM = basato su ore

Metodo EAC = Rollup da attività/sottoattività

1. Crea il Progetto A con tre attività (nessuna attività figlio) tutte assegnate all&#39;Utente 1 il cui costo/ora è pari a $100,00.
1. Aggiungere ore pianificate/effettive a ogni attività e % di completamento in base alla tabella seguente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <br> <p><strong>Attività</strong> </p> </th> 
   <th> <br> <p><strong>Ore pian.</strong> </p> </th> 
   <th> <br> <p><strong>Ore effettive</strong> </p> </th> 
   <th> <p><strong>% completato</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Attività 1</p> </td> 
   <td> <p>5 ore</p> </td> 
   <td> <p>25 ore</p> </td> 
   <td> <p>20%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 2</p> </td> 
   <td> <p>10 ore</p> </td> 
   <td> <p>25 ore</p> </td> 
   <td> <p>30%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 3</p> </td> 
   <td> <p>15 ore</p> </td> 
   <td> <p>25 ore</p> </td> 
   <td> <p>40%</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Ricalcola finanze
1. **CPI per l&#39;attività 1** = 0,04 calcolato come segue:\
   **IPC per l&#39;attività 1** = *IF* Ore effettive > 0 *THEN* IPC = TotalBudgetedCostWorkPerformed/Ore effettive\
   *ELSE* CPI = 1\
   **CPI per l&#39;attività 1** = 1 / 25\
   **CPI per l&#39;attività 1** = 0,04

1. **EAC per l&#39;attività 1** = 125 ore calcolato come segue:\
   **EAC per l&#39;attività 1** = *IF* CPI &lt;> 0 *THEN* EAC = Ore pianificate/ CPI\
   *ALTRO*

   ```
   EAC = Planned  Hours + Actual  Hours
   ```

   **EAC per l&#39;attività 1** = 5 / 04\
   **EAC per l&#39;attività 1** = 125 ore

1. CPI/EAC per le attività 2 e 3 sono:\
   Attività 2 = 0,12 / 83,33 ore\
   Attività 3 = 0,24 / 62,5 ore

1. **CPI per il progetto** = 0,13 calcolato come segue:\
   **CPI per il progetto** = *IF* Ore effettive > 0 *THEN*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* CPI = 1
   **CPI per il progetto** = 10 / 75\
   **CPI per il progetto** = 0,13

1. **EAC per il progetto** = 270,83 ore calcolato come segue\
   **EAC per il progetto** = EAC Task 1 + EAC Task 2 + EAC Task 3\
   **EAC per il progetto** = 125 + 83,33 + 62,5\
   **EAC per il progetto** = 270,83 ore

#### Esempio complicato: il progetto ha attività figlio {#complicated-example-project-has-children-tasks}

PIM = basato su ore

Metodo EAC = Rollup da attività/sottoattività

1. Creare il Progetto A con sei attività in cui l&#39;Attività 3 è l&#39;attività padre delle Attività 4 e 5 e l&#39;Attività 1 è l&#39;attività padre delle Attività 2 e 3 come illustrato di seguito:\
   Attività 1\
   Attività 2\
   Attività 3\
   Attività 4\
   Attività 5\
   Attività 6

1. Assegnare le attività 2, 4, 5 e 6 all&#39;utente 1 il cui costo/ora è pari a 100,00 $.
1. Aggiungere ore pianificate/effettive per ogni attività e % di completamento in base alla tabella seguente.

   >[!NOTE]
   >
   >Per le Attività 1 e 3 si aggiungono solo le ore effettive.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <br> <p><strong>Attività</strong> </p> </th> 
   <th> <br> <p><strong>Ore pian.</strong> </p> </th> 
   <th> <br> <p><strong>Ore effettive</strong> </p> </th> 
   <th> <p><strong>% completato</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Attività 1</p> </td> 
   <td> </td> 
   <td> <p>10 ore</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 2</p> </td> 
   <td> <p>5 ore</p> </td> 
   <td> <p>10 ore</p> </td> 
   <td> <p>20%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 3</p> </td> 
   <td> </td> 
   <td> <p>10 ore</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 4</p> </td> 
   <td> <p>10 ore</p> </td> 
   <td> <p>10 ore</p> </td> 
   <td> <p>40%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 5</p> </td> 
   <td> <p>15 ore</p> </td> 
   <td> <p>10 ore</p> </td> 
   <td> <p>50%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 6</p> </td> 
   <td> <p>20 ore</p> </td> 
   <td> <p>10 ore</p> </td> 
   <td> <p>60%</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Aggiungere 50 ore direttamente al progetto (Più>Ore>Registra ore) in modo da registrare 5.000,00 $ di costo effettivo della manodopera direttamente nel progetto.
1. Esegui ricalcolo dati finanziari
1. **CPI per l&#39;attività 2** = 0,1 calcolato come segue:\
   **CPI per l&#39;attività 2** = *IF* Ore effettive > 0 *THEN*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* CPI = 1
   **CPI per l&#39;attività 2** = 1 / 10\
   **CPI per l&#39;attività 2** = 0,1

1. **EAC per l&#39;attività 2** = 50 ore calcolato come segue:\
   **EAC per l&#39;attività 2** = *IF* CPI &lt;> 0 *THEN*

   ```
   EAC = Planned Hours / CPI
   ```

       *ELSE* EAC = ore pianificate + ore effettive
   **EAC per l&#39;attività 2** = 5 / 0,1\
   **EAC per l&#39;attività 2** = 50 ore

1. CPI/EAC per i task 4, 5 e 6:\
   Attività 4 = 0,4 / 25 ore\
   Attività 5 = 0,75 / 20 ore\
   Attività 6 = 1,2 / 16,67 ore

1. **CPI per l&#39;attività 3** = 0,38\
   **CPI per l&#39;attività 3** = *IF* Ore effettive > 0 *THEN*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* CPI = 1
   **CPI per l&#39;attività 3** = 11,5 / 30\
   **CPI per l&#39;attività 3** = 0,38

1. **EAC per l&#39;attività 3** = EAC attività 4 + EAC attività 5\
   **EAC per l&#39;attività 3** = 25 + 20\
   **EAC per l&#39;attività 3** = 45 ore

1. **CPI per l&#39;attività 1** = 0,25 calcolato come segue:\
   **CPI per l&#39;attività 1** = *IF* Ore effettive > 0 *THEN*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* CPI = 1
   **CPI per l&#39;attività 1** = 12,5 / 50\
   **CPI per l&#39;attività 1** = 0,25

1. **EAC per l&#39;attività 1** = EAC attività 2 + EAC attività 3\
   **EAC per l&#39;attività 1** = 50 + 45\
   **EAC per l&#39;attività 1** = 95 ore

1. CPI per progetto = 0,22 calcolato come segue:\
   **CPI per il progetto** = *IF* Ore effettive > 0 *THEN*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* CPI = 1
   **CPI per il progetto** = 24,5 / 110\
   **CPI per il progetto** = .22272\
   **CPI per il progetto** = 0,22

1. **EAC per il progetto** = EAC Task 1 + EAC Task 6\
   **EAC per il progetto** = 95 + 16,67\
   **EAC per il progetto** = 111,67 ore

### PIM= Basato su Costo {#pim-cost-based}

* [Esempio semplice: il progetto non ha attività secondarie](#simple-example-project-has-no-children-tasks)

#### Esempio semplice: il progetto non ha attività secondarie {#simple-example-project-has-no-children-tasks-1}

PIM = Basato su Costo

Metodo EAC = Rollup da attività/sottoattività

1. Crea il Progetto A con tre attività (nessuna attività figlio) tutte assegnate all&#39;Utente 1 il cui costo/ora è pari a $100,00.
1. Aggiungere ore pianificate/effettive a ogni attività e % di completamento in base alla tabella seguente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <br> <p><strong>Attività</strong> </p> </th> 
   <th> <br> <p><strong>Ore pian.</strong> </p> </th> 
   <th> <br> <p><strong>Costo Lav Pian</strong> </p> </th> 
   <th> <br> <p><strong>Ore effettive</strong> </p> </th> 
   <th> <br> <p><strong>Costo Lav Reale</strong> </p> </th> 
   <th> <p><strong>% completato</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Attività 1</p> </td> 
   <td> <p>5 ore</p> </td> 
   <td> <p>500,00 $</p> </td> 
   <td> <p>25 ore</p> </td> 
   <td> <p>2.500,00 $</p> </td> 
   <td> <p>20%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 2</p> </td> 
   <td> <p>10 ore</p> </td> 
   <td> <p>1.000,00 $</p> </td> 
   <td> <p>25 ore</p> </td> 
   <td> <p>2.500,00 $</p> </td> 
   <td> <p>30%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 3</p> </td> 
   <td> <p>15 ore</p> </td> 
   <td> <p>1.500,00 $</p> </td> 
   <td> <p>25 ore</p> </td> 
   <td> <p>2.500,00 $</p> </td> 
   <td> <p>40%</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Aggiungi le spese per ogni attività in base alla tabella seguente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Attività</strong> </p> </th> 
   <th> <p><strong>Spesa</strong> </p> </th> 
   <th> <p><strong>Importo pianificato</strong> </p> </th> 
   <th> <p><strong>Importo effettivo</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Attività 1</p> </td> 
   <td> <p>Task 1 Exp 1</p> </td> 
   <td> <p>300,00 $</p> </td> 
   <td> <p>400,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 1</p> </td> 
   <td> <p>Attività 1 Scad. 2</p> </td> 
   <td> <p>500,00 $</p> </td> 
   <td> <p>0,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 2</p> </td> 
   <td> <p>Scad. attività 2</p> </td> 
   <td> <p>200,00 $</p> </td> 
   <td> <p>100,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 3</p> </td> 
   <td> <p>Scad. attività 3</p> </td> 
   <td> <p>800,00 $</p> </td> 
   <td> <p>700,00 $</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Aggiungere due spese al progetto (non associate a un&#39;attività) nel modo seguente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Spesa</strong> </p> </th> 
   <th> <p><strong>Importo pianificato</strong> </p> </th> 
   <th> <p><strong>Importo effettivo</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Scad. progetto 1</p> </td> 
   <td> <p>1.000,00 $</p> </td> 
   <td> <p>1.500,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 1 Scad. 2</p> </td> 
   <td> <p>2.500,00 $</p> </td> 
   <td> <p>0,00 $</p> </td> 
  </tr> 
 </tbody> 
</table>

1. In base ai valori di cui sopra, i costi sostenuti/non sostenuti sono determinati come segue:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Attività</strong> </p> </th> 
   <th> <p><strong>Spese Pianificate Non Sostenute</strong> </p> </th> 
   <th> <p><strong>Spesa Pianificata Sostenuta</strong> </p> </th> 
   <th> <p><strong>Spese Effettive Sostenute</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Attività 1</p> </td> 
   <td> <p>500,00 $</p> </td> 
   <td> <p>300,00 $</p> </td> 
   <td> <p>400,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 2</p> </td> 
   <td> <p>0,00 $</p> </td> 
   <td> <p>200,00 $</p> </td> 
   <td> <p>100,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 3</p> </td> 
   <td> <p>0,00 $</p> </td> 
   <td> <p>800,00 $</p> </td> 
   <td> <p>700,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Progetto</p> </td> 
   <td> <p>3.000,00 $</p> </td> 
   <td> <p>2.300,00 $</p> </td> 
   <td> <p>2.700,00 $</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Da Azioni progetto, eseguire Ricalcola dati finanziari
1. **CPI****per l&#39;attività 1** = 0,14 calcolato come segue:\
   **CPI****per l&#39;attività 1** = *IF* Costo effettivo manodopera + IncurredActualExpenseCost &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   * ELSE* CPI = CPI_Labor\
     **CPI****per l&#39;attività 1** = (100+300) / (2500+400)\
     **CPI****per l&#39;attività 1** = 400/2900\
     **CPI****per l&#39;attività 1** = 0,14

1. **EAC****per l&#39;attività 1** = $ 13.400,00\
   **Manodopera IPC****per l&#39;attività 1** = SE Costo effettivo manodopera &lt;> 0 THEN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

   ELSE CPI_Labor = 1\
   **Manodopera IPC****per l&#39;attività 1** = 100/2500\
   **Manodopera IPC****per l&#39;attività 1** = 0,04

   **Manodopera EAC****per l&#39;attività 1** = *IF* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   * ELSE* Manodopera EAC = Costo manodopera pianificato + Costo manodopera effettivo\
     **Manodopera EAC****per l&#39;attività 1** = 500.00/.04\
     **Manodopera EAC****per l&#39;attività 1** = $ 12.500,00

   **Spese EAC****per l&#39;attività 1** = IncurredActualExpenseCost + NotIncurredPlannedExpense\
   **Spese EAC****per l&#39;attività 1** = $400,00 + $500,00\
   **Spese EAC****per l&#39;attività 1** = $900,00

   **EAC****per l&#39;attività 1** = Manodopera EAC + Spese EAC\
   **EAC****per l&#39;attività 1** = $ 12.500,00 + $ 900,00\
   **EAC****per l&#39;attività 1** = $ 13.400,00

1. Di seguito sono riportati i valori di CPI/EAC per i task 2 e 3:\
   Attività 2 = 0,19 / 8.433,33 $\
   Attività 3 = 0,44 / 6.950,00 $****

1. CPI per il progetto = 0,32\
   **CPI****per il progetto** = *IF* Costo effettivo manodopera + IncurredActualExpenseCost &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   * ELSE* CPI = CPI_Labor\
     **CPI****per il progetto** = (1000 + 2300) / (7500 + 2700)\
     **CPI****per il progetto** = 3300 / 10200\
     **CPI****per il progetto** = 0,32

1. EAC per il progetto è $28.783,33\
   **EAC****per il progetto** = EAC Task 1 + EAC Task 2 + EAC Task 3\
   **EAC****per il progetto** = $13.400,00 + $8.433,33 + $6.950,00\
   **EAC****per il progetto** = $ 28.783,33
