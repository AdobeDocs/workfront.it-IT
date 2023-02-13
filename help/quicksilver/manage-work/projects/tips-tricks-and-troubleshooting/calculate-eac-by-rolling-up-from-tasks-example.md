---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: Esempio di calcolo - Calcola EAC come rollup dalle attività
description: PIM = basato su ora
author: Alina
feature: Work Management
exl-id: 68b582c9-f72a-4000-9d28-f7dafa23541f
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '873'
ht-degree: 8%

---

# Esempio di calcolo - Calcola EAC come rollup dalle attività

## Metodo EAC: eseguire il rollup da attività o sottoattività

* [PIM= Basato su ora](#pim-hour-based)
* [PIM= Basato sui costi](#pim-cost-based)

### PIM= Basato su ora {#pim-hour-based}

* [Esempio semplice: il progetto non ha attività figlio](#simple-example-project-has-no-children-tasks)
* [Esempio complesso: il progetto ha attività figlio](#complicated-example-project-has-children-tasks)

#### Esempio semplice: il progetto non ha attività figlio {#simple-example-project-has-no-children-tasks}

PIM = basato su ora

Metodo EAC = aggregazione da attività/sottoattività

1. Crea il progetto A con tre attività (nessuna attività figlio) tutte assegnate all&#39;utente 1 il cui costo/ora è di $100,00.
1. Aggiungi ore pianificate/effettive a ciascuna attività e % Complete secondo la tabella seguente:

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

1. Ricalcola Finanze
1. **CPI per l&#39;attività 1** = 0,04 calcolato come segue:\
   **CPI per l&#39;attività 1** = *IF* Ore effettive > 0 *POI* CPI = Ore effettive (TotalBudgetedCostWorkPerformed)\
       *ELSE* IPC = 1\
   **CPI per l&#39;attività 1** = 1 / 25\
   **CPI per l&#39;attività 1** = 0,04

1. **EAC per l&#39;attività 1** = 125 ore calcolate come segue:\
   **EAC per l&#39;attività 1** = *IF* CPI &lt;> 0 *POI* EAC = orario pianificato/CPI\
       *ELSE*

   ```
   EAC = Planned  Hours + Actual  Hours
   ```

   **EAC per l&#39;attività 1** = 5 / 04\
   **EAC per l&#39;attività 1** = 125 ore

1. CPI / EAC per i compiti 2 e 3:\
   Attività 2 = 0,12 / 83,33 ore\
   Attività 3 = 0,24 / 62,5 ore

1. **CPI per progetto** = 0,13 calcolato come segue:\
   **CPI per progetto** = *IF* Ore effettive > 0 *POI*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* IPC = 1\
   **CPI per progetto** = 10 / 75\
   **CPI per progetto** = 0,13

1. **EAC per il progetto** = 270,83 ore calcolate come segue\
   **EAC per il progetto** = attività EAC 1 + attività EAC 2 + attività EAC 3\
   **EAC per il progetto** = 125 + 83,33 + 62,5\
   **EAC per il progetto** = 270,83 ore

#### Esempio complesso: il progetto ha attività figlio {#complicated-example-project-has-children-tasks}

PIM = basato su ora

Metodo EAC = aggregazione da attività/sottoattività

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

1. Aggiungi 50 ore direttamente al progetto (Altro>Ore>Orari di log) in modo che ci siano 5.000,00 $ del costo effettivo del lavoro registrato direttamente al progetto.
1. Esegui ricalcolo finanziario
1. **CPI per l&#39;attività 2** = 0,1 calcolato come segue:\
   **CPI per l&#39;attività 2** = *IF* Ore effettive > 0 *POI*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* IPC = 1\
   **CPI per l&#39;attività 2** = 1 / 10\
   **CPI per l&#39;attività 2** = 0,1

1. **EAC per l&#39;attività 2** = 50 ore calcolate come segue:\
   **EAC per l&#39;attività 2** = *IF* CPI &lt;> 0 *POI*

   ```
   EAC = Planned Hours / CPI
   ```

       *ELSE* EAC = ore pianificate + ore effettive\
   **EAC per l&#39;attività 2** = 5 / 0,1\
   **EAC per l&#39;attività 2** = 50 ore

1. CPI / EAC per l&#39;attività 4, l&#39;attività 5 e l&#39;attività 6:\
   Attività 4 = 0,4 / 25 ore\
   Attività 5 = 0,75 / 20 ore\
   Attività 6 = 1,2 / 16,67 ore

1. **CPI per l&#39;attività 3** = 0,38\
   **CPI per l&#39;attività 3** = *IF* Ore effettive > 0 *POI*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* IPC = 1\
   **CPI per l&#39;attività 3** = 11,5 / 30\
   **CPI per l&#39;attività 3** = 0,38

1. **EAC per l&#39;attività 3** = attività EAC 4 + attività EAC 5\
   **EAC per l&#39;attività 3** = 25 + 20\
   **EAC per l&#39;attività 3** = 45 ore

1. **CPI per l&#39;attività 1** = 0,25 calcolato come segue:\
   **CPI per l&#39;attività 1** = *IF* Ore effettive > 0 *POI*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* IPC = 1\
   **CPI per l&#39;attività 1** = 12,5 / 50\
   **CPI per l&#39;attività 1** = 0,25

1. **EAC per l&#39;attività 1** = attività dell&#39;EAC 2 + attività dell&#39;EAC 3\
   **EAC per l&#39;attività 1** = 50 + 45\
   **EAC per l&#39;attività 1** = 95 ore

1. CPI per progetto = 0,22 calcolato come segue:\
   **CPI per progetto** = *IF* Ore effettive > 0 *POI*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* IPC = 1\
   **CPI per progetto** = 24,5 / 110\
   **CPI per progetto** = 0,22272\
   **CPI per progetto** = 0,22

1. **EAC per il progetto** = attività EAC 1 + attività EAC 6\
   **EAC per il progetto** = 95 + 16,67\
   **EAC per il progetto** = 111,67 ore

### PIM= Basato sui costi {#pim-cost-based}

* [Esempio semplice: il progetto non ha attività figlio](#simple-example-project-has-no-children-tasks)

#### Esempio semplice: il progetto non ha attività figlio {#simple-example-project-has-no-children-tasks-1}

PIM = basato sui costi

Metodo EAC = aggregazione da attività/sottoattività

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
   <td> <p>$2,700.00</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Da Azioni progetto, eseguire Ricalcola finanziamento
1. **CPI****per l’attività 1** = 0,14 calcolato come segue:\
   **CPI****per l’attività 1**  = *IF* Costo manodopera effettivo + CostoEffettivoCostoSpeseEffettivo &lt;> 0 *POI*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor\
   **CPI****per l’attività 1**  = (100+300) / (2500+400)\
   **CPI****per l’attività 1**  = 400 / 2900\
   **CPI****per l’attività 1**  = 0,14

1. **EAC****per l’attività 1** = $ 13.400,00\
   **Lavoro CPI****per l&#39;attività 1** = SE il costo effettivo del lavoro &lt;> 0 THEN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **Lavoro CPI****per l&#39;attività 1** = 100/2500\
   **Lavoro CPI****per l&#39;attività 1** = 0,04

   **Lavoro EAC****per l’attività 1** = *IF* CPI_Labor &lt;> 0 *POI*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   *   ELSE* Lavoro EAC = Costo del lavoro pianificato + Costo del lavoro effettivo\
   **Lavoro EAC****per l’attività 1** = 500.00/.04\
   **Lavoro EAC****per l’attività 1** = $ 12.500,00

   **Spese EAC****per l’attività 1** = CostoEffettivoIncurred + CostoNonIncurredPlannedSpense\
   **Spese EAC****per l’attività 1** = $400,00 + $500,00\
   **Spese EAC****per l’attività 1** = $900,00

   **EAC****per l’attività 1** = manodopera EAC + spese EAC\
   **EAC****per l’attività 1**  = $ 12.500,00 + $ 900,00\
   **EAC****per l’attività 1**  = $ 13.400,00

1. Di seguito sono riportati i valori CPI / EAC per le attività 2 e 3:\
   Attività 2 = 0,19 / 8.433,33 $\
   Attività 3 = 0,44 / $ 6,950,00****

1. CPI per il progetto = 0,32\
   **CPI****per progetto** = *IF* Costo manodopera effettivo + CostoEffettivoCostoSpeseEffettivo &lt;> 0 *POI*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor\
   **CPI****per progetto** = (1000 + 2300) / (7500 + 2700)\
   **CPI****per progetto** = 3300 / 10200\
   **CPI****per progetto** = 0,32

1. EAC per il progetto è di $28.783,33\
   **EAC****per progetto** = attività EAC 1 + attività EAC 2 + attività EAC 3\
   **EAC****per progetto** = $ 13.400,00 + $ 8.433,33 + $ 6.950,00\
   **EAC****per progetto** = $28.783,33
