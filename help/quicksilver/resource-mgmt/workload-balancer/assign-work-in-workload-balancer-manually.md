---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Assegnare il lavoro manualmente utilizzando il bilanciamento del carico di lavoro
description: Puoi assegnare manualmente gli elementi di lavoro agli utenti utilizzando il servizio di bilanciamento del carico di lavoro di Adobe Workfront.
author: Alina
feature: Resource Management
exl-id: 445cb250-53a4-488b-911d-3afca3a02c23
source-git-commit: 57ca3b58f3ef39eaea82acf609135b1e5ae8e631
workflow-type: tm+mt
source-wordcount: '730'
ht-degree: 2%

---

# Assegnare il lavoro manualmente utilizzando il bilanciamento del carico di lavoro

Puoi assegnare manualmente gli elementi di lavoro agli utenti utilizzando il servizio di bilanciamento del carico di lavoro di Adobe Workfront.

Per informazioni generali sull&#39;assegnazione del lavoro agli utenti che utilizzano il bilanciamento del carico di lavoro, vedi [Panoramica dell’assegnazione del lavoro nel servizio di bilanciamento del carico di lavoro](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

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
   <td role="rowheader">Livello di accesso*</td> 
   <td> <p>Modifica l’accesso ai seguenti elementi:</p> 
    <ul> 
     <li> <p>Gestione risorse</p> </li> 
     <li> <p>Progetti</p> </li> 
     <li> <p>Attività</p> </li> 
     <li> <p>Problemi</p> </li> 
    </ul> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Autorizzazioni di Contribute o superiori ai progetti, alle attività e ai problemi che includono l'opzione Assegna assegnazioni</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Assegnare manualmente il lavoro nel servizio di bilanciamento del carico di lavoro

È possibile assegnare elementi di lavoro non ancora assegnati a un utente o riassegnare gli elementi assegnati agli utenti nel servizio di bilanciamento del carico di lavoro.

1. Passa al servizio di bilanciamento del carico di lavoro in cui desideri assegnare il lavoro.

   È possibile assegnare il lavoro agli utenti utilizzando il servizio di bilanciamento del carico di lavoro nell&#39;area Origine, nel progetto o a livello di team. Per ulteriori informazioni sulla posizione del servizio di bilanciamento del carico di lavoro in Workfront, vedi [Individua il servizio di bilanciamento del carico di lavoro](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

1. (Facoltativo) Vai a **Lavoro non assegnato** area e applicazione di un filtro per visualizzare attività o problemi

   Oppure

   Vai a **Lavoro assegnato** espandere il nome di un utente per visualizzare gli elementi di lavoro assegnati, se si desidera riassegnarne gli elementi.

1. Fai clic sul pulsante **Menu Altro** ![](assets/qs-more-menu.png) a sinistra del nome di un elemento di lavoro, quindi fare clic su **Assegna a**.

   ![](assets/assign-this-to-link-from-task-wb-nwe-350x104.png)

   >[!TIP]
   >
   >È inoltre possibile utilizzare le seguenti scelte rapide per assegnare attività o problemi:
   >
   >* In Windows: CTRL+clic sull&#39;attività o sulla barra dei problemi.
   >* In Mac: CMD+clic sull&#39;attività o sulla barra dei problemi.


1. Esegui una delle operazioni seguenti:

   * Iniziare a digitare il nome di un utente, di un ruolo o di un team che si desidera assegnare all&#39;elemento nel **Cercare persone, ruoli o team** selezionare il campo quando viene visualizzato nell&#39;elenco, quindi fare clic su **Salva**.
   >[!TIP]
   >
   >Quando aggiungi un utente, osserva l’avatar, il ruolo principale dell’utente e il relativo indirizzo e-mail per distinguere tra utenti con nomi identici. Gli utenti devono essere associati ad almeno un ruolo di lavoro per visualizzarlo durante l&#39;aggiunta.

   ![](assets/assignments-box-with-advanced-assignments-delegations-wb.png)

   >[!TIP]
   >
   > Se nell’ambiente l’amministratore di Workfront o di gruppo ha abilitato le deleghe, utilizza la scheda Assegnazioni per assegnare gli utenti all’attività o al problema. Utilizza la scheda Delegazioni per visualizzare gli utenti delegati all’elemento di lavoro. Per informazioni sulla delega del lavoro, vedi [Gestione dell&#39;attività e della delega dei problemi](../../manage-work/delegate-work/how-to-delegate-work.md).


   Questo assegna o riassegna l&#39;elemento di lavoro alle assegne specificate.

   Se si assegna un elemento solo a un team o a un ruolo di lavoro, l&#39;elemento viene visualizzato solo nell&#39;area Lavoro non assegnato. È necessario assegnare gli elementi di lavoro agli utenti per visualizzarli nell&#39;area Lavoro assegnato del servizio di bilanciamento del carico di lavoro.

   >[!TIP]
   >
   >È possibile assegnare più utenti, ruoli o team. È possibile assegnare solo utenti attivi, ruoli e team.
   >
   >
   >Se un utente, un ruolo di lavoro o un team è stato assegnato prima della disattivazione, rimangono assegnati all&#39;elemento di lavoro. In questo caso, si consiglia quanto segue:
   >
   >   
   >   
   >   * Riassegna l&#39;elemento di lavoro alle risorse attive.
   >   * Associare gli utenti di un team disattivato a un team attivo e riassegnare l&#39;elemento di lavoro al team attivo.


   * Fai clic su **Avanzate** per accedere ad Assegnazioni avanzate.

      Per ulteriori informazioni sull&#39;assegnazione avanzata, consulta [Creazione di assegnazioni avanzate](../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).


1. (Facoltativo) Fai clic sul pulsante **Icona Mostra allocazioni** ![](assets/show-allocations-icon-small.png), quindi fai clic su **Menu Altro** ![](assets/qs-more-menu.png) > **Modifica allocazioni**.

   Oppure

   Fare doppio clic su un&#39;allocazione giornaliera o settimanale per modificare il tempo assegnato dall&#39;utente all&#39;elemento di lavoro.

   Per informazioni sulla modifica delle allocazioni degli utenti nel load Balancer, consulta la sezione &quot;Modificare le allocazioni degli utenti&quot; nell’articolo [Gestire le allocazioni di utenti nel load balancer](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

   Per informazioni sulla rimozione delle assegnazioni da un elemento di lavoro utilizzando il servizio di bilanciamento del carico di lavoro, vedere [Annullare l’assegnazione del lavoro nel servizio di bilanciamento del carico di lavoro](../../resource-mgmt/workload-balancer/unassign-work-in-workload-balancer.md).

    
