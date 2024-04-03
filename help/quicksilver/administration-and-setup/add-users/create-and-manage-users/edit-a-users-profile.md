---
title: Modificare il profilo di un utente
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: In qualità di amministratore di Adobe Workfront, puoi creare nuovi utenti e gestire i profili di quelli esistenti.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 0343fe74-1be4-43e2-9e3d-8aa1f7ea26fa
source-git-commit: 02d20209b8bf53c84308707a89a5abf399494b64
workflow-type: tm+mt
source-wordcount: '3334'
ht-degree: 0%

---

# Modificare il profilo di un utente

{{highlighted-preview}}

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on editing a user's profile in the Adobe Admin Console, see the section "Edit user details" in the article [Manage users individually](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) or contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
-->

In qualità di amministratore di Adobe Workfront, puoi creare utenti e gestire i profili di quelli esistenti. Per informazioni sulla creazione di utenti, consulta [Aggiungi utenti](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

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
   <td> <p>Nuovo: Standard</p>
   Oppure
   <p>Corrente: Piano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>È necessario disporre di uno dei seguenti elementi:</p> 
    <ul> 
     <li> <p>Livello di accesso Amministratore di sistema. Per informazioni, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente l'accesso amministrativo completo</a>. </p> </li> 
     <li> <p>Il <b>Utenti</b> oggetto nel tuo livello di accesso configurato per <b>Modifica</b> accesso, con <b>Crea</b> e almeno una delle seguenti due <b>Amministratore utenti</b> opzioni abilitate in <b>Metti a punto le impostazioni</b> <img src="assets/gear-icon-in-access-levels.png">. </p> 
     <ul><li> Amministratore utenti (Tutti gli utenti)</li>
     <li>Amministratore utenti (Utenti gruppi)</li></ul>
     <p>Se  <b>Amministratore utenti (Utenti gruppi)</b> è abilitato, per poter modificare un utente è necessario essere amministratore di gruppo per un gruppo di cui l'utente è membro.</p> 
     <p>Per ulteriori informazioni su <b>Utenti</b> impostazione in un livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Concedere l’accesso agli utenti</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table> 
*Per informazioni sulla pianificazione, il tipo di licenza o l'accesso disponibili, contattare l'amministratore Workfront.

## Modificare un profilo utente

{{step-1-to-users}}

1. Seleziona l’utente, quindi fai clic su **Modifica** icona ![](assets/edit-icon.png).

   Viene visualizzata la casella Modifica utente.

1. In **Modifica utente** , modificare una delle seguenti informazioni e fare clic su **Salva modifiche** in qualsiasi momento:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Informazioni personali </td> 
      <td> 
       <ul> 
        <li><p><b>Nome</b></p></li>
        <li><p><b>Cognome</b></p></li> 
        <li> <p><b>Indirizzo e-mail:</b> L’indirizzo e-mail di un utente corrisponde anche al suo nome utente in Workfront. Questo campo distingue tra maiuscole e minuscole e deve essere univoco. Se un utente tenta di aggiungere un indirizzo e-mail non univoco 3 volte in una finestra di 10 minuti, viene visualizzata una risposta reCAPTCHA.</p> <p> Seleziona la <b>Io non sono un robot</b> prima di procedere.</p><p>Inserire nell'elenco Consentiti Se utilizzi l’e-mail e immetti un dominio e-mail non incluso nell’elenco, l’utente non riceverà notifiche e-mail. Per ulteriori informazioni sul inserisco nell'elenco Consentiti di, consulta <a href="../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md" class="MCXref xref">Configurare il inserisco nell'elenco Consentiti di e-mail per l e-mail</a>.</p> </li> 
        <li> <p><b>Reimposta password</b>: fai clic su questo collegamento per reimpostare la password dell’utente. È necessario immettere la propria password prima di reimpostare quella di un altro utente.</p> <p>Per reimpostare la password di un altro utente, è necessario essere un amministratore di Workfront o un amministratore di gruppo.</p> <p><b>NOTA</b>:  
          <ul> 
           <li> <p>Se si è un amministratore di gruppo, è possibile reimpostare le password solo per gli utenti dei gruppi in cui si è designati come amministratore. Inoltre, l’autorizzazione Amministratore utenti (utenti gruppo) deve essere abilitata nel tuo livello di accesso:</p> <p> <img src="assets/group-admin-user.png" > </p> <p>Questa impostazione è disabilitata per impostazione predefinita. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </li> 
           <li> <p>Non è possibile reimpostare la password di un amministratore Workfront.</p> </li> 
          </ul> </p> </li> 
        <li><b>&lt;sso configuration=""&gt; Nome utente</b>: se l’amministratore di Workfront ha abilitato un’integrazione SSO con Workfront, in questo campo viene visualizzato il nome utente SSO. In questo campo è visibile il tipo di configurazione SSO abilitata per l’istanza di Workfront. </li> 
        <li> <p><b>OnlyAllow &lt;sso configuration=""&gt; Autenticazione</b>: se l’amministratore di Workfront ha abilitato un’integrazione SSO con Workfront e ha aggiornato tutti gli utenti per l’SSO, questo campo è selezionato per impostazione predefinita. In questo campo è visibile il tipo di configurazione SSO abilitata per l’istanza di Workfront.</p> <p>Quando questo campo è selezionato, l’utente deve accedere a Workfront con le proprie credenziali SSO. Deselezionando questa opzione, gli utenti potranno accedere a Workfront con le credenziali Workfront.</p> <p>Per ulteriori informazioni sulla configurazione di Workfront con una soluzione SSO, vedere <a href="../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md" class="MCXref xref">Panoramica del single sign-on in Adobe Workfront</a></p> <p>Per ulteriori informazioni sull'aggiornamento degli utenti per l'SSO, vedere <a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref">Aggiornare gli utenti per il Single Sign-On</a>.</p> 
        <p><b>NOTA</b>:</p> 
        <p> Se sei un amministratore gruppo, puoi modificare &lt;sso configuration=""&gt; solo per gli utenti dei gruppi in cui sei designato come tale. Inoltre, l’autorizzazione Amministratore utenti (utenti gruppo) deve essere abilitata nel tuo livello di accesso.
        <p>Se sei un amministratore gruppo e nel tuo livello di accesso hai abilitato l’autorizzazione Amministratore utenti (tutti gli utenti), puoi modificare il &lt;sso configuration=""&gt; per tutti gli utenti.</p> </li> 
        <li><b>Informazioni processo:</b> Informazioni sulla mansione, come la qualifica (nel <b>Titolo</b> e l'area di competenza di cui è responsabile l'utente (nel <b>Parlami di</b> ).</li> 
        <li><p><b>Informazioni di contatto</b>: numero di telefono dell’utente (nel <b>Numero di telefono, est.</b>, e <b>Numero cellulare</b> ) e l'indirizzo (nel campo <b>Indirizzo, città, stato, codice postale, paese</b> campi ).</p>
        <p>Se l’utente è abilitato per Unified User Management (UUM) o Adobe Identity Management System (IMS), il <b>Paese</b> nella sezione Informazioni contatto accetta solo i valori del codice paese (ad esempio, US, GB, IN).</p></li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Preferenze </td> 
      <td> 
       <ul> 
      <li> <p><b>Fuso orario:</b> Il fuso orario dell’utente.</p> <p>Per informazioni su come aiutare gli utenti a collaborare in Workfront con fusi orari diversi, consulta <a href="../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md" class="MCXref xref">Utilizzo dei fusi orari</a>.</p> </li> 
       <li><b>Impostazioni internazionali e-mail</b>: lingua dell’e-mail preferita dall’utente. Questo influisce sul formato dei numeri e delle date nelle e-mail inviate da Workfront a questo utente.</li>

   <li><b>Ricevi e-mail da questo ambiente di test</b>: seleziona questa opzione se desideri ricevere notifiche e-mail dall’ambiente a cui hai attualmente effettuato l’accesso.
      <p><b>NOTA</b></p>
      <p>Questa opzione è disponibile solo negli ambienti di anteprima e sandbox. Per impostazione predefinita, le notifiche e-mail sono abilitate nell’ambiente di produzione. </p>
      </li>

   <li><b>Mostra la percentuale di completamento dello stato di aggiornamento</b>: seleziona questa opzione se desideri visualizzare una barra della percentuale di completamento all’interno dell’area Aggiornamento delle attività di questo utente, quando utilizzi l’esperienza di commento legacy. Per informazioni, consulta <a href="/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md">Nuova esperienza di commento</a>.
      <p><span class="preview">Questa opzione è stata rimossa dall’ambiente di anteprima.</span></p>

   </li> 
       <li><b>Invia il lavoro che assegno a me stesso alla mia scheda Lavori in corso</b>: seleziona questa opzione se desideri che tutto ciò che l’utente assegna a se stesso venga visualizzato direttamente nell’elenco Working On (Lavori su) nella sezione Home. L’impostazione predefinita consiste nell’elencare tutto ciò che è stato assegnato a un utente nell’elenco Pronto per l’avvio o Non pronto nell’area Home.</li> 
       <li><b>Genera automaticamente delle bozze durante il caricamento dei documenti</b>: seleziona questa opzione se desideri che i documenti caricati dall’utente generino immediatamente una bozza. </li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notifiche</td> 
      <td> <p>Seleziona le notifiche e-mail da abilitare per il nuovo utente.</p> <p>Puoi selezionare le notifiche istantanee e giornaliere di riepilogo.</p> <p>Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref">Configurare le notifiche degli eventi per tutti gli utenti del sistema</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Accesso</td> 
      <td> 
       <ul> 
      <li><b>È attivo:</b> Selezionare questa casella per indicare che l'utente è attivo. Gli utenti attivi utilizzano una licenza di Workfront. Deselezionando la casella di controllo, l’utente viene disattivato e non può più accedere a Workfront.</li> 
       <li> <p><b>Livello d'Accesso:</b> Selezionare il livello di accesso da assegnare all'utente.</p> 
       <p>Quando si assegna un livello di accesso a un utente, è possibile assegnare un livello uguale o inferiore al proprio livello di accesso.</p>
       <p>Ad esempio, se il livello di accesso è Piano, non è possibile assegnare il livello di accesso Amministratore. Tuttavia, non è possibile assegnare un livello di accesso che, per impostazione predefinita, è inferiore al proprio livello di accesso se l’amministratore di Workfront ha abilitato autorizzazioni non predefinite sul livello di accesso che non sono abilitate anche nel proprio livello di accesso. </p>
       <p>Ad esempio, se si dispone di una licenza Pianificazione senza accesso per eliminare le attività, non è possibile assegnare a un utente una licenza Lavoro con accesso per eliminare le attività, anche se la licenza Lavoro è inferiore alla licenza Pianificazione. Per ulteriori informazioni, consulta  <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>. </p> 
       <p>Per ulteriori informazioni sui livelli di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Configurare l’accesso ad Adobe Workfront</a>.</p>
       <p> <b>NOTA:</b></p> 
       <p> Se l’organizzazione utilizza il nuovo modello di accesso (Standard/Light/Contributor), non è possibile riassegnare un utente Standard o Light a un livello di accesso Collaboratore se tale utente ha già raggiunto il limite di decisione per il mese. </p><p>Per ulteriori informazioni sul nuovo modello di accesso, consulta <a href="../how-access-levels-work/access-level-overview.md" class="MCXref xref">Panoramica dei nuovi livelli di accesso</a>. </p><p>Per informazioni sui limiti di decisione, consulta <a href="/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md" class="MCXref xref">Documento limitato e decisione sulla bozza per utenti non pagati - Panoramica</a>.</p></li> 
       <li> <p><b>Modello di layout</b>: scegli un modello di layout per l’utente. Questo modello di layout ha la precedenza su qualsiasi modello di layout assegnato al gruppo predefinito, al team predefinito o al ruolo principale dell’utente. Per ulteriori informazioni sulla priorità di assegnazione dei modelli di layout, vedere <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Creare e gestire modelli di layout</a>.</p> <p><b>NOTA</b>:  <p>L’elenco seguente descrive come l’elenco dei modelli disponibili in questo campo dipende dal tuo accesso:</p> 
       <ul> 
       <li>In qualità di amministratore di Workfront, puoi visualizzare tutti i modelli di layout a livello di sistema e di gruppo.</li> 
       <li>In qualità di amministratore di gruppo, puoi visualizzare il modello di layout a livello di sistema e quelli associati ai gruppi gestiti.</li> 
       <li>In qualità di utente con una licenza Pianificazione e con accesso per la modifica degli utenti, puoi visualizzare solo i modelli di layout a livello di sistema.</li> 
       </ul> <p>Per ulteriori informazioni sui modelli di layout a livello di gruppo, vedere <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Creare e gestire modelli di layout</a>.</p> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Organizzazione </td> 
      <td> 
       <ul> 
      <li><b>Azienda</b>: società dell’utente. Gli utenti possono essere associati a una sola azienda. È necessario creare un'azienda prima di associarla a un utente. Nell'elenco vengono visualizzate solo le società attive. Per informazioni sulla creazione di società, consulta <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md" class="MCXref xref">Creare e modificare le società</a>.</li> 
      <li><b>Fa riferimento a:</b> Se per l'utente è stata specificata un'azienda, in questo campo è possibile specificare anche il responsabile diretto dell'utente. Un utente può avere un solo manager. Questo campo non viene visualizzato se l’utente non è prima associato a una società. </li> 
      <li><b>Report diretti:</b> Se hai specificato una società per l’utente, puoi anche specificare i referenti diretti dell’utente. Un utente può avere più referenti diretti. Questo campo non viene visualizzato se l’utente non è prima associato a una società.</li> 
      <li><b>Team predefinito</b>: specifica il team principale per l’utente. Gli utenti possono avere un solo team principale. Il team predefinito è importante quando si assegna un modello di layout o quando si definisce il pulsante Lavoraci per le attività e i problemi assegnati all’utente. </li> 
      <li><b>Altri team</b>: gli utenti possono appartenere a più team. Un utente può visualizzare gli elementi di lavoro assegnati a qualsiasi team nella propria area Home. </li> 
      <li> <p><b>Gruppo predefinito:</b> Seleziona un gruppo appropriato per assegnare l’utente. In questo modo l'utente può accedere agli oggetti condivisi con il gruppo. È inoltre possibile condividere i modelli di layout con il Gruppo predefinito dell'utente.</p> <p>Questo campo è obbligatorio. Ogni utente deve essere associato a un gruppo predefinito. Se non ne selezioni uno, il gruppo viene assegnato come gruppo predefinito del nuovo utente.</p> <p><b>NOTA</b>:</p> 
      <p> È possibile assegnare un gruppo a un utente solo se si verifica una delle condizioni seguenti:</p>
      <ul><li>sei un amministratore di Workfront</li>
      <li>sei l’amministratore del gruppo</li>
      <li>il gruppo è pubblico.</li></ul> 
      <li> <p><b>Altri gruppi</b>: gli utenti possono appartenere a più gruppi. È possibile assegnare un gruppo a un utente solo se si è un amministratore di Workfront, se si è l'amministratore del gruppo o se il gruppo è pubblico.</p> <p><b>IMPORTANTE</b>:</p> 
      <p>L’aggiunta di un utente a più di 100 gruppi può causare problemi di prestazioni in qualsiasi area di Workfront che carica l’elenco dei gruppi.</p> <p>Per ulteriori informazioni sui gruppi pubblici, consulta <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Creare un gruppo</a>.</p> <p>Per ulteriori informazioni sui gruppi, consulta <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Panoramica sui gruppi</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Pianificazione risorse </td> 
      <td> 
       <ul>
       <li>
       <b>Orario di lavoro</b>: rappresenta la percentuale di tempo FTE (Full Time Equivalent) in cui l'utente è disponibile per il lavoro effettivo, esclusi i costi comuni. L'orario di lavoro deve essere un numero decimale massimo di 1 e non può essere 0. Ad esempio, una disponibilità del 20% per il lavoro effettivo sarebbe 0,2.

   Il valore predefinito del campo è 1, che indica che un utente spende l’intero FTE per il lavoro effettivo relativo al progetto.

   Il sistema utilizza questo numero per calcolare la disponibilità dell&#39;utente per il lavoro effettivo correlato al progetto.

   Per ulteriori informazioni sulla creazione di pianificazioni in Workfront, consulta <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Creare una pianificazione</a>.

   Eccezioni alla pianificazione e indisponibilità possono influire anche sulla capacità dell&#39;utente.

   Workfront calcola la disponibilità di un utente in base alle preferenze di Gestione risorse nell’area Configura. Per ulteriori informazioni, consulta <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configurare le preferenze di Gestione risorse</a>.

   <b>SUGGERIMENTO</b>

   Impostare il valore Tempo di lavoro su 1 per indicare che l&#39;utente è disponibile per il lavoro correlato al progetto per l&#39;intero equivalente a tempo pieno.
   </li> 
      <li> <b>Pianifica disattivazione</b>: seleziona questa casella se desideri che l’utente venga disattivato in una determinata data e in un’ora specifica. </li> 
       <li><b>Data disattivazione pianificata</b>: data e ora in cui l’utente viene disattivato. Per informazioni sulla pianificazione della disattivazione degli utenti, vedere <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">Pianifica la disattivazione degli utenti</a> in <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Disattivare o riattivare un utente</a>.</li> 
       <li> <p><b>Ruolo principale</b>: questo è il ruolo principale che l’utente può svolgere in Workfront. A questa mansione vengono assegnate anche tutte le attività e tutti i problemi a cui è assegnato l’utente. I ruoli sono essenziali nella gestione delle risorse. È possibile aggiornare questo campo solo se si dispone di una licenza Pianificazione con accesso utente amministrativo o se si è un amministratore Workfront. Per ulteriori informazioni sulla configurazione degli utenti con accesso amministratore, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Concedere l’accesso agli utenti</a>.</p> <p>Nell'elenco vengono visualizzati solo i ruoli di lavoro attivi. </p> </li> 
       <li>Se hai selezionato un’ <b>Ruolo principale</b>, il <b>Percentuale di disponibilità FTE</b> viene visualizzato. Specificare la percentuale di tempo della pianificazione dell'utente allocata a questa mansione. Il valore predefinito per la percentuale di disponibilità FTE per il ruolo principale è 100%. </li> 
       <li> <p><b>Altri Ruoli</b>: un utente può avere più ruoli in Workfront. I ruoli sono essenziali nella gestione delle risorse. Non esiste alcun limite al numero di mansioni che un utente può svolgere. Tuttavia, si consiglia di non assegnare un utente a un numero eccessivamente elevato di ruoli, perché la gestione delle risorse potrebbe diventare troppo complessa per questi utenti.<p>Nell'elenco vengono visualizzati solo i ruoli di lavoro attivi. Per ulteriori informazioni sulle mansioni, consulta <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Creare e gestire le mansioni</a>.</p> <p>È possibile aggiornare questo campo solo se si dispone di una licenza Pianificazione con accesso utente amministrativo o se si è un amministratore Workfront. <br>Per ulteriori informazioni sulla configurazione degli utenti con accesso amministratore, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Concedere l’accesso agli utenti</a>.</p> </li> 
       <li> <p>(Condizionale) Se hai selezionato uno o più <b>Altri Ruoli</b>, il <b>Percentuale di disponibilità FTE</b> viene visualizzato per ogni ruolo. Specificare la percentuale di tempo della pianificazione dell'utente allocata a ogni mansione. Il valore predefinito per la percentuale di disponibilità FTE per gli altri ruoli è 0%.</p> <p><b>NOTA</b>: se gli altri ruoli hanno una disponibilità FTE pari a 0%, non vengono visualizzati nella Programmazione delle risorse, a meno che gli utenti non siano assegnati ad attività in questi ruoli.</p> <p> <img alt="user_settings_roles_and_date_boxes_rp_story.png" src="assets/user-settings-roles-and-dte-boxes-rp-story.png"> </p> <p><b>NOTA</b>: <p>La somma di tutti <b>Percentuali di disponibilità FTE</b> per tutti i ruoli deve essere uguale a 100%. Ogni percentuale di disponibilità FTE calcola le ore disponibili per ogni ruolo per utente nella Programmazione delle risorse. Le ore disponibili per ogni ruolo per utente dipendono dal tempo disponibile per l’utente.</p> <p>Il tempo disponibile per l'utente viene calcolato da Workfront in base al metodo selezionato dall'amministratore Workfront per calcolare l'FTE nelle preferenze di gestione delle risorse.</p> <p>Per informazioni sul calcolo della disponibilità per l'utente, vedere <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Panoramica del calcolo delle ore e dell'FTE per utenti e ruoli nella pianificazione risorse</a>.</p> <p>Per informazioni sulla configurazione delle preferenze di Gestione risorse, vedi <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configurare le preferenze di Gestione risorse</a>.</p> </p>
       <span class="preview"><p>(Facoltativo) Le assegnazioni di mansioni con validità data vengono utilizzate nei calcoli finanziari se il ruolo dell'utente cambia durante un progetto.</p><p>Clic <b>Definisci i ruoli per data</b>, seleziona la <b>Ruolo principale</b> e <b>Altri Ruoli</b>e immettere la percentuale di allocazione per ogni ruolo. I ruoli possono essere gli stessi dei ruoli esistenti (utilizzando percentuali diverse) o nuovi ruoli. Seleziona la <b>Data di inizio</b> quando questi ruoli diventano attivi. Questa può essere una data futura. Quando diventano attivi i ruoli più recenti, puoi fare clic su <b>Mostra ruoli precedenti</b> per visualizzare i precedenti ruoli inattivi.</p> </li></span>
       <li> <p><b>Pianificazione</b>: associa una pianificazione all’utente. La pianificazione dell'utente calcola la sequenza temporale delle attività a cui l'utente è assegnato.</p> <p>È necessario creare una pianificazione prima di associarla a un utente. Per ulteriori informazioni sulla creazione di pianificazioni, vedere <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Creare una pianificazione</a>.</p> <p><b>NOTA</b>: è consigliabile che la pianificazione associata all’utente corrisponda al fuso orario dell’utente.</p> </li> 
       <li> <p><b>Timesheet Ricorrente</b>: associa un profilo scheda orario all’utente per garantire che le schede orario vengano generate automaticamente per l’utente.</p> <p><b>NOTA</b>: l’elenco dei profili disponibili in questo campo dipende dal tuo accesso:
       <ul>
       <li>In qualità di amministratore di Workfront, puoi visualizzare tutti i profili delle schede orario a livello di sistema e di gruppo.</li>
       <li>In qualità di amministratore di gruppo, puoi visualizzare i profili delle schede orario a livello di sistema, nonché quelli associati ai gruppi gestiti.</li>
       <li>In qualità di utente con una licenza Pianificazione e con accesso alla modifica degli utenti, puoi visualizzare solo i Profili Scheda orario a livello di sistema. Per ulteriori informazioni sui profili Timesheet a livello di gruppo, vedi <a href="../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md" class="MCXref xref">Creare, modificare e assegnare profili di schede orario</a>.</li>
      </ul></p> </li> 
       <li><b>Tipo di Ora Predefinito</b>: seleziona il tipo di ora predefinito per l’utente. Questo è il tipo di ora utilizzato per impostazione predefinita quando l’utente registra l’ora.</li> 
       <li><b>Tipi di lavoro disponibili</b>: seleziona i tipi di ore che devono essere disponibili per l’utente. Questi tipi di ore sono visibili ovunque in Workfront, dove l’utente può registrare l’ora. Un utente può visualizzare solo i tipi di ore abilitati a livello di progetto e di utente. Per ulteriori informazioni sui tipi di lavoro disponibili per gli utenti, vedere <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">Definire i tipi di ore e la disponibilità per le schede orario</a>.</li> 
       <li><b>Tempo di accesso:</b> Specificare se l'utente deve registrare il tempo sugli elementi di lavoro in ore o giorni. Per ulteriori informazioni, consulta <a href="../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md" class="MCXref xref">Configurare se il tempo è registrato in ore o giorni</a>.</li>

   <li> <b>FTE</b>: Equivalente a tempo pieno dell’utente. Workfront utilizza questo numero per calcolare la disponibilità dell'utente in base alla pianificazione predefinita solo quando le preferenze di gestione delle risorse a livello di sistema sono impostate su Pianificazione predefinita.

   <p>L’FTE indica la quantità di tempo che l’utente può trascorrere al lavoro. Sono inclusi i costi comuni e il tempo dedicato al lavoro del progetto. Ad esempio, nell’FTE è incluso anche il tempo trascorso nelle riunioni o nella formazione.</p>

   L&#39;FTE deve essere un numero decimale massimo di 1 e non può essere 0. Ad esempio, se il valore FTE è 0,5 e la pianificazione predefinita in Workfront è di 40 ore, l’utente è disponibile per 20 ore alla settimana.

   Il valore predefinito del campo è 1.

   Eccezioni alla pianificazione, l&#39;indisponibilità e il valore di Tempo di lavoro possono influire sulla disponibilità dell&#39;utente.

   Workfront calcola la disponibilità di un utente in base alle preferenze di Gestione risorse nell’area Configura.

   Se le Preferenze di Gestione risorse a livello di sistema sono impostate su La pianificazione dell&#39;utente, il valore specificato in questo campo viene ignorato e l&#39;utente viene considerato disponibile in base a quanto specificato nella programmazione.

   Per ulteriori informazioni, consulta <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configurare le preferenze di Gestione risorse</a>.

   Per ulteriori informazioni sulla creazione di pianificazioni in Workfront, consulta <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Creare una pianificazione</a>.
   </li>

   <li><b>Gruppi di risorse</b>: associa l’utente ai gruppi di risorse. Per ulteriori informazioni, consulta <a href="../../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md" class="MCXref xref">Associa i pool di risorse agli utenti </a>.</li>

   <li><b>Tasso di costo</b>: la quantità di costo all’ora per l’utente.
      <p>Per le tariffe effettive per data, fare clic su <strong>Aggiungi tariffa</strong>. Inserire il valore del tasso di costo per il periodo di tempo e assegnare una data di inizio e una data di fine in base alle esigenze. La tariffa di costo 1 non avrà una data di inizio e l'ultima tariffa di costo non avrà una data di fine.</p><p>Alcune date vengono aggiunte automaticamente. Ad esempio, se il tasso di costo 1 non ha una data di fine e si aggiunge il tasso di costo 2 con una data di inizio del 1° maggio 2023, al tasso di costo 1 verrà aggiunta una data di fine del 30 aprile 2023 in modo che non esistano spazi vuoti.</p></li>

   <li><b>Tariffa di fatturazione</b>: la quantità di fatturazione all’ora per l’utente.
      <p>Per le tariffe di fatturazione effettive della data, fai clic su <strong>Aggiungi tariffa</strong>. Inserire il valore della tariffa di fatturazione per il periodo di tempo e assegnare una data di inizio e una data di fine in base alle esigenze. La tariffa di fatturazione 1 non avrà una data di inizio e l'ultima tariffa di fatturazione non avrà una data di fine.</p> <p>Alcune date vengono aggiunte automaticamente. Ad esempio, se la Tariffa di fatturazione 1 non ha una data di fine e aggiungi un secondo con una data di inizio del 1° maggio 2023, alla Tariffa di fatturazione 1 viene aggiunta una data di fine del 30 aprile 2023 in modo che non esistano spazi vuoti.</p><p> <img alt="Costo utente e tariffe di fatturazione" src="assets/edit-user-cost-billing-rate-2.png"> </p></li>

   </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Moduli personalizzati</td> 
      <td><p>Associa a questo utente un modulo personalizzato esistente. È necessario creare un modulo personalizzato prima di associarlo a un utente. Nell’elenco vengono visualizzati solo i moduli personalizzati attivi. I campi ai quali non si dispone dell'accesso per la modifica non vengono visualizzati in un singolo modulo personalizzato.</p> <p><span class="preview"><strong>Nota:</strong> Le funzioni avanzate dei moduli personalizzati, ad esempio i campi di ricerca esterna e i campi nativi di Workfront, sono disponibili solo quando si apre il record utente nella pagina dei dettagli e non nella finestra di dialogo Modifica utente. Dall’elenco degli utenti, fai clic sul nome utente per aprire i dettagli.</span></p> <p>Per informazioni sulla creazione di moduli personalizzati, consulta <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Creare o modificare un modulo personalizzato</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Commento</td> 
      <td>Digita il commento da inviare agli utenti e alla sezione Aggiornamenti dei loro profili utente.</td> 
     </tr> 
    </tbody> 
   </table>
