---
user-type: administrator
product-area: system-administration
navigation-topic: organization-setup
title: Gestire le appartenenze a società
description: Nell'area [!UICONTROL Aziende] in Configurazione è possibile aggiungere e rimuovere i membri di un'azienda. Puoi anche modificare i profili utente, ricordargli di registrarsi nel sistema  [!DNL Workfront], deactivate them in [!DNL Workfront], and remove them from the [!DNL Workfront] .
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f0efd985-76e3-435e-bf19-87008f6a5e9d
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '910'
ht-degree: 1%

---

# Gestire le appartenenze a società

Nell&#39;area [!UICONTROL Aziende] in [!UICONTROL Configurazione], puoi aggiungere e rimuovere i membri di un&#39;azienda. È inoltre possibile modificare i profili utente, ricordargli di registrarsi in [!DNL Workfront], disattivarli in [!DNL Workfront] e rimuoverli dal sistema [!DNL Workfront].

Per informazioni sulla creazione di una nuova società, vedere [Creare e modificare società](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

## Requisiti di accesso

Per gestire le società in [!DNL Workfront] è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Workfront] piano*</p> </td> 
   <td>[!UICONTROL Team] o versione successiva</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] licenza*</p> </td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Configurazioni del livello di accesso*</strong> </td> 
   <td> <p>Uno dei seguenti elementi:</p> 
    <ul> 
     <li> <p>Il livello di accesso [!UICONTROL Amministratore di sistema], che consente di modificare qualsiasi società del sistema. Per ulteriori informazioni, vedere <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente l'accesso amministrativo completo</a>. </p> </li> 
     <li> <p>Accesso amministrativo per gestire le società, che consente di modificare qualsiasi società nel sistema. Per ulteriori informazioni, vedere <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Concedere agli utenti l'accesso amministrativo ad alcune aree</a>.</p> </li> 
    </ul> <p><b>NOTA</b>:  
     <ul> 
      <li> <p>Puoi anche gestire le aziende associate a qualsiasi gruppo a cui sei assegnato come amministratore di gruppo.</p> </li> 
      <li> <p>Per aggiungere e rimuovere utenti dal sistema [!DNL Workfront], è necessario disporre di uno dei seguenti elementi:</p> 
       <ul> 
        <li> <p>Livello di accesso [!UICONTROL System Administrator]. Per ulteriori informazioni, vedere <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente l'accesso amministrativo completo</a>. </p> </li> 
        <li> <p>Nel livello di accesso, è necessario selezionare [!UICONTROL Edit] per l'impostazione [!UICONTROL Users]. Inoltre, per l'impostazione [!UICONTROL Users], in [!UICONTROL Ottimizza le impostazioni] <img src="assets/gear-icon-in-access-levels.png"> , è necessario abilitare l'opzione [!UICONTROL Create] e almeno una delle due opzioni [!UICONTROL User Admin]. </p> <p> <img src="assets/access-req-users.png"> </p> <p>Se si utilizza l'opzione [!UICONTROL User Admin (Group Users)], è necessario essere un amministratore di gruppo di un gruppo di cui l'utente è membro.</p> </li> 
       </ul> <p>Per informazioni sull'impostazione Utenti in un livello di accesso, vedere <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Concedere l'accesso agli utenti</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sulle configurazioni di piano, tipo di licenza o livello di accesso disponibili, contattare l&#39;amministratore [!DNL Workfront].

## Gestire le appartenenze a società

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **[!UICONTROL menu principale]** nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Fai clic su **[!UICONTROL Aziende]**.
1. Fai clic sul nome dell’azienda.
1. Con la sezione **[!UICONTROL Membri società]** selezionata nel pannello a sinistra, eseguire una delle operazioni seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Aggiungi un membro</td> 
      <td> <p>Fare clic su <b>[!UICONTROL Aggiungi membro]</b>, quindi selezionare una delle opzioni seguenti nel menu a discesa visualizzato:</p> 
       <ul> 
        <li> <p><b>[!UICONTROL Nuovo utente]</b>: aggiungere un utente non ancora aggiunto a [!DNL Workfront].</p> <p>Per informazioni sull'aggiunta di utenti a [!DNL Workfront], vedere <a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Aggiungere utenti</a> e <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Modificare un profilo utente</a>.</p> </li> 
        <li> <p><b>[!DNL Existing user]</b>: aggiungi un utente già esistente nel sistema e di cui disponi dell’accesso per la modifica.</p> <p><b>IMPORTANTE</b>: se l'utente è già membro di un'altra società, la nuova assegnazione sostituisce quella precedente. L’utente perde l’accesso agli elementi condivisi con la società precedente e ottiene l’accesso agli elementi condivisi con questa società.</p> </li> 
        <li> <p><b>[!UICONTROL Importa utenti]</b>: importa un utente caricando un file di importazione foglio di calcolo. Per ulteriori informazioni, vedere <a href="../../../administration-and-setup/add-users/create-and-manage-users/import-users.md" class="MCXref xref">Importa utenti</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Modifica membri</td> 
      <td> 
       <ol> 
        <li value="1"> <p>Seleziona almeno un utente, quindi fai clic sull'icona [!UICONTROL Edit] <img src="assets/edit-icon.png"> nella barra degli strumenti.</p> </li> 
        <li value="2"> <p>Configura le opzioni visualizzate nella casella <b>[!UICONTROL Modifica utente]</b>.</p> <p>Per informazioni su queste opzioni, vedere <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Modificare il profilo di un utente</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Copia membro</td> 
      <td> <p>È possibile creare un membro della società copiandone uno esistente. </p> <p><b>NOTA</b>:  <p>Quando si crea un utente in questo modo, tutte le informazioni vengono copiate dall'utente originale all'utente appena creato, ad eccezione dei seguenti elementi:</p> 
        <ul> 
         <li>Le informazioni nella sezione [!UICONTROL Informazioni personali].</li> 
         <li>[!UICONTROL Quando accedo, mostra]: in questa casella è selezionata la scheda di destinazione predefinita per il livello di accesso.</li> 
         <li>[!UICONTROL Direct Reports]</li> 
        </ul> </p> 
       <ol> 
        <li value="1"> <p>Seleziona l'utente, quindi fai clic sull'icona [!UICONTROL Copy] <img src="assets/copy-icon.png">. </p> </li> 
        <li value="2"> <p>Nella casella <b>[!UICONTROL Nuovo utente]</b> visualizzata, modificare i campi disponibili per il nuovo utente.</p> <p>Per informazioni su tutti i campi associati a un utente, vedere <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Modificare il profilo di un utente</a>.</p> </li> 
        <li value="3"> <p>Fare clic su <strong>[!UICONTROL Add This User]</strong>.</p> <p>Oppure</p> <p>Fai clic su <strong>[!UICONTROL Aggiungi utente persona e avviane un altro]</strong> per salvare il nuovo utente e aggiungerne un altro.</p> </li> 
       </ol> <p>Verrà creato un nuovo account in [!DNL Workfront] per l'utente.</p> <p>Se hai selezionato l'opzione per inviare un invito all'utente, questi dovrebbe ricevere un'e-mail in cui possono seguire un collegamento per creare la password [!DNL Workfront].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rimuovi utenti</td> 
      <td> 
       <div> 
        <p>Selezionare almeno un utente, fare clic su <b>[!UICONTROL Rimuovi utenti]</b>, quindi selezionare una delle opzioni seguenti nel menu a discesa visualizzato:</p> 
        <ul> 
         <li> <p><b>[!UICONTROL Rimuovi dalla società]</b>: rimuove l'utente o gli utenti dalla società.</p> </li> 
         <li> <p><b>[!UICONTROL Delete]</b>: elimina l'utente o gli utenti dal sistema [!DNL Workfront].</p> <p><b>IMPORTANTE</b>: l'eliminazione di un utente dal sistema comporta anche l'eliminazione delle informazioni associate all'utente che si desidera mantenere. È consigliabile disattivare gli utenti invece di eliminarli. Per ulteriori informazioni, vedere <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Disattivare o riattivare un utente</a>.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Invia un commento agli utenti e alle loro aree [!UICONTROL Updates]</td> 
      <td> 
       <ol> 
        <li value="1"> <p>Seleziona almeno un utente, quindi fai clic sull'icona [!UICONTROL Comment] <img src="assets/comment-icon.png"> nella barra degli strumenti.</p> </li> 
        <li value="2"> <p>Digitare il commento che si desidera inviare agli utenti e all'area [!UICONTROL Aggiornamenti] dei relativi profili utente.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Esporta l'elenco dei membri della società</td> 
      <td> <p>Fai clic sull'icona [!UICONTROL Export] <img src="assets/export.png"> nella barra degli strumenti, quindi seleziona il formato desiderato per il file esportato.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Disattiva membri nel sistema</td> 
      <td> <p>Seleziona almeno un utente, fai clic sull'icona [!UICONTROL Altro] <img src="assets/more-icon.png"> nella barra degli strumenti, quindi seleziona <b>[!UICONTROL Disattiva]</b>.</p> <p>Per ulteriori informazioni, vedere <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Disattivare o riattivare un utente</a>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Ricordare a un utente di registrarsi nel sistema</td> 
      <td> <p> Nella colonna <b>[!UICONTROL Name]</b>, <b>[!UICONTROL Unregistered]</b> viene visualizzato accanto al nome di ogni utente non registrato. Per ricordare a questi utenti di registrarsi nel sistema, selezionare gli utenti, fare clic sull'icona [!UICONTROL Altro] <img src="assets/more-icon.png"> nella barra degli strumenti, quindi selezionare <b>[!UICONTROL Ricorda all'utente di registrarsi]</b>.</p> </td> 
     </tr> 
    </tbody> 
   </table>
