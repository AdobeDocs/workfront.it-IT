---
user-type: administrator
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Creare una pianificazione
description: Puoi definire le settimane di lavoro degli utenti utilizzando le pianificazioni. Puoi associare una pianificazione a un utente o a un progetto. Ciò consente [!DNL Workfront] per calcolare le timeline e la disponibilità degli utenti.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f7347ba6-68bf-45d8-b5d2-6136f3e696c9
source-git-commit: 9f7f8a50bb805b1d6845df79ecffaa329d5abc26
workflow-type: tm+mt
source-wordcount: '817'
ht-degree: 0%

---

# Creare una pianificazione

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. 
Linked to Editing Users, Editing Projects, Creating and managing groups
-->

Come [!DNL Adobe Workfront] amministratore, è possibile definire la settimana lavorativa utilizzando le pianificazioni. Puoi associare una pianificazione a un utente o a un progetto. Ciò consente [!DNL Workfront] per calcolare le timeline e la disponibilità degli utenti.

Quando si dispone di utenti che lavorano in diversi fusi orari, la creazione di una pianificazione in ciascuno dei fusi orari e l&#39;associazione con tali utenti assicura che il loro lavoro venga registrato in [!DNL Workfront] in tempo reale e che la loro disponibilità è sempre accurata a seconda di quando lavorano.

Per informazioni sull&#39;associazione di pianificazioni con utenti e progetti, vedi i seguenti articoli:

* [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)
* [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md)

Gli amministratori dei gruppi possono anche creare pianificazioni associate ai gruppi che gestiscono. Per ulteriori informazioni, consulta [Creare e modificare le pianificazioni di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-schedules.md).

Per informazioni sull&#39;utilizzo delle pianificazioni per aiutare gli utenti a collaborare in [!DNL Workfront] nei diversi fusi orari, vedi [Utilizzo di fusi orari diversi](../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano [!UICONTROL Adobe Workfront]</td> 
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

## Creare una pianificazione

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe] Workfront, quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).
1. Fai clic su **[!UICONTROL Pianificazioni]**.
1. Fai clic su **[!UICONTROL Nuova pianificazione]**.
1. Specifica un nome per la pianificazione.
1. (Facoltativo) Seleziona **[!UICONTROL Pianificazione predefinita]** per identificare questa pianificazione come predefinita.

   Puoi avere più di una pianificazione in [!DNL Workfront], ma puoi avere una sola pianificazione predefinita.

   È necessario disporre di almeno una pianificazione in [!DNL Workfront]. Se ne hai solo uno, questo viene designato come pianificazione predefinita.

   >[!NOTE]
   >
   >Se si è un amministratore di gruppo, non è possibile designare una pianificazione come pianificazione predefinita. Solo un [!DNL Workfront] l&#39;amministratore può designare una pianificazione come impostazione predefinita per il sistema.

   ![](assets/new-schedule.png)

1. In **[!UICONTROL Pianificazione]** seleziona una pianificazione giornaliera trascinando il contorno blu tra i blocchi di ore per evidenziarli.

   È consigliabile selezionare 8 blocchi di un’ora su un periodo di tempo di 9 ore. Questo alloggio è a pranzo o altre pause.

   ![](assets/new-schedule-with-exceptions.png)

1. Sulla **[!UICONTROL Dettagli]** , specifica le seguenti informazioni:

   <table style="table-layout:auto">
    <tr>
     <td>[!UICONTROL Group with Administration Access]</td>
     <td><p>Indica il gruppo di cui gli amministratori dispongono dell'autorizzazione per modificare la pianificazione.</p>
     <p><b>IMPORTANTE</b>:</p>
      <ul>
       <li>
       <p>Se sei un amministratore di gruppo che crea una pianificazione, questo campo è obbligatorio.</p>
       <p>In qualità di amministratore del gruppo, è possibile creare una pianificazione solo se designata come amministratore per un gruppo o sottogruppo.</p>
       <p>Se gestisci un solo gruppo, per impostazione predefinita questo gruppo viene selezionato in questo campo.</p>
       <p>Se gestisci più gruppi, devi selezionare un gruppo in questo campo prima di salvare la pianificazione.</p></li>
       <li>Se sei un [!DNL Workfront] amministratore che crea una pianificazione, questo campo è facoltativo. Quando si crea una pianificazione senza associarla a un gruppo, questa viene salvata come pianificazione a livello di sistema e non può essere gestita da un amministratore di gruppo di alcun gruppo.
       <p>Le pianificazioni assegnate ad account o progetti sono visibili a tutti gli utenti che possono modificare tali oggetti. Questo vale sia per le pianificazioni a livello di sistema che per quelle a livello di gruppo.</p>
       </li>
       <p>La specificazione di un gruppo con accesso all'amministrazione per una pianificazione non assegna la pianificazione agli utenti del gruppo; consente solo agli amministratori del gruppo di modificare, eliminare e copiare la pianificazione.</p>
       <p>Gli amministratori dei gruppi non possono modificare, eliminare o copiare le pianificazioni a livello di sistema. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Amministratori di gruppo</a>.
     </td>
    </tr>
    <tr>
     <td>[!UICONTROL Groups with View Access (Gruppi con accesso alla visualizzazione)]</td>
     <td><p>Seleziona i gruppi con accesso [!UICONTROL View] a cui è visibile questa pianificazione.</p>
     <p>Solo gli utenti dei gruppi qui specificati possono trovare la pianificazione nel menu a discesa quando la assegnano a utenti o progetti.</p></tr>
    <tr>
     <td>[!UICONTROL Time Zone]</td>
     <td><p>Seleziona il fuso orario della pianificazione.</p>
     <p>Se si associa la pianificazione a un utente, è consigliabile che il fuso orario della pianificazione corrisponda a quello dell'utente. Per informazioni sui fusi orari dell'utente, vedere <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Modificare il profilo di un utente.
     </td>
    </tr>
   </table>


1. Sulla **[!UICONTROL Eccezioni]** Specifica le eccezioni alla pianificazione.

   Le eccezioni sono giorni interi o mezzo che devono essere esclusi dal programma, ad esempio festività o eventi aziendali.

   >[!NOTE]
   >
   >Se conosci già le eccezioni di pianificazione periodica, puoi definire le eccezioni di pianificazione per molti anni in futuro.

   I giorni interi o parziali possono essere esclusi dal programma di lavoro. Fai clic sulla data per selezionarla come eccezione, quindi seleziona la **[!UICONTROL Tutto il giorno]** campo per indicare se l&#39;eccezione è un giorno completo o meno.

   ![](assets/schedule-adding-an-all-day-exception.png)

1. Specifica l&#39;ora di inizio e di fine per le eccezioni del giorno parziale.

   ![parziale-day-exception-on-Schedule.png](assets/partial-day-exception-on-schedules.png)

1. Fai clic su **[!UICONTROL Salva]**, quindi fai clic su **[!UICONTROL Salva] Modifiche**.

1. (Facoltativo) Associa la pianificazione a un utente.

   Per informazioni, consulta [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. (Facoltativo) Associa la pianificazione a un progetto.

   Per informazioni, consulta [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md).
