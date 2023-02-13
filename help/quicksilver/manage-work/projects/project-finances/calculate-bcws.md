---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcola costo preventivato del lavoro programmato (BCWS)
description: Anche noto come Valore pianificato, il costo preventivato del lavoro programmato (BCWS) è una metrica di prestazioni del progetto che rappresenta la quantità dell'attività che deve essere stata completata al momento del calcolo di questa metrica.
author: Alina
feature: Work Management
exl-id: b9a36333-9430-42bd-99dd-3ad82803b633
source-git-commit: 1d5de5ff0ebebd84482507c71730cfbd05c513a5
workflow-type: tm+mt
source-wordcount: '644'
ht-degree: 0%

---

# Calcola costo preventivato del lavoro programmato (BCWS)

## Panoramica del costo preventivato del lavoro programmato (BCWS)

Anche noto come Valore pianificato, il costo preventivato del lavoro programmato (BCWS) è una metrica di prestazioni del progetto che rappresenta la quantità dell&#39;attività che deve essere stata completata al momento del calcolo di questa metrica.

Adobe Workfront calcola il costo preventivato del lavoro programmato (BCWS) sia per i progetti che per le attività.

Quando rivedi i valori per BCWS su un&#39;attività o un progetto, considera quanto segue:

* Workfront calcola il BCWS per un&#39;attività in base alla configurazione per il metodo di indice delle prestazioni (PIM) del progetto.

   È possibile configurare il progetto per calcolare il PIM utilizzando ore o costi; inoltre, il BCWS viene calcolato utilizzando gli stessi valori.

   Per informazioni sulla configurazione del calcolo del BCWS, consulta la sezione . [Configurare il calcolo di BCWS](#configure-how-bcws-is-calculated) in questo articolo.

* Workfront calcola il BCWS per un progetto aggiungendo tutti i valori BCWS da tutte le attività principali e dalle singole attività nel progetto.

   I valori delle attività figlio non vengono aggiunti al BCWS del progetto.

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
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica accesso a progetti</p> <p>Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestisci le autorizzazioni per il progetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Configurare il calcolo di BCWS {#configure-how-bcws-is-calculated}

Puoi configurare il calcolo del BCWS in ore o costi configurando il metodo PIM (Performance Index Method) del progetto.

1. Vai a un progetto e fai clic su **Dettagli progetto** nel pannello a sinistra.
1. In **Finanza** area, individuare **Metodo indice prestazioni** e fai doppio clic su di esso per modificarlo.

   ![](assets/pim-options-hour-cost-based-nwe.png)

1. Seleziona tra le seguenti opzioni:

   | Opzione | Modalità di esecuzione del calcolo |
   |---|---|
   | Basato su Ore | Workfront calcola il BCWS utilizzando l&#39;orario pianificato delle attività. |
   | Basato su Costo | Workfront calcola il BCWS utilizzando il costo pianificato delle attività. |


1. Fai clic su **Salva modifiche**.

   Il BCWS delle attività del progetto viene calcolato utilizzando ore o costi.

## Calcola BCWS

Workfront calcola il costo preventivato del lavoro programmato (BCWS) per le attività o i progetti utilizzando le seguenti formule:

```
Task BCWS = Planned Percent Complete x Task Budget
```

```
Project BCWS = SUM(BCWS values of all parent and individual tasks)
```

In questo calcolo vengono utilizzati i seguenti valori:

| Valore utilizzato | Descrizione del valore utilizzato |
|---|---|
| Percentuale pianificata completata | Questo è ciò che la percentuale di completamento dell&#39;attività dovrebbe essere osservando il tempo trascorso tra l&#39;inizio dell&#39;attività e oggi. |
| Budget attività | Valore per l&#39;ora pianificata o il costo pianificato dell&#39;attività. |

Ad esempio, se oggi è il 12 febbraio e un&#39;attività è prevista per la durata dal 10 febbraio al 20 febbraio, l&#39;attività dovrebbe essere completa oggi al 20%. Se il budget attività (costo pianificato) è di $10.000, il valore BCWS per l&#39;attività è:

```
Task BCWS = 20% x $10,000 = $2,000
```

## Individuare il BCWS per un progetto o un&#39;attività

È possibile visualizzare il valore del costo preventivato del lavoro programmato in un rapporto o in un elenco, aggiungendo la colonna BCWS alla visualizzazione.

1. Passare a un elenco di attività o progetti.
1. Espandi la **Visualizza** menu e seleziona **Nuova vista** o **Personalizza visualizzazione**.

1. Fai clic su **Aggiungi colonna**.
1. In **Mostra in questa colonna:** battitura inizio campo **BCWS** e fai clic su per selezionarlo quando viene visualizzato nell’elenco.

   ![](assets/bcws-in-project-view.png)

1. Fai clic su **Salva visualizzazione**.
1. La **BCWS** il campo viene visualizzato nella visualizzazione.
