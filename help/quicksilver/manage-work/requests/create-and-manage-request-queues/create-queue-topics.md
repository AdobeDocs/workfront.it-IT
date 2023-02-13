---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Crea argomenti coda
description: Gli argomenti della coda funzionano insieme alle regole di instradamento per assegnare automaticamente il lavoro in arrivo a un utente, a un ruolo di lavoro, a un team o per inserirlo in un progetto. Gli argomenti della coda definiscono le condizioni che devono esistere per l'implementazione della regola di routing.
author: Alina
feature: Work Management
exl-id: 65a74698-011f-4caa-9739-d7510faeb66f
source-git-commit: 7b61f6d9380365daa614c597ee7755d6d01d915d
workflow-type: tm+mt
source-wordcount: '885'
ht-degree: 3%

---

# Crea argomenti coda

Gli argomenti della coda funzionano insieme alle regole di instradamento per assegnare automaticamente il lavoro in arrivo a un utente, a un ruolo di lavoro, a un team o per inserirlo in un progetto. Gli argomenti della coda definiscono le condizioni che devono esistere per l&#39;implementazione della regola di routing.

Non esiste alcun limite al numero di argomenti della coda che possono essere assegnati a un gruppo di argomenti o a un progetto. Gli argomenti della coda sono un tipo di oggetto di reporting.

## Requisiti di accesso

<!--drafted - replace table with P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p> Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Devi disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica accesso a progetti</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p> Gestisci le autorizzazioni per il progetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere il piano, il tipo di licenza o l&#39;accesso a cui hai accesso, contatta il tuo amministratore Workfront

## Crea un argomento della coda

1. Creare una regola di instradamento, un gruppo di argomenti e un modulo personalizzato, se si intende associarli all&#39;argomento della coda.\
   Per ulteriori informazioni su come creare regole di instradamento, gruppi di argomenti o moduli personalizzati, vedere i seguenti articoli:

   * [Creare regole di routing](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md)
   * [Crea gruppi di argomenti](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md)
   * [Creare o modificare un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

1. Vai al progetto che hai scelto per abilitare come coda di richiesta della Guida e dove desideri creare un nuovo argomento della coda.\
   Per ulteriori informazioni su come designare un progetto come coda di richiesta della Guida, consulta il seguente articolo:\
   [Creare una coda di richiesta](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)

   È possibile organizzare gli argomenti relativi alla coda sotto un gruppo di argomenti o direttamente sotto il progetto designato come coda di richiesta della Guida. Questo fornirà al richiedente una serie di menu a discesa quando effettua una richiesta.\
   È possibile nidificare gli argomenti della coda direttamente sotto il progetto designato come coda di richiesta della Guida, senza un gruppo di argomenti.

   Per informazioni sulla creazione di gruppi di argomenti, consulta [Crea gruppi di argomenti](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md).

1. Fai clic su **Argomenti coda** nel pannello a sinistra. Potrebbe essere necessario fare clic su **Mostra altro**, quindi **Argomenti coda**.
1. Fai clic su **Nuovo argomento coda**.
1. Sulla **Nuovo argomento coda** specificare quanto segue:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Nome</strong> </td> 
      <td> Nome dell'argomento della coda.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Descrizione</strong> </td> 
      <td>Descrivi la coda richieste. La descrizione viene visualizzata quando gli utenti selezionano l’argomento della coda nel processo di invio di una nuova richiesta. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Aggiungi a gruppo argomenti</strong> </td> 
      <td> Se il progetto non contiene gruppi di argomenti, il nome del progetto verrà impostato come gruppo di argomenti predefinito.<br>Per creare altri gruppi di argomenti, seleziona <strong>Crea nuovo gruppo di argomenti</strong> dal menu a discesa.<br><img src="assets/create-new-topic-group-within-queue-topic-350x203.png" alt="create_new_topic_group_within_queue_topic.png" style="width: 350;height: 203;"></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Moduli personalizzati</strong> </td> 
      <td>Selezionare i moduli personalizzati da associare all’argomento della coda. È necessario creare moduli personalizzati per i problemi prima di poterli associare agli argomenti della coda. Per informazioni sulla creazione di moduli personalizzati, vedere <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Creare o modificare un modulo personalizzato</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Approvazione predefinita</td> 
      <td> <p>Associa un processo di approvazione a questo argomento della coda. Solo i processi di approvazione dei problemi sono visibili in questo menu a discesa. Tutti i problemi inviati a questa coda saranno associati a questo processo di approvazione. Per poter essere associati ad argomenti della coda, l’amministratore di Adobe Workfront deve definire i processi di approvazione a livello di sistema. <span>Un utente con accesso amministrativo ai processi di approvazione può anche creare processi di approvazione specifici per gruppo.</span> Per ulteriori informazioni sulla creazione dei processi di approvazione, consulta <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Creazione di un processo di approvazione per gli elementi di lavoro</a>.<br></p> 
       <div> 
        <p>Importante: Se il gruppo del progetto cambia, il processo di approvazione specifico per gruppo allegato ai problemi esistenti diventa un processo di approvazione a uso singolo. Per ulteriori informazioni su come le modifiche apportate al gruppo del progetto o al processo di approvazione influiscono sulle impostazioni di approvazione, vedere <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">Effetti delle modifiche al processo di approvazione e di gruppo sui processi di approvazione assegnati</a>.</p> 
        <p>Quando aggiungi processi di approvazione agli argomenti della coda, considera quanto segue: </p> 
        <ul style="list-style-type: circle;"> 
         <li>Nell’elenco vengono visualizzati solo i processi di approvazione attivi. </li> 
         <li> <p>Nell'elenco vengono visualizzati i processi di approvazione a livello di sistema e di gruppo. Un processo di approvazione associato a un gruppo diverso da quello del progetto non viene visualizzato nell’elenco.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Durata predefinita</strong> </td> 
      <td>Si tratta della durata predefinita della richiesta e la data di completamento pianificata della richiesta viene calcolata in base a questo valore.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Instradimento Predefinito</strong> </td> 
      <td>Specificare la regola di routing che si desidera associare all'argomento della coda. È necessario creare la regola di routing prima di poterla allegare a un argomento della coda.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Tipi di richieste</strong> </td> 
      <td> <p>Scegli il tipo di richieste che l'argomento della coda memorizza. Le opzioni visibili sono impostate sul <strong>Dettagli coda</strong> scheda del progetto. Questo è un campo obbligatorio. </p> <p>Nota: I tipi di richiesta vengono visualizzati come selezione nell'area Richieste solo se il tipo di richiesta è selezionato nelle pagine Dettagli coda e Argomento coda. Per informazioni sulla configurazione dell'area Dettagli coda di un progetto, consulta <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Creare una coda di richiesta</a>. </p> <p>Seleziona uno dei seguenti tipi:</p> 
       <ul> 
        <li>Segnalazione Bug</li> 
        <li>Richiesta di Modifica</li> 
        <li>Problema</li> 
        <li>Richiesta</li> 
       </ul> <p>È possibile che l’amministratore di Workfront abbia rinominato alcune di queste opzioni. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/new-queue-topic-box-nwe-350x375.png)

1.  
1. Fai clic su **Salva**.\
   L’argomento della coda è ora disponibile per l’utilizzo ed è visibile nell’area Richieste di Workfront, dopo aver selezionato una coda di richiesta e un gruppo di argomenti.
