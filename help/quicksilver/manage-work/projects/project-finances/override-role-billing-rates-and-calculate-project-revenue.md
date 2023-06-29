---
product-area: projects
navigation-topic: financials
title: Panoramica sulla sostituzione delle tariffe di fatturazione dei ruoli e sul calcolo dei ricavi per un progetto
description: È possibile utilizzare le tariffe di fatturazione per calcolare i ricavi sui progetti moltiplicandoli per le ore dedicate al progetto. Per ulteriori informazioni sulle tariffe di fatturazione e sui ricavi, consulta l’articolo Panoramica sulla fatturazione e sui ricavi.
author: Alina, Lisa
feature: Work Management
exl-id: 63ba6758-ba62-48b4-89f4-d784e32a1bfa
source-git-commit: 1517e3e28fe536a8a72d2802919c8b8819e9ea1a
workflow-type: tm+mt
source-wordcount: '3852'
ht-degree: 0%

---

# Panoramica sulla sostituzione delle tariffe di fatturazione dei ruoli e sul calcolo dei ricavi per un progetto

{{highlighted-preview}}

È possibile utilizzare le tariffe di fatturazione per calcolare i ricavi sui progetti moltiplicandoli per le ore dedicate al progetto. Per ulteriori informazioni sulle tariffe di fatturazione e sulle entrate, consulta l’articolo [Panoramica su fatturazione e ricavi](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: drafted because the only procedure here was moved to a different article.&nbsp;This stays as an overview)</p>
<h2>Access requirements</h2>
<p>You must have the following access to perform the steps in this article:</p>
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader">Adobe Workfront plan*</td>
<td> <p>Any</p> </td>
</tr>
<tr>
<td role="rowheader">Adobe Workfront license*</td>
<td> <p>Plan </p> </td>
</tr>
<tr>
<td role="rowheader">Access level configurations*</td>
<td> <p>Edit access to Projects and Financial&nbsp;Data</p> <note type="note">
If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see
<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.
</note> </td>
</tr>
<tr>
<td role="rowheader">Object permissions</td>
<td> <p>Manage permissions to the project with permissions to Manage Finance</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td>
</tr>
</tbody>
</table>
<p>*To find out what plan, license type, or access you have, contact your Workfront administrator.</p>
</div>
-->

## Panoramica sulle tariffe di fatturazione mansione e sui tipi di retribuzione oraria mansione

In qualità di amministratore di Adobe Workfront, puoi associare le tariffe di fatturazione sia agli utenti che alle mansioni.\
Per ulteriori informazioni sulla creazione di utenti e sulla loro associazione alle tariffe di fatturazione, consulta l’articolo [Aggiungi utenti](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md). Per ulteriori informazioni sulla creazione di mansioni e sulla loro associazione alle tariffe di fatturazione, consulta l’articolo [Creare e gestire le mansioni](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

Le tariffe di fatturazione associate agli utenti non possono essere sostituite.

Le tariffe di fatturazione associate alle mansioni possono essere sostituite a livello di società o di progetto.

Per calcolare i ricavi sui progetti in base alle tariffe di fatturazione delle mansioni, il **Tipo di retribuzione** tra le attività relative ai progetti deve figurare una delle seguenti:

* Ore Ruolo
* Ore Ruolo w/Cap
* Ore ruolo più fisso

Per ulteriori informazioni su **Tipo di retribuzione** e le tariffe di fatturazione, consulta [Panoramica su fatturazione e ricavi](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## La gerarchia delle sostituzioni delle tariffe di fatturazione durante il calcolo dei ricavi

A una mansione può essere associata una tariffa di fatturazione nei seguenti modi:

* In qualità di amministratore di Workfront, puoi definire la tariffa di fatturazione a livello di sistema associata a una mansione al momento della creazione di tale mansione.\
  Per ulteriori informazioni sulla creazione di mansioni, consulta [Creare e gestire le mansioni](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* In qualità di amministratore di Workfront, puoi definire la tariffa di fatturazione a livello di società per lo stesso ruolo al momento della creazione di una società.\
  Quando Workfront calcola i ricavi per i progetti associati a questa società, viene utilizzata la tariffa di fatturazione della società quando il ruolo viene assegnato alle attività, anziché la tariffa di fatturazione a livello di sistema per questa mansione.\
  I tassi di ruolo modificati a livello aziendale avranno effetto su tutti i progetti associati a tale società.

  >[!NOTE]
  >
  >Se devi aggiornare la tariffa di fatturazione della società, la tariffa sul progetto non verrà aggiornata automaticamente. Prima di rendere effettiva la nuova tariffa aziendale sul progetto, è necessario rimuovere la società dal progetto, aggiornare la tariffa per la società, quindi ricollegare la società al progetto. Per istruzioni su come associare un&#39;azienda a un progetto, vedi [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md).

  Per ulteriori informazioni sulla creazione di tariffe di fatturazione per mansioni specifiche per un’azienda, consulta [Creare e modificare le società](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

* In qualità di amministratore di Workfront, puoi abilitare un’opzione quando modifichi un progetto per applicare al progetto le modifiche alle tariffe di fatturazione a livello di società quando gli utenti ricalcolano manualmente i dati finanziari del progetto.\
  Per ulteriori informazioni, consulta [Sostituisci tariffe di fatturazione a livello di progetto con tariffe di fatturazione a livello di società](../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md).

<div class="preview">

* In qualità di amministratore di Workfront, puoi definire schede tariffarie con più tariffe di fatturazione per ruolo, in base alla posizione e alla data. Quando una scheda tariffa è allegata a un progetto, tutti i ruoli (per posizione, se vengono utilizzate le posizioni) e le relative tariffe di fatturazione associate vengono aggiunti alla sezione tariffe di fatturazione del progetto. Quando si allega una scheda tariffa, vengono ignorate tutte le tariffe di fatturazione esistenti sul progetto.

  Per ulteriori informazioni, consulta [Gestire le schede delle tariffe](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md) e [Allegare una scheda tariffe a un progetto](/help/quicksilver/manage-work/projects/project-finances/attach-rate-card-to-project.md).

</div>

* In qualità di project manager, puoi definire la tariffa di fatturazione per la stessa mansione a livello di progetto.\
  I tassi di ruolo modificati nel progetto avranno effetto solo su tale progetto.

  Per informazioni sulla sostituzione delle percentuali di ruolo per il progetto, consulta [Sostituisci tariffe di fatturazione mansione a livello di progetto](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

>[!IMPORTANT]
>
>Se una mansione è associata a una tariffa di fatturazione a livello di sistema, di società e di progetto, Workfront calcola i ricavi delle attività utilizzando la tariffa di fatturazione della mansione a livello di progetto, quando utilizza le tariffe delle mansioni. I ricavi di tutte le attività vengono aggregati ai ricavi del progetto.

## Sostituisci tariffe di fatturazione mansione a livello di progetto

In qualità di project manager, puoi specificare la tariffa di fatturazione per una mansione in un progetto specifico. Questa tariffa di fatturazione a livello di progetto sostituisce la tariffa di fatturazione a livello di sistema per questa mansione. Per calcolare i ricavi, Workfront utilizza la tariffa di fatturazione a livello di progetto della mansione, anziché la tariffa di fatturazione a livello di sistema.

<span class="preview">Puoi anche allegare al progetto una scheda delle tariffe, che importerà nel progetto le tariffe di fatturazione della mansione dalla scheda delle tariffe.</span>

Per informazioni su come sostituire le tariffe di fatturazione dei ruoli a livello di progetto, consulta [Sostituisci tariffe di fatturazione mansione a livello di progetto](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

Per ulteriori informazioni sulla mansione utilizzata per calcolare i ricavi sul progetto, vedere la sezione &quot;Calcolo dei ricavi per le attività in base alle assegnazioni di utenti e ruoli&quot; in [Panoramica su fatturazione e ricavi](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md). <span class="preview">Per informazioni su come allegare una scheda delle tariffe a un progetto, consulta [Allegare una scheda tariffe a un progetto](/help/quicksilver/manage-work/projects/project-finances/attach-rate-card-to-project.md).</span>

>[!NOTE]
>
>Nel caso del reddito effettivo, le tariffe di fatturazione applicate alle ore aggiunte a una fatturazione contrassegnata come Fatturata, non devono essere influenzate dalle sostituzioni delle tariffe di fatturazione che si verificano dopo la fatturazione della fatturazione.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: drafted and linked above to the stand-alone article for overriding billing rates on projects.)</p>
<p>You can override the billing rate of a job role on a project in the following ways:</p>
<ul>
<li>One time, by selecting a new rate for the job role.<br>The new rate is used for the entire duration of the project, to calculate revenue. </li>
</ul>
<ul>
<li>Several times, by selecting several new rates for specific date ranges. <br>A different rate can be used during each specified date range.</li>
</ul>
<p>To override a billing rate for a project:</p>
<ol>
<li value="1">Go to the project you want to override billing rates for.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Billing Rates</strong> in the left panel. You might have to first click <strong>Show More</strong>. </p> </li>
<li value="3"> <p>Click <strong>Add Billing Rate</strong> > <strong>New Billing Rate</strong>.</p> <p>The New Billing Rate box opens</p> <p> <img src="assets/override-billing-rate-on-project-nwe-350x310.png" style="width: 350;height: 310;"> </p> <p> <br>The <strong>Default Billing Rate</strong> field displays the system-level rate for this job role.</p> </li>
<li value="4">In the <strong>Job Role</strong> field, select the job role you want to change the billing rate for.<br></li>
<li value="5">In the <strong>Billing Rates 1</strong> field, enter the one time billing rate override, then click <strong>Save</strong> to override the billing rate one time, <br>Or Click <strong>Add Rate</strong> to add more billing rate overrides.</li>
<li value="6">(Conditional) If you are adding more than one billing rate override, specify the following information:<br>- <strong>Billing Rates 1</strong>: the value of the Billing Rate from the beginning of the project to the first date of the first override. This is typically the same amount as the <strong>Default Rate</strong>.<br>- <strong>Start Date</strong>: this is the date when the Default Rate ends.<br>- <strong>End Date</strong>: the date when the new billing rate override ends. <br>Workfront applies the override job role rate to the hours that occur during the time frames specified when calculating revenue on the project.<br>There should be no gaps between the time frames of two override rates. The <strong>Start Date</strong> of an override rate should be the day immediately following the <strong>End Date</strong> of the previous override date.<br><note type="note">
You cannot specify a
<strong>Start Date</strong> for the first override rate, nor an
<strong>End Date</strong> for the last override rate. We recommend that you use the Default Rate for the first override rate.
<br>Workfront assumes that the first override rate is applied for all hours with a date older than the
<strong>End Date</strong> of the first override, and that the last override rate is applied for all hours with a date newer than the
<strong>Start Date</strong> of the last override.
<br>If an hour is logged before the Planned Start Date of the project the very first billing rate is used.
<br>If an hour is logged after the Planned Completion Date of the project the very last billing rate is used.
</note><br></li>
<li value="7">Click <strong>Save</strong>.</li>
</ol>
</div>
-->

## Panoramica della sezione Tariffe di fatturazione di un progetto

Dopo aver specificato le tariffe di fatturazione sostitutive per i ruoli associati al progetto, puoi visualizzare tutte le mansioni e le relative sostituzioni in **Tariffe di fatturazione** del progetto.

Osserva le seguenti informazioni nell’elenco di **Tariffe di fatturazione**:

* [Raggruppamento mansioni](#job-role-grouping)
* [Valore tariffa di fatturazione progetto](#project-billing-rate-value)
* [Valore tariffa di fatturazione predefinita](#default-billing-rate-value)
* [Valore tariffa di fatturazione della società](#company-billing-rate-value)
* [Più valori di tariffa di fatturazione e intervalli di tempo](#multiple-billing-rate-values-and-timeframes)

### Raggruppamento mansioni {#job-role-grouping}

Le tariffe di fatturazione sono raggruppate in **Tariffe di fatturazione** in base alle rispettive mansioni. <span class="preview">Se al progetto è allegata una scheda delle tariffe, anche le mansioni sono raggruppate per scheda delle tariffe. Se le posizioni vengono applicate ai ruoli, il nome della posizione viene incluso nel nome del ruolo. Lo stesso ruolo potrebbe essere elencato per più posizioni.</span>

### Valore tariffa di fatturazione progetto {#project-billing-rate-value}

Nella riga di raggruppamento corrispondente a una mansione, nota la tariffa di fatturazione per tale mansione a livello di progetto in **Tariffa di fatturazione del progetto** colonna. Se la mansione dispone di più tassi di sostituzione, il tasso di sostituzione corrispondente alla data corrente viene visualizzato nella riga di raggruppamento in **Tariffa di fatturazione del progetto** colonna.

### Valore tariffa di fatturazione predefinita {#default-billing-rate-value}

Nella riga di raggruppamento di una mansione, nota la tariffa di fatturazione per tale mansione a livello di sistema in **Tariffa di fatturazione predefinita** colonna.

>[!NOTE]
>
>Se sono presenti tariffe di fatturazione del progetto per una mansione, il **Tariffa di fatturazione predefinita** non viene mai applicato al calcolo dei ricavi per il progetto. Solo il **Tariffe di fatturazione del progetto** vengono applicati per calcolare i ricavi.

### Valore tariffa di fatturazione della società {#company-billing-rate-value}

Nella riga di raggruppamento di una mansione, nota la tariffa di fatturazione per tale mansione a livello di società in **Tariffa di fatturazione della società** colonna. Ciò significa che esiste un’azienda associata a questo progetto e che questa mansione ha una tariffa di fatturazione diversa per tale azienda. Viene visualizzata la tariffa di fatturazione per l’azienda, anche se è uguale alla tariffa del progetto.

>[!NOTE]
>
><span class="preview">Quando al progetto è allegata una scheda delle tariffe, il **Tariffe di fatturazione della società** non vengono importati nelle tariffe di fatturazione. I calcoli si basano sulle tariffe delle schede delle tariffe o sulle tariffe aziendali per le mansioni.</span>
>
>Se sono presenti tariffe di fatturazione del progetto per una mansione, il **Tariffa di fatturazione della società** non viene mai applicato al calcolo dei ricavi per il progetto. Solo il **Tariffe di fatturazione del progetto** vengono applicati per calcolare i ricavi.

### Più valori di tariffa di fatturazione e intervalli di tempo {#multiple-billing-rate-values-and-timeframes}

Se si dispone di più tariffe di fatturazione sostitutive per una mansione specifica, queste vengono elencate nel raggruppamento per tale mansione. Utilizzando la modifica in linea, puoi modificare le percentuali di sostituzione e il **Inizio** **Data** e **Data di fine** delle tariffe di fatturazione sostituite in questa scheda.

>[!NOTE]
>
>Impossibile specificare un **Data di inizio** per il primo tasso di sostituzione e non è possibile specificare un **Data di fine** per la percentuale di sostituzione più recente. Workfront presuppone che la prima tariffa di sostituzione venga applicata a tutte le ore con una data precedente alla **Data di fine** della prima sostituzione e che l’ultima tariffa di sostituzione venga applicata a tutte le ore con una data più recente della **Data di inizio** dell’ultima sostituzione.\
>Se viene registrata un’ora prima della data di inizio pianificata del progetto, viene utilizzata la prima tariffa di fatturazione.\
>Se viene registrata un’ora dopo la data di completamento pianificata del progetto, viene utilizzata l’ultima tariffa di fatturazione.

## Calcola retribuzione pianificata

* [Calcola il reddito pianificato in base alla sostituzione una tantum della tariffa di fatturazione](#calculate-planned-revenue-based-on-a-one-time-billing-rate-override)
* [Calcola il reddito pianificato in base a più sostituzioni della tariffa di fatturazione](#calculate-planned-revenue-based-on-multiple-billing-rate-overrides)
* [Distribuzione delle ore pianificate per la durata di un&#39;attività](#distribution-of-planned-hours-across-the-duration-of-a-task)

### Calcola il reddito pianificato in base alla sostituzione una tantum della tariffa di fatturazione {#calculate-planned-revenue-based-on-a-one-time-billing-rate-override}

Quando si calcola la retribuzione pianificata in base a una sostituzione della tariffa di fatturazione una tantum, tenere presente quanto segue:

* Quando **Tipo di retribuzione** di un’attività è **Ore Ruolo**, Workfront moltiplica le Ore pianificate di un&#39;attività per la tariffa di fatturazione della mansione associata all&#39;attività per calcolare la Retribuzione pianificata sull&#39;attività.

* Quando la tariffa di fatturazione della mansione è stata sostituita a livello di progetto, Workfront utilizza la tariffa di sostituzione del progetto per calcolare la Retribuzione pianificata.
* Quando un&#39;attività ha più assegnazioni, la Retribuzione pianificata viene calcolata moltiplicando la tariffa di fatturazione della mansione di ciascuna assegnazione e la rispettiva allocazione delle Ore pianificate.

>[!NOTE]
>
>Le ore pianificate per assegnazione non corrispondono alle ore pianificate per l&#39;attività, nel caso di più assegnazioni.

Per ulteriori informazioni sulla mansione utilizzata per calcolare i ricavi pianificati, vedere la sezione &quot;Informazioni sui calcoli dei ricavi per le attività in base alle assegnazioni di utenti e ruoli&quot; nell&#39;articolo [Panoramica su fatturazione e ricavi](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

### Calcola il reddito pianificato in base a più sostituzioni della tariffa di fatturazione {#calculate-planned-revenue-based-on-multiple-billing-rate-overrides}

Quando si calcola la retribuzione pianificata in base a più sostituzioni della tariffa di fatturazione, tenere presente quanto segue:

* Quando **Tipo di retribuzione** di un’attività è **Ore Ruolo**, Workfront moltiplica le Ore pianificate di un&#39;attività per la tariffa di fatturazione della mansione associata all&#39;attività per calcolare la Retribuzione pianificata sull&#39;attività.

  Per ulteriori informazioni sulla mansione utilizzata per calcolare i ricavi pianificati, vedere la sezione &quot;Informazioni sui calcoli dei ricavi per le attività in base alle assegnazioni di utenti e ruoli&quot; nell&#39;articolo [Panoramica su fatturazione e ricavi](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

* In caso di sostituzioni di più tariffe di fatturazione, la tariffa in base alla quale vengono moltiplicate le ore pianificate cambia durante un&#39;attività. Per impostazione predefinita, Workfront distribuisce le ore pianificate in modo uniforme per tutta la durata di un&#39;attività, allocando un numero uguale di ore per ogni giorno dell&#39;attività. Durante il calcolo **Reddito Pianificato** per un&#39;attività, Workfront moltiplica l&#39;Ora pianificata al giorno per la tariffa di fatturazione di quel giorno. In caso di tariffe di fatturazione multiple, quella tariffa potrebbe essere diversa ogni giorno.

  Ad esempio, un&#39;attività ha un&#39;Ora Ruolo **Tipo di retribuzione**. L&#39;attività ha una durata di 5 giorni e un valore di Lavoro Necessario di 40 ore. Le ore pianificate al giorno sono di 8 ore. Assegnare un ruolo di Project Manager all&#39;attività e sostituire la tariffa di fatturazione di questa mansione per gli ultimi 3 giorni dell&#39;attività, in modo da avere una tariffa di fatturazione Tasso 1 per i primi due giorni e una tariffa di fatturazione Tasso 2 per i restanti 3 giorni dell&#39;attività per questa mansione.

  La formula che calcola **Reddito Pianificato** di questa attività è:

  ```
  Planned Revenue = (Rate 1) * (Planned Hours for Day 1) + (Rate 1) * (Planned hours for Day 2) + (Rate 2) * (Planned hours for Day 3) + (Rate 2) * (Planned hours for Day 4) + (Rate 2) * (Planned hours for Day 5)
  ```

Per ulteriori informazioni su come trovare l’importo delle ore pianificate al giorno in Workfront, consulta la sezione [Distribuzione delle ore pianificate per la durata di un&#39;attività](#distribution-of-planned-hours-across-the-duration-of-a-task) in questo articolo.

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

* [Calcola il reddito effettivo in base alla sostituzione della tariffa di fatturazione una tantum](#calculate-actual-revenue-based-on-a-one-time-billing-rate-override)
* [Calcola il reddito effettivo in base a più sostituzioni della tariffa di fatturazione](#calculate-actual-revenue-based-on-multiple-billing-rate-overrides)

### Calcola il reddito effettivo in base alla sostituzione della tariffa di fatturazione una tantum {#calculate-actual-revenue-based-on-a-one-time-billing-rate-override}

Quando si calcola il reddito effettivo in base a una sostituzione della tariffa di fatturazione una tantum, tenere presente quanto segue:

* Quando **Tipo di retribuzione** di un’attività è **Ore Ruolo**, Workfront moltiplica il **Ore effettive** di un&#39;attività in base alla tariffa di fatturazione della mansione associata all&#39;attività da calcolare **Reddito Reale** sull&#39;attività. Le ore effettive sono ore registrate direttamente nell&#39;attività.

  Per ulteriori informazioni sulla mansione utilizzata per calcolare **Reddito Reale**, vedere la sezione &quot;Informazioni sul calcolo dei ricavi per le attività in base alle assegnazioni di utenti e ruoli&quot; nell&#39;articolo [Panoramica su fatturazione e ricavi](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

* Se la tariffa di fatturazione della mansione è stata sostituita a livello di progetto, Workfront utilizza la tariffa di sostituzione del progetto per calcolare la Retribuzione effettiva. Quando si sostituisce la tariffa di fatturazione della mansione nel progetto, il **Reddito Reale** del progetto viene ricalcolato automaticamente utilizzando il nuovo tasso adeguato.

  Per informazioni sulla sostituzione delle percentuali di ruolo per il progetto, consulta [Sostituisci tariffe di fatturazione mansione a livello di progetto](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

>[!NOTE]
>
>Se vuoi mantenere le ore che hai già effettuato l&#39;accesso al progetto prima di sovrascrivere la tariffa di fatturazione originale fatturata alla tariffa originale, devi includerle in una **Fatturazione**, e devi contrassegnare **Fatturazione** as **Fatturato**. In caso contrario, **Reddito Reale** dalle ore registrate prima della sostituzione della tariffa di fatturazione per il progetto verrà ricalcolato utilizzando la nuova tariffa quando vengono ricalcolati i dati finanziari dei progetti.\
>Per ulteriori informazioni sull’inclusione delle ore in un record di fatturazione e sulla relativa contrassegnazione come **Fatturato**, vedi l’articolo [Crea record fatturazione](../../../manage-work/projects/project-finances/create-billing-records.md).

### Calcola il reddito effettivo in base a più sostituzioni della tariffa di fatturazione {#calculate-actual-revenue-based-on-multiple-billing-rate-overrides}

Quando si calcola il reddito effettivo in base a più sostituzioni della tariffa di fatturazione, tenere presente quanto segue:

* Quando **Tipo di retribuzione** di un’attività è **Ore Ruolo**, Workfront moltiplica il **Ore effettive** sull&#39;attività con la tariffa di fatturazione delle mansioni assegnate all&#39;attività da calcolare **Reddito Reale** sull&#39;attività. Le ore effettive sono ore registrate direttamente nell&#39;attività.

* In caso di sostituzioni di più tariffe di fatturazione, la tariffa di cui **Ore effettive** vengono moltiplicati per calcolare **Reddito Reale** potrebbe cambiare durante la durata di un&#39;attività. Workfront utilizza la tariffa di fatturazione della mansione il cui intervallo di tempo corrisponde a **Data immissione** delle ore registrate per l&#39;attività da calcolare **Reddito Reale.**

  Ad esempio, un’attività presenta **Tipo di retribuzione** di **Ore Ruolo** e viene assegnato al ruolo di Project Manager. Sostituisci la tariffa di fatturazione di questa mansione con la tariffa 1 per le date tra il 19 giugno e il 25 giugno. A partire dal 26 giugno, sostituisci la tariffa di fatturazione con la Tariffa 2. Registrare 2 ore per il 20 giugno e 3 ore per il 28 giugno.

  Workfront calcola **Reddito Reale** per questa attività utilizzando la formula seguente:

  ```
  Actual Revenue = 2 * Rate 1 + 3 * Rate 2
  ```

  Per ulteriori informazioni sulla mansione utilizzata per calcolare **Reddito Reale**, vedere la sezione &quot;Informazioni sul calcolo dei ricavi per le attività in base alle assegnazioni di utenti e ruoli&quot; nell&#39;articolo [Panoramica su fatturazione e ricavi](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## L’impatto dei fusi orari nel calcolo dei ricavi in base a più tariffe di fatturazione

Gli utenti possono visualizzare ore pianificate al giorno diverse dagli altri utenti, se si verificano differenze di fuso orario tra loro e altre entità in Workfront. I seguenti scenari possono distorcere le informazioni sulle ore pianificate al giorno per un utente rispetto a quelle visualizzate da un altro utente:

* I computer dei due utenti potrebbero essere impostati per due fusi orari diversi
* I due profili utente in Workfront potrebbero essere impostati su due fusi orari diversi
* Il fuso orario associato al profilo utente potrebbe essere diverso da quello di Workfront
* Il fuso orario associato al profilo utente potrebbe essere diverso da quello della pianificazione del progetto.

In questi casi, il numero di ore pianificate al giorno potrebbe essere diverso tra due utenti che non condividono le stesse impostazioni per i fusi orari. Visualizzeranno anche numeri di Ricavi pianificati diversi quando si utilizzano sostituzioni di tariffe di fatturazione multiple su un progetto.

* [Calcola il reddito pianificato per gli utenti in diversi fusi orari](#calculate-planned-revenue-for-users-in-different-time-zones)
* [Calcola la retribuzione effettiva per gli utenti con fusi orari diversi](#calculate-actual-revenue-for-users-in-different-time-zones)

### Calcola il reddito pianificato per gli utenti in diversi fusi orari {#calculate-planned-revenue-for-users-in-different-time-zones}

>[!NOTE]
>
>Se utenti con fusi orari diversi lavorano sugli stessi progetti, ti consigliamo di non modificare le sostituzioni delle tariffe di fatturazione per i progetti durante la settimana. In questo modo potrebbe essere visualizzata una quantità errata di Reddito Pianificato per il progetto, a causa delle differenze di ore tra i fusi orari nella pianificazione degli utenti e il fuso orario del sistema Workfront. La maggior parte delle pianificazioni consente di escludere i fine settimana dai calcoli delle ore pianificate. Se si verifica una modifica nella sostituzione della tariffa di fatturazione di una mansione, è meglio che questa si verifichi durante un fine settimana piuttosto che a metà settimana, quando potrebbe coincidere con la metà della durata di un&#39;attività.

Quando calcoli la Retribuzione Pianificata per utenti con fusi orari diversi, considera quanto segue:

* Per le attività con **Tipo di retribuzione** di **Ore Ruolo** e sono assegnati a mansioni, **Reddito Pianificato** viene calcolato moltiplicando il valore **Ore pianificate** di un&#39;attività in base alla tariffa di fatturazione della mansione.

* Il **Ore pianificate** sono distribuiti in modo uniforme in **Durata** dell&#39;attività.

* Il **Durata** è il periodo di tempo tra **Inizio pianificato** **Data** e **Data di completamento Pianificata** dell&#39;attività. Perché il **Data Inizio Pianificata** e **Data di completamento Pianificata** Le attività possono variare a seconda del fuso orario degli utenti che visualizzano l&#39;attività, la quantità di ore pianificate al giorno può essere diversa per due utenti in due fusi orari diversi.

* La quantità di ore pianificate al giorno non modifica la retribuzione pianificata di un progetto se la tariffa di fatturazione della mansione non viene modificata o se è presente una sola sostituzione della tariffa di fatturazione. In questo caso, anche se due utenti di due fusi orari diversi visualizzano ore pianificate al giorno diverse, il ricavo pianificato complessivo del progetto è identico tra i due utenti.

  Tuttavia, in caso di sostituzioni di più tariffe di fatturazione, il valore complessivo **Reddito Pianificato** del progetto potrebbe sembrare diverso per due utenti in due fusi orari diversi, perché si basa sulla quantità di ore pianificate al giorno (che potrebbe essere diversa per i due utenti) e sulla sostituzione della tariffa di fatturazione (che potrebbe essere diversa per lo stesso giorno, quando ogni utente osserva l’attività nel proprio fuso orario).

* L&#39;accurato **Reddito Pianificato** La quantità è quella visualizzata dall’utente che ha lo stesso fuso orario del fuso orario dell’istanza di Workfront. L&#39;amministratore di Workfront definisce il fuso orario di Workfront nell&#39;area Informazioni cliente di sistema.\
  Per ulteriori informazioni sulla definizione del fuso orario del sistema, vedere l&#39;articolo [Configurare le informazioni di base per il sistema](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

### Calcola la retribuzione effettiva per gli utenti con fusi orari diversi {#calculate-actual-revenue-for-users-in-different-time-zones}

Nel calcolare la retribuzione effettiva per utenti con fusi orari diversi, considera quanto segue:

* Quando **Tipo di retribuzione** di un’attività è **Ore Ruolo**, Workfront moltiplica il **Ore effettive** sull&#39;attività con la tariffa di fatturazione delle mansioni assegnate all&#39;attività per calcolare **Reddito Reale**. Le ore effettive sono ore registrate direttamente nell&#39;attività.

* In caso di sostituzioni di più tariffe di fatturazione, Workfront utilizza la tariffa di fatturazione della mansione il cui intervallo di tempo corrisponde a **Data immissione** delle ore registrate per l&#39;attività da calcolare **Reddito Reale**.

* Perché non è presente alcuna marca temporale sul **Data immissione** delle ore registrate e non esiste una marca temporale sugli intervalli di date delle sostituzioni di più tariffe di fatturazione, **Reddito Reale** I calcoli non sono influenzati dal fuso orario associato agli utenti.

Per ulteriori informazioni sulla mansione utilizzata per calcolare **Reddito Reale**, vedere la sezione &quot;Informazioni sul calcolo dei ricavi per le attività in base alle assegnazioni di utenti e ruoli&quot; nell&#39;articolo [Panoramica su fatturazione e ricavi](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## Ricalcola dati finanziari progetto

I dati finanziari vengono calcolati su un progetto in base alle modifiche apportate nelle ore registrate per il progetto.

Se i tassi vengono modificati durante il ciclo di vita di un progetto, è possibile ricalcolare manualmente i costi e i ricavi del progetto utilizzando l&#39;opzione Ricalcola contabilità su un progetto. Inoltre, alcune azioni attivano un ricalcolo automatico.

Per ulteriori informazioni sul ricalcolo dei dati finanziari del progetto, vedere l&#39;articolo [Ricalcolare i dati finanziari del progetto](../../../manage-work/projects/project-finances/recalculate-project-finances.md).

## Aggiungere una nuova tariffa di fatturazione utilizzando l’API

Per aggiungere una nuova tariffa di fatturazione per una mansione utilizzando l’API, esegui una *setRatesForRole* azione per **Tariffa** oggetto utilizzando *metodo PUT*.
L’azione e i campi data nella **Tariffa** sono disponibili nella versione API 8.0. Se hai già definito diverse tariffe di fatturazione per una mansione in un progetto e desideri aggiungerne una nuova con un nuovo intervallo di date, devi includere sia la tariffa esistente che quella da aggiungere nella stessa chiamata API. È simile a come si aggiornano le raccolte sugli oggetti.

La seguente chiamata API è un esempio in cui **attachableID** è il **ID Progetto** del progetto in cui si sta aggiungendo la tariffa e **RoleID** è il **ID Ruolo** per il quale si sta aggiungendo la nuova tariffa di fatturazione.<pre>{</pre><pre>&quot;attachableID&quot;:&quot;593f01500000557d75fdd4fdfcc624f2&quot;,</pre><pre>&quot;attachableObjCode&quot;:&quot;PROJ&quot;,</pre><pre>&quot;roleID&quot;:&quot;544820df000014148cda5136d4b79d09&quot;, </pre><pre>&quot;tariffe&quot;:[</pre><pre>         {&quot;rateValue&quot;:&quot;0.00&quot;,&quot;startDate&quot;:null,&quot;endDate&quot;:&quot;2017-06-11&quot;},</pre><pre>         {&quot;rateValue&quot;:&quot;45.00&quot;,&quot;startDate&quot;:&quot;2017-06-12&quot;,&quot;endDate&quot;:&quot;2017-06-17&quot;},</pre><pre>         {&quot;rateValue&quot;:&quot;95.00&quot;,&quot;startDate&quot;:&quot;2017-06-21&quot;,&quot;endDate&quot;:null}</pre><pre>]</pre><pre>}</pre>Per ulteriori informazioni sull’utilizzo dell’API di Workfront, consulta l’articolo [Nozioni di base sulle API](https://experience.workfront.com/s/article/API-Basics-638808549).
