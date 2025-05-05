---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: 'Esempio di calcolo: calcolare EAC a livello di progetto'
description: PIM = basato su ore
author: Alina
feature: Work Management
exl-id: ff88b7e3-2a5b-464f-bed1-6848067840b8
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '2194'
ht-degree: 0%

---

# Esempio di calcolo: calcolare EAC a livello di progetto

## Metodo EAC: calcolo a livello di progetto

* [PIM = basato su ore](#pim-hour-based)
* [PIM= Basato su Costo](#pim-cost-based)

### PIM = basato su ore {#pim-hour-based}

* [Esempio semplice: il progetto non ha attività secondarie](#simple-example-project-has-no-children-tasks)
* [Esempio complicato: il progetto ha attività figlio](#complicated-example-project-has-children-tasks)

#### Esempio semplice: il progetto non ha attività secondarie {#simple-example-project-has-no-children-tasks}

PIM = basato su ore

Metodo EAC = Calcola a livello di progetto **&#x200B;**

1. Crea il Progetto A con tre attività (nessuna attività figlio) tutte assegnate all&#39;Utente 1 il cui costo/ora è pari a $100,00.
1. Aggiungere ore pianificate ed effettive a ogni attività e % di completamento in base alla tabella seguente:

   <table style="table-layout:auto">
    <col>
    <col>
    <col>
    <col>
    <thead>
     <tr>
      <th><br><p><strong>Attività</strong></p></th>
      <th><br><p><strong>Ore pian.</strong></p></th>
      <th><br><p><strong>Lav Real</strong></p></th>
      <th><p><strong>% completamento</strong></p></th>
     </tr>
    </thead>
    <tbody>
     <tr>
      <td><p>Attività 1</p></td>
      <td><p>5 ore</p></td>
      <td><p>25 ore</p></td>
      <td><p>20%</p></td>
     </tr>
     <tr>
      <td><p>Attività 2</p></td>
      <td><p>10 ore</p></td>
      <td><p>25 ore</p></td>
      <td><p>30%</p></td>
     </tr>
     <tr>
      <td><p>Attività 3</p></td>
      <td><p>15 ore</p></td>
      <td><p>25 ore</p></td>
      <td><p>40%</p></td>
     </tr>
    </tbody>
   </table>

1. Ricalcola dati finanziari sul progetto.
1. **CPI per l&#39;attività 1** = 0,04 calcolato come segue:\
   **IPC per l&#39;attività 1** = *IF* Ore effettive > 0 *THEN* IPC = TotalBudgetedCostWorkPerformed/Ore effettive\
      *ELSE* CPI = 1\
   **CPI per l&#39;attività 1** = 1 / 25\
   **CPI per l&#39;attività 1** = 0,04

1. **EAC per l&#39;attività 1** = 125 ore calcolato come segue:\
   **EAC per l&#39;attività 1** = *IF* CPI &lt;> 0 *THEN* EAC = Lavoro Necessario/CPI\
       *ELSE* EAC = Pianificato  Ore + Effettivo  Ore\
   **EAC per l&#39;attività 1** = 5 / 04\
   **EAC per l&#39;attività 1** = 125 ore&#x200B;**&#x200B;**

1. CPI/EAC per le attività 2 e 3 sono:\
   Attività  2 = 0,12 / 83,33  ore\
   Attività 3 = 0,24 / 62,5 ore

1. **CPI per il progetto** = 0,13 calcolato come segue:\
   **IPC per il progetto** = *IF* Ore effettive > 0 *THEN* IPC = TotalBudgetedCostWorkPerformed/Ore effettive\
       *ELSE* CPI = 1\
   **CPI per il progetto** = 10 / 75\
   **CPI per il progetto** = 0,13

1. **EAC per il progetto** = 225 ore calcolato come segue:\
   **EAC per il progetto** = *IF* CPI &lt;> 0 *THEN* EAC = Ore pianificate/CPI\
       *ELSE* EAC = Pianificato  Ore + Effettivo  Ore\
   **EAC per il progetto** = 30 / .13333\
   **EAC per il progetto** = 225 ore

#### Esempio complicato: il progetto ha attività figlio {#complicated-example-project-has-children-tasks}

PIM = basato su ore

Metodo EAC = Calcola a livello di progetto

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
   <td> </td> 
   <td> <p>10 ore</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 2</p> </td> 
   <td> <p>5 ore</p> </td> 
   <td> <p>10 ore</p> </td> 
   <td> <p>20%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 3</p> </td> 
   <td> </td> 
   <td> <p>10 ore</p> </td> 
   <td> </td> 
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

1. Aggiungi 50 ore direttamente al progetto (Altro>Ore>Registra ore).
1. **CPI per l&#39;attività 2** = 0,1 calcolato come segue:\
   **IPC per l&#39;attività 2** = *IF* Ore effettive > 0 *THEN* IPC = TotalBudgetedCostWorkPerformed/Ore effettive\
       *ELSE* CPI = 1\
   **CPI per l&#39;attività 2** = 1 / 10\
   **CPI per l&#39;attività 2** = 0,1

1. **EAC per l&#39;attività 2** = 50 ore calcolato come segue:\
   **EAC per l&#39;attività 2** = *IF* CPI &lt;> 0 *THEN* EAC = Lavoro Necessario/CPI\
       *ELSE* EAC = Pianificato  Ore + Effettivo  Ore\
   **EAC per l&#39;attività 2** = 5 / 0,1\
   **EAC per l&#39;attività 2** = 50 ore

1. L&#39;IPC / EAC per i compiti 4, 5 e 6 è il seguente:\
   Attività 4: 0,4 / 25 ore\
   Attività 5: 0,75 / 20 ore\
   Attività 6: 1,2 / 16,67 ore

1. **CPI per l&#39;attività 3** = 0,38  calcolato come segue:\
   **IPC per l&#39;attività 3** = *IF* Ore effettive > 0 *THEN* IPC = TotalBudgetedCostWorkPerformed/Ore effettive\
       *ELSE* CPI = 1\
   **CPI per l&#39;attività 3** = 11,5 / 30\
   **CPI per l&#39;attività 3** = 0,38

1. **EAC per l&#39;attività 3** = 65,22 ore calcolato come segue:\
   **EAC per l&#39;attività 3** = *IF* CPI &lt;> 0 *THEN* EAC = Lavoro Necessario/CPI\
       *ELSE* EAC = Pianificato  Ore + Effettivo  Ore\
   **EAC per l&#39;attività 3** =  25 / .383333\
   **EAC per l&#39;attività 3** = 65,22 ore

1. **CPI per l&#39;attività 1** = 0,25 calcolato come segue:\
   **IPC per l&#39;attività 1** = *IF* Ore effettive > 0 *THEN* IPC = TotalBudgetedCostWorkPerformed/Ore effettive\
       *ELSE* CPI = 1\
   **CPI per l&#39;attività 1** = 12,5 / 50\
   **CPI per l&#39;attività 1** = 0,25

1. **EAC per l&#39;attività 1** = 120 ore calcolato come segue:\
   **EAC per l&#39;attività 1** = *IF* CPI &lt;> 0 *THEN* EAC = Lavoro Necessario / CPI\
       *ELSE* EAC = Pianificato  Ore + Effettivo  Ore\
   **EAC per l&#39;attività 1** =  30/ 0,25\
   **EAC per l&#39;attività 1** = 120 ore

1. **CPI per il progetto** = 0,22 calcolato come segue:\
   **IPC per il progetto** = *IF* Ore effettive > 0 *THEN* IPC = TotalBudgetedCostWorkPerformed/Ore effettive\
       *ELSE* CPI = 1\
   **CPI per il progetto** = 24,5 / 110\
   **CPI per il progetto** = .22272\
   **CPI per il progetto** = 0,22

1. **EAC per il progetto** = 224,49  ore calcolate come segue:\
   **EAC per il progetto** = *IF* CPI &lt;> 0 *THEN* EAC = Ore pianificate/CPI\
       *ELSE* EAC = Pianificato  Ore + Effettivo  Ore\
   **EAC per il progetto** =  50/22272\
   **EAC per il progetto** = 224,49 ore

### PIM= Basato su Costo {#pim-cost-based}

* [Esempio semplice: il progetto non ha attività secondarie](#simple-example-project-has-no-children-tasks)
* [Esempio complicato: il progetto ha attività figlio](#complicated-example-project-has-children-tasks)

#### Esempio semplice: il progetto non ha attività secondarie {#simple-example-project-has-no-children-tasks-1}

PIM = Basato su Costo

Metodo EAC = Calcola a livello di progetto

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
   <td> <p> 2.700,00 $ <strong></strong></p> </td> 
  </tr> 
 </tbody> 
</table>

1. Da Azioni progetto, eseguire Ricalcola dati finanziari
1. **CPI per l&#39;attività 1** = 0,14
1. **CPI**&#x200B;**per l&#39;attività 1** = 0,14 calcolato come segue:\
   **CPI**  **per l&#39;attività 1** = *IF* Costo effettivo manodopera + IncurredActualExpenseCost  &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   *    ELSE* CPI = CPI_Labor\
   **CPI**&#x200B;**per l&#39;attività 1** = (100+300) / (2500+400)\
   **CPI**  **per l&#39;attività 1** = 400 / 2900\
   **CPI**  **per l&#39;attività 1**  = 0,14&#x200B;**&#x200B;**

1. **EAC**&#x200B;**per l&#39;attività 1** = $ 13.400,00\
   **Manodopera IPC**  **per l&#39;attività 1** = SE Costo effettivo manodopera &lt;> 0 THEN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed/Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **Manodopera IPC**  **per l&#39;attività 1** = 100/2500\
   **Manodopera IPC**  **per l&#39;attività 1** = .04 **&#x200B;**&#x200B;**&#x200B; Manodopera EAC &#x200B;**&#x200B;**per l&#39;attività 1 &#x200B;**=*IF *CPI_Labor &lt;> 0*THEN *Manodopera EAC = Costo manodopera pianificata/CPI_Labor\
   *    ELSE* EAC  Manodopera = Costo manodopera pianificato + Costo manodopera effettivo\
   **Manodopera EAC &#x200B;**&#x200B;**per l&#39;attività 1** = 500.00/.04\
   **Manodopera EAC**&#x200B;**per l&#39;attività 1** = $ 12.500,00\
   **Spese EAC**&#x200B;**per l&#39;attività 1** = IncurredActualExpenseCost + NotIncurredPlannedExpense\
   **Spese EAC**&#x200B;**per l&#39;attività 1** = $400,00 + $500,00\
   **Spese EAC**&#x200B;**per l&#39;attività 1** = $900,00\
   **EAC**&#x200B;**per l&#39;attività 1** = Manodopera EAC + Spese EAC\
   **EAC**&#x200B;**per l&#39;attività 1**  = $12.500,00 + $900,00\
   **EAC**&#x200B;**per l&#39;attività 1**  = $ 13.400,00

1. Di seguito sono riportati i valori di CPI/EAC per i task 2 e 3:\
   Attività 2 = 0,19 / 8.433,33 $\
   Attività 3 = 0,44 / 6.950,00 $

1. **CPI per il progetto** = 0,32 calcolato come segue:\
   **CPI**&#x200B;**per il progetto** = *IF* Costo effettivo manodopera + IncurredActualExpenseCost  &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor\
   **CPI**&#x200B;**per il progetto** = (1000 + 2300) / (7500 + 2700)\
   **CPI**&#x200B;**per il progetto** = 3300 / 10200\
   **CPI**&#x200B;**per il progetto** = 0,32

1. **EAC per il progetto** = $28.200,00 calcolato come segue:\
   **Manodopera IPC**&#x200B;**per il progetto** = SE Costo effettivo manodopera &lt;> 0 THEN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed/Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **Manodopera IPC**&#x200B;**per il progetto** = 1000/7500\
   **Manodopera IPC**&#x200B;**per il progetto** = .13333\
   **Manodopera IPC**&#x200B;**per il progetto** = 0,13

   **Manodopera EAC**&#x200B;**per il progetto** = *IF* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost/CPI_Labor
   ```

   *   ELSE* EAC  Manodopera = Costo manodopera pianificato + Costo manodopera effettivo\
   **Manodopera EAC**&#x200B;**per il progetto** = 3000/ .13333\
   **Manodopera EAC**&#x200B;**per il progetto** = $22.500,00

   **Spese EAC**&#x200B;**Progetto** =

   ```
   IncurredActualExpenseCost + NotIncurredPlannedExpense
   ```

   **Spese EAC**&#x200B;**Progetto** = $3000,00 + 2.700,00\
   **Spese EAC**&#x200B;**Progetto** = $5.700,00

   **EAC**&#x200B;**Progetto** = Manodopera EAC + Spese EAC\
   **EAC**&#x200B;**Progetto**  = $22.500,00 + $5.700,00\
   **EAC**&#x200B;**Progetto**  = 28.200,00 $

#### Esempio complicato: il progetto ha attività figlio {#complicated-example-project-has-children-tasks-1}

PIM = Basato su Costo

Metodo EAC = Calcola a livello di progetto

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
   <td> </td> 
   <td> </td> 
   <td> <p>10 ore</p> </td> 
   <td> <p>1.000,00 $</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 2</p> </td> 
   <td> <p>5 ore</p> </td> 
   <td> <p>500,00 $</p> </td> 
   <td> <p>10 ore</p> </td> 
   <td> <p>1.000,00 $</p> </td> 
   <td> <p>20%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 3</p> </td> 
   <td> </td> 
   <td> </td> 
   <td> <p>10 ore</p> </td> 
   <td> <p>1.000,00 $</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 4</p> </td> 
   <td> <p>10 ore</p> </td> 
   <td> <p>1.000,00 $</p> </td> 
   <td> <p>10 ore</p> </td> 
   <td> <p>1.000,00 $</p> </td> 
   <td> <p>40%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 5</p> </td> 
   <td> <p>15 ore</p> </td> 
   <td> <p>1.500,00 $</p> </td> 
   <td> <p>10 ore</p> </td> 
   <td> <p>1.000,00 $</p> </td> 
   <td> <p>50%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 6</p> </td> 
   <td> <p>20 ore</p> </td> 
   <td> <p>2.000,00 $</p> </td> 
   <td> <p>10 ore</p> </td> 
   <td> <p>1.000,00 $</p> </td> 
   <td> <p>60%</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Aggiungere 50 ore direttamente al progetto (Più>Ore>Registra ore) in modo da registrare 5.000,00 $ di costo effettivo della manodopera direttamente nel progetto. **&#x200B;**
1. Aggiungi le spese per ogni attività in base alla tabella seguente (ho aggiunto una riga vuota tra ogni attività per facilitarne la lettura):

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
   <td> <p>- $ 400,00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 1</p> </td> 
   <td> <p>Attività 1 Scad. 2</p> </td> 
   <td> <p>- 500,00 $</p> </td> 
   <td> <p>800,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 1</p> </td> 
   <td> <p>Attività 1 Scad. 3</p> </td> 
   <td> <p>400,00 $</p> </td> 
   <td> <p>0,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 2</p> </td> 
   <td> <p>Attività 2 Scad. 1</p> </td> 
   <td> <p>500,00 $</p> </td> 
   <td> <p>700,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 2</p> </td> 
   <td> <p>Attività 2 Scad. 2</p> </td> 
   <td> <p>- $ 400,00</p> </td> 
   <td> <p>0,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 2</p> </td> 
   <td> <p>Attività 2 Scad. 3</p> </td> 
   <td> <p>- 200,00 $</p> </td> 
   <td> <p>600,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 2</p> </td> 
   <td> <p>Attività 2 Scad. 4</p> </td> 
   <td> <p>700,00 $</p> </td> 
   <td> <p>- 200,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 3</p> </td> 
   <td> <p>Scad. attività 3</p> </td> 
   <td> <p>0,00 $</p> </td> 
   <td> <p>1.000,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 4</p> </td> 
   <td> <p>Attività 4 Scad. 1</p> </td> 
   <td> <p>800,00 $</p> </td> 
   <td> <p>0,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 4</p> </td> 
   <td> <p>Attività 4 Scad. 2</p> </td> 
   <td> <p>- $ 100,00</p> </td> 
   <td> <p>300,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 4 </p> </td> 
   <td> <p>Attività 4 Scad. 3</p> </td> 
   <td> <p>-200,00</p> </td> 
   <td> <p>0,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 5</p> </td> 
   <td> <p>Task 5 Exp 1</p> </td> 
   <td> <p>700,00 $</p> </td> 
   <td> <p>800,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 5</p> </td> 
   <td> <p>Attività 5 Scad. 2</p> </td> 
   <td> <p>- $ 100,00</p> </td> 
   <td> <p>300,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 5</p> </td> 
   <td> <p>Attività 5 Scad. 3</p> </td> 
   <td> <p>- $ 400,00</p> </td> 
   <td> <p>- 200,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 6</p> </td> 
   <td> <p>Attività 6 Scad. 1</p> </td> 
   <td> <p>600,00 $</p> </td> 
   <td> <p>700,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 6</p> </td> 
   <td> <p>Attività 6 Scad. 2</p> </td> 
   <td> <p>500,00 $</p> </td> 
   <td> <p>- $ 300,0</p> </td> 
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
   <td> <p> 0,00 $ <strong></strong></p> </td> 
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
   <td> <p>400,00 $</p> </td> 
   <td> <p>- 500,00 $</p> </td> 
   <td> <p>800,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 2</p> </td> 
   <td> <p>- $ 400,00</p> </td> 
   <td> <p>300,00 $</p> </td> 
   <td> <p>1.300,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 3</p> </td> 
   <td> <p>0,00 $</p> </td> 
   <td> <p>0,00 $</p> </td> 
   <td> <p>1.000,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 4</p> </td> 
   <td> <p>600,00 $</p> </td> 
   <td> <p>- $ 100,00</p> </td> 
   <td> <p>300,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 5</p> </td> 
   <td> <p>0,00 $</p> </td> 
   <td> <p>600,00 $</p> </td> 
   <td> <p>1.100,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 6</p> </td> 
   <td> <p>0,00 $</p> </td> 
   <td> <p>600,00 $</p> </td> 
   <td> <p>700,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Progetto</p> </td> 
   <td> <p>2.500,00 $</p> </td> 
   <td> <p>1000,00 $</p> </td> 
   <td> <p>1.500,00 $</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Da Azioni progetto, eseguire Ricalcola dati finanziari
1. **CPI** per l&#39;attività 2 = 0,17 calcolato come segue:\
   **Attività IPC 2** = *IF* Costo effettivo manodopera + IncurredActualExpenseCost  &lt;> 0 *THEN* IPC = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)\
   *   ELSE* CPI = CPI_Labor\
   **CPI**&#x200B;**Attività 2** = (100+300) / (1000+1300)\
   **CPI**&#x200B;**Attività 2**  = 400 / 2300\
   **CPI**&#x200B;**Attività 2**  = 0,17

1. **EAC** per l&#39;attività 2 = $5.900,00\
   **Manodopera IPC**&#x200B;**Attività 2** = SE Costo effettivo manodopera &lt;> 0 THEN CPI_Labor = TotalBudgetedCostWorkPerformed / Costo effettivo manodopera\
      ELSE CPI_Labor = 1\
   **Manodopera IPC**&#x200B;**Attività 2** = 100/1000\
   **Manodopera IPC**&#x200B;**Attività 2** = 0,1

   **Manodopera EAC**&#x200B;**Attività 2** = *IF* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost/CPI_Labor
   ```

   *   ELSE* EAC  Manodopera = Costo manodopera pianificato + Costo manodopera effettivo\
   **Manodopera EAC**&#x200B;**Attività 2** = 500.00/.1\
   **Manodopera EAC**&#x200B;**Attività 2** = $5.000,00 **&#x200B;**&#x200B;**&#x200B; Spese EAC &#x200B;**&#x200B;**Attività 2 &#x200B;**= IncurredActualExpenseCost + NotIncurredPlannedExpense\
   **Spesa EAC &#x200B;**&#x200B;**Attività 2** = $ 1.300,00 + - $ 400,00\
   **Spese EAC**&#x200B;**Attività 2** = $900,00

   **EAC**&#x200B;**Attività 2** = Manodopera EAC + Spese EAC\
   **EAC**&#x200B;**Attività 2**  = $5.000,00 + $900,00\
   **EAC**&#x200B;**Attività 2**  = $5.900,00

1. Il CPI/EAC per le Attività 4, 5 e 6 è determinato nello stesso modo, quindi fornirò questi valori qui sotto:\
   Attività 4: 0,23 / 3.400,00 $\
   Attività 5: 0,64 / 3.100,00 $\
   Attività 6: 1,06 / 2.366,67 $

1. CPI per il task 3 = 0,31 calcolato come segue:\
   **CPI**&#x200B;**Attività 3** = *IF* Costo effettivo manodopera + IncurredActualExpenseCost  &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor\
   **CPI**&#x200B;**Attività 3**  = (1,150 + 500) / (3000 + 2400)\
   **CPI**&#x200B;**Attività 3**  =  1650/5400\
   **CPI**&#x200B;**Attività 3**  = .31 **&#x200B;**&#x200B;**&#x200B; EAC per l&#39;attività 3 &#x200B;**= $9.521,74 calcolato come segue:\
   **Manodopera IPC &#x200B;**&#x200B;**Attività 3** = SE Costo effettivo manodopera &lt;> 0 THEN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **Manodopera IPC**&#x200B;**Attività 3** = 1150/3000\
   **Manodopera IPC**&#x200B;**Attività 3** = .383333\
   **Manodopera IPC**&#x200B;**Attività 3** = 0,38

   **Manodopera EAC**&#x200B;**Attività 3** = *IF* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   *   ELSE* EAC  Manodopera = Costo manodopera pianificato + Costo manodopera effettivo\
   **Manodopera EAC**&#x200B;**Attività 3** = $2.500,00 / .383333\
   **Manodopera EAC**&#x200B;**Attività 3** = $ 6.521,74

   **Spesa**&#x200B;**Attività EAC 3** = IncurredActualExpenseCost + NotIncurredPlannedExpense\
   **Spese EAC**&#x200B;**Attività 3** = $2.400,00 + $600,00\
   **Spese EAC**&#x200B;**Attività 3** = $ 3.000,00

   **EAC**&#x200B;**Attività 3** = Manodopera EAC + Spese EAC\
   **EAC**&#x200B;**Attività 3**  = $6.521,74 + $3.000,00\
   **EAC**&#x200B;**Attività 3**  = 9.521,74 $

1. CPI per il task 1 = 0,16 calcolato come segue:\
   **CPI**&#x200B;**Attività 1** = *IF* Costo effettivo manodopera + IncurredActualExpenseCost  &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor\
   **CPI**&#x200B;**Attività 1**  = (1250 + 300) / (5000 + 4500)\
   **CPI**&#x200B;**Attività 1**  =  1550/9500=\
   **CPI**&#x200B;**Attività 1**  = 0,16

1. L&#39;EAC per l&#39;attività 1 è pari a $17.100,00, calcolato come segue:\
   **Manodopera IPC**&#x200B;**Attività 1** = SE Costo effettivo manodopera &lt;> 0 THEN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **Manodopera IPC**&#x200B;**Attività 1** = 1250/5000\
   **Manodopera IPC**&#x200B;**Attività 1** = 0,25

   **Manodopera EAC**&#x200B;**Attività 1** = *IF* CPI_Labor &lt;> 0 *THEN* Manodopera EAC = Costo manodopera pianificato / CPI_Labor\
   *   ELSE* EAC  Manodopera = Costo manodopera pianificato + Costo manodopera effettivo\
   **Manodopera EAC**&#x200B;**Attività 1** = $3.000,00 / .25\
   **Manodopera EAC**&#x200B;**Attività 1** = $ 12.000,00

   **Spese EAC**&#x200B;**Attività 1** = IncurredActualExpenseCost + NotIncurredPlannedExpense\
   **Spese EAC**&#x200B;**Attività 1** = $4.500 + 600\
   **Spese EAC**&#x200B;**Attività 1** = $5.100,00

   **EAC**&#x200B;**Attività 1** = Manodopera EAC + Spese EAC\
   **EAC**&#x200B;**Attività 1**  = $12.000,00 + 5.100,00\
   **EAC**&#x200B;**Attività 1**  = $ 17.100,00

1. CPI per il progetto: 0,25\
   **CPI**&#x200B;**per il progetto** = *IF* Costo effettivo manodopera + IncurredActualExpenseCost  &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor

   **CPI**&#x200B;**per il progetto** = (2450 + 1900) / (11000 + 6700)\
   **CPI**&#x200B;**per il progetto** =   4350/17700\
   **CPI**&#x200B;**per il progetto** = 0,25

1. **EAC per il progetto** = $32.248,98 calcolato come segue:\
   **Manodopera IPC**&#x200B;**per il progetto** = SE Costo effettivo manodopera &lt;> 0 THEN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **Manodopera IPC**&#x200B;**per il progetto** = 2450 / 11000\
   **Manodopera IPC**&#x200B;**per il progetto** = .22272\
   **Manodopera IPC**&#x200B;**per il progetto** = 0,22

   **Manodopera EAC**&#x200B;**per il progetto** = *IF* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   *   ELSE* EAC  Manodopera = Costo manodopera pianificato + Costo manodopera effettivo\
   **Manodopera EAC**&#x200B;**per il progetto** = $5.000,00 / .22272\
   **Manodopera EAC**&#x200B;**per il progetto** = $ 22.448,97959\
   **Manodopera EAC**&#x200B;**per il progetto** = $ 22.448,98

   **Spese EAC**&#x200B;**Progetto** = IncurredActualExpenseCost + NotIncurredPlannedExpense\
   **Spese EAC**&#x200B;**Progetto** = $3.100,00 + $6.700,00\
   **Spese EAC**&#x200B;**Progetto** = $9.800,00

   **EAC**&#x200B;**Progetto** = Manodopera EAC + Spese EAC\
   **EAC**&#x200B;**Progetto**  = 22.448,98 $ + 9.800,00\
   **EAC**&#x200B;**Progetto**  = 32.248,98 $
