---
title: Configurare le impostazioni di approvazione globali
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: In qualità di amministratore di Adobe Workfront, puoi determinare le impostazioni globali per i processi di approvazione in Workfront. Queste impostazioni hanno effetto su tutti i processi di approvazione degli elementi di lavoro nel sistema.
author: Alina, Lisa
feature: System Setup and Administration
role: Admin
exl-id: 2fb0c647-bb6d-46d0-a985-6ab820b4a7f2
source-git-commit: 1397702a6b50953e7abcfe491b95aeb8b981df5b
workflow-type: tm+mt
source-wordcount: '879'
ht-degree: 2%

---

# Configurare le impostazioni di approvazione globali

In qualità di amministratore di Adobe Workfront, puoi determinare le impostazioni globali per i processi di approvazione in Workfront. Queste impostazioni hanno effetto su tutti i processi di approvazione degli elementi di lavoro nel sistema.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>È necessario essere amministratore di sistema o disporre di una licenza Pianificazione con accesso amministrativo ai processi di approvazione</p> <p><b>NOTA</b>: se non disponi ancora dell'accesso, chiedi all'amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

+++

## Configurare le impostazioni di approvazione globali

{{step-1-to-setup}}

1. Fare clic su **Processi** > **Approvazioni**.

1. Fai clic sull&#39;icona **Impostazioni** ![Icona Impostazioni ingranaggio](assets/gear-icon-settings.png) accanto al nome dell&#39;area **Approvazioni**.

1. Nella casella **Impostazioni approvazione** visualizzata, specificare le informazioni seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Aggiungi &lt;number&gt; giorni alla data di completamento pianificata per i processi di approvazione</td> 
      <td> <p>Specificare il numero di minuti, ore, giorni, settimane o mesi per aggiungere tempo alla data di completamento pianificata dell'attività che deve essere approvata. Selezionare "Trascorsi" minuti, ore, giorni o settimane per aggiungere l'ora che include tutti i fine settimana, le festività e le ore non lavorative specificate nel calendario della programmazione del lavoro di sistema.</p> 
      <p>Ad esempio, se un'attività viene assegnata il venerdì e ha una durata di 3 giorni, la data di completamento dell'attività viene impostata per il lunedì (supponendo che sabato e domenica siano un fine settimana). Se l'attività ha una durata di 3 giorni (non trascorsa), la data di completamento dell'attività viene impostata su Mercoledì.</p>
      <p><b>NOTA</b>: l'abilitazione di un tempo aggiuntivo per l'approvazione delle attività influirà sulla sequenza temporale dell'attività e del progetto.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Non è necessario che l'approvatore sia nel team di progetto (per i processi di approvazione che includono una mansione)</td> 
      <td> <p>Selezionare questa opzione se non è necessario che un approvatore appartenga al team di progetto quando un processo di approvazione include un ruolo. Qualsiasi utente con tale mansione riceve la richiesta di approvazione indipendentemente dal fatto che si trovi o meno nel team del progetto, anche se non gli viene concesso automaticamente l’accesso al progetto. Per informazioni sulla modifica del ruolo di progetto di un utente, vedere <a href="../../../manage-work/projects/planning-a-project/manage-project-team.md" class="MCXref xref">Gestione del team di progetto</a>. </p> 
      <p><b>SUGGERIMENTO</b>: quando si assegna un'approvazione a un ruolo e l'opzione <b>Approvatore non obbligatorio nel team di progetto (per i processi di approvazione che includono un ruolo)</b> è disabilitata, ma non vi sono ruoli nel team di progetto che corrispondono al ruolo nell'approvazione, l'approvazione viene riassegnata al proprietario del progetto. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Disabilita la delega delle approvazioni</td> 
      <td> <p>Seleziona questa opzione per disabilitare la funzionalità di delega delle approvazioni a un altro utente da parte degli utenti del sistema. Quando questa opzione è selezionata, l’opzione di delega delle approvazioni viene rimossa da Workfront e tutte le deleghe di approvazione esistenti vengono interrotte.</p> <p>Per ulteriori informazioni sulla delega delle approvazioni in Workfront, vedere <a href="../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md" class="MCXref xref">Delegare la richiesta di approvazione</a> .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Consenti modifica del modulo personalizzato quando il progetto, l’attività o il problema è in attesa di approvazione</td> 
      <td> <p>Selezionare questa opzione per consentire agli utenti di modificare il modulo personalizzato di progetti, attività e problemi nello stato In attesa di approvazione. Questa è l'impostazione predefinita.</p> 
      <p>Quando questa opzione è selezionata:</p> 
       <ul> 
       <li>Tutti gli approvatori (e tutti gli altri utenti che hanno accesso alla modifica del modulo personalizzato) possono apportare modifiche al modulo personalizzato quando l’oggetto è in attesa di approvazione, indipendentemente dal percorso di approvazione o dal passaggio di approvazione corrente.</li> 
       <li>Le modifiche apportate al modulo personalizzato durante un processo di approvazione non influiscono sulle decisioni di approvazione eseguite prima della modifica.</li> 
       <li> <p>Tutte le modifiche apportate al progetto, all’attività o al problema vengono tracciate allo stesso modo, indipendentemente da questa impostazione. </p> <p>Ad esempio, se sono stati aggiunti campi modulo personalizzati da tracciare nel flusso di aggiornamento, tutte le modifiche apportate al modulo verranno tracciate nel flusso di aggiornamento dell'oggetto.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Consenti agli utenti di richiamare le richieste di nuova creazione in attesa di approvazione</td> 
      <td> <p>Seleziona questa opzione per configurare se gli utenti possono richiamare un problema o una richiesta in attesa di approvazione per il loro primo stato. È possibile associare il primo stato di un problema o di una richiesta a un processo di approvazione configurando le code delle richieste. </p> 
      <p>Per ulteriori informazioni sulle code di richieste, vedere <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Creare una coda di richieste</a>.</p> 
      <p>Esegui una delle operazioni seguenti:</p> 
       <ul> 
       <li>Selezionare questa opzione per consentire agli utenti di richiamare un'approvazione per il primo stato di un problema o di una richiesta. In questo caso, può visualizzare il pulsante Recall&lt; (Richiama) su un nuovo problema o richiesta con stato in attesa di approvazione. Quando sceglie di richiamare il problema, riceve un avviso che indica che anche il problema verrà eliminato. Il problema viene cancellato dopo che hanno confermato di averlo richiamato. </li> 
       <li> <p>Deseleziona questa opzione per impedire agli utenti di richiamare un problema o una richiesta il cui primo stato è In attesa di approvazione. Non visualizzano il pulsante Recall&lt; (Richiama) sul nuovo problema o sulla nuova richiesta ed è necessario concedere l’approvazione. Questa è l'opzione predefinita.</p> 
       <p>Per ulteriori informazioni sulla revisione degli elementi in attesa di approvazione, vedere <a href="../../../review-and-approve-work/manage-approvals/view-approvals.md" class="MCXref xref">Visualizza approvazioni </a>.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Salva modifiche.**
