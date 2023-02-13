---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Creare regole di routing
description: Le regole di routing controllano le operazioni eseguite da Adobe Workfront con i problemi quando vengono inviate a una coda di richiesta. Per ulteriori informazioni sulla creazione delle code di richiesta, vedere Creazione di una coda di richiesta.
author: Alina
feature: Work Management
exl-id: 640f9054-f2f8-4594-9311-e93518f58453
source-git-commit: 7b61f6d9380365daa614c597ee7755d6d01d915d
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 2%

---

# Creare regole di routing

Le regole di routing controllano le operazioni eseguite da Adobe Workfront con i problemi quando vengono inviate a una coda di richiesta. Per ulteriori informazioni sulla creazione delle code di richiesta, vedi [Creare una coda di richiesta](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Le regole di routing inviano problemi a utenti o ruoli di lavoro specifici meglio attrezzati per risolvere il problema o la richiesta inoltrati. Le regole di routing sono solitamente associate agli argomenti della coda, utilizzati per controllare quale regola di routing verrà applicata al problema o alla richiesta.

## Requisiti di accesso

<!--drafted - replace the table at P&P:

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
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
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
   <td> <p>Modifica accesso a progetti</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p> Gestisci le autorizzazioni per il progetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per sapere quale piano, tipo di licenza o accesso si dispone, contattare l&#39;amministratore Workfront

## Creare una regola di routing

1. Passa al progetto al quale desideri aggiungere le regole di indirizzamento per le richieste.
1. Fai clic su **Regole di routing** nel pannello a sinistra. Potrebbe essere necessario fare clic su **Mostra altro**, quindi **Regole di routing**.
1. Fai clic su **Nuove regole di routing** per aggiungere la nuova regola.
1. Specifica le seguenti informazioni per la regola di routing:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Nome</strong> </td> 
      <td> <p>Nome della regola di routing. Puoi visualizzare la regola di routing se hai accesso per visualizzare queste informazioni sul progetto.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Descrizione</strong> </td> 
      <td>Aggiungi una descrizione per la regola di routing.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>l'Incaricato Predefinito*</strong> </td> 
      <td>Aggiungi un utente attivo o un ruolo di lavoro attivo a cui assegnare i nuovi problemi. In questo campo è possibile avere un solo assegnatario predefinito. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Team predefinito*</strong> </td> 
      <td>Aggiungi un team attivo a cui assegnare il nuovo problema. In questo campo è possibile avere un solo team predefinito.

   <p><b>NOTA</b></p>

   Dopo aver inviato il problema, puoi modificarne le assegnazioni e assegnare altri utenti, ruoli o team. Per informazioni, consulta  <a href="../../../manage-work/issues/manage-issues/assign-issues.md">Assegnare i problemi </a>.

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Instrada al Progetto</strong> </td> 
      <td>Questo è il progetto in cui viene aggiunto il problema.</td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >*Se un utente, un ruolo o un team sono disattivati dopo essere stati associati a una regola di routing, le richieste continuano a essere indirizzate a tali utenti. È necessario prendere periodicamente un inventario di tutte le regole di ciclo e sostituire le assegnazioni disattivate con quelle attive.

   Quando si indirizza un problema a un progetto, gli utenti con autorizzazioni sul problema ricevono le autorizzazioni impostate per quel progetto. Per informazioni sull&#39;impostazione delle autorizzazioni sui progetti, vedi [Condivisione di un progetto in Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

   ![](assets/new-routing-rule-box-nwe-350x419.png)

1. Fai clic su **Salva**.

   Questo processo definisce solo la regola di routing. Per assicurarsi che il problema venga instradato quando viene inviato alla coda delle richieste, è necessario selezionare la regola di routing nella **Dettagli coda** scheda sotto **Percorso predefinito**.

   Per informazioni sull&#39;aggiunta di un percorso predefinito a una coda di richiesta, consulta [Creare una coda di richiesta](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

   Se si desidera associare più regole di instradamento alla coda di richiesta, è necessario creare più argomenti della coda e associarli a una regola di instradamento separata. Per ulteriori informazioni sulla creazione di un argomento della coda, consulta [Crea argomenti coda](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).
