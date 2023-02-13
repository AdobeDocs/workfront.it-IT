---
user-type: administrator
product-area: system-administration
navigation-topic: organization-setup
title: Gestire le iscrizioni aziendali
description: In [!UICONTROL Aziende] in Configurazione è possibile aggiungere e rimuovere i membri di una società. È inoltre possibile modificare i profili utente, ricordare loro di registrarsi [!DNL Workfront], deactivate them in [!DNL Workfront], and remove them from the [!DNL Workfront] sistema.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f0efd985-76e3-435e-bf19-87008f6a5e9d
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '910'
ht-degree: 1%

---

# Gestire le iscrizioni aziendali

In [!UICONTROL Aziende] area [!UICONTROL Configurazione], è possibile aggiungere e rimuovere i membri di una società. È inoltre possibile modificare i profili utente, ricordare loro di registrarsi [!DNL Workfront], disattivali in [!DNL Workfront], e rimuoverle dal [!DNL Workfront] sistema.

Per informazioni sulla creazione di una nuova società, consulta [Creare e modificare aziende](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

## Requisiti di accesso

Per gestire le aziende in è necessario disporre dei seguenti elementi [!DNL Workfront]:

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Workfront] piano*</p> </td> 
   <td>Team [!UICONTROL] o superiore</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] licenza*</p> </td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Configurazioni a livello di accesso*</strong> </td> 
   <td> <p>Una delle seguenti opzioni:</p> 
    <ul> 
     <li> <p>Livello di accesso [!UICONTROL System Administrator], che consente di modificare qualsiasi azienda nel sistema. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente pieno accesso amministrativo</a>. </p> </li> 
     <li> <p>Accesso amministrativo alla gestione delle aziende, che consente di modificare qualsiasi azienda nel sistema. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Consentire agli utenti l'accesso amministrativo a determinate aree</a>.</p> </li> 
    </ul> <p><b>NOTA</b>:  
     <ul> 
      <li> <p>Puoi anche gestire le società associate a qualsiasi gruppo a cui ti viene assegnato come amministratore di gruppo.</p> </li> 
      <li> <p>Per aggiungere e rimuovere utenti dalla [!DNL Workfront] è necessario disporre di una delle seguenti caratteristiche:</p> 
       <ul> 
        <li> <p>Livello di accesso [!UICONTROL System Administrator]. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente pieno accesso amministrativo</a>. </p> </li> 
        <li> <p>Nel tuo livello di accesso, [!UICONTROL Edit] deve essere selezionato per l’impostazione [!UICONTROL Users]. Inoltre, per l'impostazione [!UICONTROL Users], in [!UICONTROL Ottimizza le impostazioni] <img src="assets/gear-icon-in-access-levels.png"> , l’opzione [!UICONTROL Crea] e almeno una delle due opzioni [!UICONTROL User Admin] devono essere abilitate. </p> <p> <img src="assets/access-req-users.png"> </p> <p>Se utilizzi l’opzione [!UICONTROL User Admin (Group Users)] , devi essere un amministratore di gruppo di un gruppo in cui l’utente è membro.</p> </li> 
       </ul> <p>Per informazioni sull'impostazione Utenti in un livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Concedere l’accesso agli utenti</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o configurazioni del livello di accesso hai, contatta il tuo [!DNL Workfront] amministratore.

## Gestire le iscrizioni aziendali

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Fai clic su **[!UICONTROL Aziende]**.
1. Fai clic sul nome della società.
1. Con la **[!UICONTROL Membri dell&#39;azienda]** selezionate nel pannello a sinistra, effettuate una delle seguenti operazioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Aggiungi un membro</td> 
      <td> <p>Fai clic su <b>[!UICONTROL Aggiungi membro]</b>, quindi seleziona una delle seguenti opzioni nel menu a discesa visualizzato:</p> 
       <ul> 
        <li> <p><b>[!UICONTROL Nuovo utente]</b>: Aggiungi un utente che non è ancora stato aggiunto a [!DNL Workfront].</p> <p>Per informazioni sull’aggiunta di utenti a [!DNL Workfront], vedi <a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Aggiungi utenti</a> e <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Modificare il profilo di un utente</a>.</p> </li> 
        <li> <p><b>[!DNL Existing user]</b>: Aggiungi già un utente esistente nel sistema che hai accesso per la modifica.</p> <p><b>IMPORTANTE</b>: Se l'utente è già membro di un'altra società, la nuova assegnazione sostituisce quella precedente. L'utente perde l'accesso agli articoli condivisi con la società precedente e ottiene l'accesso agli articoli condivisi con questa società.</p> </li> 
        <li> <p><b>[!UICONTROL Import Users]</b>: Importa un utente caricando un file di importazione del foglio di calcolo. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/add-users/create-and-manage-users/import-users.md" class="MCXref xref">Importare utenti</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Modifica membri</td> 
      <td> 
       <ol> 
        <li value="1"> <p>Seleziona almeno un utente, quindi fai clic sull’icona Modifica <img src="assets/edit-icon.png"> nella barra degli strumenti.</p> </li> 
        <li value="2"> <p>Configura le opzioni in <b>[!UICONTROL Modifica utente]</b> che viene visualizzata.</p> <p>Per informazioni su queste opzioni, consulta <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Modificare il profilo di un utente</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Copia membro</td> 
      <td> <p>Puoi creare un membro della società copiandone uno esistente. </p> <p><b>NOTA</b>:  <p>Quando crei un utente in questo modo, tutte le informazioni vengono copiate dall'utente originale all'utente appena creato, fatta eccezione per quanto segue:</p> 
        <ul> 
         <li>Informazioni nella sezione [!UICONTROL Personal Info].</li> 
         <li>[!UICONTROL Quando accedo, mostro]: In questa casella viene selezionata la scheda di destinazione predefinita per il livello di accesso.</li> 
         <li>Rapporti diretti di [!UICONTROL]</li> 
        </ul> </p> 
       <ol> 
        <li value="1"> <p>Seleziona l’utente, quindi fai clic sull’icona [!UICONTROL Copy] <img src="assets/copy-icon.png">. </p> </li> 
        <li value="2"> <p>In <b>[!UICONTROL Nuovo utente]</b> in cui vengono visualizzati, modificare i campi disponibili per il nuovo utente.</p> <p>Per informazioni su tutti i campi associati a un utente, consulta <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Modificare il profilo di un utente</a>.</p> </li> 
        <li value="3"> <p>Fai clic su <strong>[!UICONTROL Aggiungi questo utente]</strong>.</p> <p>Oppure</p> <p>Fai clic su <strong>[!UICONTROL Aggiungi utente e avvia un altro]</strong> per salvare il nuovo utente e aggiungerne un altro.</p> </li> 
       </ol> <p>In questo modo viene creato un nuovo account in [!DNL Workfront] per l'utente.</p> <p>Se hai selezionato l’opzione per inviare un invito all’utente, questi deve ricevere un’e-mail in cui possono seguire un collegamento per creare il proprio [!DNL Workfront] password.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rimuovi utenti</td> 
      <td> 
       <div> 
        <p>Seleziona almeno un utente e fai clic su <b>[!UICONTROL Rimuovere utenti]</b>, quindi seleziona una delle seguenti opzioni nel menu a discesa visualizzato:</p> 
        <ul> 
         <li> <p><b>[!UICONTROL Rimuovi dalla società]</b>: Rimuove l’utente o gli utenti dalla società.</p> </li> 
         <li> <p><b>[!UICONTROL Elimina]</b>: Elimina l'utente o gli utenti dal [!DNL Workfront] sistema.</p> <p><b>IMPORTANTE</b>: Se si elimina un utente dal sistema, vengono anche eliminate le informazioni associate all'utente che si desidera mantenere. È consigliabile disattivare gli utenti invece di eliminarli. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Disattivare o riattivare un utente</a>.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Invia un commento agli utenti e alle loro aree [!UICONTROL Updates]</td> 
      <td> 
       <ol> 
        <li value="1"> <p>Seleziona almeno un utente, quindi fai clic sull’icona [!UICONTROL Commento] <img src="assets/comment-icon.png"> nella barra degli strumenti.</p> </li> 
        <li value="2"> <p>Digita il commento da inviare agli utenti e all’area [!UICONTROL Updates] dei loro profili utente.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Esportare l’elenco dei membri della società</td> 
      <td> <p>Fai clic sull’icona [!UICONTROL Export] <img src="assets/export.png"> nella barra degli strumenti, selezionare il formato desiderato per il file esportato.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Disattiva membri nel sistema</td> 
      <td> <p>Seleziona almeno un utente e fai clic sull’icona Altro <img src="assets/more-icon.png"> nella barra degli strumenti, seleziona <b>[!UICONTROL Disattiva]</b>.</p> <p>Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Disattivare o riattivare un utente</a>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Ricordare a un utente di registrarsi nel sistema</td> 
      <td> <p> In <b>[!UICONTROL Name]</b> colonna, <b>[!UICONTROL non registrato]</b> viene visualizzato accanto al nome di ogni utente non registrato. Per ricordare a questi utenti di registrarsi nel sistema, seleziona gli utenti e fai clic sull’icona Altro <img src="assets/more-icon.png"> nella barra degli strumenti, seleziona <b>[!UICONTROL Richiedere all’utente di registrarsi]</b>.</p> </td> 
     </tr> 
    </tbody> 
   </table>
