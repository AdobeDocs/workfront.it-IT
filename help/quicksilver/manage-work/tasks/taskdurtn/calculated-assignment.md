---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: '''Panoramica sul tipo di durata: Assegnazione calcolata"'
description: L'assegnazione calcolata è un tipo di durata che è possibile impostare per un'attività in Adobe Workfront. Per informazioni generali sui tipi di durata in Workfront, consulta Panoramica sulla durata e sul tipo di durata dell’attività.
author: Alina
feature: Work Management
exl-id: 5f1f6109-5d54-4c3f-9aa5-dc6ce165a1cd
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 0%

---

# Panoramica sul tipo di durata: Assegnazione calcolata

L&#39;assegnazione calcolata è un tipo di durata che è possibile impostare per un&#39;attività in Adobe Workfront. Per informazioni generali sui tipi di durata in Workfront, vedi [Panoramica del tipo di durata e durata dell’attività](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

## Panoramica del tipo di durata dell&#39;assegnazione calcolata

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This Hub issue has a powerpoint that highlights information that is useful to users when using Calculated Assignment duration type. I don't think we can use the powerpoint, because it's old. I also don't know if the things they discuss are still relevant, since the PP is from 2015. I've closed the issue, but I'm putting a link here just in case the info is useful. https://hub.workfront.com/issue/5a9dd7d5007d02a8966014557c23cc89/updates)</p>
-->

* Quando si utilizza un tipo di durata dell&#39;assegnazione calcolata, è necessario specificare sia la Durata sia il numero di ore pianificate per l&#39;attività. Workfront quindi divide la quantità di ore pianificate per la quantità di ore nella durata, quindi per il numero di risorse assegnate all&#39;attività per calcolare la percentuale di allocazione (calcola l&#39;assegnazione) per ciascuna risorsa. Ogni risorsa avrà lo stesso valore per la propria percentuale di allocazione. In questo caso, non è possibile modificare i valori di allocazione per ogni risorsa.
* L&#39;amministratore Workfront o di gruppo può impostare il tipo di durata predefinito del sistema o del gruppo come Assegnazione calcolata. In questo caso, tutte le nuove attività verranno create con questo tipo di durata. Per informazioni su come modificare l&#39;attività e le preferenze relative ai problemi nell&#39;ambito delle preferenze di progetto a livello di sistema o di gruppo, consulta [Configurare le preferenze relative alle attività e ai problemi a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

   In questo caso, l’attività ha un valore predefinito di una durata di un giorno e un valore predefinito di 0 ore pianificate. A meno che il project manager non imposti una durata più accurata e non compili il campo Ora pianificata con una stima realistica, le risorse vengono visualizzate come sottoassegnate.

L&#39;assegnazione calcolata è il tipo di durata preferito nelle situazioni seguenti:

* Quando le assegnazioni hanno una finestra di attività ma non richiedono l&#39;intera durata assegnata per completare il loro lavoro. Ad esempio, ti viene assegnato di consegnare un rapporto al tuo supervisore entro la fine della settimana. Hai una durata di cinque giorni, ma la bozza del documento richiederà solo dieci ore.
* Quando una singola risorsa viene assegnata a un&#39;attività, in quanto il project manager può stimare la durata pianificata e l&#39;entità dello sforzo pianificato indipendentemente l&#39;uno dall&#39;altro.

   È possibile utilizzare il tipo di durata del lavoro calcolato per lo stesso risultato, ma il project manager deve inserire un&#39;allocazione percentuale per la risorsa per influenzare il valore calcolato per le ore pianificate. Ciò rende la pianificazione dei progetti più difficile e dispendiosa dal punto di vista del tempo.

La percentuale di allocazione per ogni risorsa viene calcolata come segue:

```
Planned Hours / Duration / Number of Resources = Allocation Percentage for each resource
```

Ad esempio, nello scenario descritto di seguito, ogni attività ha una Durata di 3 giorni. Il project manager immette manualmente sia la Durata (3 giorni o 24 ore) che l&#39;Ora pianificata e, di conseguenza, viene calcolata la percentuale di allocazione (o percentuale di assegnazione):

![](assets/calcassign-350x80.png)

## Modificare il tipo di durata di un&#39;attività in Assegnazione calcolata

Per informazioni sulla modifica del tipo di durata di un&#39;attività, vedere [Aggiornare il tipo di durata di un&#39;attività](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replaced with new article linked above)</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Go to a task for which you want to change the Duration Type.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel, then in the Overview area double click <strong>Duration Type</strong>. </p> </li>
<li value="3">Select <strong>Calculated Assignment</strong> from the drop-down menu.</li>
<li value="4">Click <strong>Save</strong> <strong>Changes</strong>.</li>
</ol>
-->
