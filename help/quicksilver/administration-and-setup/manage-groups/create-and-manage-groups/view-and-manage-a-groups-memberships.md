---
user-type: administrator
product-area: system-administration;user-management
keywords: aggiungi,utenti,gruppo,aggiungi,altro,assegna,amministratore,rimuovi,utente,visualizzazione,ruoli,membri,esportazione,appartenenza,dati
navigation-topic: create-and-manage-groups
title: Visualizzare e gestire le appartenenze di un gruppo
description: In qualità di amministratore di Adobe Workfront, puoi visualizzare, aggiungere, rimuovere, esportare, attivare e disattivare i membri di qualsiasi gruppo gestito. Puoi anche modificarne i profili, aggiungervi aggiornamenti e assegnarli come amministratori di gruppo aggiuntivi per il gruppo.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 219e5fa3-cf25-477d-82f6-046e3ff30989
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 1%

---

# Visualizzare e gestire le appartenenze di un gruppo

In qualità di amministratore di Adobe Workfront, puoi visualizzare, aggiungere, rimuovere, esportare, attivare e disattivare i membri di qualsiasi gruppo gestito. Puoi anche modificarne i profili, aggiungervi aggiornamenti e assegnarli come amministratori di gruppo aggiuntivi per il gruppo.

Se ci sono gruppi al di sopra del gruppo, gli amministratori possono eseguire queste operazioni anche per il gruppo. Lo stesso vale per gli amministratori di Workfront (per qualsiasi gruppo).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Workfront*</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> <p>Devi essere un amministratore di gruppo del gruppo o un amministratore di Workfront. Per ulteriori informazioni, vedere <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Amministratori di gruppi</a> e <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente l'accesso amministrativo completo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano o il tipo di licenza di cui si dispone, contattare l&#39;amministratore di Workfront.

## Visualizzare e gestire le appartenenze di un gruppo

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **menu principale** nell&#39;angolo superiore destro di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **Gruppi**.

   Nell’elenco visualizzato, gli amministratori di Workfront possono visualizzare tutti i gruppi e i sottogruppi. Gli amministratori di gruppi possono visualizzare solo i gruppi e i sottogruppi che amministrano.

1. Fare clic sul nome del gruppo da modificare.
1. Nella pagina visualizzata, con **Membri gruppo** selezionati nel menu a sinistra, eseguire una delle operazioni seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Aggiungere un utente al gruppo</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">Fare clic su <strong>Aggiungi membri</strong> <img src="assets/add-icon-plus-in-circle.png">, iniziare a digitare il nome dell'utente, quindi selezionarlo quando viene visualizzato.</li> 
        <li value="2"> <p>Ripetere l'operazione per tutti gli altri utenti che si desidera aggiungere.</p> <p>Se si decide di non aggiungere un utente, è possibile fare clic sulla X a destra di un nome.</p> </li> 
        <li value="3">Al termine, fai clic su <strong>Fine</strong>.</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rimuovere un utente dal gruppo</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">Selezionare uno o più nomi utente, quindi fare clic su <strong>Rimuovi membro</strong><img src="assets/remove-icon---x-in-circle.png">.</li> 
        <li value="2"> <p>Fare clic su <strong>Rimuovi</strong> nel messaggio di avviso visualizzato.</p> <p>Per trovare un utente da rimuovere dall'elenco, fare clic su <strong>Cerca persone e gruppi nell'elenco</strong>, digitarne il nome nella casella e fare clic sul nome quando viene visualizzato.</p> <p><b>NOTA</b>:  
          <ul> 
           <li>Se questo è il Gruppo Predefinito per un utente che si desidera rimuovere, è necessario innanzitutto assegnare un altro Gruppo Predefinito nel profilo dell'utente. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/manage-groups/groups-overview/home-groups.md" class="MCXref xref">Panoramica sui gruppi principali</a> e <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Modifica il profilo di un utente</a>.</li> 
           <li>Se il gruppo ha un solo amministratore e devi rimuoverlo dal gruppo, devi prima assegnare al gruppo un altro amministratore.</li> 
           <li>Un utente può appartenere individualmente a un sottogruppo e al gruppo principale. Quando si rimuove qualcuno da un sottogruppo, questo rimane parte del gruppo principale. Analogamente, quando li rimuovete dal gruppo principale, rimarranno parte del sottogruppo. Se non si desidera che un utente disponga dell'accesso consentito per il gruppo padre, è necessario rimuovere l'utente sia dai sottogruppi che dal gruppo padre, se sono elencati singolarmente in entrambi i punti.</li> 
          </ul> </p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Modificare le informazioni del profilo di un utente</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">Seleziona uno o più nomi utente, quindi fai clic su <strong>Modifica</strong> <img src="assets/edit-icon.png">.</li> 
        <li value="2"> <p>Modifica le informazioni sul profilo dell’utente.</p> <p>Per informazioni sulle modifiche che è possibile apportare, vedere <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Modificare il profilo di un utente</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Esporta dati di iscrizione utente</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">Seleziona uno o più nomi utente, quindi fai clic su <strong>Esporta</strong> <img src="assets/export.png">.</li> 
        <li value="2"> <p>Esporta i dati come file PDF, Excel o delimitato da tabulazioni.</p> <p>Per ulteriori informazioni sull'esportazione dei dati, vedere <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref">Esporta dati</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Visualizzare e modificare i ruoli gruppo dei membri</td> 
      <td> <p>La colonna <strong>Ruolo gruppo</strong> elenca il ruolo di ogni membro. In qualità di amministratore di gruppo, puoi fare doppio clic sul ruolo di un membro per modificarlo.</p> <p>Questa colonna non è modificabile per i membri del gruppo che non sono amministratori di gruppo.</p> <p>Gli amministratori di gruppi sono sempre in cima all’elenco.</p> </td> 
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
      <td role="rowheader">Disattivare un utente in Workfront</td> 
      <td>Seleziona uno o più utenti attivi, quindi fai clic su <strong>Disattiva utente</strong><img src="assets/deactivate-user.png"> per disattivarli in Workfront.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ordina per colonna</td> 
      <td>Fare clic sull'intestazione di una colonna per ordinare l'elenco in base al contenuto della colonna.</td> 
     </tr> 
    </tbody> 
   </table>
