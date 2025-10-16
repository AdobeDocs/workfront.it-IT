---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: 'Panoramica sul tipo di durata: basata sulle risorse'
description: Effort Driven è un tipo di durata che è possibile impostare per un'attività in Adobe Workfront. Per informazioni generali sui tipi di durata in Workfront, vedere Panoramica sulla durata e sul tipo di durata dell'attività.
author: Alina
feature: Work Management
exl-id: 3c8534f7-02d0-4404-a37b-0ef6360e8efc
source-git-commit: c1b8af0d8a95714bb597db7a429794773358cf05
workflow-type: tm+mt
source-wordcount: '862'
ht-degree: 1%

---

# Panoramica sul tipo di durata: basata sulle risorse

Effort Driven è un tipo di durata che è possibile impostare per un&#39;attività in Adobe Workfront. Per informazioni generali sui tipi di durata in Workfront, vedere [Panoramica sulla durata dell&#39;attività e sul tipo di durata](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

## Panoramica del tipo di durata basata sulle risorse

Il Workfront o un amministratore di gruppo può impostare il Tipo di durata predefinito del sistema o del gruppo come Basato sull&#39;impegno. In questo caso, tutte le nuove attività verranno create con questo Tipo di durata. Per informazioni sulla modifica delle preferenze di attività e problemi come parte delle preferenze di progetto a livello di sistema o di gruppo, consulta [Configurare le preferenze di problema e attività a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

In questo scenario, esiste il rischio di abbreviare arbitrariamente il piano del progetto, a meno che il project manager non dedichi del tempo a valutare se l&#39;attività è effettivamente un&#39;attività basata sulle risorse.

Utilizza Impegno per:

* Determinare la durata pianificata in base al numero di risorse disponibili per l&#39;attività. La durata è uguale alle ore pianificate. La Durata Pianificata è uguale alle Ore Pianificate divisa per il numero di assegnatari.

  Il livello di impegno applicato all&#39;attività determina la divisione del lavoro e la durata.

* Monitora il numero totale di ore dedicate a un&#39;attività quando vengono assegnate più risorse.

  Quando si aggiungono risorse, la durata pianificata dell&#39;attività diminuisce. (Il principio &quot;molte mani fanno funzionare la luce&quot; illustra l&#39;effetto che questo Tipo di Durata ha sulla Durata Pianificata di un&#39;attività.)

Nelle sezioni seguenti vengono fornite informazioni più dettagliate sul modo in cui Workfront calcola la durata pianificata di un&#39;attività basata sulle risorse e sull&#39;effetto dell&#39;aggiunta di risorse sull&#39;attività con questo tipo di durata.

## Panoramica della formula Tipo di durata basata sull&#39;impegno

La formula per il calcolo della Durata pianificata per un&#39;attività con Tipo di durata impostato su Impegno dipende dalla percentuale di allocazione di ogni risorsa assegnata all&#39;attività. Nel caso di un&#39;attività basata sulle risorse, Workfront calcola le ore pianificate dell&#39;attività e sono sempre uguali alla durata dell&#39;attività:

```
Planned Hours (in hours) = Duration (in days)
```

È possibile regolare manualmente la durata dell&#39;attività.

Workfront presuppone che vi siano 8 ore lavorative in una giornata lavorativa. L’amministratore del Workfront o del gruppo definisce le ore per giorno lavorativo con l’impostazione Tipiche di ore per giorno lavorativo nelle Preferenze progetto in Configurazione. Per ulteriori informazioni sulla modifica delle preferenze di attività e problemi come parte delle preferenze di progetto a livello di sistema, consulta [Configurare le preferenze di problema e attività a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

>[!TIP]
>
>Workfront considera la pianificazione per ogni risorsa assegnata all&#39;attività per determinare la percentuale di allocazione per ogni risorsa dell&#39;attività. Per informazioni sulla creazione e l&#39;assegnazione di pianificazioni agli utenti, vedere [Creare una pianificazione](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

Considera i seguenti scenari:

* [Le risorse sono allocate al 100% all&#39;attività](#resources-are-allocated-100-to-the-task)
* [Le risorse vengono allocate per varie percentuali di tempo all&#39;attività](#resources-are-allocated-for-various-percentages-of-time-to-the-task)

### Le risorse vengono allocate al 100% all&#39;attività {#resources-are-allocated-100-to-the-task}

Questa formula presuppone che tutte le risorse siano allocate al 100% all&#39;attività.

```
Planned Duration = (Planned Hours / Number of Resources) / 8
```

Questo calcolo presuppone che il numero di ore in una giornata lavorativa normale sia 8. L&#39;equazione include questo valore in modo che la durata pianificata venga visualizzata in giorni.

### Le risorse vengono allocate per varie percentuali di tempo all&#39;attività {#resources-are-allocated-for-various-percentages-of-time-to-the-task}

Poiché ogni risorsa assegnata può avere un livello di allocazione univoco, la formula effettiva tiene conto dei seguenti valori di allocazione:

```
Planned Duration = (Planned Hours / SUM(Percent allocation for each resource for the task)) / 8
```

Questo calcolo presuppone che il numero di ore in una giornata lavorativa normale sia 8. L&#39;equazione include questo valore in modo che la durata pianificata venga visualizzata in giorni.

## L&#39;effetto dell&#39;aggiunta di più risorse a un&#39;attività

Quando si aggiungono o si rimuovono assegnatari a un&#39;attività con il tipo di durata basata sulle risorse, la durata e le ore pianificate non cambiano. Tuttavia, la Durata Pianificata cambia.

Nell’esempio seguente, l’impostazione Ore tipiche per giorno lavorativo è 8 nelle Preferenze progetto nella configurazione del sistema. Poiché la durata è di 3 giorni, le ore pianificate vengono impostate su 24 (3 giorni x 8 ore per giorno lavorativo = 24 ore pianificate).

>[!NOTE]
>
>Quando si utilizza il vincolo dell&#39;attività Date fisse, la durata pianificata rimane invariata quando si aggiungono o si rimuovono gli assegnatari, mentre la durata e le ore pianificate vengono regolate. Quando si utilizza un vincolo attività diverso dalle date fisse, la durata pianificata viene regolata.

Nella tabella seguente viene illustrato il modo in cui la durata pianificata cambia quando si aggiungono risorse all&#39;attività:

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th> <p><strong>Numero di assegnatari (ogni 100% allocato)</strong> </p> </th> 
   <th> <p><strong>Durata</strong> </p> </th> 
   <th> <p><strong>Ore pianificate</strong> </p> </th> 
   <th><strong>Durata Pianificata</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> </td> 
   <td> <p>1</p> </td> 
   <td> <p>3 giorni</p> </td> 
   <td> <p>24 Hours</p> <p>(3 giorni x 8 ore per giorno lavorativo = 24 ore pianificate)</p> </td> 
   <td> <p>3 giorni</p> <p>(24 ore pianificate/1 assegnatario = 3 giorni)</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> <p>2</p> </td> 
   <td> <p>3 giorni</p> </td> 
   <td> <p>24 Hours</p> <p>(3 giorni x 8 ore per giorno lavorativo = 24 ore pianificate)</p> </td> 
   <td> <p>1,5 giorni</p> <p>(24 ore pianificate/2 assegnatari = 12 ore o 1,5 giorni)</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> <p>3</p> </td> 
   <td> <p>3 giorni</p> </td> 
   <td> <p>24 Hours</p> <p>(3 giorni x 8 ore per giorno lavorativo = 24 ore pianificate)</p> </td> 
   <td> <p>1 giorno</p> <p>(24 ore pianificate / 3 assegnatari = 8 ore o 1 giorno)</p> </td> 
  </tr> 
 </tbody> 
</table>

## Modificare il tipo di durata di un&#39;attività in Basato sulle risorse

Per informazioni sulla modifica del tipo di durata di un&#39;attività, vedere [Aggiornare il tipo di durata di un&#39;attività](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replaced with new article linked above)</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Go to a task for which you want to change the Duration Type.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel, then in the Overview area click <strong>Duration Type</strong>. </p> </li>
<li value="3"> <p>Select <strong>Effort Driven</strong> from the drop-down menu.</p> </li>
<li value="4">Click <strong>Save</strong><strong>Changes</strong>.</li>
</ol>
-->
