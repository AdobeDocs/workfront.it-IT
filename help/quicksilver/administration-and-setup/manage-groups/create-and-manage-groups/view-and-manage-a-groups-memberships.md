---
user-type: administrator
product-area: system-administration;user-management
keywords: aggiungi,utenti,gruppo,aggiungi,altro,assegna,amministratore,rimuovi,utente,visualizzazione,ruoli,membri,esportazione,appartenenza,dati
navigation-topic: create-and-manage-groups
title: Visualizzare e gestire le appartenenze a un gruppo
description: In qualità di amministratore di Adobe Workfront, puoi visualizzare, aggiungere, rimuovere, esportare, attivare e disattivare i membri di qualsiasi gruppo gestito. Puoi anche modificare i loro profili, aggiungere Aggiornamenti ai loro profili e assegnarli come amministratori di gruppo aggiuntivi per il gruppo.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 219e5fa3-cf25-477d-82f6-046e3ff30989
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 1%

---

# Visualizzare e gestire le appartenenze a un gruppo

In qualità di amministratore di Adobe Workfront, puoi visualizzare, aggiungere, rimuovere, esportare, attivare e disattivare i membri di qualsiasi gruppo gestito. Puoi anche modificare i loro profili, aggiungere Aggiornamenti ai loro profili e assegnarli come amministratori di gruppo aggiuntivi per il gruppo.

Se ci sono gruppi al di sopra del gruppo, i loro amministratori possono fare queste cose anche per il tuo gruppo. Lo stesso vale per gli amministratori di Workfront (per qualsiasi gruppo).

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

## Visualizzare e gestire le appartenenze a un gruppo

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **Gruppi**.

   Nell’elenco visualizzato, gli amministratori di Workfront possono visualizzare tutti i gruppi e sottogruppi. Gli amministratori dei gruppi possono visualizzare solo i gruppi e i sottogruppi che amministrano.

1. Fare clic sul nome del gruppo che si desidera modificare.
1. Sulla pagina visualizzata, con **Membri del gruppo** selezionate nel menu a sinistra, effettuate una delle seguenti operazioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Aggiungi un utente al gruppo</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">Fai clic su <strong>Aggiungi membri</strong> <img src="assets/add-icon-plus-in-circle.png">, inizia a digitare il nome dell’utente, quindi selezionalo quando viene visualizzato.</li> 
        <li value="2"> <p>Ripeti questa operazione per tutti gli altri utenti che desideri aggiungere.</p> <p>Puoi fare clic sulla X a destra di un nome se decidi di non aggiungere quell’utente.</p> </li> 
        <li value="3">Fai clic su <strong>Fine</strong> quando hai finito.</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rimuovere un utente dal gruppo</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">Seleziona uno o più nomi utente, quindi fai clic su <strong>Rimuovi membro</strong><img src="assets/remove-icon---x-in-circle.png">.</li> 
        <li value="2"> <p>Fai clic su <strong>Rimuovi</strong> nel messaggio di avviso visualizzato.</p> <p>Per trovare un utente da rimuovere dall’elenco, fai clic su <strong>Cercare persone e gruppi nell’elenco</strong>, digita il nome nella casella, quindi fai clic sul nome quando viene visualizzato.</p> <p><b>NOTA</b>:  
          <ul> 
           <li>Se questo gruppo è il gruppo principale per un utente che si desidera rimuovere, è innanzitutto necessario assegnare un altro gruppo principale nel profilo dell'utente. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/manage-groups/groups-overview/home-groups.md" class="MCXref xref">Panoramica dei gruppi principali</a> e <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Modificare il profilo di un utente</a>.</li> 
           <li>Se il gruppo dispone di un solo amministratore di gruppo e devi rimuoverlo dal gruppo, devi prima assegnare un altro amministratore di gruppo al gruppo.</li> 
           <li>Un utente può appartenere singolarmente a un sottogruppo e al gruppo principale. Quando si rimuove un utente da un sottogruppo, questo rimane parte del gruppo principale. Allo stesso modo, quando li rimuovi dal gruppo principale, rimarranno parte del sottogruppo. Se non si desidera che un utente disponga dell'accesso consentito per il gruppo padre, è necessario rimuovere l'utente sia dai sottogruppi che dal gruppo padre, se questi sono elencati in entrambe le posizioni singolarmente.</li> 
          </ul> </p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Modificare le informazioni di profilo di un utente</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">Seleziona uno o più nomi utente, quindi fai clic su <strong>Modifica</strong> <img src="assets/edit-icon.png">.</li> 
        <li value="2"> <p>Modifica le informazioni sul profilo dell’utente.</p> <p>Per informazioni sulle modifiche apportate, consulta <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Modificare il profilo di un utente</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Esportare i dati di iscrizione utente</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">Seleziona uno o più nomi utente, quindi fai clic su <strong>Esporta</strong> <img src="assets/export.png">.</li> 
        <li value="2"> <p>Esporta i dati come file PDF, Excel o delimitato da tabulazioni.</p> <p>Per ulteriori informazioni sull’esportazione dei dati, consulta <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref">Esportare i dati</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Visualizzare e modificare i ruoli dei gruppi dei membri</td> 
      <td> <p>La <strong>Ruolo gruppo</strong> elenca il ruolo di ciascun membro. In qualità di amministratore di gruppo, è possibile fare doppio clic sul ruolo di un membro per modificarlo.</p> <p>Per i membri del gruppo che non sono amministratori di gruppo, questa colonna non è modificabile.</p> <p>Gli amministratori dei gruppi sono sempre in cima all’elenco.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Invia un commento ai membri del gruppo</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">Seleziona uno o più nomi utente, quindi fai clic su <strong>Aggiorna</strong> <img src="assets/comment-icon.png">.</li> 
        <li value="2">Digita il commento.</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Attivare un utente in Workfront</td> 
      <td>Seleziona uno o più utenti inattivi, quindi fai clic su <strong>Attiva utente</strong> per attivarli in Workfront. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Disattiva un utente in Workfront</td> 
      <td>Seleziona uno o più utenti attivi, quindi fai clic su <strong>Disattiva utente</strong><img src="assets/deactivate-user.png"> per disattivarli in Workfront.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ordina per colonna</td> 
      <td>Fai clic sull’intestazione di una colonna per ordinare l’elenco in base al contenuto della colonna.</td> 
     </tr> 
    </tbody> 
   </table>
