---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Modificare i profili utente in blocco
description: In qualità di amministratore di Adobe Workfront, puoi modificare gli account utente in blocco.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: cb709b2f-659e-4110-81ac-a1ef967d534c
source-git-commit: c7b91828e5a4f961fc48e857eb63756b9b38f664
workflow-type: tm+mt
source-wordcount: '2625'
ht-degree: 0%

---

# Modificare i profili utente in blocco

{{highlighted-preview}}

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on editing a user's profile in the Adobe Admin Console, see the section "Edit user details" in the article [Bulk Upload Users](https://helpx.adobe.com/it/enterprise/using/bulk-upload-users.html) or contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
-->

È possibile modificare gli account utente in blocco. Quando si modificano gli utenti in blocco, solo i campi selezionati in modo specifico vengono aggiornati con le stesse informazioni per tutti gli utenti selezionati. Tutti gli altri campi non selezionati rimangono invariati per ogni singolo utente, anche se sono diversi per ogni utente.

>[!NOTE]
>
>* Non è possibile modificare in blocco la sezione Informazioni personali dei profili degli utenti perché tali informazioni devono essere univoche per ogni utente.
>* Per garantire la precisione dei dati e prestazioni ottimali, si consiglia di selezionare non più di 2.000 utenti alla volta per un montaggio in blocco.
>

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

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
   <td><p>Nuovo: Standard</p><p>Oppure</p><p>Corrente: Piano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>È necessario disporre di uno dei seguenti elementi:</p> 
    <ul> 
     <li> <p>Livello di accesso Amministratore di sistema. </li> 
     <li> <p>Impostazione di <b>Utenti</b> nel livello di accesso configurato per l'accesso di <b>Modifica</b>, con <b>Crea</b> e almeno una delle due opzioni di <b>Amministratore utenti</b> abilitate in <b>Ottimizza le impostazioni</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Di queste due opzioni, se <b>User Admin (Group Users)</b> è abilitato, è necessario essere un amministratore di gruppo di un gruppo di cui l'utente è membro.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Modificare gli account utente in blocco

{{step-1-to-users}}

1. Seleziona più di un utente, quindi fai clic sull&#39;icona **Modifica** ![Modifica icona](assets/edit-icon.png).

1. Nella casella **Modifica utente**, modifica le informazioni in una delle sezioni e fai clic su **Salva modifiche** <span class="preview">o **Salva**</span> in qualsiasi momento.

### Preferenze

* **Fuso orario**: il fuso orario dell&#39;utente.

  Per informazioni su come aiutare gli utenti a collaborare in Workfront con fusi orari diversi, consulta [Lavorare con fusi orari diversi](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).

* **Impostazioni locali e-mail**: impostazioni locali e-mail preferite dall&#39;utente. Questo influisce sul formato dei numeri e delle date nelle e-mail inviate da Workfront a questo utente.

  >[!NOTE]
  >
  >Quando la tua organizzazione utilizza Adobe Unified Experience, le preferenze della lingua dell’utente vengono memorizzate nel suo profilo Adobe e le impostazioni locali dell’e-mail non vengono utilizzate. Per informazioni sull&#39;accesso a queste preferenze, vedere [Esperienza unificata Adobe per Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

### Notifiche

Seleziona le notifiche e-mail da abilitare per gli utenti.

Puoi selezionare le notifiche istantanee e giornaliere di riepilogo. Tutte le notifiche di riepilogo giornaliere vengono inviate qualche volta dopo la stessa ora per tutti gli utenti selezionati.

Per ulteriori informazioni, vedere [Configurare le notifiche degli eventi per tutti gli utenti del sistema](/help/quicksilver/administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

### Accesso

* **È attivo** / <span class="preview">**L&#39;utente è attivo**</span>: abilitare questa opzione per indicare che gli utenti sono attivi. Gli utenti attivi utilizzano una licenza di Workfront. La disattivazione del campo disattiva gli utenti e impedisce loro di accedere a Workfront.

* **Livello di accesso**: selezionare il livello di accesso da assegnare a questi utenti. Tutti gli utenti selezionati avranno lo stesso livello di accesso.

  Quando si assegna un livello di accesso agli utenti, è possibile assegnare un livello uguale o inferiore al proprio livello di accesso. Ad esempio, se il livello di accesso è Standard, non è possibile assegnare il livello di accesso Amministratore.

  Tuttavia, non è possibile assegnare un livello di accesso che, per impostazione predefinita, è inferiore al proprio livello di accesso se l’amministratore di Workfront ha abilitato autorizzazioni non predefinite sul livello di accesso che non sono abilitate anche nel proprio livello di accesso.

  Ad esempio, se si dispone di una licenza Standard senza accesso per eliminare le attività, non è possibile assegnare a un utente una licenza Light con accesso per eliminare le attività, anche se la licenza Light è inferiore alla licenza Standard. Per ulteriori informazioni, vedere [Creare o modificare livelli di accesso personalizzati](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

  Per ulteriori informazioni sui livelli di accesso, vedere [Configurare l&#39;accesso ad Adobe Workfront](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/configure-access.md).

  >[!NOTE]
  >
  >Se l’organizzazione utilizza il nuovo modello di accesso (Standard/Light/Contributor), non è possibile riassegnare un utente Standard o Light a un livello di accesso Collaboratore se tale utente ha già raggiunto il limite di decisione per il mese.
  >
  >Per ulteriori informazioni sul nuovo modello di accesso, vedere [Panoramica sui nuovi livelli di accesso](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md).
  >
  >Per informazioni sui limiti di decisione, consulta [Documento limitato e decisione sulla bozza per utenti non pagati, panoramica](/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md).

* **Modello di layout**: scegliere un modello di layout per gli utenti. questo modello di layout ha la precedenza su qualsiasi modello di layout assegnato al proprio Gruppo predefinito, Team predefinito o Ruolo principale. Per ulteriori informazioni sulla priorità di assegnazione dei modelli di layout, vedere [Creare e gestire modelli di layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

  L’elenco seguente descrive come l’elenco dei modelli disponibili in questo campo dipende dal tuo accesso:

   * In qualità di amministratore di Workfront, puoi visualizzare tutti i modelli di layout a livello di sistema e di gruppo.
   * In qualità di amministratore di gruppo, puoi visualizzare il modello di layout a livello di sistema e quelli associati ai gruppi gestiti.
   * In qualità di utente con una licenza Standard o Plan e con accesso per la modifica degli utenti, puoi visualizzare solo i modelli di layout a livello di sistema.

     Per ulteriori informazioni sui modelli di layout a livello di gruppo, vedere [Creare e modificare i modelli di layout di un gruppo](/help/quicksilver/administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

### Organizzazione

* **Società**: la società degli utenti. Gli utenti possono essere associati a una sola azienda. È necessario creare un&#39;azienda prima di associarla a un utente. Nell&#39;elenco vengono visualizzate solo le società attive. Per informazioni sulla creazione di società, vedere [Creare e modificare società](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).
* **Team predefinito**: specificare il team predefinito per gli utenti. Gli utenti possono avere un solo team principale.
* **Altri team**: gli utenti possono appartenere a più team.
* **Gruppo predefinito** / <span class="preview">**Gruppo predefinito corrente**</span>: selezionare un gruppo appropriato per assegnare gli utenti. In questo modo gli utenti possono accedere agli oggetti condivisi con il gruppo. È inoltre possibile condividere i modelli di layout con un gruppo predefinito.

  Questo campo è obbligatorio. Ogni utente deve essere associato a un gruppo predefinito. Se non ne selezioni uno, il Gruppo predefinito viene assegnato come Gruppo predefinito.

  È possibile assegnare un gruppo a un utente solo se si verifica una delle condizioni seguenti:

   * sei un amministratore di Workfront
   * sei l’amministratore del gruppo
   * il gruppo è pubblico

* **Altri gruppi**: gli utenti possono appartenere a più gruppi. È possibile assegnare un gruppo a un utente solo se si è un amministratore di Workfront, se si è l&#39;amministratore del gruppo o se il gruppo è pubblico.

  >[!IMPORTANT]
  >
  >L’aggiunta di un utente a più di 100 gruppi può causare problemi di prestazioni in qualsiasi area di Workfront che carica l’elenco dei gruppi.

  Per ulteriori informazioni sui gruppi pubblici, vedere [Creare un gruppo](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

  Per ulteriori informazioni sui gruppi, vedere [Panoramica sui gruppi](/help/quicksilver/administration-and-setup/manage-groups/groups-overview/groups.md).

### Pianificazione risorse

* **Tempo di lavoro**: rappresenta la percentuale del tempo FTE (Full Time Equivalent) in cui gli utenti sono disponibili per il lavoro effettivo, esclusi i costi comuni. L&#39;orario di lavoro deve essere un numero decimale massimo di 1 e non può essere 0. Ad esempio, una disponibilità del 20% per il lavoro effettivo sarebbe 0,2.

  Il valore predefinito del campo è 1, che indica che un utente spende l’intero FTE per il lavoro effettivo relativo al progetto.

  Il sistema utilizza questo numero per calcolare la disponibilità dell&#39;utente per il lavoro effettivo correlato al progetto.

  Per ulteriori informazioni sulla creazione di pianificazioni in Workfront, vedere [Creare una pianificazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

  Eccezioni alla pianificazione e indisponibilità possono influire anche sulla capacità dell&#39;utente.

  Workfront calcola la disponibilità di un utente in base alle preferenze di Gestione risorse nell’area Configura. Per ulteriori informazioni, vedere [Configurare le preferenze di Gestione risorse](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

  >[!TIP]
  >
  >Impostare il valore Tempo di lavoro su 1 per indicare che l&#39;utente è disponibile per il lavoro correlato al progetto per l&#39;intero equivalente a tempo pieno.

* **Pianifica disattivazione** / <span class="preview">**Imposta data di disattivazione**</span>: seleziona questa casella / <span class="preview">fai clic su questo pulsante</span> per pianificare la disattivazione di questi utenti in una data e in un&#39;ora specifiche.
* **Data disattivazione pianificata** / <span class="preview">**Data disattivazione**</span>: la data e l&#39;ora in cui gli utenti vengono disattivati. Per informazioni sulla pianificazione della disattivazione degli utenti, vedere [Pianificare la disattivazione degli utenti](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#schedule-users-for-deactivation) in [Disattivare o riattivare un utente](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).
* **Ruolo principale**: è il ruolo principale che gli utenti possono svolgere in Workfront. A ogni attività e problema assegnato agli utenti viene assegnata questa mansione. I ruoli sono essenziali nella gestione delle risorse. È possibile aggiornare questo campo solo se si dispone di una licenza Standard o Full con accesso utente amministrativo o se si è un amministratore Workfront. Per ulteriori informazioni sulla configurazione degli utenti con accesso amministrativo, vedere [Concedere l&#39;accesso agli utenti](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

  Nell&#39;elenco vengono visualizzati solo i ruoli di lavoro attivi.

* (Condizionale) Se hai selezionato un **Ruolo principale**, viene visualizzato il campo **Percentuale di disponibilità FTE**. Specifica la percentuale di tempo delle pianificazioni degli utenti allocata a questa mansione. Il valore predefinito per la percentuale di disponibilità FTE per il ruolo principale è 100%.
* **Altri ruoli**: gli utenti possono avere più ruoli in Workfront. I ruoli sono essenziali nella gestione delle risorse. Non esiste alcun limite al numero di mansioni che un utente può svolgere. Tuttavia, si consiglia di non assegnare un utente a un numero eccessivamente elevato di ruoli, perché la gestione delle risorse potrebbe diventare troppo complessa per questi utenti.

  Nell&#39;elenco vengono visualizzati solo i ruoli di lavoro attivi. Per ulteriori informazioni sulle mansioni, vedere [Creare e gestire le mansioni](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

  È possibile aggiornare questo campo solo se si dispone di una licenza Standard o Full con accesso utente amministrativo o se si è un amministratore Workfront.

  Per ulteriori informazioni sulla configurazione degli utenti con accesso amministrativo, vedere [Concedere l&#39;accesso agli utenti](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

* (Condizionale) Se hai selezionato uno o più **Altri ruoli**, per ogni ruolo viene visualizzato il campo **Percentuale di disponibilità FTE**. Specifica la percentuale di tempo delle pianificazioni degli utenti allocata a ogni mansione. Il valore predefinito per la percentuale di disponibilità FTE per gli altri ruoli è 0%.

  Se Altri ruoli hanno una disponibilità FTE pari a 0%, non vengono visualizzati nella Programmazione delle risorse, a meno che gli utenti non siano assegnati ad attività in questi ruoli.

  La somma di tutte le **percentuali di disponibilità FTE** per tutti i ruoli deve essere uguale al 100%. Ogni percentuale di disponibilità FTE calcola le ore disponibili per ogni ruolo per utente nella Programmazione delle risorse. Le ore disponibili per ogni ruolo per utente dipendono dal tempo disponibile per l’utente.

  Il tempo disponibile per l&#39;utente viene calcolato da Workfront in base al metodo selezionato dall&#39;amministratore Workfront per calcolare l&#39;FTE nelle preferenze di gestione delle risorse.

  Per informazioni sul calcolo della disponibilità per l&#39;utente, vedere [Panoramica sul calcolo delle ore e dell&#39;FTE per gli utenti e i ruoli nella Programmazione delle risorse](/help/quicksilver/resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md).

  Per informazioni sulla configurazione delle preferenze di Gestione risorse, vedere [Configurare le preferenze di Gestione risorse](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

* **Pianificazione**: associa una pianificazione agli utenti. La pianificazione degli utenti calcola la sequenza temporale delle attività a cui gli utenti sono assegnati.

  È necessario creare una pianificazione prima di associarla agli utenti. Per ulteriori informazioni sulla creazione di pianificazioni, vedere [Creare una pianificazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

  >[!IMPORTANT]
  >
  >Workfront utilizza la pianificazione di un utente solo quando l&#39;impostazione **Calcola disponibilità risorse utilizzando** è impostata su **La pianificazione dell&#39;utente**. Per informazioni su come questa impostazione influisce sulla pianificazione utilizzata per Gestione risorse, vedere [Configurare le preferenze di Gestione risorse](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

* **Profilo scheda orario**: associa un profilo scheda orario agli utenti per garantire che le schede orario vengano generate automaticamente.

  L’elenco dei profili disponibili in questo campo dipende dal tuo accesso:

   * In qualità di amministratore di Workfront, puoi visualizzare tutti i profili delle schede orario a livello di sistema e di gruppo.
   * In qualità di amministratore di gruppo, puoi visualizzare i profili delle schede orario a livello di sistema, nonché quelli associati ai gruppi gestiti.
   * In qualità di utente con una licenza Standard o Plan e con accesso in modifica agli utenti, puoi visualizzare solo i profili delle schede orario a livello di sistema. Per ulteriori informazioni sui profili delle schede orario a livello di gruppo, vedere [Creare, modificare e assegnare profili delle schede orario](/help/quicksilver/timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

* **Tipo di Ora Predefinito**: Selezionare il tipo di Ora predefinito per gli utenti. Questo è il tipo di ora utilizzato per impostazione predefinita quando gli utenti registrano l’ora.
* **Tipi di ore disponibili**: selezionare i tipi di ore che devono essere disponibili per gli utenti. Questi tipi di ore sono visibili ovunque in Workfront, dove gli utenti possono registrare l’ora. Gli utenti possono visualizzare solo i tipi di ore abilitati a livello di progetto e di utente. Per ulteriori informazioni sui tipi di ore disponibili per gli utenti, vedere [Definire i tipi di ore e la disponibilità](/help/quicksilver/timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).
* **FTE**: questo è l&#39;equivalente a tempo pieno degli utenti. Workfront utilizza questo numero per calcolare la disponibilità degli utenti in base alla pianificazione predefinita solo quando le preferenze di gestione delle risorse a livello di sistema sono impostate su Pianificazione predefinita.

  L’FTE indica la quantità di tempo che gli utenti possono trascorrere al lavoro. Sono inclusi i costi comuni e il tempo dedicato al lavoro del progetto. Ad esempio, nell’FTE è incluso anche il tempo trascorso nelle riunioni o nella formazione.

  L&#39;FTE deve essere un numero decimale massimo di 1 e non può essere 0. Ad esempio, se il valore FTE è 0,5 e la pianificazione predefinita in Workfront è di 40 ore, gli utenti sono disponibili per 20 ore alla settimana.

  Il valore predefinito del campo è 1.

  Eccezioni alla pianificazione, indisponibilità e valore dell&#39;orario di lavoro possono influire sulla disponibilità degli utenti.

  Workfront calcola la disponibilità di un utente in base alle preferenze di Gestione risorse nell’area Configura.

  Se le Preferenze di Gestione risorse a livello di sistema sono impostate su La pianificazione dell&#39;utente, il valore specificato in questo campo viene ignorato e l&#39;utente viene considerato disponibile in base a quanto specificato nella programmazione.

  Per ulteriori informazioni, vedere [Configurare le preferenze di Gestione risorse](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

  Per ulteriori informazioni sulla creazione di pianificazioni in Workfront, vedere [Creare una pianificazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* **Pool di Risorse**: associa gli utenti ai Pool di Risorse.

  >[!NOTE]
  >
  >In questo campo vengono visualizzati solo i pool di risorse comuni a tutti gli utenti selezionati. Se gli utenti selezionati non dispongono di pool di risorse condivisi, questo campo è vuoto. Se questo campo è vuoto, i pool di risorse specificati in questo campo sovrascriveranno i singoli pool di risorse.

  Per ulteriori informazioni sui pool di risorse, vedere [Associare i pool di risorse agli utenti](/help/quicksilver/resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md).

* **Tariffa di costo**: importo del costo orario per l&#39;utente.

  Per le tariffe effettive della data, fare clic su **Aggiungi tariffa**. Inserire il valore del tasso di costo per il periodo di tempo e assegnare una data di inizio e una data di fine in base alle esigenze. La tariffa di costo 1 non avrà una data di inizio e l&#39;ultima tariffa di costo non avrà una data di fine.

  Alcune date vengono aggiunte automaticamente. Ad esempio, se il tasso di costo 1 non ha una data di fine e si aggiunge il tasso di costo 2 con una data di inizio del 1° maggio 2023, al tasso di costo 1 verrà aggiunta una data di fine del 30 aprile 2023 in modo che non esistano spazi vuoti.

* **Tariffa di fatturazione**: la quantità di fatturazione all&#39;ora per l&#39;utente.

  Per le tariffe di fatturazione effettive della data, fare clic su **Aggiungi tariffa**. Inserire il valore della tariffa di fatturazione per il periodo di tempo e assegnare una data di inizio e una data di fine in base alle esigenze. La tariffa di fatturazione 1 non avrà una data di inizio e l&#39;ultima tariffa di fatturazione non avrà una data di fine.

  Alcune date vengono aggiunte automaticamente. Ad esempio, se la Tariffa di fatturazione 1 non ha una data di fine e aggiungi un secondo con una data di inizio del 1° maggio 2023, alla Tariffa di fatturazione 1 viene aggiunta una data di fine del 30 aprile 2023 in modo che non esistano spazi vuoti.

### Moduli personalizzati

Associa agli utenti un modulo personalizzato esistente. È necessario creare un modulo personalizzato prima di associarlo a un utente. Nell’elenco vengono visualizzati solo i moduli personalizzati attivi. I campi ai quali non si dispone dell&#39;accesso per la modifica non vengono visualizzati in un singolo modulo personalizzato.

>[!NOTE]
>
>Le funzioni avanzate dei moduli personalizzati, ad esempio i campi di ricerca esterni e i campi nativi di Workfront, sono disponibili solo quando si apre il record utente nella pagina dei dettagli e non nella finestra di dialogo Modifica utente. Dall’elenco degli utenti, fai clic sul nome utente per aprire i dettagli.

Facoltativamente, è possibile selezionare l&#39;opzione **Ricalcola espressioni personalizzate** per assicurarsi che tutti i campi personalizzati calcolati nei moduli personalizzati allegati agli utenti selezionati siano aggiornati.

Per informazioni sulla creazione di moduli personalizzati, vedere [Creare un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

### Commento

Digita il commento da inviare agli utenti e alla sezione Aggiornamenti dei loro profili utente.

<!--
   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Preferences</td> 
      <td> 
       <ul> 
        <li><b>Time Zone:</b> The users' time zone.</li> 
        <li><b>Locale</b>: The users' preferred locale. This affects the format of numbers and dates in the emails that come from Workfront.</li> 
        <li><b>Send work I assign to myself to my Working On tab</b>: This setting refers to a deprecated feature that has been removed from Workfront.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notifications</td> 
      <td>Select the email notifications which should be enabled for the new user.<p>You can select instant as well as daily digest notifications. All the daily digest notifications are delivered sometime after the same time for all the users selected. For more information, see <a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref">Configure event notifications for everyone in the system</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Access</td> 
      <td> 
       <ul> 
        <li><b>Is Active:</b> Select this field to indicate whether the users are active. Active users use a Workfront license. Deselecting the field deactivates the users.</li> 
        <li> 
        <p><b>Access Level:</b> Select the access level to assign to these users. All users selected will have the same access level.
        </p> 
        <p>When you assign an access level to users, you can assign a level equal to or less than your own access level. (For example, if your access level is Planner, you cannot assign the Administrator access level.) </p>
        <p>However, you cannot assign an access level that is lower than your own if the Workfront administrator has enabled permissions on the access level that are not also enabled in your own (via the Fine-Tune settings, as described in <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>).</p> 
        <p>For more information about access levels, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Configure access to Adobe Workfront</a>.</p> 
         </li> 
        <li> 
        <p><b>Layout Template</b>: Choose a layout template for the users. The layout template assigned to the users will take precedence over any layout template assigned to their Home Group, Home Team or primary job role. For more information about the assignment priority of layout template, see <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Create and manage layout templates</a>.</p> 
        <p><b>NOTE</b>:  The list of layout templates you have available in this field depends on your access:
          <ul>
           <li>As a Workfront administrator, you can see all system-level and group-level layout templates.</li>
           <li>As a group administrator, you can see system-level layout templates, as well as those associated with the groups that you manage.</li>
           <li><p>As a user with a Planner license and access to edit users, you can see only system-level layout templates. </p>
           <p>For information about group-level layout templates, see <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Create and manage layout templates</a>.</p>
           </li>
          </ul></p> 
          </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Organization</td> 
      <td> 
       <ul> 
        <li><b>Company</b>: The company of the users. Users can be associated only with one company. You must create a company before you can associate it with a user. Only active companies display in the list. For information about creating companies, see Understanding and Managing Companies.</li> 
        <li><b>Home Team</b>: Specify the home team for the users. Users can only have one home team. </li> 
        <li><b>Other Teams</b>: Users can belong to multiple teams. </li> 
        <li> <p><b>Home Group:</b> Select an appropriate group to assign the users as their Home Group. This gives the user the ability to access objects that are shared with the group.</p> <p><b>NOTE</b>:  This is a required field. You cannot have users not associated with a Home Group.</p> <p>You can assign a group to users only in the following situations:</p> 
         <ul> 
          <li>You are a Workfront administrator.</li> 
          <li>You are the administrator of that group.</li> 
          <li>The group is public.</li> 
         </ul> </li> 
        <li> <p><b>Other Groups</b>: Users can belong to multiple groups. You can assign a group to a user only  in the following situations:</p> 
         <ul> 
          <li>You are a Workfront administrator.</li> 
          <li>You are the administrator of that group.</li> 
          <li> <p>The group is public. </p> 
          <p>For more information about public groups, see <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Create a group</a>.</p> 
          <p>For more information about groups, see <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Groups overview</a>.</p> 
          </li> 
         </ul> 
         </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Resource Planning</td> 
      <td> 
       <ul> 
      
      <li>
       <b>Work Time</b>: Represents the percentage of the Full Time Equivalent (FTE) time that the user is available for actual work, not including overhead. Work Time must be a decimal number up to 1, and it cannot be 0. For example, a 20% availability for actual work would be 0.2.

      The field's default is 1, indicating that a user spends their entire FTE on actual, project-related work. 

      The system uses this number to calculate the availability of the user for actual, project-related work. 

      For more information about creating schedules in Workfront, see <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Create a schedule</a>.

      Schedule exceptions and time off might also affect the user capacity. 

      Workfront calculates a user's availability depending on the Resource Management preferences in your Setup area. For more information, see <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configure Resource Management preferences</a>. 

      <b>TIP</b>

      Set the Work Time value to  1 to indicate that the user is available for project-related work their entire full-time equivalent.
      </li> 

      <li><b>Schedule Deactivation</b>: Check this box if you want to schedule users to be deactivated after a period of time.</li> 
       <li><b>Scheduled Deactivation Date</b>: The date after which the users become deactivated. For more information about scheduling users for deactivation, see the section <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">Schedule users for deactivation</a> in <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Deactivate or reactivate a user</a>.</li> 
       <li> <p><b>Primary Role</b>: This is the primary job role that a user has in Workfront. Every task and issue that the users are assigned to is also assigned to this job role, by default. Job roles are essential in resource management. For more information about job roles, see <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Create and manage job roles</a></p> <p>You can update this field only if you have a Plan license with administrative user access, or if you are a Workfront administrator. For more information about setting up users with administrative user access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> </li> 
       <li>(Conditional) If you selected a <b>Primary Role</b>, the <b>Percentage of FTE Availability</b> field displays. Specify what percentage of time of the users' schedules is allocated to this job role. The default value for the Percentage of FTE Availability for the Primary Role is 100%.</li> 
       <li> <p><b>Other Roles</b>: Users can have multiple job roles in Workfront. Job roles are essential in resource management. There is no limit for how many job roles a user can fulfill. However, we recommend to not assign one user to an excessively large number of job roles, because resource management might become too complex for these users.</p> <p>For more information about job roles, see <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Create and manage job roles</a>.</p> <p>You can update this field only if you have a Plan license with administrative user access, or if you are a Workfront administrator. For more information about setting up users with administrative user access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> </li> 
       <li> <p>(Conditional) If you selected one or multiple <b>Other Roles</b>, the <b>Percentage of FTE Availability</b> field displays for each role. Specify what percentage of time of the users' schedules is allocated to each job role. The default value for the Percentage of FTE Availability for the Other Roles is 0%.</p> <p><b>NOTE</b>:  
       <ul> 
       <li>If Other Roles have a 0% FTE Availability, they do not display in the Resource Planner, unless the users are assigned to tasks in these roles.</li> 
       <li> <p>The sum of all Percentages of FTE Availability for all roles must equal 100%. Each Percentage of FTE Availability calculates the Available Hours for each role per user in the Resource Planner. The Available Hours for each role per user depends on the available time for the user.</p> <p>The available time for the user is calculated by Workfront depending on the method that has been selected by the Workfront administrator to calculate the FTE in the Resource Management Preferences.</p> <p>For more information about calculating availability for the user, see <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Overview of calculating hours and FTE for users and roles in the Resource Planner</a>.</p> <p>For more information about configuring Resource Management preferences, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configure Resource Management preferences</a>.</p> </li> 
       </ul> </p> </li> 
       <li> <p><b>Schedule</b>: Associate a schedule with the users. The schedule of the users calculates the timeline of the tasks the users are assigned to.</p> <p>A Workfront administrator or a group administrator must create a schedule before it can be associated with users.</p> <p>Select a system-level or a group schedule to assign it to the selected users.</p> <p>For more information about system-level and group schedules, see <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.</p> <p><b>IMPORTANT</b>: Workfront uses the schedule of a user only when the Calculate Resource Availability Using setting is set to The User's Schedule. For information about how the Calculate Resource Availability Using setting affects which schedule is used for Resource Management, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configure Resource Management preferences</a>.</p> </li> 
       <li> <p><b>Timesheet Profile</b>: Associate a Timesheet Profile with the users. This ensures that timesheets generate automatically for the users.</p> 
       <p><b>NOTE</b>:  
       <ul> 
       <li>The list of timesheet profiles you have available in this field depends on your access:
       <ul>
       <li>As a Workfront administrator, you can see all system-level and group-level timesheet profiles.</li>
       <li><p>As a group administrator, you can see system-level timesheet profiles, as well as those associated with the groups that you manage.</p></li>
       <li><p>As a user with a Planner license and access to edit users, you can see only system-level timesheet profiles.</p></li>
       </ul></li> 
       <li>If you are a group administrator, all of the users you are editing must be members of a group that you administer.</li> 
       </ul> </p> </li> 
       <li><b>Default Hour Type</b>: Select the default hour type for the users. This is the hour type that is used by default when the users log time.</li> 
       <li> <p><b>Available Hour Types</b>: Select the hour types that should be available to the user. These hour types are visible everywhere in Workfront where the users can log time. A user can only see the hour types that are enabled at the project level as well as the user level.</p> 
       <p>For more information about what hour types are available to users, see <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">Define hour types and availability</a>.</p> 
       </li> 
       <li> <b>FTE</b>: This is the Full Time Equivalent of the user. Workfront uses this number to calculate the availability of the user based on the Default Schedule only when the Resource Management Preferences at the system level are set to The Default Schedule. 

      <p>The FTE indicates the amount of time that the user can spend at work. This includes overhead, as well as time spent on project work. For example, time that is spent in meetings, or training is also included in the FTE.</p> 

      The FTE must be a decimal number up to 1, and it cannot be 0. For example, if the FTE value is 0.5 and the Default Schedule in Workfront is 40 hours, the user is available for 20 hours a week. 

      The field's default is 1.

      Schedule exceptions, time off might, and the value of Work Time may affect the availability of the user. 

      Workfront calculates a user's availability depending on the Resource Management preferences in your Setup area.

      If the Resource Management Preferences at the system level are set to The User's Schedule, the value you specify here is ignored and the user is considered to be available according to what is specified in their schedule. 

      For more information, see <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configure Resource Management preferences</a>. 

      For more information about creating schedules in Workfront, see <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Create a schedule</a>.
      </li> 
       <li> <p><b>Resource Pools</b>: Associate the users with resource pools.</p> <p><b>NOTE</b>:  Only the resource pools that are common to all the users selected appear in this field. If the users selected have no shared resource pools, this field is empty. If this field is empty, the resource pools you specify here will overwrite their individual resource pools.</p> 
       <p>For more information about resource pools, see <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Resource pools overview </a>.</p> </li> 
       <li><b>Cost Per Hour</b>: The amount of cost per hour for the user. </li> 
       <li><b>Billing Per Hour</b>: The amount of billing per hour for the user.</li> 
       <li><b>Custom Forms</b>: Associate an existing user custom form with the users. You must create a custom form before you can associate it with a user. Only active custom forms display in the list. For information about creating custom forms, see <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Create a custom form</a>.</li> 
       <li><b>Comment</b>: Enter a comment in the field provided. All users selected will receive an in-app notification as well as an email notification with your comment. The comment shows in the Updates tab of the users' profile.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>
-->

