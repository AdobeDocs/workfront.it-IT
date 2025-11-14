---
product-area: projects
navigation-topic: financials
title: Panoramica sulla sostituzione delle tariffe di fatturazione dei ruoli e sul calcolo dei ricavi per un progetto
description: È possibile utilizzare le tariffe di fatturazione per calcolare i ricavi sui progetti moltiplicandoli per le ore dedicate al progetto. Per ulteriori informazioni sulle tariffe di fatturazione e sui ricavi, consulta l’articolo Panoramica sulla fatturazione e sui ricavi.
author: Lisa
feature: Work Management
exl-id: 63ba6758-ba62-48b4-89f4-d784e32a1bfa
source-git-commit: 01a80f6140650ca12aaee14115f79449dcfa2a18
workflow-type: tm+mt
source-wordcount: '3859'
ht-degree: 0%

---

# Panoramica sulla sostituzione delle tariffe di fatturazione dei ruoli e sul calcolo dei ricavi per un progetto

{{highlighted-preview}}

È possibile utilizzare le tariffe di fatturazione per calcolare i ricavi sui progetti moltiplicandoli per le ore dedicate al progetto. Per ulteriori informazioni sulle tariffe di fatturazione e sui ricavi, vedere l&#39;articolo [Panoramica su fatturazione e ricavi](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## Panoramica sulle tariffe di fatturazione mansione e sui tipi di retribuzione oraria mansione

In qualità di amministratore di Adobe Workfront, puoi associare le tariffe di fatturazione sia agli utenti che alle mansioni.\
Per ulteriori informazioni sulla creazione di utenti e sull&#39;associazione di tali utenti alle tariffe di fatturazione, vedere l&#39;articolo [Aggiungere utenti](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md). Per ulteriori informazioni sulla creazione di ruoli e sull&#39;associazione di tali ruoli alle tariffe di fatturazione, vedere l&#39;articolo [Creare e gestire ruoli](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

Le tariffe di fatturazione associate agli utenti non possono essere sostituite.

Le tariffe di fatturazione associate alle mansioni possono essere sostituite a livello di società o di progetto.

Per calcolare le entrate per i progetti in base alle tariffe di fatturazione delle mansioni, il **Tipo di retribuzione** delle attività nei progetti deve essere uno dei seguenti:

* Ore Ruolo
* Ore ruolo con limite
* Ore ruolo più fisso

Per ulteriori informazioni su **Tipo di retribuzione** e tariffe di fatturazione, vedere [Panoramica su fatturazione e retribuzioni](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## La gerarchia delle sostituzioni delle tariffe di fatturazione durante il calcolo dei ricavi

A una mansione può essere associata una tariffa di fatturazione nei seguenti modi:

* In qualità di amministratore di Workfront, puoi definire la tariffa di fatturazione a livello di sistema associata a una mansione al momento della creazione di tale mansione.\
  Per ulteriori informazioni sulla creazione di ruoli, vedere [Creare e gestire ruoli](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* In qualità di amministratore di Workfront, puoi definire la tariffa di fatturazione a livello di società per lo stesso ruolo al momento della creazione di una società.\
  Quando Workfront calcola i ricavi per i progetti associati a questa società, viene utilizzata la tariffa di fatturazione della società quando il ruolo viene assegnato alle attività, anziché la tariffa di fatturazione a livello di sistema per questa mansione.\
  I tassi di ruolo modificati a livello aziendale avranno effetto su tutti i progetti associati a tale società.

  >[!NOTE]
  >
  >Se devi aggiornare la tariffa di fatturazione della società, la tariffa sul progetto non verrà aggiornata automaticamente. Prima che la nuova tariffa aziendale venga applicata al progetto, è necessario rimuovere la società dal progetto, aggiornare la tariffa per la società, quindi ricollegare la società al progetto. Per istruzioni su come allegare una società a un progetto, vedi [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md).

  Per ulteriori informazioni sulla creazione di tariffe di fatturazione dei ruoli specifiche per una società, vedere [Creare e modificare società](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

* In qualità di amministratore di Workfront, puoi abilitare un’opzione quando modifichi un progetto per applicare al progetto le modifiche alle tariffe di fatturazione a livello di società quando gli utenti ricalcolano manualmente i dati finanziari del progetto.\
  Per ulteriori informazioni, vedere [Sostituire le tariffe di fatturazione a livello di progetto con le tariffe di fatturazione a livello di società](../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md).

<div class="preview">

* In qualità di amministratore di Workfront, puoi definire schede tariffarie con più tariffe di fatturazione per ruolo, in base alla posizione e alla data. Quando una scheda tariffa è allegata a un progetto, tutti i ruoli (per posizione, se vengono utilizzate le posizioni) e le relative tariffe di fatturazione associate vengono aggiunti alla sezione tariffe di fatturazione del progetto. Quando si allega una scheda tariffa, vengono ignorate tutte le tariffe di fatturazione esistenti sul progetto.

  Per ulteriori informazioni, consulta [Gestire le schede tariffarie](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md) e [Allegare una scheda tariffaria a un progetto](/help/quicksilver/manage-work/projects/project-finances/attach-rate-card-to-project.md).

</div>

* In qualità di project manager, puoi definire la tariffa di fatturazione per la stessa mansione a livello di progetto.\
  I tassi di ruolo modificati nel progetto avranno effetto solo su tale progetto.

  Per informazioni sulla sostituzione delle tariffe dei ruoli per il progetto, vedere [Sostituire le tariffe di fatturazione dei ruoli a livello di progetto](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

>[!IMPORTANT]
>
>Se una mansione è associata a una tariffa di fatturazione a livello di sistema, di società e di progetto, Workfront calcola i ricavi delle attività utilizzando la tariffa di fatturazione della mansione a livello di progetto, quando utilizza le tariffe delle mansioni. I ricavi di tutte le attività vengono aggregati ai ricavi del progetto.

## Sostituisci tariffe di fatturazione mansione a livello di progetto

In qualità di project manager, puoi specificare la tariffa di fatturazione per una mansione in un progetto specifico. Questa tariffa di fatturazione a livello di progetto sostituisce la tariffa di fatturazione a livello di sistema per questa mansione. Per calcolare i ricavi, Workfront utilizza la tariffa di fatturazione a livello di progetto della mansione, anziché la tariffa di fatturazione a livello di sistema.

<span class="preview">È inoltre possibile allegare al progetto una scheda delle tariffe, che importerà le tariffe di fatturazione della mansione dalla scheda delle tariffe nel progetto.</span>

Per informazioni su come sostituire le tariffe di fatturazione dei ruoli a livello di progetto, vedere [Sostituire le tariffe di fatturazione dei ruoli a livello di progetto](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

Per ulteriori informazioni sulla mansione utilizzata per calcolare i ricavi sul progetto, vedere la sezione &quot;Calcolo dei ricavi per le attività basate sulle assegnazioni di utenti e ruoli&quot; in [Panoramica su fatturazione e ricavi](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md). <span class="preview">Per informazioni su come allegare una scheda tariffe a un progetto, vedere [Allegare una scheda tariffe a un progetto](/help/quicksilver/manage-work/projects/project-finances/attach-rate-card-to-project.md).</span>

>[!NOTE]
>
>Nel caso del reddito effettivo, le tariffe di fatturazione applicate alle ore aggiunte a una fatturazione contrassegnata come Fatturata, non devono essere influenzate dalle sostituzioni delle tariffe di fatturazione che si verificano dopo la fatturazione della fatturazione.

## Panoramica della sezione Tariffe di fatturazione di un progetto

Dopo aver specificato le tariffe di fatturazione sostitutive per le mansioni associate al progetto, puoi visualizzare tutte le mansioni e le sostituzioni corrispondenti nella scheda **Tariffe di fatturazione** del progetto.

Osserva le seguenti informazioni nell&#39;elenco di **Tariffe di fatturazione**:

* [Raggruppamento mansioni](#job-role-grouping)
* [Valore tariffa di fatturazione del progetto](#project-billing-rate-value)
* [Valore tariffa di fatturazione predefinita](#default-billing-rate-value)
* [Valore tariffa di fatturazione società](#company-billing-rate-value)
* [Più valori di tariffa di fatturazione e intervalli di tempo](#multiple-billing-rate-values-and-timeframes)

### Raggruppamento mansioni {#job-role-grouping}

Le tariffe di fatturazione sono raggruppate nell&#39;area **Tariffe di fatturazione** in base alle rispettive mansioni. <span class="preview">Se al progetto è allegata una scheda delle tariffe, anche le mansioni sono raggruppate per scheda delle tariffe. Se le posizioni vengono applicate ai ruoli, il nome della posizione viene incluso nel nome del ruolo. Lo stesso ruolo potrebbe essere elencato per più posizioni.</span>

### Valore tariffa di fatturazione progetto {#project-billing-rate-value}

Nella riga di raggruppamento corrispondente a una mansione, notare la tariffa di fatturazione per tale mansione a livello di progetto nella colonna **Tariffa di fatturazione progetto**. Se il ruolo dispone di più tassi di sostituzione, il tasso di sostituzione corrispondente alla data corrente viene visualizzato nella riga di raggruppamento nella colonna **Tariffa di fatturazione progetto**.

### Valore tariffa di fatturazione predefinita {#default-billing-rate-value}

Nella riga di raggruppamento di una mansione, notare la tariffa di fatturazione per tale mansione a livello di sistema nella colonna **Tariffa di fatturazione predefinita**.

>[!NOTE]
>
>Se sono presenti tariffe di fatturazione del progetto per una mansione, la **Tariffa di fatturazione predefinita** non viene mai applicata al calcolo dei ricavi per il progetto. Per calcolare i ricavi vengono applicate solo le **tariffe di fatturazione del progetto**.

### Valore tariffa di fatturazione della società {#company-billing-rate-value}

Nella riga di raggruppamento di una mansione, notare la tariffa di fatturazione per tale mansione a livello aziendale nella colonna **Tariffa di fatturazione società**. Ciò significa che esiste un’azienda associata a questo progetto e che questa mansione ha una tariffa di fatturazione diversa per tale azienda. Viene visualizzata la tariffa di fatturazione per l’azienda, anche se è uguale alla tariffa del progetto.

>[!NOTE]
>
><span class="preview">Quando al progetto viene allegata una scheda delle tariffe, le **Tariffe di fatturazione della società** non vengono importate nelle tariffe di fatturazione. I calcoli si basano sulle tariffe delle schede delle tariffe o sulle tariffe aziendali per le mansioni.</span>
>
>Se sono presenti tariffe di fatturazione del progetto per una mansione, la **Tariffa di fatturazione società** non viene mai applicata al calcolo dei ricavi per il progetto. Per calcolare le entrate vengono applicate solo le **tariffe di fatturazione del progetto**.

### Più valori di tariffa di fatturazione e intervalli di tempo {#multiple-billing-rate-values-and-timeframes}

Se si dispone di più tariffe di fatturazione sostitutive per una mansione specifica, queste vengono elencate nel raggruppamento per tale mansione. Utilizzando la modifica in linea, puoi modificare le tariffe di sostituzione e **Inizio** **Data** e **Data di fine** delle tariffe di fatturazione di sostituzione in questa scheda.

>[!NOTE]
>
>Impossibile specificare una **Data inizio** per la prima tariffa di sostituzione e non è possibile specificare una **Data fine** per l&#39;ultima tariffa di sostituzione. Workfront presuppone che la prima tariffa di sostituzione venga applicata a tutte le ore con una data precedente alla **Data di fine** della prima sostituzione e che l&#39;ultima tariffa di sostituzione venga applicata a tutte le ore con una data successiva alla **Data di inizio** dell&#39;ultima sostituzione.\
>Se viene registrata un’ora prima della data di inizio pianificata del progetto, viene utilizzata la prima tariffa di fatturazione.\
>Se viene registrata un’ora dopo la data di completamento pianificata del progetto, viene utilizzata l’ultima tariffa di fatturazione.

## Calcola retribuzione pianificata

* [Calcola il reddito pianificato in base a una sostituzione della tariffa di fatturazione una tantum](#calculate-planned-revenue-based-on-a-one-time-billing-rate-override)
* [Calcola il reddito pianificato in base a più sostituzioni della tariffa di fatturazione](#calculate-planned-revenue-based-on-multiple-billing-rate-overrides)
* [Distribuzione delle ore pianificate per la durata di un&#39;attività](#distribution-of-planned-hours-across-the-duration-of-a-task)

### Calcola il reddito pianificato in base alla sostituzione una tantum della tariffa di fatturazione {#calculate-planned-revenue-based-on-a-one-time-billing-rate-override}

Quando si calcola la retribuzione pianificata in base a una sostituzione della tariffa di fatturazione una tantum, tenere presente quanto segue:

* Quando il tipo di retribuzione **1} di un&#39;attività è** Ore ruolo **, Workfront moltiplica le Ore pianificate di un&#39;attività per la tariffa di fatturazione della mansione associata all&#39;attività per calcolare la retribuzione pianificata dell&#39;attività.**

* Quando la tariffa di fatturazione della mansione è stata sostituita a livello di progetto, Workfront utilizza la tariffa di sostituzione del progetto per calcolare la Retribuzione pianificata.
* Quando un&#39;attività ha più assegnazioni, la Retribuzione pianificata viene calcolata moltiplicando la tariffa di fatturazione della mansione di ciascuna assegnazione e la rispettiva allocazione delle Ore pianificate.

>[!NOTE]
>
>Le ore pianificate per assegnazione non corrispondono alle ore pianificate per l&#39;attività, nel caso di più assegnazioni.

Per ulteriori informazioni sulla mansione utilizzata per calcolare i ricavi pianificati, vedere la sezione &quot;Informazioni sui calcoli dei ricavi per le attività basate sulle assegnazioni di utenti e ruoli&quot; nell&#39;articolo [Panoramica su fatturazione e ricavi](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

### Calcola il reddito pianificato in base a più sostituzioni della tariffa di fatturazione {#calculate-planned-revenue-based-on-multiple-billing-rate-overrides}

Quando si calcola la retribuzione pianificata in base a più sostituzioni della tariffa di fatturazione, tenere presente quanto segue:

* Quando il tipo di retribuzione **1} di un&#39;attività è** Ore ruolo **, Workfront moltiplica le Ore pianificate di un&#39;attività per la tariffa di fatturazione della mansione associata all&#39;attività per calcolare la retribuzione pianificata dell&#39;attività.**

  Per ulteriori informazioni sulla mansione utilizzata per calcolare i ricavi pianificati, vedere la sezione &quot;Informazioni sui calcoli dei ricavi per le attività basate sulle assegnazioni di utenti e ruoli&quot; nell&#39;articolo [Panoramica su fatturazione e ricavi](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

* In caso di sostituzioni di più tariffe di fatturazione, la tariffa in base alla quale vengono moltiplicate le ore pianificate cambia durante un&#39;attività. Per impostazione predefinita, Workfront distribuisce le ore pianificate in modo uniforme per tutta la durata di un&#39;attività, allocando un numero uguale di ore per ogni giorno dell&#39;attività. Quando si calcolano le **retribuzioni pianificate** per un&#39;attività, Workfront moltiplica l&#39;Ora pianificata al giorno per la tariffa di fatturazione di quel giorno. In caso di tariffe di fatturazione multiple, quella tariffa potrebbe essere diversa ogni giorno.

  Ad esempio, si dispone di un&#39;attività con un Tipo di Reddito **Orario Ruolo**. L&#39;attività ha una durata di 5 giorni e un valore di Lavoro Necessario di 40 ore. Le ore pianificate al giorno sono di 8 ore. Assegnare un ruolo di Project Manager all&#39;attività e sostituire la tariffa di fatturazione di questa mansione per gli ultimi 3 giorni dell&#39;attività, in modo da avere una tariffa di fatturazione Tasso 1 per i primi due giorni e una tariffa di fatturazione Tasso 2 per i restanti 3 giorni dell&#39;attività per questa mansione.

  La formula che calcola il **ricavo pianificato** di questa attività è:

  ```
  Planned Revenue = (Rate 1) * (Planned Hours for Day 1) + (Rate 1) * (Planned hours for Day 2) + (Rate 2) * (Planned hours for Day 3) + (Rate 2) * (Planned hours for Day 4) + (Rate 2) * (Planned hours for Day 5)
  ```

Per ulteriori informazioni sulla ricerca della quantità di ore pianificate al giorno in Workfront, vedere la sezione [Distribuzione delle ore pianificate per la durata di un&#39;attività](#distribution-of-planned-hours-across-the-duration-of-a-task) in questo articolo.

>[!NOTE]
>
>Se si dispone di più assegnatari per l&#39;attività, la quantità di ore pianificate viene prima distribuita a ogni assegnatario e quindi a ogni giorno durante la durata dell&#39;attività. In questo caso, la Retribuzione pianificata verrà calcolata tenendo conto della quantità di ore giornaliere per ogni assegnatario e della tariffa di fatturazione di ogni mansione che potrebbe cambiare durante la durata dell&#39;attività, in caso di più tariffe di fatturazione.

### Distribuzione delle ore pianificate per la durata di un&#39;attività {#distribution-of-planned-hours-across-the-duration-of-a-task}

Quando si comprende la distribuzione delle ore pianificate per la durata di un&#39;attività, tenere presente quanto segue:

* Per impostazione predefinita, Workfront distribuisce le ore pianificate in modo uniforme per la durata di un&#39;attività, allocando un numero uguale di ore pianificate per ogni giorno dell&#39;attività, in base alla disponibilità della pianificazione del progetto.

  Per ulteriori informazioni sulla distribuzione delle ore pianificate per la durata di un&#39;attività, vedere la sezione &quot;Informazioni sulla distribuzione delle ore pianificate per la durata di un&#39;attività&quot; nell&#39;articolo [Panoramica sulle ore pianificate](../../../manage-work/tasks/task-information/planned-hours.md).

  >[!NOTE]
  >
  >Le ore pianificate al giorno sono l&#39;allocazione delle ore pianificate per ogni giorno durante la durata dell&#39;attività. Se l&#39;attività ha un&#39;assegnazione, questo numero rappresenta anche le Ore pianificate al giorno per assegnazione. Se l&#39;attività ha più assegnazioni, le ore pianificate al giorno per ogni assegnazione sono diverse dalle ore pianificate al giorno per l&#39;attività. In Workfront non è disponibile alcuna rappresentazione visiva per le ore pianificate al giorno per assegnazione, per le attività con più assegnazioni.
  >
  >
  >Le Ore pianificate al giorno vengono moltiplicate per la tariffa di fatturazione per la mansione assegnata all&#39;attività per quel giorno per calcolare la Retribuzione pianificata al giorno per quell&#39;attività. Una somma di tutte le Retribuzioni pianificate giornaliere calcolata in questo modo equivale alla Retribuzione pianificata per l&#39;attività.

## Calcola retribuzione effettiva

* [Calcola il reddito effettivo in base a una sostituzione della tariffa di fatturazione una tantum](#calculate-actual-revenue-based-on-a-one-time-billing-rate-override)
* [Calcola il reddito effettivo in base a più sostituzioni della tariffa di fatturazione](#calculate-actual-revenue-based-on-multiple-billing-rate-overrides)

### Calcola il reddito effettivo in base alla sostituzione della tariffa di fatturazione una tantum {#calculate-actual-revenue-based-on-a-one-time-billing-rate-override}

Quando si calcola il reddito effettivo in base a una sostituzione della tariffa di fatturazione una tantum, tenere presente quanto segue:

* Se il tipo di retribuzione **Tipo di retribuzione** di un&#39;attività è **Ore ruolo**, Workfront moltiplica le **Ore effettive** di un&#39;attività per la tariffa di fatturazione della mansione associata all&#39;attività per calcolare le **Entrate effettive** dell&#39;attività. Le ore effettive sono ore registrate direttamente nell&#39;attività.

  Per ulteriori informazioni sulla mansione utilizzata per calcolare il **ricavo effettivo**, vedere la sezione &quot;Informazioni sui calcoli dei ricavi per le attività basate sulle assegnazioni di utenti e ruoli&quot; nell&#39;articolo [Panoramica su fatturazione e ricavi](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

* Se la tariffa di fatturazione della mansione è stata sostituita a livello di progetto, Workfront utilizza la tariffa di sostituzione del progetto per calcolare la Retribuzione effettiva. Quando si sostituisce la tariffa di fatturazione della mansione nel progetto, il **Ricavo effettivo** del progetto viene ricalcolato automaticamente utilizzando la nuova tariffa adeguata.

  Per informazioni sulla sostituzione delle tariffe dei ruoli per il progetto, vedere [Sostituire le tariffe di fatturazione dei ruoli a livello di progetto](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

>[!NOTE]
>
>Se si desidera mantenere le ore già registrate nel progetto prima di sovrascrivere la tariffa di fatturazione originale fatturata alla tariffa originale, è necessario includerle in un **record fatturazione** e contrassegnare il **record fatturazione** come **fatturato**. In caso contrario, il **Ricavo effettivo** dalle ore registrate prima che la tariffa di fatturazione fosse sostituita per il progetto verrà ricalcolato utilizzando la nuova tariffa quando vengono ricalcolati i dati finanziari dei progetti.\
>Per ulteriori informazioni sull&#39;inclusione delle ore in un record di fatturazione e sul contrassegno come **Fatturato**, vedi l&#39;articolo [Crea record di fatturazione](../../../manage-work/projects/project-finances/create-billing-records.md).

### Calcola il reddito effettivo in base a più sostituzioni della tariffa di fatturazione {#calculate-actual-revenue-based-on-multiple-billing-rate-overrides}

Quando si calcola il reddito effettivo in base a più sostituzioni della tariffa di fatturazione, tenere presente quanto segue:

* Se il tipo di retribuzione **Tipo di retribuzione** di un&#39;attività è **Ore ruolo**, Workfront moltiplica le **Ore effettive** dell&#39;attività con la tariffa di fatturazione dei ruoli assegnati all&#39;attività per calcolare le **Entrate effettive** dell&#39;attività. Le ore effettive sono ore registrate direttamente nell&#39;attività.

* In caso di sostituzioni di più tariffe di fatturazione, la tariffa in base alla quale le **Ore effettive** vengono moltiplicate per calcolare le **Entrate effettive** potrebbe cambiare durante la durata di un&#39;attività. Workfront utilizza la tariffa di fatturazione della mansione il cui intervallo di tempo corrisponde alla **Data di ingresso** delle ore registrate per l&#39;attività per calcolare il **Ricavo effettivo.**

  Ad esempio, un&#39;attività ha il **Tipo di retribuzione** di **Ore Ruolo** ed è assegnata al ruolo di Project Manager. Sostituisci la tariffa di fatturazione di questa mansione con la tariffa 1 per le date tra il 19 giugno e il 25 giugno. A partire dal 26 giugno, sostituisci la tariffa di fatturazione con la Tariffa 2. Registrare 2 ore per il 20 giugno e 3 ore per il 28 giugno.

  Workfront calcola il **ricavo effettivo** per questa attività utilizzando la seguente formula:

  ```
  Actual Revenue = 2 * Rate 1 + 3 * Rate 2
  ```

  Per ulteriori informazioni sulla mansione utilizzata per calcolare il **ricavo effettivo**, vedere la sezione &quot;Informazioni sui calcoli dei ricavi per le attività basate sulle assegnazioni di utenti e ruoli&quot; nell&#39;articolo [Panoramica su fatturazione e ricavi](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## L’impatto dei fusi orari nel calcolo dei ricavi in base a più tariffe di fatturazione

Gli utenti possono visualizzare ore pianificate al giorno diverse dagli altri utenti, se si verificano differenze di fuso orario tra loro e altre entità in Workfront. I seguenti scenari possono distorcere le informazioni sulle ore pianificate al giorno per un utente rispetto a quelle visualizzate da un altro utente:

* I computer dei due utenti potrebbero essere impostati per due fusi orari diversi
* I due profili utente in Workfront potrebbero essere impostati su due fusi orari diversi
* Il fuso orario associato al profilo utente potrebbe essere diverso da quello di Workfront
* Il fuso orario associato al profilo utente potrebbe essere diverso da quello della pianificazione del progetto.

In questi casi, il numero di ore pianificate al giorno potrebbe essere diverso tra due utenti che non condividono le stesse impostazioni per i fusi orari. Visualizzeranno anche numeri di Ricavi pianificati diversi quando si utilizzano sostituzioni di tariffe di fatturazione multiple su un progetto.

* [Calcola la retribuzione pianificata per utenti con fusi orari diversi](#calculate-planned-revenue-for-users-in-different-time-zones)
* [Calcola la retribuzione effettiva per gli utenti con fusi orari diversi](#calculate-actual-revenue-for-users-in-different-time-zones)

### Calcola il reddito pianificato per gli utenti in diversi fusi orari {#calculate-planned-revenue-for-users-in-different-time-zones}

>[!NOTE]
>
>Se utenti con fusi orari diversi lavorano sugli stessi progetti, ti consigliamo di non modificare le sostituzioni delle tariffe di fatturazione per i progetti durante la settimana. In questo modo potrebbe essere visualizzata una quantità errata di Reddito Pianificato per il progetto, a causa delle differenze di ore tra i fusi orari nella pianificazione degli utenti e il fuso orario del sistema Workfront. La maggior parte delle pianificazioni consente di escludere i fine settimana dai calcoli delle ore pianificate. Se si verifica una modifica nella sostituzione della tariffa di fatturazione di una mansione, è meglio che questa si verifichi durante un fine settimana piuttosto che a metà settimana, quando potrebbe coincidere con la metà della durata di un&#39;attività.

Quando calcoli la Retribuzione Pianificata per utenti con fusi orari diversi, considera quanto segue:

* Per le attività con **Tipo di retribuzione** di **Ore ruolo** e assegnate alle mansioni, **Reddito pianificato** viene calcolato moltiplicando le **Ore pianificate** di un&#39;attività per la tariffa di fatturazione della mansione.

* Le **ore pianificate** sono distribuite in modo uniforme nell&#39;arco della **Durata** dell&#39;attività.

* La **Durata** è il periodo di tempo compreso tra il **Inizio pianificato** **Data** e la **Data di completamento pianificata** dell&#39;attività. Poiché la **Data inizio pianificata** e la **Data completamento pianificata** delle attività possono variare a seconda dei fusi orari degli utenti che visualizzano l&#39;attività, la quantità di ore pianificate al giorno potrebbe essere diversa per due utenti in due fusi orari diversi.

* La quantità di ore pianificate al giorno non modifica la retribuzione pianificata di un progetto se la tariffa di fatturazione della mansione non viene modificata o se è presente una sola sostituzione della tariffa di fatturazione. In questo caso, anche se due utenti di due fusi orari diversi visualizzano ore pianificate al giorno diverse, il ricavo pianificato complessivo del progetto è identico tra i due utenti.

  Tuttavia, nel caso di sostituzioni di più tariffe di fatturazione, il **Ricavo pianificato** complessivo del progetto potrebbe sembrare diverso per due utenti in due fusi orari diversi, perché si basa sulla quantità di ore pianificate al giorno (che potrebbe essere diversa per i due utenti) e sulla sostituzione della tariffa di fatturazione (che potrebbe essere diversa per lo stesso giorno, quando ogni utente osserva l&#39;attività nel proprio fuso orario).

* L&#39;importo preciso di **Entrate pianificate** è quello visualizzato dall&#39;utente che ha lo stesso fuso orario dell&#39;istanza di Workfront. L&#39;amministratore di Workfront definisce il fuso orario di Workfront nell&#39;area Informazioni cliente di sistema.\
  Per ulteriori informazioni sulla definizione del fuso orario per il sistema, vedere l&#39;articolo [Configurare le informazioni di base per il sistema](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

### Calcola la retribuzione effettiva per gli utenti con fusi orari diversi {#calculate-actual-revenue-for-users-in-different-time-zones}

Nel calcolare la retribuzione effettiva per utenti con fusi orari diversi, considera quanto segue:

* Se il tipo di retribuzione **Tipo di retribuzione** di un&#39;attività è **Ore ruolo**, Workfront moltiplica le **Ore effettive** dell&#39;attività con la tariffa di fatturazione dei ruoli assegnati all&#39;attività per calcolare le **Entrate effettive**. Le ore effettive sono ore registrate direttamente nell&#39;attività.

* In caso di sostituzioni di più tariffe di fatturazione, Workfront utilizza la tariffa di fatturazione della mansione il cui intervallo di tempo corrisponde alla **Data di ingresso** delle ore registrate per l&#39;attività per calcolare **Entrate effettive**.

* Poiché non è presente alcun timestamp nella **Data di ingresso** delle ore registrate e non è presente alcun timestamp negli intervalli di date delle sostituzioni di più tariffe di fatturazione, **I calcoli delle entrate effettive** non sono influenzati dal fuso orario associato agli utenti.

Per ulteriori informazioni sulla mansione utilizzata per calcolare il **ricavo effettivo**, vedere la sezione &quot;Informazioni sui calcoli dei ricavi per le attività basate sulle assegnazioni di utenti e ruoli&quot; nell&#39;articolo [Panoramica su fatturazione e ricavi](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## Ricalcola dati finanziari progetto

I dati finanziari vengono calcolati su un progetto in base alle modifiche apportate nelle ore registrate per il progetto.

Se i tassi vengono modificati durante il ciclo di vita di un progetto, è possibile ricalcolare manualmente i costi e i ricavi del progetto utilizzando l&#39;opzione Ricalcola contabilità su un progetto. Inoltre, alcune azioni attivano un ricalcolo automatico.

Per ulteriori informazioni sul ricalcolo dei dati finanziari del progetto, vedere l&#39;articolo [Ricalcolare i dati finanziari del progetto](../../../manage-work/projects/project-finances/recalculate-project-finances.md).

## Aggiungere una nuova tariffa di fatturazione utilizzando l’API

Per aggiungere una nuova tariffa di fatturazione per una mansione utilizzando l&#39;API, eseguire un&#39;azione *setRatesForRole* per l&#39;oggetto **Rate** utilizzando il metodo *PUT*.
L&#39;azione e i campi data nell&#39;oggetto **Rate** sono disponibili nella versione 8.0 dell&#39;API.
Se hai già definito diverse tariffe di fatturazione per una mansione in un progetto e desideri aggiungerne una nuova con un nuovo intervallo di date, devi includere sia la tariffa esistente che quella da aggiungere nella stessa chiamata API. È simile a come si aggiornano le raccolte sugli oggetti.

La seguente chiamata API è un esempio in cui **attachableID** è l&#39;**ID progetto** del progetto in cui si sta aggiungendo la tariffa e **RoleID** è il **ID ruolo** per il quale si sta aggiungendo la nuova tariffa di fatturazione.<pre>{</pre><pre>&quot;attachableID&quot;:&quot;593f01500000557d75fdd4fdfcc624f2&quot;,</pre><pre>&quot;attachableObjCode&quot;:&quot;PROJ&quot;,</pre><pre>&quot;roleID&quot;:&quot;544820df000014148cda5136d4b79d09&quot;, </pre><pre>&quot;tariffe&quot;:[</pre><pre>         {&quot;rateValue&quot;:&quot;0.00&quot;,&quot;startDate&quot;:null,&quot;endDate&quot;:&quot;2017-06-11&quot;},</pre><pre>         {&quot;rateValue&quot;:&quot;45.00&quot;,&quot;startDate&quot;:&quot;2017-06-12&quot;,&quot;endDate&quot;:&quot;2017-06-17&quot;},</pre><pre>         {&quot;rateValue&quot;:&quot;95.00&quot;,&quot;startDate&quot;:&quot;2017-06-21&quot;,&quot;endDate&quot;:null}</pre><pre>]</pre><pre>}</pre>Per ulteriori informazioni sull&#39;utilizzo dell&#39;API Workfront, vedere l&#39;articolo [Nozioni di base sull&#39;API](https://experience.workfront.com/s/article/API-Basics-638808549).
