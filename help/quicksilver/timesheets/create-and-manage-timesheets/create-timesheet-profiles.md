---
product-area: timesheets;system-administration
navigation-topic: create-and-manage-timesheets
title: Creare, modificare e assegnare profili di schede orario
description: Puoi creare, modificare e assegnare profili di schede orario che generino schede orario ricorrenti per gli utenti senza ulteriori interventi da parte tua. In questo modo si risparmia tempo e si garantisce coerenza tra gli utenti.
author: Alina
feature: Timesheets
exl-id: 8f4826bd-82b4-4157-a7d4-a7c94b8fc879
source-git-commit: 9b6552fe496a1602786cdc6b6050d02cd367a531
workflow-type: tm+mt
source-wordcount: '1519'
ht-degree: 1%

---

# Creare, modificare e assegnare profili di schede orario

Puoi creare, modificare e assegnare profili di schede orario che generino schede orario ricorrenti per gli utenti senza ulteriori interventi da parte tua. In questo modo si risparmia tempo e si assicura che le seguenti operazioni siano coerenti tra gli utenti:

* Intervallo temporale scheda orario
* Approvatori
* Tipi di ore generali

Per ulteriori informazioni sulla creazione manuale di una scheda orario, consulta [Creare una scheda orario monouso](../../timesheets/create-and-manage-timesheets/create-tmshts.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>È necessario disporre dell'accesso amministrativo alle schede orario. </p> <p>Per ulteriori informazioni, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">Concedere agli utenti l'accesso amministrativo a determinate aree</a>.</p>  <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
 </tbody> 
</table>

*Per informazioni sulla pianificazione, il tipo di licenza o l&#39;accesso disponibili, contattare l&#39;amministratore Workfront.

## Creare o modificare un profilo di scheda orario

<!--
<div style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p style="color: #ff1493;">Alina drafted an Important note under this heading because Tracy/WorkEx said this is not working as designed - the changes WILL take effect the minute to make them for existing timesheets - see this issue - https://hub.workfront.com/issue/5dba59f600c401cca536567c368aa299/overview</p>
<p style="color: #ff1493;">Important: The changes you make to an existing timesheet profile are not automatically applied to timesheets that have already been generated. The changes you make to a timesheet prile are applied only to the timesheets that are&nbsp;generated after the timesheet profiles changes are made. To&nbsp;apply your&nbsp;changes to the timesheet profile for the timesheets that are already generated, you must delete the existing timesheets and manually generate&nbsp;them.For more information about deleting and manually generating timesheets, see&nbsp;Delete and manually generating Timesheets.</p>
</div>
-->

>[!IMPORTANT]
>
>Per abilitare le modifiche al profilo della scheda orario nelle schede orario correnti, devi eliminare le schede orario esistenti e quindi generarne di nuove. Per istruzioni, consulta [Eliminare i timesheet in Adobe Workfront](../../timesheets/create-and-manage-timesheets/delete-timesheets.md) e [Genera manualmente i timesheet](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md).

1. Fai clic su **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Se stai creando o modificando un profilo di scheda orario da utilizzare in tutto il sistema, fai clic su **Timesheet e ore**.

   Oppure

   Se crei o modifichi un profilo di scheda orario per un gruppo, fai clic su **Gruppi**, quindi fare clic sul nome del gruppo.

1. Clic **Profili Timesheet**.
1. Per creare un nuovo profilo di scheda orario, fai clic su **Nuovo profilo**.

   Oppure

   Per modificare un profilo di scheda orario esistente, seleziona il profilo che desideri modificare, quindi fai clic su **Modifica**.

   Viene visualizzato il profilo della scheda orario nuovo o esistente.


1. Il giorno **Imposta dettagli** , digitare un **Nome** e **Descrizione** per il profilo della scheda orario e fornire le seguenti informazioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Gruppo con accesso amministratore</strong> </td> 
      <td> <p> 
      <ul> 
      <li> <p>Se stai creando un profilo di scheda orario a livello di sistema, lascia vuoto questo campo.</p> <p>Qualsiasi utente che può modificare gli account utente può allegare una scheda orario a livello di sistema ad altri utenti.</p> <p>Solo un amministratore di Workfront può modificare un profilo di scheda orario a livello di sistema.</p> </li> 
      </ul> 
     <ul> 
      <li> <p>Se stai creando un profilo di scheda orario per un gruppo che amministri, identifica il gruppo qui.</p> <p>Questo non assegna il profilo della scheda orario agli utenti del gruppo, ma consente solo agli amministratori del gruppo di modificare il profilo della scheda orario. Assegnerai il profilo agli utenti nel passaggio 6.</p> <p><b>NOTA</b>

   Quando utenti esterni al gruppo allegano profili della scheda orario a un altro utente, non possono visualizzare o allegare questo profilo.</p> </li>
   </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Crea schede orario</strong> </td> 
      <td> <p> <p>Specifica quando il profilo della scheda orario deve generare le schede orario. Una scheda orario può essere impostata per essere generata automaticamente su base settimanale, bisettimanale, semestrale o mensile. Seleziona il giorno della settimana in cui desideri che venga prodotta la scheda orario.</p>
      <p>Una scheda orario settimanale inizia nella data in cui viene generata. Ad esempio, se crei schede orario settimanali ogni giovedì, il primo giorno della settimana nella scheda orario è giovedì.</p>
      <p><b>NOTA</b></p>

   <p>Workfront crea sempre due schede orario alla volta: la prima scheda orario include sempre la data corrente e la seconda inizia quando termina l’intervallo di tempo della prima scheda orario.</p> </p> </td> 
    </tr> 
     <tr> 
      <td role="rowheader"><p><strong>Approvatori</strong></p> </td> 
      <td> <p> <p>Gli approvatori sono utenti che approvano la scheda orario per gli utenti associati alla scheda orario. È possibile identificare fino a 7 utenti come approvatori in una scheda orario. L'identificazione di più utenti è utile per garantire la disponibilità di un approvatore quando un utente si trova fuori sede. Tutti gli approvatori ricevono una notifica quando un utente invia la scheda orario per l’approvazione. È sufficiente un solo utente per approvare la scheda orario.</p> <p>Solo gli utenti con diritti di amministrazione della scheda orario possono essere impostati come approvatori. Per ulteriori informazioni sui diritti amministrativi delle schede orario, vedere <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Concedere agli utenti l'accesso amministrativo a determinate aree</a>.</p> <p>Utilizzare il menu a discesa per selezionare l'approvatore per la scheda orario (se è necessario un approvatore). Puoi scegliere tra le seguenti opzioni:</p> 
      <ul> 
      <li><strong>Nessuno</strong>: la scheda orario non deve essere approvata.</li> 
      <li><strong>Il loro manager</strong>: questo è l’approvatore predefinito, impostato dal sistema. In questo caso, l’utente designato come proprio manager approva la scheda orario quando questa viene inviata per l’approvazione.</li> 
      <li><strong>Persone specifiche:</strong> È possibile designare utenti specifici, per nome, come approvatori della scheda orario. In una scheda orario possono essere presenti più approvatori. In questo caso, dopo che uno degli approvatori ha approvato la scheda orario, questa viene contrassegnata come <strong>Chiuso</strong> e scompare dall’elenco approvazioni scheda orario di tutti gli approvatori rimanenti.</li> 
       </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Può modificare l’ora </strong> </td> 
      <td> <p> <p>Selezionare questa opzione per consentire agli approvatori di modificare le ore nella scheda orario.

   Questa opzione funziona con **Limita la modifica della scheda orario a proprietari e amministratori** nell&#39;area Setup (Configurazione) > Timesheet &amp; Hours (Schede orario e ore) > Preferences (Preferenze). Per ulteriori informazioni, consulta <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md">Configurare le preferenze di orario e scheda orario</a>.

   Esistono i seguenti scenari:

   <ul>
      <li>Quando <b>Limita la modifica della scheda orario a proprietari e amministratori</b> l'opzione è abilitata:</li>
      <ul><li>Gli approvatori possono approvare e rifiutare solo la scheda orario, indipendentemente dal fatto che <b>Può modificare l’ora</b> è abilitato o meno. </li>
      <li>I responsabili dei proprietari delle schede orario possono visualizzare solo le schede orario dei loro referenti diretti.</li></ul>
      <li>Quando <b>Limita la modifica della scheda orario a proprietari e amministratori</b> l'opzione è disabilitata:</li>
    <ul><li>Quando <b>Può modificare l’ora</b> è attivato, gli approvatori possono inviare, riaprire o chiudere la scheda orario e possono modificare l’ora.</li>
      <li>Quando <b>Può modificare l’ora</b> è disattivato, gli approvatori non possono inviare, riaprire o chiudere la scheda orario e non possono modificare l’ora. Gli approvatori possono approvare o rifiutare solo la scheda orario. </li>
      <li>I responsabili dei proprietari delle schede orario possono inviare, richiamare, riaprire e modificare le schede orario dei loro referenti diretti.</li></ul>
      </ul>

   <p><b>NOTA</b>

   Dopo aver inviato una scheda orario per l&#39;approvazione, non è più possibile modificare le ore. Per ripristinare lo stato modificabile di una scheda orario inviata, richiamarla o richiedere all&#39;approvatore di rifiutarla. Per ulteriori informazioni, consulta <a href="../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md">Invia una scheda orario per l&#39;approvazione</a> e<a href="../../timesheets/create-and-manage-timesheets/timesheet-approvals.md">Approvare una scheda orario</a>.</p> </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader"><strong>Tipi di lavoro disponibili</strong> </td> 
      <td><p>Questa impostazione si riferisce solo ai Tipi di Ora generali e non ai Tipi di Ora specifici del progetto. </p>
      <p>Per impostazione predefinita, gli utenti visualizzano tutte le ore generali su una scheda orario. Tuttavia, se la tua organizzazione desidera che vengano visualizzate solo ore generali specifiche per un particolare gruppo di utenti, puoi selezionare le ore generali da visualizzare nelle schede orario selezionandole nel loro profilo Scheda orario in questo campo. Se vuoi disattivare tutte le ore generali, deseleziona tutti i tipi di ore per generare la scheda orario senza una sezione per le ore generali.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span style="font-weight: bold;">Straordinari</span> </td> 
      <td>È possibile scegliere di nascondere la casella Straordinari nelle schede orario. Questa opzione è disabilitata per impostazione predefinita.</td> 
     </tr> 
    </tbody> 
    </table>

1. Fai clic su **Assegna persone** scheda per associare il profilo scheda orario a utenti, gruppi o team specifici (se sei un amministratore Workfront). Iniziare a digitare il nome dell&#39;utente, del gruppo o del team, quindi fare clic su di esso quando viene visualizzato nell&#39;elenco a discesa.

   Se sei un amministratore gruppo, puoi assegnare il profilo scheda orario ai gruppi che amministri, ma non ai team. Per ulteriori informazioni, consulta [Limitazioni per un amministratore gruppo che assegna un profilo scheda orario](#limitations-for-a-group-administrator-assigning-a-timesheet-profile) in questo articolo.

   >[!NOTE]
   >
   >* È inoltre possibile associare un utente a un profilo scheda orario modificando il profilo utente. Per ulteriori informazioni, consulta [Modificare il profilo di un utente](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
   >* Quando si aggiunge un gruppo, nella scheda Assegna persone viene visualizzato solo il nome del gruppo e non l&#39;elenco dei membri del gruppo. Se si desidera visualizzare i membri del gruppo elencati, fare clic su Salva modifiche, quindi sul nome del profilo della scheda attività appena creato.
   >* Al termine di questi passaggi, il profilo scheda orario genera le schede orario solo per gli utenti o i membri del gruppo assegnati che non dispongono di schede orario esistenti per il periodo corrente.

1. Clic **Salva modifiche**.

   La prima volta che il profilo della scheda orario genera schede orario, vengono create 2 schede orario per ogni utente. Successivamente, ogni volta che genera nuove schede orario, viene creata una scheda orario per utente.

   <!--the content in the table above will need to match the content in the Create timesheets article-->

## Limitazioni per un amministratore gruppo che assegna un profilo scheda orario {#limitations-for-a-group-administrator-assigning-a-timesheet-profile}

Se sei un amministratore gruppo e l’opzione di accesso amministrativo Timesheets &amp; hours (Schede orario e ore) è disabilitata nel tuo livello di accesso, puoi creare profili di schede orario, ma puoi assegnarli solo a:

* Gruppi che amministrate
* Singoli utenti con accesso in modifica che fanno parte di un gruppo amministrato

Per questi gruppi e utenti, non potrai accedere alle schede orario generate dal profilo della scheda orario.

Inoltre, se l’opzione Amministratore utenti (Utenti gruppi) è disabilitata anche nel livello di accesso, puoi assegnare il profilo della scheda orario a un gruppo che amministri, ma influisce solo sugli utenti del gruppo che puoi modificare. Se il gruppo contiene utenti ai quali non hai accesso per la modifica, non viene loro assegnato il profilo della scheda orario insieme al resto del gruppo.

Per informazioni sulle opzioni Schede orario e ore nel livello di accesso, consulta [Concedere agli utenti l&#39;accesso amministrativo a determinate aree](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

Per informazioni sull&#39;opzione Amministratore utenti (Utenti gruppi) nel livello di accesso, vedi [Concedere l’accesso agli utenti](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

## Più profili di schede orario ricorrenti

Puoi avere più di un profilo di scheda orario per la tua organizzazione se sono presenti:

* Periodi di pagamento univoci per diversi gruppi di utenti
* Approvatori univoci per diversi set di utenti
* Requisiti generali univoci per le ore per i diversi gruppi di utenti

Un utente non può essere associato a più di un profilo di scheda orario alla volta. 
