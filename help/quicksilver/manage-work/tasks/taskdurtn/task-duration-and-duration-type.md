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
source-git-commit: 6327e5625481ce7ff8d744bc6eb50d417cbb4413
workflow-type: tm+mt
source-wordcount: '1647'
ht-degree: 1%

---

# Panoramica sulla durata e sul tipo di durata dell&#39;attività

<!-- Audited: 12/2023 -->

<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo i rilasci mensili in Produzione, le stesse funzioni sono disponibili nell’ambiente di Produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedere [Abilitare o disabilitare le versioni rapide per l&#39;organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

La Durata attività è la differenza tra la Data di completamento pianificata e la Data di inizio pianificata dell&#39;attività. La Durata indica l&#39;intervallo di tempo disponibile per il completamento dell&#39;attività.

Il tipo di durata di un&#39;attività identifica la relazione tra il numero di risorse assegnate a un&#39;attività, l&#39;impegno totale e la durata totale dell&#39;attività.

## Panoramica sulla durata dell’attività

Se le date di inizio e di completamento effettive dell&#39;attività non rientrano nella programmazione del progetto, dell&#39;assegnatario principale o della programmazione predefinita, la durata dell&#39;attività è pari a zero.

>[!BEGINSHADEBOX]

**ESEMPIO**
Se una pianificazione inizia alle 9 e termina alle 12 e un&#39;attività è pianificata per iniziare alle 14 e terminare alle 16, la durata dell&#39;attività sarà zero.


>[!ENDSHADEBOX]

Di seguito sono riportati due scenari che esistono durante il calcolo della durata in Adobe Workfront:

* Se l’attività è assegnata a un utente, esistono i seguenti scenari in base all’ambiente utilizzato:

   * Nell’ambiente di produzione, Workfront utilizza una delle seguenti pianificazioni, nell’ordine esatto per calcolare la Durata:

   1. Workfront tiene conto della pianificazione dell’utente.
   1. Se l’utente non è associato a una pianificazione, Workfront tiene conto della pianificazione del progetto.
   1. Se il progetto non è associato a una pianificazione, Workfront prende in considerazione la pianificazione predefinita del sistema. Per informazioni sulle pianificazioni, vedere [Creare una pianificazione](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

<div class="preview">

* Nell’ambiente di anteprima:

   1. Workfront prende in considerazione la pianificazione del progetto o quella dell’utente assegnato all’attività.

      L&#39;amministratore del Workfront o del gruppo determina la pianificazione utilizzata da Workfront quando un&#39;attività viene assegnata a un utente. Per informazioni, vedere [Configurare le preferenze di progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   1. Se l&#39;utente o il progetto non dispone di una pianificazione, Workfront utilizza la pianificazione predefinita del sistema.

      I passaggi sono simili al primo scenario dopo aver compreso quale pianificazione utilizza Workfront per calcolare la durata.

</div>

* Se l&#39;attività è assegnata a più utenti:

   1. Workfront prende in considerazione la pianificazione del progetto o quella dell’assegnatario principale.

      L&#39;amministratore del Workfront o del gruppo determina la pianificazione utilizzata da Workfront quando un&#39;attività viene assegnata a più utenti. Per informazioni, vedere [Configurare le preferenze di progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   1. Se l&#39;assegnatario principale o il progetto non dispone di una pianificazione, Workfront utilizza la pianificazione predefinita del sistema.

  I passaggi sono simili al primo scenario dopo aver compreso quale pianificazione utilizza Workfront per calcolare la durata.

>[!NOTE]
>
>Se si tiene conto del tempo libero dell&#39;assegnatario principale in un progetto, le date pianificate dell&#39;attività potrebbero essere modificate, ma la durata dell&#39;attività rimane invariata. Per informazioni su come tenere conto del tempo libero dell&#39;assegnatario principale durante la pianificazione di un progetto, vedere [Configurare le preferenze di progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Durata originale di un&#39;attività padre

La durata originale di un&#39;attività è la durata che un&#39;attività aveva prima di diventare un&#39;attività padre, espressa in minuti.

Quando un&#39;attività diventa padre, la durata tra la data di inizio pianificata del primo figlio e la data di completamento pianificata dell&#39;ultimo figlio viene aggregata all&#39;attività padre e diventa la durata dell&#39;attività padre. Questo sostituisce la Durata dell&#39;attività originale.

Per ulteriori informazioni, vedere [Panoramica sulla durata originale dell&#39;attività e sulle ore pianificate originali](/help/quicksilver/manage-work/tasks/task-information/task-original-duration-and-original-planned-hours.md).

## Unità di tempo per la durata dell&#39;attività

È possibile indicare la durata dell&#39;attività sia nell&#39;ora normale che nel tempo trascorso tra le date di inizio pianificata e di completamento pianificata.

Quando si aggiorna la Durata delle attività in un elenco, è possibile utilizzare le seguenti abbreviazioni per indicare le unità di tempo in Workfront:

| Unità di tempo | Abbreviazione |
|---|---|
| Minuti | M |
| Ore | H |
| Giorni. Questa è l&#39;impostazione predefinita. | Dsbld |
| Settimane | M |
| Mesi | T, MO |
| Minuti trascorsi | EM |
| Ore trascorse | EH |
| Giorni trascorsi | ED |
| Settimane trascorse | EW |
| Mesi trascorsi | ET |

{style="table-layout:auto"}

**Esempio:** Se si desidera indicare che la durata di un&#39;attività è di 3 giorni trascorsi, digitare &quot;3 ED&quot; nel campo Durata di un elenco di attività.  È inoltre possibile selezionare l&#39;opzione desiderata per l&#39;unità di tempo di durata dal menu a discesa disponibile quando si modifica un&#39;attività o nella sezione Dettagli attività. Per informazioni sulla modifica delle attività, vedere [Modifica attività](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

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

![duration_type_triangle.png](assets/duration_type_triangle.png)

## Definire i tipi di durata

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th scope="row"><p><strong>Tipo di Durata</strong></p></th> 
   <th scope="col"> <p><strong>Funzione</strong> </p> </th> 
   <th scope="col"> <p><strong>Effetti Delle Risorse</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <th scope="col"> <p><strong>Assegnazione calcolata</strong> </p> </th> 
   <td scope="col"> <p>Calcola la percentuale di allocazione per ogni assegnatario di un'attività. </p> <p>Quando si sceglie questo Tipo di durata, è possibile immettere la durata e le ore pianificate per l'attività. Workfront divide le ore pianificate per il numero di ore all'interno della Durata dell'attività e quindi per il numero di risorse assegnate all'attività per calcolare l'allocazione per ciascun assegnatario.</p> <p>Per informazioni più dettagliate, vedere <a href="../../../manage-work/tasks/taskdurtn/calculated-assignment.md" class="MCXref xref">Panoramica del tipo di durata: assegnazione calcolata</a>.</p> </td> 
   <td scope="col">La durata e le ore pianificate non cambiano quando si aggiungono o si rimuovono assegnatari all'attività. </td> 
  </tr> 
  <tr> 
   <th scope="col"> <p><strong>Lavoro Calcolato</strong> </p> </th> 
   <td scope="col"> <p>Determina le ore pianificate (quantità di impegno) necessarie per il completamento dell'attività.</p> <p>Normalmente utilizzato quando le risorse assegnate all'attività vengono allocate per l'intera Durata dell'attività.</p> <p>Quando si sceglie questo Tipo di durata, è possibile immettere una singola Durata per l'attività. Workfront calcola le ore pianificate per l'attività moltiplicando il numero di giorni nella durata per il numero di ore lavorative nella pianificazione e per il numero di assegnatari dell'attività. </p> <p>È possibile modificare manualmente la percentuale di allocazione di ogni assegnatario all'attività, riducendo così la quantità di ore pianificate.</p> <p>Per informazioni più dettagliate, vedere <a href="../../../manage-work/tasks/taskdurtn/calculated-work.md" class="MCXref xref">Panoramica del tipo di durata: Lavoro calcolato</a>.</p> </td> 
   <td scope="col"> <p>Le ore pianificate aumentano quando gli assegnatari vengono aggiunti all'attività. </p> <p>Le ore pianificate diminuiscono quando gli assegnatari vengono rimossi dall'attività.</p> </td> 
  </tr> 
  <tr> 
   <th scope="col"> <p><strong>Impegno Aggiuntivo</strong></p> </th> 
   <td scope="col"> <p>Determina le ore pianificate in base al numero di risorse.</p> <p>Quando si sceglie questo Tipo di durata, è possibile immettere una singola Durata per l'attività. Workfront calcola le ore pianificate per l'attività moltiplicando il numero di giorni nella durata per il numero di ore lavorative nella programmazione e dividendo tale numero per il numero di assegnatari dell'attività. </p> <p>È possibile modificare manualmente la percentuale di allocazione di ogni assegnatario all'attività, ma il numero di ore pianificate rimane invariato.</p> <p>Per informazioni più dettagliate, consulta <a href="../../../manage-work/tasks/taskdurtn/effort-driven.md" class="MCXref xref">Panoramica del tipo di durata: Basata sulle risorse</a>.</p> </td> 
   <td scope="col"> <p>Le ore pianificate aumentano quando gli assegnatari vengono rimossi dall'attività.</p> <p>Le ore pianificate diminuiscono quando gli assegnatari vengono aggiunti all'attività. </p> <p>La Durata rimane invariata, indipendentemente dalle modifiche apportate al numero di assegnatari o alla loro pianificazione. </p> <p>La durata è uguale alle ore pianificate. La Durata Pianificata è uguale alle Ore Pianificate divisa per il numero di assegnatari.</p> </td> 
  </tr> 
  <tr> 
   <th scope="col"> <p><strong>Semplice</strong> </p> </th> 
   <td scope="col"> <p>Determina le ore pianificate e la durata (che sono uguali, per questo tipo di durata) in base al numero di ore per cui ogni assegnatario è allocato. </p> <p>Workfront calcola le ore pianificate sommando le ore allocate pianificate per ciascun assegnatario. </p> <p>Puoi modificare manualmente la quantità di ore per cui è allocato ciascun assegnatario, e il numero di ore pianificate e la quantità della Durata cambiano di conseguenza. Se si sceglie un numero totale di ore allocate per tutti gli assegnatari, tale numero viene diviso equamente tra ciascun assegnatario.</p> <p>Per informazioni più dettagliate, vedere <a href="../../../manage-work/tasks/taskdurtn/simple-duration-type.md" class="MCXref xref">Panoramica del tipo di durata: semplice</a>.</p> </td> 
   <td scope="col"> <p>Le ore vengono distribuite in modo uniforme tra gli assegnatari se si sceglie un numero totale di ore allocate. Tuttavia, in qualità di project manager, puoi regolare manualmente le ore per ogni assegnatario. </p> <p>È possibile modificare le ore pianificate e la durata di un'attività con un tipo di durata semplice in linea o a livello di attività. </p> <p>Se a un’attività viene assegnato un team agile, il Tipo di durata viene impostato automaticamente su Semplice e non può essere modificato. La durata dell'attività per un team Agile deve essere maggiore di 0 minuti.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Tipo di durata delle nuove attività

Il Tipo di Durata di una nuova attività corrisponde al Tipo di Durata impostato nel sistema. Il tipo di durata predefinito è Assegnazione calcolata. L’amministratore di Workfront o un amministratore gruppo può aggiornare il Tipo di durata predefinito per il sistema o per il gruppo associato al progetto. Per informazioni, consulta [Configurare le preferenze per attività e problemi a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## Modificare il tipo di durata di un&#39;attività

Per informazioni sulla modifica del tipo di durata di un&#39;attività, vedere [Aggiornare il tipo di durata di un&#39;attività](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).
