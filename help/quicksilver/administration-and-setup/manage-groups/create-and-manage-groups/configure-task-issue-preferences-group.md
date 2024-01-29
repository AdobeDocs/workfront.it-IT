---
title: Configurare le preferenze per attività e problemi per un gruppo
user-type: administrator
product-area: system-administration;user-management;setup
keywords: gruppo,preferenze,attività,problema,sblocca
navigation-topic: create-and-manage-groups
description: Se i gruppi dell’organizzazione devono configurare una preferenza per attività o problemi indipendentemente dalla modalità di configurazione a livello di sistema, un amministratore Adobe Workfront può sbloccare la preferenza. Quindi, in qualità di amministratore di gruppo, puoi configurare la preferenza per il gruppo e influenzerà tutte le attività o i problemi associati al gruppo.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 6889b94a-1be6-4be9-8397-c38f890f9103
source-git-commit: 4a9936b6bc034f2176167fc3939d647ee679a888
workflow-type: tm+mt
source-wordcount: '1895'
ht-degree: 2%

---

# Configurare le preferenze per attività e problemi per un gruppo

Se i gruppi dell’organizzazione devono configurare una preferenza per attività o problemi indipendentemente dalla modalità di configurazione a livello di sistema, un amministratore Adobe Workfront può sbloccare la preferenza. Quindi, in qualità di amministratore di gruppo, puoi configurare la preferenza per il gruppo e influenzerà tutte le attività o i problemi associati al gruppo.

Se al di sopra del gruppo gestito sono presenti gruppi, anche gli amministratori possono eseguire questa operazione per il gruppo. Lo stesso vale per gli amministratori di Workfront (per qualsiasi gruppo).

Per informazioni su come l’amministratore di Workfront sblocca le preferenze, consulta [Blocca o sblocca le preferenze di progetto per tutti i gruppi nel sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

>[!TIP]
>
>La configurazione a livello di gruppo è possibile anche per le preferenze di progetto. Per informazioni, consulta [Configurare le preferenze di progetto per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md).

>[!NOTE]
>
>* In genere, una preferenza sbloccata rimane sbloccata a tempo indeterminato. Se l&#39;amministratore di Workfront la sblocca nuovamente, l&#39;impostazione di sistema riprende ad avere effetto e le impostazioni relative alle preferenze impostate dagli amministratori di gruppo andranno perse.
>* Le preferenze impostate per il gruppo associato a un progetto hanno la precedenza su quelle impostate per il gruppo predefinito dell&#39;utente che crea il progetto.
>* Alcune preferenze a livello di gruppo influiscono sui modelli di progetto creati per il gruppo. Per ulteriori informazioni, consulta la sezione [Visualizzare, utilizzare e creare modelli per il gruppo dall&#39;area Gruppi](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#view) nell’articolo [Creare e modificare i modelli di progetto di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
>
>* Dopo che un amministratore di Workfront ha sbloccato una preferenza a livello di sistema, è possibile configurarla e quindi bloccarla per assicurarsi che tutti gli utenti del gruppo e dei relativi sottogruppi utilizzino la stessa configurazione. Ciò è parallelo alla possibilità che un amministratore di Workfront deve configurare e bloccare una preferenza per tutti gli utenti del sistema. Per ulteriori informazioni, consulta [Bloccare o sbloccare una preferenza di progetto, attività o problema per i sottogruppi](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).
>

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Workfront*</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> <p>Devi essere un amministratore di gruppo del gruppo o un amministratore di Workfront. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Amministratori di gruppi</a> e <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente l'accesso amministrativo completo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano o il tipo di licenza disponibile, contattare l&#39;amministratore di Workfront.

## Configurare le preferenze per attività e problemi sbloccati per un gruppo di primo livello

>[!TIP]
>
>Se sei un amministratore di Workfront, puoi evitare i passaggi 1-4 andando in Configurazione > Preferenze progetto > Attività e problemi, quindi cercando il nome del gruppo nella casella nella parte superiore della pagina.

1. Fai clic su **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **Gruppi** ![](assets/groups-icon.png).

1. Fare clic sul nome del gruppo per il quale si desidera configurare le preferenze per attività sbloccate e problemi.
1. Nella pagina visualizzata per il gruppo, nel pannello a sinistra, fai clic su **Preferenze attività e problemi**.
1. Nella pagina visualizzata, continua con una delle 5 sezioni elencate di seguito per configurare le impostazioni per le aree Nuovi valori predefiniti attività, Problemi, Eliminazione, Date effettive e Accesso, quindi fai clic su **Salva**.

   Se passi il cursore sull’icona del lucchetto ![](assets/lock-toggle-button-dimmed.png) per una preferenza da configurare e una descrizione comando che indica che è bloccata, puoi chiedere all’amministratore di Workfront di sbloccarla per tutti i gruppi dell’organizzazione.

   Una volta sbloccato, l’utente e gli altri amministratori di gruppi possono configurarlo separatamente per i propri gruppi. Inoltre, puoi bloccarlo per il tuo gruppo e per tutti i suoi sottogruppi.

   * [Nuovi valori predefiniti attività](#new-task-defaults)
   * [Problemi](#issues)
   * [Eliminazione](#deletion)
   * [Date effettive](#actual-dates)

     <!--   
     <li><a href="#work-on-it" class="MCXref xref">Work On It</a> </li>   
     -->

   * [Accesso](#access)

### Nuovi valori predefiniti attività {#new-task-defaults}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Data di inizio per le nuove attività</td> 
      <td> <p>Determina la data di inizio predefinita per le nuove attività dei project manager. La data di inizio per le nuove attività può essere la data di inizio pianificata del progetto o il giorno in cui l'attività viene creata.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Tipo di Durata </p> </td> 
      <td> <p>Determina la relazione tra il numero di risorse (e la relativa percentuale di allocazione) e la durata o l'impegno totale per l'attività. Per ulteriori informazioni, consulta <a href="../../../manage-work/tasks/taskdurtn/task-duration-duration-type.md" class="MCXref xref">Tipi di durata e durata task: indice articolo</a></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo di Reddito</td> 
      <td> <p>Calcola le stime dei ricavi pianificati ed effettivi per un'attività. Quando <strong>Tipo di retribuzione</strong> è impostato su<strong>Non Fatturabile</strong>, le ore pianificate e quelle effettive registrate non generano una stima dei ricavi per l'attività e il lavoro sull'attività non contribuisce ai ricavi a livello di progetto.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo Cst</td> 
      <td> <p>Calcola le stime dei costi pianificati ed effettivi per un'attività. Se impostato su <strong>Nessun costo</strong>, le ore pianificate e le ore effettive registrate non generano una stima dei costi pianificati o effettivi per l'attività e il lavoro relativo all'attività non contribuisce ai costi a livello di progetto.</p> </td> 
     </tr> 
    </tbody> 
   </table>

### Problemi {#issues}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Aggiorna automaticamente lo stato del problema risolvibile quando lo stato dell'oggetto risolutivo cambia</td> 
      <td> <p>Quando un utente converte un problema in un progetto o in un’attività, sia il problema originale che il progetto o l’attività convertiti diventano oggetti di risoluzione. Questa impostazione consente di correlare la risoluzione del problema originale alla risoluzione del relativo oggetto risolvibile. Per ulteriori informazioni sulla risoluzione degli oggetti, vedere <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Panoramica sugli oggetti risolvibili e risolvibili </a>.</p> <p>Affinché questa impostazione abbia effetto, l'opzione <strong>Mantieni il problema originale e collegane la risoluzione all'attività</strong> deve essere selezionato.</p> 
       <ul> 
        <li>Quando questa impostazione è abilitata, puoi creare stati personalizzati con la stessa chiave sia per i problemi che per i progetti o le attività. Quando il progetto o l’attività (come oggetto risolvibile) diventa lo stato personalizzato, la modifica si riflette anche sullo stato del problema. La chiave dello stato deve essere la stessa per lo stato del problema e per quello del progetto o dell’attività.</li> 
        <li>Quando questa impostazione è disattivata, gli stati degli oggetti di risoluzione vengono impostati automaticamente sullo stato predefinito, anziché su quelli personalizzati. Per ulteriori informazioni sugli stati predefiniti, consulta <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">Accedere all’elenco degli stati dei problemi di sistema</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Quando si converte un problema in un'attività</td> 
      <td> <p>Le impostazioni in questa sezione determinano cosa accade durante il processo di conversione da un problema all’altro:</p> 
       <ul> 
        <li><strong>Mantieni il problema originale e collegane la risoluzione all'attività</strong>: durante la conversione del problema, questo rimane visibile come problema fino al completamento dell’attività. Lo stato del problema diventa automaticamente Chiuso al completamento dell’attività.</li> 
        <li><strong>Consenti al contatto principale di accedere all'attività</strong>: consente al contatto principale (autore del problema) di accedere all’attività per rivederla, apportare aggiornamenti e rimanere informato sul suo avanzamento</li> 
        <li> <p><strong>Consenti la modifica di queste impostazioni durante la conversione</strong>: consente all’utente che converte il problema di modificare queste opzioni durante la conversione di un problema in un’attività.</p> <!--
          Screenshot when possible</p>
         --> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Quando si converte un problema in un progetto</td> 
      <td> <p>Le impostazioni in questa sezione determinano cosa accade durante il processo di conversione da un problema all’altro:</p> 
       <ul> 
        <li><strong>Mantieni il problema originale e collegane la risoluzione al progetto</strong>: durante la conversione del problema, questo rimane visibile come problema fino al completamento del progetto. Lo stato del problema diventa automaticamente Chiuso al completamento del progetto.</li> 
        <li><strong>Consenti al contatto principale di accedere al progetto</strong>: consente al contatto principale (autore del problema) di accedere al progetto per esaminarlo, aggiornarlo e tenersi informato sui suoi progressi.</li> 
        <li><strong>Consenti la modifica di queste impostazioni durante la conversione</strong>: consente all’utente che converte il problema di modificare le opzioni elencate durante la conversione di un problema in un progetto.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

### Eliminazione {#deletion}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Consenti agli utenti di eliminare le attività e i problemi con ore registrate</td> 
      <td> <p> Consente di determinare se consentire l’eliminazione di attività o problemi in cui sono registrate le ore. Questa opzione è selezionata per impostazione predefinita.</p> 
       <div> 
        <p><b>Suggerimento</b>: questa impostazione si applica anche all’eliminazione di progetti con attività o problemi con ore collegate. Questa impostazione non si applica all’eliminazione di progetti in cui il tempo viene registrato direttamente per il progetto. </p> 
        <p>Considera quanto segue:</p> 
        <ul> 
         <li> <p>Quando viene selezionato, quando si elimina un'attività o un problema si riceve un avviso informativo. L’avviso ricorda che se l’attività o il problema ha registrato ore, queste verranno spostate nel progetto o eliminate. Puoi configurare se le ore vengono eliminate o spostate nel progetto nell’area Preferenze scheda orario e ore della Configurazione. Dopo aver confermato di aver visualizzato l’avviso, l’attività o il problema viene eliminato. Per ulteriori informazioni sulla configurazione delle preferenze per i Timesheet e le ore, consulta <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref">Configurare le preferenze di orario e scheda orario</a>. </p> <p>Suggerimento <span>Quando elimini un progetto con attività e problemi che hanno registrato ore, le ore registrate vengono eliminate o vengono mantenute in base alle impostazioni nell’area Preferenze scheda orario e ore della Configurazione</span>. </p> </li> 
         <li><span>Quando deselezioni questa opzione, viene visualizzato un avviso proibitivo quando elimini un’attività o un problema con ore registrate, o quando elimini un progetto con ore registrate per le relative attività o problemi</span> <span>.</span> L'avviso specifica che l'amministratore non consente l'eliminazione di attività o problemi con ore registrate. Le attività, i problemi<span>, o progetti per i quali sono state registrate ore per attività e problemi</span> non può essere eliminato. </li> 
        </ul> 
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

### Date effettive {#actual-dates}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Quando un'attività o un problema passa dallo stato "Nuovo" a "In corso", imposta la data di inizio effettiva su</td> 
      <td> <p>Selezionare una delle seguenti opzioni per la registrazione della data di inizio effettiva in Workfront quando un'attività o un problema inizia <strong>Nuovo</strong> a <strong>In corso</strong>:</p> 
       <ul> 
        <li><strong>Ora:</strong> La data di inizio effettiva viene impostata sulla data corrente.</li> 
        <li><strong>La data di inizio pianificata:</strong> La Data di inizio effettiva è impostata sulla Data di inizio pianificata dell’attività o del problema.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Quando un'attività o un problema è completato, imposta la Data di completamento effettiva su</td> 
      <td> <p>Seleziona una delle seguenti opzioni per quando la Data di completamento effettiva viene registrata in Workfront al completamento di un'attività o di un problema:</p> 
       <ul> 
        <li><strong>Ora:</strong> La data di completamento effettiva è impostata sulla data corrente.</li> 
        <li> <p><strong>La data di completamento pianificata:</strong> La Data di completamento effettiva è impostata sulla Data di completamento pianificata dell’attività o del problema.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

<!--
   This was a Ninja story in Summer/Fall 2020 that may never be implemented Leaving it here drafted in case Ninja decides to add it. Here's what Jeremy Flores says on 12/1/20:
   
   I have not had a chance to follow up with customers to verify if this is still a need. It has not come up organically. I can follow up with a few customers, but overall I would say that we're probably safe to move on and just mark what we've done to support this as complete. It could still come up but I don't want to push it unless customers really want it.
   You can replace the Work On It button with a Start button. When a user assigned to a task or issue clicks Start, the status and Actual Start Date of the work item update automatically, letting others know that the user started work.
   Workfront's default Work On It button also signals that a user started work on a task or issue, but it doesn't update the status and Actual Start Date.

   To switch to the Start button:
   
   Select Change the Work On It button to a Start button to automatically update the status of an item. 
   In the lists of check boxes that display below this option, select one or more statuses for each work item type. With multiple statuses selected here, when a user clicks Start on a work item, a drop-down menu lets the user choose a status for the item. 
     
   Making this change does not affect tasks and issues where the Actual Start Date was already updated. For these, the button displays as Work On It even if it is replaced with the Start button.
   If you select New as a status for a work item type (in step 2 above), the Actual Start Date does not update when a user clicks the Start button and then chooses New. This is because a Workfront item is not yet in progress (therefore not yet started) when New is its current status.
   This setting is not currently available in
   
   The Workfront Mobile App
   Workfront for Office 365
   Workfront email notifications
   
   This setting can be configured both at the system level and at the Team level. Enabling the Start button for everyone in the system automatically disables the same setting at the Team level.
   If the Work On It setting is enabled, then disabled, tasks and issues function with a Work On It button the way they did before.
   -->

### Accesso {#access}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Quando a un utente viene assegnata un'attività</td> 
      <td> 
       <ul> 
        <li><strong>Concedi loro l'accesso a un'attività</strong>: definisce l’autorizzazione predefinita di un utente per l’attività a cui è assegnato. Per ulteriori informazioni sulle autorizzazioni per le attività, consulta<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref"> Concedere l’accesso agli utenti</a>.</li> 
        <li> <p><strong>Concedi loro anche ... l'accesso al progetto</strong>: definisce l’autorizzazione predefinita di un utente per il progetto al quale è stata assegnata un’attività. Per ulteriori informazioni sulle autorizzazioni per i progetti, consulta <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurare le preferenze di progetto a livello di sistema</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Quando a un utente viene assegnato un problema</td> 
      <td> 
       <ul> 
        <li><strong>Concedi loro l'accesso a un'attività</strong>: definisce l’autorizzazione predefinita di un utente per l’attività a cui è assegnato. Per ulteriori informazioni sulle autorizzazioni per le attività, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Concedere l’accesso agli utenti</a>.</li> 
        <li> <p><strong>Concedi loro anche ... l'accesso al progetto</strong>: definisce l’autorizzazione predefinita di un utente per il progetto al quale è stata assegnata un’attività. Per ulteriori informazioni sulle autorizzazioni per i progetti, consulta <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurare le preferenze di progetto a livello di sistema</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Quando qualcuno invia una richiesta</td> 
      <td> 
       <ul> 
        <li><strong>Concedi loro ... l'accesso al problema</strong>: definisce l’autorizzazione predefinita di un utente per una richiesta inviata. Per ulteriori informazioni, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Condividere un problema</a>.</li> 
        <li> <p><strong>Le persone della stessa società erediteranno le stesse autorizzazioni per tutte le richieste</strong>: consente agli utenti di visualizzare le richieste inviate da altri utenti della stessa società. Su tali richieste dispongono delle stesse autorizzazioni delle proprie richieste inviate.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>
