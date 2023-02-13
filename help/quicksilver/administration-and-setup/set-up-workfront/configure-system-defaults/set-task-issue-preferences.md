---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Configurare le preferenze relative alle attività e ai problemi a livello di sistema
description: È possibile configurare le preferenze a livello di sistema per attività e problemi. Queste preferenze influiscono sul modo in cui gli utenti creano attività e problemi in Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 8b99f939-12fe-4470-9dc8-f8a92c6db334
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '2089'
ht-degree: 1%

---

# Configurare le preferenze relative alle attività e ai problemi a livello di sistema

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
Linked to Converting Issues.-->

Come [!DNL Adobe Workfront] amministratore, puoi configurare le preferenze a livello di sistema per attività e problemi. Queste preferenze influiscono sul modo in cui gli utenti creano attività e problemi in [!DNL Workfront].

Per impostazione predefinita, le preferenze relative a attività e problemi sono bloccate e gli amministratori di gruppo non possono modificarle a livello di gruppo a meno che non le sbloccate per tutti i gruppi in tutto il sistema. Per ulteriori informazioni, consulta la sezione . [Bloccare le preferenze di attività ed emissione per i gruppi](#lock-task-and-issue-preferences-for-groups) in questo articolo.

<!--SPLIT OUT BOTTOM SECTION TO NEW ARTICLE?-->

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso</td> 
   <td> <p>Devi essere un [!DNL Workfront] amministratore.</p> <p><b>NOTA</b>: Se non hai ancora accesso, chiedi [!DNL Workfront] amministratore se imposta ulteriori restrizioni nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configura le preferenze per le attività e i problemi per tutti gli utenti di [!DNL Workfront]

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **[!UICONTROL Preferenze del progetto]** >**[!UICONTROL Attività e problemi].**

1. Nella pagina visualizzata, continua con una delle 5 sezioni elencate di seguito per configurare le impostazioni per [!UICONTROL Nuovi valori predefiniti attività], [!UICONTROL Problemi], [!UICONTROL Eliminazione], [!UICONTROL Date effettive]e [!UICONTROL Accesso].
1. Fai clic su **[!UICONTROL Salva]**.

* [[!UICONTROL Nuovi valori predefiniti attività]](#new-task-defaults)
* [[!UICONTROL Problemi]](#issues)
* [[!UICONTROL Eliminazione]](#deletion)
* [[!UICONTROL Date effettive]](#actual-dates)
* [[!UICONTROL Delega]](#delegation)

   <!--
  <li class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#work-on-it" class="MCXref xref">Work On It</a> </li>
  -->

* [[!UICONTROL Accesso]](#access)

### [!UICONTROL Nuovi valori predefiniti attività] {#new-task-defaults}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data di inizio sulle nuove attività]</td> 
   <td> <p>Determina la data di inizio predefinita per le nuove attività per i project manager. La data di inizio per le nuove attività può essere la data di inizio pianificata del progetto o il giorno in cui l'attività viene creata.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Tipo di durata] </p> </td> 
   <td> <p>Determina la relazione tra il numero di risorse (e la relativa percentuale di allocazione) e la durata o lo sforzo totale per l'attività. Per ulteriori informazioni, consulta <a href="../../../manage-work/tasks/taskdurtn/task-duration-duration-type.md" class="MCXref xref">Tipi di durata e durata dell’attività</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di ricavi]</td> 
   <td> <p>Calcola le stime dei ricavi pianificati ed effettivi per un'attività. Quando il <strong>[!UICONTROL Tipo di ricavi]</strong> è impostato su<strong>[!UICONTROL Non fatturabile]</strong>, le ore pianificate e le ore effettive registrate non generano una stima dei ricavi per l'attività e il lavoro sull'attività non contribuisce ai ricavi a livello di progetto.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di costo]</td> 
   <td> <p>Calcola le stime dei costi pianificati ed effettivi per un'attività. Quando è impostato su <strong>[!UICONTROL Nessun costo]</strong>, le ore pianificate e le ore effettive registrate non generano una stima dei costi prevista o effettiva per l'attività e il lavoro sull'attività non contribuisce ai costi a livello di progetto.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Problemi {#issues}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Aggiorna automaticamente lo stato del problema risolvibile quando cambia lo stato dell'oggetto di risoluzione]</td> 
   <td> <p>Quando un problema viene convertito in un progetto o un'attività, sia il problema originale che il progetto o l'attività convertiti diventano la risoluzione degli oggetti. Questa impostazione consente di correlare la risoluzione del problema originale alla risoluzione del relativo oggetto risolvibile. Per ulteriori informazioni sulla risoluzione degli oggetti, vedere <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Panoramica sulla risoluzione e risoluzione di oggetti </a>.</p> <p>Affinché questa impostazione abbia effetto, è possibile <strong>[!UICONTROL Mantieni il problema originale e collega la sua risoluzione all'attività]</strong> deve essere selezionato.</p> 
    <ul> 
     <li>Quando questa impostazione è abilitata, puoi creare stati personalizzati con la stessa chiave sia per i problemi che per i progetti o le attività. Quando il progetto o l'attività (come oggetto risolvibile) si trasforma in stato personalizzato, la modifica si riflette anche sullo stato del problema. La chiave di stato deve essere la stessa per il problema e lo stato del progetto o dell'attività.</li> 
     <li>Se questa impostazione è disabilitata, lo stato di risoluzione degli oggetti viene impostato automaticamente sullo stato predefinito, anziché su quello personalizzato. Per ulteriori informazioni sugli stati predefiniti, consulta <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">Accedere all’elenco degli stati dei problemi del sistema</a>.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader" [!UICONTROL>Durante la conversione di un problema in un'attività]</td> 
   <td> <p>Le impostazioni in questa sezione determinano cosa accade durante il processo di conversione da un problema all’altro:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mantieni il problema originale e collega la sua risoluzione all'attività]</strong>: Durante la conversione, il problema rimane visibile come problema fino al completamento dell’attività. Al termine dell’attività, lo stato del problema diventa automaticamente [!UICONTROL Closed]. Quando questa opzione è deselezionata, il problema viene eliminato.</p> <p><b>NOTA</b>:  <p>Gli utenti senza accesso o autorizzazioni per eliminare i problemi non saranno in grado di eliminare il problema durante la conversione, indipendentemente dallo stato di questa impostazione. Per informazioni sull’accesso e le autorizzazioni per i problemi, consulta:</p> 
       <ul> 
        <li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Concedere l’accesso ai problemi</a> </p> </li> 
        <li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Condividere un problema </a> </p> </li> 
       </ul> </p> </li> 
     <li><strong>[!UICONTROL Consenti accesso all'attività al contatto primario]</strong>: Consente al contatto principale (creatore di problemi) di accedere all’attività per rivedere l’attività, effettuare aggiornamenti e rimanere informato dei suoi progressi</li> 
     <li> <p><strong>[!UICONTROL Consenti la modifica di queste impostazioni durante la conversione]</strong>: Consente all’utente che sta convertendo il problema di modificare queste opzioni durante la conversione di un problema in un’attività.</p> <!--
       Screenshot when possible</p>
      --> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Durante la conversione di un problema in un progetto]</td> 
   <td> <p>Le impostazioni in questa sezione determinano cosa accade durante il processo di conversione da un problema all’altro:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mantenere il problema originale e legarne la risoluzione al progetto]</strong>: Durante la conversione, il problema rimane visibile come problema fino al completamento del progetto. Al termine del progetto, lo stato del problema diventa automaticamente [!UICONTROL Closed]. Quando questa opzione è deselezionata, il problema viene eliminato. </p> <p><b>NOTA</b>:  <p>Gli utenti senza accesso o autorizzazioni per eliminare i problemi non saranno in grado di eliminare il problema durante la conversione, indipendentemente dallo stato di questa impostazione. Per informazioni sull’accesso e le autorizzazioni per i problemi, consulta:</p> 
       <ul> 
        <li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Concedere l’accesso ai problemi</a> </p> </li> 
        <li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Condividere un problema </a> </p> </li> 
       </ul> </p> </li> 
     <li><strong>[!UICONTROL Consenti accesso al progetto al contatto primario]</strong>: Consente al contatto principale (creatore di problemi) di accedere al progetto per rivedere il progetto, effettuare aggiornamenti e rimanere informato dei suoi progressi.</li> 
     <li><strong>[!UICONTROL Consenti la modifica di queste impostazioni durante la conversione]</strong>: Consente all’utente che sta convertendo il problema di modificare le opzioni elencate durante la conversione di un problema in un progetto.</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Eliminazione] {#deletion}

**[!UICONTROL Consenti agli utenti di eliminare attività e problemi relativi alle ore registrate]**: Consente di determinare se consentire l&#39;eliminazione di attività o problemi in cui vengono registrate ore. Questa opzione è selezionata per impostazione predefinita.

>[!TIP]
>
>Questa impostazione si applica anche all’eliminazione di progetti che hanno attività o problemi con ore di accesso. Questa impostazione non si applica all’eliminazione di progetti in cui il tempo viene registrato direttamente per il progetto.

* Quando è selezionata, viene visualizzato un avviso informativo quando si elimina un&#39;attività o un problema. L’avviso ti ricorda che se l’attività o il problema ha registrato ore, verranno spostati nel progetto o eliminati. Puoi configurare se le ore vengono eliminate o spostate nel progetto nel [!UICONTROL Preferenze scheda attività e ora] area [!UICONTROL Configurazione]. Dopo aver confermato di aver visualizzato l’avviso, l’attività o il problema viene eliminato. Per ulteriori informazioni sulla configurazione delle preferenze per schede attività e ore, vedere [Configurare le preferenze relative a schede attività e ora](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

   >[!TIP]
   >
   >Quando elimini un progetto con attività e problemi che hanno registrato ore, le ore registrate vengono eliminate o mantenute in base alle impostazioni nella [!UICONTROL Preferenze scheda attività e ora] area [!UICONTROL Configurazione]. Il messaggio di avviso non viene visualizzato quando si elimina un progetto.

* Quando si deseleziona questa opzione, viene visualizzato un avviso proibitivo quando si elimina un&#39;attività o un problema relativo alle ore registrate o quando si elimina un progetto con ore registrate per le attività o i problemi relativi. L&#39;avviso specifica che l&#39;amministratore non consente l&#39;eliminazione di attività o problemi relativi alle ore registrate. Non è possibile eliminare le attività, i problemi o i progetti per i quali sono registrate ore di lavoro per attività e problemi.

### [!UICONTROL Date effettive] {#actual-dates}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Quando un'attività o un problema va da "Nuovo" a "In corso", imposta la data di inizio effettiva su]</td> 
   <td> <p>Selezionare una delle opzioni seguenti per la registrazione della data di inizio effettiva [!DNL Workfront] quando un'attività o un problema viene da <strong>[!UICONTROL Nuovo]</strong> a <strong>[!UICONTROL In Corso]</strong>:</p> 
    <ul> 
     <li><strong>[!UICONTROL Now]:</strong> La data di inizio effettivo è impostata sulla data corrente.</li> 
     <li><strong>[!UICONTROL La Data Di Inizio Pianificata]:</strong> La data di inizio effettiva è impostata sulla data di inizio pianificata dell'attività o del problema.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Quando un'attività o un problema viene completato, imposta la data di completamento effettivo su]</td> 
   <td> <p>Selezionare una delle opzioni seguenti per la registrazione della data di completamento effettiva [!DNL Workfront] al completamento di un'attività o di un problema:</p> 
    <ul> 
     <li><strong>[!UICONTROL Now]:</strong> La data di completamento effettivo è impostata sulla data corrente.</li> 
     <li> <p><strong>[!UICONTROL La Data Di Completamento Pianificata]:</strong> La data di completamento effettivo è impostata sulla data di completamento pianificata dell'attività o del problema.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Delega

Abilitazione della [!UICONTROL Consenti agli utenti di delegare le loro attività e i loro problemi] consente a tutti gli utenti di in di delegare temporaneamente il proprio lavoro ad altri.

Quando questa impostazione è abilitata, gli utenti possono vedere quanto segue:

* La [!UICONTROL Delega] collegamento [!UICONTROL Pagina principale] area. Possono delegare le approvazioni, le attività e le assegnazioni da qui.
* Indicazione che un&#39;attività o un problema viene delegato a un altro utente nel [!UICONTROL Assegnazioni e delegazioni] nell&#39;intestazione dell&#39;attività o del problema.

Se disattivi la [!UICONTROL Consenti agli utenti di delegare le loro attività e i loro problemi] le delegazioni attualmente pianificate si fermeranno e gli utenti delegati riceveranno una notifica e-mail dell’arresto della delega.

Per informazioni sulla delega del lavoro ad altri, vedere i seguenti articoli:

* [Panoramica sul lavoro delegato](../../../manage-work/delegate-work/delegate-work-overview.md)
* [Gestione dell&#39;attività e della delega dei problemi](../../../manage-work/delegate-work/how-to-delegate-work.md)

<!--
<p><strong>Work On It</strong></p>
This was a Ninja story in Summer/Fall 2020 that may never be implemented Leaving it here drafted in case Ninja decides to add it.</p>
Here's what Jeremy Flores says on 12/1/20:</p>
I have not had a chance to follow up with customers to verify if this is still a need. It has not come up organically. I can follow up with a few customers, but overall I would say that we're probably safe to move on and just mark what we've done to support this as complete. It could still come up but I don't want to push it unless customers really want it.</p>
<p>You can replace the Work On It button with a Start button. When a user assigned to a task or issue clicks Start, the status and Actual Start Date of the work item update automatically, letting others know that the user started work.</p>
<p>Workfront's default Work On It button also signals that a user started work on a task or issue, but it doesn't update the status and Actual Start Date.</p>
<p>To switch to the Start button:</p>
<ol>
<li value="1"> <p>Select <strong>Change the Work On It button to a Start button to automatically update the status of an item</strong>.</p> </li>
<li value="2"> <p>In the lists of check boxes that display below this option, select one or more statuses for each work item type.</p> <p>With multiple statuses selected here, when a user clicks Start on a work item, a drop-down menu lets the user choose a status for the item.</p> </li>
</ol> <note type="note">
<ul class="preview">
<li>Making this change does not affect tasks and issues where the Actual Start Date was already updated. For these, the button displays as Work On It even if it is replaced with the Start button.</li>
<li>If you select New as a status for a work item type (in step 2 above), the Actual Start Date does not update when a user clicks the Start button and then chooses New. This is because a Workfront item is not yet in progress (therefore not yet started) when New is its current status.</li>
<li>This setting is not currently available in
<ul>
<li>The Workfront Mobile App</li>
<li>Workfront for Office 365</li>
<li>Workfront email notifications</li>
</ul></li>
<li>This setting can be configured both at the system level and at the Team level. Enabling the Start button for everyone in the system automatically disables the same setting at the Team level.</li>
<li>If the Work On It setting is enabled, then disabled, tasks and issues function with a Work On It button the way they did before.</li>
</ul>
</note>
-->

### [!UICONTROL Accesso] {#access}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Quando un utente viene assegnato a un'attività]</td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL Concedi loro ... accesso a un’attività]</strong>: Definisce l'autorizzazione predefinita di un utente per l'attività a cui è assegnato. Per ulteriori informazioni sulle autorizzazioni delle attività, consulta<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Concedere l’accesso agli utenti</a>.</li> 
     <li> <p><strong>[!UICONTROL Concedi loro anche ... accesso al progetto]</strong>: Definisce l'autorizzazione predefinita di un utente al progetto a cui è assegnato un task. Per ulteriori informazioni sulle autorizzazioni del progetto, consulta <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurare le preferenze del progetto a livello di sistema</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Quando qualcuno viene assegnato a un problema]</td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL Concedi loro ... accesso a un’attività]</strong>: Definisce l'autorizzazione predefinita di un utente per l'attività a cui è assegnato. Per ulteriori informazioni sulle autorizzazioni delle attività, consulta<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Concedere l’accesso agli utenti</a>.</li> 
     <li> <p><strong>[!UICONTROL Concedi loro anche ... accesso al progetto]</strong>: Definisce l'autorizzazione predefinita di un utente al progetto a cui è assegnato un task. Per ulteriori informazioni sulle autorizzazioni del progetto, consulta <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurare le preferenze del progetto a livello di sistema</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Quando qualcuno invia una richiesta]</td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL Concedi loro ... accesso al problema]</strong>: Definisce l'autorizzazione predefinita di un utente per una richiesta inviata. Per ulteriori informazioni, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Condividere un problema </a>.</li> 
     <li> <p><strong>[!UICONTROL Le persone della stessa azienda erediteranno le stesse autorizzazioni per tutte le richieste]</strong>: Consente agli utenti di visualizzare le richieste inviate da altri utenti della stessa società. Hanno le stesse autorizzazioni per queste richieste che hanno per le proprie richieste inviate.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Bloccare le preferenze di attività ed emissione per i gruppi {#lock-task-and-issue-preferences-for-groups}

Se i gruppi dell’organizzazione necessitano di un’attività o di una preferenza per un problema configurata in modo diverso per i propri flussi di lavoro univoci, puoi sbloccare la preferenza per tutti i gruppi dell’organizzazione in modo che possano configurarla autonomamente. Quando una preferenza viene sbloccata e l&#39;amministratore del gruppo la modifica, le attività o i problemi associati al gruppo vengono influenzati dall&#39;impostazione a livello di gruppo per la preferenza invece che dall&#39;impostazione a livello di sistema.

Per informazioni su come un amministratore del gruppo configura le attività e genera le preferenze per un gruppo, consulta [Configurare le preferenze per attività e problemi per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

>[!NOTE]
>
>Dopo un [!DNL Workfront] l’amministratore sblocca una preferenza a livello di sistema, qualsiasi amministratore di gruppo può configurarla e quindi bloccarla per garantire che tutti i membri del proprio gruppo e dei sottogruppi sottostanti utilizzino la stessa configurazione. Ciò è parallelo alla capacità di un [!DNL Workfront] l’amministratore deve configurare e bloccare una preferenza per tutti gli utenti del sistema. Per ulteriori informazioni, consulta [Configurare le preferenze di progetto per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) e [Bloccare o sbloccare un progetto, un&#39;attività o una preferenza di problema per i sottogruppi](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).

Per bloccare o sbloccare un&#39;attività o una preferenza di problema in modo che i gruppi possano configurarla

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Fai clic su **[!UICONTROL Preferenze del progetto]** > **[!UICONTROL Attività e problemi]**.

1. Effettua una delle seguenti operazioni:

   * Se desideri che gli amministratori dei gruppi al di sotto del tuo gruppo siano in grado di configurare una preferenza per i loro gruppi, sbloccarla ![](assets/unlock-toggle-button.png).
   * Se desideri che il gruppo e tutti i gruppi sottostanti utilizzino la configurazione per una preferenza, accertati che sia bloccato (questa è l’impostazione predefinita).

      >[!IMPORTANT]
      >
      >È consigliabile comunicare con gli amministratori e gli utenti di gruppi in tutto il sistema per garantire che tutte le esigenze siano prese in considerazione nel modo in cui si configura una preferenza bloccata. Quando lo si blocca, la configurazione per esso viene ereditata da tutti i gruppi del sistema. E se la preferenza è stata sbloccata per un qualsiasi periodo di tempo, la configurazione sostituisce quelle che gli amministratori del gruppo potrebbero aver effettuato.

1. Fai clic su **[!UICONTROL Salva]**.
