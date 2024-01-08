---
user-type: administrator
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Creare una pianificazione
description: Puoi definire le settimane lavorative degli utenti con le pianificazioni. È possibile associare una pianificazione a un utente o a un progetto. Ciò consente [!DNL Workfront] per calcolare le timeline e la disponibilità dell’utente.
author: Lisa, Alina
feature: System Setup and Administration
role: Admin
exl-id: f7347ba6-68bf-45d8-b5d2-6136f3e696c9
source-git-commit: 9d2165cdc9399273a4f79b90d4049f50097cadee
workflow-type: tm+mt
source-wordcount: '808'
ht-degree: 0%

---

# Creare una pianificazione

<!--Audited: 01/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. 
Linked to Editing Users, Editing Projects, Creating and managing groups
-->

Come un [!DNL Adobe Workfront] amministratore, puoi definire la tua settimana lavorativa con le programmazioni. È possibile associare una pianificazione a un utente o a un progetto. Ciò consente [!DNL Workfront] per calcolare le timeline e la disponibilità dell’utente.

Se gli utenti lavorano in fusi orari diversi, la creazione di una pianificazione in ciascuno dei fusi orari e l’associazione di quest’ultimo agli utenti assicura che il loro lavoro venga registrato in [!DNL Workfront] in tempo reale e che la loro disponibilità sia sempre precisa in base al momento in cui funzionano.

Per informazioni sull&#39;associazione delle pianificazioni a utenti e progetti, vedere [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) e [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md).

Gli amministratori di gruppi possono anche creare pianificazioni associate ai gruppi che gestiscono. Per ulteriori informazioni, consulta [Creare e modificare le pianificazioni di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-schedules.md).

Per informazioni sull&#39;utilizzo delle pianificazioni per consentire agli utenti di collaborare in [!DNL Workfront] tra fusi orari, vedi [Utilizzo dei fusi orari](../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).

Per informazioni sull&#39;utilizzo delle pianificazioni nella pianificazione delle risorse, vedere [Panoramica sugli Schedules](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/schedules-overview.md) e [Panoramica di Programmazione delle risorse](/help/quicksilver/resource-mgmt/resource-planning/get-started-resource-planner.md).

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
   <td><p>Nuovo: [!UICONTROL Standard]</p>
       <p>Oppure</p>
       <p>Corrente: [!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td>Devi essere un [!DNL Workfront] amministratore. </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Creare una pianificazione

{{step-1-to-setup}}

1. Clic **[!UICONTROL Schedules]**.
1. Clic **[!UICONTROL Crea Schedule]**.
1. Immettere un nome per la programmazione.
1. (Facoltativo) Seleziona **[!UICONTROL Pianificazione predefinita]** per identificare questa pianificazione come predefinita.

   Devi avere almeno una pianificazione in [!DNL Workfront]. Se ne hai solo uno, viene designato come pianificazione predefinita.

   È possibile avere più di una pianificazione, ma una sola pianificazione predefinita.

   >[!NOTE]
   >
   >Se si è un amministratore di gruppo, non è possibile impostare una pianificazione come predefinita. Solo un [!DNL Workfront] l&#39;amministratore può designare una pianificazione come predefinita per il sistema.

   ![Crea Schedule](assets/new-schedule.png)

1. Il giorno **[!UICONTROL Pianificazione]** , seleziona una pianificazione giornaliera trascinando il contorno blu tra i blocchi orari per evidenziarli.

   È consigliabile selezionare 8 blocchi di un’ora in un periodo di tempo di 9 ore. Questo è adatto per il pranzo o altre pause.

   ![Blocchi di tempo in una pianificazione](assets/new-schedule-with-exceptions.png)

1. Il giorno **[!UICONTROL Dettagli]** , immettere le informazioni seguenti:

   <table style="table-layout:auto">
    <tr>
     <td>[!UICONTROL Group con accesso amministratore]</td>
     <td><p>Selezionare il gruppo i cui amministratori dispongono delle autorizzazioni per modificare la pianificazione.</p>
     <p><b>IMPORTANTE</b>:</p>
      <ul>
       <li>
       <p>Questo campo è obbligatorio per gli amministratori di gruppi che creano una pianificazione.</p>
       <p>In qualità di amministratore di gruppo, puoi creare una pianificazione solo se è designata per un gruppo o un sottogruppo per il quale sei designato come amministratore.</p>
       <p>Se gestisci un solo gruppo, per impostazione predefinita quest’ultimo viene selezionato in questo campo.</p>
       <p>Se gestisci più gruppi, devi selezionare un gruppo in questo campo prima di poter salvare la pianificazione.</p></li>
       <li>Se sei un [!DNL Workfront] amministratore che crea una pianificazione, questo campo è facoltativo. Quando si crea una pianificazione senza associarla a un gruppo, questa viene salvata come pianificazione a livello di sistema e non può essere gestita da un amministratore di gruppo di alcun gruppo.
       <p>Le pianificazioni assegnate ad account o progetti sono visibili a tutti gli utenti che possono modificare questi oggetti. Ciò vale sia per le pianificazioni a livello di sistema che per quelle a livello di gruppo.</p>
       </li>
       <p>La specifica di un gruppo con accesso amministratore per una pianificazione non assegna la pianificazione agli utenti del gruppo, ma consente solo agli amministratori del gruppo di modificare, eliminare e copiare la pianificazione.</p>
       <p>Gli amministratori di gruppi non possono modificare, eliminare o copiare pianificazioni a livello di sistema. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Amministratori di gruppi</a>.
     </td>
    </tr>
    <tr>
     <td>[!UICONTROL Groups with View Access]</td>
     <td><p>Selezionare i gruppi con accesso [!UICONTROL View] che possono visualizzare questa pianificazione.</p>
     <p>Solo gli utenti dei gruppi qui specificati possono trovare la pianificazione nel menu a discesa quando la assegnano a utenti o progetti.</p></tr>
    <tr>
     <td>Fuso orario di [!UICONTROL]</td>
     <td><p>Seleziona il fuso orario per la pianificazione.</p>
     <p>Se si associa la pianificazione a un utente, è consigliabile che il fuso orario della pianificazione corrisponda a quello dell'utente. Per informazioni sui fusi orari degli utenti, vedi <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Modifica il profilo di un utente.
     </td>
    </tr>
   </table>


1. Il giorno **[!UICONTROL Eccezioni]** , specificare eventuali eccezioni alla pianificazione.

   Le eccezioni sono giornate piene o mezze giornate che devono essere escluse dalla pianificazione, come festività o eventi aziendali.

   >[!NOTE]
   >
   >Se si conoscono già le eccezioni ricorrenti, è possibile definire le eccezioni per molti anni in futuro.

   I giorni completi o parziali possono essere esclusi dal programma di lavoro. Fai clic sulla data per selezionarla come eccezione, quindi seleziona la **[!UICONTROL Tutto il giorno]** per indicare se l&#39;eccezione è un giorno intero o meno.

   ![Eccezione giornata intera](assets/schedule-adding-an-all-day-exception.png)

1. Inserire l&#39;ora di inizio e di fine per le eccezioni dei giorni parziali.

   ![Eccezione per giorno parziale](assets/partial-day-exception-on-schedules.png)

1. Clic **[!UICONTROL Salva]**, quindi fai clic su **[!UICONTROL Salva] Modifiche**.

1. (Facoltativo) Associa la pianificazione a un utente.

   Per informazioni, consulta [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. (Facoltativo) Associa la pianificazione a un progetto.

   Per informazioni, consulta [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md).
