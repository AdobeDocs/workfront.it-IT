---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcola costo preventivato del lavoro programmato (BCWS)
description: Anche noto come valore pianificato, il costo preventivato del lavoro programmato (BCWS, Budgeted Cost of Work Scheduled) è una metrica delle prestazioni del progetto che rappresenta la quantità di attività che deve essere completata al momento del calcolo di questa metrica.
author: Lisa
feature: Work Management
exl-id: b9a36333-9430-42bd-99dd-3ad82803b633
source-git-commit: b983a780198743a2b87b4b48cf4d6afdf1cee437
workflow-type: tm+mt
source-wordcount: '621'
ht-degree: 2%

---

# Calcola costo preventivato del lavoro programmato (BCWS)

## Panoramica sul costo preventivato del lavoro programmato (BCWS)

Anche noto come valore pianificato, il costo preventivato del lavoro programmato (BCWS, Budgeted Cost of Work Scheduled) è una metrica delle prestazioni del progetto che rappresenta la quantità di attività che deve essere completata al momento del calcolo di questa metrica.

Adobe Workfront calcola il costo preventivato del lavoro programmato (BCWS) sia per i progetti che per le attività.

Quando si esaminano i valori per il BCWS di un&#39;attività o di un progetto, tenere presente quanto segue:

* Workfront calcola il valore BCWS per un&#39;attività in base alla configurazione del metodo PIM (Performance Index Method) del progetto.

  È possibile configurare il progetto per il calcolo del PIM utilizzando ore o costo e anche il valore BCWS viene calcolato utilizzando gli stessi valori.

  Per informazioni sulla configurazione del metodo di calcolo di BCWS, vedere la sezione [Configurare il metodo di calcolo di BCWS](#configure-how-bcws-is-calculated) in questo articolo.

* Workfront calcola il valore BCWS per un progetto aggiungendo tutti i valori BCWS di tutte le attività padre e delle singole attività del progetto.

  I valori delle attività figlio non vengono aggiunti al file BCWS del progetto.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td>
   <p>Nuovo: Standard</p>
   <p>oppure</p>
   <p>Corrente: Piano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td>Modifica accesso ai progetti</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td>Gestire le autorizzazioni per il progetto</td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurare la modalità di calcolo di BCWS {#configure-how-bcws-is-calculated}

È possibile specificare se il valore BCWS deve essere calcolato in ore o costi configurando il metodo PIM (Performance Index Method) del progetto.

1. Vai a un progetto e fai clic su **Dettagli progetto** nel pannello a sinistra.
1. Nell&#39;area **Finance** individuare il campo **Metodo indice prestazioni** e fare doppio clic su di esso per modificarlo.

   ![Opzioni PIM](assets/pim-options-hour-cost-based-nwe.png)

1. Selezionare una delle opzioni seguenti:

   | Opzione | Modalità di esecuzione del calcolo |
   |---|---|
   | Basato su Ore | Workfront calcola il valore BCWS utilizzando le ore pianificate delle attività. |
   | Basato su Costo | Workfront calcola il valore BCWS utilizzando il Costo pianificato delle attività. |


1. Fai clic su **Salva modifiche**.

   Il valore BCWS delle attività del progetto viene calcolato in base alle ore o ai costi.

## Calcola BCWS

Workfront calcola il costo preventivato del lavoro programmato (BCWS, Budgeted Cost of Work Scheduled) per le attività o i progetti utilizzando le formule seguenti:

```
Task BCWS = Planned Percent Complete x Task Budget
```

```
Project BCWS = SUM(BCWS values of all parent and individual tasks)
```

In questo calcolo vengono utilizzati i seguenti valori:

| Valore utilizzato | Descrizione del valore utilizzato |
|---|---|
| Percentuale pianificata completata | Questo valore indica la percentuale di completamento dell&#39;attività osservando il tempo trascorso tra l&#39;inizio dell&#39;attività e la data corrente. |
| Budget Attività | Questo è il valore per le ore pianificate o il costo pianificato dell&#39;attività. |

Ad esempio, se è oggi 12 febbraio e la durata di un&#39;attività è pianificata dal 10 al 20 febbraio, l&#39;attività deve essere completata al 20% oggi. Se il Budget attività (Costo pianificato) è pari a $10.000, il valore BCWS per l&#39;attività è:

```
Task BCWS = 20% x $10,000 = $2,000
```

## Individuare il file BCWS per un progetto o un&#39;attività

È possibile visualizzare il valore del Costo preventivato del lavoro programmato in un report o in un elenco aggiungendo la colonna BCWS alla visualizzazione.

1. Consente di passare a un elenco di attività o progetti.
1. Espandere il menu **Visualizza** e selezionare **Nuova visualizzazione** o **Personalizza visualizzazione**.

1. Fai clic su **Aggiungi colonna**.
1. Nel campo **Mostra in questa colonna:** inizia a digitare **BCWS** e fai clic su per selezionarlo quando viene visualizzato nell&#39;elenco.

   ![BCWS nella visualizzazione del progetto](assets/bcws-in-project-view.png)

1. Fai clic su **Salva vista**.
1. Il campo **BCWS** viene visualizzato nella visualizzazione.
