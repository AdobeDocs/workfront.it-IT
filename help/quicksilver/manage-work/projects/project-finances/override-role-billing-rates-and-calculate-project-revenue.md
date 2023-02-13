---
product-area: projects
navigation-topic: financials
title: Panoramica sulla priorità dei tassi di fatturazione dei ruoli di lavoro e sul calcolo dei ricavi per un progetto
description: Puoi utilizzare i tassi di fatturazione per calcolare i ricavi dei progetti quando li moltiplichi per le ore trascorse sul progetto. Per ulteriori informazioni su tassi di fatturazione e ricavi, consulta l’articolo Panoramica di fatturazione e ricavi.
author: Alina
feature: Work Management
exl-id: 63ba6758-ba62-48b4-89f4-d784e32a1bfa
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '3644'
ht-degree: 0%

---

# Panoramica sulla priorità dei tassi di fatturazione dei ruoli di lavoro e sul calcolo dei ricavi per un progetto

Puoi utilizzare i tassi di fatturazione per calcolare i ricavi dei progetti quando li moltiplichi per le ore trascorse sul progetto. Per ulteriori informazioni su tariffe e ricavi di fatturazione, consulta l’articolo [Panoramica di fatturazione e ricavi](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

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

## Panoramica dei tassi di fatturazione del ruolo del lavoro e dei tipi di ricavi orari del ruolo

In qualità di amministratore di Adobe Workfront, puoi associare le tariffe di fatturazione sia con gli utenti che con i ruoli di lavoro.\
Per ulteriori informazioni sulla creazione di utenti e sull&#39;associazione di utenti con le tariffe di fatturazione, consulta l&#39;articolo [Aggiungi utenti](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md). Per ulteriori informazioni sulla creazione di ruoli di lavoro e sull&#39;associazione di questi con i tassi di fatturazione, consulta l&#39;articolo [Creare e gestire ruoli di lavoro](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

Le tariffe di fatturazione associate agli utenti non possono essere ignorate.

I tassi di fatturazione associati ai ruoli di lavoro possono essere ignorati a livello di azienda o di progetto.

Per calcolare i ricavi sui progetti in base ai tassi di fatturazione dei ruoli del lavoro, la **Tipo di ricavo** dei compiti relativi ai progetti deve essere uno dei seguenti:

* Ore Ruolo
* Ore Ruolo w/Cap
* Ruolo orario più fisso

Per ulteriori informazioni **Tipo di ricavo** e le tariffe di fatturazione, vedi [Panoramica di fatturazione e ricavi](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## Gerarchia delle sostituzioni del tasso di fatturazione durante il calcolo dei ricavi

A un ruolo di lavoro può essere associato un tasso di fatturazione nei seguenti modi:

* In qualità di amministratore di Workfront, è possibile definire il tasso di fatturazione a livello di sistema associato a un ruolo di lavoro durante la creazione del ruolo di lavoro.\
   Per ulteriori informazioni sulla creazione dei ruoli di lavoro, consulta [Creare e gestire ruoli di lavoro](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* In qualità di amministratore di Workfront, puoi definire il tasso di fatturazione a livello aziendale per lo stesso ruolo di lavoro quando crei una società.\
   Quando Workfront calcola i ricavi per i progetti associati a questa società, il tasso di fatturazione della società viene utilizzato quando il ruolo viene assegnato alle attività, anziché il tasso di fatturazione a livello di sistema per questo ruolo di lavoro.\
   I tassi di ruolo modificati a livello aziendale avranno un impatto su tutti i progetti associati a tale azienda.

   >[!NOTE]
   >
   >Se devi aggiornare il tasso di fatturazione dell&#39;azienda, il tasso del progetto non verrà aggiornato automaticamente. È necessario rimuovere l&#39;Azienda dal progetto, aggiornare il tasso per l&#39;Azienda, quindi ricollegare l&#39;Azienda al progetto, prima che il tasso della nuova Azienda abbia effetto sul progetto. Per istruzioni su come collegare un&#39;Azienda a un progetto, vedi [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md).

   Per ulteriori informazioni sulla creazione di tassi di fatturazione dei ruoli di lavoro specifici per un&#39;azienda, consulta [Creare e modificare aziende](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

* In qualità di amministratore di Workfront, puoi abilitare un’opzione quando modifichi un progetto per applicare al progetto modifiche ai tassi di fatturazione a livello aziendale quando gli utenti ricalcolano manualmente le finanze del progetto.\
   Per ulteriori informazioni, consulta [Sostituisci i tassi di fatturazione a livello di progetto con i tassi di fatturazione a livello di società](../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md).

* In qualità di project manager, puoi definire il tasso di fatturazione per lo stesso ruolo di processo a livello di progetto.\
   Le percentuali di ruolo modificate nel progetto avranno un impatto solo sul progetto.

   Per informazioni sull’override delle percentuali di ruolo per il progetto, consulta [Ignora tassi di fatturazione ruolo lavoro a livello di progetto](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

>[!IMPORTANT]
>
>Se un ruolo di lavoro è associato a un tasso di fatturazione a livello di sistema, a livello di azienda e a livello di progetto, Workfront calcola i ricavi delle attività utilizzando il tasso di fatturazione del ruolo di lavoro a livello di progetto, quando utilizza i tassi di ruolo del lavoro. I ricavi di tutte le attività si estendono ai ricavi del progetto.

## Ignora tassi di fatturazione ruolo lavoro a livello di progetto

In qualità di project manager, puoi specificare il tasso di fatturazione per un ruolo di lavoro in un progetto specifico. Questo tasso di fatturazione a livello di progetto sostituisce il tasso di fatturazione a livello di sistema per questo ruolo di lavoro. Workfront utilizza il tasso di fatturazione a livello di progetto del ruolo di processo per calcolare i ricavi, invece di utilizzare il tasso di fatturazione a livello di sistema.

Per informazioni su come ignorare i tassi di fatturazione del ruolo di lavoro a livello di progetto, vedere [Ignora tassi di fatturazione ruolo lavoro a livello di progetto](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

Per ulteriori informazioni sul ruolo di lavoro utilizzato per calcolare i ricavi del progetto, vedere la sezione &quot;Calcoli dei ricavi per le attività basate sulle assegnazioni utente e ruolo&quot; in [Panoramica di fatturazione e ricavi](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

>[!NOTE]
>
>Nel caso dei ricavi effettivi, i tassi di fatturazione applicati alle ore aggiunte a un record di fatturazione contrassegnato come Fatturato non devono essere influenzati dalle sostituzioni dei tassi di fatturazione che si verificano dopo la fatturazione del record di fatturazione.

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

## Panoramica della sezione Tassi di fatturazione di un progetto

Dopo aver specificato i tassi di fatturazione di sostituzione per i ruoli di lavoro associati al progetto, è possibile visualizzare tutti i ruoli di lavoro e le relative sostituzioni nel **Tassi di fatturazione** scheda del progetto.

Osserva le seguenti informazioni nell’elenco di **Tassi di fatturazione**:

* [Raggruppamento ruoli processo](#job-role-grouping)
* [Valore del tasso di fatturazione del progetto](#project-billing-rate-value)
* [Valore del tasso di fatturazione predefinito](#default-billing-rate-value)
* [Valore del tasso di fatturazione della società](#company-billing-rate-value)
* [Valori e tempi di fatturazione multipli](#multiple-billing-rate-values-and-timeframes)

### Raggruppamento ruoli processo {#job-role-grouping}

Le tariffe di fatturazione sono raggruppate in **Tassi di fatturazione** in base ai rispettivi ruoli.

### Valore del tasso di fatturazione del progetto {#project-billing-rate-value}

Nella riga di raggruppamento corrispondente a un ruolo di lavoro, nota il tasso di fatturazione per quel ruolo di lavoro a livello di progetto nella **Tasso di fatturazione del progetto** colonna. Se il ruolo del lavoro dispone di più tassi di sostituzione, il tasso di sostituzione corrispondente alla data corrente viene visualizzato nella riga di raggruppamento nel **Tasso di fatturazione del progetto** colonna.

### Valore del tasso di fatturazione predefinito {#default-billing-rate-value}

Nella riga di raggruppamento di un ruolo di lavoro, nota il tasso di fatturazione per quel ruolo di lavoro a livello di sistema nel **Tasso di fatturazione predefinito** colonna.

>[!NOTE]
>
>Se esistono tassi di fatturazione del progetto per un ruolo di lavoro, la **Tasso di fatturazione predefinito** non viene mai applicato al calcolo dei ricavi per il progetto. Solo il **Tassi di fatturazione del progetto** vengono applicati per calcolare i ricavi.

### Valore del tasso di fatturazione della società {#company-billing-rate-value}

Nella riga di raggruppamento di un ruolo di lavoro, nota il tasso di fatturazione per quel ruolo di lavoro a livello di società nel **Tasso di fatturazione della società** colonna. Ciò significa che esiste un&#39;azienda associata a questo progetto e che questo ruolo di lavoro ha un tasso di fatturazione diverso per l&#39;azienda. Viene visualizzato il tasso di fatturazione per l&#39;azienda, anche se è lo stesso del tasso di progetto.

>[!NOTE]
>
>Se esistono tassi di fatturazione del progetto per un ruolo di lavoro, la **Tasso di fatturazione della società** non viene mai applicato al calcolo dei ricavi per il progetto. Solo il **Tassi di fatturazione del progetto** vengono applicati per calcolare i ricavi.

### Valori e tempi di fatturazione multipli {#multiple-billing-rate-values-and-timeframes}

Se si dispone di più tassi di fatturazione di sostituzione per un ruolo di lavoro specifico, questi vengono elencati nel raggruppamento per quel ruolo di lavoro. Utilizzando la modifica in linea, puoi modificare le percentuali di sostituzione e il **Inizio** **Data** e **Data di fine** dei tassi di fatturazione di sostituzione in questa scheda.

>[!NOTE]
>
>Non è possibile specificare un **Data di inizio** per il primo tasso di sostituzione e non è possibile specificare un **Data di fine** per l&#39;ultimo tasso di sostituzione. Workfront presuppone che il primo tasso di sostituzione sia applicato per tutte le ore con una data precedente alla **Data di fine** del primo override e che l&#39;ultimo tasso di sostituzione è applicato per tutte le ore con una data successiva a quella **Data di inizio** dell&#39;ultima sostituzione.\
>Se viene registrata un&#39;ora prima della data di inizio pianificata del progetto, viene utilizzato il primo tasso di fatturazione.\
>Se dopo la data di completamento pianificata del progetto viene registrata un’ora, viene utilizzato l’ultimo tasso di fatturazione.

## Calcola ricavi pianificati

* [Calcola i ricavi pianificati in base a una sostituzione del tasso di fatturazione una tantum](#calculate-planned-revenue-based-on-a-one-time-billing-rate-override)
* [Calcola i ricavi pianificati in base a più sostituzioni del tasso di fatturazione](#calculate-planned-revenue-based-on-multiple-billing-rate-overrides)
* [Distribuzione di ore pianificate per tutta la durata di un&#39;attività](#distribution-of-planned-hours-across-the-duration-of-a-task)

### Calcola i ricavi pianificati in base a una sostituzione del tasso di fatturazione una tantum {#calculate-planned-revenue-based-on-a-one-time-billing-rate-override}

Quando si calcolano i ricavi pianificati in base a una sostituzione del tasso di fatturazione una tantum, tenere presente quanto segue:

* Quando il **Tipo di ricavo** di un&#39;attività **Ruolo orario**, Workfront moltiplica l&#39;orario pianificato di un&#39;attività per il tasso di fatturazione del ruolo del lavoro associato all&#39;attività per calcolare i ricavi pianificati sull&#39;attività.

* Quando il tasso di fatturazione del ruolo di lavoro viene ignorato a livello di progetto, Workfront utilizza il tasso di sostituzione del progetto per calcolare i ricavi pianificati.
* Quando un&#39;attività dispone di più assegnazioni, i Ricavi pianificati vengono calcolati moltiplicando il tasso di fatturazione del ruolo di lavoro di ogni assegnazione e la rispettiva allocazione oraria pianificata.

>[!NOTE]
>
>Le ore pianificate per assegnazione non sono uguali alle ore pianificate per l&#39;attività, nel caso di più assegnazioni.

Per ulteriori informazioni sul ruolo del lavoro utilizzato per calcolare i ricavi pianificati, consulta la sezione &quot;Informazioni sui calcoli dei ricavi per le attività in base alle assegnazioni di utenti e ruoli&quot; nell’articolo [Panoramica di fatturazione e ricavi](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

### Calcola i ricavi pianificati in base a più sostituzioni del tasso di fatturazione {#calculate-planned-revenue-based-on-multiple-billing-rate-overrides}

Quando si calcolano i ricavi pianificati in base a più sostituzioni del tasso di fatturazione, tenere presente quanto segue:

* Quando il **Tipo di ricavo** di un&#39;attività **Ruolo orario**, Workfront moltiplica l&#39;orario pianificato di un&#39;attività per il tasso di fatturazione del ruolo del lavoro associato all&#39;attività per calcolare i ricavi pianificati sull&#39;attività.

   Per ulteriori informazioni sul ruolo del lavoro utilizzato per calcolare i ricavi pianificati, consulta la sezione &quot;Informazioni sui calcoli dei ricavi per le attività in base alle assegnazioni di utenti e ruoli&quot; nell’articolo [Panoramica di fatturazione e ricavi](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

* In caso di sostituzioni del tasso di fatturazione multiple, il tasso di moltiplicazione delle ore pianificate cambia durante la durata di un&#39;attività. Per impostazione predefinita, Workfront distribuisce le ore pianificate in modo uniforme per tutta la durata di un&#39;attività, allocando un numero uguale di ore per ogni giorno dell&#39;attività. Nel calcolo **Ricavi pianificati** per un’attività, Workfront moltiplica l’ora pianificata per giorno per il tasso di fatturazione di quel giorno. In caso di tariffe di fatturazione multiple, tale tasso potrebbe essere diverso ogni giorno.

   Ad esempio, per un’attività con un ruolo orario **Tipo di ricavo**. L’attività ha una durata di 5 giorni e un valore di Ora pianificata di 40 ore. L&#39;orario pianificato è di 8 ore al giorno. Assegnare un ruolo di lavoro di Project Manager all&#39;attività e sostituire il tasso di fatturazione di questo ruolo di processo per gli ultimi 3 giorni dell&#39;attività, in modo da avere un tasso di fatturazione 1 per i primi due giorni e tasso di fatturazione 2 per i restanti 3 giorni dell&#39;attività per questo ruolo di lavoro.

   La formula che calcola il **Ricavi pianificati** di questo compito:

   ```
   Planned Revenue = (Rate 1) * (Planned Hours for Day 1) + (Rate 1) * (Planned hours for Day 2) + (Rate 2) * (Planned hours for Day 3) + (Rate 2) * (Planned hours for Day 4) + (Rate 2) * (Planned hours for Day 5)
   ```

Per ulteriori informazioni su come trovare l’importo in Orari pianificati per giorno in Workfront, consulta la sezione . [Distribuzione di ore pianificate per tutta la durata di un&#39;attività](#distribution-of-planned-hours-across-the-duration-of-a-task) in questo articolo.

>[!NOTE]
>
>Se si dispone di più assegnatari sull&#39;attività, la quantità di ore pianificate viene prima distribuita a ciascun assegnatario e poi a ogni giorno durante la durata dell&#39;attività. In questo caso, il Ricavo pianificato verrà calcolato tenendo conto della quantità di ore giornaliere per ciascun assegnatario e del tasso di fatturazione di ciascun ruolo di lavoro che potrebbe cambiare durante la durata dell&#39;attività, in caso di più tassi di fatturazione.

### Distribuzione di ore pianificate per tutta la durata di un&#39;attività {#distribution-of-planned-hours-across-the-duration-of-a-task}

Quando si comprende la distribuzione delle ore pianificate per tutta la durata di un&#39;attività, tenere presente quanto segue:

* Per impostazione predefinita, Workfront distribuisce le ore pianificate in modo uniforme per tutta la durata di un&#39;attività, allocando un numero uguale di ore pianificate per ogni giorno dell&#39;attività, in base alla disponibilità della pianificazione del progetto.

   Per ulteriori informazioni sulla distribuzione delle ore pianificate per tutta la durata di un&#39;attività, consulta la sezione &quot;Informazioni sulla distribuzione delle ore pianificate per tutta la durata di un&#39;attività&quot; nell&#39;articolo [Panoramica sull’orario pianificato](../../../manage-work/tasks/task-information/planned-hours.md).

   >[!NOTE]
   >
   >L&#39;orario pianificato per giorno è l&#39;allocazione di ore pianificate per ogni giorno durante la durata dell&#39;attività. Se l&#39;attività dispone di un&#39;assegnazione, questo numero rappresenta anche le ore pianificate per giorno per assegnazione. Se l&#39;attività dispone di più assegnazioni, l&#39;orario pianificato per giorno per assegnazione è diverso dall&#39;orario pianificato per giorno per l&#39;attività. In Workfront non è disponibile alcuna rappresentazione visiva per le ore pianificate per giorno per assegnazione, per le attività con più assegnazioni.
   >
   >
   >Le ore pianificate per giorno vengono moltiplicate per il tasso di fatturazione per il ruolo di processo assegnato all&#39;attività per quel giorno per calcolare le entrate pianificate per giorno per quell&#39;attività. Una somma di tutti i ricavi pianificati giornalieri calcolati in questo modo è uguale ai ricavi pianificati per l&#39;attività.

## Calcola ricavi effettivi

* [Calcola i ricavi effettivi in base a una sostituzione del tasso di fatturazione una tantum](#calculate-actual-revenue-based-on-a-one-time-billing-rate-override)
* [Calcola i ricavi effettivi in base a più sostituzioni del tasso di fatturazione](#calculate-actual-revenue-based-on-multiple-billing-rate-overrides)

### Calcola i ricavi effettivi in base a una sostituzione del tasso di fatturazione una tantum {#calculate-actual-revenue-based-on-a-one-time-billing-rate-override}

Quando si calcolano i ricavi effettivi in base a una sostituzione del tasso di fatturazione una tantum, tenere presente quanto segue:

* Quando il **Tipo di ricavo** di un&#39;attività **Ruolo orario**, Workfront moltiplica il **Ore effettive** di un&#39;attività in base al tasso di fatturazione del ruolo di lavoro associato all&#39;attività da calcolare **Entrate effettive** sull&#39;attività. Le ore effettive sono ore registrate direttamente nell&#39;attività.

   Per ulteriori informazioni sul ruolo di lavoro da calcolare **Entrate effettive**, consulta la sezione &quot;Informazioni sui calcoli dei ricavi per le attività in base alle assegnazioni di utenti e ruoli&quot; nell’articolo [Panoramica di fatturazione e ricavi](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

* Se il tasso di fatturazione del ruolo di lavoro è stato ignorato a livello di progetto, Workfront utilizza il tasso di sostituzione del progetto per calcolare i ricavi effettivi. Quando sovrascrivi il tasso di fatturazione del ruolo del lavoro nel progetto, la **Entrate effettive** del progetto viene ricalcolato automaticamente utilizzando il nuovo tasso adeguato.

   Per informazioni sull’override delle percentuali di ruolo per il progetto, consulta [Ignora tassi di fatturazione ruolo lavoro a livello di progetto](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

>[!NOTE]
>
>Se si desidera mantenere le ore che si sono già registrate sul progetto prima di sovrascrivere il tasso di fatturazione originale fatturato al tasso originale, è necessario includerle in un **Record di fatturazione**, e devi contrassegnare il **Record di fatturazione** come **Fatturato**. In caso contrario, la **Entrate effettive** dalle ore registrate prima dell&#39;override del tasso di fatturazione per il progetto, verrà ricalcolato utilizzando il nuovo tasso al momento del ricalcolo delle finanze dei progetti.\
>Per ulteriori informazioni sull&#39;inclusione delle ore in un record di fatturazione e sul relativo contrassegno **Fatturato**, vedi l&#39;articolo [Creazione di record di fatturazione](../../../manage-work/projects/project-finances/create-billing-records.md).

### Calcola i ricavi effettivi in base a più sostituzioni del tasso di fatturazione {#calculate-actual-revenue-based-on-multiple-billing-rate-overrides}

Quando si calcolano i ricavi effettivi in base a più sostituzioni del tasso di fatturazione, tenere presente quanto segue:

* Quando il **Tipo di ricavo** di un&#39;attività **Ruolo orario**, Workfront moltiplica il **Ore effettive** sull&#39;attività con il tasso di fatturazione dei ruoli job assegnati all&#39;attività da calcolare **Entrate effettive** sull&#39;attività. Le ore effettive sono ore registrate direttamente nell&#39;attività.

* In caso di sostituzioni di più tassi di fatturazione, il tasso di cui **Ore effettive** vengono moltiplicati per calcolare il **Entrate effettive** potrebbe cambiare durante la durata di un&#39;attività. Workfront utilizza il tasso di fatturazione del ruolo di lavoro il cui intervallo di tempo corrisponde al **Data di ingresso** delle ore registrate per il calcolo dell&#39;attività **Entrate effettive.**

   Ad esempio, un’attività ha **Tipo di ricavo** di **Ruolo orario** e viene assegnato al ruolo di Project Manager. Sostituisci il tasso di fatturazione di questo ruolo di lavoro con il tasso 1 per le date tra il 19 giugno e il 25 giugno. A partire dal 26 giugno, sovrascrivi il tasso di fatturazione con Tasso 2. Log 2 ore per il 20 giugno e 3 ore per il 28 giugno.

   Workfront calcola il **Entrate effettive** per questa attività utilizzando la seguente formula:

   ```
   Actual Revenue = 2 * Rate 1 + 3 * Rate 2
   ```

   Per ulteriori informazioni sul ruolo di lavoro da calcolare **Entrate effettive**, consulta la sezione &quot;Informazioni sui calcoli dei ricavi per le attività in base alle assegnazioni di utenti e ruoli&quot; nell’articolo [Panoramica di fatturazione e ricavi](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## L’impatto dei Fusi orari durante il calcolo dei ricavi in base a più tassi di fatturazione

Gli utenti possono visualizzare ore pianificate diverse per giorno rispetto ad altri utenti, se si verificano differenze di fuso orario tra loro e altre entità in Workfront. Gli scenari seguenti potrebbero distorcere le informazioni relative alle ore pianificate per giorno per un utente da ciò che un altro utente vede:

* I due utenti potrebbero avere i propri computer impostati per due diversi fusi orari
* I due profili utente in Workfront possono essere impostati su due fusi orari diversi
* Il fuso orario associato al profilo utente potrebbe essere diverso dal fuso orario del sistema in Workfront
* Il fuso orario associato al profilo utente potrebbe essere diverso da quello della pianificazione del progetto.

In questi casi, il numero di ore pianificate per giorno potrebbe essere diverso tra due utenti che non condividono le stesse impostazioni per i fusi orari. Visualizzeranno anche diversi numeri di Ricavo pianificato quando si utilizzano più sostituzioni del tasso di fatturazione su un progetto.

* [Calcola i ricavi pianificati per gli utenti in diversi Fusi orari](#calculate-planned-revenue-for-users-in-different-time-zones)
* [Calcolare i ricavi effettivi per gli utenti in diversi Fusi orari](#calculate-actual-revenue-for-users-in-different-time-zones)

### Calcola i ricavi pianificati per gli utenti in diversi Fusi orari {#calculate-planned-revenue-for-users-in-different-time-zones}

>[!NOTE]
>
>Se gli utenti di diversi fusi orari lavorano sugli stessi progetti, si consiglia di non modificare le sostituzioni dei tassi di fatturazione per i progetti durante la settimana. In questo modo è possibile visualizzare una quantità errata di Ricavi pianificati per il progetto, a causa delle differenze di ora tra i fusi orari nella pianificazione degli utenti e il fuso orario del sistema Workfront . La maggior parte delle pianificazioni consente di escludere i fine settimana dai calcoli dell&#39;orario pianificato. Se si verifica una modifica nella sostituzione del tasso di fatturazione di un ruolo di lavoro, è meglio che si verifichi durante un fine settimana che a metà settimana quando potrebbe coincidere con la metà della durata di un&#39;attività.

Quando si calcolano i ricavi pianificati per gli utenti in diversi Fusi orari, considera quanto segue:

* Per le attività che hanno un **Tipo di ricavo** di **Ruolo orario** e sono assegnati a ruoli di lavoro, **Ricavi pianificati** è calcolato moltiplicando il **Orari pianificati** di un&#39;attività in base al tasso di fatturazione del ruolo del lavoro.

* La **Orari pianificati** sono distribuiti in modo uniforme tra i **Durata** del compito.

* La **Durata** è il periodo di tempo tra **Inizio pianificato** **Data** e **Data completamento pianificata** del compito. Perché&#x200B;**Data di inizio prevista** e **Data completamento pianificata** delle attività possono variare a seconda dei fusi orari degli utenti che visualizzano l&#39;attività, la quantità di ore pianificate per giorno potrebbe essere diversa per due utenti in due fusi orari diversi.

* La quantità di ore pianificate per giorno non modifica i ricavi pianificati di un progetto se il tasso di fatturazione del ruolo di lavoro non viene modificato o se è presente una sola sostituzione del tasso di fatturazione. In questo caso, anche se due utenti con due diversi orari visualizzano ore pianificate diverse per giorno, il Ricavo pianificato complessivo del progetto è identico tra i due utenti.

   Tuttavia, nel caso di più sostituzioni dei tassi di fatturazione, il **Ricavi pianificati** del progetto potrebbe sembrare diverso per due utenti in due diversi orari, perché si basa sulla quantità di ore pianificate al giorno (che potrebbe essere diversa per i due utenti) e sull’override del tasso di fatturazione (che potrebbe essere diverso per lo stesso giorno, quando ogni utente sta guardando l’attività nel proprio fuso orario).

* La precisione **Ricavi pianificati** amount è quella visualizzata dall’utente che ha lo stesso fuso orario dell’istanza Workfront. L’amministratore di Workfront definisce il fuso orario Workfront nell’area Informazioni cliente di sistema.\
   Per ulteriori informazioni sulla definizione del fuso orario del sistema, consulta l’articolo [Configurare le informazioni di base per il sistema](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

### Calcolare i ricavi effettivi per gli utenti in diversi Fusi orari {#calculate-actual-revenue-for-users-in-different-time-zones}

Quando si calcolano i ricavi effettivi per gli utenti in diversi Fusi orari, considera quanto segue:

* Quando il **Tipo di ricavo** di un&#39;attività **Ruolo orario**, Workfront moltiplica il **Ore effettive** sull&#39;attività con il tasso di fatturazione dei ruoli del processo assegnati all&#39;attività per calcolare il **Entrate effettive**. Le ore effettive sono ore registrate direttamente nell&#39;attività.

* In caso di sostituzioni del tasso di fatturazione multiple, Workfront utilizza il tasso di fatturazione del ruolo di lavoro il cui intervallo di tempo corrisponde al **Data di ingresso** delle ore registrate per il calcolo dell&#39;attività **Entrate effettive**.

* Perché non c&#39;è una marca temporale nel **Data di ingresso** di ore registrate e non vi è timestamp sugli intervalli di date di più sostituzioni dei tassi di fatturazione, **Entrate effettive** i calcoli non sono influenzati dal fuso orario associato agli utenti.

Per ulteriori informazioni sul ruolo di lavoro da calcolare **Entrate effettive**, consulta la sezione &quot;Informazioni sui calcoli dei ricavi per le attività in base alle assegnazioni di utenti e ruoli&quot; nell’articolo [Panoramica di fatturazione e ricavi](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## Ricalcola finanziamenti progetto

I finanziamenti vengono calcolati su un progetto quando le modifiche si verificano nelle ore registrate per il progetto.

Se i tassi vengono modificati durante la durata di un progetto, è possibile ricalcolare manualmente i costi e i ricavi del progetto utilizzando l&#39;opzione Ricalcola finanziamenti su un progetto. Inoltre, alcune azioni attivano un ricalcolo automatico.

Per ulteriori informazioni sul ricalcolo delle finanze dei progetti, consulta l’articolo [Ricalcolare le finanze del progetto](../../../manage-work/projects/project-finances/recalculate-project-finances.md).

## Aggiungi un nuovo tasso di fatturazione utilizzando l’API

Per aggiungere un nuovo tasso di fatturazione per un ruolo di lavoro utilizzando l’API, esegui una *setRatesForRole* per **Rate** utilizzando *metodo PUT*.
L’azione e i campi data nella sezione **Rate** L&#39;oggetto è disponibile nella versione API 8.0. Se sono già stati definiti diversi tassi di fatturazione per un ruolo di lavoro in un progetto e si desidera aggiungere un nuovo tasso di fatturazione per esso con un nuovo intervallo di date, è necessario includere sia il tasso esistente sia il tasso da aggiungere nella stessa chiamata API. È simile alla modalità di aggiornamento delle raccolte sugli oggetti.

La seguente chiamata API è un esempio in cui **attachmentID** è **ID progetto** del progetto in cui si aggiunge il tasso e **RoleID** è **ID ruolo lavoro** per il quale stai aggiungendo il nuovo tasso di fatturazione.<pre>{</pre><pre>&quot;attachmentID&quot;:&quot;593f0150000557d75fdd4fdfcc624f2&quot;,</pre><pre>&quot;attachmentObjCode&quot;:&quot;PROJ&quot;,</pre><pre>&quot;roleID&quot;:&quot;544820df00014148cda5136d4b79d09&quot;, </pre><pre>&quot;tariffe&quot;:[</pre><pre>         {&quot;rateValue&quot;:&quot;0.0&quot;,&quot;startDate&quot;:null,&quot;endDate&quot;:&quot;2017-06-11&quot;},</pre><pre>         {&quot;rateValue&quot;:&quot;45.00&quot;,&quot;startDate&quot;:&quot;2017-06-12&quot;,&quot;endDate&quot;:&quot;2017-06-17&quot;},</pre><pre>         {&quot;rateValue&quot;:&quot;95.0&quot;,&quot;startDate&quot;:&quot;2017-06-21&quot;,&quot;endDate&quot;:null}</pre><pre>]</pre><pre>}</pre>Per ulteriori informazioni sull’utilizzo dell’API Workfront, consulta l’articolo [Nozioni di base sulle API](https://experience.workfront.com/s/article/API-Basics-638808549).
