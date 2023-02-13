---
title: Consentire agli utenti l'accesso amministrativo a determinate aree
description: In qualità di amministratore di Adobe Workfront, puoi utilizzare un livello di accesso per concedere agli utenti con una licenza di piano l’accesso amministrativo a determinate aree del sistema.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 9d12895d-cf7f-41c6-a2ac-bb731770c187
source-git-commit: 253a116e04e0b3a729331f5d0a29405e82808390
workflow-type: tm+mt
source-wordcount: '846'
ht-degree: 2%

---

# Consentire agli utenti l&#39;accesso amministrativo a determinate aree

<!--Linked in several places, do not rename or change URL.-->

In qualità di amministratore di Adobe Workfront, puoi utilizzare un livello di accesso per concedere agli utenti con una licenza di piano l’accesso amministrativo a determinate aree del sistema.

>[!NOTE]
>
>Ciò è diverso dal fornire a un utente pieno accesso amministrativo a Workfront, come spiegato in [Concedere a un utente pieno accesso amministrativo](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md)&#x200B;

## Requisiti di accesso

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
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso</td> 
   <td> <p>Devi essere un amministratore Workfront.</p> <p><b>NOTA</b>: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Consentire agli utenti del piano l’accesso amministrativo a determinate aree di Workfront

>[!IMPORTANT]
>
>È vivamente consigliato lasciare invariati i livelli di accesso incorporati, in modo da potervi fare riferimento dopo aver configurato gli utenti. Per personalizzare un livello di accesso, copia il livello di accesso predefinito e modifica la copia. (È possibile eseguire questa operazione per ogni livello di accesso, ad eccezione di Amministratore di sistema e Utente esterno.)

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **Livelli di accesso**.
1. Fare clic sul nome del livello di accesso che si desidera utilizzare per concedere agli utenti l&#39;accesso amministrativo a determinate aree di Workfront.
1. In **Consenti accesso amministrativo per** sezione, caselle di controllo per concedere l&#39;accesso amministrativo necessario.

   Queste opzioni ti consentono di concedere le seguenti funzionalità:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Processi di approvazione</td> 
      <td><p>Creare e gestire processi di approvazione da utilizzare in tutto il sistema e per gruppi specifici.</p><p>Senza questo accesso, gli utenti possono creare solo processi di approvazione ad hoc sugli elementi che possono gestire.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aziende</td> 
      <td><p>Aggiungi nuove società e modifica società esistenti in Workfront</p>
      <p>Senza questo accesso, gli utenti possono visualizzare solo le aziende esistenti.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Moduli personalizzati</td> 
      <td><p>Creare e modificare (aggiungere, modificare ed eliminare i campi) moduli personalizzati all’interno del gruppo.</p><p>Senza questo accesso, gli utenti possono allegare i moduli esistenti solo agli oggetti in cui hanno accesso per contribuire o gestire.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tassi di cambio</td> 
      <td> <p>Aggiungi nuova valuta in Workfront.</p> <p>Senza questo accesso, l’utente può solo aggiungere una valuta esistente a un progetto creato.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Spese</td> 
      <td><p>Visualizza tutte le spese relative agli oggetti in Workfront.</p><p>Ciò non consente all'utente di creare nuovi tipi di spesa.</p><p>Senza questo accesso, l'utente può solo visualizzare quanto segue:</p>
       <ul>
        <li>Spese relative a progetti, attività o problemi che gestiscono</li>
        <li>Le proprie spese</li>
        <li>Le spese dei loro subordinati</li>
       </ul></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mansioni</td> 
      <td> <p>Con questo accesso, l'utente può effettuare le seguenti operazioni:</p> 
       <ul> 
        <li>Visualizzare e modificare i ruoli di lavoro esistenti</li> 
        <li>Aggiungi nuovi ruoli di lavoro</li> 
        <li>Modificare la fatturazione dei ruoli e le tariffe dei costi</li> 
       </ul> <p><b>IMPORTANTE</b>: Se si concede a un utente Planner l'accesso amministrativo ai ruoli di lavoro, l'impostazione di accesso ai dati finanziari Modifica fatturazione ruolo e tassi di costo è abilitata automaticamente per l'utente. Successivamente, se si disabilita l'accesso amministrativo ai ruoli di lavoro per l'utente Planner, i ruoli di lavoro saranno ancora visibili all'utente perché l'impostazione Modifica fatturazione e tassi di costo ruolo è ancora abilitata. Se questo accade e devi rimuovere l'accesso dell'utente per visualizzare i ruoli di lavoro, devi disabilitare l'impostazione di autorizzazione Modifica fatturazione ruolo e tassi di costo dell'utente. Per istruzioni, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Concedere l’accesso ai dati finanziari</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Milestone nel mio gruppo</td> 
      <td>Visualizzare tutti i percorsi delle fasi cardine nel sistema nel menu Percorsi Milestone in Configurazione. Gli utenti possono inoltre modificare o eliminare qualsiasi percorso cardine appartenente a uno qualsiasi dei loro gruppi. Gli utenti non possono gestire (modificare o eliminare) i percorsi delle attività cardine non assegnati a nessuno dei loro gruppi.<br><p>Senza questo accesso, gli utenti possono visualizzare solo i percorsi cardine esistenti e applicarli ai progetti a cui hanno accesso per la gestione.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notifiche promemoria</td> 
      <td>Crea e gestisci notifiche di promemoria in Workfront.<br>Senza questo accesso, gli utenti sono limitati alla ricezione e alla visualizzazione di notifiche.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Schede orario e ore</td> 
      <td> <p>Consente agli utenti di visualizzare tutte le ore e i fogli presenze in Workfront.</p> <p>Quando questa opzione è disabilitata, gli utenti possono visualizzare solo ore:</p> 
       <ul> 
        <li>Progetti, attività o problemi che gestiscono</li> 
        <li>Scheda attività propria</li> 
        <li>Scheda attività di un utente che effettua un report</li> 
        <li>Scheda attività approvata</li> 
       </ul> <p><b>NOTA</b>:  <p>Se questa opzione è abilitata o disabilitata, gli amministratori dei gruppi possono creare profili della scheda attività per i gruppi e i sottogruppi che gestiscono e assegnarli ai membri del gruppo i cui profili utente hanno accesso alla modifica.</p> <p>L'abilitazione di questa opzione potrebbe fornire troppo accesso ad alcuni amministratori di gruppo perché possono visualizzare i fogli presenze generati dai profili della scheda attività (e le ore) per tutti gli utenti del sistema, non solo per quelli dei gruppi che amministrano. È possibile disabilitare questa opzione per gli amministratori di gruppo che non hanno bisogno di questo molto accesso.</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Al termine, fai clic su **Salva**.
1. Assegna il nuovo livello di accesso a un utente, come descritto in [Aggiungi utenti](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

   >[!NOTE]
   >
   >Puoi consentire agli utenti di avere accesso amministrativo agli utenti. Per ulteriori informazioni su come consentire agli utenti l&#39;accesso amministrativo agli utenti in modo che possano gestire gli account utente, consulta [Concedere l’accesso agli utenti](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
