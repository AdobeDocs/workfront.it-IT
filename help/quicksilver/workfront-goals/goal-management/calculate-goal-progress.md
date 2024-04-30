---
product-previous: workfront-goals
navigation-topic: goal-management
title: Panoramica dell’avanzamento e della condizione dell’obiettivo in Obiettivi di Adobe Workfront
description: Il progresso degli obiettivi è guidato da indicatori di progresso come attività, risultati o obiettivi secondari. La condizione dell’obiettivo è determinata dall’avanzamento dell’obiettivo nel momento corrente.
author: Alina
feature: Workfront Goals
exl-id: 3050f7ff-a579-4fb8-82fd-bef850f27c20
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '856'
ht-degree: 1%

---

# Panoramica dell’avanzamento e della condizione dell’obiettivo in Obiettivi di Adobe Workfront

Per utilizzare le funzionalità descritte in questo articolo, l’organizzazione deve disporre dei seguenti elementi:

* Per il nuovo piano e la nuova struttura delle licenze:

   * Un piano Ultimate

     Oppure

     Una licenza aggiuntiva per Adobe Workfront Goals per i piani Prime o Select Adobe Workfront. Per informazioni, consulta [piano Adobe Workfront](https://www.workfront.com/plans).

* Per il piano corrente e la struttura delle licenze:

   * A Pro o superiore
   * Una licenza Adobe Workfront Goals oltre a una licenza Workfront.

Contatta il tuo account manager Workfront per saperne di più su una licenza Workfront Goals.

Per ulteriori informazioni sull’accesso agli obiettivi di Workfront, consulta [Requisiti per l’utilizzo degli obiettivi di Workfront](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).

Adobe Workfront calcola automaticamente il progresso dell’obiettivo in base al progresso dei suoi indicatori di progresso.

## Prerequisiti

Prima di iniziare, è necessario disporre dei seguenti elementi:

* Modello di layout che include l&#39;area Obiettivi nel menu principale.

## Panoramica dell’avanzamento e della soglia dell’obiettivo

Dopo aver attivato un obiettivo, Workfront Goals inizia a calcolarne l’avanzamento e la condizione e visualizza i seguenti indicatori quando passi il cursore del mouse sul campo Progress (Avanzamento):

| Indicatore | Descrizione indicatore |
|---|---|
| Percentuale di completamento effettiva | Quanta parte dell&#39;obiettivo è stato effettivamente raggiunto finora. Workfront Goals calcola questo valore calcolando la media della percentuale di completamento di tutti gli indicatori di avanzamento associati all&#39;obiettivo. |
| Percentuale di completamento prevista | Quanto dell’obiettivo deve essere completato finora affinché l’obiettivo possa essere completato in tempo. Obiettivi Workfront calcola questo valore osservando la Durata dell’obiettivo e il momento nel tempo corrente. Se l’obiettivo deve essere completato in tempo, questo valore dovrebbe essere visualizzato all’ora corrente. |
| Avanzamento | Etichetta che indica se l’obiettivo è nel target da completare in tempo, o se è a rischio o ha problemi a non completarlo. |

![](assets/in-trouble-goal-progress-expanded.png)

<!--drafted for the redesign: replace the screen shot above with the redesigned one which is white, not black-->

* [Percentuale di completamento effettiva](#actual-percent-complete)
* [Percentuale di completamento prevista](#expected-percent-complete)
* [Avanzamento e condizione](#progress)

### Percentuale di completamento effettiva {#actual-percent-complete}

Obiettivi Workfront calcola automaticamente la percentuale effettiva di completamento di un obiettivo in base alla media percentuale di completamento degli indicatori di avanzamento dell’obiettivo.

I seguenti elementi sono considerati indicatori di progresso per gli obiettivi:

* Risultati

  Per informazioni sull’aggiunta di risultati agli obiettivi, consulta [Aggiungere risultati agli obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/results-and-activities/add-results-to-goals.md).

* Attività

  Per informazioni sull’aggiunta di attività, compresi i progetti, agli obiettivi, vedi [Aggiungere attività agli obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/results-and-activities/add-activities-to-goals.md).

* Obiettivi figlio allineati

  Per informazioni sugli obiettivi principali e secondari, consulta [Allineare gli obiettivi collegandoli in Obiettivi di Adobe Workfront](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

  Obiettivi Workfront calcola la percentuale effettiva di completamento utilizzando la formula seguente:

  ```
  Actual percent complete of goal = SUM(Percent complete of goal progress indicators)* 100 / Number of progress indicators
  ```

  Ad esempio, se un obiettivo ha un Risultato completato al 20%, una Barra di avanzamento manuale completata al 30%, un progetto completato al 10% e un obiettivo secondario completato al 40%, l’obiettivo completato in percentuale è del 25%.

### Percentuale di completamento prevista {#expected-percent-complete}

Obiettivi Workfront calcola automaticamente la percentuale di completamento prevista di un obiettivo in base al numero totale di giorni nella durata dell’obiettivo e al numero di giorni trascorsi dalla data di inizio dell’obiettivo.

Obiettivi Workfront calcola la percentuale di completamento prevista utilizzando la formula seguente:

```
Expected percent complete of goal = Number of days since the goal start date * 100/ Number of days in the goal duration
```

Ad esempio, se un obiettivo deve essere completato entro 90 giorni e oggi è il 45° giorno di tale durata, la percentuale di completamento prevista è del 50%.

### Avanzamento e condizione {#progress}

Obiettivi Workfront calcola una percentuale di avanzamento e assegna un’etichetta di avanzamento agli obiettivi, in base alla percentuale di completamento prevista raggiunta nel momento corrente. Il colore della barra della percentuale di completamento dell&#39;obiettivo cambia per indicare l&#39;avanzamento dell&#39;obiettivo.

Anche la condizione dell’obiettivo viene aggiornata, di conseguenza, per indicare se l’obiettivo è sul target da completare in tempo o se è in ritardo.

Workfront Goals calcola la percentuale di avanzamento di un obiettivo utilizzando la formula seguente:

```
Goal progress percentage = Actual percent complete * 100 / Expected percent complete
```

Ad esempio, se la percentuale di completamento prevista è del 53% al momento e la percentuale di completamento effettiva è del 30%, la percentuale di completamento obiettivo è del 56%. Gli obiettivi di Workfront etichettano questo obiettivo con una condizione di &quot;In Trouble&quot;.

Il grafico seguente illustra la relazione tra le etichette delle condizioni e la percentuale di avanzamento:

![](assets/progress-status-labels-charted-after-match-with-project-condition-350x147.png)

La tabella seguente elenca le etichette delle condizioni di obiettivo e le percentuali di avanzamento dell’obiettivo associate a ciascuna etichetta.

>[!TIP]
>
>Le etichette delle condizioni dell’obiettivo corrispondono al nome e al colore della condizione del progetto Workfront.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>Nome avanzamento obiettivo</b></td> 
   <td><b>Definizione avanzamento obiettivo</b></td> 
   <td><b>Percentuale di avanzamento obiettivo</b></td> 
   <td><b>Colore della barra della percentuale di completamento</b></td> 
   <td><b>Icona indicatore di condizione</b></td> 
  </tr> 
  <tr> 
   <td>Nuovo</td> 
   <td> <p>L’obiettivo è stato appena creato e non sta ancora registrando l’avanzamento. L’avanzamento di un obiettivo viene visualizzato come Nuovo finché non viene aggiornato per la prima volta. </p> <p>Per informazioni sull’aggiornamento dell’avanzamento dell’obiettivo, consulta <a href="../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md" class="MCXref xref">Aggiornamento dell’avanzamento dell’obiettivo in Obiettivi di Adobe Workfront</a>.</p> </td> 
   <td>Nessuna percentuale</td> 
   <td>Nessuna barra</td> 
   <td><img src="assets/new-goal-icon-condition.png" alt="new_goal_icon_condition.png"></td>
  </tr> 
  <tr> 
   <td> <p><span>On Target</span> </p> </td> 
   <td>L’obiettivo funziona come previsto ed è molto probabile che venga completato in tempo. </td> 
   <td>90-100%</td> 
   <td>Verde</td> 
    <td><img src="assets/on-target-icon-condition.png" alt="on_target_icon_condition.png"></td>
  </tr> 
  <tr> 
   <td> <p><span>A Rischio</span> </p> </td> 
   <td>L'obiettivo è in ritardo, ma potrebbe essere ancora possibile completarlo in tempo. </td> 
   <td>70-89,99%</td> 
   <td>Giallo</td>
   <td><img src="assets/at-risk-icon-condition.png" alt="at_risk_icon_condition.png"></td> 
  </tr> 
  <tr> 
   <td> <p><span>In difficoltà</span> </p> </td> 
   <td> <p>È molto probabile che l’obiettivo non venga completato in tempo. </p> </td> 
   <td>0-69,99%</td> 
   <td>Rosso</td> 
   <td><img src="assets/in-trouble-icon-condition.png" alt="in_trouble_icon_condition.png"></td> 
  </tr> 
 </tbody> 
</table>