---
product-area: timesheets;system-administration
navigation-topic: create-and-manage-timesheets
title: Creare, modificare e assegnare profili della scheda orario
description: Puoi creare, modificare e assegnare profili di schede orario che generino schede orario ricorrenti per gli utenti senza ulteriori interventi da parte tua. In questo modo si risparmia tempo e si garantisce coerenza tra gli utenti.
author: Lisa
feature: Timesheets
exl-id: 8f4826bd-82b4-4157-a7d4-a7c94b8fc879
source-git-commit: b0b9b80b4eb718e3e131ee0cd022f54cb906f187
workflow-type: tm+mt
source-wordcount: '1584'
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
   <td>Pacchetto Adobe Workfront</td> 
   <td><p>Qualsiasi</p></td> 
  </tr> 
  <tr> 
   <td>Licenza Adobe Workfront</td> 
   <td>
   <p>Standard</p>
   <p>Piano</p></td>
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td><p>Accesso amministrativo alle schede orario</p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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

1. Aggiorna le seguenti informazioni:

   * **Nome**: aggiungi un nome per il profilo della scheda orario. Potrebbe essere il nome di un team o di un gruppo le cui persone condividono lo stesso arco temporale per le loro schede orario. Questo è un campo obbligatorio.
   * **Descrizione**: aggiungi ulteriori informazioni sul profilo scheda orario.
   * **Gruppo con accesso amministratore**: se stai creando un profilo di scheda orario a livello di sistema, lascia vuoto questo campo.

     Qualsiasi utente che può modificare gli account utente può allegare una scheda orario a livello di sistema ad altri utenti.

     Solo un amministratore di Workfront può modificare un profilo di scheda orario a livello di sistema.

     Se stai creando un profilo di scheda orario per un gruppo che amministri, identifica il gruppo qui.

     Questo non assegna il profilo della scheda orario agli utenti del gruppo, ma consente solo agli amministratori del gruppo di modificare il profilo della scheda orario. Assegnerai il profilo agli utenti nel passaggio 6.

     >[!NOTE]
     >
     >Quando utenti esterni al gruppo allegano profili di schede orario ad altri utenti, non potranno vedere o allegare questo profilo di schede orario.

   * **Crea schede orario**: specifica quando il profilo della scheda orario deve generare le schede orario. Una scheda orario può essere impostata per essere generata automaticamente su base settimanale, bisettimanale, semestrale o mensile. Seleziona il giorno della settimana in cui desideri che venga prodotta la scheda orario.

     Una scheda orario settimanale inizia nella data in cui viene generata. Ad esempio, se crei schede orario settimanali ogni giovedì, il primo giorno della settimana nella scheda orario è giovedì.

     >[!NOTE]
     >
     >Workfront crea sempre due schede orario alla volta: la prima scheda orario include sempre la data corrente e la seconda inizia quando termina l’intervallo di tempo della prima scheda orario.

   * **Approvatori**: gli approvatori sono utenti che approvano la scheda orario per gli utenti associati alla scheda orario. È possibile identificare fino a 7 utenti come approvatori in una scheda orario. L&#39;identificazione di più utenti è utile per garantire la disponibilità di un approvatore quando un utente si trova fuori sede. Tutti gli approvatori ricevono una notifica quando un utente invia la scheda orario per l’approvazione. È sufficiente un solo utente per approvare la scheda orario.

     Solo gli utenti con diritti di amministrazione della scheda orario possono essere impostati come approvatori. Per ulteriori informazioni sui diritti amministrativi delle schede orario, vedere [Concedere agli utenti l&#39;accesso amministrativo ad alcune aree](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

     Utilizzare il menu a discesa per selezionare l&#39;approvatore per la scheda orario (se è necessario un approvatore). Puoi scegliere una delle opzioni seguenti:

      * **Nessuno**: la scheda orario non deve essere approvata.
      * **Responsabile**: è l&#39;approvatore predefinito, impostato dal sistema. In questo caso, l’utente designato come proprio manager approva la scheda orario quando questa viene inviata per l’approvazione.
      * **Persone specifiche**: è possibile designare utenti specifici, per nome, come approvatori della scheda orario. In una scheda orario possono essere presenti più approvatori. In questo caso, dopo che uno degli approvatori ha approvato la scheda orario, la scheda viene contrassegnata come **Chiusa** e scompare dall&#39;elenco delle approvazioni della scheda orario di tutti gli approvatori rimanenti.

   * **Può modificare l&#39;ora**: selezionare questa opzione per consentire agli approvatori di modificare le ore nella scheda orario.

     Questa opzione funziona con l&#39;impostazione **Limita la modifica della scheda orario a proprietari e amministratori** nell&#39;area Configurazione > Scheda orario e ore > Preferenze. Per ulteriori informazioni, consulta [Configurare le preferenze di orario e scheda orario](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

     Esistono i seguenti scenari:

     Quando l&#39;opzione **Limita la modifica della scheda orario a proprietari e amministratori** è abilitata:

      * Gli approvatori possono approvare e rifiutare solo le schede orario, indipendentemente dal fatto che l’opzione Può modificare sia abilitata o meno.
      * I responsabili dei proprietari delle schede orario possono visualizzare solo le schede orario dei loro referenti diretti.

     Quando l&#39;opzione **Limita la modifica della scheda orario a proprietari e amministratori** è disabilitata:

      * Quando **Può modificare l&#39;ora** è abilitato, gli approvatori possono inviare, riaprire o chiudere la scheda orario e modificare l&#39;ora.
      * Se **L&#39;ora di modifica** è disabilitata, gli approvatori non possono inviare, riaprire o chiudere la scheda orario e non possono modificare l&#39;ora. Gli approvatori possono approvare o rifiutare solo la scheda orario.
      * I responsabili dei proprietari delle schede orario possono inviare, richiamare, riaprire e modificare le schede orario dei loro referenti diretti.

     >[!NOTE]
     >
     >Dopo aver inviato una scheda orario per l&#39;approvazione, non è più possibile modificare le ore. Per ripristinare lo stato modificabile di una scheda orario inviata, richiamarla o richiedere all&#39;approvatore di rifiutarla. Per ulteriori informazioni, vedere [Inviare una scheda orario per l&#39;approvazione](/help/quicksilver/timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md) e [Approvare una scheda orario](/help/quicksilver/timesheets/create-and-manage-timesheets/timesheet-approvals.md).

   * **Straordinari**: puoi scegliere di nascondere la casella Straordinari nelle schede orario. Questa opzione è disabilitata per impostazione predefinita.
   * **Tipi di lavoro disponibili**: questa impostazione fa riferimento solo ai tipi di lavoro generali e non ai tipi di lavoro specifici del progetto.

     Per impostazione predefinita, gli utenti visualizzano tutte le ore generali su una scheda orario. Tuttavia, se la tua organizzazione desidera che vengano visualizzate solo ore generali specifiche per un particolare gruppo di utenti, puoi selezionare le ore generali da visualizzare nelle schede orario selezionandole nel loro profilo Scheda orario in questo campo. Se vuoi disattivare tutte le ore generali, deseleziona tutti i tipi di ore per generare la scheda orario senza una sezione per le ore generali.

   * **Notifiche promemoria**: aggiungere una notifica promemoria. Workfront invierà dei promemoria agli utenti per chiedere loro di completare o approvare le schede orario. È necessario creare notifiche promemoria prima di associarle a un profilo scheda orario.

1. Per associare il profilo della scheda orario a utenti, gruppi o team specifici (se sei un amministratore di Workfront), scorri verso il fondo della pagina e individua la sezione **Assegna persone**.

   Iniziare a digitare il nome dell&#39;utente, del gruppo o del team, quindi fare clic su di esso quando viene visualizzato nell&#39;elenco a discesa.

   <!--To associate the timesheet profile with specific users, groups, or (if you are a Workfront administrator) teams, scroll towards the bottom of the page and find the **Assign People** section.-->

   Se sei un amministratore gruppo, puoi assegnare il profilo scheda orario ai gruppi che amministri, ma non ai team. Per ulteriori informazioni, vedere [Limitazioni per un amministratore di gruppo che assegna un profilo di scheda orario](#limitations-for-a-group-administrator-assigning-a-timesheet-profile) in questo articolo.

   >[!NOTE]
   >
   >* È inoltre possibile associare un utente a un profilo scheda orario modificando il profilo utente. Per ulteriori informazioni, vedere [Modificare il profilo di un utente](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
   >* Quando si aggiunge un gruppo, nella scheda Assegna persone viene visualizzato solo il nome del gruppo e non l&#39;elenco dei membri del gruppo. Se si desidera visualizzare i membri del gruppo elencati, fare clic su Salva modifiche, quindi sul nome del profilo della scheda attività appena creato.
   >* Al termine di questi passaggi, il profilo scheda orario genera le schede orario solo per gli utenti o i membri del gruppo assegnati che non dispongono di schede orario esistenti per il periodo corrente.

1. Fai clic su **Salva**.

1. Nella parte superiore dell&#39;elenco dei profili della scheda orario, fai clic sull&#39;icona **Altro** ![Altro](assets/more-icon.png), quindi fai clic su **Genera schede orario**.

   Nella parte inferiore della schermata viene visualizzata una conferma che le schede orario sono state generate correttamente. Le nuove schede orario vengono generate in base ai nuovi profili creati.

   Per ulteriori informazioni, vedere [Generare manualmente le schede orario](/help/quicksilver/timesheets/create-and-manage-timesheets/manually-generate-timesheets.md).

   La prima volta che il profilo della scheda orario genera le schede orario, vengono create due schede orario per ogni utente, sia per l’intervallo temporale che include l’ora corrente che per l’intervallo temporale seguente.

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

<!--
<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Name</strong> </td> 
      <td> <p> Add a name for the timesheet profile. It could be the name of a team or a group whose people share the same timeframe for their timesheets. </p> <p>This ia a required field.</p> </td> 
     </tr> 

   <tr> 
      <td role="rowheader"><strong>Description</strong> </td> 
      <td> <p> Add more information about the timesheet profile.     
      </p> </td> 
     </tr>

   <tr> 
   <td role="rowheader"><strong>Group with Administration Access</strong> </td> 
      <td> <p> 
      <ul> 
      <li> <p>If you are creating a system-level timesheet profile, leave this field blank.</p> <p>Any user who can edit user accounts can attach a system-level timesheet to other users.</p> <p>Only a Workfront administrator can edit a system-level timesheet profile.</p> </li> 
      </ul> 
     <ul> 
      <li> <p>If you are creating a timesheet profile for a group you administer, identify the group here.</p> <p>This does not assign the timesheet profile to the users in the group; it only allows the group's administrators to modify the timesheet profile. You will assign the profile to users in Step 6.</p>

   <p><b>NOTE</b>: When users outside the group are attaching timesheet profiles to other users, they won't be able to see or attach this timesheet profile.</p> </li> 
      </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Create timesheets</strong> </td> 
      <td> <p> <p>Specify when the timesheet profile should generate the timesheets. A timesheet can be set to automatically generate on a weekly, bi-weekly, semi-monthly, or monthly basis. Select the day of the week when you want the timesheet to be produced.</p>
      <p>A weekly timesheet begins on the date it is generated. For example, if you create weekly timesheets every Thursday, the first day of the week on the timesheet is Thursday.</p>
    
      
   <p><b>NOTE</b>: Workfront always creates two timesheets at a time: the first timesheet always includes the current date, and the second timesheet starts when the time frame of the first one ends.</p> </p> </td> 
   </tr> 
     <tr> 
      <td role="rowheader"><p><strong>Approvers</strong></p> </td> 
      <td> <p> <p>Approvers are users who approve the timesheet for the users associated with the timesheet. You can identify up to 7 users as approvers on a timesheet. Identifying multiple users is useful to ensure an approver is available when someone is out of the office. All approvers are notified when a user submits the timesheet for approval. Only one user is required to approve the timesheet in order for it to be approved.</p> <p>Only users with timesheet administrative rights can be set as approvers. For more information about timesheet administrative rights, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Grant users administrative access to certain areas</a>.</p> <p>Use the drop-down menu&nbsp;to select&nbsp;the approver&nbsp;for the timesheet (if an approver is required). You can select from the following options:</p> 
      <ul> 
      <li><strong>None</strong>: The timesheet does not need to&nbsp;be approved.</li> 
      <li><strong>Their Manager</strong>: This is the default approver, set by the system. In this case, the user designated as their manager approves the timesheet when it is submitted for approval.</li> 
      <li><strong>Specific People:</strong>&nbsp;You can designate specific users, by name, as timesheet approvers. You can have multiple approvers on a timesheet. In this case, after&nbsp;one of the approvers approves the timesheet, the timesheet is marked as <strong>Closed</strong> and it disappears from the timesheet approvals list of all the remaining approvers.</li> 
       </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Can edit time </strong> </td> 
      <td> <p> <p>Select this option to allow the approvers to edit hours on the timesheet. 

   <p>This option works together with the **Restrict timesheet editing to owners and admins** setting in the Setup > Timesheet & Hours > Preferences area. For more information, see <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md">Configure timesheet and hour preferences</a>.</p>

   <p>The following scenarios exist: </p>

   <ul>
      <li>When the <b>Restrict timesheet editing to owners and admins</b> option is enabled:</li>
      <ul><li>Approvers can only approve and reject timesheet, regardless of whether the <b>Can edit time</b> is enabled or not. </li>
      <li>Timesheet owners' managers can only view their direct reports' timesheets.</li></ul>
      <li>When the <b>Restrict timesheet editing to owners and admins</b> option is disabled:</li>
    <ul><li>When the <b>Can edit time</b> is enabled, approvers can submit, reopen, or close the timesheet and can edit the time.</li>
      <li>When the <b>Can edit time</b> is disabled, approvers cannot submit, reopen, or close the timesheet and cannot edit the time. Approvers can only approve or reject the timesheet. </li>
      <li>Timesheet owners' managers can submit, recall, reopen, and edit their direct reports' timesheets.</li></ul>
      </ul>

   <p>

   <b>NOTE</b>: Once you submit a timesheet for approval, you can no longer edit the hours. To return a submitted timesheet to an editable state, recall the timesheet or have the approver reject the timesheet. For more information, see <a href="../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md">Submit a timesheet for approval</a> and <a href="../../timesheets/create-and-manage-timesheets/timesheet-approvals.md">Approve a timesheet</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Overtime</strong> </td> 
      <td>You can choose to hide the Overtime box in timesheets. This option is disabled by default.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Available Hour Types</strong> </td> 
      <td><p>This setting refers only to General Hour Types, and not to project-specific hour types. </p>
      <p>By default, users see all general hours on a timesheet. However, if your organization wants only specific general hours to be shown for a particular set of users, you can select the general hours that they need to see in their timesheets by selecting them in their timesheet profile in this field. If you want to disable all general hours, deselect all hour types to generate the timesheet without a section for general hours.</p></td> 
     </tr> 

   <tr> 
      <td role="rowheader"><strong>Reminder notifications</strong> </td> 
      <td> <p> Add a reminder notification. Workfront will send reminders to users to ask them to complete or approve their timesheets. You must create reminder notifications before you can associate them with a timesheet profile.  </p> </td> 
     </tr>
    </tbody> 
   </table>
-->