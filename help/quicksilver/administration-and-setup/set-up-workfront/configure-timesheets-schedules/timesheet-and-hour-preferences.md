---
user-type: administrator
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Configurare le preferenze relative a schede attività e ora
description: Come [!DNL Adobe Workfront] amministratore, puoi specificare le preferenze per le schede attività e le ore in [!DNL Workfront] per definire con quali elementi i fogli preselezionati possono essere precompilati e a quali elementi gli utenti possono registrare il tempo di registrazione.
author: Courtney and Alina
feature: System Setup and Administration
role: Admin
exl-id: 8cc49dc2-b23f-4899-85dd-bd53d5242dbe
source-git-commit: 3b0a82381d1c33d897b123a597df21ba54cc2565
workflow-type: tm+mt
source-wordcount: '1310'
ht-degree: 1%

---

# Configurare le preferenze relative a schede attività e ora

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Come [!DNL Adobe Workfront] amministratore, puoi specificare le preferenze per le schede attività e le ore in [!DNL Workfront] per definire con quali elementi i fogli preselezionati possono essere precompilati e a quali elementi gli utenti possono registrare il tempo di registrazione.

Le modifiche apportate ai fogli presenze hanno effetto su tutti i fogli presenze creati in futuro.

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
   <td> <p>Devi essere un [!DNL Workfront] amministratore.</p> <p><b>NOTA</b>

Se non hai ancora accesso, chiedi [!DNL Workfront] amministratore se imposta ulteriori restrizioni nel livello di accesso. Per informazioni su come [!DNL Workfront] l&#39;amministratore può modificare il livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
 </tbody> 
</table>

## Impostare le preferenze per la scheda attività e l&#39;ora

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Fai clic su **[!UICONTROL Scheda attività e ore]** > **[!UICONTROL Preferenze]**.

1. Nella pagina visualizzata, nella **[!UICONTROL Preferenze generali]** configura una delle seguenti opzioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Log time for future date]</td> 
      <td> <p>Consente agli utenti di registrare l’ora per le date future in tutto il sistema in:</p> 
       <ul> 
        <li>Qualsiasi progetto, attività e problemi a cui hanno accesso al tempo di log</li> 
        <li>I fogli presenze come ora generale</li> 
       </ul> <p>Questo è utile quando gli utenti hanno intenzione di essere lontani dall'ufficio e vogliono registrare quel tempo in anticipo.</p> <p><b>NOTA</b>: Non è possibile impedire agli utenti di registrare il tempo su attività o problemi chiusi o annullati. È possibile solo impedire agli utenti di registrare il tempo su progetti completi o morti. È consigliabile utilizzare i filtri negli elenchi di attività e problemi per escludere quelli completati o annullati dalla visualizzazione degli utenti.</p> </td> 
     </tr>

   <tr> 
      <td role="rowheader">[!UICONTROL Assegna manualmente ruoli processo alle voci ora]</td> 
      <td> <p>Consente agli utenti di selezionare manualmente qualsiasi Ruolo processo assegnato nel profilo utente o assegnato all’oggetto.</p> <p><b>IMPORTANTE</b>:  
        <ul> 
         <li>Se disattivi questa impostazione dopo aver assegnato i ruoli di lavoro alle voci orarie, gli utenti devono regolare le ore registrate in vari ruoli nella scheda [!UICONTROL Hours] del progetto, dell’attività o del problema.</li> 
         <li>Se all’utente non è assegnato un ruolo di lavoro nel profilo e un’attività è assegnata come [!UICONTROL Task Owner] nella finestra di dialogo [!UICONTROL Advanced Assignments] (Assegnazioni avanzate), tale ruolo viene visualizzato quando l’utente accede al tempo dell’attività.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Limita la modifica della scheda attività a proprietari e amministratori]</td> 
      <td> <p>Limita la modifica ai proprietari della scheda attività e [!DNL Workfront] amministratori. Quando questa opzione è disabilitata, le schede attività possono essere modificate anche da:</p> 
       <ul> 
        <li> <p>Utenti con accesso amministrativo a schede e ore nel loro livello di accesso</p> </li> 
        <li> <p>Gli approvatori della scheda attività se l'opzione "Può modificare le ore" è abilitata nella scheda attività</p> </li> 
        <li> <p>Il gestore del proprietario della scheda attività</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Limita la modifica delle ore a proprietari e amministratori]</td> 
      <td>Limita la modifica all’utente che ha inserito le ore e [!DNL Workfront] amministratori. Questa impostazione si applica alla scheda [!UICONTROL Hours] in un progetto o in un rapporto Hours.</td> 
     </tr> 
    </tbody> 
   </table>

1. In **[!UICONTROL Dove gli utenti possono registrare il tempo]** configura una delle seguenti opzioni:

   <table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Log time direttamente sui progetti]</td>
        <td>Consente agli utenti di registrare il tempo sul progetto (sia nella scheda [!UICONTROL Updates] che nella scheda Scheda attività). Se gli utenti non registrano l’ora a livello di progetto, questa opzione deve rimanere deselezionata.</td>
    </tr>
    <tr>
        <td>Registra tempo suoi progetti completi</td>
        <td>Consente agli utenti di registrare il tempo su un progetto contrassegnato come completato. Se questa opzione è disabilitata, gli utenti non possono registrare il tempo del lavoro completato sui progetti nello stato [!UICONTROL Complete].</td>
    </tr>
    <tr>
        <td>Registra tempo suoi progetti inattivi</td>
        <td>Quando questa opzione è abilitata, gli utenti possono accedere alle ore dei progetti con uno stato [!UICONTROL Dead].</td>
    </tr>
   </table>

1. In **[!UICONTROL Fogli temporali precompilati]** configura una delle seguenti opzioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Work in] &lt;number of="" weeks=""&gt; [!UICONTROL dell'intervallo di lavoro della scheda attività]</td> 
      <td> <p>Definisce il numero di settimane prima e dopo l'intervallo di date della scheda attività che contiene le date delle attività e dei problemi assegnati all'utente. L’impostazione predefinita è 1 settimana ed è possibile estendere questo intervallo a 4 settimane. Ciò significa che la scheda attività è precompilata con attività e problemi con date comprese tra quattro settimane prima dell'intervallo di date della scheda attività fino a quattro settimane dopo l'intervallo di date della scheda attività, se si seleziona 4 settimane per l'intervallo. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Attività e problemi che sono stati completati]</td> 
      <td>Se più risorse vengono generalmente assegnate a una singola attività, è consigliabile impostare questa opzione. Ciò significa che quando una risorsa registra il tempo rispetto all'attività e la contrassegna come completata, le altre risorse assegnate all'attività possono comunque trovare l'attività o il problema nella relativa scheda attività, per registrare le ore.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Attività e problemi che hanno date previste nell'intervallo di date della scheda attività]</td> 
      <td> <p>Se selezionata, la scheda attività include le attività e i problemi che presentano una data di inizio pianificata o una data di completamento compresa nell'intervallo di date della scheda attività.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> [!UICONTROL Attività che hanno date previste nell'intervallo di date della scheda attività]</td> 
      <td> <p>Se selezionata, la scheda attività include attività che presentano una data di inizio prevista o una data di completamento entro l'intervallo di tempo del progetto, anche se la data pianificata dell'emissione o dell'attività non rientra nell'intervallo di date della scheda attività.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. In **[!UICONTROL Progetti, attività e problemi eliminati]** specifica quanto segue:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Durante l’eliminazione di progetti]</td> 
      <td> 
       <ul> 
        <li><strong>[!UICONTROL Mantieni il tempo di registrazione già aggiunto ai fogli presenze come ora generale]</strong>: Se il progetto viene ripristinato in un secondo momento, il tempo rimane nella scheda attività.</li> 
        <li><strong>[!UICONTROL Elimina qualsiasi ora registrata]</strong>: Se il progetto viene successivamente ripristinato, il tempo già registrato viene ripristinato nel progetto.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Durante l'eliminazione di attività o problemi]</td> 
      <td> 
       <ul> 
        <li><strong>[!UICONTROL Sposta qualsiasi ora registrata nel progetto in cui si trova l'attività o il problema]</strong>: Se l’attività o il problema viene successivamente ripristinato, il tempo rimane sul progetto.<br></li> 
        <li> <p><strong>[!UICONTROL Elimina qualsiasi ora registrata]</strong>: Se l'attività o il problema viene successivamente ripristinato, il tempo di accesso viene ripristinato all'attività o al problema.</p> <p>Per informazioni più dettagliate su queste opzioni, vedi <a href="../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md" class="MCXref xref">[!UICONTROL Configura effetto] nelle ore in cui un oggetto viene eliminato e ripristinato</a>.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **[!UICONTROL Salva]**.

## Sblocca le preferenze della scheda attività e dell&#39;ora per i gruppi

I gruppi dell&#39;organizzazione potrebbero aver bisogno di una scheda attività o di una preferenza oraria configurata in modo diverso per i flussi di lavoro univoci. È possibile sbloccare la preferenza per tutti i gruppi all’interno dell’organizzazione in modo che possano configurarla autonomamente.

Quando una preferenza viene sbloccata e un amministratore di gruppo la modifica, la modifica interessa i proprietari della scheda attività se il gruppo è il gruppo principale.

Per informazioni su come un amministratore del gruppo configura le preferenze relative alla scheda attività e all&#39;ora per un gruppo, vedere [Configurare le preferenze relative a schede attività e ora per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

>[!NOTE]
>
>Dopo un [!DNL Workfront] l’amministratore sblocca una preferenza a livello di sistema, qualsiasi amministratore di gruppo può configurarla e quindi bloccarla per garantire che tutti i membri del proprio gruppo e dei sottogruppi sottostanti utilizzino la stessa configurazione. Ciò è parallelo alla capacità di un [!DNL Workfront] l’amministratore deve configurare e bloccare una preferenza per tutti gli utenti del sistema. Per ulteriori informazioni, consulta [Bloccare o sbloccare una scheda attività e una preferenza ora del gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-timesheet-hour-preference.md).

Per sbloccare una preferenza di progetto in modo che i gruppi possano configurarla:

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe] Workfront, quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **[!UICONTROL Tempi e ore]**, quindi fai clic su **[!UICONTROL Preferenze]**.

1. Effettua una delle seguenti operazioni:

   * Se desideri che gli amministratori dei gruppi siano in grado di configurare una preferenza per i loro gruppi, sbloccarla ![](assets/unlock-toggle-button.png).
   * Se desideri che tutti i gruppi utilizzino la configurazione per una preferenza, accertati che sia bloccata (questa è l’impostazione predefinita).

      >[!IMPORTANT]
      >
      >È consigliabile comunicare con gli amministratori e gli utenti di gruppi in tutto il sistema per garantire che tutte le esigenze siano prese in considerazione nel modo in cui si configura una preferenza bloccata. Quando lo si blocca, la configurazione per esso viene ereditata da tutti i gruppi del sistema. E se la preferenza è stata sbloccata per un qualsiasi periodo di tempo, la configurazione sostituisce quelle che gli amministratori del gruppo potrebbero aver effettuato.

1. Fai clic su **[!UICONTROL Salva]**.
