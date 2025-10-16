---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: 'Panoramica sul tipo di durata: assegnazione calcolata'
description: L'assegnazione calcolata è un tipo di durata che è possibile impostare per un'attività in Adobe Workfront. Per informazioni generali sui tipi di durata in Workfront, vedere Panoramica sulla durata e sul tipo di durata dell'attività.
author: Alina
feature: Work Management
exl-id: 5f1f6109-5d54-4c3f-9aa5-dc6ce165a1cd
source-git-commit: c1b8af0d8a95714bb597db7a429794773358cf05
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 0%

---

# Panoramica sul tipo di durata: assegnazione calcolata

<!-- Audited: 5/2025 -->

L&#39;assegnazione calcolata è un tipo di durata che è possibile impostare per un&#39;attività in Adobe Workfront. Per informazioni generali sui tipi di durata in Workfront, vedere [Panoramica sulla durata dell&#39;attività e sul tipo di durata](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

## Panoramica del tipo di durata dell&#39;assegnazione calcolata

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This Hub issue has a powerpoint that highlights information that is useful to users when using Calculated Assignment duration type. I don't think we can use the powerpoint, because it's old. I also don't know if the things they discuss are still relevant, since the PP is from 2015. I've closed the issue, but I'm putting a link here just in case the info is useful. https://hub.workfront.com/issue/5a9dd7d5007d02a8966014557c23cc89/updates)</p>
-->

* Quando si utilizza un Tipo di durata assegnazione calcolata, è necessario specificare sia una durata che un numero di ore pianificate per l&#39;attività. Workfront divide quindi la quantità di ore pianificate per la quantità di ore nella Durata e quindi per il numero di risorse assegnate all&#39;attività per calcolare la percentuale di allocazione (calcola l&#39;assegnazione) per ciascuna risorsa. Ogni risorsa avrà lo stesso valore per la percentuale di allocazione. In questo caso, non è possibile modificare i valori di allocazione per ogni risorsa.
* Il Workfront o un amministratore di gruppo può impostare il Tipo di durata predefinito del sistema o del gruppo come Assegnazione calcolata. In questo caso, tutte le nuove attività verranno create con questo Tipo di durata. Per informazioni sulla modifica delle preferenze di attività e problemi come parte delle preferenze di progetto a livello di sistema o di gruppo, consulta [Configurare le preferenze di problema e attività a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

  In questo caso, l&#39;attività ha una durata predefinita di un giorno e una durata predefinita di 0 ore. A meno che il project manager non imposti una durata più precisa e non popola il campo Ore pianificate con una stima realistica, le risorse appaiono sottoassegnate.

Assegnazione calcolata è il tipo di durata preferito nelle situazioni seguenti:

* Quando le assegnazioni hanno una finestra di attività ma non prendono l&#39;intera Durata assegnata per completare il loro lavoro. Ad esempio, ti viene assegnato il compito di consegnare un rapporto al tuo supervisore entro la fine della settimana. Hai una durata di cinque giorni, ma la bozza del documento richiederà solo 10 ore.
* Quando a un&#39;attività viene assegnata una singola risorsa perché il project manager può stimare la durata pianificata e la quantità di impegno pianificata in modo indipendente l&#39;una dall&#39;altra.

  È possibile utilizzare il tipo di durata del lavoro calcolato per lo stesso risultato, ma il project manager deve immettere un&#39;allocazione percentuale per la risorsa per poter influire sul valore calcolato per le ore pianificate. Ciò rende la pianificazione del progetto più difficile e dispendiosa in termini di tempo.

La percentuale di allocazione per ogni risorsa viene calcolata nel modo seguente:

```
Planned Hours / Duration / Number of Resources = Allocation Percentage for each resource
```

Ad esempio, nello scenario descritto di seguito, ogni attività ha una durata di 3 giorni. Il project manager immette manualmente sia la durata (3 giorni o 24 ore) che le ore pianificate e di conseguenza viene calcolata la percentuale di allocazione (o percentuale di assegnazione):

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
