---
user-type: administrator
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Configurare le preferenze di orario e scheda orario
description: In qualità di amministratore di  [!DNL Adobe Workfront] , puoi specificare le preferenze per le schede orario e le ore in  [!DNL Workfront]  per definire gli elementi con cui le schede orario possono essere precompilate e a quali elementi gli utenti possono registrare il tempo.
author: Alina and Lisa
feature: System Setup and Administration
role: Admin
exl-id: 8cc49dc2-b23f-4899-85dd-bd53d5242dbe
source-git-commit: 66e6c96ca51a159f6e9a16178f06dd016217c7d8
workflow-type: tm+mt
source-wordcount: '1409'
ht-degree: 0%

---

# Configurare le preferenze di orario e scheda orario

<!--Audited: 01/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

In qualità di amministratore di [!DNL Adobe Workfront], puoi specificare le preferenze per le schede orario e le ore in [!DNL Workfront] per definire gli elementi con cui le schede orario possono essere precompilate e a quali elementi gli utenti possono registrare il tempo.

>[!IMPORTANT]
>
>Oltre agli elementi che precompilano una scheda orario in base alle condizioni descritte in questo articolo, per impostazione predefinita vengono visualizzati anche i seguenti elementi nelle schede orario:
>
>* Elementi per i quali hai effettuato l’accesso durante l’intervallo di tempo della scheda orario
>* Elementi bloccati sulla scheda orario
>* Elementi cercati e aggiunti manualmente alla scheda orario. Per impostazione predefinita, gli elementi aggiunti manualmente vengono bloccati.
>
>Per ulteriori informazioni, consulta [Registra ora](../../../timesheets/create-and-manage-timesheets/log-time.md) e [Panoramica schede orario](/help/quicksilver/timesheets/timesheets/timesheets-overview.md).



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
   <td><p>Corrente:[!UICONTROL Plan]</p>
   Oppure
   <p>Nuovo: Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore [!DNL Workfront].</p>  </td>
</tr> 
 </tbody> 
</table>

*Per ulteriori informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Impostare le preferenze di ora e scheda orario

{{step-1-to-setup}}

1. Fai clic su **[!UICONTROL Scheda orario e ore]** > **[!UICONTROL Preferenze]**.

   Viene visualizzata la pagina Timesheets (Schede orario) e Preferenze ore (Ore).

1. (Facoltativo) Nella casella di ricerca **Schede orario di sistema e preferenze ore**, inizia a digitare il nome di un gruppo, quindi selezionalo quando viene visualizzato nell&#39;elenco.

   ![](assets/search-for-group-box-in-timesheets-preferences-page.png)

   La pagina Preferenze scheda orario e ore viene aggiornata con le preferenze per il gruppo selezionato. Per poter modificare le preferenze a livello di gruppo, è necessario sbloccare le preferenze a livello di sistema. Per ulteriori informazioni, vedere la sezione [Sbloccare le preferenze di orario e orario per i gruppi](#unlock-timesheet-and-hour-preferences-for-groups) in questo articolo.

1. Nella sezione **[!UICONTROL Preferenze generali]**, configura una delle seguenti opzioni:

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
      <td> <p>Limita la modifica ai proprietari della scheda orario e agli amministratori [!DNL Workfront]. Se questa opzione è disabilitata, le schede orario possono anche essere modificate da:</p> 
       <ul> 
        <li> <p>Utenti con accesso amministrativo a schede orario e ore nel proprio livello di accesso</p> </li> 
        <li> <p>Approvatori schede orario se nella scheda orario è abilitato "Può modificare le ore"</p> </li> 
        <li> <p>Manager del proprietario della scheda orario</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Limita la modifica delle ore a proprietari e amministratori]</td> 
      <td>Limita la modifica all'utente che ha inserito le ore e agli amministratori di [!DNL Workfront]. Questa impostazione si applica alla scheda [!UICONTROL Hours] di un progetto o di un rapporto Hours.</td> 
     </tr> 
    </tbody> 
   </table>

1. Nella sezione **[!UICONTROL Dove gli utenti possono registrare l&#39;ora]**, configura una delle seguenti opzioni:

   <table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL direttamente sui progetti]</td>
        <td>Consente agli utenti di registrare l'ora nel progetto (sia nella scheda [!UICONTROL Aggiornamenti] che nella scheda orario). Se gli utenti non registrano il tempo a livello di progetto, questa opzione deve rimanere deselezionata.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Su progetti completati]</td>
        <td>Consente agli utenti di registrare il tempo su un progetto contrassegnato come completato. Se questa opzione è disattivata, gli utenti non possono registrare il tempo per il lavoro completato sui progetti con stato [!UICONTROL Complete].</td>
    </tr>
    <tr>
        <td>[!UICONTROL Su progetti inattivi]</td>
        <td>Quando questa opzione è abilitata, gli utenti possono registrare le ore per i progetti con stato [!UICONTROL Dead].</td>
    </tr>
   </table>

1. Nella sezione **[!UICONTROL Precompila schede orario]**, configura una delle seguenti opzioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Lavoro entro] &lt;numero di settimane&gt; [!UICONTROL dell'intervallo di lavoro della scheda orario]</td> 
      <td> <p>Definisce il numero di settimane precedenti e successive all'intervallo di date della scheda orario contenente le date delle attività e delle Issues assegnate all'utente.</p> 
      <p>L’impostazione predefinita è 1 settimana e puoi estendere questo intervallo a 4 settimane.</p> 
      <p>Ciò significa che la scheda orario è precompilata con attività e problemi che hanno date comprese tra quattro settimane prima dell’intervallo di date della scheda orario e fino a quattro settimane dopo l’intervallo di date della scheda orario, se selezioni 4 settimane per l’intervallo. </p> </td> 
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

1. Nella sezione **[!UICONTROL Progetti, attività e problemi eliminati]**, specifica quanto segue:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> Durante l’eliminazione di progetti</td> 
      <td> 
       <ul> 
        <li><strong>[!UICONTROL Il tempo di connessione è già stato aggiunto alle schede orario come tempo generale]</strong>: se il progetto viene ripristinato in un secondo momento, il tempo rimane nella scheda orario.</li> 
        <li><strong>[!UICONTROL Elimina tempo registrato]</strong>: se il progetto viene successivamente ripristinato, il tempo già registrato viene ripristinato nel progetto.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Quando si eliminano attività o problemi</td> 
      <td> 
       <ul> 
        <li><strong>[!UICONTROL Sposta il tempo registrato nel progetto]</strong> in cui si trova l'attività o il problema: se l'attività o il problema viene successivamente ripristinato, il tempo rimane nel progetto.<br></li> 
        <li> <p><strong>[!UICONTROL Elimina tempo registrato]</strong>: se l'attività o il problema viene successivamente ripristinato, il tempo registrato viene ripristinato per l'attività o il problema.</p> <p>Per informazioni più dettagliate su queste opzioni, vedere <a href="../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md" class="MCXref xref">[!UICONTROL Configure effect] nelle ore in cui un oggetto viene eliminato e ripristinato</a>.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **[!UICONTROL Salva]**.

## Sblocca le preferenze orario e scheda orario per i gruppi

I gruppi della tua organizzazione potrebbero aver bisogno di schede orario o preferenze di ore configurate in modo diverso per i loro flussi di lavoro univoci. Puoi sbloccare le preferenze per tutti i gruppi dell’organizzazione in modo che possano configurarle autonomamente.

Quando una preferenza viene sbloccata e modificata da un amministratore di gruppo, influisce sui proprietari della scheda orario se il gruppo è il proprio Gruppo predefinito.

Per informazioni su come un amministratore di gruppo configura le preferenze delle ore e della scheda orario per un gruppo, vedere [Configurare le preferenze delle ore e della scheda orario per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

>[!NOTE]
>
>Dopo che un amministratore [!DNL Workfront] ha sbloccato una preferenza a livello di sistema, qualsiasi amministratore di gruppo può configurarla e quindi bloccarla per assicurarsi che tutti gli utenti del gruppo e i sottogruppi di seguito utilizzino la stessa configurazione. Ciò è parallelo alla possibilità che un amministratore [!DNL Workfront] deve configurare e bloccare una preferenza per tutti gli utenti del sistema. Per ulteriori informazioni, vedere [Bloccare o sbloccare una scheda orario e una preferenza orario di gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-timesheet-hour-preference.md).

Per sbloccare una preferenza di progetto in modo che i gruppi possano configurarla:

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **[!UICONTROL Schede orario e ore]**, quindi su **[!UICONTROL Preferenze]**.

1. Effettua una delle seguenti operazioni:

   * Se vuoi che gli amministratori dei gruppi possano configurare una preferenza per i loro gruppi, fai clic sull&#39;interruttore **sblocca** ![](assets/unlock-toggle-button.png) per sbloccarla.
   * Se desideri che tutti i gruppi utilizzino la configurazione per una preferenza, accertati che l&#39;interruttore sia bloccato ![](assets/locked-preference-toggle.png) (impostazione predefinita).

     >[!IMPORTANT]
     >
     >È consigliabile comunicare con gli amministratori e gli utenti in gruppi in tutto il sistema per garantire che tutte le esigenze vengano considerate nel modo in cui si configura una preferenza bloccata.
     >
     >Quando la blocchi, la configurazione viene ereditata da tutti i gruppi del sistema. E se la preferenza è stata sbloccata per un qualsiasi periodo di tempo, la configurazione sostituisce quelle che gli amministratori del gruppo potrebbero aver effettuato.

1. Fai clic su **[!UICONTROL Salva]**.
