---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcola stima al completamento (EAC)
description: Come metrica delle prestazioni, la stima al completamento (CES) rappresenta il costo totale previsto del progetto o dell'attività al completamento.
author: Lisa
feature: Work Management
exl-id: 9061fa56-cff3-4fe2-866e-1fdda9d43efc
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '825'
ht-degree: 1%

---

# Calcola stima al completamento (EAC)

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link!) </p>
-->

Come metrica delle prestazioni, la stima al completamento (CES) rappresenta il costo totale previsto del progetto o dell&#39;attività al completamento.

Come impostazione, ti consente di definire come deve essere calcolato il valore EAC.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacchetto Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td>Licenza Adobe Workfront</td> 
   <td>
   <p>Chiaro o superiore</p>
   <p>Revisione o successiva</p></td>  
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td>Accesso ai progetti e ai dati finanziari</td> 
  </tr> 
  <tr> 
   <td>Autorizzazioni oggetto</td> 
   <td>Visualizza o autorizzazioni superiori per il progetto con autorizzazioni Visualizza contabilità</td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Definire la modalità di calcolo EAC

Come parte delle preferenze di sistema del progetto, l’amministratore di Adobe Workfront può definire come calcolare la CES. EAC può essere calcolato in uno dei due modi seguenti:

* [Calcola a livello di progetto](#calculate-at-the-project-level)
* [Esegui il rollup da attività e sottoattività](#roll-up-from-tasks-and-subtasks)

Per ulteriori informazioni sulla configurazione delle preferenze del progetto in Workfront, incluso il calcolo della stima al completamento, vedi [Configurare le preferenze del progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

In qualità di project manager, è inoltre possibile modificare questa preferenza a livello di progetto nella scheda secondaria Finanza del progetto. Per ulteriori informazioni sulla modifica della scheda secondaria Finanza di un progetto, vedere [Gestire le informazioni nell&#39;area Finanza del progetto](../../../manage-work/projects/project-finances/manage-project-finance-area.md).

### Calcola a livello di progetto {#calculate-at-the-project-level}

Il costo effettivo della manodopera per l&#39;attività e il progetto padre viene determinato inserendo il costo effettivo della manodopera/ore effettive nelle formule EAC. Questo calcolo include le ore effettive, i costi e le spese aggiunti direttamente all&#39;attività o al progetto padre.

### Esegui il rollup da attività e sottoattività {#roll-up-from-tasks-and-subtasks}

L&#39;EAC per l&#39;attività e il progetto padre viene determinato sommando l&#39;EAC per ogni attività figlio. Questo calcolo esclude le ore effettive, i costi e le spese aggiunti direttamente all&#39;attività o al progetto padre.

## Come calcolare EAC in base al metodo PIM (Performance Index Method)

In Workfront, il calcolo per EAC dipende dal metodo PIM (Performance Index Method) selezionato per il progetto. Per ulteriori informazioni sull&#39;impostazione del PIM per il sistema o per il progetto, vedere [Impostare il metodo PIM (Performance Index Method)](../../../manage-work/projects/project-finances/set-pim.md).

* [Calcola EAC con PIM basato su ore](#calculate-eac-using-hour-based-pim)
* [Calcola EAC utilizzando PIM basata sui costi](#calculate-eac-using-cost-based-pim)

### Calcola EAC utilizzando PIM basata su ore {#calculate-eac-using-hour-based-pim}

```
EAC = Total Planned Hours / CPI*
```

&#42;Se Indice prestazioni costi [Calcola indice prestazioni costi (IPC)](../../../manage-work/projects/project-finances/calculate-cpi.md) = 0, CES = Ore pianificate totali + Ore effettive. Ciò si verifica quando le ore sono state acquisite, ma il progetto/attività è completato allo 0%.

Per ulteriori informazioni sul calcolo dell&#39;IPC, vedere [Calcolare l&#39;indice di prestazioni dei costi (IPC)](../../../manage-work/projects/project-finances/calculate-cpi.md).

### Calcola EAC utilizzando PIM basata sui costi {#calculate-eac-using-cost-based-pim}

L’EAC di un progetto viene calcolato con la seguente formula:

```
EAC = EAC Labor + EAC Expense 
```

<pre>Manodopera EAC = <em>IF</em> Manodopera CPI &lt;&gt; 0 THEN Manodopera EAC = Costo manodopera pianificata / Manodopera CPI</pre><pre><em>ELSE</em> Manodopera EAC = Costo manodopera pianificato + Costo manodopera effettivo</pre><pre>Manodopera IPC = IF Costo effettivo manodopera &lt;&gt; 0 THEN Manodopera IPC = TotalBudgetedCostWorkPerformed / Costo effettivo manodopera</pre><pre>ELSE CPI Manodopera = 1 </pre>I seguenti campi sono presi in considerazione nel calcolo della CES:

* Costo preventivato totale lavoro eseguito (BCWP) = risultato della moltiplicazione del costo preventivato del lavoro pianificato (costo preventivato) e della percentuale di completamento dell&#39;attività.

  Per informazioni sul valore BCWP (Total Budgeted Cost Work Performed), vedere [Calcolare il lavoro BCWP (Calculate Cost Work Performed)](../../../manage-work/projects/project-finances/calculate-bcwp.md).

   * **Per attività non padre:**

     ```
     Total Budgeted Cost Work Performed = Planned Hours * (Percent Complete/100)
     ```

   * **Per un&#39;attività padre:**
Costo preventivato totale lavoro eseguito = somma del campo Costo preventivato totale lavoro eseguito per tutte le attività figlio dirette.

   * **Per un progetto:**
Costo preventivato totale lavoro eseguito = somma del campo Costo preventivato totale lavoro eseguito per tutte le attività di livello superiore (attività padre e attività autonome).

* Spesa CES = risultato dell&#39;aggiunta del Costo di Spesa Effettivo Sostenuto al Costo di Spesa Pianificato Non Sostenuto. Viene calcolata con la seguente formula:

  ```
  EAC Expense = Incurred Actual Expense Cost + Not Incurred Planned Expense
  ```

   * Costo spesa effettivo sostenuto = Somma del campo Importo pianificato per tutte le spese in cui il campo Importo effettivo è > 0. Ad esempio, se si crea una spesa per l&#39;Attività 1 e si immette $500,00 nel campo Importo pianificato e un importo > 0 nel campo Importo effettivo (ovvero $600,00), il costo delle spese pianificate sostenute per questa attività è $500,00.
   * Spesa pianificata non sostenuta = Somma del campo Importo pianificato per tutte le spese in cui il campo Importo effettivo = 0. Ad esempio, se si creano due spese per l&#39;Attività 1 in cui per la prima spesa il valore nel campo Importo pianificato è $500,00 e il valore nel campo Importo effettivo è $600,00 e per la seconda spesa, il valore nel campo Importo pianificato è $300,00 e il valore del campo Importo effettivo è $0,00, il valore della spesa pianificata non sostenuta per questa attività è $300,00.

## Individuare l&#39;EAC in un progetto o in un&#39;attività

1. Passare al progetto o all&#39;attività in cui si desidera visualizzare la CES.
1. Espandere **Dettagli progetto** o **Dettagli attività** nel pannello a sinistra del progetto o dell&#39;attività, a seconda della posizione di visualizzazione della CES.

1. Fare clic su **Finanza**.

   Il valore EAC viene visualizzato nel campo **Stima al completamento**.

   ![EAC sul progetto](assets/eac-highlighted-on-project-350x112.png)
