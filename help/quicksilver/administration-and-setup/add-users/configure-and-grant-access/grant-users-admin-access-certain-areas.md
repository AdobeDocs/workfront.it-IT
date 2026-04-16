---
title: Concedere agli utenti l'accesso amministrativo ad alcune aree
description: In qualità di amministratore di Adobe Workfront, puoi utilizzare un livello di accesso per concedere agli utenti con una licenza Pianificazione l’accesso amministrativo a determinate aree del sistema.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 9d12895d-cf7f-41c6-a2ac-bb731770c187
source-git-commit: 85399542ce8e92de6da5a1de0960194e72958987
workflow-type: tm+mt
source-wordcount: '686'
ht-degree: 8%

---

# Concedere agli utenti l&#39;accesso amministrativo a determinate aree

<!--Linked in several places, do not rename or change URL.-->

In qualità di amministratore di Adobe Workfront, puoi utilizzare un livello di accesso per concedere agli utenti con una licenza Standard o Plan l’accesso amministrativo a determinate aree del sistema.

>[!NOTE]
>
>Ciò è diverso dall&#39;assegnare a un utente l&#39;accesso amministrativo completo a Workfront, come illustrato in [Concedere a un utente l&#39;accesso amministrativo completo](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).&#x200B;

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td>   <p>Standard</p>
   <p>Piano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore di Workfront.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Concedere agli utenti Standard o Plan l&#39;accesso amministrativo ad alcune aree di Workfront

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


<!--     
     <tr> 
      <td role="rowheader">Job roles</td> 
      <td> <p><b>NOTE</b>: In the Preview environment, access to job roles is controlled as an object type in the access level. See <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-job-roles.md">Grant access to job roles</a>.</p>
      <p>With this access, the user is allowed to do the following:</p> 
       <ul> 
        <li>View and edit existing job roles</li> 
        <li>Add new job roles</li> 
        <li>Edit role billing and cost rates</li> 
       </ul> <p><b>IMPORTANT</b>: If you grant a Standard or Plan user administrative access to job roles, the Financial Data access setting Edit Role Billing &amp; Cost Rates is enabled for the user automatically. Later, if you disable administrative access to job roles for the Standard or Plan user, job roles are still visible to the user because the Edit Role Billing &amp; Cost Rates setting is still enabled. If this happens and you need to remove the user's access to view job roles, you need to disable the user's Edit Role Billing &amp; Cost Rates permission setting. For instructions, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Grant access to financial data</a>.</p> </td> 
     </tr>
-->
