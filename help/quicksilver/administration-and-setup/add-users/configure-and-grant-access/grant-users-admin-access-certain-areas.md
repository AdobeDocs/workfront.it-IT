---
title: Concedere agli utenti l'accesso amministrativo ad alcune aree
description: In qualità di amministratore di Adobe Workfront, puoi utilizzare un livello di accesso per concedere agli utenti con una licenza Pianificazione l’accesso amministrativo a determinate aree del sistema.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 9d12895d-cf7f-41c6-a2ac-bb731770c187
source-git-commit: c887569d59c7751210671cab97c492ee1752fffc
workflow-type: tm+mt
source-wordcount: '843'
ht-degree: 2%

---

# Concedere agli utenti l&#39;accesso amministrativo a determinate aree

<!--Linked in several places, do not rename or change URL.-->

In qualità di amministratore di Adobe Workfront, puoi utilizzare un livello di accesso per concedere agli utenti con una licenza Pianificazione l’accesso amministrativo a determinate aree del sistema.

>[!NOTE]
>
>Ciò è diverso dall&#39;assegnare a un utente l&#39;accesso amministrativo completo a Workfront, come illustrato in [Concedere a un utente l&#39;accesso amministrativo completo](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).&#x200B;

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
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore di Workfront.</p> <p><b>NOTA</b>: se non disponi ancora dell'accesso, chiedi all'amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Concedere agli utenti del piano l&#39;accesso amministrativo ad alcune aree di Workfront

>[!IMPORTANT]
>
>È consigliabile lasciare invariati i livelli di accesso incorporati in modo da potervi fare riferimento dopo aver configurato gli utenti. Per personalizzare un livello di accesso, copiare il livello di accesso predefinito e modificare la copia. Questa operazione può essere eseguita per ogni livello di accesso, ad eccezione di Amministratore di sistema e Utente esterno.

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Livelli di accesso**.
1. Fare clic sul nome del livello di accesso che si desidera utilizzare per concedere agli utenti l&#39;accesso amministrativo a determinate aree di Workfront.
1. Nella sezione **Consenti accesso amministrativo per**, selezionare le caselle di controllo per concedere l&#39;accesso amministrativo necessario.

   Queste opzioni ti consentono di concedere le seguenti funzionalità:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Processi di approvazione</td> 
      <td><p>Crea e gestisci i processi di approvazione per l’utilizzo in tutto il sistema e per gruppi specifici.</p><p>Senza questo accesso, gli utenti possono creare solo processi di approvazione ad hoc sugli elementi che hanno accesso da gestire.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aziende</td> 
      <td><p>Aggiungere nuove società e modificare quelle esistenti in Workfront</p>
      <p>Senza questo accesso, gli utenti possono solo visualizzare le aziende esistenti.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Moduli personalizzati</td> 
      <td><p>Creare e modificare (aggiungere, modificare ed eliminare i campi) i moduli personalizzati all’interno del loro gruppo.</p><p>Senza questo accesso, gli utenti possono allegare i moduli esistenti solo agli oggetti a cui hanno accesso per contribuire o gestire.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tassi di cambio</td> 
      <td> <p>Aggiungi nuova valuta in Workfront.</p> <p>Senza questo accesso, l’utente può solo aggiungere una valuta esistente a un progetto che ha creato.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Spese</td> 
      <td><p>Visualizza tutte le spese sugli oggetti in Workfront.</p><p>Ciò non consente all’utente di creare nuovi Tipi di Spesa.</p><p>Senza questo accesso, l’utente può visualizzare solo quanto segue:</p>
       <ul>
        <li>Spese per progetti, attività o problemi da loro gestiti</li>
        <li>Le proprie spese</li>
        <li>Le spese dei loro subordinati</li>
       </ul></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mansioni</td> 
      <td> <p>Con questo accesso, l’utente può effettuare le seguenti operazioni:</p> 
       <ul> 
        <li>Visualizza e modifica i ruoli esistenti</li> 
        <li>Aggiungi nuove mansioni</li> 
        <li>Modifica fatturazione mansioni e tassi di costo</li> 
       </ul> <p><b>IMPORTANTE</b>: se si concede a un utente Planner l'accesso amministrativo alle mansioni, l'impostazione di accesso ai dati finanziari Modifica fatturazione mansione e tassi di costo viene abilitata automaticamente per l'utente. In seguito, se si disabilita l'accesso amministrativo alle mansioni per l'utente Planner, le mansioni saranno ancora visibili perché l'impostazione Modifica fatturazione mansione e tassi di costo è ancora abilitata. Se ciò accade e devi rimuovere l’accesso dell’utente per visualizzare le mansioni, devi disabilitare l’impostazione di autorizzazione Modifica fatturazione mansione e tassi di costo dell’utente. Per istruzioni, vedere <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Concedere l'accesso ai dati finanziari</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Milestone nel mio gruppo</td> 
      <td>Visualizza tutti i percorsi milestone nel sistema nel menu Percorsi milestone in Configurazione. Gli utenti possono anche modificare o eliminare qualsiasi percorso milestone appartenente a uno qualsiasi dei loro gruppi. Gli utenti non possono gestire (modificare o eliminare) i percorsi milestone non assegnati a nessuno dei loro gruppi.<br><p>Senza questo accesso, gli utenti possono solo visualizzare i percorsi milestone esistenti e applicarli ai progetti che hanno accesso per gestire.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notifiche promemoria</td> 
      <td>Crea e gestisci le notifiche dei promemoria in Workfront.<br>Senza questo accesso, gli utenti possono ricevere e visualizzare solo le notifiche.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Schede orario e ore</td> 
      <td> <p>Consente agli utenti di visualizzare tutte le ore e le schede orario in Workfront.</p> <p>Se questa opzione è disabilitata, gli utenti possono visualizzare solo le ore per:</p> 
       <ul> 
        <li>Progetti, attività o problemi da loro gestiti</li> 
        <li>Scheda orario personale</li> 
        <li>Una scheda orario di qualcuno che fa riferimento a loro</li> 
        <li>Una scheda orario da approvare</li> 
       </ul> <p><b>NOTA</b>:  <p>Se questa opzione è abilitata o disabilitata, gli amministratori dei gruppi possono creare profili di schede orario per i gruppi e i sottogruppi che gestiscono e assegnarli ai membri del gruppo i cui profili utente hanno accesso alla modifica.</p> <p>L’abilitazione di questa opzione potrebbe fornire un accesso eccessivo ad alcuni amministratori di gruppi, in quanto possono visualizzare le schede orario generate dai profili delle schede orario (e le ore) per tutti gli utenti del sistema, non solo per quelli dei gruppi che amministrano. È possibile disattivare questa opzione per gli amministratori di gruppi che non necessitano di questo livello di accesso.</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Al termine, fare clic su **Salva**.
1. Assegnare il nuovo livello di accesso a un utente, come descritto in [Aggiungi utenti](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

   >[!NOTE]
   >
   >Puoi consentire agli utenti di avere accesso come amministratore. Per ulteriori informazioni su come concedere agli utenti l&#39;accesso amministrativo per gestire gli account utente, vedere [Concedere l&#39;accesso agli utenti](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
