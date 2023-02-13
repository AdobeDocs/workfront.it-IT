---
title: Configurare le preferenze per attività e problemi per un gruppo
user-type: administrator
product-area: system-administration;user-management;setup
keywords: gruppo, preferenze, compito, problema, sblocca
navigation-topic: create-and-manage-groups
description: Se i gruppi dell’organizzazione devono configurare un’attività o una preferenza per un problema indipendentemente dalla modalità di configurazione a livello di sistema, un amministratore di Adobe Workfront può sbloccare la preferenza. Quindi, in qualità di amministratore del gruppo, puoi configurare la preferenza per il gruppo e questo interesserà tutte le attività o i problemi associati al gruppo.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 6889b94a-1be6-4be9-8397-c38f890f9103
source-git-commit: 7fa4791e19a84d7215e341e8bbde8dd4d4d8ccc6
workflow-type: tm+mt
source-wordcount: '1894'
ht-degree: 3%

---

# Configurare le preferenze per attività e problemi per un gruppo

Se i gruppi dell’organizzazione devono configurare un’attività o una preferenza per un problema indipendentemente dalla modalità di configurazione a livello di sistema, un amministratore di Adobe Workfront può sbloccare la preferenza. Quindi, in qualità di amministratore del gruppo, puoi configurare la preferenza per il gruppo e questo interesserà tutte le attività o i problemi associati al gruppo.

Se ci sono gruppi al di sopra del gruppo che gestisci, i loro amministratori possono farlo anche per il tuo gruppo. Lo stesso vale per gli amministratori di Workfront (per qualsiasi gruppo).

Per informazioni su come l’amministratore di Workfront sblocca le preferenze, consulta [Bloccare o sbloccare le preferenze del progetto per tutti i gruppi del sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

>[!TIP]
>
>La configurazione a livello di gruppo è possibile anche per le preferenze del progetto. Per informazioni, consulta [Configurare le preferenze di progetto per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md).

>[!NOTE]
>
>* In genere, una preferenza sbloccata rimane sbloccata a tempo indeterminato. Se l’amministratore di Workfront lo blocca nuovamente, l’impostazione di sistema ha effetto nuovamente e le impostazioni relative alle preferenze effettuate dagli amministratori del gruppo vengono perse.
>* Le preferenze impostate per il gruppo associato a un progetto hanno la precedenza sulle preferenze impostate per il gruppo Home dell’utente che crea il progetto.
>* Alcune preferenze a livello di gruppo influiscono sui modelli di progetto creati per il gruppo. Per ulteriori informazioni, consulta la sezione . [Visualizza, utilizza e crea modelli per il gruppo dall’area Gruppi](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#view) nell&#39;articolo [Creare e modificare i modelli di progetto di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
>
>* Dopo che un amministratore di Workfront sblocca una preferenza a livello di sistema, puoi configurarla e bloccarla per garantire che tutti gli utenti del gruppo e dei sottogruppi utilizzino la stessa configurazione. Ciò è parallelo alla possibilità che un amministratore di Workfront debba configurare e bloccare una preferenza per tutti gli utenti del sistema. Per ulteriori informazioni, consulta [Bloccare o sbloccare un progetto, un&#39;attività o una preferenza di problema per i sottogruppi](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).
>


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

## Configurare le preferenze relative alle attività sbloccate e ai problemi per un gruppo di livello superiore

>[!TIP]
>
>Se sei un amministratore di Workfront, puoi ignorare i passaggi 1-4 andando su Configurazione > Preferenze progetto > Attività e problemi, quindi cercare il nome del gruppo nella casella in alto nella pagina.

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **Gruppi** ![](assets/groups-icon.png).

1. Fare clic sul nome del gruppo per il quale si desidera configurare l&#39;attività sbloccata e le preferenze relative ai problemi.
1. Nella pagina visualizzata per il gruppo, nel pannello a sinistra, fai clic su **Preferenze attività e problemi**.
1. Nella pagina visualizzata, continuare con una delle 5 sezioni elencate di seguito per configurare le impostazioni per le aree Nuovi valori predefiniti attività, Problemi, Eliminazione, Date effettive e Accesso, quindi fare clic su **Salva**.

   Se passi il cursore sull’icona Blocca ![](assets/lock-toggle-button-dimmed.png) per una preferenza da configurare e viene visualizzata una descrizione comandi per indicare che è bloccato, è possibile chiedere all’amministratore di Workfront di sbloccarlo per tutti i gruppi dell’organizzazione.

   Quando viene sbloccato, tu e gli altri amministratori di gruppo potete configurarlo separatamente per i vostri gruppi. Inoltre, puoi bloccarlo per il gruppo e per tutti i sottogruppi al di sotto del gruppo.

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
      <td role="rowheader">Data di inizio delle nuove attività</td> 
      <td> <p>Determina la data di inizio predefinita per le nuove attività per i project manager. La data di inizio per le nuove attività può essere la data di inizio pianificata del progetto o il giorno in cui l'attività viene creata.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Tipo di Durata </p> </td> 
      <td> <p>Determina la relazione tra il numero di risorse (e la relativa percentuale di allocazione) e la durata o lo sforzo totale per l'attività. Per ulteriori informazioni, consulta <a href="../../../manage-work/tasks/taskdurtn/task-duration-duration-type.md" class="MCXref xref">Tipi di durata e durata dell’attività</a></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo di Reddito</td> 
      <td> <p>Calcola le stime dei ricavi pianificati ed effettivi per un'attività. Quando il <strong>Tipo di ricavo</strong> è impostato su<strong>Non fatturabile</strong>, le ore pianificate e le ore effettive registrate non generano una stima dei ricavi per l'attività e il lavoro sull'attività non contribuisce ai ricavi a livello di progetto.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo Cst</td> 
      <td> <p>Calcola le stime dei costi pianificati ed effettivi per un'attività. Quando è impostato su <strong>Nessun costo</strong>, le ore pianificate e le ore effettive registrate non generano una stima dei costi prevista o effettiva per l'attività e il lavoro sull'attività non contribuisce ai costi a livello di progetto.</p> </td> 
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
      <td> <p>Quando un problema viene convertito in un progetto o un'attività, sia il problema originale che il progetto o l'attività convertiti diventano la risoluzione degli oggetti. Questa impostazione consente di correlare la risoluzione del problema originale alla risoluzione del relativo oggetto risolvibile. Per ulteriori informazioni sulla risoluzione degli oggetti, vedere <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Panoramica sulla risoluzione e risoluzione di oggetti </a>.</p> <p>Affinché questa impostazione abbia effetto, è possibile <strong>Mantenere il problema originale e legarne la risoluzione all'attività</strong> deve essere selezionato.</p> 
       <ul> 
        <li>Quando questa impostazione è abilitata, puoi creare stati personalizzati con la stessa chiave sia per i problemi che per i progetti o le attività. Quando il progetto o l'attività (come oggetto risolvibile) si trasforma in stato personalizzato, la modifica si riflette anche sullo stato del problema. La chiave di stato deve essere la stessa per il problema e lo stato del progetto o dell'attività.</li> 
        <li>Se questa impostazione è disabilitata, lo stato di risoluzione degli oggetti viene impostato automaticamente sullo stato predefinito, anziché su quello personalizzato. Per ulteriori informazioni sugli stati predefiniti, consulta <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">Accedere all’elenco degli stati dei problemi del sistema</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Durante la conversione di un problema in un’attività</td> 
      <td> <p>Le impostazioni in questa sezione determinano cosa accade durante il processo di conversione da un problema all’altro:</p> 
       <ul> 
        <li><strong>Mantenere il problema originale e legarne la risoluzione all'attività</strong>: Durante la conversione, il problema rimane visibile come problema fino al completamento dell’attività. Lo stato del problema cambia automaticamente in Chiuso al completamento dell'attività.</li> 
        <li><strong>Consenti accesso all'attività al contatto primario</strong>: Consente al contatto principale (creatore di problemi) di accedere all’attività per rivedere l’attività, effettuare aggiornamenti e rimanere informato dei suoi progressi</li> 
        <li> <p><strong>Consenti la modifica di queste impostazioni durante la conversione</strong>: Consente all’utente che sta convertendo il problema di modificare queste opzioni durante la conversione di un problema in un’attività.</p> <!--
          Screenshot when possible</p>
         --> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Durante la conversione di un problema in un progetto</td> 
      <td> <p>Le impostazioni in questa sezione determinano cosa accade durante il processo di conversione da un problema all’altro:</p> 
       <ul> 
        <li><strong>Mantenere il problema originale e legarne la risoluzione al progetto</strong>: Durante la conversione, il problema rimane visibile come problema fino al completamento del progetto. Al termine del progetto, lo stato del problema diventa automaticamente Chiuso .</li> 
        <li><strong>Consenti l'accesso al progetto al contatto primario</strong>: Consente al contatto principale (creatore di problemi) di accedere al progetto per rivedere il progetto, effettuare aggiornamenti e rimanere informato dei suoi progressi.</li> 
        <li><strong>Consenti la modifica di queste impostazioni durante la conversione</strong>: Consente all’utente che sta convertendo il problema di modificare le opzioni elencate durante la conversione di un problema in un progetto.</li> 
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
      <td> <p> Consente di determinare se consentire l'eliminazione di attività o problemi in cui vengono registrate ore. Questa opzione è selezionata per impostazione predefinita.</p> 
       <div> 
        <p><b>Suggerimento</b>: Questa impostazione si applica anche all’eliminazione di progetti che hanno attività o problemi con ore di accesso. Questa impostazione non si applica all’eliminazione di progetti in cui il tempo viene registrato direttamente per il progetto. </p> 
        <p>Considera quanto segue:</p> 
        <ul> 
         <li> <p>Quando è selezionata, viene visualizzato un avviso informativo quando si elimina un'attività o un problema. L’avviso ti ricorda che se l’attività o il problema ha registrato ore, verranno spostati nel progetto o eliminati. È possibile configurare se le ore vengono eliminate o spostate nel progetto nell'area Preferenze foglio presenze e ore dell'impostazione. Dopo aver confermato di aver visualizzato l’avviso, l’attività o il problema viene eliminato. Per ulteriori informazioni sulla configurazione delle preferenze per schede attività e ore, vedere <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref">Configurare le preferenze relative a schede attività e ora</a>. </p> <p>Suggerimento: <span>Quando si elimina un progetto con attività e problemi che hanno registrato ore, le ore registrate vengono eliminate o mantenute in base alle impostazioni nell'area Preferenze foglio presenze e ore di Configurazione</span>. </p> </li> 
         <li><span>Quando si deseleziona questa opzione, viene visualizzato un avviso di divieto quando si elimina un'attività o un problema relativo alle ore registrate oppure quando si elimina un progetto con ore registrate per le attività o i problemi relativi</span> <span>.</span> L'avviso specifica che l'amministratore non consente l'eliminazione di attività o problemi relativi alle ore registrate. Compiti, problemi<span>, o progetti con ore di registrazione per attività e problemi</span> non può essere eliminato. </li> 
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
      <td role="rowheader">Quando un'attività o un problema va da "Nuovo" a "In corso", impostare la data di inizio effettiva su</td> 
      <td> <p>Selezionare una delle opzioni seguenti per quando la data di inizio effettivo viene registrata in Workfront quando un'attività o un problema viene generato <strong>Nuovo</strong> a <strong>In corso</strong>:</p> 
       <ul> 
        <li><strong>Ora:</strong> La data di inizio effettivo è impostata sulla data corrente.</li> 
        <li><strong>La Data Di Inizio Pianificata:</strong> La data di inizio effettiva è impostata sulla data di inizio pianificata dell'attività o del problema.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Quando un'attività o un problema è completato, impostare la data di completamento effettiva su</td> 
      <td> <p>Selezionare una delle opzioni seguenti per la registrazione della data di completamento effettiva in Workfront al completamento di un'attività o di un problema:</p> 
       <ul> 
        <li><strong>Ora:</strong> La data di completamento effettivo è impostata sulla data corrente.</li> 
        <li> <p><strong>La Data Di Completamento Pianificata:</strong> La data di completamento effettivo è impostata sulla data di completamento pianificata dell'attività o del problema.</p> </li> 
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
      <td role="rowheader">Quando un utente viene assegnato a un'attività</td> 
      <td> 
       <ul> 
        <li><strong>Dare loro ... accesso a un'attività</strong>: Definisce l'autorizzazione predefinita di un utente per l'attività a cui è assegnato. Per ulteriori informazioni sulle autorizzazioni delle attività, consulta<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref"> Concedere l’accesso agli utenti</a>.</li> 
        <li> <p><strong>Consentire loro ... di accedere al progetto</strong>: Definisce l'autorizzazione predefinita di un utente al progetto a cui è assegnato un task. Per ulteriori informazioni sulle autorizzazioni del progetto, consulta <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurare le preferenze del progetto a livello di sistema</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Quando un utente viene assegnato a un problema</td> 
      <td> 
       <ul> 
        <li><strong>Dare loro ... accesso a un'attività</strong>: Definisce l'autorizzazione predefinita di un utente per l'attività a cui è assegnato. Per ulteriori informazioni sulle autorizzazioni delle attività, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Concedere l’accesso agli utenti</a>.</li> 
        <li> <p><strong>Consentire loro ... di accedere al progetto</strong>: Definisce l'autorizzazione predefinita di un utente al progetto a cui è assegnato un task. Per ulteriori informazioni sulle autorizzazioni del progetto, consulta <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurare le preferenze del progetto a livello di sistema</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Quando qualcuno invia una richiesta</td> 
      <td> 
       <ul> 
        <li><strong>Dare loro ... accesso al problema</strong>: Definisce l'autorizzazione predefinita di un utente per una richiesta inviata. Per ulteriori informazioni, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Condividere un problema</a>.</li> 
        <li> <p><strong>Le persone della stessa società erediteranno le stesse autorizzazioni per tutte le richieste</strong>: Consente agli utenti di visualizzare le richieste inviate da altri utenti della stessa società. Hanno le stesse autorizzazioni per queste richieste che hanno per le proprie richieste inviate.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>
