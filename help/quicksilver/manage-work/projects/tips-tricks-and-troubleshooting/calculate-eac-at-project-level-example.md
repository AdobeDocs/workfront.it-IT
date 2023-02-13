---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: Esempio di calcolo - calcola EAC a livello di progetto
description: PIM = basato su ora
author: Alina
feature: Work Management
exl-id: ff88b7e3-2a5b-464f-bed1-6848067840b8
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '1768'
ht-degree: 9%

---

# Esempio di calcolo - calcola EAC a livello di progetto

## Metodo EAC: Calcola a livello di progetto

* [PIM = basato su ora](#pim-hour-based)
* [PIM= Basato sui costi](#pim-cost-based)

### PIM = basato su ora {#pim-hour-based}

* [Esempio semplice: il progetto non ha attività figlio](#simple-example-project-has-no-children-tasks)
* [Esempio complesso: il progetto ha attività figlio](#complicated-example-project-has-children-tasks)

#### Esempio semplice: il progetto non ha attività figlio {#simple-example-project-has-no-children-tasks}

PIM = basato su ora

Metodo EAC = Calcola a livello di progetto ****

1. Crea il progetto A con tre attività (nessuna attività figlio) tutte assegnate all&#39;utente 1 il cui costo/ora è di $100,00.
1. Aggiungi le ore pianificate e effettive a ogni attività e % complete secondo la tabella seguente:

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

1. Ricalcola finanza sul progetto.
1. **CPI per l&#39;attività 1** = 0,04 calcolato come segue:\
   **CPI per l&#39;attività 1** = *IF* Ore effettive > 0 *POI* CPI = Ore effettive (TotalBudgetedCostWorkPerformed)\
      *ELSE* IPC = 1\
   **CPI per l&#39;attività 1** = 1 / 25\
   **CPI per l&#39;attività 1** = 0,04

1. **EAC per l&#39;attività 1** = 125 ore calcolate come segue:\
   **EAC per l&#39;attività 1** = *IF* CPI &lt;> 0 *POI* EAC = orario pianificato/CPI\
       *ELSE* EAC = ore pianificate + ore effettive\
   **EAC per l&#39;attività 1** = 5 / 04\
   **EAC per l&#39;attività 1** = 125 ore****

1. CPI / EAC per i compiti 2 e 3:\
   Attività 2 = 0,12 / 83,33 ore\
   Attività 3 = 0,24 / 62,5 ore

1. **CPI per progetto** = 0,13 calcolato come segue:\
   **CPI per progetto** = *IF* Ore effettive > 0 *POI* CPI = Ore effettive (TotalBudgetedCostWorkPerformed)\
       *ELSE* IPC = 1\
   **CPI per progetto** = 10 / 75\
   **CPI per progetto** = 0,13

1. **EAC per il progetto** = 225 ore calcolate come segue:\
   **EAC per il progetto** = *IF* CPI &lt;> 0 *POI* EAC = orario pianificato/CPI\
       *ELSE* EAC = ore pianificate + ore effettive\
   **EAC per il progetto** = 30 / 13333\
   **EAC per il progetto** = 225 ore

#### Esempio complesso: il progetto ha attività figlio {#complicated-example-project-has-children-tasks}

PIM = basato su ora

Metodo EAC = Calcola a livello di progetto

1. Crea il progetto A con sei attività in cui l&#39;attività 3 è l&#39;elemento padre delle attività 4 e 5 e l&#39;attività 1 è l&#39;elemento padre delle attività 2 e 3, come illustrato di seguito:\
   Attività 1\
      Attività 2\
      Attività 3\
         Attività 4\
         Attività 5\
   Attività 6

1. Assegna le attività 2, 4, 5 e 6 all&#39;utente 1 il cui costo/ora è di $100,00.
1. Aggiungi ore pianificate/effettive per ciascuna attività e % complete secondo la tabella seguente.

   >[!NOTE]
   >
   >Per le attività 1 e 3, si aggiungono solo le ore effettive.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <br> <p><strong>Attività</strong> </p> </th> 
   <th> <br> <p><strong>Ore pian.</strong> </p> </th> 
   <th> <br> <p><strong>Lav Real</strong> </p> </th> 
   <th> <p><strong>% Completato</strong> </p> </th> 
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

1. Aggiungi 50 ore direttamente al progetto (Altro>Ore>Orari di log).
1. **CPI per l&#39;attività 2** = 0,1 calcolato come segue:\
   **CPI per l&#39;attività 2** = *IF* Ore effettive > 0 *POI* CPI = Ore effettive (TotalBudgetedCostWorkPerformed)\
       *ELSE* IPC = 1\
   **CPI per l&#39;attività 2** = 1 / 10\
   **CPI per l&#39;attività 2** = 0,1

1. **EAC per l&#39;attività 2** = 50 ore calcolate come segue:\
   **EAC per l&#39;attività 2** = *IF* CPI &lt;> 0 *POI* EAC = orario pianificato/CPI\
       *ELSE* EAC = ore pianificate + ore effettive\
   **EAC per l&#39;attività 2** = 5 / 0,1\
   **EAC per l&#39;attività 2** = 50 ore

1. L&#39;IPC / EAC per le funzioni 4, 5 e 6 è il seguente:\
   Attività 4: 0,4 / 25 ore\
   Attività 5: 0,75 / 20 ore\
   Attività 6: 1,2 / 16,67 ore

1. **CPI per l&#39;attività 3** = 0,38 calcolato come segue:\
   **CPI per l&#39;attività 3** = *IF* Ore effettive > 0 *POI* CPI = Ore effettive (TotalBudgetedCostWorkPerformed)\
       *ELSE* IPC = 1\
   **CPI per l&#39;attività 3** = 11,5 / 30\
   **CPI per l&#39;attività 3** = 0,38

1. **EAC per l&#39;attività 3** = 65,22 ore calcolate come segue:\
   **EAC per l&#39;attività 3** = *IF* CPI &lt;> 0 *POI* EAC = orario pianificato/CPI\
       *ELSE* EAC = ore pianificate + ore effettive\
   **EAC per l&#39;attività 3** = 25 / 0,38333\
   **EAC per l&#39;attività 3** = 65,22 ore

1. **CPI per l&#39;attività 1** = 0,25 calcolato come segue:\
   **CPI per l&#39;attività 1** = *IF* Ore effettive > 0 *POI* CPI = Ore effettive (TotalBudgetedCostWorkPerformed)\
       *ELSE* IPC = 1\
   **CPI per l&#39;attività 1** = 12,5 / 50\
   **CPI per l&#39;attività 1** = 0,25

1. **EAC per l&#39;attività 1** = 120 ore calcolate come segue:\
   **EAC per l&#39;attività 1** = *IF* CPI &lt;> 0 *POI* EAC = ore previste / CPI\
       *ELSE* EAC = ore pianificate + ore effettive\
   **EAC per l&#39;attività 1** = 30/ 0,25\
   **EAC per l&#39;attività 1** = 120 ore

1. **CPI per progetto** = 0,22 calcolato come segue:\
   **CPI per progetto** = *IF* Ore effettive > 0 *POI* CPI = Ore effettive (TotalBudgetedCostWorkPerformed)\
       *ELSE* IPC = 1\
   **CPI per progetto** = 24,5 / 110\
   **CPI per progetto** = 0,22272\
   **CPI per progetto** = 0,22

1. **EAC per il progetto** = 224,49 ore calcolate come segue:\
   **EAC per il progetto** = *IF* CPI &lt;> 0 *POI* EAC = orario pianificato/CPI\
       *ELSE* EAC = ore pianificate + ore effettive\
   **EAC per il progetto** = 50 / 22272\
   **EAC per il progetto** = 224,49 ore

### PIM= Basato sui costi {#pim-cost-based}

* [Esempio semplice: il progetto non ha attività figlio](#simple-example-project-has-no-children-tasks)
* [Esempio complesso: il progetto ha attività figlio](#complicated-example-project-has-children-tasks)

#### Esempio semplice: il progetto non ha attività figlio {#simple-example-project-has-no-children-tasks-1}

PIM = basato sui costi

Metodo EAC = Calcola a livello di progetto

1. Crea il progetto A con tre attività (nessuna attività figlio) tutte assegnate all&#39;utente 1 il cui costo/ora è di $100,00.
1. Aggiungi ore pianificate/effettive a ciascuna attività e % Complete secondo la tabella seguente:

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
   <th> <br> <p><strong>Costo Lbr Pln</strong> </p> </th> 
   <th> <br> <p><strong>Lav Real</strong> </p> </th> 
   <th> <br> <p><strong>Costo Lbr</strong> </p> </th> 
   <th> <p><strong>% Completato</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Attività 1</p> </td> 
   <td> <p>5 ore</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>25 ore</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p>20%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 2</p> </td> 
   <td> <p>10 ore</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>25 ore</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p>30%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 3</p> </td> 
   <td> <p>15 ore</p> </td> 
   <td> <p>$1,500.00</p> </td> 
   <td> <p>25 ore</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p>40%</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Aggiungi le spese a ogni attività in base alla tabella seguente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Attività</strong> </p> </th> 
   <th> <p><strong>Spesa</strong> </p> </th> 
   <th> <p><strong>Somma Pianificato</strong> </p> </th> 
   <th> <p><strong>Somma Reale</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Attività 1</p> </td> 
   <td> <p>Attività 1 Exp 1</p> </td> 
   <td> <p>$300.00</p> </td> 
   <td> <p>$400.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 1</p> </td> 
   <td> <p>Attività 1 Exp 2</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 2</p> </td> 
   <td> <p>Attività 2 Exp</p> </td> 
   <td> <p>$200.00</p> </td> 
   <td> <p>$100.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 3</p> </td> 
   <td> <p>Attività 3 Exp</p> </td> 
   <td> <p>$800.00</p> </td> 
   <td> <p>$700.00</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Aggiungi due spese al progetto (cioè non legate a un&#39;attività) come segue:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Spesa</strong> </p> </th> 
   <th> <p><strong>Somma Pianificato</strong> </p> </th> 
   <th> <p><strong>Somma Reale</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Progetto Exp 1</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>$1,500.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 1 Exp 2</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
 </tbody> 
</table>

1. In base ai valori sopra indicati, i costi sostenuti/non sostenuti sono determinati come segue:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Attività</strong> </p> </th> 
   <th> <p><strong>Spese pianificate non garantite</strong> </p> </th> 
   <th> <p><strong>Spese pianificate garantite</strong> </p> </th> 
   <th> <p><strong>Spese effettive garantite</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Attività 1</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>$300.00</p> </td> 
   <td> <p>$400.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 2</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$200.00</p> </td> 
   <td> <p>$100.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 3</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$800.00</p> </td> 
   <td> <p>$700.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Progetto</p> </td> 
   <td> <p>$3,000.00</p> </td> 
   <td> <p>$2,300.00</p> </td> 
   <td> <p> $2,700.00 <strong></strong></p> </td> 
  </tr> 
 </tbody> 
</table>

1. Da Azioni progetto, eseguire Ricalcola finanziamento
1. **CPI per l&#39;attività 1** = 0,14
1. **CPI****per l’attività 1** = 0,14 calcolato come segue:\
   **CPI**  **per l&#39;attività 1** = *IF* Costo manodopera effettivo + CostoEffettivoCostoSpeseEffettivo &lt;> 0 *POI*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   *    ELSE* CPI = CPI_Labor\
   **CPI****per l’attività 1** = (100+300) / (2500+400)\
   **CPI**  **per l&#39;attività 1** = 400 / 2900\
   **CPI**  **per l&#39;attività 1**  = 0,14****

1. **EAC****per l’attività 1** = $ 13.400,00\
   **Lavoro al CPI**  **per l&#39;attività 1** = SE il costo effettivo del lavoro &lt;> 0 THEN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed/Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **Lavoro al CPI**  **per l&#39;attività 1** = 100/2500\
   **Lavoro al CPI**  **per l&#39;attività 1** = 0,04 ****** Lavoro EAC ****per l&#39;attività 1 **=*IF *CPI_Labor &lt;> 0*POI *EAC Labor = costo del lavoro pianificato/CPI_Labor\
   *    ELSE* Lavoro EAC = Costo del lavoro pianificato + Costo del lavoro effettivo\
   **Lavoro EAC ****per l’attività 1** = 500.00/.04\
   **Lavoro EAC****per l’attività 1** = $ 12.500,00\
   **Spese EAC****per l’attività 1** = CostoEffettivoIncurred + CostoNonIncurredPlannedSpense\
   **Spese EAC****per l’attività 1** = $400,00 + $500,00\
   **Spese EAC****per l’attività 1** = $900,00\
   **EAC****per l’attività 1** = manodopera EAC + spese EAC\
   **EAC****per l’attività 1**  = $ 12.500,00 + $ 900,00\
   **EAC****per l’attività 1**  = $ 13.400,00

1. Di seguito sono riportati i valori CPI / EAC per le attività 2 e 3:\
   Attività 2 = 0,19 / 8.433,33 $\
   Attività 3 = 0,44 / 6.950,00 $

1. **CPI per progetto** = 0,32 calcolato come segue:\
   **CPI****per progetto** = *IF* Costo manodopera effettivo + CostoEffettivoCostoSpeseEffettivo &lt;> 0 *POI*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor\
   **CPI****per progetto** = (1000 + 2300) / (7500 + 2700)\
   **CPI****per progetto** = 3300 / 10200\
   **CPI****per progetto** = 0,32

1. **EAC per il progetto** = $ 28.200,00 calcolati come segue:\
   **Lavoro CPI****per progetto** = SE il costo effettivo del lavoro &lt;> 0 THEN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed/Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **Lavoro CPI****per progetto** = 1000 / 7500\
   **Lavoro CPI****per progetto** = 0,13333\
   **Lavoro CPI****per progetto** = 0,13

   **Lavoro EAC****per progetto** = *IF* CPI_Labor &lt;> 0 *POI*

   ```
   EAC Labor = Planned Labor Cost/CPI_Labor
   ```

   *   ELSE* Lavoro EAC = Costo del lavoro pianificato + Costo del lavoro effettivo\
   **Lavoro EAC****per progetto** = 3000/.13333\
   **Lavoro EAC****per progetto** = $22.500,00

   **Spese EAC****Progetto** =

   ```
   IncurredActualExpenseCost + NotIncurredPlannedExpense
   ```

   **Spese EAC****Progetto** = $3000,00 + 2.700,00\
   **Spese EAC****Progetto** = $5.700,00

   **Progetto EAC****** = manodopera EAC + spese EAC\
   **Progetto EAC******  = $22.500,00 + $5.700,00\
   **Progetto EAC******  = $ 28.200,00

#### Esempio complesso: il progetto ha attività figlio {#complicated-example-project-has-children-tasks-1}

PIM = basato sui costi

Metodo EAC = Calcola a livello di progetto

1. Crea il progetto A con sei attività in cui l&#39;attività 3 è l&#39;elemento padre delle attività 4 e 5 e l&#39;attività 1 è l&#39;elemento padre delle attività 2 e 3, come illustrato di seguito:\
   Attività 1\
      Attività 2\
      Attività 3\
         Attività 4\
         Attività 5\
   Attività 6

1. Assegna le attività 2, 4, 5 e 6 all&#39;utente 1 il cui costo/ora è di $100,00.
1. Aggiungi ore pianificate/effettive per ciascuna attività e % complete secondo la tabella seguente.

   >[!NOTE]
   >
   >Per le attività 1 e 3, si aggiungono solo le ore effettive.

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
   <th> <br> <p><strong>Costo Lbr Pln</strong> </p> </th> 
   <th> <br> <p><strong>Lav Real</strong> </p> </th> 
   <th> <br> <p><strong>Costo Lbr</strong> </p> </th> 
   <th> <p><strong>% Completato</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Attività 1</p> </td> 
   <td> </td> 
   <td> </td> 
   <td> <p>10 ore</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 2</p> </td> 
   <td> <p>5 ore</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>10 ore</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>20%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 3</p> </td> 
   <td> </td> 
   <td> </td> 
   <td> <p>10 ore</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 4</p> </td> 
   <td> <p>10 ore</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>10 ore</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>40%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 5</p> </td> 
   <td> <p>15 ore</p> </td> 
   <td> <p>$1,500.00</p> </td> 
   <td> <p>10 ore</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>50%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 6</p> </td> 
   <td> <p>20 ore</p> </td> 
   <td> <p>$2,000.00</p> </td> 
   <td> <p>10 ore</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>60%</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Aggiungi 50 ore direttamente al progetto (Altro>Ore>Orari di log) in modo che ci siano 5.000,00 $ del costo effettivo del lavoro registrato direttamente al progetto. ****
1. Aggiungi le spese a ogni attività in base alla tabella seguente (ho aggiunto una riga vuota tra ciascuna attività per facilitare la lettura):

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Attività</strong> </p> </th> 
   <th> <p><strong>Spesa</strong> </p> </th> 
   <th> <p><strong>Somma Pianificato</strong> </p> </th> 
   <th> <p><strong>Somma Reale</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Attività 1</p> </td> 
   <td> <p>Attività 1 Exp 1</p> </td> 
   <td> <p>$300.00</p> </td> 
   <td> <p>-$400.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 1</p> </td> 
   <td> <p>Attività 1 Exp 2</p> </td> 
   <td> <p>-$500.00</p> </td> 
   <td> <p>$800.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 1</p> </td> 
   <td> <p>Attività 1 Exp 3</p> </td> 
   <td> <p>$400.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 2</p> </td> 
   <td> <p>Attività 2 Exp 1</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>$700.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 2</p> </td> 
   <td> <p>Attività 2 Exp 2</p> </td> 
   <td> <p>-$400.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 2</p> </td> 
   <td> <p>Attività 2 Exp 3</p> </td> 
   <td> <p>-$200.00</p> </td> 
   <td> <p>$600.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 2</p> </td> 
   <td> <p>Attività 2 Exp 4</p> </td> 
   <td> <p>$700.00</p> </td> 
   <td> <p>-$200.00</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 3</p> </td> 
   <td> <p>Attività 3 Exp</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$1,000.00</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 4</p> </td> 
   <td> <p>Task 4 Exp 1</p> </td> 
   <td> <p>$800.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 4</p> </td> 
   <td> <p>Attività 4 Exp 2</p> </td> 
   <td> <p>-$100.00</p> </td> 
   <td> <p>$300.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 4 </p> </td> 
   <td> <p>Task 4 Exp 3</p> </td> 
   <td> <p>-200.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 5</p> </td> 
   <td> <p>Attività 5 Exp 1</p> </td> 
   <td> <p>$700.00</p> </td> 
   <td> <p>$800.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 5</p> </td> 
   <td> <p>Attività 5 Exp 2</p> </td> 
   <td> <p>-$100.00</p> </td> 
   <td> <p>$300.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 5</p> </td> 
   <td> <p>Attività 5 Exp 3</p> </td> 
   <td> <p>-$400.00</p> </td> 
   <td> <p>-$200.00</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 6</p> </td> 
   <td> <p>Attività 6 Exp 1</p> </td> 
   <td> <p>$600.00</p> </td> 
   <td> <p>$700.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 6</p> </td> 
   <td> <p>Attività 6 Exp 2</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>-$300.0</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Aggiungi due spese al progetto (cioè non legate a un&#39;attività) come segue:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Spesa</strong> </p> </th> 
   <th> <p><strong>Somma Pianificato</strong> </p> </th> 
   <th> <p><strong>Somma Reale</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Progetto Exp 1</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>$1,500.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 1 Exp 2</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p> $0.00 <strong></strong></p> </td> 
  </tr> 
 </tbody> 
</table>

1. In base ai valori sopra indicati, i costi sostenuti/non sostenuti sono determinati come segue:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Attività</strong> </p> </th> 
   <th> <p><strong>Spese pianificate non garantite</strong> </p> </th> 
   <th> <p><strong>Spese pianificate garantite</strong> </p> </th> 
   <th> <p><strong>Spese effettive garantite</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Attività 1</p> </td> 
   <td> <p>$400.00</p> </td> 
   <td> <p>-$500.00</p> </td> 
   <td> <p>$800.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 2</p> </td> 
   <td> <p>-$400.00</p> </td> 
   <td> <p>$300.00</p> </td> 
   <td> <p>$1,300.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 3</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$1,000.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 4</p> </td> 
   <td> <p>$600.00</p> </td> 
   <td> <p>-$100.00</p> </td> 
   <td> <p>$300.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 5</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$600.00</p> </td> 
   <td> <p>$1,100.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attività 6</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$600.00</p> </td> 
   <td> <p>$700.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Progetto</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p>$1000.00</p> </td> 
   <td> <p>$1,500.00</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Da Azioni progetto, eseguire Ricalcola finanziamento
1. **CPI** per l&#39;attività 2 = 0,17 calcolato come segue:\
   **Attività CPI 2** = *IF* Costo manodopera effettivo + CostoEffettivoCostoSpeseEffettivo &lt;> 0 *POI* CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)\
   *   ELSE* CPI = CPI_Labor\
   **CPI***Attività 2** = (100+300) / (1000+1300)\
   **CPI***Attività 2**  = 400 / 2300\
   **CPI***Attività 2**  = 0,17

1. **EAC** per l&#39;attività 2 = $5.900,00\
   **Lavoro CPI****Attività 2** = SE Costo manodopera effettivo &lt;> 0 THEN CPI_Labor = CostoCostoLavoroEffettivo/Costo manodopera effettivo\
      ELSE CPI_Labor = 1\
   **Lavoro CPI****Attività 2** = 100/1000\
   **Lavoro CPI****Attività 2** = 0,1

   **Lavoro EAC***Attività 2** = *IF* CPI_Labor &lt;> 0 *POI*

   ```
   EAC Labor = Planned Labor Cost/CPI_Labor
   ```

   *   ELSE* Lavoro EAC = Costo del lavoro pianificato + Costo del lavoro effettivo\
   **Lavoro EAC***Attività 2** = 500.00/.1\
   **Lavoro EAC***Attività 2** = $5.000,00 ****** Spese EAC ****Attività 2 **= CostoEffettivoIncurred + CostoNonIncurredPlannedSpense\
   **Spese EAC ****Attività 2** = $ 1.300,00 + - $ 400,00\
   **Spese EAC***Attività 2** = $900,00

   **EAC***Attività 2** = manodopera EAC + spese EAC\
   **EAC***Attività 2**  = $5.000,00 + $900,00\
   **EAC***Attività 2**  = $5.900,00

1. Il CPI/EAC per le attività 4, 5 e 6 è determinato nello stesso modo in modo che io fornisca semplicemente i seguenti valori:\
   Attività 4: 0,23 / 3.400,00 $\
   Attività 5: 0,64 / 3.100,00 $\
   Attività 6: 1,06 / 2.366,67 $

1. CPI per l&#39;attività 3 = 0,31 calcolato come segue:\
   **CPI***Attività 3** = *IF* Costo manodopera effettivo + CostoEffettivoCostoSpeseEffettivo &lt;> 0 *POI*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor\
   **CPI***Attività 3**  = (1.150 + 500) / (3000 + 2400)\
   **CPI***Attività 3**  = 1650 / 5400\
   **CPI***Attività 3**  = 0,31 ****** EAC per l&#39;attività 3 **= $9.521,74 calcolato come segue:\
   **Lavoro CPI ****Attività 3** = costo effettivo del lavoro IF &lt;> 0 THEN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **Lavoro CPI****Attività 3** = 1150/3000\
   **Lavoro CPI****Attività 3** = 0,383333\
   **Lavoro CPI****Attività 3** = 0,38

   **Lavoro EAC***Attività 3** = *IF* CPI_Labor &lt;> 0 *POI*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   *   ELSE* Lavoro EAC = Costo del lavoro pianificato + Costo del lavoro effettivo\
   **Lavoro EAC***Attività 3** = $2.500,00 / .383333\
   **Lavoro EAC***Attività 3** = $6.521,74

   **Spese EAC***Attività 3** = CostoEffettivoIncurred + CostoNonIncurredPlannedSpense\
   **Spese EAC***Attività 3** = $2.400,00 + $600,00\
   **Spese EAC***Attività 3** = $3.000,00

   **EAC***Attività 3** = manodopera EAC + spese EAC\
   **EAC***Attività 3**  = $6.521,74 + $3.000,00\
   **EAC***Attività 3**  = $ 9.521,74

1. CPI per l&#39;attività 1 = 0,16 calcolato come segue:\
   **CPI***Attività 1** = *IF* Costo manodopera effettivo + CostoEffettivoCostoSpeseEffettivo &lt;> 0 *POI*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor\
   **CPI***Attività 1**  = (1250 + 300) / (5000 + 4500)\
   **CPI***Attività 1**  = 1550 / 9500=\
   **CPI***Attività 1**  = 0,16

1. L&#39;EAC per l&#39;attività 1 è di $17.100,00 calcolato come segue:\
   **Lavoro CPI****Attività 1** = SE il costo effettivo del lavoro &lt;> 0 THEN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **Lavoro CPI****Attività 1** = 1250 / 5000\
   **Lavoro CPI****Attività 1** = 0,25

   **Lavoro EAC***Attività 1** = *IF* CPI_Labor &lt;> 0 *POI* Lavoro EAC = costo del lavoro pianificato / CPI_Labor\
   *   ELSE* Lavoro EAC = Costo del lavoro pianificato + Costo del lavoro effettivo\
   **Lavoro EAC***Attività 1** = $3.000,00 / .25\
   **Lavoro EAC***Attività 1** = $ 12.000,00

   **Spese EAC***Attività 1** = CostoEffettivoIncurred + CostoNonIncurredPlannedSpense\
   **Spese EAC***Attività 1** = $4500 + $600\
   **Spese EAC***Attività 1** = $5.100,00

   **EAC***Attività 1** = manodopera EAC + spese EAC\
   **EAC***Attività 1**  = $ 12.000,00 + 5.100,00\
   **EAC***Attività 1**  = $ 17.100,00

1. CPI per progetto è 0,25\
   **CPI****per progetto** = *IF* Costo manodopera effettivo + CostoEffettivoCostoSpeseEffettivo &lt;> 0 *POI*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor

   **CPI****per progetto** = (2450 + 1900) / (11000 + 6700)\
   **CPI****per progetto** = 4350 / 17700\
   **CPI****per progetto** = 0,25

1. **EAC per il progetto** = $32.248,98 calcolato come segue:\
   **Lavoro CPI****per progetto** = SE il costo effettivo del lavoro &lt;> 0 THEN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **Lavoro CPI****per progetto** = 2450 / 11000\
   **Lavoro CPI****per progetto** = 0,22272\
   **Lavoro CPI****per progetto** = 0,22

   **Lavoro EAC****per progetto** = *IF* CPI_Labor &lt;> 0 *POI*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   *   ELSE* Lavoro EAC = Costo del lavoro pianificato + Costo del lavoro effettivo\
   **Lavoro EAC****per progetto** = $5.000,00 / .22272\
   **Lavoro EAC****per progetto** = $22.448,97959\
   **Lavoro EAC****per progetto** = $22.448,98

   **Spese EAC****Progetto** = CostoEffettivoIncurred + CostoNonIncurredPlannedSpense\
   **Spese EAC****Progetto** = $ 3.100,00 + $ 6.700,00\
   **Spese EAC****Progetto** = $9.800,00

   **Progetto EAC****** = manodopera EAC + spese EAC\
   **Progetto EAC******  = $ 22.448,98 + 9.800,00\
   **Progetto EAC******  = $32.248,98
