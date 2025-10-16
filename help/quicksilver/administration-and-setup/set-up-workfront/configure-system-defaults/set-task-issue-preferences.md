---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Configurare le preferenze per attività e problemi a livello di sistema
description: Puoi configurare le preferenze a livello di sistema per le attività e i problemi. Queste preferenze influiscono sul modo in cui gli utenti creano attività e problemi in Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 8b99f939-12fe-4470-9dc8-f8a92c6db334
source-git-commit: 20ebcb74c79aea67ea7cb1ba083dfea623fe7c16
workflow-type: tm+mt
source-wordcount: '2228'
ht-degree: 0%

---

# Configurare le preferenze relative alle attività e ai problemi a livello di sistema

<!-- Audited: 2/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
Linked to Converting Issues.-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->


In qualità di amministratore [!DNL Adobe Workfront], puoi configurare le preferenze a livello di sistema per le attività e i problemi. Queste preferenze influiscono sul modo in cui gli utenti creano attività e problemi in [!DNL Workfront].

Per impostazione predefinita, le preferenze relative a attività e problemi sono bloccate e gli amministratori dei gruppi non possono modificarle a livello di gruppo a meno che non vengano sbloccate per tutti i gruppi del sistema. Per ulteriori informazioni, vedere la sezione [Bloccare le attività e le preferenze relative ai problemi per i gruppi](#lock-task-and-issue-preferences-for-groups) in questo articolo.


## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] pacchetto</td> 
   <td><p>Qualsiasi</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licenza</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td>[!UICONTROL Amministratore di sistema]</td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configura le preferenze per attività e problemi per tutti in [!DNL Workfront]

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **[!UICONTROL Preferenze progetto]** >**[!UICONTROL Attività e problemi].**

1. Nella pagina visualizzata, continuare con una delle sei sezioni elencate di seguito per configurare le impostazioni per [!UICONTROL Nuovi valori predefiniti attività], [!UICONTROL Problemi], [!UICONTROL Eliminazione], [!UICONTROL Date effettive] e [!UICONTROL Accesso]:

   * [[!UICONTROL Nuovi valori predefiniti attività]](#new-task-defaults)
   * [[!UICONTROL Problemi]](#issues)
   * [[!UICONTROL Eliminazione]](#deletion)
   * [Sposta](#move)
   * [[!UICONTROL Date effettive]](#actual-dates)
   * [[!UICONTROL Delega]](#delegation)
   * [[!UICONTROL Accedere ad]](#access)


### [!UICONTROL Nuovi valori predefiniti attività] {#new-task-defaults}

<table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td role="rowheader">[!UICONTROL Data Inizio]</td> 
    <td> <p>Determina la data di inizio predefinita per le nuove attività dei project manager. La data di inizio per le nuove attività può essere la data di inizio pianificata del progetto o il giorno in cui l'attività viene creata.</p> </td> 
    </tr> 
    <tr> 
    <td role="rowheader"> <p>Tipo di durata  </p> </td> 
    <td> <p>Determina la relazione tra il numero di risorse (e la relativa percentuale di allocazione) e la durata o l'impegno totale per l'attività. Per ulteriori informazioni, vedere <a href="../../../manage-work/tasks/taskdurtn/task-duration-duration-type.md" class="MCXref xref">Tipi di durata e durata attività</a></p> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL Tipo di retribuzione]</td> 
    <td> <p>Calcola le stime dei ricavi pianificati ed effettivi per un'attività. Quando il tipo di retribuzione <strong></strong> è impostato su <strong>[!UICONTROL Non fatturabile]</strong>, le ore pianificate e le ore effettive registrate non generano una stima dei ricavi per l'attività e il lavoro sull'attività non contribuisce ai ricavi a livello di progetto.</p>
         <p>Per informazioni sui diversi tipi di ricavi, vedere <a href="/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md">Panoramica su fatturazione e ricavi</a>.</p></td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL Tipo di costo]</td> 
    <td> <p>Calcola le stime dei costi pianificati ed effettivi per un'attività. Se impostata su <strong>[!UICONTROL Nessun costo]</strong>, le ore pianificate e le ore effettive registrate non generano una stima dei costi pianificati o effettivi per l'attività e il lavoro svolto non contribuisce ai costi a livello di progetto.</p> </td> 
    </tr> 
  </tbody> 
</table>

### Problemi {#issues}

<table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td role="rowheader">[!UICONTROL Aggiorna automaticamente lo stato del problema risolvibile quando lo stato dell'oggetto risolutivo cambia]</td> 
    <td> <p>Quando un utente converte un problema in un progetto o in un’attività, sia il problema originale che il progetto o l’attività convertiti diventano oggetti di risoluzione. Questa impostazione consente di correlare la risoluzione del problema originale alla risoluzione del relativo oggetto risolvibile. Per ulteriori informazioni sulla risoluzione degli oggetti, vedere <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Panoramica sugli oggetti risolvibili e risolvibili </a>.</p> <p>Affinché questa impostazione abbia effetto, è necessario selezionare l'opzione <strong>[!UICONTROL Mantieni il problema originale e collegarne la risoluzione all'attività]</strong>.</p> 
      <ul> 
      <li>Quando questa impostazione è abilitata, puoi creare stati personalizzati con la stessa chiave sia per i problemi che per i progetti o le attività. Quando il progetto o l’attività (come oggetto risolvibile) diventa lo stato personalizzato, la modifica si riflette anche sullo stato del problema. La chiave dello stato deve essere la stessa per lo stato del problema e per quello del progetto o dell’attività.</li> 
      <li>Quando questa impostazione è disattivata, gli stati degli oggetti di risoluzione vengono impostati automaticamente sullo stato predefinito, anziché su quelli personalizzati. Per ulteriori informazioni sugli stati predefiniti, vedere <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">Accedere all'elenco degli stati dei problemi di sistema</a>.</li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL Quando si converte un problema in un'attività]</td> 
    <td> <p>Le impostazioni in questa sezione determinano cosa accade durante il processo di conversione da un problema all’altro:</p> 
      <ul> 
      <li> <p><strong>[!UICONTROL Mantieni il problema originale e collegane la risoluzione all'attività]</strong>: durante la conversione del problema, questo rimane visibile come problema fino al completamento dell'attività. Lo stato del problema cambia automaticamente in [!UICONTROL Closed] al completamento dell'attività. Se questa opzione è deselezionata, il problema viene eliminato.</p> <p><b>NOTA</b>:  <p>Gli utenti che non dispongono dell’accesso o delle autorizzazioni necessarie per eliminare un problema non potranno eliminarlo mentre lo stanno convertendo, indipendentemente dallo stato di questa impostazione. Per informazioni sull’accesso e le autorizzazioni per i problemi, consulta:</p> 
        <ul> 
          <li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Concedi l'accesso ai problemi</a> </p> </li> 
          <li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Condividi un problema </a> </p> </li> 
        </ul> </p> </li> 
      <li><strong>[!UICONTROL Consenti al contatto principale di accedere all'attività]</strong>: concede al contatto principale (autore del problema) l'accesso in visualizzazione all'attività per esaminarla, tenerne informato l'avanzamento e aggiungere commenti nella sezione Aggiornamenti dell'attività.</li> 
      <li> <p><strong>[!UICONTROL Consenti la modifica di queste impostazioni durante la conversione]</strong>: consente all'utente che converte il problema di modificare queste opzioni durante la conversione di un problema in un'attività.</p></li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL Quando si converte un problema in un progetto]</td> 
    <td> <p>Le impostazioni in questa sezione determinano cosa accade durante il processo di conversione da un problema all’altro:</p> 
      <ul> 
      <li> <p><strong>[!UICONTROL Mantieni il problema originale e collegane la risoluzione al progetto]</strong>: durante la conversione del problema, questo rimane visibile come problema fino al completamento del progetto. Lo stato del problema cambia automaticamente in [!UICONTROL Closed] al completamento del progetto. Se questa opzione è deselezionata, il problema viene eliminato. </p> <p><b>NOTA</b>:  <p>Gli utenti che non dispongono dell’accesso o delle autorizzazioni necessarie per eliminare un problema non potranno eliminarlo mentre lo stanno convertendo, indipendentemente dallo stato di questa impostazione. Per informazioni sull’accesso e le autorizzazioni per i problemi, consulta:</p> 
        <ul> 
          <li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Concedi l'accesso ai problemi</a> </p> </li> 
          <li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Condividi un problema </a> </p> </li> 
        </ul> </p> </li> 
      <li><strong>[!UICONTROL Consenti al contatto principale di accedere al progetto]</strong>: concede al contatto principale (autore del problema) l'accesso in visualizzazione al progetto per esaminarlo, tenerlo informato sullo stato di avanzamento e aggiungere commenti alla sezione Aggiornamenti del progetto.</li> 
      <li><strong>[!UICONTROL Consenti la modifica di queste impostazioni durante la conversione]</strong>: consente all'utente che converte il problema di modificare le opzioni elencate durante la conversione di un problema in un progetto.</li> 
      </ul> </td>
    </tr> 
  </tbody> 
  </table>

### [!UICONTROL Eliminazione] {#deletion}

**[!UICONTROL Consenti agli utenti di eliminare attività e problemi con ore registrate]**: consente di determinare se consentire l&#39;eliminazione di attività o problemi in cui sono registrate ore. Questa opzione è selezionata per impostazione predefinita.

>[!TIP]
>
>Questa impostazione si applica anche all’eliminazione di progetti con attività o problemi con ore collegate. Questa impostazione non si applica all’eliminazione di progetti in cui il tempo viene registrato direttamente per il progetto.

* Quando viene selezionato, quando si elimina un&#39;attività o un problema si riceve un avviso informativo. L’avviso ricorda che se l’attività o il problema ha registrato ore, queste verranno spostate nel progetto o eliminate. Puoi configurare se le ore vengono eliminate o spostate nel progetto nell&#39;area [!UICONTROL Timesheet &amp; Hours Preferences] della [!UICONTROL Configurazione]. Dopo aver confermato di aver visualizzato l’avviso, l’attività o il problema viene eliminato. Per ulteriori informazioni sulla configurazione delle preferenze per le ore e la scheda orario, vedere [Configurare le preferenze per le ore e la scheda orario](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

  >[!TIP]
  >
  >Quando elimini un progetto con attività e problemi che hanno registrato ore, le ore registrate vengono eliminate o vengono mantenute in base alle impostazioni nell&#39;area [!UICONTROL Preferenze schede orario e ore] di [!UICONTROL Configurazione]. Il messaggio di avviso non viene visualizzato quando si elimina un progetto.

* Quando deselezioni questa opzione, viene visualizzato un avviso proibitivo quando elimini un’attività o un problema con ore registrate o quando elimini un progetto con ore registrate per le relative attività o problemi. L&#39;avviso specifica che l&#39;amministratore non consente l&#39;eliminazione di attività o problemi con ore registrate. Impossibile eliminare le attività, i problemi o i progetti per i quali sono state registrate ore per attività e problemi.

### Sposta

**[!UICONTROL Consenti agli utenti di spostare attività e problemi con ore registrate]**: consente di determinare se consentire lo spostamento di attività o problemi in cui sono registrate ore. Questa opzione è selezionata per impostazione predefinita.

* Quando è selezionato, puoi spostare le attività e i problemi con tempo registrato. Le ore vengono spostate anche con le attività o i problemi.

* Quando deselezioni questa opzione, ricevi un avviso proibitivo quando sposti un’attività o un problema con ore registrate in un altro progetto. L&#39;avviso specifica che l&#39;amministratore non consente lo spostamento di attività o problemi con ore registrate. Impossibile spostare le attività o i problemi con ore registrate. È possibile spostare le attività all’interno dello stesso progetto, anche quando questa opzione è deselezionata.

### [!UICONTROL Date effettive] {#actual-dates}

<table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td role="rowheader">[!UICONTROL Quando un'attività o un problema passa da "Nuovo" a "In corso", imposta la data di inizio effettiva su]</td> 
    <td> <p>Selezionare una delle opzioni seguenti per la registrazione della data di inizio effettiva in [!DNL Workfront] quando un'attività o un problema passa da <strong>[!UICONTROL Nuovo]</strong> a <strong>[!UICONTROL In corso]</strong>:</p> 
      <ul> 
      <li><strong>[!UICONTROL Now]:</strong> La data di inizio effettiva è impostata sulla data corrente.</li> 
      <li><strong>[!UICONTROL Data inizio pianificata]:</strong> La data inizio effettiva è impostata sulla data inizio pianificata dell'attività o del problema.</li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL Quando un'attività o un problema è completato, impostare la data di completamento effettiva su]</td> 
    <td> <p>Selezionare una delle opzioni seguenti per la registrazione della data di completamento effettiva in [!DNL Workfront] quando un'attività o un problema è completato:</p> 
      <ul> 
      <li><strong>[!UICONTROL Now]:</strong> La data di completamento effettiva è impostata sulla data corrente.</li> 
      <li> <p><strong>[!UICONTROL La data di completamento pianificata]:</strong> La data di completamento effettiva è impostata sulla data di completamento pianificata dell'attività o del problema.</p> </li> 
      </ul> </td> 
    </tr> 
  </tbody> 
</table>

### Delega

L&#39;abilitazione dell&#39;impostazione **[!UICONTROL Consenti agli utenti di delegare le loro attività e i loro problemi]** consente a tutti gli utenti del sistema di delegare temporaneamente il loro lavoro ad altri.

Quando questa impostazione è abilitata, gli utenti possono visualizzare quanto segue:

* Il collegamento [!UICONTROL **Delega**] nei rispettivi widget [!UICONTROL Il mio lavoro], [!UICONTROL Le mie attività] o [!UICONTROL I miei problemi] nell&#39;area [!UICONTROL Home]. Da lì possono delegare le assegnazioni di attività e problemi.

  >[!NOTE]
  >
  >  Il collegamento [!UICONTROL **Delegate approvals**] è sempre abilitato nell&#39;area [!UICONTROL Home].

* Indica che un&#39;attività o un problema è delegato a un altro utente nell&#39;area [!UICONTROL Assegnazioni e deleghe] nell&#39;intestazione dell&#39;attività o del problema.
* Indica che un&#39;attività o un problema è delegato a un altro utente nel widget [!UICONTROL Il mio lavoro] in [!UICONTROL Home].

  Se disattivi l&#39;impostazione [!UICONTROL Consenti agli utenti di delegare le attività e i problemi], le deleghe attualmente pianificate verranno interrotte e gli utenti delegati riceveranno una notifica e-mail di interruzione della delega.

Per informazioni sulla delega del lavoro ad altri, vedere gli articoli seguenti:

* [Panoramica sul lavoro dei delegati](../../../manage-work/delegate-work/delegate-work-overview.md)
* [Delega attività e problemi](../../../manage-work/delegate-work/how-to-delegate-work.md)


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

### [!UICONTROL Accedere ad] {#access}

<table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td role="rowheader">[!UICONTROL Quando un utente viene assegnato a un'attività]</td> 
    <td> 
      <ul> 
      <li><strong>[!UICONTROL Concedi loro ... l'accesso a un'attività]</strong>: definisce l'autorizzazione predefinita di un utente per l'attività a cui è assegnato. Per ulteriori informazioni sulle autorizzazioni per l'attività, vedere <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Concedere l'accesso agli utenti</a>.</li> 
      <li> <p><strong>[!UICONTROL Concedi anche loro ... l'accesso al progetto]</strong>: definisce l'autorizzazione predefinita di un utente al progetto al quale è stata assegnata un'attività. Per ulteriori informazioni sulle autorizzazioni del progetto, vedere <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurare le preferenze di progetto a livello di sistema</a>.</p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL Quando a un utente viene assegnato un problema]</td> 
    <td> 
      <ul> 
      <li><strong>[!UICONTROL Concedi loro ... l'accesso a un'attività]</strong>: definisce l'autorizzazione predefinita di un utente per l'attività a cui è assegnato. Per ulteriori informazioni sulle autorizzazioni per l'attività, vedere <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Concedere l'accesso agli utenti</a>.</li> 
      <li> <p><strong>[!UICONTROL Concedi anche loro ... l'accesso al progetto]</strong>: definisce l'autorizzazione predefinita di un utente al progetto al quale è stata assegnata un'attività. Per ulteriori informazioni sulle autorizzazioni del progetto, vedere <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurare le preferenze di progetto a livello di sistema</a>.</p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL Quando qualcuno invia una richiesta]</td> 
    <td> 
      <ul> 
      <li><strong>[!UICONTROL Concedi loro ... l'accesso al problema]</strong>: definisce l'autorizzazione predefinita di un utente per una richiesta inviata. Per ulteriori informazioni, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Condividere un problema </a>.</li> 
      <li> <p><strong>[!UICONTROL Le persone della stessa società erediteranno le stesse autorizzazioni per tutte le richieste]</strong>: consente agli utenti di visualizzare le richieste inviate da altri utenti della stessa società. Su tali richieste dispongono delle stesse autorizzazioni delle proprie richieste inviate.</p> </li> 
      </ul> </td> 
    </tr> 
  </tbody> 
</table>

1. Fai clic su **[!UICONTROL Salva]**.

## Blocca le preferenze di attività e problemi per i gruppi {#lock-task-and-issue-preferences-for-groups}

Se i gruppi dell’organizzazione necessitano di una preferenza per attività o problemi configurata in modo diverso per i propri flussi di lavoro univoci, puoi sbloccare la preferenza per tutti i gruppi dell’organizzazione in modo che possano configurarla autonomamente. Quando una preferenza viene sbloccata e l&#39;amministratore del gruppo la modifica, le attività o i problemi associati al gruppo vengono influenzati dall&#39;impostazione a livello di gruppo della preferenza anziché dall&#39;impostazione a livello di sistema.

Per informazioni su come un amministratore di gruppo configura le preferenze per attività e problemi di un gruppo, vedi [Configurare le preferenze per attività e problemi di un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

>[!NOTE]
>
>Dopo che un amministratore [!DNL Workfront] ha sbloccato una preferenza a livello di sistema, qualsiasi amministratore di gruppo può configurarla e quindi bloccarla per assicurarsi che tutti gli utenti del gruppo e i sottogruppi di seguito utilizzino la stessa configurazione. Ciò è parallelo alla possibilità che un amministratore [!DNL Workfront] deve configurare e bloccare una preferenza per tutti gli utenti del sistema. Per ulteriori informazioni, vedere [Configurare le preferenze di progetto per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) e [Bloccare o sbloccare un progetto, un&#39;attività o una preferenza di problema per i sottogruppi](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).

Per bloccare o sbloccare un&#39;attività o una preferenza di problema in modo che i gruppi possano configurarla:

{{step-1-to-setup}}

1. Fai clic su **[!UICONTROL Preferenze progetto]** > **[!UICONTROL Attività e problemi]**.

1. Effettua una delle seguenti operazioni:

   * Se vuoi che gli amministratori dei gruppi al di sotto del gruppo possano configurare una preferenza per i loro gruppi, sbloccarla ![Attiva/Disattiva blocco](assets/unlock-toggle-button.png).
   * Se si desidera che il gruppo e tutti i gruppi sottostanti utilizzino la configurazione per una preferenza, assicurarsi che sia bloccata (impostazione predefinita).

     >[!IMPORTANT]
     >
     >È consigliabile comunicare con gli amministratori e gli utenti in gruppi in tutto il sistema per garantire che tutte le esigenze vengano considerate nel modo in cui si configura una preferenza bloccata. Quando la blocchi, la configurazione viene ereditata da tutti i gruppi del sistema. E se la preferenza è stata sbloccata per un qualsiasi periodo di tempo, la configurazione sostituisce quelle che gli amministratori del gruppo potrebbero aver effettuato.

1. Fai clic su **[!UICONTROL Salva]**.
