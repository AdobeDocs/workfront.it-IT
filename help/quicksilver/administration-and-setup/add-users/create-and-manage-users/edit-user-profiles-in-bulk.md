---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Modificare in blocco i profili utente
description: In qualità di amministratore di Adobe Workfront, puoi modificare gli account utente in blocco.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: cb709b2f-659e-4110-81ac-a1ef967d534c
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '2194'
ht-degree: 0%

---

# Modificare in blocco i profili utente

>[!IMPORTANT]
>
>La procedura descritta in questa pagina si applica solo alle organizzazioni che non sono ancora state integrate nell’Admin Console. Se l’organizzazione è stata configurata per Adobe Admin Console, devi eseguire questa azione tramite Adobe Admin Console.
>
>Per istruzioni su come modificare il profilo di un utente in Adobe Admin Console, consulta la sezione &quot;Modifica i dettagli utente&quot; nell’articolo [Caricamento in blocco degli utenti](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html) oppure contatta l’amministratore Adobe Admin Console.
>
>Per un elenco delle procedure che variano a seconda che l’organizzazione sia stata caricata in Adobe Admin Console, consulta [Differenze di amministrazione basate su piattaforma (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Puoi modificare gli account utente in blocco. Quando si modificano in serie gli utenti, solo i campi selezionati in modo specifico vengono aggiornati con le stesse informazioni per tutti gli utenti selezionati. Tutti gli altri campi lasciati non selezionati rimangono invariati per ogni singolo utente, anche se sono diversi per ogni utente.

>[!NOTE]
>
>* Non è possibile modificare in blocco la sezione Informazioni personali dei profili degli utenti perché tali informazioni devono essere univoche per ogni utente.
>* Per garantire la precisione dei dati e prestazioni ottimali, consigliamo di selezionare non più di 2000 utenti alla volta per un editing in serie.
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
   <td role="rowheader">Configurazioni a livello di accesso</td> 
   <td> <p>Devi disporre di una delle seguenti caratteristiche:</p> 
    <ul> 
     <li> <p>Livello di accesso amministratore di sistema. Per informazioni, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente pieno accesso amministrativo</a>. </p> </li> 
     <li> <p><b>Utenti</b> impostazione nel livello di accesso configurato per <b>Modifica</b> accesso, con <b>Crea</b> e almeno uno dei due <b>Amministratore utente</b> opzioni attivate in <b>Ottimizzare le impostazioni</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Di queste due opzioni, se Utente <b>Amministratore (utenti del gruppo)</b> è abilitato, devi essere un amministratore di gruppo di un gruppo in cui l’utente è membro.</p> <p>Per ulteriori informazioni sulla <b>Utenti</b> impostazione in un livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Concedere l’accesso agli utenti</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Modificare account utente in blocco

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Utenti** ![](assets/users-icon-in-main-menu.png).

1. Seleziona più utenti, quindi fai clic sull’icona Modifica ![](assets/edit-icon.png).

1. In **Modifica utente** nella casella visualizzata, modificare una delle seguenti opzioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Preferenze</td> 
      <td> 
       <ul> 
        <li><b>Fuso orario:</b> Il fuso orario degli utenti.</li> 
        <li><b>Impostazioni internazionali</b>: Le impostazioni internazionali preferite degli utenti. Questo influisce sul formato dei numeri e delle date nelle e-mail provenienti da Workfront.</li> 
        <li><b>Mostra percentuale di completamento allo stato dell'aggiornamento</b>: Selezionare questa opzione se si desidera visualizzare una barra della percentuale di completamento all'interno del flusso di aggiornamento delle attività per tutti gli utenti.</li> 
        <li><b>Invia il lavoro da me assegnato alla scheda Lavoro</b>: Selezionare questa opzione se si desidera che tutto ciò che gli utenti assegnano a se stessi venga visualizzato direttamente nella scheda Lavorare su. L’impostazione predefinita consiste nell’elencare tutti gli elementi assegnati a un utente nella relativa scheda Richiesta di lavoro.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notifiche</td> 
      <td>Seleziona le notifiche e-mail che devono essere abilitate per il nuovo utente.<p>Puoi selezionare notifiche digest istantanee e giornaliere. Tutte le notifiche digest giornaliere vengono inviate dopo la stessa ora per tutti gli utenti selezionati. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref">Configurare le notifiche degli eventi per tutti gli utenti del sistema</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Accesso</td> 
      <td> 
       <ul> 
        <li><b>È attivo:</b> Seleziona questo campo per indicare se gli utenti sono attivi. Gli utenti attivi utilizzano una licenza Workfront. Deselezionando il campo, gli utenti vengono disattivati.</li> 
        <li> 
        <p><b>Livello di accesso:</b> Selezionare il livello di accesso da assegnare a questi utenti. Tutti gli utenti selezionati avranno lo stesso livello di accesso.
        </p> 
        <p>Quando assegni un livello di accesso agli utenti, puoi assegnare un livello uguale o inferiore al livello di accesso desiderato. Ad esempio, se il livello di accesso è Planner, non è possibile assegnare il livello di accesso Amministratore. </p>
        <p>Tuttavia, non è possibile assegnare un livello di accesso inferiore al proprio se l’amministratore di Workfront dispone di autorizzazioni abilitate per il livello di accesso che non sono abilitate anche nel proprio (tramite le impostazioni di fine tuning, come descritto in <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>).</p> 
        <p>Per ulteriori informazioni sui livelli di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Configurare l’accesso ad Adobe Workfront</a>.</p> 
         </li> 
        <li> 
        <p><b>Modello di layout</b>: Scegli un modello di layout per gli utenti. Il modello di layout assegnato agli utenti avrà la precedenza su qualsiasi modello di layout assegnato al gruppo principale, al team principale o al ruolo di lavoro principale. Per ulteriori informazioni sulla priorità di assegnazione del modello layout, vedere <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Creare e gestire modelli di layout</a>.</p> 
        <p><b>NOTA</b>: L’elenco dei modelli di layout disponibili in questo campo dipende dall’accesso:
          <ul>
           <li>In qualità di amministratore di Workfront, puoi visualizzare tutti i modelli di layout a livello di sistema e di gruppo.</li>
           <li>Gli amministratori di gruppo possono visualizzare i modelli di layout a livello di sistema e quelli associati ai gruppi gestiti.</li>
           <li><p>In qualità di utente con una licenza Planner e con accesso per modificare gli utenti, puoi visualizzare solo i modelli di layout a livello di sistema. </p>
           <p>Per informazioni sui modelli di layout a livello di gruppo, consulta <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Creare e gestire modelli di layout</a>.</p>
           </li>
          </ul></p> 
          </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Organizzazione</td> 
      <td> 
       <ul> 
        <li><b>Azienda</b>: Società degli utenti. Gli utenti possono essere associati a una sola società. È necessario creare una società prima di poterla associare a un utente. Nell’elenco vengono visualizzate solo le società attive. Per informazioni sulla creazione di società, consulta Comprensione e gestione di società .</li> 
        <li><b>Team principale</b>: Specifica il team principale per gli utenti. Gli utenti possono avere un solo team domestico. </li> 
        <li><b>Altri team</b>: Gli utenti possono appartenere a più team. </li> 
        <li> <p><b>Gruppo principale:</b> Selezionare un gruppo appropriato per assegnare gli utenti come gruppo principale. Questo consente all’utente di accedere agli oggetti condivisi con il gruppo.</p> <p><b>NOTA</b>: Questo campo è obbligatorio. Non è possibile associare utenti a un gruppo home.</p> <p>È possibile assegnare un gruppo agli utenti solo nelle situazioni seguenti:</p> 
         <ul> 
          <li>Sei un amministratore di Workfront.</li> 
          <li>Sei l'amministratore di quel gruppo.</li> 
          <li>Il gruppo è pubblico.</li> 
         </ul> </li> 
        <li> <p><b>Altri gruppi</b>: Gli utenti possono appartenere a più gruppi. È possibile assegnare un gruppo a un utente solo nelle situazioni seguenti:</p> 
         <ul> 
          <li>Sei un amministratore di Workfront.</li> 
          <li>Sei l'amministratore di quel gruppo.</li> 
          <li> <p>Il gruppo è pubblico. </p> 
          <p>Per ulteriori informazioni sui gruppi pubblici, vedi <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Creare un gruppo</a>.</p> 
          <p>Per ulteriori informazioni sui gruppi, consulta <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Panoramica sui gruppi</a>.</p> 
          </li> 
         </ul> 
         </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Pianificazione risorse</td> 
      <td> 
       <ul> 
        <li><b>Disattivazione programmata</b>: Seleziona questa casella se desideri pianificare la disattivazione degli utenti dopo un periodo di tempo.</li> 
        <li><b>Data di disattivazione pianificata</b>: Data dopo la quale gli utenti vengono disattivati. Per ulteriori informazioni sulla pianificazione degli utenti per la disattivazione, consulta la sezione . <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">Pianificare gli utenti per la disattivazione</a> in <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Disattivare o riattivare un utente</a>.</li> 
        <li> <p><b>Ruolo principale</b>: Questo è il ruolo principale di un utente in Workfront. Per impostazione predefinita, a ogni attività e problema a cui sono assegnati gli utenti viene assegnato anche questo ruolo di lavoro. I ruoli di lavoro sono essenziali nella gestione delle risorse. Per ulteriori informazioni sui ruoli di lavoro, consulta <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Creare e gestire ruoli di lavoro</a></p> <p>È possibile aggiornare questo campo solo se si dispone di una licenza Plan con accesso amministrativo per gli utenti o se si è un amministratore Workfront. Per ulteriori informazioni sulla configurazione degli utenti con accesso amministrativo agli utenti, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Concedere l’accesso agli utenti</a>.</p> </li> 
        <li>(Condizionale) Se hai selezionato un <b>Ruolo principale</b>, <b>Percentuale di disponibilità FTE</b> viene visualizzato il campo . Specificare la percentuale di tempo delle pianificazioni degli utenti allocata a questo ruolo di lavoro. Il valore predefinito per la percentuale di disponibilità FTE per il ruolo principale è 100%.</li> 
        <li> <p><b>Altri ruoli</b>: Gli utenti possono avere più ruoli di lavoro in Workfront. I ruoli di lavoro sono essenziali nella gestione delle risorse. Non vi è alcun limite per il numero di ruoli di lavoro che un utente può svolgere. Tuttavia, consigliamo di non assegnare un utente a un numero eccessivo di ruoli di lavoro, perché la gestione delle risorse potrebbe diventare troppo complessa per questi utenti.</p> <p>Per ulteriori informazioni sui ruoli di lavoro, consulta <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Creare e gestire ruoli di lavoro</a>.</p> <p>È possibile aggiornare questo campo solo se si dispone di una licenza Plan con accesso amministrativo per gli utenti o se si è un amministratore Workfront. Per ulteriori informazioni sulla configurazione degli utenti con accesso amministrativo agli utenti, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Concedere l’accesso agli utenti</a>.</p> </li> 
        <li> <p>(Condizionale) Se hai selezionato uno o più <b>Altri ruoli</b>, <b>Percentuale di disponibilità FTE</b> viene visualizzato un campo per ciascun ruolo. Specificare la percentuale di tempo delle pianificazioni degli utenti allocata a ciascun ruolo di lavoro. Il valore predefinito per la percentuale di disponibilità FTE per gli altri ruoli è 0%.</p> <p><b>NOTA</b>:  
          <ul> 
           <li>Se la disponibilità di altri ruoli è pari a 0%, questi non vengono visualizzati nel Planner risorse, a meno che gli utenti non siano assegnati a attività in questi ruoli.</li> 
           <li> <p>La somma di tutte le percentuali di disponibilità FTE per tutti i ruoli deve essere uguale al 100%. Ogni percentuale di disponibilità FTE calcola le ore disponibili per ogni ruolo per utente nel Resource Planner. L’orario disponibile per ogni ruolo per utente dipende dal tempo disponibile per l’utente.</p> <p>Il tempo disponibile per l’utente viene calcolato da Workfront in base al metodo selezionato dall’amministratore Workfront per calcolare l’ETP nelle Preferenze di gestione delle risorse.</p> <p>Per ulteriori informazioni sul calcolo della disponibilità per l'utente, consulta <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Panoramica del calcolo delle ore e degli FTE per utenti e ruoli nel Planner risorse</a>.</p> <p>Per ulteriori informazioni sulla configurazione delle preferenze di Gestione risorse, consulta <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configurare le preferenze di Gestione risorse</a>.</p> </li> 
          </ul> </p> </li> 
        <li> <p><b>Pianificazione</b>: Associa una pianificazione agli utenti. La pianificazione degli utenti calcola la cronologia delle attività a cui sono assegnati gli utenti.</p> <p>Per poter essere associato agli utenti, un amministratore di Workfront o un amministratore di gruppo deve creare una pianificazione.</p> <p>Selezionare una pianificazione a livello di sistema o di gruppo per assegnarla agli utenti selezionati.</p> <p>Per ulteriori informazioni sulle pianificazioni a livello di sistema e di gruppo, consulta <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Creare una pianificazione</a>.</p> <p><b>IMPORTANTE</b>: Workfront utilizza la pianificazione di un utente solo quando l’impostazione Calcola disponibilità risorse utilizzando è impostata su Pianificazione dell’utente. Per informazioni su come l'impostazione Calcola disponibilità risorse utilizzando influisce sulla pianificazione utilizzata per la gestione delle risorse, vedere <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configurare le preferenze di Gestione risorse</a>.</p> </li> 
        <li> <p><b>Profilo scheda attività</b>: Associa un profilo scheda attività agli utenti. In questo modo i fogli presenze vengono generati automaticamente per gli utenti.</p> 
        <p><b>NOTA</b>:  
          <ul> 
           <li>L'elenco dei profili della scheda attività disponibili in questo campo dipende dall'accesso:
            <ul>
             <li>In qualità di amministratore di Workfront, è possibile visualizzare tutti i profili della scheda attività a livello di sistema e di gruppo.</li>
             <li><p>In qualità di amministratore di gruppo, è possibile visualizzare i profili della scheda attività a livello di sistema e quelli associati ai gruppi gestiti.</p></li>
             <li><p>In qualità di utente con una licenza Planner e accesso per modificare gli utenti, è possibile visualizzare solo i profili della scheda attività a livello di sistema.</p></li>
            </ul></li> 
           <li>Se sei un amministratore di gruppo, tutti gli utenti che stai modificando devono essere membri di un gruppo che amministri.</li> 
          </ul> </p> </li> 
        <li><b>Tipo orario predefinito</b>: Seleziona il tipo di ora predefinito per gli utenti. Questo è il tipo di ora utilizzato per impostazione predefinita quando l’utente registra l’ora.</li> 
        <li> <p><b>Tipi di ora disponibili</b>: Seleziona i tipi di ora che devono essere disponibili per l’utente. Questi tipi di ora sono visibili ovunque in Workfront, dove gli utenti possono registrare il tempo. Un utente può visualizzare solo i tipi di ora abilitati a livello di progetto e a livello di utente.</p> 
        <p>Per ulteriori informazioni sui tipi di ora disponibili per gli utenti, consulta <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">Definire i tipi di ora e la disponibilità per i fogli presenze</a>.</p> 
        </li> 
        <li> <p><b>FTE</b>: Il numero specificato viene preso in considerazione per calcolare la disponibilità dell'utente in base alla pianificazione predefinita solo quando le preferenze di gestione delle risorse a livello di sistema sono impostate su <b>Pianificazione predefinita</b>.</p> 
        <p>Ad esempio, se il valore FTE è 0,5 e la pianificazione predefinita è 40 ore, l’utente può lavorare 20 ore alla settimana. Per ulteriori informazioni su come le eccezioni di pianificazione o il tempo di inattività potrebbero influire sulla disponibilità dell'utente quando è selezionata la pianificazione predefinita, vedere <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configurare le preferenze di Gestione risorse</a>. </p> 
        <p>Se le preferenze di Gestione risorse a livello di sistema sono impostate su <b>Pianificazione dell'utente</b>, il valore specificato viene ignorato e l’utente viene considerato disponibile in base a quanto specificato nella pianificazione. In questo caso, l’FTE dell’utente per il Planner risorse viene calcolato dalla seguente formula:</p>
        <p><code style="font-style: normal;">User Available FTE = Hours from the Schedule of the User/ Default Schedule Hours</code> </p> <p>Per ulteriori informazioni sul calcolo dell’FTE per l’utente, consulta <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Panoramica del calcolo delle ore e degli FTE per utenti e ruoli nel Planner risorse</a>.</p> <p>Per ulteriori informazioni sulla creazione di pianificazioni in Workfront, vedi <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Creare una pianificazione</a>.</p> <p>Per ulteriori informazioni sulla configurazione delle preferenze di gestione delle risorse, consulta <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configurare le preferenze di Gestione risorse</a>.</p> 
        </li> 
        <li> <p><b>Pool di risorse</b>: Associa gli utenti ai pool di risorse.</p> <p><b>NOTA</b>: In questo campo vengono visualizzati solo i pool di risorse comuni a tutti gli utenti selezionati. Se gli utenti selezionati non dispongono di pool di risorse condivise, questo campo è vuoto. Se questo campo è vuoto, i pool di risorse specificati in questo campo sovrascriveranno i singoli pool di risorse.</p> 
        <p>Per ulteriori informazioni sui pool di risorse, consulta <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Panoramica dei pool di risorse </a>.</p> </li> 
        <li><b>Costo/ora</b>: Importo del costo all'ora per l'utente. </li> 
        <li><b>Fatturazione per ora</b>: La quantità di fatturazione all'ora per l'utente.</li> 
        <li><b>Forms personalizzato</b>: Associa un modulo personalizzato utente esistente agli utenti. È necessario creare un modulo personalizzato prima di poterlo associare a un utente. Nell’elenco vengono visualizzati solo i moduli personalizzati attivi. Per informazioni sulla creazione di moduli personalizzati, vedere <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Creare o modificare un modulo personalizzato</a>.</li> 
        <li><b>Commento</b>: Immetti un commento nel campo fornito. Tutti gli utenti selezionati riceveranno una notifica in-app e una notifica e-mail con il tuo commento. Il commento viene visualizzato nella scheda Aggiornamenti del profilo dell’utente.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facoltativo) In **Forms personalizzato** seleziona la sezione **Ricalcola espressioni personalizzate** per garantire che tutti i campi personalizzati calcolati nei moduli personalizzati allegati agli utenti selezionati siano aggiornati.

1. Fai clic su **Salva modifiche**.
