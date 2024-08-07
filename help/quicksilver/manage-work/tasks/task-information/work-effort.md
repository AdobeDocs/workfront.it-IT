---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Panoramica sull’impegno di lavoro
description: Panoramica sull’impegno di lavoro
author: Alina
feature: Work Management
exl-id: 70f51e4b-43cc-427a-99e4-ebb056bb1070
source-git-commit: 84c5772d130be78d9f9b9aef342c57183d5ec985
workflow-type: tm+mt
source-wordcount: '1505'
ht-degree: 0%

---

# Panoramica sull’impegno di lavoro

<!--Audited: 01/2024-->

<!--
(NOTE: Linked to the UI >> in the Project/ Template edit box > Tasks area> Learn more)
-->

In qualità di project manager, è possibile decidere come stimare la quantità di lavoro necessaria per il completamento delle attività in un progetto. Stimare la quantità di lavoro necessaria per completare le attività utilizzando uno dei seguenti indicatori:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Lavoro Necessario</td> 
   <td> <p> Inserimento numerico manuale o calcolo Adobe Workfront che visualizza il numero di ore necessarie per il completamento delle risorse assegnate a un'attività. </p> <p>Considera le seguenti informazioni sulle ore pianificate: </p> 
    <ul> 
     <li>Questo è il metodo predefinito. </li> 
     <li>È possibile aggiornare manualmente le ore pianificate solo per le attività con tipo di durata Assegnazione calcolata o Semplice. </li> 
    </ul> <p>Per informazioni sulle ore pianificate, vedi <a href="../../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref">Panoramica sulle ore pianificate</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Impegno di lavoro </td> 
   <td> <p>Etichetta manuale che definisce se è necessario uno sforzo giornaliero minimo, medio o elevato per completare un'attività. <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       The level of effort is estimated to be a percentage of the daily amount of working time. (NOTE: keep this drafted. Vazgen said it's not needed, but waiting for feedback from users)
      </MadCap:conditionalText>
     --> </p> <p>Considera quanto segue su Impegno di lavoro:</p> 
    <ul> 
     <li>Questo campo è disponibile solo per le attività con tipo di durata semplice. </li> 
     <li>Puoi abilitare l’uso di questa etichetta e definire la percentuale di orario di lavoro associata a livello di progetto. </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Questo articolo descrive l&#39;impegno di lavoro e il modo in cui utilizzarlo per stimare la quantità di lavoro per le attività.

>[!NOTE]
>
>Le ore pianificate e l&#39;impegno di lavoro si influenzano a vicenda. L&#39;aggiornamento delle ore pianificate può aggiornare l&#39;impegno di lavoro e l&#39;aggiornamento dell&#39;impegno di lavoro può aggiornare le ore pianificate dell&#39;attività.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Corrente: Piano </p>
   Oppure
   <p>Nuovo: Standard </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazione del livello di accesso</td> 
   <td> <p>Modificare l’accesso a Progetti e Attività</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un progetto e le relative attività</p>  </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront. Per ulteriori informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerazioni per l’utilizzo dell’impegno di lavoro

* Se le attività del progetto hanno 0 ore pianificate e si abilita l&#39;impostazione Usa impegno di lavoro per calcolare automaticamente le ore pianificate per l&#39;attività nel progetto, il livello predefinito di impegno di lavoro associato sarà Medium. Le ore pianificate vengono aggiornate automaticamente per le attività con tipo di durata semplice. Per ulteriori informazioni, vedere la sezione [Livelli di impegno di lavoro](#levels-of-work-effort) in questo articolo.
* Quando le attività del progetto hanno Ore pianificate superiori a 0 e si abilita l&#39;opzione Usa impegno di lavoro per calcolare automaticamente le ore pianificate per l&#39;attività nel progetto, il livello di impegno di lavoro viene aggiornato in base alla quantità di ore pianificate senza modificare la quantità di ore pianificate per le attività di tipo Durata semplice. Per ulteriori informazioni, vedere la sezione [Come Workfront calcola l&#39;impegno di lavoro in base alle ore pianificate](#how-workfront-calculates-work-effort-based-on-planned-hours) in questo articolo.
* Se le attività del progetto hanno 0 Ore pianificate e si abilita l&#39;opzione Usa impegno di lavoro per calcolare automaticamente le ore pianificate per l&#39;attività nel progetto, quindi si aggiorna il livello di impegno di lavoro da Medium a Piccolo o Grande, anche le ore pianificate vengono aggiornate. Per ulteriori informazioni, vedere la sezione [Come Workfront calcola le ore pianificate in base all&#39;impegno di lavoro](#how-workfront-calculates-planned-hours-based-on-work-effort) in questo articolo.
* Quando si modificano contemporaneamente le attività in linea e i campi Lavoro pianificato e Impegno di lavoro per l&#39;attività, le ore pianificate vengono aggiornate con il valore specificato, mentre il valore Impegno di lavoro viene calcolato in base alle ore pianificate aggiornate.
* Quando si aggiorna il valore Impegno di lavoro di un&#39;attività, la Durata non viene più calcolata automaticamente in base alle Ore pianificate. Per ulteriori informazioni sul calcolo della durata per le attività con durata semplice, vedere [Panoramica sul tipo di durata: semplice](../../../manage-work/tasks/taskdurtn/simple-duration-type.md).
* Quando si modifica il Tipo di durata di un&#39;attività da Semplice a qualsiasi altro tipo, il campo Impegno di lavoro è nascosto nell&#39;attività. Le ore pianificate rimangono invariate.
* Non è possibile aggiornare il livello Impegno di lavoro su un&#39;attività padre. Il livello Impegno di lavoro per un&#39;attività padre viene calcolato automaticamente in base al numero di ore pianificate per le attività, che è un rollup di tutte le attività figlio. Per informazioni sulle attività padre, vedere [Creare sottoattività](../../../manage-work/tasks/create-tasks/create-subtasks.md).

## Abilita l’utilizzo dell’Impegno di lavoro invece delle Ore pianificate

1. Vai a un progetto e fai clic sul menu **Altro** ![](assets/more-icon.png), quindi fai clic su **Modifica**.
1. Fai clic su **Impostazioni attività**, quindi seleziona l&#39;opzione **Utilizza Impegno di lavoro per calcolare automaticamente le ore pianificate per l&#39;attività**. Questa opzione è deselezionata per impostazione predefinita.

   ![](assets/nwe-work-effort-on-projects-350x182.png)

   Per ulteriori informazioni sull&#39;abilitazione dell&#39;utilizzo dell&#39;impegno di lavoro in un progetto, vedere la sezione &quot;Impostazioni attività&quot; nell&#39;articolo [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Fai clic su **Attività** nel pannello a sinistra, quindi fai clic sul nome di un&#39;attività per accedervi.
1. Fai clic sul menu **Altro** ![](assets/more-icon.png), quindi fai clic su **Modifica**. Assicurati che l’attività abbia un tipo di durata semplice.

   >[!TIP]
   >
   >È possibile aggiornare l&#39;Impegno di lavoro per un&#39;attività anche nella sezione Dettagli attività.

1. Nell&#39;area **Panoramica**, fare clic sul menu a discesa Impegno di lavoro per correggere l&#39;impegno necessario per completare l&#39;attività.

   ![](assets/work-effort-on-edit-task-page-350x239.png)

   Per ulteriori informazioni sull&#39;aggiornamento del campo Impegno di lavoro per un&#39;attività, vedere gli articoli seguenti:

   * La sezione &quot;Panoramica&quot; nell&#39;articolo [Modifica attività](../../../manage-work/tasks/manage-tasks/edit-tasks.md)
   * [Gestire le informazioni sull&#39;attività nell&#39;area Panoramica dettagli attività](../../../manage-work/tasks/manage-tasks/task-information-in-overview.md)

## Livelli di impegno di lavoro {#levels-of-work-effort}

In qualità di project manager, puoi identificare tre livelli di impegno di lavoro per i tuoi progetti. Ogni livello di impegno corrisponde a una percentuale del tempo giornaliero necessario agli utenti per completare l&#39;attività.

Quando si imposta il livello di Impegno di lavoro, è necessario porsi la domanda: &quot;Quanto tempo deve trascorrere quotidianamente un utente assegnato a questa attività per completarla in tempo?&quot;

La tabella seguente illustra i possibili livelli di Impegno di lavoro e le relative percentuali corrispondenti predefinite. In qualità di project manager, puoi aggiornare le percentuali in base alle esigenze della tua organizzazione. Puoi eseguire questa operazione mentre modifichi un progetto. Per informazioni sulla modifica dei progetti, vedere [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md).

In qualità di amministratore di Workfront, definisci le ore tipiche per giornata lavorativa nell’area Preferenze progetto di Configura. Si tratta della quantità giornaliera di tempo considerata come orario di lavoro. Per informazioni sulla configurazione delle preferenze di progetto per l&#39;istanza di Workfront, vedere [Configurare le preferenze di progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

>[!NOTE]
>
>Negli esempi seguenti, si presuppone che l’amministratore di Workfront abbia impostato l’importo Tipico di ore per giornata lavorativa su 8 ore.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Livello di impegno di lavoro</td> 
   <td>Valori percentuali</td> 
  </tr> 
  <tr> 
   <td>Piccola </td> 
   <td>Un piccolo livello di impegno per il completamento di un'attività è impostato al 25% delle ore tipiche per giorno lavorativo. Ciò significa che un'attività assegnata a questo livello di Impegno di lavoro dovrebbe richiedere fino a 2 ore al giorno per essere completata in un giorno. <code>(0.25*8=2)</code></td> 
  </tr> 
  <tr> 
   <td>Medio</td> 
   <td> <p>Un livello di impegno Medium per il completamento di un'attività è impostato sul 50% delle ore tipiche per giornata lavorativa. Ciò significa che il completamento di un'attività assegnata a questo livello di Impegno di lavoro dovrebbe richiedere più di 2 e meno di 6 ore in un giorno. <code>(0.50*80=4)</code> </p> <p>Nota: quando l'impostazione Usa impegno di lavoro per calcolare automaticamente le ore pianificate per l'attività è abilitata nel progetto, questa è l'impostazione predefinita per un'attività, se l'attività aveva 0 ore pianificate prima che questa impostazione fosse abilitata. In questo modo l'attività Lavoro Necessario viene aggiornata a 4 ore. </p> </td> 
  </tr> 
  <tr> 
   <td>Grande</td> 
   <td>Un grande sforzo per completare un'attività è impostato al 75% delle ore tipiche per giorno lavorativo. Ciò significa che un'attività assegnata a questo livello di Impegno di lavoro dovrebbe richiedere 6 ore o più per essere completata in un giorno. <code>(0.75*8=6)</code></td> 
  </tr> 
 </tbody> 
</table>

## Come Workfront calcola le ore pianificate in base all’impegno di lavoro {#how-workfront-calculates-planned-hours-based-on-work-effort}

Quando si abilita l&#39;impostazione Usa impegno di lavoro per calcolare automaticamente le ore pianificate per un&#39;attività in un progetto, Workfront calcola il numero di ore pianificate per un&#39;attività con un tipo di durata semplice utilizzando la formula seguente:

```
Task Planned Hours = Number of days in task Duration * Work Effort percentage * Typical hours per work day
```

Ad esempio, un&#39;attività con una durata di 3 giorni e un impegno di lavoro di Medium ha 12 ore pianificate:

```
Planned Hours = 3*4=12
```

dove il valore Tipico di ore per giorno lavorativo è 8 ore.

>[!TIP]
>
>Quando un&#39;attività viene assegnata a più risorse, le ore pianificate vengono distribuite in modo uniforme a ciascuna risorsa per ogni giorno della durata dell&#39;attività.

## Come Workfront calcola l’impegno di lavoro in base alle ore pianificate {#how-workfront-calculates-work-effort-based-on-planned-hours}

Se si abilita l&#39;opzione Usa impegno di lavoro per calcolare automaticamente le ore pianificate per un&#39;attività in un progetto e si dispone già di ore pianificate per l&#39;attività oppure si modifica il numero di ore pianificate per l&#39;attività, Workfront aggiorna il valore Impegno di lavoro.

Workfront utilizza la formula seguente per aggiornare il livello di Impegno di lavoro in base alle Ore pianificate:

```
Work Effort level = Task Planned Hours / Duration / Typical hours per work day
```

Ad esempio, se un&#39;attività ha una Durata di 2 giorni e si aggiornano le Ore pianificate da 8 a 20 ore, l&#39;Impegno di lavoro per l&#39;attività viene aggiornato da Medium a Grande:

```
Work Effort level = 20 / 2 / 8 = 125 % = Large
```

## Individua impegno di lavoro per attività e progetti

* [Impegno di lavoro per i progetti](#work-effort-for-projects)
* [Impegno di lavoro per le attività](#work-effort-for-tasks)

### Impegno di lavoro per i progetti {#work-effort-for-projects}

Puoi individuare la sezione Impegno di lavoro su un progetto nella seguente area:

* Nell&#39;area Impostazioni attività della casella Modifica progetto

### Impegno di lavoro per le attività {#work-effort-for-tasks}

È possibile individuare il campo Impegno di lavoro per un&#39;attività nelle seguenti aree:

* L&#39;area Panoramica nella casella Modifica attività
* L&#39;area Panoramica della sezione Dettagli attività, nell&#39;area Orario di lavoro
* Un elenco di attività o un report
