---
user-type: administrator
product-area: system-administration;user-management
keywords: gruppo,preferenze,attività,gruppi,problema,sblocca
navigation-topic: create-and-manage-groups
title: Configurare le preferenze di Ore e Timesheet per un gruppo
description: A livello di sistema, un amministratore Adobe Workfront può sbloccare le sezioni delle preferenze relative a schede orario e ore Preferenze generali e Precompila schede orario con. Questo consente agli amministratori di gruppi di configurare le opzioni in tali sezioni in modo indipendente per i propri gruppi.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 1ee9343e-9452-4e41-a9ff-a6c865d4813b
source-git-commit: a42a167447d2f11b5502e4a0953b5e7eec2e67b1
workflow-type: tm+mt
source-wordcount: '1336'
ht-degree: 1%

---

# Configurare le preferenze di orario e scheda orario per un gruppo

Un amministratore di Adobe Workfront può sbloccare le seguenti sezioni delle preferenze delle schede orario e delle ore a livello di sistema in modo che gli amministratori dei gruppi possano configurarle in modo indipendente per i propri gruppi:

* Preferenze generali
* Dove gli utenti possono registrare le ore
* Precompila schede orario

Se al di sopra del gruppo gestito sono presenti gruppi, anche gli amministratori possono eseguire questa operazione per il gruppo. Lo stesso vale per gli amministratori di Workfront (per qualsiasi gruppo).

Le sezioni seguenti della pagina Preferenze scheda orario e ore sono configurabili solo a livello di sistema e non possono essere sbloccate per i gruppi:

* Progetti, attività e problemi eliminati

Per informazioni su come un amministratore di Workfront sblocca una preferenza di tipo scheda orario e ora, vedere la sezione [Sbloccare le preferenze di tipo scheda orario e ora per i gruppi](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md#lock) nell&#39;articolo [Configurare le preferenze di tipo scheda orario e ora](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

>[!TIP]
>
>La configurazione a livello di gruppo è possibile anche per le preferenze del progetto e per le preferenze di attività e problemi. Per informazioni, consulta [Configurare le preferenze del progetto per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) e [Configurare le preferenze per attività e problemi per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

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
   <td><p>Standard</p>
       <p>Piano</p></td>
  </tr>
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td>Devi essere un amministratore di gruppo del gruppo o un amministratore di sistema.</td>
  </tr>
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Raggruppa le preferenze di orario e scheda orario

Considera le seguenti informazioni sulla configurazione di una scheda orario sbloccata o di una preferenza orario per un gruppo:

* Se si è un amministratore gruppo e si configura una preferenza di tipo Scheda orario o Ora per il gruppo, questa modifica avrà effetto sugli utenti che utilizzano il gruppo come Gruppo predefinito.
* In genere, una preferenza sbloccata rimane sbloccata a tempo indeterminato. Se l&#39;amministratore di Workfront la sblocca nuovamente, l&#39;impostazione di sistema riprende ad avere effetto e le impostazioni relative alle preferenze impostate dagli amministratori di gruppo andranno perse.
* Una scheda orario eredita le preferenze della scheda orario e delle ore configurate per il Gruppo predefinito del proprietario della scheda orario.

  <!--
  Add example here?
  -->

* Dopo che un amministratore di Workfront sblocca una preferenza a livello di sistema e la configuri per il gruppo, puoi bloccarla per garantire che tutti gli utenti dei gruppi sottostanti utilizzino la stessa configurazione. Ciò è parallelo alla possibilità che un amministratore di Workfront deve configurare e bloccare una preferenza per tutti gli utenti del sistema. Per ulteriori informazioni, vedere [Bloccare o sbloccare una scheda orario e una preferenza orario di gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-timesheet-hour-preference.md).

## Configurare una preferenza per schede orario o ore sbloccate per un gruppo

>[!TIP]
>
>Se sei un amministratore di Workfront, puoi saltare i passaggi 1-4 da Configurazione > Scheda orario e ore > Preferenze, quindi cercare il nome del gruppo nella casella nella parte superiore della pagina.

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Gruppi** ![Gruppi](assets/groups-icon.png).

1. Fai clic sul nome del gruppo di cui desideri configurare le preferenze per le ore o la scheda orario.
1. Nel pannello a sinistra, fai clic su **Schede orario e ore**.

1. Nella pagina visualizzata, nella sezione **Preferenze generali** configura una delle seguenti opzioni:

   >[!TIP]
   >
   >Se passi il cursore del mouse su una preferenza e viene visualizzato un suggerimento che informa che è bloccata, puoi chiedere all’amministratore di Workfront di sbloccarla per tutti i gruppi dell’organizzazione.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Tempo di connessione per date future</td> 
      <td> <p>Consente agli utenti di registrare le ore per le date future in tutto il sistema in:</p> 
       <ul> 
       <li>Tutti i progetti, le attività e i problemi a cui hanno accesso in tempo di registro, indipendentemente dal gruppo del progetto</li> 
       <li>Le loro schede orario come Ora generale</li>
       </ul> 
       <p>Questa funzione è utile quando gli utenti hanno intenzione di allontanarsi dall’ufficio e desiderano registrare in anticipo l’ora.</p> 
       <p><b>NOTA</b>: non è possibile impedire agli utenti di registrare il tempo per attività o problemi chiusi o annullati. Puoi impedire agli utenti di registrare solo il tempo su progetti completi o inattivi. È consigliabile utilizzare i filtri negli elenchi di attività e problemi per escludere che quelli completati o annullati siano visibili agli utenti.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aggiungi spese da una scheda orario</td> 
      <td> <p>Consente agli utenti di registrare tempo e spese nella scheda orario.</p> 
      <p>Quando questa preferenza è abilitata per un gruppo e il gruppo è impostato come gruppo predefinito per alcuni utenti, accanto ai progetti e alle attività viene visualizzata un'icona di spesa nelle schede attività di tali utenti. Gli utenti possono fare clic su questa icona per aggiungere o modificare le spese per il progetto o l'attività.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Assegna mansioni alle ore manualmente</td> 
      <td> <p>Consenti agli utenti di selezionare manualmente qualsiasi Ruolo assegnato nel loro profilo utente o assegnato all'oggetto.</p> <p><b>IMPORTANTE</b>:  
        <ul> 
         <li>Se disattivi questa impostazione dopo aver assegnato i ruoli alle voci orarie, gli utenti devono regolare le ore registrate in vari ruoli nella scheda Ore del progetto, dell’attività o del problema.</li> 
         <li>Se all'utente non è stata assegnata una mansione nel profilo e nella finestra di dialogo Assegnazioni avanzate è stata assegnata un'attività come Proprietario dell'attività, tale mansione viene visualizzata quando l'utente accede all'attività.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Limita la modifica della scheda orario a proprietari e amministratori</td> 
      <td> <p>Limita la modifica ai proprietari delle schede orario, indipendentemente dal gruppo del progetto e dagli amministratori di Workfront. Se questa opzione è disabilitata, le schede orario possono anche essere modificate da:</p> 
       <ul> 
        <li> <p>Utenti con accesso amministrativo a schede orario e ore nel proprio livello di accesso</p> </li> 
        <li> <p>Approvatori schede orario se nella scheda orario è abilitato "Può modificare le ore"</p> </li> 
        <li> <p>Manager del proprietario della scheda orario</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Limita la modifica delle ore a proprietari e amministratori</td> 
      <td>Limita la modifica all’utente che ha inserito le ore e agli amministratori di Workfront. Questa impostazione si applica alla scheda Ore in un progetto o in un rapporto Ore.</td> 
     </tr> 
    </tbody> 
   </table>

1. Nella sezione **Dove gli utenti possono registrare l&#39;ora**, configura una delle seguenti opzioni:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader">Registra tempo direttamente sui progetti</td> 
      <td>Consente agli utenti di registrare il tempo sul progetto (sia nella scheda Aggiornamenti che nella scheda orario). Se desideri limitare il tempo di registrazione degli utenti a livello di progetto, lascia deselezionata questa opzione.</td>
     </tr>
     <tr>
      <td role="rowheader">Tempo di connessione per i progetti completati</td>
      <td>Consente agli utenti di registrare il tempo su un progetto contrassegnato come completato. Se questa opzione è disattivata, gli utenti non possono registrare il tempo per il lavoro completato sui progetti nello stato Completato.</td>
     </tr>
     <tr>
      <td role="rowheader">Registra tempo su progetti inattivi</td> 
      <td>Quando questa opzione è abilitata, gli utenti possono registrare le ore sui progetti con uno stato Dead (Inattivo).</td>
     </tr>
    </tbody>
   </table>

   >[!NOTE]
   >
   >Questa preferenza viene applicata in base alla configurazione delle preferenze del Gruppo Predefinito dell&#39;utente. Se queste impostazioni sono abilitate nelle preferenze del Gruppo predefinito dell’utente, quest’ultimo potrà registrare il tempo direttamente sui progetti, compresi quelli completati o inattivi, indipendentemente dal fatto che le preferenze di gruppo del progetto lo consentano o meno.

1. Nella sezione **Precompila schede orario**, configura una delle seguenti opzioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Lavoro che si trova entro &lt;numero di settimane&gt; dell’intervallo di lavoro della scheda orario</td> 
      <td> <p>Definisce il numero di settimane precedenti e successive all'intervallo di date della scheda orario contenente le date delle attività e delle Issues assegnate all'utente. L’impostazione predefinita è 1 settimana e puoi estendere questo intervallo a 4 settimane. Ciò significa che la scheda orario è precompilata con attività e problemi che hanno date comprese tra quattro settimane prima dell’intervallo di date della scheda orario e fino a quattro settimane dopo l’intervallo di date della scheda orario, se selezioni 4 settimane per l’intervallo. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Attività e problemi completati</td> 
      <td>Se a una singola attività vengono in genere assegnate più risorse, si consiglia questa impostazione. Ciò significa che quando una risorsa registra il tempo relativo all’attività e la contrassegna come completata, le altre risorse assegnate all’attività possono ancora trovare l’attività o il problema nella propria scheda orario, per registrare le proprie ore.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Attività e problemi con date pianificate nell'intervallo date della scheda orario</td> 
      <td> <p>Se selezionata, la scheda attività include attività e problemi con una Data inizio pianificata o una Data completamento compresa nell'intervallo di date della scheda attività.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> Attività con date previste nell'intervallo date della scheda orario</td> 
      <td> <p>Se questa opzione è selezionata, la scheda attività include attività con una data di inizio prevista o una data di completamento compresa nell'intervallo di tempo del progetto, anche se la data pianificata del problema o dell'attività non rientra nell'intervallo di date della scheda attività.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Salva**.
