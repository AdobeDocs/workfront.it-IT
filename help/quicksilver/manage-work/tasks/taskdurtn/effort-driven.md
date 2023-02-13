---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: '''Panoramica sul tipo di durata: Sforzo Guidato"'
description: Sforzo guidato è un tipo di durata che è possibile impostare per un'attività in Adobe Workfront. Per informazioni generali sui tipi di durata in Workfront, consulta Panoramica sulla durata e sul tipo di durata dell’attività.
author: Alina
feature: Work Management
exl-id: 3c8534f7-02d0-4404-a37b-0ef6360e8efc
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '821'
ht-degree: 1%

---

# Panoramica sul tipo di durata: Guida allo sforzo

Sforzo guidato è un tipo di durata che è possibile impostare per un&#39;attività in Adobe Workfront. Per informazioni generali sui tipi di durata in Workfront, vedi [Panoramica del tipo di durata e durata dell’attività](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

## Panoramica del tipo di durata guidata dello sforzo

L&#39;amministratore Workfront o di gruppo può impostare il tipo di durata predefinito del sistema o del gruppo come Unità di sforzo. In questo caso, tutte le nuove attività verranno create con questo tipo di durata. Per informazioni su come modificare l&#39;attività e le preferenze relative ai problemi nell&#39;ambito delle preferenze di progetto a livello di sistema o di gruppo, consulta [Configurare le preferenze relative alle attività e ai problemi a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

In questo scenario, esiste il rischio di accorciare arbitrariamente il piano di progetto, a meno che tu, in qualità di project manager, non ti occupi del tempo necessario per considerare se l&#39;attività è effettivamente un&#39;attività guidata da uno sforzo.

Utilizzare Effort Driven per:

* Determina la durata pianificata in base al numero di risorse disponibili per l&#39;attività. La durata è uguale a Ora pianificata. La durata prevista è uguale a Ore pianificate divise per il numero di assegnatari.

   Il livello di sforzo applicato all&#39;attività determina la divisione del lavoro e la durata.

* Tenere traccia del numero totale di ore trascorse su un&#39;attività quando vengono assegnate più risorse.

   Man mano che vengono aggiunte risorse, la Durata pianificata dell’attività diminuisce. (Il principio di &quot;molte mani fanno funzionare la luce&quot; illustra l&#39;effetto che questo tipo di durata ha sulla durata pianificata di un&#39;attività.)

Le sezioni seguenti forniscono informazioni più dettagliate su come Workfront calcola la durata pianificata di un&#39;attività guidata da sforzo e sull&#39;effetto che l&#39;aggiunta di risorse ha sull&#39;attività con questo tipo di durata.

## Panoramica della formula del tipo di Durata guidata sforzo

La formula per il calcolo della durata prevista per un&#39;attività con un tipo di sforzo di durata dipende dalla percentuale di allocazione di ogni risorsa assegnata all&#39;attività. Nel caso di un&#39;attività guidata da sforzo, Workfront calcola gli orari pianificati dell&#39;attività e sono sempre uguali alla durata dell&#39;attività:

```
Planned Hours (in hours) = Duration (in days)
```

È possibile regolare manualmente la durata dell&#39;attività.

Workfront presuppone che ci siano 8 ore lavorative in un giorno lavorativo. L’amministratore di Workfront o di gruppo definisce le ore per giorno lavorativo con l’impostazione Ore tipiche per giorno di lavoro nelle preferenze del progetto in Configurazione. Per ulteriori informazioni sulla modifica dell&#39;attività e sulle preferenze relative ai problemi nell&#39;ambito delle preferenze di progetto a livello di sistema, consulta [Configurare le preferenze relative alle attività e ai problemi a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

>[!TIP]
>
>Workfront considera la pianificazione per ogni risorsa assegnata all&#39;attività per determinare la percentuale di allocazione per ogni risorsa per l&#39;attività. Per informazioni sulla creazione e l&#39;assegnazione di pianificazioni agli utenti, consulta [Creare una pianificazione](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

Considera i seguenti scenari:

* [Le risorse vengono assegnate al 100% per l&#39;attività](#resources-are-allocated-100-to-the-task)
* [Le risorse vengono assegnate per varie percentuali di tempo all&#39;attività](#resources-are-allocated-for-various-percentages-of-time-to-the-task)

### Le risorse vengono assegnate al 100% per l&#39;attività {#resources-are-allocated-100-to-the-task}

Questa formula presuppone che tutte le risorse siano allocate al 100% all&#39;attività.

```
Planned Duration = (Planned Hours / Number of Resources) / 8
```

Questo calcolo presuppone che il numero di ore in un normale giorno lavorativo sia 8. L&#39;equazione include questo valore in modo che la Durata pianificata venga visualizzata in giorni.

### Le risorse vengono assegnate per varie percentuali di tempo all&#39;attività {#resources-are-allocated-for-various-percentages-of-time-to-the-task}

Poiché ogni risorsa assegnata può avere un livello di allocazione univoco, la formula effettiva tiene conto di questi valori di allocazione:

```
Planned Duration = (Planned Hours / SUM(Percent allocation for each resource for the task)) / 8
```

Questo calcolo presuppone che il numero di ore in un normale giorno lavorativo sia 8. L&#39;equazione include questo valore in modo che la Durata pianificata venga visualizzata in giorni.

## Effetto dell’aggiunta di più risorse a un’attività

Quando si aggiungono o rimuovono assegnatari a un&#39;attività con il tipo di durata guidata sforzo, la durata e l&#39;orario pianificato non cambiano. Tuttavia, la Durata pianificata cambia.

Nell’esempio seguente, l’opzione Ore tipiche per giorno di lavoro è impostata su 8 nelle Preferenze progetto nella configurazione del sistema. Poiché la durata è di 3 giorni, l&#39;ora pianificata è impostata su 24 (3 giorni x 8 ore al giorno lavorativo = 24 ore pianificate).

>[!NOTE]
>
>Quando si utilizza il Vincolo di attività Date fisse, la Durata pianificata rimane invariata quando si aggiungono o rimuovono assegnatari, mentre la Durata e le Ore pianificate vengono modificate. Quando si utilizza un vincolo di attività diverso da Date fisse, la Durata pianificata viene modificata.

Nella tabella seguente viene illustrato il modo in cui viene modificata la Durata pianificata con l’aggiunta di risorse all’attività:

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
   <th> <p><strong>Lavoro Necessario</strong> </p> </th> 
   <th><strong>Durata Pianificata</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> </td> 
   <td> <p>1</p> </td> 
   <td> <p>3 giorni</p> </td> 
   <td> <p>24 Hours</p> <p>(3 giorni x 8 ore per giorno lavorativo = 24 ore previste)</p> </td> 
   <td> <p>3 giorni</p> <p>(24 ore previste / 1 assegnatario = 3 giorni)</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> <p>2</p> </td> 
   <td> <p>3 giorni</p> </td> 
   <td> <p>24 Hours</p> <p>(3 giorni x 8 ore per giorno lavorativo = 24 ore previste)</p> </td> 
   <td> <p>1,5 giorni</p> <p>(24 ore previste / 2 assegnatari = 12 ore, o 1,5 giorni)</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> <p>3</p> </td> 
   <td> <p>3 giorni</p> </td> 
   <td> <p>24 Hours</p> <p>(3 giorni x 8 ore per giorno lavorativo = 24 ore previste)</p> </td> 
   <td> <p>1 giorno</p> <p>(24 ore previste / 3 assegnatari = 8 ore, o 1 giorno)</p> </td> 
  </tr> 
 </tbody> 
</table>

## Cambia il tipo di durata di un&#39;attività in guidata da sforzo

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
