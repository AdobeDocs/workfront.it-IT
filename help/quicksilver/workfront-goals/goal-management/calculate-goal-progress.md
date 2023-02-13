---
product-previous: workfront-goals
navigation-topic: goal-management
title: Panoramica dell’avanzamento e della condizione dell’obiettivo in Obiettivi di Adobe Workfront
description: Il progresso dell'obiettivo è guidato da indicatori di progresso come attività, risultati o obiettivi per bambini. La condizione dell’obiettivo è determinata dal progresso dell’obiettivo al momento attuale.
author: Alina
feature: Workfront Goals
exl-id: 3050f7ff-a579-4fb8-82fd-bef850f27c20
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '821'
ht-degree: 1%

---

# Panoramica dell’avanzamento e della condizione dell’obiettivo in Obiettivi di Adobe Workfront

<!--drafted for P&P release: the note at the top will need to be replaced with this:

Your organization must have the following to use the functionality described in this article:

* For the legacy plan and license structure: 

  * A Pro or higher [Adobe Workfront plan](https://www.workfront.com/plans). 
  * An Adobe Workfront Goals license in addition to a Workfront license.

* For the current plan and license structure:

  * An Ultimate plan 
    
    Or
    
    An additional license for Adobe Workfront Goals for the Prime or Select Adobe Workfront plans. <is there a link we can add here for the plans and what they contain?!>

Contact your Workfront account manager to learn about a Workfront Goals license.

For additional information about access to Workfront Goals, see [Requirements to use Workfront Goals](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
-->

>[!NOTE]
>
>Per utilizzare la funzionalità descritta in questo articolo, l’organizzazione deve disporre delle seguenti caratteristiche:
>
>* A Pro o superiore [piano Adobe Workfront](https://www.workfront.com/plans).
>* Una licenza Adobe Workfront Obiettivi oltre a una licenza Workfront.
>
>Contatta il tuo account manager Workfront per saperne di più su una licenza di Workfront Obiettivi .
>Per ulteriori informazioni sull&#39;accesso agli obiettivi di Workfront, vedi [Requisiti per l&#39;utilizzo degli obiettivi di Workfront](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).

Adobe Workfront calcola automaticamente l’avanzamento dell’obiettivo in base all’avanzamento dei suoi indicatori di avanzamento.

## Prerequisiti

È necessario disporre dei seguenti elementi prima di poter iniziare:

* Modello di layout che include l’area Obiettivi del menu principale.

## Panoramica del progresso e della soglia dell’obiettivo

Dopo aver attivato un obiettivo, Obiettivi di Workfront inizia a calcolarne l’avanzamento e la condizione e visualizza i seguenti indicatori quando passi il cursore del mouse sul campo Avanzamento :

| Indicatore | Descrizione indicatore |
|---|---|
| Percentuale effettiva completata | Quanto dell&#39;obiettivo è stato effettivamente raggiunto finora. Obiettivi di Workfront calcola questo valore calcolando la media della percentuale di completamento di tutti gli indicatori di avanzamento associati all’obiettivo. |
| Percentuale di completamento prevista | Quanto dell&#39;obiettivo dovrebbe essere completato finora per completare l&#39;obiettivo in tempo. Obiettivi di Workfront calcola questo valore guardando la Durata dell’obiettivo e il momento nel tempo corrente. L&#39;obiettivo deve visualizzare questo valore al momento attuale, se deve essere completato in tempo. |
| Avanzamento | Etichetta che indica se l’obiettivo è su target da completare in tempo, o se è a rischio o in difficoltà a non essere completato. |

![](assets/in-trouble-goal-progress-expanded.png)

<!--drafted for the redesign: replace the screen shot above with the redesigned one which is white, not black-->

* [Percentuale effettiva completata](#actual-percent-complete)
* [Percentuale di completamento prevista](#expected-percent-complete)
* [Avanzamento e condizione](#progress)

### Percentuale effettiva completata {#actual-percent-complete}

Obiettivi di Workfront calcola automaticamente la percentuale effettiva di completamento di un obiettivo in base alla media percentuale completa degli indicatori di avanzamento dell&#39;obiettivo.

Sono considerati indicatori di progresso per gli obiettivi i seguenti elementi:

* Risultati

   Per informazioni sull’aggiunta di risultati agli obiettivi, consulta [Aggiungere risultati agli obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/results-and-activities/add-results-to-goals.md).

* Attività

   Per informazioni sull’aggiunta di attività, compresi progetti agli obiettivi, consulta [Aggiungere attività agli obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/results-and-activities/add-activities-to-goals.md).

* Obiettivi per bambini allineati

   Per informazioni sugli obiettivi padre e figlio, vedi [Allineare gli obiettivi collegandoli negli obiettivi di Adobe Workfront](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

   Obiettivi di Workfront calcola la percentuale effettiva di completamento utilizzando la seguente formula:

   ```
   Actual percent complete of goal = SUM(Percent complete of goal progress indicators)* 100 / Number of progress indicators
   ```

   Ad esempio, se un obiettivo ha un risultato completato del 20%, una barra di avanzamento manuale completata al 30%, un progetto completato al 10% e un obiettivo figlio completato al 40%, l’obiettivo percentuale di completamento è del 25%.

### Percentuale di completamento prevista {#expected-percent-complete}

Obiettivi di Workfront calcola automaticamente la percentuale di completamento prevista di un obiettivo in base al numero totale di giorni nella durata dell&#39;obiettivo e al numero di giorni passati dalla data di inizio dell&#39;obiettivo.

Obiettivi di Workfront calcola la percentuale di completamento prevista utilizzando la seguente formula:

```
Expected percent complete of goal = Number of days since the goal start date * 100/ Number of days in the goal duration
```

Ad esempio, se un obiettivo deve essere completato in 90 giorni e oggi è il 45° giorno di quella durata, la percentuale di completamento prevista è del 50%.

### Avanzamento e condizione {#progress}

Obiettivi di Workfront calcola una percentuale di avanzamento e assegna un’etichetta di avanzamento agli obiettivi, in base alla percentuale di completamento previsto raggiunta nel momento corrente. Il colore della barra di completamento della percentuale dell&#39;obiettivo cambia per indicare l&#39;avanzamento dell&#39;obiettivo.

Anche la condizione dell’obiettivo viene aggiornata, di conseguenza, per indicare se l’obiettivo è su target da completare in tempo o se è in ritardo.

Obiettivi di Workfront calcola la percentuale di avanzamento di un obiettivo utilizzando la seguente formula:

```
Goal progress percentage = Actual percent complete * 100 / Expected percent complete
```

Ad esempio, se la percentuale di completamento prevista è del 53% al momento attuale e la percentuale di completamento effettivo è del 30%, la percentuale di completamento dell’avanzamento dell’obiettivo è del 56%. Obiettivi di Workfront assegna all’obiettivo la condizione &quot;In Trouble&quot; (In Trouble).

Il grafico seguente illustra la relazione tra le etichette della condizione e la percentuale di avanzamento:

![](assets/progress-status-labels-charted-after-match-with-project-condition-350x147.png)

Nella tabella seguente sono elencate le etichette della condizione obiettivo e le percentuali di avanzamento obiettivo associate a ciascuna etichetta.

>[!TIP]
>
>Le etichette della condizione dell’obiettivo corrispondono al nome e al colore della condizione del progetto Workfront.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>Nome dell'avanzamento dell'obiettivo</b></td> 
   <td><b>Definizione dell'avanzamento dell'obiettivo</b></td> 
   <td><b>Percentuale di progresso obiettivo</b></td> 
   <td><b>Colore della barra completa percentuale</b></td> 
   <td><b>Icona dell’indicatore di condizione</b></td> 
  </tr> 
  <tr> 
   <td>Nuovo</td> 
   <td> <p>L'obiettivo è stato appena creato e non registra ancora l'avanzamento. L’avanzamento di un obiettivo viene visualizzato come Nuovo fino a quando qualcuno non ne aggiorna l’avanzamento per la prima volta. </p> <p>Per informazioni sull'aggiornamento dell'avanzamento dell'obiettivo, vedi <a href="../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md" class="MCXref xref">Aggiornare lo stato dell’obiettivo negli obiettivi di Adobe Workfront</a>.</p> </td> 
   <td>Nessuna percentuale</td> 
   <td>Nessuna barra</td> 
   <td><img src="assets/new-goal-icon-condition.png" alt="new_go_icon_condition.png"></td>
  </tr> 
  <tr> 
   <td> <p><span>Puntuale</span> </p> </td> 
   <td>L'obiettivo funziona come previsto ed è molto probabile che venga completato in tempo. </td> 
   <td>90-100%</td> 
   <td>Verde</td> 
    <td><img src="assets/on-target-icon-condition.png" alt="on_target_icon_condition.png"></td>
  </tr> 
  <tr> 
   <td> <p><span>A Rischio</span> </p> </td> 
   <td>L'obiettivo è in ritardo, ma potrebbe ancora essere possibile completarlo in tempo. </td> 
   <td>70-89.99%</td> 
   <td>Giallo</td>
   <td><img src="assets/at-risk-icon-condition.png" alt="at_risk_icon_condition.png"></td> 
  </tr> 
  <tr> 
   <td> <p><span>In difficoltà</span> </p> </td> 
   <td> <p>È molto probabile che l'obiettivo non venga completato in tempo. </p> </td> 
   <td>0-69.99%</td> 
   <td>Rosso</td> 
   <td><img src="assets/in-trouble-icon-condition.png" alt="in_trou_icon_condition.png"></td> 
  </tr> 
 </tbody> 
</table>