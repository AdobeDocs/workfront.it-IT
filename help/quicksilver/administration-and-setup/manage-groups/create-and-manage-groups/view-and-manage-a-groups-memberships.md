---
user-type: administrator
product-area: system-administration;user-management
keywords: aggiungi,utenti,gruppo,aggiungi,altro,assegna,amministratore,rimuovi,utente,visualizzazione,ruoli,membri,esportazione,appartenenza,dati
navigation-topic: create-and-manage-groups
title: Visualizzare e gestire le appartenenze di un gruppo
description: In qualità di amministratore di Adobe Workfront, puoi visualizzare, aggiungere, rimuovere, esportare, attivare e disattivare i membri di qualsiasi gruppo gestito. Puoi anche modificarne i profili, aggiungervi aggiornamenti e assegnarli come amministratori di gruppo aggiuntivi per il gruppo.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 219e5fa3-cf25-477d-82f6-046e3ff30989
source-git-commit: c23b3967cf06aaff1bcd7465ce6c7a0c7b7fe9af
workflow-type: tm+mt
source-wordcount: '750'
ht-degree: 0%

---

# Visualizzare e gestire le appartenenze di un gruppo

In qualità di amministratore di Adobe Workfront, puoi visualizzare, aggiungere, rimuovere, esportare, attivare e disattivare i membri di qualsiasi gruppo gestito. Puoi anche modificarne i profili, aggiungervi aggiornamenti e assegnarli come amministratori di gruppo aggiuntivi per il gruppo.

Se ci sono gruppi al di sopra del gruppo, gli amministratori possono eseguire queste operazioni anche per il gruppo. Lo stesso vale per gli amministratori di Workfront (per qualsiasi gruppo).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td><p>Nuovo: Standard</p>
       <p>Oppure</p>
       <p>Corrente: Piano</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td>Devi essere un amministratore di gruppo del gruppo o un amministratore di sistema.</td>
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visualizzare e gestire le appartenenze di un gruppo

{{step-1-to-setup}}

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
       <ol> 
        <li>Fare clic su <strong>Aggiungi membri</strong> <img src="assets/add-icon-plus-in-circle.png">, iniziare a digitare il nome dell'utente, quindi selezionarlo quando viene visualizzato.</li>
        <li> <p>Ripetere l'operazione per tutti gli altri utenti che si desidera aggiungere.</p> <p>Se si decide di non aggiungere un utente, è possibile fare clic sulla X a destra di un nome.</p> </li>
        <li>Al termine, fai clic su <strong>Fine</strong>.</li>
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rimuovere un utente dal gruppo</td> 
      <td> 
       <ol> 
        <li>Selezionare uno o più nomi utente, quindi fare clic su <strong>Rimuovi membro</strong><img src="assets/remove-icon---x-in-circle.png">.</li> 
        <li> <p>Fare clic su <strong>Rimuovi</strong> nel messaggio di avviso visualizzato.</p> <p>Per trovare un utente da rimuovere dall'elenco, fare clic su <strong>Cerca persone e gruppi nell'elenco</strong>, digitarne il nome nella casella e fare clic sul nome quando viene visualizzato.</p> <p><b>NOTA</b>:  
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
       <ol> 
        <li>Seleziona uno o più nomi utente, quindi fai clic su <strong>Modifica</strong> <img src="assets/edit-icon.png">.</li> 
        <li> <p>Modifica le informazioni sul profilo dell’utente.</p> <p>Per informazioni sulle modifiche che è possibile apportare, vedere <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Modificare il profilo di un utente</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Esporta dati di iscrizione utente</td> 
      <td> 
       <ol> 
        <li>Seleziona uno o più nomi utente, quindi fai clic su <strong>Esporta</strong> <img src="assets/export.png">.</li> 
        <li> <p>Esporta i dati come file delimitato da tabulazioni, PDF o Excel.</p> <p>Per ulteriori informazioni sull'esportazione dei dati, vedere <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref">Esporta dati</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Visualizzare e modificare i ruoli gruppo dei membri</td> 
      <td> <p>La colonna <strong>Ruolo gruppo</strong> elenca il ruolo di ogni membro. In qualità di amministratore di gruppo, puoi fare doppio clic sul ruolo di un membro per modificarlo.</p> <p>Questa colonna non è modificabile per i membri del gruppo che non sono amministratori di gruppo.</p> <p>Gli amministratori di gruppi sono sempre in cima all’elenco.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Invia un commento ai membri del gruppo</td> 
      <td> 
       <ol> 
        <li>Selezionare almeno un membro del gruppo, quindi fare clic su <strong>Invia aggiornamento all'utente</strong> nella barra degli strumenti.</li> 
        <li><p>Digita il commento da inviare agli utenti e alla sezione Aggiornamenti dei loro profili utente.</p>
        <p>Per ulteriori informazioni, vedere <a href="/help/quicksilver/people-teams-and-groups/work-directly-with-others/send-direct-messages-to-other-users.md">Inviare messaggi diretti ad altri utenti</a>.</p></li> 
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
