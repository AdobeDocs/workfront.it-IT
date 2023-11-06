---
user-type: administrator
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Configurare le preferenze di orario e scheda orario
description: Come un [!DNL Adobe Workfront] amministratore, puoi specificare le preferenze per le schede orario e le ore in [!DNL Workfront] per definire gli elementi con cui le schede orario possono precompilare e a quali elementi gli utenti possono registrare il tempo.
author: Courtney and Alina
feature: System Setup and Administration
role: Admin
exl-id: 8cc49dc2-b23f-4899-85dd-bd53d5242dbe
source-git-commit: 62c600a13f61f7f5e889a92b446252e5ca0777f9
workflow-type: tm+mt
source-wordcount: '1352'
ht-degree: 1%

---

# Configurare le preferenze di orario e scheda orario

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Come un [!DNL Adobe Workfront] amministratore, puoi specificare le preferenze per le schede orario e le ore in [!DNL Workfront] per definire gli elementi con cui le schede orario possono precompilare e a quali elementi gli utenti possono registrare il tempo.

>[!NOTE]
>
>Gli elementi per i quali hai effettuato l’accesso durante l’intervallo di tempo della scheda orario vengono visualizzati nella scheda orario per impostazione predefinita, anche se potrebbero non soddisfare le condizioni descritte in questo articolo per la precompilazione della scheda orario.
>
>Per informazioni sull&#39;ora di registrazione, vedere [Tempo di connessione](../../../timesheets/create-and-manage-timesheets/log-time.md).


Qualsiasi modifica apportata alle schede orario influisce su tutte le schede orario create in futuro.

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
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un [!DNL Workfront] amministratore.</p> <p><b>NOTA</b>

Se ancora non disponi dell’accesso, chiedi al tuo [!DNL Workfront] amministratore se impostano restrizioni aggiuntive nel livello di accesso. Per informazioni su come [!DNL Workfront] l&#39;amministratore può modificare il tuo livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
 </tbody> 
</table>

## Impostare le preferenze di ora e scheda orario

1. Fai clic su **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Clic **[!UICONTROL Timesheet e ore]** > **[!UICONTROL Preferenze]**.

1. Nella pagina visualizzata, in **[!UICONTROL Preferenze generali]** configurare una delle opzioni seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Registra ore per date future]</td> 
      <td> <p>Consente agli utenti di registrare le ore per le date future in tutto il sistema in:</p> 
       <ul> 
        <li>Tutti i progetti, le attività e i problemi per i quali dispongono dell'accesso al tempo di registrazione</li> 
        <li>Le loro schede orario come Ora generale</li> 
       </ul> <p>Questa funzione è utile quando gli utenti hanno intenzione di allontanarsi dall’ufficio e desiderano registrare in anticipo l’ora.</p> <p><b>NOTA</b>:</p> 
       <p>Non è possibile impedire agli utenti di registrare ore per attività o problemi chiusi o annullati. Puoi impedire agli utenti di registrare solo il tempo su progetti completi o inattivi. È consigliabile utilizzare i filtri negli elenchi di attività e problemi per escludere che quelli completati o annullati siano visibili agli utenti.</p> </td> 
     </tr>

   <tr> 
      <td role="rowheader">[!UICONTROL Assegna manualmente ruoli alle voci orarie]</td> 
      <td> <p>Consenti agli utenti di selezionare manualmente qualsiasi Ruolo assegnato nel loro profilo utente o assegnato all'oggetto.</p> <p><b>IMPORTANTE</b>:  
        <ul> 
         <li>Se disattivi questa impostazione dopo aver assegnato i ruoli alle voci orarie, gli utenti devono regolare le ore registrate in vari ruoli nella scheda [!UICONTROL Hours] del progetto, dell’attività o del problema.</li> 
         <li>Se all'utente non è stata assegnata una mansione nel profilo ed è presente un'attività assegnata come [!UICONTROL Proprietario attività] nella finestra di dialogo [!UICONTROL Assegnazioni avanzate], tale mansione viene visualizzata quando l'utente accede all'attività.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Limita la modifica della scheda orario a proprietari e amministratori]</td> 
      <td> <p>Limita la modifica ai proprietari della scheda orario e [!DNL Workfront] amministratori. Se questa opzione è disabilitata, le schede orario possono anche essere modificate da:</p> 
       <ul> 
        <li> <p>Utenti con accesso amministrativo a schede orario e ore nel proprio livello di accesso</p> </li> 
        <li> <p>Approvatori schede orario se nella scheda orario è abilitato "Può modificare le ore"</p> </li> 
        <li> <p>Manager del proprietario della scheda orario</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Limita la modifica delle ore a proprietari e amministratori]</td> 
      <td>Limita la modifica all’utente che ha inserito le ore e [!DNL Workfront] amministratori. Questa impostazione si applica alla scheda [!UICONTROL Hours] di un progetto o di un rapporto Hours.</td> 
     </tr> 
    </tbody> 
   </table>

1. In **[!UICONTROL Dove gli utenti possono registrare il tempo]** configurare una delle opzioni seguenti:

   <table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Registra tempo direttamente sui progetti]</td>
        <td>Consente agli utenti di registrare l'ora nel progetto (sia nella scheda [!UICONTROL Aggiornamenti] che nella scheda orario). Se gli utenti non registrano il tempo a livello di progetto, questa opzione deve rimanere deselezionata.</td>
    </tr>
    <tr>
        <td>Registra tempo suoi progetti completi</td>
        <td>Consente agli utenti di registrare il tempo su un progetto contrassegnato come completato. Se questa opzione è disattivata, gli utenti non possono registrare il tempo per il lavoro completato sui progetti con stato [!UICONTROL Complete].</td>
    </tr>
    <tr>
        <td>Registra tempo suoi progetti inattivi</td>
        <td>Quando questa opzione è abilitata, gli utenti possono registrare le ore per i progetti con stato [!UICONTROL Dead].</td>
    </tr>
   </table>

1. In **[!UICONTROL Precompila le schede orario]** configurare una delle opzioni seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Lavoro che si trova in] &lt;number of="" weeks=""&gt; [!UICONTROL dell'intervallo di lavoro della scheda orario]</td> 
      <td> <p>Definisce il numero di settimane precedenti e successive all'intervallo di date della scheda orario contenente le date delle attività e delle Issues assegnate all'utente. L’impostazione predefinita è 1 settimana e puoi estendere questo intervallo a 4 settimane. Ciò significa che la scheda orario è precompilata con attività e problemi che hanno date comprese tra quattro settimane prima dell’intervallo di date della scheda orario e fino a quattro settimane dopo l’intervallo di date della scheda orario, se selezioni 4 settimane per l’intervallo. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Attività e problemi completati]</td> 
      <td>Se a una singola attività vengono in genere assegnate più risorse, si consiglia questa impostazione. Ciò significa che quando una risorsa registra il tempo relativo all’attività e la contrassegna come completata, le altre risorse assegnate all’attività possono ancora trovare l’attività o il problema nella propria scheda orario, per registrare le proprie ore.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Attività e problemi con date pianificate nell'intervallo date della scheda orario]</td> 
      <td> <p>Se selezionata, la scheda attività include attività e problemi con una Data inizio pianificata o una Data completamento compresa nell'intervallo di date della scheda attività.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> [!UICONTROL Attività con date previste nell'intervallo date della scheda orario]</td> 
      <td> <p>Se questa opzione è selezionata, la scheda attività include attività con una data di inizio prevista o una data di completamento compresa nell'intervallo di tempo del progetto, anche se la data pianificata del problema o dell'attività non rientra nell'intervallo di date della scheda attività.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. In **[!UICONTROL Progetti, attività e problemi eliminati]** , specificare quanto segue:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL durante l'eliminazione dei progetti]</td> 
      <td> 
       <ul> 
        <li><strong>[!UICONTROL Tempo di connessione già aggiunto alle schede orario come tempo generale]</strong>: se il progetto viene ripristinato in un secondo momento, l’ora rimane nella scheda orario.</li> 
        <li><strong>[!UICONTROL Elimina qualsiasi ora registrata]</strong>: se il progetto viene successivamente ripristinato, l’ora già registrata viene ripristinata nel progetto.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Durante l'eliminazione di attività o problemi]</td> 
      <td> 
       <ul> 
        <li><strong>[!UICONTROL Spostare il tempo registrato nel progetto in cui si trova l'attività o il problema]</strong>: se l’attività o il problema viene successivamente ripristinato, il tempo rimane sul progetto.<br></li> 
        <li> <p><strong>[!UICONTROL Elimina qualsiasi ora registrata]</strong>: se l’attività o il problema viene successivamente ripristinato, il tempo registrato viene ripristinato per l’attività o il problema.</p> <p>Per informazioni più dettagliate su queste opzioni, vedi <a href="../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md" class="MCXref xref">[!UICONTROL Configura effetto] nelle ore in cui un oggetto viene eliminato e ripristinato</a>.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **[!UICONTROL Salva]**.

## Sblocca le preferenze orario e scheda orario per i gruppi

I gruppi dell’organizzazione potrebbero aver bisogno di una preferenza per schede orario o ore configurata in modo diverso per i loro flussi di lavoro univoci. Puoi sbloccare la preferenza per tutti i gruppi dell’organizzazione in modo che possano configurarla autonomamente.

Quando una preferenza viene sbloccata e modificata da un amministratore di gruppo, influisce sui proprietari della scheda orario se il gruppo è il proprio Gruppo predefinito.

Per informazioni su come un amministratore di gruppo configura le preferenze delle ore e della scheda orario per un gruppo, consulta [Configurare le preferenze di orario e scheda orario per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

>[!NOTE]
>
>Dopo un [!DNL Workfront] l’amministratore sblocca una preferenza a livello di sistema, qualsiasi amministratore di gruppo può configurarla e quindi bloccarla per garantire che tutti gli utenti del gruppo e i sottogruppi sottostanti utilizzino la stessa configurazione. Questo è parallelo alla capacità che un [!DNL Workfront] l’amministratore deve configurare e bloccare una preferenza per tutti gli utenti del sistema. Per ulteriori informazioni, consulta [Blocca o sblocca una preferenza di tipo Timesheet gruppo e Ora](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-timesheet-hour-preference.md).

Per sbloccare una preferenza di progetto in modo che i gruppi possano configurarla:

1. Fai clic su **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe] Workfront, quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **[!UICONTROL Schede orario e ore]**, quindi fai clic su **[!UICONTROL Preferenze]**.

1. Effettua una delle seguenti operazioni:

   * Se desideri che gli amministratori dei gruppi possano configurare una preferenza per i loro gruppi, sbloccalo ![](assets/unlock-toggle-button.png).
   * Se si desidera che tutti i gruppi utilizzino la configurazione per una preferenza, assicurarsi che sia bloccata (impostazione predefinita).

     >[!IMPORTANT]
     >
     >È consigliabile comunicare con gli amministratori e gli utenti in gruppi in tutto il sistema per garantire che tutte le esigenze vengano considerate nel modo in cui si configura una preferenza bloccata. Quando la blocchi, la configurazione viene ereditata da tutti i gruppi del sistema. E se la preferenza è stata sbloccata per un qualsiasi periodo di tempo, la configurazione sostituisce quelle che gli amministratori del gruppo potrebbero aver effettuato.

1. Fai clic su **[!UICONTROL Salva]**.
