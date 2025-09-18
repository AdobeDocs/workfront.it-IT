---
product-area: timesheets;system-administration
navigation-topic: create-and-manage-timesheets
title: Creare, modificare e assegnare profili della scheda orario
description: Puoi creare, modificare e assegnare profili di schede orario che generino schede orario ricorrenti per gli utenti senza ulteriori interventi da parte tua. In questo modo si risparmia tempo e si garantisce coerenza tra gli utenti.
author: Lisa
feature: Timesheets
exl-id: 8f4826bd-82b4-4157-a7d4-a7c94b8fc879
source-git-commit: 764200970aeb8d121cd99a8d4239e0b9853670a9
workflow-type: tm+mt
source-wordcount: '1635'
ht-degree: 2%

---

# Creare, modificare e assegnare profili della scheda orario

<!--Audited: 06/2025-->

Puoi creare, modificare e assegnare profili di schede orario che generino schede orario ricorrenti per gli utenti senza ulteriori interventi da parte tua. In questo modo si risparmia tempo e si assicura che le seguenti operazioni siano coerenti tra gli utenti:

* Intervallo temporale scheda orario
* Approvatori
* Tipi di ore generali

Per ulteriori informazioni sulla creazione manuale di una scheda orario, vedere [Creare una scheda orario monouso](../../timesheets/create-and-manage-timesheets/create-tmshts.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

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
   <td> <p>Nuovo: Standard </p>
 <p>oppure</p> 
<p>Corrente: Piano </p> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>È necessario disporre dell'accesso amministrativo alle schede orario. </p> </td> 
  </tr> 
 </tbody> 
</table>

*Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creare o modificare un profilo di scheda orario

<!--Old info: 
<div style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p style="color: #ff1493;">Alina drafted an Important note under this heading because Tracy/WorkEx said this is not working as designed - the changes WILL take effect the minute to make them for existing timesheets - see this issue - https://hub.workfront.com/issue/5dba59f600c401cca536567c368aa299/overview</p>
<p style="color: #ff1493;">Important: The changes you make to an existing timesheet profile are not automatically applied to timesheets that have already been generated. The changes you make to a timesheet prile are applied only to the timesheets that are&nbsp;generated after the timesheet profiles changes are made. To&nbsp;apply your&nbsp;changes to the timesheet profile for the timesheets that are already generated, you must delete the existing timesheets and manually generate&nbsp;them.For more information about deleting and manually generating timesheets, see&nbsp;Delete and manually generating Timesheets.</p>
</div>
-->

>[!IMPORTANT]
>
>Per abilitare le modifiche al profilo della scheda orario nelle schede orario correnti, è necessario eliminare le schede orario esistenti prima di apportare le modifiche ai profili delle schede orario, quindi generare nuove schede orario. Per istruzioni, vedere [Eliminare i Timesheets in Adobe Workfront](../../timesheets/create-and-manage-timesheets/delete-timesheets.md) e [Generare manualmente i Timesheets](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md).

{{step-1-to-setup}}

1. Se crei o modifichi un profilo di scheda orario da utilizzare in tutto il sistema, fai clic su **Scheda orario e ore**.

   Oppure

   Se crei o modifichi un profilo di scheda orario per un gruppo, fai clic su **Gruppi**, quindi fai clic sul nome del gruppo.

1. Fare clic su **Profili scheda orario**.
1. Per creare un profilo di scheda orario, fare clic su **Nuovo profilo**.

   Oppure

   Per modificare un profilo di scheda orario esistente, selezionare il profilo di scheda orario che si desidera modificare, quindi fare clic su **Modifica**.

   Viene visualizzata la pagina del profilo della scheda orario nuova o esistente.


1. Fai clic sulla scheda **Imposta dettagli**, quindi aggiorna le seguenti informazioni: <!-- at the Production release, change the order of some of these rows, as they changed in the unshimmed UI-->

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Nome</strong> </td> 
      <td> <p> Aggiungi un nome per il profilo della scheda orario. Potrebbe essere il nome di un team o di un gruppo le cui persone condividono lo stesso arco temporale per le loro schede orario. </p> <p>Questo è un campo obbligatorio.</p> </td> 
     </tr>

   <tr> 
      <td role="rowheader"><strong>Descrizione</strong> </td> 
      <td> <p> Aggiungi ulteriori informazioni sul profilo della scheda orario.     
      </p> </td> 
     </tr>

   <tr> 
   <td role="rowheader"><strong>Gruppo con accesso amministratore</strong> </td> 
      <td> <p> 
      <ul> 
      <li> <p>Se stai creando un profilo di scheda orario a livello di sistema, lascia vuoto questo campo.</p> <p>Qualsiasi utente che può modificare gli account utente può allegare una scheda orario a livello di sistema ad altri utenti.</p> <p>Solo un amministratore di Workfront può modificare un profilo di scheda orario a livello di sistema.</p> </li> 
      </ul> 
     <ul> 
      <li> <p>Se stai creando un profilo di scheda orario per un gruppo che amministri, identifica il gruppo qui.</p> <p>Questo non assegna il profilo della scheda orario agli utenti del gruppo, ma consente solo agli amministratori del gruppo di modificare il profilo della scheda orario. Assegnerai il profilo agli utenti nel passaggio 6.</p>

   <p><b>NOTA</b>: quando utenti esterni al gruppo allegano profili di schede orario a un altro utente, non potranno vedere o allegare questo profilo di schede orario.</p> </li> 
      </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Crea schede orario</strong> </td> 
      <td> <p> <p>Specifica quando il profilo della scheda orario deve generare le schede orario. Una scheda orario può essere impostata per essere generata automaticamente su base settimanale, bisettimanale, semestrale o mensile. Seleziona il giorno della settimana in cui desideri che venga prodotta la scheda orario.</p>
      <p>Una scheda orario settimanale inizia nella data in cui viene generata. Ad esempio, se crei schede orario settimanali ogni giovedì, il primo giorno della settimana nella scheda orario è giovedì.</p>


   <p><b>NOTA</b>: Workfront crea sempre due schede orario alla volta: la prima scheda orario include sempre la data corrente e la seconda scheda orario inizia quando termina l'intervallo di tempo della prima.</p> </p> </td> 
   </tr> 
     <tr> 
      <td role="rowheader"><p><strong>Approvatori</strong></p> </td> 
      <td> <p> <p>Gli approvatori sono utenti che approvano la scheda orario per gli utenti associati alla scheda orario. È possibile identificare fino a 7 utenti come approvatori in una scheda orario. L'identificazione di più utenti è utile per garantire la disponibilità di un approvatore quando un utente si trova fuori sede. Tutti gli approvatori ricevono una notifica quando un utente invia la scheda orario per l’approvazione. È sufficiente un solo utente per approvare la scheda orario.</p> <p>Solo gli utenti con diritti di amministrazione della scheda orario possono essere impostati come approvatori. Per ulteriori informazioni sui diritti amministrativi delle schede orario, vedere <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Concedere agli utenti l'accesso amministrativo ad alcune aree</a>.</p> <p>Utilizzare il menu a discesa per selezionare l'approvatore per la scheda orario (se è necessario un approvatore). Puoi scegliere una delle opzioni seguenti:</p> 
      <ul> 
      <li><strong>Nessuno</strong>: la scheda orario non deve essere approvata.</li> 
      <li><strong>Responsabile</strong>: è l'approvatore predefinito, impostato dal sistema. In questo caso, l’utente designato come proprio manager approva la scheda orario quando questa viene inviata per l’approvazione.</li> 
      <li><strong>Persone specifiche:</strong> È possibile designare utenti specifici, per nome, come approvatori della scheda orario. In una scheda orario possono essere presenti più approvatori. In questo caso, dopo che uno degli approvatori ha approvato la scheda orario, la scheda viene contrassegnata come <strong>Chiusa</strong> e scompare dall'elenco delle approvazioni della scheda orario di tutti gli approvatori rimanenti.</li> 
       </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>È possibile modificare l'ora </strong> </td> 
      <td> <p> <p>Selezionare questa opzione per consentire agli approvatori di modificare le ore nella scheda orario.

   <p>Questa opzione funziona con l’impostazione **Limita la modifica della scheda orario a proprietari e amministratori** nell’area Configurazione &gt; Scheda orario e ore &gt; Preferenze. Per ulteriori informazioni, consulta <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md">Configurare le preferenze di orario e scheda orario</a>.</p>

   <p>Esistono i seguenti scenari: </p>

   <ul>
      <li>Quando l'opzione <b>Limita la modifica della scheda orario a proprietari e amministratori</b> è abilitata:</li>
      <ul><li>Gli approvatori possono solo approvare e rifiutare la scheda orario, indipendentemente dal fatto che l'<b>orario di modifica</b> sia abilitato o meno. </li>
      <li>I responsabili dei proprietari delle schede orario possono visualizzare solo le schede orario dei loro referenti diretti.</li></ul>
      <li>Quando l'opzione <b>Limita la modifica della scheda orario a proprietari e amministratori</b> è disabilitata:</li>
    <ul><li>Quando l'ora <b>Può modificare</b> è abilitata, gli approvatori possono inviare, riaprire o chiudere la scheda orario e modificare l'ora.</li>
      <li>Se l'ora <b>Può modificare</b> è disabilitata, gli approvatori non possono inviare, riaprire o chiudere la scheda orario e non possono modificare l'ora. Gli approvatori possono approvare o rifiutare solo la scheda orario. </li>
      <li>I responsabili dei proprietari delle schede orario possono inviare, richiamare, riaprire e modificare le schede orario dei loro referenti diretti.</li></ul>
      </ul>

   <p>

   <b>NOTA</b>: dopo aver inviato una scheda orario per l&#39;approvazione, non è più possibile modificare le ore. Per ripristinare lo stato modificabile di una scheda orario inviata, richiamarla o richiedere all&#39;approvatore di rifiutarla. Per ulteriori informazioni, vedere <a href="../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md">Inviare una scheda orario per l&#39;approvazione</a> e<a href="../../timesheets/create-and-manage-timesheets/timesheet-approvals.md">Approvare una scheda orario</a>.</p> </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader"><strong>Tipi di lavoro disponibili</strong> </td> 
      <td><p>Questa impostazione si riferisce solo ai Tipi di Ora generali e non ai Tipi di Ora specifici del progetto. </p>
      <p>Per impostazione predefinita, gli utenti visualizzano tutte le ore generali su una scheda orario. Tuttavia, se la tua organizzazione desidera che vengano visualizzate solo ore generali specifiche per un particolare gruppo di utenti, puoi selezionare le ore generali da visualizzare nelle schede orario selezionandole nel loro profilo Scheda orario in questo campo. Se vuoi disattivare tutte le ore generali, deseleziona tutti i tipi di ore per generare la scheda orario senza una sezione per le ore generali.</p></td> 
     </tr>

   <tr> 
      <td role="rowheader"><strong>Notifiche promemoria</strong> </td> 
      <td> <p> Aggiungi una notifica di promemoria. Workfront invierà dei promemoria agli utenti per chiedere loro di completare o approvare le schede orario. È necessario creare notifiche promemoria prima di associarle a un profilo scheda orario.  </p> </td> 
     </tr>

   <tr data-mc-conditions=""> 
      <td role="rowheader"><span style="font-weight: bold;">Straordinari</span> </td> 
      <td>È possibile scegliere di nascondere la casella Straordinari nelle schede orario. Questa opzione è disabilitata per impostazione predefinita.</td> 
     </tr> 
    </tbody> 
    </table>

1. Durante la creazione di profili di schede orario a livello di gruppo, fare clic sulla scheda **Assegna persone** per associare il profilo della scheda orario a utenti, gruppi o team specifici (se si è un amministratore Workfront). <!--Keep the reference to the group upon release to Prod, for now, until they unshim the group Timesheet Profiles-->

   Durante la creazione dei profili della scheda orario per il sistema, scorri verso il fondo della pagina e trova la sezione **Assegna persone**. <!--Keep the reference to the system when releasing to Prod, until they unshim the group Timesheet Profile-->

   Iniziare a digitare il nome dell&#39;utente, del gruppo o del team, quindi fare clic su di esso quando viene visualizzato nell&#39;elenco a discesa.

   Se sei un amministratore gruppo, puoi assegnare il profilo scheda orario ai gruppi che amministri, ma non ai team. Per ulteriori informazioni, vedere [Limitazioni per un amministratore di gruppo che assegna un profilo di scheda orario](#limitations-for-a-group-administrator-assigning-a-timesheet-profile) in questo articolo.

   >[!NOTE]
   >
   >* È inoltre possibile associare un utente a un profilo scheda orario modificando il profilo utente. Per ulteriori informazioni, vedere [Modificare il profilo di un utente](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
   >* Quando si aggiunge un gruppo, nella scheda Assegna persone viene visualizzato solo il nome del gruppo e non l&#39;elenco dei membri del gruppo. Se si desidera visualizzare i membri del gruppo elencati, fare clic su Salva modifiche, quindi sul nome del profilo della scheda attività appena creato.
   >* Al termine di questi passaggi, il profilo scheda orario genera le schede orario solo per gli utenti o i membri del gruppo assegnati che non dispongono di schede orario esistenti per il periodo corrente.

1. Fai clic su **Salva**.

1. Nella parte superiore dell&#39;elenco dei profili della scheda orario, fare clic sull&#39;icona **Altro** ![Altro icona](assets/more-icon.png) per i profili della scheda orario a livello di sistema oppure **Altro** per i profili della scheda orario di gruppo, quindi fare clic su **Genera schede orario**.

   Nella parte inferiore della schermata viene visualizzata una conferma che le schede orario sono state generate correttamente. Le nuove schede orario vengono generate in base ai nuovi profili creati.

   Per ulteriori informazioni, vedere [Generare manualmente le schede orario](/help/quicksilver/timesheets/create-and-manage-timesheets/manually-generate-timesheets.md).

   La prima volta che il profilo della scheda orario genera schede orario, vengono create 2 schede orario per ogni utente, sia per l’intervallo temporale che include l’ora corrente che per l’intervallo temporale seguente.

   Successivamente, ogni volta che genera nuove schede orario, viene creata una scheda orario per utente.

   <!--the content in the table above will need to match the content in the Create timesheets article-->

## Limitazioni per un amministratore gruppo che assegna un profilo scheda orario {#limitations-for-a-group-administrator-assigning-a-timesheet-profile}

Se sei un amministratore gruppo e l’opzione di accesso amministrativo Timesheets &amp; hours (Schede orario e ore) è disabilitata nel tuo livello di accesso, puoi creare profili di schede orario, ma puoi assegnarli solo a:

* Gruppi che amministrate
* Singoli utenti con accesso in modifica che fanno parte di un gruppo amministrato

Per questi gruppi e utenti, non potrai accedere alle schede orario generate dal profilo della scheda orario.

Inoltre, se l’opzione Amministratore utenti (Utenti gruppi) è disabilitata anche nel livello di accesso, puoi assegnare il profilo della scheda orario a un gruppo che amministri, ma influisce solo sugli utenti del gruppo che puoi modificare. Se il gruppo contiene utenti ai quali non hai accesso per la modifica, non viene loro assegnato il profilo della scheda orario insieme al resto del gruppo.

Per informazioni sull&#39;opzione Timesheets &amp; hours nel tuo livello di accesso, vedi [Concedere agli utenti l&#39;accesso amministrativo ad alcune aree](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

Per informazioni sull&#39;opzione Amministratore utenti (Utenti gruppi) nel proprio livello di accesso, vedere [Concedere l&#39;accesso agli utenti](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

## Più profili di schede orario ricorrenti

Puoi avere più di un profilo di scheda orario per la tua organizzazione se sono presenti:

* Periodi di pagamento univoci per diversi gruppi di utenti
* Approvatori univoci per diversi set di utenti
* Requisiti generali univoci per le ore per i diversi gruppi di utenti

Un utente non può essere associato a più di un profilo di scheda orario alla volta.
