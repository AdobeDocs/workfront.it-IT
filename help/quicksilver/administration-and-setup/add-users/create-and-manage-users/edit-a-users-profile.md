---
title: Modificare il profilo di un utente
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: In qualità di amministratore di Adobe Workfront, puoi creare nuovi utenti e gestire i profili di quelli esistenti.
author: Courtney, Alina
feature: System Setup and Administration
role: Admin
exl-id: 0343fe74-1be4-43e2-9e3d-8aa1f7ea26fa
source-git-commit: fed4713d1e9044879db6d34dc4725245a2516634
workflow-type: tm+mt
source-wordcount: '2786'
ht-degree: 0%

---

# Modificare il profilo di un utente


>[!IMPORTANT]
>
>La procedura descritta in questa pagina si applica solo alle organizzazioni che non sono ancora state integrate nell’Admin Console. Se l’organizzazione è stata configurata per Adobe Admin Console, devi eseguire questa azione tramite Adobe Admin Console.
>
>Per istruzioni su come modificare il profilo di un utente in Adobe Admin Console, consulta la sezione &quot;Modifica i dettagli utente&quot; nell’articolo [Gestire gli utenti individualmente](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) oppure contatta l’amministratore Adobe Admin Console.
>
>Per un elenco delle procedure che variano a seconda che l’organizzazione sia stata caricata in Adobe Admin Console, consulta [Differenze di amministrazione basate su piattaforma (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

In qualità di amministratore di Adobe Workfront, puoi creare nuovi utenti e gestire i profili di quelli esistenti. Per informazioni sulla creazione degli utenti, consulta [Aggiungi utenti](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

Gli utenti con una licenza Plan possono inoltre creare e gestire gli utenti. Per informazioni sull&#39;accesso necessario per modificare gli utenti, vedi [Concedere l’accesso agli utenti](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso</td> 
   <td> <p>Devi disporre di una delle seguenti caratteristiche:</p> 
    <ul> 
     <li> <p>Livello di accesso amministratore di sistema. Per informazioni, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente pieno accesso amministrativo</a>. </p> </li> 
     <li> <p><b>Utenti</b> impostazione nel livello di accesso configurato per <b>Modifica</b> accesso, con <b>Crea</b> e almeno uno dei due <b>Amministratore utente</b> opzioni attivate in <b>Ottimizzare le impostazioni</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Di queste due opzioni, se Utente <b>Amministratore (utenti del gruppo)</b> è abilitato, devi essere un amministratore di gruppo di un gruppo in cui l’utente è membro.</p> <p>Per ulteriori informazioni sulla <b>Utenti</b> impostazione in un livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Concedere l’accesso agli utenti</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Modificare un profilo utente

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Utenti** ![](assets/users-icon-in-main-menu.png).
1. Seleziona l’utente, quindi fai clic sull’icona Modifica ![](assets/edit-icon.png).

1. In **Modifica utente** casella visualizzata, modificare le seguenti informazioni, quindi fare clic su **Salva modifiche**:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Informazioni personali </td> 
      <td> 
       <ul> 
        <li><b>Nome</b>, <b>Cognome</b></li> 
        <li> <p><b>Indirizzo e-mail:</b> L’indirizzo e-mail di un utente è anche il loro nome utente in Workfront. Questo campo è sensibile a maiuscole e minuscole e deve essere univoco. Se un utente tenta di aggiungere un indirizzo e-mail non univoco 3 volte all’interno di una finestra di 10 minuti, viene visualizzata una risposta reCAPTCHA.</p> <p>Se utilizzi l’inserire nell'elenco Consentiti e-mail e immetti un dominio e-mail non presente nell’elenco, l’utente non riceverà notifiche e-mail. Per ulteriori informazioni sull'inserire nell'elenco Consentiti, vedi <a href="../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md" class="MCXref xref">Configurare l’inserire nell'elenco Consentiti e-mail</a>.</p> </li> 
        <li> <p><b>Ripristina password</b>: Fai clic su questo collegamento per reimpostare la password dell’utente. Prima di reimpostare la password di un utente, viene richiesto di specificare la password.</p> <p>Per reimpostare la password di un altro utente, è necessario essere un amministratore di Workfront o un amministratore di gruppo.</p> <p><b>NOTA</b>:  
          <ul> 
           <li> <p>Se sei un amministratore di gruppo, puoi reimpostare le password solo per gli utenti dei gruppi in cui sei designato come tale. Inoltre, l’autorizzazione Amministratore utenti (Utenti gruppo) deve essere abilitata nel livello di accesso:</p> <p> <img src="assets/group-admin-user.png" > </p> <p>Questa impostazione è disabilitata per impostazione predefinita. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </li> 
           <li> <p>Non è possibile reimpostare la password di un amministratore Workfront.</p> </li> 
          </ul> </p> </li> 
        <li><b>&lt;sso configuration=""&gt; Nome utente</b>: Se l'amministratore Workfront ha abilitato un'integrazione SSO con Workfront, in questo campo viene visualizzato il nome utente SSO. In questo campo è visibile il tipo di configurazione SSO abilitata per l’istanza Workfront. </li> 
        <li> <p><b>OnlyAllow &lt;sso configuration=""&gt; Autenticazione</b>: Se l’amministratore Workfront ha abilitato un’integrazione SSO con Workfront e ha aggiornato tutti gli utenti per SSO, questo campo è selezionato per impostazione predefinita. In questo campo è visibile il tipo di configurazione SSO abilitata per l’istanza Workfront.</p> <p>Quando questo campo è selezionato, l’utente deve accedere a Workfront con le proprie credenziali SSO. Deselezionando questa opzione, gli utenti potranno accedere a Workfront con le proprie credenziali Workfront.</p> <p>Per ulteriori informazioni sulla configurazione di Workfront con una soluzione SSO, vedi <a href="../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md" class="MCXref xref">Panoramica del single sign-on in Adobe Workfront</a></p> <p>Per ulteriori informazioni sull'aggiornamento degli utenti per SSO, vedi <a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref">Aggiornare gli utenti per il single sign-on</a>.</p> <p><b>NOTA</b>: Se sei un amministratore di gruppo, puoi modificare il &lt;sso configuration=""&gt; campi solo per gli utenti dei gruppi in cui sei designato come tale. Inoltre, l’autorizzazione Amministratore utente (Utenti del gruppo) deve essere abilitata nel livello di accesso.
        <p>Se sei un amministratore di gruppo e disponi dell’autorizzazione Amministratore utente (tutti gli utenti) abilitata nel tuo livello di accesso, puoi modificare il &lt;sso configuration=""&gt; campi per tutti gli utenti.</p> </li> 
        <li><b>Informazioni processo:</b> Informazioni sul lavoro, come il titolo del lavoro, e di quale area di competenza è responsabile l'utente.</li> 
        <li><p><b>Informazioni contatto</b>: Numero di telefono e indirizzo dell'utente.</p>
        <p>Se l’utente è abilitato per Unified User Management (UUM) o Adobe Identity Management System (IMS), la variabile <b>Paese</b> nella sezione Informazioni contatto accetta solo i valori del codice del paese (ad esempio, US, GB, IN).</p></li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Preferenze </td> 
      <td> 
       <ul> 
      <li> <p><b>Fuso orario:</b> Il fuso orario dell’utente.</p> <p>Per informazioni su come aiutare gli utenti a collaborare in Workfront nei diversi fusi orari, vedi <a href="../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md" class="MCXref xref">Utilizzo di fusi orari diversi</a>.</p> </li> 
       <li><b>Impostazioni internazionali e-mail</b>: Le impostazioni internazionali e-mail preferite dell’utente. Questo influisce sul formato dei numeri e delle date nelle e-mail provenienti da Workfront.</li>

   <li><b>Ricevi e-mail da questo ambiente di test</b>: Seleziona questa opzione se desideri ricevere notifiche e-mail dall’ambiente attualmente connesso.
      <p><b>NOTA</b></p>
      Questa opzione è disponibile solo negli ambienti Anteprima e Sandbox. Le notifiche e-mail sono abilitate nell’ambiente di produzione per impostazione predefinita. 
      </li>

   <li><b>Mostra percentuale di completamento allo stato dell'aggiornamento</b>: Selezionare questa opzione se si desidera visualizzare una barra della percentuale di completamento all'interno dell'area Aggiorna delle attività dell'utente.</li> 
       <li><b>Invia il lavoro da me assegnato alla scheda Lavoro</b>: Selezionare questa opzione se si desidera che tutto ciò che l'utente assegna a se stesso venga visualizzato direttamente nella scheda Attivato. L’impostazione predefinita consiste nell’elencare tutti gli elementi assegnati a un utente nella relativa scheda Richiesta di lavoro.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notifiche</td> 
      <td> <p>Seleziona le notifiche e-mail che devono essere abilitate per il nuovo utente.</p> <p>Puoi selezionare notifiche digest istantanee e giornaliere.</p> <p>Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref">Configurare le notifiche degli eventi per tutti gli utenti del sistema</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Accesso</td> 
      <td> 
       <ul> 
      <li><b>È attivo:</b> Selezionare questa casella per indicare che l’utente è attivo. Gli utenti attivi utilizzano una licenza Workfront. Se si deseleziona la casella, l’utente viene disattivato.</li> 
       <li> <p><b>Livello di accesso:</b> Selezionare il livello di accesso da assegnare all'utente.</p> 
       <p>Quando assegni un livello di accesso a un utente, puoi assegnare un livello uguale o inferiore al livello di accesso desiderato. Ad esempio, se il livello di accesso è Planner, non è possibile assegnare il livello di accesso Amministratore. Tuttavia, non è possibile assegnare un livello di accesso che per impostazione predefinita è inferiore al proprio livello di accesso se l’amministratore di Workfront ha abilitato autorizzazioni non predefinite sul livello di accesso che non sono abilitate anche nel proprio livello di accesso (tramite le impostazioni di fine tuning, come descritto in <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>). </p> 
       <p>Per ulteriori informazioni sui livelli di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Configurare l’accesso ad Adobe Workfront</a>.</p> </li> 
       <li> <p><b>Modello di layout</b>: Scegliere un modello di layout per l’utente. Questo modello di layout ha la precedenza su qualsiasi modello di layout assegnato al gruppo principale, al team principale o al ruolo di lavoro principale dell'utente. Per ulteriori informazioni sulla priorità di assegnazione dei modelli di layout, vedere <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Creare e gestire modelli di layout</a>.</p> <p><b>NOTA</b>:  <p>L’elenco dei modelli disponibili in questo campo dipende dall’accesso:</p> 
       <ul> 
       <li>In qualità di amministratore di Workfront, puoi visualizzare tutti i modelli di layout a livello di sistema e di gruppo.</li> 
       <li>In qualità di amministratore del gruppo, è possibile visualizzare il modello di layout a livello di sistema e quelli associati ai gruppi gestiti.</li> 
       <li>In qualità di utente con licenza Pianifica e accesso per modificare gli utenti, è possibile visualizzare solo i modelli di layout a livello di sistema.</li> 
       </ul> <p>Per ulteriori informazioni sui modelli di layout a livello di gruppo, consulta <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Creare e gestire modelli di layout</a>.</p> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Organizzazione </td> 
      <td> 
       <ul> 
      <li><b>Azienda</b>: Società dell'utente. Gli utenti possono essere associati a una sola società. È necessario creare una società prima di poterla associare a un utente. Nell’elenco vengono visualizzate solo le società attive. Per informazioni sulla creazione di aziende, consulta <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md" class="MCXref xref">Creare e modificare aziende</a>.</li> 
      <li><b>Report a:</b> Se hai specificato una società per l’utente, puoi anche specificare il gestore diretto dell’utente in questo campo. Un utente può avere un solo manager.</li> 
      <li><b>Rapporti diretti:</b> Se hai specificato una società per l’utente, puoi anche specificare i rapporti diretti dell’utente. Un utente può avere più rapporti diretti.</li> 
      <li><b>Team principale</b>: Specifica il team principale per l'utente. Gli utenti possono avere un solo team domestico.</li> 
      <li><b>Altri team</b>: Gli utenti possono appartenere a più team.</li> 
      <li> <p><b>Gruppo principale:</b> Selezionare un gruppo appropriato per assegnare l'utente. Questo consente all’utente di accedere agli oggetti condivisi con il gruppo.</p> <p>Questo campo è obbligatorio. Ogni utente deve essere associato a un gruppo home. Se non ne selezioni uno, il gruppo viene assegnato come gruppo home del nuovo utente.</p> <p><b>NOTA</b>: È possibile assegnare un gruppo a un utente solo se si è un amministratore Workfront, se si è l'amministratore del gruppo o se il gruppo è pubblico.</p> </li> 
      <li> <p><b>Altri gruppi</b>: Gli utenti possono appartenere a più gruppi. È possibile assegnare un gruppo a un utente solo se si è un amministratore Workfront, se si è l'amministratore del gruppo o se il gruppo è pubblico.</p> <p><b>IMPORTANTE</b>: L’aggiunta di un utente a più di 100 gruppi può causare problemi di prestazioni in qualsiasi area di Workfront che carica l’elenco dei gruppi.</p> <p>Per ulteriori informazioni sui gruppi pubblici, vedi <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Creare un gruppo</a>.</p> <p>Per ulteriori informazioni sui gruppi, consulta <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Panoramica sui gruppi</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Pianificazione risorse </td> 
      <td> 
       <ul>
       <li>
       <b>Tempo di lavoro</b>: Rappresenta la percentuale del tempo equivalente a tempo pieno (FTE) disponibile per il lavoro effettivo, esclusi i costi comuni. Il tempo di lavoro deve essere un numero decimale fino a 1 e non può essere 0. Ad esempio, una disponibilità del 20% per il lavoro effettivo sarebbe 0,2.

   L’impostazione predefinita del campo è 1, a indicare che un utente spende l’intero FTE sul lavoro effettivo correlato al progetto.

   Il sistema utilizza questo numero per calcolare la disponibilità dell&#39;utente per il lavoro effettivo relativo al progetto.

   Per ulteriori informazioni sulla creazione di pianificazioni in Workfront, vedi <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Creare una pianificazione</a>.

   Le eccezioni di pianificazione e il tempo di inattività potrebbero influire anche sulla capacità dell&#39;utente.

   Workfront calcola la disponibilità di un utente in base alle preferenze di Gestione risorse nell’area Configurazione. Per ulteriori informazioni, consulta <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configurare le preferenze di Gestione risorse</a>.

   <b>SUGGERIMENTO</b>

   Impostare il valore Ora di lavoro su 1 per indicare che l’utente è disponibile per il lavoro relativo al progetto per l’intero equivalente a tempo pieno.
   </li> 
      <li> <b>Disattivazione programmata</b>: Selezionare questa casella se si desidera che l'utente venga disattivato dopo un periodo di tempo. </li> 
       <li><b>Data di disattivazione pianificata</b>: Data dopo la quale l’utente viene disattivato. Per informazioni sulla pianificazione degli utenti per la disattivazione, consulta la sezione <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">Pianificare gli utenti per la disattivazione</a> in <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Disattivare o riattivare un utente</a>.</li> 
       <li> <p><b>Ruolo principale</b>: Si tratta del ruolo principale che l’utente può svolgere in Workfront. A questo ruolo viene assegnato anche ogni attività e problema a cui l’utente è assegnato. I ruoli di lavoro sono essenziali nella gestione delle risorse. È possibile aggiornare questo campo solo se si dispone di una licenza Plan con accesso amministrativo per gli utenti o se si è un amministratore Workfront. Per ulteriori informazioni sulla configurazione degli utenti con accesso amministrativo agli utenti, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Concedere l’accesso agli utenti</a>.</p> <p>Nell’elenco vengono visualizzati solo i ruoli di lavoro attivi. </p> </li> 
       <li>Se hai selezionato un <b>Ruolo principale</b>, <b>Percentuale di disponibilità FTE</b> viene visualizzato il campo . Specificare la percentuale di tempo della pianificazione dell'utente allocata a questo ruolo di lavoro. Il valore predefinito per la percentuale di disponibilità FTE per il ruolo principale è 100%. </li> 
       <li> <p><b>Altri ruoli</b>: Un utente può avere più ruoli di lavoro in Workfront. I ruoli di lavoro sono essenziali nella gestione delle risorse. Non vi è alcun limite per il numero di ruoli di lavoro che un utente può svolgere. Tuttavia, consigliamo di non assegnare un utente a un numero eccessivo di ruoli di lavoro, perché la gestione delle risorse potrebbe diventare troppo complessa per questi utenti.<p>Nell’elenco vengono visualizzati solo i ruoli di lavoro attivi. Per ulteriori informazioni sui ruoli di lavoro, consulta <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Creare e gestire ruoli di lavoro</a>.</p> <p>È possibile aggiornare questo campo solo se si dispone di una licenza Plan con accesso amministrativo per gli utenti o se si è un amministratore Workfront. <br>Per ulteriori informazioni sulla configurazione degli utenti con accesso amministrativo agli utenti, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Concedere l’accesso agli utenti</a>.</p> </li> 
       <li> <p>(Condizionale) Se hai selezionato uno o più <b>Altri ruoli</b>, <b>Percentuale di disponibilità FTE</b> viene visualizzato un campo per ciascun ruolo. Specificare la percentuale di tempo della pianificazione dell'utente allocata a ciascun ruolo di lavoro. Il valore predefinito per la percentuale di disponibilità FTE per gli altri ruoli è 0%.</p> <p><b>NOTA</b>: Se la disponibilità di altri ruoli è pari a 0%, questi non vengono visualizzati nel Planner risorse, a meno che gli utenti non siano assegnati a attività in questi ruoli.</p> <p> <img alt="user_settings_role_and_dte_boxes_rp_story.png" src="assets/user-settings-roles-and-dte-boxes-rp-story.png"> </p> <p><b>NOTA</b>: <p>La somma di tutti <b>Percentuali di disponibilità FTE</b> per tutti i ruoli deve essere uguale a 100%. Ogni percentuale di disponibilità FTE calcola le ore disponibili per ogni ruolo per utente nel Resource Planner. L’orario disponibile per ogni ruolo per utente dipende dal tempo disponibile per l’utente.</p> <p>Il tempo disponibile per l’utente viene calcolato da Workfront in base al metodo selezionato dall’amministratore Workfront per calcolare l’ETP nelle Preferenze di gestione delle risorse.</p> <p>Per informazioni sul calcolo della disponibilità per l'utente, vedere <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Panoramica del calcolo delle ore e degli FTE per utenti e ruoli nel Planner risorse</a>.</p> <p>Per informazioni sulla configurazione delle preferenze di Gestione risorse, consulta <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configurare le preferenze di Gestione risorse</a>.</p> </p> </li> 
       <li> <p><b>Pianificazione</b>: Associa una pianificazione all'utente. La pianificazione dell'utente calcola la cronologia delle attività a cui l'utente è assegnato.</p> <p>È necessario creare una pianificazione prima di poterla associare a un utente. Per ulteriori informazioni sulla creazione delle pianificazioni, consulta <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Creare una pianificazione</a>.</p> <p><b>NOTA</b>: È consigliabile che la pianificazione associata all’utente corrisponda al fuso orario dell’utente.</p> </li> 
       <li> <p><b>Profilo scheda attività</b>: Associare un profilo foglio presenze all'utente per garantire che i fogli presenze vengano generati automaticamente per l'utente.</p> <p><b>NOTA</b>: L’elenco dei profili disponibili in questo campo dipende dall’accesso:
       <ul>
       <li>In qualità di amministratore di Workfront, è possibile visualizzare tutti i profili a livello di sistema e tutti i profili a livello di gruppo della scheda attività.</li>
       <li>In qualità di amministratore di gruppo, è possibile visualizzare i profili a livello di sistema e quelli associati ai gruppi gestiti.</li>
       <li>In qualità di utente con licenza Pianifica e accesso per modificare gli utenti, è possibile visualizzare solo i profili a livello di sistema della scheda attività. Per ulteriori informazioni sui profili della scheda attività a livello di gruppo, vedere <a href="../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md" class="MCXref xref">Creare, modificare e assegnare profili della scheda attività</a>.</li>
      </ul></p> </li> 
       <li><b>Tipo orario predefinito</b>: Seleziona il tipo di ora predefinito per l’utente. Questo è il tipo di ora utilizzato per impostazione predefinita quando l’utente registra il tempo.</li> 
       <li><b>Tipi di ora disponibili</b>: Seleziona i tipi di ora che devono essere disponibili per l’utente. Questi tipi di ora sono visibili ovunque in Workfront, dove l’utente può registrare il tempo. Un utente può visualizzare solo i tipi di ora abilitati a livello di progetto e a livello di utente. Per ulteriori informazioni sui tipi di ora disponibili per gli utenti, consulta <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">Definire i tipi di ora e la disponibilità per i fogli presenze</a>.</li> 
       <li><b>Ora di accesso:</b> Selezionare se l'utente deve registrare l'ora degli elementi di lavoro in ore o giorni. Per ulteriori informazioni, consulta <a href="../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md" class="MCXref xref">Configura se l'ora è registrata in ore o giorni</a>.</li>

   <li> <b>FTE</b>: È l'equivalente a tempo pieno dell'utente. Workfront utilizza questo numero per calcolare la disponibilità dell'utente in base alla pianificazione predefinita solo quando le preferenze di gestione delle risorse a livello di sistema sono impostate su La pianificazione predefinita.

   <p>L’FTE indica la quantità di tempo che l’utente può trascorrere al lavoro. Ciò include i costi comuni e il tempo impiegato per il lavoro del progetto. Ad esempio, il tempo trascorso nelle riunioni o la formazione è incluso anche nell’ETP.</p>

   L’ETP deve essere un numero decimale massimo di 1 e non può essere 0. Ad esempio, se il valore FTE è 0,5 e la pianificazione predefinita in Workfront è 40 ore, l’utente è disponibile per 20 ore alla settimana.

   Il valore predefinito del campo è 1.

   È possibile che le eccezioni programmate, i tempi di inattività e il valore del tempo di lavoro influiscano sulla disponibilità dell&#39;utente.

   Workfront calcola la disponibilità di un utente in base alle preferenze di Gestione risorse nell’area Configurazione.

   Se le preferenze di gestione delle risorse a livello di sistema sono impostate su Pianificazione dell&#39;utente, il valore specificato viene ignorato e l&#39;utente viene considerato disponibile in base a quanto specificato nella relativa pianificazione.

   Per ulteriori informazioni, consulta <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configurare le preferenze di Gestione risorse</a>.

   Per ulteriori informazioni sulla creazione di pianificazioni in Workfront, vedi <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Creare una pianificazione</a>.
   </li>

   <li><b>Pool di risorse</b>: Associa l’utente ai pool di risorse. Per ulteriori informazioni, consulta <a href="../../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md" class="MCXref xref">Associare pool di risorse con gli utenti </a>.</li> 
        <li><b>Costo/ora</b>: Importo del costo all'ora per l'utente. </li> 
        <li><b>Fatturazione per ora</b>: La quantità di fatturazione all'ora per l'utente.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Moduli personalizzati</td> 
      <td>Associa un modulo personalizzato utente esistente a questo utente. È necessario creare un modulo personalizzato prima di poterlo associare a un utente. Nell’elenco vengono visualizzati solo i moduli personalizzati attivi. Per informazioni sulla creazione di moduli personalizzati, vedere <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Creare o modificare un modulo personalizzato</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Commento</td> 
      <td> <p>Digita il commento da inviare agli utenti e all’area Aggiornamenti dei loro profili utente.</p> </td> 
     </tr> 
    </tbody> 
   </table>
