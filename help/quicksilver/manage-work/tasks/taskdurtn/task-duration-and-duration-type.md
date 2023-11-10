---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: Panoramica sulla durata e sul tipo di durata dell'attività
description: La Durata attività è la differenza tra la Data di completamento pianificata e la Data di inizio pianificata dell'attività. La Durata indica l'intervallo di tempo disponibile per il completamento dell'attività.
author: Alina
feature: Work Management
recommendations: noDisplay, noCatalog
exl-id: c81e485a-7e8c-4907-8e6c-9991681c3541
source-git-commit: 48f46abab1958325aba6832b85247dc2c80f4e80
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Panoramica sulla durata e sul tipo di durata dell&#39;attività

La Durata attività è la differenza tra la Data di completamento pianificata e la Data di inizio pianificata dell&#39;attività. La Durata indica l&#39;intervallo di tempo disponibile per il completamento dell&#39;attività.

Il tipo di durata di un&#39;attività identifica la relazione tra il numero di risorse assegnate a un&#39;attività, l&#39;impegno totale e la durata totale dell&#39;attività.

## Panoramica sulla durata dell’attività

>[!NOTE]
>
>Se si tiene conto del tempo libero dell&#39;assegnatario principale in un progetto, le date pianificate dell&#39;attività potrebbero essere modificate, ma la durata dell&#39;attività rimane invariata. Per informazioni su come considerare il tempo libero dell’assegnatario principale durante la pianificazione di un progetto, consulta  [Configurare le preferenze di progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Se le date di inizio e di completamento effettive dell&#39;attività non rientrano nella programmazione del progetto, dell&#39;assegnatario principale o della programmazione predefinita, la durata dell&#39;attività è pari a zero.

**Esempio:** Se una pianificazione inizia alle 9 e termina alle 12 e un&#39;attività è pianificata per iniziare alle 14 e terminare alle 16, la durata dell&#39;attività sarà zero.

Di seguito sono riportati due scenari che esistono durante il calcolo della durata in Adobe Workfront.

* Se l&#39;attività è assegnata a un utente, Workfront utilizza una delle seguenti pianificazioni, nell&#39;ordine esatto per calcolare la Durata:

   1. Workfront tiene conto della pianificazione dell’utente.
   1. Se l’utente non è associato a una pianificazione, Workfront tiene conto della pianificazione del progetto.
   1. Se il progetto non è associato a una pianificazione, Workfront prende in considerazione la pianificazione predefinita del sistema. Per informazioni sulle pianificazioni, consulta [Creare una pianificazione](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* Se l&#39;attività è assegnata a più utenti:

  Workfront prende in considerazione la pianificazione del progetto o quella dell’assegnatario principale.

  L&#39;amministratore di Workfront determina la pianificazione utilizzata da Workfront quando un&#39;attività viene assegnata a più utenti. Per informazioni, consulta [Configurare le preferenze di progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

  I passaggi sono simili al primo scenario dopo aver compreso quale pianificazione utilizza Workfront per calcolare la durata.

## Unità di tempo per la durata dell&#39;attività

È possibile indicare la durata dell&#39;attività sia nell&#39;ora normale che nel tempo trascorso tra le date di inizio pianificata e di completamento pianificata.

Quando si aggiorna la Durata delle attività in un elenco, è possibile utilizzare le seguenti abbreviazioni per indicare le unità di tempo in Workfront:

| Unità di tempo | Abbreviazione |
|---|---|
| Minuti | M |
| Ore | H |
| Giorni. Questa è l&#39;impostazione predefinita. | Dsbld |
| Settimane | M |
| Mesi | G |
| Minuti trascorsi | EM |
| Ore trascorse | EH |
| Giorni trascorsi | ED |
| Settimane trascorse | EW |
| Mesi trascorsi | ET |

{style="table-layout:auto"}

**Esempio:** Se si desidera indicare che la durata di un&#39;attività è di 3 giorni trascorsi, digitare &quot;3 ED&quot; nel campo Durata in un elenco di attività.  È inoltre possibile selezionare l&#39;opzione desiderata per l&#39;unità di tempo di durata dal menu a discesa disponibile quando si modifica un&#39;attività o nella sezione Dettagli attività. Per informazioni sulla modifica delle attività, vedere [Modifica attività](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: stays QS only forever; for the pictures below: make the first one classic at preview time and the second one stays QS always. The second one is yellow >> take out at 21.2 production!!)</p>
-->

![](assets/duration-elapsed-days-tasks-nwe-350x282.png)

Quando si indica la durata di un&#39;attività, tenere presente quanto segue:

* Il tempo trascorso è un&#39;unità di tempo per la durata di un&#39;attività. Si tratta del tempo che intercorre tra la Data inizio pianificata e la Data completamento pianificata di un&#39;attività e che include ferie, fine settimana e ferie. In altre parole, il tempo trascorso è il trascorrere dei giorni di calendario.
* L&#39;orario regolare prende in considerazione le festività, i fine settimana e le ferie e le esclude dalla Durata dell&#39;attività.

* Quando si indica la Durata di un&#39;attività in settimane, Workfront calcola la Durata in giorni e ore in base alle impostazioni Giornate lavorative tipiche e Ore tipiche per giorno lavorativo impostate dall&#39;amministratore di Workfront nell&#39;area Preferenze progetto di configurazione.
* Per calcolare la durata in mesi, Workfront utilizza la durata predefinita di 4 settimane per un mese.

## Panoramica sul tipo di durata dell’attività

La gestione del tipo di durata di un&#39;attività consente di impostare assegnazioni di risorse coerenti in base alle esigenze dell&#39;attività.

Il Tipo di Durata consente di rispondere alle seguenti domande:

* Quanto saremo impegnati?
* Quanto è grande il lavoro?
* Quanto ci vorrà?

![duration_type_triangle.png](assets/duration-type-triangle-350x245.png)

## Definire i tipi di durata

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th scope="row">Tipo di Durata </th> 
   <th scope="col"> <p><strong>Funzione</strong> </p> </th> 
   <th scope="col"> <p><strong>Effetti delle risorse</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <th scope="col"> <p><strong>Incarico Calcolato</strong> </p> </th> 
   <td scope="col"> <p>Calcola la percentuale di allocazione per ogni assegnatario di un'attività. </p> <p>Quando si sceglie questo Tipo di durata, è possibile immettere la durata e le ore pianificate per l'attività. Workfront divide le ore pianificate per il numero di ore all'interno della Durata dell'attività e quindi per il numero di risorse assegnate all'attività per calcolare l'allocazione per ciascun assegnatario.</p> <p>Per informazioni più dettagliate, consulta <a href="../../../manage-work/tasks/taskdurtn/calculated-assignment.md" class="MCXref xref">Panoramica sul tipo di durata: assegnazione calcolata</a>.</p> </td> 
   <td scope="col">La durata e le ore pianificate non cambiano quando si aggiungono o si rimuovono assegnatari all'attività. </td> 
  </tr> 
  <tr> 
   <th scope="col"> <p><strong>Lavoro Calcolato</strong> </p> </th> 
   <td scope="col"> <p>Determina le ore pianificate (quantità di impegno) necessarie per il completamento dell'attività.</p> <p>Normalmente utilizzato quando le risorse assegnate all'attività vengono allocate per l'intera Durata dell'attività.</p> <p>Quando si sceglie questo Tipo di durata, è possibile immettere una singola Durata per l'attività. Workfront calcola le ore pianificate per l'attività moltiplicando il numero di giorni nella durata per il numero di ore lavorative nella pianificazione e per il numero di assegnatari dell'attività. </p> <p>È possibile modificare manualmente la percentuale di allocazione di ogni assegnatario all'attività, riducendo così la quantità di ore pianificate.</p> <p>Per informazioni più dettagliate, consulta <a href="../../../manage-work/tasks/taskdurtn/calculated-work.md" class="MCXref xref">Panoramica sul tipo di durata: lavoro calcolato</a>.</p> </td> 
   <td scope="col"> <p>Le ore pianificate aumentano quando gli assegnatari vengono aggiunti all'attività. </p> <p>Le ore pianificate diminuiscono quando gli assegnatari vengono rimossi dall'attività.</p> </td> 
  </tr> 
  <tr> 
   <th scope="col"> <p>Impegno Aggiuntivo</p> </th> 
   <td scope="col"> <p>Determina le ore pianificate in base al numero di risorse.</p> <p>Quando si sceglie questo Tipo di durata, è possibile immettere una singola Durata per l'attività. Workfront calcola le ore pianificate per l'attività moltiplicando il numero di giorni nella durata per il numero di ore lavorative nella programmazione e dividendo tale numero per il numero di assegnatari dell'attività. </p> <p>È possibile modificare manualmente la percentuale di allocazione di ogni assegnatario all'attività, ma il numero di ore pianificate rimane invariato.</p> <p>Per informazioni più dettagliate, consulta <a href="../../../manage-work/tasks/taskdurtn/effort-driven.md" class="MCXref xref">Panoramica sul tipo di durata: basata sulle risorse</a>.</p> </td> 
   <td scope="col"> <p>Le ore pianificate aumentano quando gli assegnatari vengono rimossi dall'attività.</p> <p>Le ore pianificate diminuiscono quando gli assegnatari vengono aggiunti all'attività. </p> <p>La Durata rimane invariata, indipendentemente dalle modifiche apportate al numero di assegnatari o alla loro pianificazione. </p> <p>La durata è uguale alle ore pianificate. La Durata Pianificata è uguale alle Ore Pianificate divisa per il numero di assegnatari.</p> </td> 
  </tr> 
  <tr> 
   <th scope="col"> <p><strong>Semplice</strong> </p> </th> 
   <td scope="col"> <p>Determina le ore pianificate e la durata (che sono uguali, per questo tipo di durata) in base al numero di ore per cui ogni assegnatario è allocato. </p> <p>Workfront calcola le ore pianificate sommando le ore allocate pianificate per ciascun assegnatario. </p> <p>Puoi modificare manualmente la quantità di ore per cui è allocato ciascun assegnatario, e il numero di ore pianificate e la quantità della Durata cambiano di conseguenza. Se si sceglie un numero totale di ore allocate per tutti gli assegnatari, tale numero viene diviso equamente tra ciascun assegnatario.</p> <p>Per informazioni più dettagliate, consulta <a href="../../../manage-work/tasks/taskdurtn/simple-duration-type.md" class="MCXref xref">Panoramica sul tipo di durata: semplice</a>.</p> </td> 
   <td scope="col"> <p>Le ore vengono distribuite in modo uniforme tra gli assegnatari se si sceglie un numero totale di ore allocate. Tuttavia, in qualità di project manager, puoi regolare manualmente le ore per ogni assegnatario. </p> <p>È possibile modificare le ore pianificate e la durata di un'attività con un tipo di durata semplice in linea o a livello di attività. </p> <p>Se a un’attività viene assegnato un team agile, il Tipo di durata viene impostato automaticamente su Semplice e non può essere modificato. La durata dell'attività per un team Agile deve essere maggiore di 0 minuti.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Tipo di durata delle nuove attività

Il Tipo di Durata di una nuova attività corrisponde al Tipo di Durata impostato nel sistema. Il tipo di durata predefinito è Assegnazione calcolata. L’amministratore di Workfront o un amministratore gruppo può aggiornare il Tipo di durata predefinito per il sistema o per il gruppo associato al progetto. Per informazioni, consulta [Configurare le preferenze per attività e problemi a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## Modificare il tipo di durata di un&#39;attività

Per informazioni sulla modifica del tipo di durata di un&#39;attività, vedere [Aggiornare il tipo di durata di un&#39;attività](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).
