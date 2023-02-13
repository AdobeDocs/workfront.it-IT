---
title: Configurare le impostazioni di approvazione globali
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: In qualità di amministratore di Adobe Workfront, puoi determinare le impostazioni globali per i processi di approvazione in Workfront. Queste impostazioni influiscono su tutti i processi di approvazione degli elementi di lavoro nel sistema.
author: Alina, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2fb0c647-bb6d-46d0-a985-6ab820b4a7f2
source-git-commit: a3cb3d9d340d377e301c98480324bfe8bf507382
workflow-type: tm+mt
source-wordcount: '907'
ht-degree: 3%

---

# Configurare le impostazioni di approvazione globali

In qualità di amministratore di Adobe Workfront, puoi determinare le impostazioni globali per i processi di approvazione in Workfront. Queste impostazioni influiscono su tutti i processi di approvazione degli elementi di lavoro nel sistema.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>È necessario essere un amministratore di sistema o disporre di una licenza di piano con accesso amministrativo ai processi di approvazione</p> <p><b>NOTA</b>: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Configurare le impostazioni di approvazione globali

1. Accedi a Workfront come amministratore Workfront .
1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Fai clic su **Processi** > **Approvazioni** .

1. Fai clic sul pulsante **Impostazioni** icona ![](assets/gear-icon-settings.png) accanto al **Approvazioni** nome dell&#39;area.

1. In **Impostazioni di approvazione** nella casella visualizzata, specificare le seguenti informazioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Aggiungi &lt;number&gt; Giorni alla data di completamento pianificata per accogliere i processi di approvazione</td> 
      <td> <p>Specificare il numero di minuti, ore, giorni, settimane o mesi da aggiungere alla data di completamento pianificata dell'attività che richiede l'approvazione. Selezionare "Trascorsi" minuti, ore, giorni o settimane per aggiungere un orario che includa i fine settimana, le festività e gli orari non lavorativi indicati nel calendario del programma di lavoro del sistema.</p> 
      <p>Ad esempio, se un’attività viene assegnata il venerdì e ha una durata di 3 giorni trascorsi, la data di completamento dell’attività viene impostata per il lunedì (partendo dal presupposto che il sabato e la domenica siano weekend). Se l'attività ha una durata di 3 giorni (non trascorsi), la data di completamento dell'attività è impostata per mercoledì.</p>
      <p><b>NOTA</b>: L’aggiunta di tempo aggiuntivo per l’approvazione delle attività influisce sulla timeline dell’attività e del progetto.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Non è necessario che l'approvatore sia nel team di progetto (per i processi di approvazione che includono una mansione)</td> 
      <td> <p>Selezionare questa opzione se non è necessario che un approvatore faccia parte del team del progetto quando un processo di approvazione include un ruolo. Quando si assegna la decisione di approvazione a un ruolo di lavoro, l'approvazione verrà visualizzata solo dagli utenti a cui è associato un ruolo nel progetto. Se abiliti questa impostazione, qualsiasi utente con quel ruolo di lavoro riceve la richiesta di approvazione, che si trovi o meno nel team di progetto. Per informazioni sulla modifica del ruolo di progetto di un utente, consulta <a href="../../../manage-work/projects/planning-a-project/manage-project-team.md" class="MCXref xref">Gestione del team del progetto</a>. </p> 
      <p><b>SUGGERIMENTO</b>: Quando assegni un'approvazione a un ruolo e a un'opzione <b>L’approvatore non deve far parte del team di progetto (per i processi di approvazione che includono un ruolo)</b> è disabilitato, ma non ci sono ruoli nel team di progetto che corrispondono al ruolo nell'approvazione, l'approvazione viene riassegnata al proprietario del progetto. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Disabilita la delega delle approvazioni</td> 
      <td> <p>Selezionare questa opzione per disabilitare la funzionalità che consente agli utenti del sistema di delegare le approvazioni a un altro utente. Quando questa opzione è selezionata, l’opzione per delegare le approvazioni viene rimossa da Workfront e tutte le delegazioni di approvazione esistenti vengono arrestate.</p> <p>Per ulteriori informazioni sulla delega delle approvazioni in Workfront, vedi <a href="../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md" class="MCXref xref">Delega richiesta di approvazione</a> .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Consenti modifica del modulo personalizzato quando il progetto, l'attività o il problema è nello stato di approvazione in sospeso</td> 
      <td> <p>Selezionare questa opzione per consentire agli utenti di modificare la forma personalizzata di progetti, attività e problemi quando si trova nello stato Approvazione in sospeso. Questa è l’impostazione predefinita.</p> 
      <p>Quando questa opzione è selezionata:</p> 
       <ul> 
       <li>Tutti gli approvatori (e tutti gli altri utenti che hanno accesso alla modifica del modulo personalizzato) possono apportare modifiche al modulo personalizzato quando l'oggetto è in attesa di approvazione, indipendentemente dal percorso di approvazione o dal passaggio di approvazione corrente.</li> 
       <li>Le modifiche apportate al modulo personalizzato durante un processo di approvazione non influiscono sulle decisioni di approvazione effettuate prima della modifica.</li> 
       <li> <p>Le modifiche apportate al progetto, all'attività o al problema vengono tracciate nello stesso modo, indipendentemente da questa impostazione. </p> <p>Ad esempio, se si aggiungono campi modulo personalizzati da tracciare nel flusso di aggiornamento, tutte le modifiche apportate al modulo vengono tracciate nel flusso di aggiornamento dell’oggetto.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Consenti agli utenti di richiamare le richieste di nuova creazione in attesa di approvazione</td> 
      <td> <p>Seleziona questa opzione per configurare se gli utenti possono richiamare un problema o una richiesta in attesa di approvazione per il loro primo stato. Puoi associare il primo stato di un problema o di una richiesta a un processo di approvazione configurando le code di richieste. </p> 
      <p>Per ulteriori informazioni sulle code di richiesta, vedi <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Creare una coda di richiesta</a>.</p> 
      <p>Esegui una delle operazioni seguenti:</p> 
       <ul> 
       <li>Seleziona questa opzione per consentire agli utenti di richiamare un’approvazione per il primo stato di un problema o di una richiesta. In questo caso, possono visualizzare un pulsante Richiama&lt; su un nuovo problema o richiesta in attesa di approvazione. Quando scelgono di richiamare il problema, riceveranno un avviso che avvisa che anche il problema verrà eliminato. Il problema viene eliminato dopo che hanno confermato il loro richiamo. </li> 
       <li> <p>Deseleziona questa opzione per impedire agli utenti di richiamare un problema o una richiesta il cui primo stato è in attesa di approvazione. Non possono visualizzare un pulsante Richiama&lt; sul nuovo problema o richiesta e l'approvazione deve essere rilasciata. Questa è l’opzione predefinita.</p> 
       <p>Per ulteriori informazioni sulla revisione degli elementi in attesa di approvazione, consulta <a href="../../../review-and-approve-work/manage-approvals/view-approvals.md" class="MCXref xref">Visualizza approvazioni </a>.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Salva le modifiche.**
