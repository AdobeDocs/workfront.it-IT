---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Annullare l’assegnazione del lavoro nel servizio di bilanciamento del carico di lavoro
description: È possibile annullare l’assegnazione degli utenti dagli elementi di lavoro nell’area Lavoro assegnato di Adobe Workfront Workload Balancer o riassegnarli ad altri utenti, ruoli o team.
author: Alina
feature: Resource Management
exl-id: e4293d4a-afb8-48ef-8a8e-6fad2ef82a25
source-git-commit: 57ca3b58f3ef39eaea82acf609135b1e5ae8e631
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 2%

---

# Annullare l’assegnazione del lavoro nel servizio di bilanciamento del carico di lavoro

È possibile annullare l’assegnazione degli utenti dagli elementi di lavoro nell’area Lavoro assegnato di Adobe Workfront Workload Balancer o riassegnarli ad altri utenti, ruoli o team.

È possibile annullare l’assegnazione degli utenti dagli elementi di lavoro manualmente, trascinandoli o in blocco. Questo articolo descrive come annullare manualmente l’assegnazione degli utenti.

Per informazioni sull’annullamento dell’assegnazione degli utenti tramite trascinamento, consulta [Assegnare il lavoro nel bilanciamento del carico di lavoro trascinandolo e rilasciandolo](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-by-drag-and-drop.md)

Per informazioni sull’annullamento dell’assegnazione degli utenti in blocco, consulta [Assegnare il lavoro in blocco utilizzando il bilanciamento del carico di lavoro](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

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
   <td> <p>Pianificare quando si utilizza il servizio di bilanciamento del carico di lavoro nell'area Origine</p>
   <p>Lavoro, quando si utilizza il bilanciamento del carico di lavoro di un team o di un progetto</p>

</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica l’accesso ai seguenti elementi:</p> 
    <ul> 
     <li> <p>Gestione risorse</p> </li> 
     <li> <p>Progetti</p> </li> 
     <li> <p>Attività</p> </li> 
     <li> <p>Problemi</p> </li> 
    </ul> <p>Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Autorizzazioni di Contribute o superiori ai progetti, alle attività e ai problemi che includono l'opzione Assegna assegnazioni</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

 

## Annullare l&#39;assegnazione di elementi di lavoro nel servizio di bilanciamento del carico di lavoro

È possibile annullare l’assegnazione degli elementi dagli utenti e spostarli nell’area di lavoro non assegnata o riassegnarli ad altri utenti.

Per annullare l&#39;assegnazione di elementi di lavoro da parte degli utenti:

1. Nel servizio di bilanciamento del carico di lavoro, passa a **Lavoro assegnato** e espandere un utente.
1. Esegui una delle operazioni seguenti:

   * Individuare l&#39;elemento da annullare nell&#39;area di un utente, fare clic su di esso e trascinarlo nell&#39;area Non assegnata o nell&#39;area di un altro utente.
   * Fai clic sul pulsante **Altro** icona ![](assets/more-icon-task-list.png) a destra del nome di un elemento di lavoro, fare clic su **Assegna a**, quindi rimuovere il nome delle entità assegnate all&#39;elemento di lavoro o immettere un altro nome e fare clic su **Salva**.

      ![](assets/assign-this-to-link-from-task-wb-nwe-350x104.png)
   L&#39;elemento viene visualizzato nell&#39;area di lavoro non assegnata se corrisponde ai criteri di filtro per quell&#39;area e non viene assegnato ad altri utenti, oppure viene visualizzato nell&#39;area utente se è assegnato a un altro utente.

   Per informazioni sul filtro delle informazioni nel servizio di bilanciamento del carico di lavoro, consulta [Filtrare le informazioni nel servizio di bilanciamento del carico di lavoro](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).
