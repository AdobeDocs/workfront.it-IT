---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcola costo preventivato del lavoro eseguito (BCWP)
description: Il valore BCWP (Costo preventivato del lavoro eseguito, Budgeted Cost of Work Performed) è una metrica delle prestazioni del progetto che rappresenta la quantità di attività effettivamente completata al momento del calcolo di questa metrica.
author: Lisa
feature: Work Management
exl-id: 203709a7-e522-4875-b3eb-40b967a938ec
source-git-commit: cd0214917620e0b147d0da3402ea2d34e28bc9c3
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 2%

---

# Calcola costo preventivato del lavoro eseguito (BCWP)

## Panoramica sul costo preventivato del lavoro eseguito (BCWP)

Il valore BCWP (Costo preventivato del lavoro eseguito, Budgeted Cost of Work Performed) è una metrica delle prestazioni del progetto che rappresenta la quantità di attività effettivamente completata al momento del calcolo di questa metrica.

Adobe Workfront calcola il costo preventivato del lavoro eseguito (BCWP) sia per i progetti che per le attività.

Quando si esaminano i valori del campo BCWP per un&#39;attività o un progetto, tenere presente quanto segue:

* In Workfront il valore BCWP di un&#39;attività viene calcolato in base alla configurazione del metodo di indicizzazione delle prestazioni (PMI) del progetto.

  È possibile configurare il progetto per il calcolo delle PMI utilizzando ore o costo e anche il valore BCWP viene calcolato utilizzando gli stessi valori.

  Per informazioni sulla configurazione del metodo di calcolo del valore BCWP, vedere la sezione [Configurare il metodo di calcolo del valore BCWP](#configure-how-bcwp-is-calculated) in questo articolo.

* In Workfront il valore BCWP di un progetto viene calcolato sommando tutti i valori BCWP di tutte le attività padre e delle singole attività del progetto.

  I valori delle attività figlio non vengono aggiunti al BCWP del progetto.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

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
   <p>Standard</p>
   <p>Piano</p></td> 
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td>Modifica accesso ai progetti</td> 
  </tr> 
  <tr> 
   <td>Autorizzazioni oggetto</td> 
   <td>Gestire le autorizzazioni per il progetto</td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurare la modalità di calcolo del valore BCWP {#configure-how-bcwp-is-calculated}

È possibile specificare se il valore BCWP deve essere calcolato in ore o in costi configurando il metodo PIM (Performance Index Method) del progetto.

1. Vai a un progetto ed espandi **Dettagli progetto** nel pannello a sinistra.
1. Nell&#39;area **Finance** individuare il campo **Metodo indice prestazioni** e fare doppio clic per modificarlo.

   ![Opzioni PIM](assets/pim-options-hour-cost-based-nwe.png)

1. Selezionare una delle opzioni seguenti:

   | Opzione | Modalità di esecuzione del calcolo |
   |---|---|
   | Basato su Ore | In Workfront il valore BCWP viene calcolato in base alle ore pianificate delle attività. |
   | Basato su Costo | Workfront calcola il valore BCWP in base al costo pianificato delle attività. |

1. Fai clic su **Salva modifiche**.

   Il valore BCWP delle attività del progetto viene calcolato in base alle ore o ai costi.

## Calcola BCWP

In Workfront il valore BCWP (Costo preventivato del lavoro eseguito, Budgeted Cost of Work Performed) di un&#39;attività o di un progetto viene calcolato utilizzando le formule riportate di seguito.

```
Task BCWP = Actual Percent Complete x Task Budget
```

```
Project BCWP = SUM(BCWP values of all parent and individual tasks)
```

In questi calcoli vengono utilizzati i seguenti valori:

| Valore utilizzato | Descrizione del valore utilizzato |
|---|---|
| Percentuale di completamento effettiva | Questa è la percentuale effettiva di completamento dell&#39;attività così come viene visualizzata in Workfront. |
| Budget Attività | Questo è il valore per le ore pianificate o il costo pianificato dell&#39;attività. |

Ad esempio, se la percentuale di completamento effettiva dell&#39;attività è 25% e il Budget attività o il Costo pianificato è pari a $10.000, il valore BCWP per l&#39;attività è:

```
BCWP = 25% x $10,000 = $2,500
```

## Individuare il campo BCWP per un progetto o un&#39;attività

È possibile visualizzare il valore del Costo preventivato del lavoro eseguito in un report o in un elenco aggiungendo la colonna BCWP alla visualizzazione.

1. Consente di passare a un elenco di attività o progetti.
1. Espandere il menu **Visualizza** e selezionare **Nuova visualizzazione** o **Personalizza visualizzazione**.

1. Fai clic su **Aggiungi colonna**.
1. Nel campo **Mostra in questa colonna:** inizia a digitare **BCWP** e fai clic su per selezionarlo quando viene visualizzato nell&#39;elenco.

   ![BCWP in visualizzazione progetto](assets/bcwp-project-view.png)

1. Fai clic su **Salva vista**.
1. Nella visualizzazione viene visualizzato il campo BCWP.
