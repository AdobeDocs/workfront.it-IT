---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Assegnare il lavoro manualmente utilizzando il Bilanciatore dei carichi di lavoro
description: È possibile assegnare manualmente gli elementi di lavoro agli utenti utilizzando il Bilanciatore dei carichi di lavoro di Adobe Workfront.
author: Lisa
feature: Resource Management
role: User
exl-id: 445cb250-53a4-488b-911d-3afca3a02c23
source-git-commit: e1580f7b9065fce7bb31ab0c7edb00fd2856e1df
workflow-type: tm+mt
source-wordcount: '747'
ht-degree: 1%

---

# Assegnare il lavoro manualmente utilizzando il Bilanciatore dei carichi di lavoro

È possibile assegnare manualmente gli elementi di lavoro agli utenti utilizzando il Bilanciatore dei carichi di lavoro di Adobe Workfront.

Per informazioni generali sull&#39;assegnazione del lavoro agli utenti che utilizzano il Bilanciatore dei carichi di lavoro, vedere [Panoramica sull&#39;assegnazione del lavoro nel Bilanciatore dei carichi di lavoro](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacchetto Adobe Workfront</td> 
   <td><p>Qualsiasi</p></td>
  </tr>
  <tr> 
   <td>Licenza Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Pianificare, quando si utilizza il Bilanciatore dei carichi di lavoro nell'area Risorse; lavorare, quando si utilizza il Bilanciatore dei carichi di lavoro di un team o progetto</p></td>
  </tr>
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td> <p>Modifica accesso a:</p> 
    <ul> 
     <li>Gestione risorse</li> 
     <li>Progetti</li> 
     <li>Attività</li> 
     <li>Problemi</li> 
    </ul>
   </td> 
  </tr> 
  <tr> 
   <td>Autorizzazioni oggetto</td> 
   <td>Autorizzazioni di Contribute o superiori per i progetti, le attività e i problemi che includono Assegnazioni</td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Assegnazione manuale del lavoro nel Bilanciatore dei carichi di lavoro

È possibile assegnare elementi di lavoro non ancora assegnati a un utente o riassegnare elementi assegnati a utenti nel Bilanciatore dei carichi di lavoro.

1. Andare al Bilanciatore dei carichi di lavoro nel punto in cui si desidera assegnare il lavoro.

   È possibile assegnare il lavoro agli utenti utilizzando il Bilanciatore dei carichi di lavoro nell&#39;area Risorse, a livello di progetto o di team. Per ulteriori informazioni sulla posizione del Bilanciatore dei carichi di lavoro in Workfront, vedere [Individuare il Bilanciatore dei carichi di lavoro](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

1. (Facoltativo) Vai all&#39;area **Lavoro non assegnato** e applica un filtro per visualizzare attività, problemi o assegnazioni di ruoli.

   Oppure

   Passare all&#39;area **Lavoro assegnato** ed espandere il nome di un utente per visualizzare gli elementi di lavoro assegnati, se si desidera riassegnare i relativi elementi.

   >[!NOTE]
   >
   >Le assegnazioni di ruolo vengono visualizzate in elementi di lavoro nell&#39;area Lavoro non assegnato quando l&#39;impostazione Mostra assegnazioni di ruolo è abilitata. Per ulteriori informazioni, vedere [Personalizzare la visualizzazione](/help/quicksilver/resource-mgmt/workload-balancer/navigate-the-workload-balancer.md#customize-the-view) in [Navigare nel Bilanciatore dei carichi di lavoro](/help/quicksilver/resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

1. Fai clic sul **Altro menu** ![Altro menu](assets/qs-more-menu.png) a sinistra del nome di un elemento di lavoro o dell&#39;assegnazione di un ruolo, quindi fai clic su **Assegna a**.

   ![Assegna a](assets/assign-this-to-link-from-task-wb-nwe-350x104.png)

   >[!TIP]
   >
   >Per assegnare attività o problemi, è inoltre possibile utilizzare le seguenti scelte rapide:
   >
   >* In Windows: CTRL+clic sulla barra delle attività o dei problemi.
   >* In Mac: CMD+fai clic sulla barra delle attività o dei problemi.

1. Esegui una delle operazioni seguenti:

   * Inizia a digitare il nome di un utente, una mansione o un team che desideri assegnare all&#39;elemento nel campo **Cerca persone, mansione o team**, selezionalo quando viene visualizzato nell&#39;elenco, quindi fai clic su **Salva**.

   >[!TIP]
   >
   >Quando aggiungi un utente, osserva l’avatar, il ruolo principale dell’utente e il suo indirizzo e-mail per distinguere gli utenti con nomi identici.
   >
   >Gli utenti devono essere associati ad almeno una mansione per visualizzarla quando vengono aggiunti.
   >
   > Per consentire agli utenti di visualizzare le e-mail degli utenti, nel proprio livello di accesso deve essere abilitata l’impostazione Visualizza informazioni di contatto. Per informazioni, vedere [Concedere l&#39;accesso agli utenti](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).


   ![Assegnazioni avanzate](assets/assignments-box-with-advanced-assignments-delegations-wb.png)

   >[!TIP]
   >
   > Se l’amministratore di Workfront o di gruppo ha abilitato le deleghe nell’ambiente, utilizza la scheda Assegnazioni per assegnare gli utenti all’attività o al problema. Utilizzare la scheda Deleghe per visualizzare gli utenti delegati all&#39;elemento di lavoro. Per informazioni sulla delega del lavoro, vedere [Delegare attività e problemi](../../manage-work/delegate-work/how-to-delegate-work.md).


   In questo modo l&#39;elemento di lavoro viene assegnato o riassegnato agli assegnatari specificati.

   Se si assegna un elemento solo a un team o a una mansione, l&#39;elemento viene visualizzato solo nell&#39;area Lavoro non assegnato. Per visualizzarli nell&#39;area Lavoro assegnato del Bilanciatore dei carichi di lavoro, è necessario assegnare gli elementi di lavoro agli utenti.

   >[!TIP]
   >
   >Puoi assegnare più utenti, mansioni o team. Puoi assegnare solo utenti attivi, mansioni e team.
   >
   >
   >Se un utente, una mansione o un team è stato assegnato prima della disattivazione, rimane assegnato all&#39;elemento di lavoro. In questo caso, consigliamo quanto segue:
   >
   >   
   >   
   >   * Riassegnare l&#39;elemento di lavoro alle risorse attive.
   >   * Associare gli utenti di un team disattivato a un team attivo e riassegnare l&#39;elemento di lavoro al team attivo.
   >   
   >

   * Fai clic su **Avanzate** per accedere alle assegnazioni avanzate.

     Per ulteriori informazioni sull&#39;esecuzione di assegnazioni avanzate, vedere [Creare assegnazioni avanzate](../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

1. (Facoltativo) Fai clic sull&#39;icona **Mostra allocazioni** ![Mostra allocazioni](assets/show-allocations-icon-small.png), quindi fai clic sul **Altro menu** ![Altro menu](assets/qs-more-menu.png) > **Modifica allocazioni**.

   Oppure

   Fare doppio clic su un&#39;allocazione giornaliera o settimanale per modificare la quantità di tempo assegnata all&#39;elemento di lavoro.

   Per informazioni sulla modifica delle allocazioni utente nel Bilanciatore dei carichi di lavoro, vedere la sezione &quot;Modifica allocazioni utente&quot; nell&#39;articolo [Gestione delle allocazioni utente nel Bilanciatore dei carichi di lavoro](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

   Per informazioni sulla rimozione delle assegnazioni da un elemento di lavoro tramite il Bilanciatore dei carichi di lavoro, vedere [Annullamento dell&#39;assegnazione del lavoro nel Bilanciatore dei carichi di lavoro](../../resource-mgmt/workload-balancer/unassign-work-in-workload-balancer.md).

    
