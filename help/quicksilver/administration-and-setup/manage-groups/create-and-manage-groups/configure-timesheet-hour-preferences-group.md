---
user-type: administrator
product-area: system-administration;user-management
keywords: gruppo, preferenze, compito, gruppi, problema, sblocca
navigation-topic: create-and-manage-groups
title: Configurare le preferenze relative a schede attività e ora per un gruppo
description: A livello di sistema, un amministratore di Adobe Workfront può sbloccare le sezioni relative alle preferenze relative alla scheda attività e alle ore con Preferenze generali e Precompilazione fogli preselezionati. Questo consente agli amministratori di gruppo di configurare le opzioni in tali sezioni in modo indipendente per i propri gruppi.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 1ee9343e-9452-4e41-a9ff-a6c865d4813b
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1203'
ht-degree: 5%

---

# Configurare le preferenze relative a schede attività e ora per un gruppo

Un amministratore di Adobe Workfront può sbloccare le sezioni seguenti delle preferenze relative alla scheda attività e alle ore a livello di sistema, in modo che gli amministratori dei gruppi possano configurarle in modo indipendente per i propri gruppi:

* Preferenze Generali
* Precompila le schede orario con

Se ci sono gruppi al di sopra del gruppo che gestisci, i loro amministratori possono farlo anche per il tuo gruppo. Lo stesso vale per gli amministratori di Workfront (per qualsiasi gruppo).

Le sezioni seguenti nella pagina Preferenze scheda attività e ora sono configurabili solo a livello di sistema e non possono essere sbloccate per i gruppi:

* Tempo di registrazione
* Preferenze per l&#39;eliminazione di progetti, attività o problemi

Per informazioni su come un amministratore di Workfront sblocca una scheda attività e una preferenza oraria, consulta la sezione . [Sblocca le preferenze della scheda attività e dell&#39;ora per i gruppi](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md#lock) nell&#39;articolo [Configurare le preferenze relative a schede attività e ora](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

>[!TIP]
>
>La configurazione a livello di gruppo è possibile anche per le preferenze del progetto e per le preferenze relative a attività ed emissioni. Per informazioni, consulta [Configurare le preferenze di progetto per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) e [Configurare le preferenze per attività e problemi per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Workfront*</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> <p>È necessario essere un amministratore del gruppo o un amministratore di Workfront. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Amministratori di gruppo</a> e <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente pieno accesso amministrativo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano o tipo di licenza hai, contatta il tuo amministratore Workfront.

## Raggruppa le preferenze relative alla scheda attività e all&#39;ora

Considera le seguenti informazioni sulla configurazione di una scheda attività o di una preferenza ora sbloccata per un gruppo:

* Se si è un amministratore di gruppo e si configura una scheda attività o una preferenza oraria per il gruppo, questo interesserà le persone che utilizzano il gruppo come gruppo principale.
* In genere, una preferenza sbloccata rimane sbloccata a tempo indeterminato. Se l’amministratore di Workfront lo blocca nuovamente, l’impostazione di sistema ha effetto nuovamente e le impostazioni relative alle preferenze effettuate dagli amministratori del gruppo vengono perse.
* Una scheda attività eredita le preferenze relative alla scheda attività e all&#39;ora configurate per il gruppo home del proprietario della scheda attività.

   <!--
  Add example here?
  -->

* Dopo che un amministratore di Workfront sblocca una preferenza a livello di sistema e la configura per il gruppo, puoi bloccarla per assicurarti che tutti i gruppi sotto di te utilizzino la stessa configurazione. Ciò è parallelo alla possibilità che un amministratore di Workfront debba configurare e bloccare una preferenza per tutti gli utenti del sistema. Per ulteriori informazioni, consulta [Bloccare o sbloccare una scheda attività e una preferenza ora del gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-timesheet-hour-preference.md).

## Configurare una scheda attività o una preferenza ora sbloccata per un gruppo

>[!TIP]
>
>Se sei un amministratore di Workfront, puoi ignorare i passaggi 1-4 andando su Configurazione > Scheda attività e ore > Preferenze, quindi cercando il nome del gruppo nella casella nella parte superiore della pagina.

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **Gruppi** ![](assets/groups-icon.png).

1. Fare clic sul nome del gruppo di cui si desidera configurare le preferenze relative alla scheda attività o all&#39;ora.
1. Nel pannello a sinistra, fai clic su **Tempi e ore**.

1. Nella pagina visualizzata, nella **Preferenze generali** configura una delle seguenti opzioni:

   >[!TIP]
   >
   >Se passi il puntatore del mouse su una preferenza e viene visualizzata una descrizione comandi che indica che è bloccata, puoi chiedere all’amministratore di Workfront di sbloccarla per tutti i gruppi dell’organizzazione.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Registra ore per le date future</td> 
      <td> <p>Consente agli utenti di registrare l’ora per le date future in tutto il sistema in:</p> 
       <ul> 
       <li>Qualsiasi progetto, attività e problemi a cui hanno accesso al tempo di log, indipendentemente dal gruppo del progetto</li> 
       <li>I fogli presenze come ora generale</li>
       </ul> 
       <p>Questo è utile quando gli utenti hanno intenzione di essere lontani dall'ufficio e vogliono registrare quel tempo in anticipo.</p> 
       <p><b>NOTA</b>: Non è possibile impedire agli utenti di registrare il tempo su attività o problemi chiusi o annullati. È possibile solo impedire agli utenti di registrare il tempo su progetti completi o morti. È consigliabile utilizzare i filtri negli elenchi di attività e problemi per escludere quelli completati o annullati dalla visualizzazione degli utenti.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aggiungi le spese da una scheda orario</td> 
      <td> <p>Consente agli utenti di registrare il tempo e le spese nella scheda attività.</p> 
      <p>Quando questa preferenza è abilitata per un gruppo e il gruppo è impostato come gruppo principale per alcuni utenti, accanto ai progetti e alle attività nelle schede attività di tali utenti viene visualizzata un'icona di spesa. Gli utenti possono fare clic su questa icona per aggiungere o modificare le spese per il progetto o l'attività.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Assegna mansioni alle ore manualmente</td> 
      <td> <p>Consente agli utenti di selezionare manualmente qualsiasi Ruolo processo assegnato nel profilo utente o assegnato all’oggetto.</p> <p><b>IMPORTANTE</b>:  
        <ul> 
         <li>Se si disabilita questa impostazione dopo aver assegnato i ruoli di lavoro alle voci dell'ora, gli utenti devono regolare le ore registrate con vari ruoli nella scheda Ore del progetto, dell'attività o del problema.</li> 
         <li>Se l'utente non dispone di un ruolo di lavoro assegnato nel proprio profilo ed è presente un'attività assegnata come Proprietario attività nella finestra di dialogo Assegnazioni avanzate, tale ruolo viene visualizzato quando l'utente accede al tempo dell'attività.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Limita la modifica della scheda orario a proprietari e amministratori</td> 
      <td> <p>Limita la modifica ai proprietari della scheda attività, indipendentemente dal gruppo del progetto e dagli amministratori Workfront. Quando questa opzione è disabilitata, le schede attività possono essere modificate anche da:</p> 
       <ul> 
        <li> <p>Utenti con accesso amministrativo a schede e ore nel loro livello di accesso</p> </li> 
        <li> <p>Gli approvatori della scheda attività se l'opzione "Può modificare le ore" è abilitata nella scheda attività</p> </li> 
        <li> <p>Il gestore del proprietario della scheda attività</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Limitare la modifica delle ore a proprietari e amministratori</td> 
      <td>Limita la modifica all'utente che ha inserito le ore e agli amministratori di Workfront. Questa impostazione si applica alla scheda Ore in un progetto o in un rapporto Ore .</td> 
     </tr> 
    </tbody> 
   </table>

1. In **Precompilazione dei fogli preselezionati con** configura una delle seguenti opzioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Lavoro all'interno di &lt;number of="" weeks=""&gt; dell'intervallo di lavoro della scheda attività</td> 
      <td> <p>Definisce il numero di settimane prima e dopo l'intervallo di date della scheda attività che contiene le date delle attività e dei problemi assegnati all'utente. L’impostazione predefinita è 1 settimana ed è possibile estendere questo intervallo a 4 settimane. Ciò significa che la scheda attività è precompilata con attività e problemi con date comprese tra quattro settimane prima dell'intervallo di date della scheda attività fino a quattro settimane dopo l'intervallo di date della scheda attività, se si seleziona 4 settimane per l'intervallo. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Attività e problemi completati</td> 
      <td>Se più risorse vengono generalmente assegnate a una singola attività, è consigliabile impostare questa opzione. Ciò significa che quando una risorsa registra il tempo rispetto all'attività e la contrassegna come completata, le altre risorse assegnate all'attività possono comunque trovare l'attività o il problema nella relativa scheda attività, per registrare le ore.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Attività e problemi con date pianificate nell'intervallo date della scheda orario</td> 
      <td> <p>Se selezionata, la scheda attività include le attività e i problemi che presentano una data di inizio pianificata o una data di completamento compresa nell'intervallo di date della scheda attività.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> Attività e problemi con date previste nell'intervallo date della scheda orario</td> 
      <td> <p>Se selezionata, la scheda attività include attività che presentano una data di inizio prevista o una data di completamento entro l'intervallo di tempo del progetto, anche se la data pianificata dell'emissione o dell'attività non rientra nell'intervallo di date della scheda attività.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Salva**.
