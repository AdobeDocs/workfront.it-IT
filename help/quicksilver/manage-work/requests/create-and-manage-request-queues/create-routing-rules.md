---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Creare regole di instradamento
description: Le regole di instradamento controllano le operazioni di Adobe Workfront con i problemi quando vengono inviati a una coda di richieste.
author: Alina
feature: Work Management, Requests
topic: Collaboration
role: User, Admin
exl-id: 640f9054-f2f8-4594-9311-e93518f58453
source-git-commit: 8ec279ece400c10a37e67664b77b1e0df6639724
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 1%

---

# Creare regole di instradamento

<!-- Audited: 12/2023 -->

Le regole di instradamento controllano le operazioni di Adobe Workfront con i problemi quando vengono inviati a una coda di richieste. Per ulteriori informazioni sulla creazione di code di richieste, vedere [Creare una coda di richieste](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Le regole di instradamento inviano i problemi a utenti o ruoli specifici in grado di risolvere nel modo migliore il problema o la richiesta inviati. Le regole di instradamento sono solitamente associate agli argomenti della coda, utilizzati per controllare quale regola di instradamento verrà applicata al problema o alla richiesta.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>piano Adobe Workfront</p></td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Nuova licenza: Standard </p> 
   Oppure
   <p>Licenza corrente: Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica accesso ai progetti</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p> Gestire le autorizzazioni per il progetto</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creare una regola di instradamento

1. Passare al progetto in cui si desidera aggiungere regole di instradamento per le richieste.
1. Fai clic su **Regole di indirizzamento** nel pannello a sinistra. Potrebbe essere necessario fare clic su **Mostra altro**, quindi su **Regole di routing**.
1. Fare clic su **Nuova regola di routing** per aggiungere la nuova regola. Viene visualizzata la casella **Nuova regola di routing**.

   ![Casella Nuova regola di routing](assets/new-routing-rule-box.png)
1. Inserire le seguenti informazioni per la Regola di instradamento:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Nome</strong> </td> 
      <td>Nome della regola di routing. Se si dispone dell'accesso per visualizzare queste informazioni sul progetto, è possibile visualizzare la regola di instradamento.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Descrizione</strong> </td> 
      <td>Aggiungere una descrizione per la regola di routing.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Assegnatario predefinito*</strong> </td> 
      <td>Aggiungi un utente attivo o una mansione attiva a cui assegnare i nuovi problemi. In questo campo può essere presente un solo assegnatario predefinito. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Team predefinito*</strong> </td> 
      <td>Aggiungi un team attivo a cui assegnare il nuovo problema. In questo campo è disponibile un solo team predefinito.

   <p><b>NOTA</b></p>

   Dopo l’invio del problema, puoi modificarne le assegnazioni e assegnare altri utenti, ruoli o team. Per informazioni, vedere <a href="../../../manage-work/issues/manage-issues/assign-issues.md">Assegnare problemi</a>.

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Instrada al progetto</strong> </td> 
      <td>Questo è il progetto in cui viene aggiunto il problema.</td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >*Se un utente, una mansione o un team viene disattivato dopo essere stato associato a una regola di instradamento, le richieste continuano a essere instradate a loro. È necessario eseguire periodicamente un inventario di tutte le regole di instradamento e sostituire le assegnazioni disattivate con quelle attive.

   Quando si indirizza un problema a un progetto, gli utenti con autorizzazioni per il problema ricevono le autorizzazioni impostate per tale progetto. Per informazioni sull&#39;impostazione delle autorizzazioni per i progetti, vedere [Condividere un progetto in Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

1. Fai clic su **Salva**.

   Questo processo definisce solo la Regola di instradamento. Per assicurarsi che il problema venga instradato quando viene inviato alla coda richieste, è necessario selezionare la regola di instradamento nella scheda **Dettagli coda** in **Percorso predefinito**.

   Per informazioni sull&#39;aggiunta di una route predefinita a una coda richieste, vedere [Creare una coda richieste](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

   Se si desidera associare più regole di instradamento alla coda di richieste, è necessario creare più argomenti della coda e associarli a una regola di instradamento separata. Per ulteriori informazioni sulla creazione di un argomento della coda, vedere [Creare argomenti della coda](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).
