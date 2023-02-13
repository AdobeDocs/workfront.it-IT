---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: Panoramica del tipo di durata e durata dell’attività
description: La durata dell'attività è la differenza tra la data di completamento pianificata e la data di inizio pianificata dell'attività. La durata indica l'intervallo di tempo disponibile per il completamento dell'attività.
author: Alina
feature: Work Management
exl-id: c81e485a-7e8c-4907-8e6c-9991681c3541
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1383'
ht-degree: 2%

---

# Panoramica del tipo di durata e durata dell’attività

La durata dell&#39;attività è la differenza tra la data di completamento pianificata e la data di inizio pianificata dell&#39;attività. La durata indica l&#39;intervallo di tempo disponibile per il completamento dell&#39;attività.

Il tipo di durata di un&#39;attività identifica la relazione tra il numero di risorse assegnate a un&#39;attività, lo sforzo totale e la durata totale dell&#39;attività.

## Panoramica sulla durata dell’attività

>[!NOTE]
>
>Quando si tiene conto del tempo di inattività dell&#39;assegnatario primario su un progetto, è possibile che le date pianificate dell&#39;attività vengano modificate, ma la durata dell&#39;attività rimane invariata. Per informazioni su come tenere conto del tempo trascorso dall&#39;assegnatario principale durante la pianificazione di un progetto, consulta  [Configurare le preferenze del progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Se le date di inizio effettivo e di completamento effettivo dell&#39;attività non rientrano nella programmazione del progetto, dell&#39;assegnatario principale o della programmazione predefinita, la durata dell&#39;attività è pari a zero.

**Esempio:** Se si dispone di un programma che inizia alle 09:00 e termina alle 22:00 e un&#39;attività è prevista per l&#39;inizio alle 2:00 e termina alle 04:00, la durata dell&#39;attività è pari a zero.

Di seguito sono riportati due scenari esistenti per il calcolo della durata in Adobe Workfront.

* Se l&#39;attività viene assegnata a un utente Workfront utilizza una delle seguenti pianificazioni, in questo preciso ordine di calcolo della Durata:

   1. Workfront tiene conto della pianificazione dell’utente.
   1. Se l’utente non è associato a una pianificazione, Workfront prende in considerazione la pianificazione del progetto.
   1. Se il progetto non è associato a una pianificazione, Workfront prende in considerazione la pianificazione predefinita del sistema. Per informazioni sulle pianificazioni, consulta [Creare una pianificazione](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* Se l’attività viene assegnata a più utenti:

   Workfront prende in considerazione la pianificazione del progetto o quella dell’assegnatario principale.

   L’amministratore di Workfront determina la pianificazione utilizzata da Workfront quando un’attività viene assegnata a più utenti. Per informazioni, consulta [Configurare le preferenze del progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   I passaggi sono simili al primo scenario dopo aver compreso quale pianificazione Workfront utilizza per calcolare la durata.

## Unità di tempo per la durata dell&#39;attività

È possibile indicare la durata dell&#39;attività sia nel tempo regolare che nel tempo trascorso tra le date di inizio pianificato e di completamento pianificato.

Quando si aggiorna la Durata delle attività in un elenco, è possibile utilizzare le abbreviazioni seguenti per indicare le unità di tempo in Workfront:

| Unità di tempo | Abbreviazione |
|---|---|
| Minuti | M |
| Ore | H |
| Giorni. Questa è l’impostazione predefinita. | Dsbld |
| Settimane | M |
| Mesi | G |
| Minuti trascorsi | EM |
| Ore trascorse | EH |
| Giorni trascorsi | ED |
| Settimane trascorse | EW |
| Mesi trascorsi | ET |

{style=&quot;table-layout:auto&quot;}

**Esempio:** Se si desidera indicare che la durata di un&#39;attività è di 3 giorni trascorsi, digitare &quot;3 ED&quot; nel campo Durata in un elenco di attività.  È inoltre possibile selezionare l&#39;opzione preferita per Unità di tempo di durata dal menu a discesa disponibile quando si modifica un&#39;attività o nella sezione Dettagli attività. Per informazioni sulle attività di modifica, consulta [Modifica delle attività](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: stays QS only forever; for the pictures below: make the first one classic at preview time and the second one stays QS always. The second one is yellow >> take out at 21.2 production!!)</p>
-->

![](assets/duration-elapsed-days-tasks-nwe-350x282.png)

Quando si indica la Durata di un&#39;attività, tenere presente quanto segue:

* Il tempo trascorso è un&#39;unità di tempo per la durata di un&#39;attività. È l&#39;intervallo tra la data di inizio pianificata e la data di completamento pianificata di un&#39;attività che include le festività, i fine settimana e l&#39;ora di inattività. In altre parole, il tempo trascorso è il passaggio dei giorni di calendario.
* L&#39;ora regolare prende in considerazione le festività, i fine settimana e l&#39;ora di riposo e li esclude dalla Durata dell&#39;attività.

* Quando si indica la Durata di un&#39;attività in settimane, Workfront calcola la Durata in giorni e ore in base alle impostazioni di giorni lavorativi tipici della settimana e orari tipici per giorno lavorativo impostate dall&#39;amministratore Workfront nell&#39;area Preferenze progetto di Configurazione.
* Workfront utilizza la durata predefinita di 4 settimane per un mese quando si calcola la Durata in mesi.

## Panoramica sul tipo di durata dell&#39;attività

La gestione del tipo di durata di un&#39;attività consente di impostare assegnazioni di risorse coerenti in base alle esigenze dell&#39;attività.

Il tipo di durata consente di rispondere alle seguenti domande:

* Quanto saremo occupati?
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
   <th scope="col"> <p><strong>Influenza delle risorse</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <th scope="col"> <p><strong>Incarico Calcolato</strong> </p> </th> 
   <td scope="col"> <p>Calcola la percentuale di allocazione per ogni assegnatario di un'attività. </p> <p>Quando si sceglie questo tipo di durata, è possibile inserire la durata individuale e l'ora pianificata per l'attività. Workfront divide le ore pianificate in base al numero di ore all’interno della durata dell’attività, quindi in base al numero di risorse assegnate all’attività per calcolare l’allocazione per ogni assegnatario.</p> <p>Per informazioni più dettagliate, consulta <a href="../../../manage-work/tasks/taskdurtn/calculated-assignment.md" class="MCXref xref">Panoramica sul tipo di durata: Assegnazione calcolata</a>.</p> </td> 
   <td scope="col">La durata e le ore pianificate non vengono modificate quando si aggiungono o rimuovono assegnatari all'attività. </td> 
  </tr> 
  <tr> 
   <th scope="col"> <p><strong>Lavoro Calcolato</strong> </p> </th> 
   <td scope="col"> <p>Determina le ore pianificate (sforzo) necessarie per completare l'attività.</p> <p>Utilizzato normalmente quando le risorse assegnate all'attività vengono allocate per l'intera durata dell'attività.</p> <p>Quando si sceglie questo tipo di durata, è possibile inserire una singola durata per l'attività. Workfront calcola gli orari pianificati per l'attività moltiplicando il numero di giorni nella durata per il numero di ore lavorative nella pianificazione e per il numero di assegnatari nell'attività. </p> <p>È possibile modificare manualmente la percentuale di allocazione di ciascun assegnatario nell'attività, riducendo così la quantità di ore pianificate.</p> <p>Per informazioni più dettagliate, consulta <a href="../../../manage-work/tasks/taskdurtn/calculated-work.md" class="MCXref xref">Panoramica sul tipo di durata: Lavoro calcolato</a>.</p> </td> 
   <td scope="col"> <p>Le ore pianificate aumentano quando gli assegnatari vengono aggiunti all'attività. </p> <p>Le ore pianificate diminuiscono quando gli assegnatari vengono rimossi dall'attività.</p> </td> 
  </tr> 
  <tr> 
   <th scope="col"> <p>Impegno Aggiuntivo</p> </th> 
   <td scope="col"> <p>Determina le ore pianificate in base al numero di risorse.</p> <p>Quando si sceglie questo tipo di durata, è possibile inserire una singola durata per l'attività. Workfront calcola gli orari pianificati per l'attività moltiplicando il numero di giorni nella durata per il numero di ore lavorative nella pianificazione e dividendo tale numero per il numero di assegnatari nell'attività. </p> <p>È possibile modificare manualmente la percentuale di allocazione di ciascun assegnatario all'attività, ma il numero di ore pianificate rimane lo stesso.</p> <p>Per informazioni più dettagliate, consulta <a href="../../../manage-work/tasks/taskdurtn/effort-driven.md" class="MCXref xref">Panoramica sul tipo di durata: Guida allo sforzo</a>.</p> </td> 
   <td scope="col"> <p>Le ore pianificate aumentano quando gli assegnatari vengono rimossi dall'attività.</p> <p>Le ore pianificate diminuiscono quando gli assegnatari vengono aggiunti all'attività. </p> <p>La durata non cambia, indipendentemente dalle modifiche nel numero di assegnatari o dalla loro pianificazione. </p> <p>La durata è uguale a Ora pianificata. La durata prevista è uguale a Ore pianificate divise per il numero di assegnatari.</p> </td> 
  </tr> 
  <tr> 
   <th scope="col"> <p><strong>Semplice</strong> </p> </th> 
   <td scope="col"> <p>Determina le ore pianificate e la durata (uguali, per questo tipo di durata) in base al numero di ore per le quali ogni assegnatario è allocato. </p> <p>Workfront calcola le ore pianificate sommando le ore allocate pianificate per ogni assegnatario. </p> <p>È possibile modificare manualmente la quantità di ore per le quali ogni assegnatario è assegnato e il numero di ore pianificate e la quantità di Durata cambia di conseguenza. Se si sceglie un numero totale di ore assegnate per tutti gli assegnatari, tale numero viene suddiviso equamente tra ciascun assegnatario.</p> <p>Per informazioni più dettagliate, consulta <a href="../../../manage-work/tasks/taskdurtn/simple-duration-type.md" class="MCXref xref">Panoramica sul tipo di durata: Semplice</a>.</p> </td> 
   <td scope="col"> <p>Le ore sono distribuite in modo uniforme tra gli assegnatari se si sceglie un numero totale di ore assegnate. Tuttavia, in qualità di project manager, puoi regolare manualmente le ore di ogni assegnatario. </p> <p>È possibile modificare le ore pianificate e la durata di un'attività con un tipo di durata semplice in linea o a livello di attività. </p> <p>Se un team agile viene assegnato a un'attività, il Tipo di durata viene impostato automaticamente su Semplice e non può essere modificato. La durata dell'attività per un team agile deve essere maggiore di 0 minuti.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Tipo di durata delle nuove attività

Il tipo di durata di una nuova attività corrisponde al tipo di durata impostato nel sistema. Il tipo di durata predefinito è Calculated Assignment. L’amministratore di Workfront o un amministratore di gruppo può aggiornare il tipo di durata predefinito per il sistema o per il gruppo associato al progetto. Per informazioni, consulta [Configurare le preferenze relative alle attività e ai problemi a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## Modificare il tipo di durata di un&#39;attività

Per informazioni sulla modifica del tipo di durata di un&#39;attività, vedere [Aggiornare il tipo di durata di un&#39;attività](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).
