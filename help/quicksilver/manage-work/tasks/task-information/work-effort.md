---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Panoramica sullo sforzo di lavoro
description: Panoramica sullo sforzo di lavoro
author: Alina
feature: Work Management
exl-id: 70f51e4b-43cc-427a-99e4-ebb056bb1070
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1512'
ht-degree: 0%

---

# Panoramica sullo sforzo di lavoro

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the UI >> in the Project/ Template edit box > Tasks area> Learn more) </p>
-->

In qualità di project manager, puoi decidere come stimare la quantità di lavoro necessaria per completare le attività in un progetto. Stimare la quantità di lavoro necessaria per completare i compiti utilizzando uno dei seguenti indicatori:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Lavoro Necessario</td> 
   <td> <p> Voce numerica manuale o calcolo Adobe Workfront che visualizza il numero di ore necessarie per il completamento delle risorse assegnate a un'attività. </p> <p>Considera quanto segue sulle ore pianificate: </p> 
    <ul> 
     <li>Questo è il metodo predefinito. </li> 
     <li>È possibile aggiornare manualmente le ore pianificate solo per le attività con un tipo di durata di assegnazione calcolata o semplice. </li> 
    </ul> <p>Per informazioni sull'orario pianificato, vedi <a href="../../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref">Panoramica sull’orario pianificato</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Impegno di lavoro </td> 
   <td> <p>Etichetta manuale che definisce se un utente deve compiere un piccolo, medio o grande sforzo giornaliero per completare un'attività. <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       The level of effort is estimated to be a percentage of the daily amount of working time. (NOTE: keep this drafted. Vazgen said it's not needed, but waiting for feedback from users)
      </MadCap:conditionalText>
     --> </p> <p>Considera quanto segue sullo sforzo di lavoro:</p> 
    <ul> 
     <li>Questo campo è disponibile solo per le attività con un tipo di durata semplice. </li> 
     <li>Puoi abilitare l’utilizzo di questa etichetta e definire la percentuale di tempo di lavoro associato a essa a livello di progetto. </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Questo articolo descrive cosa è lo sforzo di lavoro e come è necessario utilizzarlo per stimare la quantità di lavoro per le attività.

>[!NOTE]
>
>Ore pianificate e sforzo di lavoro influenzano l&#39;un l&#39;altro. L’aggiornamento dell’orario pianificato può aggiornare lo sforzo di lavoro e l’aggiornamento dello sforzo di lavoro può aggiornare l’orario pianificato dell’attività.

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
   <td> <p>Modifica accesso a progetti e attività</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un progetto e le relative attività</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Considerazioni sull’utilizzo dello sforzo di lavoro

* Quando le attività del progetto hanno 0 ore pianificate e si attiva l&#39;opzione Usa impegno lavoro per calcolare automaticamente le impostazioni Orari pianificati attività del progetto, il livello predefinito di sforzo lavoro associato al progetto sarà Medio. L&#39;aggiornamento automatico delle ore pianificate per le attività di tipo Durata semplice. Per ulteriori informazioni, consulta la sezione .  [Livelli dello sforzo di lavoro](#levels-of-work-effort) in questo articolo.
* Quando le attività del progetto dispongono di ore pianificate superiori a 0 e si consente all&#39;utente di utilizzare lo sforzo di lavoro per calcolare automaticamente l&#39;impostazione Ore pianificate delle attività nel progetto, il livello di sforzo di lavoro viene aggiornato in base alla quantità di ore pianificate senza modificare la quantità di ore pianificate per le attività di tipo Durata semplice. Per ulteriori informazioni, consulta la sezione . [Come Workfront calcola lo sforzo di lavoro in base alle ore pianificate](#how-workfront-calculates-work-effort-based-on-planned-hours) in questo articolo.
* Quando le attività del progetto hanno 0 ore pianificate e si abilita l&#39;opzione Usa impegno lavoro per calcolare automaticamente le impostazioni Orario pianificato attività sul progetto, quindi aggiornare il livello di Sforzo lavoro da Medio a Piccolo o Grande, viene aggiornato anche l&#39;orario pianificato. Per ulteriori informazioni, consulta la sezione . [Modalità di calcolo delle ore pianificate in base allo sforzo sul lavoro da parte di Workfront](#how-workfront-calculates-planned-hours-based-on-work-effort) in questo articolo.
* Quando si allineano le attività di modifica e si modificano contemporaneamente sia il campo Ore pianificate che il campo Sforzo lavoro per l&#39;attività, le ore pianificate verranno aggiornate con il valore specificato, mentre il valore Sforzo lavoro viene calcolato in base alle ore pianificate aggiornate.
* Quando si aggiorna il valore dello sforzo di lavoro di un&#39;attività, la durata non viene più calcolata automaticamente in base alle ore pianificate. Per ulteriori informazioni sul calcolo della durata per le attività di Durata semplice, vedere [Panoramica sul tipo di durata: Semplice](../../../manage-work/tasks/taskdurtn/simple-duration-type.md).
* Quando si modifica il tipo di durata di un&#39;attività da Semplice a qualsiasi altro tipo, il campo di impegno del lavoro è nascosto sull&#39;attività. Le ore previste rimangono invariate.
* Non è possibile aggiornare il livello di sforzo di lavoro su un&#39;attività padre. Il livello di sforzo di lavoro per un&#39;attività padre viene calcolato automaticamente in base al numero di ore pianificate per le attività, che è un rollup di tutte le attività figlio. Per informazioni sulle attività principali, vedere [Creare sottoattività](../../../manage-work/tasks/create-tasks/create-subtasks.md).

## Abilita l’utilizzo di Work Sfort invece che di Planned Hours

1. Passa a un progetto e fai clic sul pulsante **Altro** menu ![](assets/more-icon.png), quindi fai clic su **Modifica**.
1. Fai clic su **Impostazioni attività**, quindi seleziona l’opzione **Utilizzare l&#39;impegno di lavoro per calcolare automaticamente le ore pianificate dell&#39;attività**. Questa opzione è deselezionata per impostazione predefinita.

   ![](assets/nwe-work-effort-on-projects-350x182.png)

   Per ulteriori informazioni sull&#39;abilitazione dell&#39;utilizzo dello sforzo di lavoro su un progetto, consulta la sezione &quot;Impostazioni attività&quot; in [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md) articolo.

1. Fai clic su **Attività** nel pannello a sinistra , fai clic sul nome di un’attività per accedervi.
1. Fai clic sul pulsante **Altro** menu ![](assets/more-icon.png), quindi fai clic su **Modifica**. Assicurarsi che l&#39;attività abbia un tipo di durata semplice.

   >[!TIP]
   >
   >È possibile aggiornare lo sforzo di lavoro per un&#39;attività anche nella sezione Dettagli attività .

1. In **Panoramica** fare clic sul menu a discesa Attività per correggere la quantità di lavoro necessaria per completare l&#39;attività.

   ![](assets/work-effort-on-edit-task-page-350x239.png)

   Per ulteriori informazioni sull&#39;aggiornamento del campo Attività di un&#39;attività, vedere i seguenti articoli:

   * La sezione &quot;Panoramica&quot; nella sezione [Modifica delle attività](../../../manage-work/tasks/manage-tasks/edit-tasks.md) articolo
   * [Gestire le informazioni sulle attività nell&#39;area Panoramica dettagli attività](../../../manage-work/tasks/manage-tasks/task-information-in-overview.md)

## Livelli dello sforzo di lavoro {#levels-of-work-effort}

In qualità di project manager, puoi identificare tre livelli di impegno di lavoro per i tuoi progetti. Ogni livello di impegno corrisponde a una percentuale del tempo giornaliero necessario agli utenti per completare l’attività.

Quando si imposta il livello di sforzo di lavoro è necessario porsi la domanda: &quot;Quanto tempo deve trascorrere ogni giorno un utente assegnato a questa attività per farla svolgere in tempo?&quot; 

La tabella seguente illustra i possibili livelli di impegno di lavoro e le relative percentuali predefinite. In qualità di project manager, puoi aggiornare le percentuali in base alle esigenze della tua organizzazione. Questa operazione viene eseguita durante la modifica di un progetto. Per informazioni sulla modifica dei progetti, consulta [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md).

In qualità di amministratore di Workfront, puoi definire gli orari tipici per giorno lavorativo nell’area Preferenze progetto di Configurazione. Si tratta della quantità giornaliera di tempo considerata come orario di lavoro. Per informazioni sulla configurazione delle preferenze di progetto per l&#39;istanza di Workfront, vedi [Configurare le preferenze del progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

>[!NOTE]
>
>Negli esempi seguenti, si presuppone che l’amministratore di Workfront abbia impostato l’importo di 8 ore per giorno lavorativo tipico.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Livello dello sforzo di lavoro</td> 
   <td>Valori percentuali</td> 
  </tr> 
  <tr> 
   <td>Piccolo </td> 
   <td>Un piccolo livello di impegno per il completamento di un'attività è impostato sul 25% delle ore tipiche per giorno lavorativo. Ciò significa che un compito assegnato a questo livello di sforzo di lavoro dovrebbe richiedere fino a 2 ore al giorno per essere completato in un giorno. <code>(0.25*8=2)</code></td> 
  </tr> 
  <tr> 
   <td>Medio</td> 
   <td> <p>Un livello medio di impegno per il completamento di un'attività è impostato sul 50% delle ore tipiche per giorno lavorativo. Ciò significa che un compito assegnato a questo livello di sforzo di lavoro dovrebbe richiedere più di 2 e meno di 6 ore per essere completato in un giorno. <code>(0.50*80=4)</code> </p> <p>Nota: Quando l'impostazione Usa impegno lavoro per calcolare automaticamente l'ora pianificata dell'attività è abilitata nel progetto, questa è l'impostazione predefinita per un'attività, se l'attività aveva 0 ore pianificate prima dell'attivazione di questa impostazione. In questo modo l'attività Orari pianificati viene aggiornata a 4 ore. </p> </td> 
  </tr> 
  <tr> 
   <td>Grande</td> 
   <td>Un grande impegno per il completamento di un'attività è impostato al 75% delle ore tipiche per giorno lavorativo. Ciò significa che un compito assegnato a questo livello di sforzo di lavoro dovrebbe richiedere 6 ore o più per essere completato in un giorno. <code>(0.75*8=6)</code></td> 
  </tr> 
 </tbody> 
</table>

## Modalità di calcolo delle ore pianificate in base allo sforzo sul lavoro da parte di Workfront {#how-workfront-calculates-planned-hours-based-on-work-effort}

Quando si abilita l&#39;impostazione Usa impegno lavoro per calcolare automaticamente le ore pianificate delle attività di un progetto, Workfront calcola il numero di ore pianificate per un&#39;attività con un tipo di durata semplice utilizzando la seguente formula:

```
Task Planned Hours = Number of days in task Duration * Work Effort percentage * Typical hours per work day
```

Ad esempio, un’attività con una durata di 3 giorni e uno sforzo di lavoro di medio ha 12 ore pianificate:

```
Planned Hours = 3*4=12
```

dove il valore di ore tipiche per giorno lavorativo è di 8 ore.

>[!TIP]
>
>Quando un&#39;attività viene assegnata a più risorse, le ore pianificate vengono distribuite in modo uniforme a ciascuna risorsa per ogni giorno della sua durata.

## Come Workfront calcola lo sforzo di lavoro in base alle ore pianificate {#how-workfront-calculates-work-effort-based-on-planned-hours}

Quando si abilita l&#39;opzione Usa impegno lavoro per calcolare automaticamente l&#39;impostazione Orario pianificato dell&#39;attività su un progetto e si dispone già di Ore pianificate sull&#39;attività oppure si modifica il numero di Ore pianificate sull&#39;attività, Workfront aggiorna il valore dello sforzo di lavoro.

Workfront utilizza la seguente formula per aggiornare il livello di impegno di lavoro in base all’orario pianificato:

```
Work Effort level = Task Planned Hours / Duration / Typical hours per work day
```

Ad esempio, se si dispone di un&#39;attività con una durata di 2 giorni e si aggiorna l&#39;orario pianificato da 8 a 20 ore, lo sforzo di lavoro per l&#39;attività viene aggiornato da medio a grande:

```
Work Effort level = 20 / 2 / 8 = 125 % = Large
```

## Individuare lo sforzo di lavoro per attività e progetti

* [Sforzo di lavoro per i progetti](#work-effort-for-projects)
* [Sforzo di lavoro per le attività](#work-effort-for-tasks)

### Sforzo di lavoro per i progetti {#work-effort-for-projects}

È possibile individuare la sezione relativa allo sforzo di lavoro in un progetto nell’area seguente:

* Area Impostazioni attività nella casella Modifica progetto

### Sforzo di lavoro per le attività {#work-effort-for-tasks}

È possibile individuare il campo di impegno del lavoro per un&#39;attività nelle aree seguenti:

* Area Panoramica nella casella Modifica attività
* Area Panoramica della sezione Dettagli attività, nell’area Orario di lavoro
* Un elenco di attività o un rapporto
