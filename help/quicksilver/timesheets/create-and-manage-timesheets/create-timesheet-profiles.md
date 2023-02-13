---
product-area: timesheets;system-administration
navigation-topic: create-and-manage-timesheets
title: Creare, modificare e assegnare profili della scheda attività
description: È possibile creare, modificare e assegnare profili della scheda attività che generano fogli presenze ricorrenti per gli utenti senza ulteriori interventi da parte dell'utente. Ciò ti consente di risparmiare tempo e assicura che i seguenti elementi siano coerenti tra gli utenti - EDIT ME.
author: Alina
feature: Timesheets
exl-id: 8f4826bd-82b4-4157-a7d4-a7c94b8fc879
source-git-commit: 7e2a4b02277e8b82ac6ee92a7994250fcdebb0b0
workflow-type: tm+mt
source-wordcount: '1509'
ht-degree: 1%

---

# Creare, modificare e assegnare profili della scheda attività

È possibile creare, modificare e assegnare profili della scheda attività che generano fogli presenze ricorrenti per gli utenti senza ulteriori interventi da parte dell&#39;utente. In questo modo potrai risparmiare tempo e garantire che i seguenti elementi siano coerenti tra gli utenti:

* Intervallo temporale della scheda attività
* Approvatori
* Tipi di ore generali

Per ulteriori informazioni sulla creazione manuale di una scheda attività, vedere [Creare una scheda attività a uso singolo](../../timesheets/create-and-manage-timesheets/create-tmshts.md).

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
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>È necessario disporre dell’accesso amministrativo ai fogli presenze. </p> <p>Per ulteriori informazioni, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">Consentire agli utenti l'accesso amministrativo a determinate aree</a>.</p>  <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
 </tbody> 
</table>

*Per sapere quale piano, tipo di licenza o accesso si dispone, contattare l&#39;amministratore Workfront.

## Creare o modificare un profilo di una scheda attività

<!--
<div style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p style="color: #ff1493;">Alina drafted an Important note under this heading because Tracy/WorkEx said this is not working as designed - the changes WILL take effect the minute to make them for existing timesheets - see this issue - https://hub.workfront.com/issue/5dba59f600c401cca536567c368aa299/overview</p>
<p style="color: #ff1493;">Important: The changes you make to an existing timesheet profile are not automatically applied to timesheets that have already been generated. The changes you make to a timesheet prile are applied only to the timesheets that are&nbsp;generated after the timesheet profiles changes are made. To&nbsp;apply your&nbsp;changes to the timesheet profile for the timesheets that are already generated, you must delete the existing timesheets and manually generate&nbsp;them.For more information about deleting and manually generating timesheets, see&nbsp;Delete and manually generating Timesheets.</p>
</div>
-->

>[!IMPORTANT]
>
>Per abilitare le modifiche del profilo della scheda attività nei fogli presenze correnti, è necessario eliminare i fogli presenze esistenti e quindi generarne di nuovi. Per istruzioni, consulta [Eliminare i fogli presenze in Adobe Workfront](../../timesheets/create-and-manage-timesheets/delete-timesheets.md) e [Generare manualmente fogli presenze](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md).

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Se si sta creando o modificando un profilo della scheda attività da utilizzare in tutto il sistema, fare clic su **Scheda attività e ore**.

   Oppure

   Se si crea o si modifica un profilo foglio presenze per un gruppo, fare clic su **Gruppi**, quindi fai clic sul nome del gruppo.

1. Fai clic su **Profili scheda attività**.
1. Per creare un nuovo profilo della scheda attività, fare clic su **Nuovo profilo**.

   Oppure

   Per modificare un profilo della scheda attività esistente, selezionare il profilo della scheda attività che si desidera modificare, quindi fare clic su **Modifica**.

   Viene visualizzato il profilo della scheda attività nuova o esistente.


1. Sulla **Imposta dettagli** scheda, digita un **Nome** e **Descrizione** per il profilo della scheda attività e fornire le seguenti informazioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Gruppo con accesso amministratore</strong> </td> 
      <td> <p> 
      <ul> 
      <li> <p>Se si sta creando un profilo della scheda attività a livello di sistema, lasciare vuoto questo campo.</p> <p>Qualsiasi utente che può modificare gli account utente può allegare una scheda attività a livello di sistema ad altri utenti.</p> <p>Solo un amministratore Workfront può modificare un profilo della scheda attività a livello di sistema.</p> </li> 
      </ul> 
     <ul> 
      <li> <p>Se si sta creando un profilo della scheda attività per un gruppo amministrato, identificare il gruppo qui.</p> <p>Questo non assegna il profilo della scheda attività agli utenti del gruppo; consente solo agli amministratori del gruppo di modificare il profilo della scheda attività. Il profilo verrà assegnato agli utenti nel passaggio 6.</p> <p><b>NOTA</b>

   Quando gli utenti al di fuori del gruppo collegano i profili della scheda attività ad altri utenti, non saranno in grado di visualizzare o allegare questo profilo della scheda attività.</p> </li>
   </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Crea schede orario</strong> </td> 
      <td> <p> <p>Specifica quando il profilo della scheda attività deve generare i fogli presenze. È possibile impostare una scheda attività per generare automaticamente su base settimanale, bisettimanale, semestrale o mensile. Selezionare il giorno della settimana in cui si desidera produrre la scheda attività.</p> <p><b>NOTA</b>

   Se si configura un profilo della scheda attività per creare fogli presenze il venerdì, gli utenti non possono registrare le ore del venerdì, del sabato e della domenica per la settimana corrente.</p> <p>Workfront crea sempre due fogli presenze alla volta: la prima scheda attività include sempre la data corrente e la seconda scheda attività inizia quando termina l&#39;intervallo di tempo del primo.</p> </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader"><p><strong>Approvatori</strong></p> </td> 
      <td> <p> <p>Gli approvatori sono utenti che approvano la scheda attività per gli utenti associati alla scheda attività. È possibile identificare fino a 7 utenti come approvatori in una scheda attività. Identificare più utenti è utile per garantire che un approvatore sia disponibile quando qualcuno è fuori ufficio. Tutti gli approvatori vengono avvisati quando un utente invia la scheda attività per l'approvazione. Per approvare la scheda attività è necessario un solo utente.</p> <p>È possibile impostare come approvatori solo gli utenti con diritti di amministrazione della scheda attività. Per ulteriori informazioni sui diritti amministrativi della scheda attività, vedere <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Consentire agli utenti l'accesso amministrativo a determinate aree</a>.</p> <p>Utilizzare il menu a discesa per selezionare l'approvatore per la scheda attività (se è richiesto un approvatore). Puoi scegliere tra le seguenti opzioni:</p> 
      <ul> 
      <li><strong>Nessuno</strong>: La scheda attività non deve essere approvata.</li> 
      <li><strong>Manager</strong>: Questo è l'approvatore predefinito impostato dal sistema. In questo caso, l'utente designato come proprio responsabile approva la scheda attività quando viene inviata per l'approvazione.</li> 
      <li><strong>Persone specifiche:</strong> È possibile designare utenti specifici, per nome, come approvatori della scheda attività. È possibile avere più approvatori in una scheda attività. In questo caso, dopo che uno degli approvatori approva la scheda attività, la scheda attività viene contrassegnata come <strong>Chiuso</strong> e scompare dall'elenco delle approvazioni della scheda attività di tutti gli approvatori rimanenti.</li> 
       </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Può modificare l’ora </strong> </td> 
      <td> <p> <p>Selezionare questa opzione per consentire agli approvatori di modificare le ore nella scheda attività.

   Questa opzione funziona insieme al **Limita la modifica della scheda attività a proprietari e amministratori** nell&#39;area Configurazione > Scheda attività e ore > Preferenze. Per ulteriori informazioni, consulta <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md">Configurare le preferenze relative a schede attività e ora</a>.

   Esistono i seguenti scenari:

   <ul>
      <li>Quando il <b>Limita la modifica della scheda attività a proprietari e amministratori</b> è abilitata:</li>
      <ul><li>Gli approvatori possono solo approvare e rifiutare la scheda attività, indipendentemente dal fatto che la <b>Può modificare il tempo</b> è abilitato o meno. </li>
      <li>I responsabili dei proprietari dei fogli presenze possono visualizzare solo i fogli presenze dei loro rapporti diretti.</li></ul>
      <li>Quando il <b>Limita la modifica della scheda attività a proprietari e amministratori</b> è disabilitata:</li>
    <ul><li>Quando il <b>Può modificare il tempo</b> è abilitato, gli approvatori possono inviare, riaprire o chiudere la scheda attività e possono modificare l'ora.</li>
      <li>Quando il <b>Può modificare il tempo</b> è disabilitato, gli approvatori non possono inviare, riaprire o chiudere la scheda attività e non possono modificare l'ora. Gli approvatori possono solo approvare o rifiutare la scheda attività. </li>
      <li>I responsabili dei proprietari dei fogli presenze possono inviare, richiamare, riaprire e modificare i fogli presenze dei loro report diretti.</li></ul>
      </ul>

   <p><b>NOTA</b>

   Dopo aver inviato una scheda attività per l&#39;approvazione, non è più possibile modificare le ore. Per restituire una scheda attività inviata a uno stato modificabile, richiamare la scheda attività o chiedere al responsabile approvazione di rifiutare la scheda attività. Per ulteriori informazioni, consulta <a href="../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md">Invia una scheda attività per l&#39;approvazione</a> e<a href="../../timesheets/create-and-manage-timesheets/timesheet-approvals.md">Approva una scheda attività</a>.</p> </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader"><strong>Tipi di lavoro disponibili</strong> </td> 
      <td>Per impostazione predefinita, gli utenti visualizzano tutte le ore generali in una scheda attività. Tuttavia, se l'organizzazione desidera che vengano visualizzate solo le ore generali specifiche per un particolare set di utenti, è possibile selezionare le ore generali da visualizzare nelle schede attività selezionando le relative ore nel profilo della scheda attività in questo campo. Se si desidera disattivare tutte le ore generali, deselezionare tutti i tipi di ora per generare la scheda attività senza una sezione per le ore generali.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span style="font-weight: bold;">Straordinari</span> </td> 
      <td>È possibile scegliere di nascondere la casella Overtime nei fogli presenze. Questa opzione è disabilitata per impostazione predefinita.</td> 
     </tr> 
    </tbody> 
    </table>

1. Fai clic sul pulsante **Assegna persone** scheda per associare il profilo della scheda attività a specifici utenti, gruppi o team (se si è un amministratore di Workfront). Inizia a digitare il nome dell’utente, del gruppo o del team, quindi fai clic su di esso quando viene visualizzato nell’elenco a discesa.

   Se si è un amministratore di gruppo, è possibile assegnare il profilo della scheda attività ai gruppi amministrati, ma non ai team. Per ulteriori informazioni, consulta [Limitazioni per l&#39;assegnazione di un profilo della scheda attività da parte di un amministratore di gruppo](#limitations-for-a-group-administrator-assigning-a-timesheet-profile) in questo articolo.

   >[!NOTE]
   >
   >* È inoltre possibile associare un utente a un profilo scheda attività modificando il profilo utente. Per ulteriori informazioni, consulta [Modificare il profilo di un utente](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
   >* Quando si aggiunge un gruppo, nella scheda Assegna persone viene visualizzato solo il nome del gruppo, non l’elenco dei membri del gruppo. Se si desidera visualizzare i membri del gruppo elencati qui, fare clic su Salva modifiche, quindi fare clic sul nome del profilo della scheda attività appena creato.
   >* Al termine di questi passaggi, il profilo scheda attività genera fogli presenze solo per gli utenti o i membri del gruppo assegnati che non dispongono di fogli presenze per il periodo corrente.


1. Fai clic su **Salva modifiche**.

   La prima volta che il profilo della scheda attività genera fogli presenze, vengono creati 2 fogli presenze per ogni utente. Dopo di che, ogni volta che genera nuovi fogli presenze, viene creata una scheda attività per utente.

   <!--the content in the table above will need to match the content in the Create timesheets article-->

## Limitazioni per l&#39;assegnazione di un profilo della scheda attività da parte di un amministratore di gruppo {#limitations-for-a-group-administrator-assigning-a-timesheet-profile}

Se si è un amministratore di gruppo e l&#39;opzione di accesso amministrativo Pagine e ore è disabilitata a livello di accesso, è possibile creare profili della scheda attività, ma è possibile assegnarli solo a:

* Gruppi da amministrare
* Singoli utenti a cui hai accesso per modificare appartenenti a un gruppo da amministrare

Per questi gruppi e utenti, non sarà possibile accedere ai fogli presenze generati dal profilo della scheda attività.

Inoltre, se l&#39;opzione Amministratore utente (Utenti del gruppo) è disabilitata anche nel livello di accesso, è possibile assegnare il profilo della scheda attività a un gruppo che si amministra, ma influisce solo sugli utenti del gruppo a cui si ha accesso per la modifica. Se il gruppo contiene utenti a cui non è possibile accedere per la modifica, non viene assegnato loro il profilo della scheda attività insieme al resto del gruppo.

Per informazioni sull&#39;opzione Fascicolo e orario nel livello di accesso, vedi [Consentire agli utenti l&#39;accesso amministrativo a determinate aree](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

Per informazioni sull’opzione Amministratore utente (Utenti del gruppo) nel livello di accesso, consulta [Concedere l’accesso agli utenti](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

## Profili attività ricorrenti

È possibile avere più di un profilo scheda attività per la propria organizzazione se sono presenti:

* Periodi di pagamento univoci per diversi set di utenti
* Approvatori unici per diversi set di utenti
* Requisiti unici dell&#39;orario generale per diversi gruppi di utenti

Un utente non può essere associato a più di un profilo della scheda attività alla volta. 
