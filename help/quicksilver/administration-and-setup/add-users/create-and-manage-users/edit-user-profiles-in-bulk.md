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
source-git-commit: e52881a03f69d7c4d6a62dcdc9c6044f6f5dd016
workflow-type: tm+mt
source-wordcount: '2246'
ht-degree: 0%

---

# Modificare i profili utente in blocco

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on editing a user's profile in the Adobe Admin Console, see the section "Edit user details" in the article [Bulk Upload Users](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html) or contact your Adobe Admin Console Administrator.
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
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>È necessario disporre di uno dei seguenti elementi:</p> 
    <ul> 
     <li> <p>Livello di accesso Amministratore di sistema. Per informazioni, vedere <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente l'accesso amministrativo completo</a>. </p> </li> 
     <li> <p>Impostazione di <b>Utenti</b> nel livello di accesso configurato per l'accesso di <b>Modifica</b>, con <b>Crea</b> e almeno una delle due opzioni di <b>Amministratore utenti</b> abilitate in <b>Ottimizza le impostazioni</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Di queste due opzioni, se l'utente <b>Amministratore (utenti gruppo)</b> è abilitato, è necessario essere un amministratore di gruppo di un gruppo di cui l'utente è membro.</p> <p>Per ulteriori informazioni sull'impostazione <b>Utenti</b> in un livello di accesso, vedere <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Concedere l'accesso agli utenti</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Modificare gli account utente in blocco

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **menu principale** nell&#39;angolo superiore destro di Adobe Workfront, quindi fai clic su **Utenti** ![](assets/users-icon-in-main-menu.png).

1. Selezionare più utenti, quindi fare clic sull&#39;icona Modifica ![](assets/edit-icon.png).

1. Nella casella **Modifica utente** visualizzata, modificare una delle opzioni seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Preferenze</td> 
      <td> 
       <ul> 
        <li><b>Fuso orario:</b> Il fuso orario degli utenti.</li> 
        <li><b>Impostazioni locali</b>: impostazioni locali preferite dagli utenti. Questo influisce sul formato dei numeri e delle date nelle e-mail provenienti da Workfront.</li> 
        <li><b>Invia il lavoro che assegno a me stesso alla mia scheda Lavori in corso</b>: seleziona questa opzione se vuoi che tutto ciò che gli utenti assegnano a se stessi appaia direttamente nella loro scheda Lavori in corso. L’impostazione predefinita consiste nell’elencare tutto ciò che è stato assegnato a un utente nella relativa scheda Work Request (Richiesta di lavoro).</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notifiche</td> 
      <td>Seleziona le notifiche e-mail da abilitare per il nuovo utente.<p>Puoi selezionare le notifiche istantanee e giornaliere di riepilogo. Tutte le notifiche di riepilogo giornaliere vengono inviate qualche volta dopo la stessa ora per tutti gli utenti selezionati. Per ulteriori informazioni, vedere <a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref">Configurare le notifiche degli eventi per tutti gli utenti del sistema</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Accesso</td> 
      <td> 
       <ul> 
        <li><b>È attivo:</b> Selezionare questo campo per indicare se gli utenti sono attivi. Gli utenti attivi utilizzano una licenza di Workfront. Deselezionando il campo si disattivano gli utenti.</li> 
        <li> 
        <p><b>Livello di accesso:</b> Selezionare il livello di accesso da assegnare a questi utenti. Tutti gli utenti selezionati avranno lo stesso livello di accesso.
        </p> 
        <p>Quando si assegna un livello di accesso agli utenti, è possibile assegnare un livello uguale o inferiore al proprio livello di accesso. Ad esempio, se il livello di accesso è Planner, non è possibile assegnare il livello di accesso Amministratore. </p>
        <p>Tuttavia, non è possibile assegnare un livello di accesso inferiore al proprio se l'amministratore di Workfront dispone di autorizzazioni abilitate per il livello di accesso che non sono abilitate anche nel proprio (tramite le impostazioni di ottimizzazione, come descritto in <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>).</p> 
        <p>Per ulteriori informazioni sui livelli di accesso, vedere <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Configurare l'accesso ad Adobe Workfront</a>.</p> 
         </li> 
        <li> 
        <p><b>Modello di layout</b>: scegliere un modello di layout per gli utenti. Il modello di layout assegnato agli utenti avrà la precedenza su qualsiasi modello di layout assegnato al loro gruppo predefinito, team predefinito o ruolo principale. Per ulteriori informazioni sulla priorità di assegnazione del modello di layout, vedere <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Creare e gestire modelli di layout</a>.</p> 
        <p><b>NOTA</b>: l'elenco dei modelli di layout disponibili in questo campo dipende dall'accesso:
          <ul>
           <li>In qualità di amministratore di Workfront, puoi visualizzare tutti i modelli di layout a livello di sistema e di gruppo.</li>
           <li>In qualità di amministratore di gruppo, puoi visualizzare i modelli di layout a livello di sistema e quelli associati ai gruppi gestiti.</li>
           <li><p>In qualità di utente con una licenza Planner e con accesso per la modifica degli utenti, puoi visualizzare solo i modelli di layout a livello di sistema. </p>
           <p>Per informazioni sui modelli di layout a livello di gruppo, vedere <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Creare e gestire modelli di layout</a>.</p>
           </li>
          </ul></p> 
          </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Organizzazione</td> 
      <td> 
       <ul> 
        <li><b>Società</b>: la società degli utenti. Gli utenti possono essere associati a una sola azienda. È necessario creare un'azienda prima di associarla a un utente. Nell'elenco vengono visualizzate solo le società attive. Per informazioni sulla creazione di società, consulta Informazioni e gestione delle società.</li> 
        <li><b>Team predefinito</b>: specificare il team predefinito per gli utenti. Gli utenti possono avere un solo team principale. </li> 
        <li><b>Altri team</b>: gli utenti possono appartenere a più team. </li> 
        <li> <p><b>Gruppo predefinito:</b> Selezionare un gruppo appropriato per assegnare gli utenti come gruppo predefinito. In questo modo l'utente può accedere agli oggetti condivisi con il gruppo.</p> <p><b>NOTA</b>: campo obbligatorio. Gli utenti non possono essere associati a un gruppo predefinito.</p> <p>È possibile assegnare un gruppo agli utenti solo nelle situazioni seguenti:</p> 
         <ul> 
          <li>Sei un amministratore di Workfront.</li> 
          <li>L'utente corrente è l'amministratore del gruppo.</li> 
          <li>Il gruppo è pubblico.</li> 
         </ul> </li> 
        <li> <p><b>Altri gruppi</b>: gli utenti possono appartenere a più gruppi. È possibile assegnare un gruppo a un utente solo nelle situazioni seguenti:</p> 
         <ul> 
          <li>Sei un amministratore di Workfront.</li> 
          <li>L'utente corrente è l'amministratore del gruppo.</li> 
          <li> <p>Il gruppo è pubblico. </p> 
          <p>Per ulteriori informazioni sui gruppi pubblici, vedere <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Creare un gruppo</a>.</p> 
          <p>Per ulteriori informazioni sui gruppi, vedere <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Panoramica sui gruppi</a>.</p> 
          </li> 
         </ul> 
         </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Pianificazione risorse</td> 
      <td> 
       <ul>

   <li>
       <b>Tempo di lavoro</b>: rappresenta la percentuale del tempo FTE (Full Time Equivalent) a cui l'utente è disponibile per il lavoro effettivo, esclusi i costi comuni. L'orario di lavoro deve essere un numero decimale massimo di 1 e non può essere 0. Ad esempio, una disponibilità del 20% per il lavoro effettivo sarebbe 0,2.

   Il valore predefinito del campo è 1, che indica che un utente spende l’intero FTE per il lavoro effettivo relativo al progetto.

   Il sistema utilizza questo numero per calcolare la disponibilità dell&#39;utente per il lavoro effettivo correlato al progetto.

   Per ulteriori informazioni sulla creazione di pianificazioni in Workfront, vedere <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Creare una pianificazione</a>.

   Eccezioni alla pianificazione e indisponibilità potrebbero influire anche sulla capacità dell&#39;utente.

   Workfront calcola la disponibilità di un utente in base alle preferenze di Gestione risorse nell’area Configura. Per ulteriori informazioni, vedere <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configurare le preferenze di Gestione risorse</a>.

   <b>SUGGERIMENTO</b>

   Impostare il valore Tempo di lavoro su 1 per indicare che l&#39;utente è disponibile per il lavoro correlato al progetto per l&#39;intero equivalente a tempo pieno.
   </li>

   <li><b>Pianifica disattivazione</b>: selezionare questa casella se si desidera pianificare la disattivazione degli utenti dopo un certo periodo di tempo.</li> 
       <li><b>Data disattivazione pianificata</b>: la data dopo la quale gli utenti vengono disattivati. Per ulteriori informazioni sulla pianificazione della disattivazione degli utenti, vedere la sezione <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">Pianificare la disattivazione degli utenti</a> in <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Disattivare o riattivare un utente</a>.</li> 
       <li> <p><b>Ruolo principale</b>: questa è la mansione principale di un utente in Workfront. Per impostazione predefinita, a ogni attività e problema assegnato agli utenti viene assegnata anche questa mansione. I ruoli sono essenziali nella gestione delle risorse. Per ulteriori informazioni sulle mansioni, vedere <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Creare e gestire le mansioni</a></p> <p>È possibile aggiornare questo campo solo se si dispone di una licenza Pianificazione con accesso utente amministrativo o se si è un amministratore Workfront. Per ulteriori informazioni sulla configurazione degli utenti con accesso amministrativo, vedere <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Concedere l'accesso agli utenti</a>.</p> </li> 
       <li>(Condizionale) Se hai selezionato un <b>Ruolo principale</b>, viene visualizzato il campo <b>Percentuale di disponibilità FTE</b>. Specifica la percentuale di tempo delle pianificazioni degli utenti allocata a questa mansione. Il valore predefinito per la percentuale di disponibilità FTE per il ruolo principale è 100%.</li> 
       <li> <p><b>Altri ruoli</b>: gli utenti possono avere più ruoli in Workfront. I ruoli sono essenziali nella gestione delle risorse. Non esiste alcun limite al numero di mansioni che un utente può svolgere. Tuttavia, si consiglia di non assegnare un utente a un numero eccessivamente elevato di ruoli, perché la gestione delle risorse potrebbe diventare troppo complessa per questi utenti.</p> <p>Per ulteriori informazioni sulle mansioni, vedere <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Creare e gestire le mansioni</a>.</p> <p>È possibile aggiornare questo campo solo se si dispone di una licenza Pianificazione con accesso utente amministrativo o se si è un amministratore Workfront. Per ulteriori informazioni sulla configurazione degli utenti con accesso amministrativo, vedere <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Concedere l'accesso agli utenti</a>.</p> </li> 
       <li> <p>(Condizionale) Se hai selezionato uno o più <b>Altri ruoli</b>, per ogni ruolo viene visualizzato il campo <b>Percentuale di disponibilità FTE</b>. Specifica la percentuale di tempo delle pianificazioni degli utenti allocata a ogni mansione. Il valore predefinito per la percentuale di disponibilità FTE per gli altri ruoli è 0%.</p> <p><b>NOTA</b>:  
       <ul> 
       <li>Se Altri ruoli hanno una disponibilità FTE pari a 0%, non vengono visualizzati nella Programmazione delle risorse, a meno che gli utenti non siano assegnati ad attività in questi ruoli.</li> 
       <li> <p>La somma di tutte le percentuali di disponibilità FTE per tutti i ruoli deve essere uguale al 100%. Ogni percentuale di disponibilità FTE calcola le ore disponibili per ogni ruolo per utente nella Programmazione delle risorse. Le ore disponibili per ogni ruolo per utente dipendono dal tempo disponibile per l’utente.</p> <p>Il tempo disponibile per l'utente viene calcolato da Workfront in base al metodo selezionato dall'amministratore Workfront per calcolare l'FTE nelle preferenze di gestione delle risorse.</p> <p>Per ulteriori informazioni sul calcolo della disponibilità per l'utente, vedere <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Panoramica sul calcolo delle ore e dell'FTE per gli utenti e i ruoli nella Programmazione delle risorse</a>.</p> <p>Per ulteriori informazioni sulla configurazione delle preferenze di Gestione risorse, vedere <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configurare le preferenze di Gestione risorse</a>.</p> </li> 
       </ul> </p> </li> 
       <li> <p><b>Pianificazione</b>: associa una pianificazione agli utenti. La pianificazione degli utenti calcola la sequenza temporale delle attività a cui gli utenti sono assegnati.</p> <p>Un amministratore di Workfront o un amministratore di gruppo deve creare una pianificazione prima di associarla agli utenti.</p> <p>Seleziona una pianificazione a livello di sistema o di gruppo per assegnarla agli utenti selezionati.</p> <p>Per ulteriori informazioni sulle pianificazioni a livello di sistema e di gruppo, vedere <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Creare una pianificazione</a>.</p> <p><b>IMPORTANTE</b>: Workfront utilizza la pianificazione di un utente solo quando l'impostazione Calcola disponibilità risorsa utilizzando è impostata su Pianificazione dell'utente. Per informazioni sul modo in cui l'impostazione Calcola disponibilità risorse utilizzando influisce sulla pianificazione utilizzata per Gestione risorse, vedere <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configurare le preferenze di Gestione risorse</a>.</p> </li> 
       <li> <p><b>Profilo scheda orario</b>: associare un profilo scheda orario agli utenti. In questo modo le schede orario vengono generate automaticamente per gli utenti.</p> 
       <p><b>NOTA</b>:  
       <ul> 
       <li>L’elenco dei profili della scheda orario disponibili in questo campo dipende dal tuo accesso:
       <ul>
       <li>In qualità di amministratore di Workfront, puoi visualizzare tutti i profili delle schede orario a livello di sistema e di gruppo.</li>
       <li><p>In qualità di amministratore di gruppo, puoi visualizzare i profili delle schede orario a livello di sistema, nonché quelli associati ai gruppi gestiti.</p></li>
       <li><p>In quanto utente con una licenza Planner e con accesso in modifica agli utenti, puoi visualizzare solo i profili delle schede orario a livello di sistema.</p></li>
       </ul></li> 
       <li>Se si è un amministratore gruppo, tutti gli utenti che si stanno modificando devono essere membri di un gruppo amministrato.</li> 
       </ul> </p> </li> 
       <li><b>Tipo di Ora Predefinito</b>: Selezionare il tipo di Ora predefinito per gli utenti. Questo è il tipo di ora utilizzato per impostazione predefinita quando gli utenti registrano l’ora.</li> 
       <li> <p><b>Tipi di lavoro disponibili</b>: selezionare i tipi di lavoro disponibili per l'utente. Questi tipi di ore sono visibili ovunque in Workfront, dove gli utenti possono registrare l’ora. Un utente può visualizzare solo i tipi di ore abilitati a livello di progetto e di utente.</p> 
       <p>Per ulteriori informazioni sui tipi di ore disponibili per gli utenti, vedere <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">Definire i tipi di ore e la disponibilità</a>.</p> 
       </li> 
       <li> <b>FTE</b>: equivalente a tempo pieno dell'utente. Workfront utilizza questo numero per calcolare la disponibilità dell'utente in base alla pianificazione predefinita solo quando le preferenze di gestione delle risorse a livello di sistema sono impostate su Pianificazione predefinita.

   <p>L’FTE indica la quantità di tempo che l’utente può trascorrere al lavoro. Sono inclusi i costi comuni e il tempo dedicato al lavoro del progetto. Ad esempio, nell’FTE è incluso anche il tempo trascorso nelle riunioni o nella formazione.</p>

   L&#39;FTE deve essere un numero decimale massimo di 1 e non può essere 0. Ad esempio, se il valore FTE è 0,5 e la pianificazione predefinita in Workfront è di 40 ore, l’utente è disponibile per 20 ore alla settimana.

   Il valore predefinito del campo è 1.

   Eccezioni alla pianificazione, l&#39;indisponibilità e il valore di Tempo di lavoro possono influire sulla disponibilità dell&#39;utente.

   Workfront calcola la disponibilità di un utente in base alle preferenze di Gestione risorse nell’area Configura.

   Se le Preferenze di Gestione risorse a livello di sistema sono impostate su La pianificazione dell&#39;utente, il valore specificato in questo campo viene ignorato e l&#39;utente viene considerato disponibile in base a quanto specificato nella programmazione.

   Per ulteriori informazioni, vedere <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configurare le preferenze di Gestione risorse</a>.

   Per ulteriori informazioni sulla creazione di pianificazioni in Workfront, vedere <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Creare una pianificazione</a>.
   </li> 
       <li> <p><b>Pool di Risorse</b>: associa gli utenti ai pool di risorse.</p> <p><b>NOTA</b>: in questo campo vengono visualizzati solo i pool di risorse comuni a tutti gli utenti selezionati. Se gli utenti selezionati non dispongono di pool di risorse condivisi, questo campo è vuoto. Se questo campo è vuoto, i pool di risorse specificati in questo campo sovrascriveranno i singoli pool di risorse.</p> 
       <p>Per ulteriori informazioni sui pool di risorse, vedere <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Panoramica sui pool di risorse </a>.</p> </li> 
       <li><b>Costo orario</b>: la quantità di costo orario per l'utente. </li> 
       <li><b>Fatturazione ad ore</b>: la quantità di fatturazione ad ore per l'utente.</li> 
       <li><b>Forms personalizzato</b>: associa agli utenti un modulo personalizzato esistente. È necessario creare un modulo personalizzato prima di associarlo a un utente. Nell’elenco vengono visualizzati solo i moduli personalizzati attivi. Per informazioni sulla creazione di moduli personalizzati, vedere <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Progettare un modulo con Progettazione moduli</a>.</li> 
       <li><b>Commento</b>: immetti un commento nel campo fornito. Tutti gli utenti selezionati riceveranno una notifica in-app e una notifica e-mail con il tuo commento. Il commento viene visualizzato nella scheda Aggiornamenti del profilo dell’utente.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facoltativo) Nella sezione **Forms personalizzato**, selezionare l&#39;opzione **Ricalcola espressioni personalizzate** per assicurarsi che tutti i campi personalizzati calcolati nei moduli personalizzati allegati agli utenti selezionati siano aggiornati.

1. Fai clic su **Salva modifiche**.
