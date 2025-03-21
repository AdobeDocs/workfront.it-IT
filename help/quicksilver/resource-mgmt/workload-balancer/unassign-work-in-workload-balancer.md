---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Annullare l’assegnazione del lavoro nel Bilanciatore dei carichi di lavoro
description: È possibile annullare l’assegnazione degli utenti agli elementi di lavoro nell’area Lavoro assegnato del Bilanciatore dei carichi di lavoro di Adobe Workfront o riassegnarli ad altri utenti, ruoli o team.
author: Lisa
feature: Resource Management
exl-id: e4293d4a-afb8-48ef-8a8e-6fad2ef82a25
source-git-commit: 23c6d9335b0adcafc4e2ecdd8ef2d0ab09709fa8
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 2%

---

# Revoca assegnazione lavoro nel Bilanciatore dei carichi di lavoro

È possibile annullare l’assegnazione degli utenti agli elementi di lavoro nell’area Lavoro assegnato del Bilanciatore dei carichi di lavoro di Adobe Workfront o riassegnarli ad altri utenti, ruoli o team.

È possibile annullare l’assegnazione degli utenti agli elementi di lavoro manualmente, trascinandoli o in blocco. Questo articolo descrive come annullare l’assegnazione manuale degli utenti.

Per informazioni sulla rimozione dell&#39;assegnazione degli utenti mediante trascinamento, vedere [Assegnare il lavoro nel Bilanciatore dei carichi di lavoro mediante trascinamento](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-by-drag-and-drop.md)

Per informazioni sulla rimozione in blocco dell&#39;assegnazione di utenti, vedere [Assegnare il lavoro in blocco utilizzando il Bilanciatore dei carichi di lavoro](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td><p>Nuovo: Standard</p>
       <p>oppure</p>
       <p>Corrente: piano, quando si utilizza il Bilanciatore dei carichi di lavoro nell'area Risorse;</br>
       Utilizzare il Bilanciatore dei carichi di lavoro di un team o di un progetto</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica accesso a:</p> 
    <ul> 
     <li>Gestione risorse</li> 
     <li>Progetti</li> 
     <li>Attività</li> 
     <li>Problemi</li> 
    </ul></td>
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td>Autorizzazioni di Contribute o superiori per i progetti, le attività e i problemi che includono Assegnazioni</td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Annullare l’assegnazione degli elementi di lavoro nel Bilanciatore dei carichi di lavoro

È possibile annullare l&#39;assegnazione degli elementi agli utenti e spostarli nell&#39;area Lavoro non assegnato oppure riassegnarli ad altri utenti.

Per annullare l&#39;assegnazione degli elementi di lavoro agli utenti:

1. Nel Bilanciatore dei carichi di lavoro, vai all&#39;area **Lavoro assegnato** ed espandi un utente.
1. Esegui una delle operazioni seguenti:

   * Individuare l&#39;elemento di cui si desidera annullare l&#39;assegnazione nell&#39;area di un utente, fare clic su di esso e trascinarlo nell&#39;area Non assegnato o nell&#39;area di un altro utente.
   * Fai clic sull&#39;icona **Altro** ![Icona Altro](assets/more-icon-task-list.png) a destra del nome di un elemento di lavoro, fai clic su **Assegna a**, quindi rimuovi il nome delle entità assegnate all&#39;elemento di lavoro o immetti un altro nome e fai clic su **Salva**.

     ![Assegna a](assets/assign-this-to-link-from-task-wb-nwe-350x104.png)

   L’elemento viene visualizzato nell’area Lavoro non assegnato se corrisponde ai criteri di filtro per tale area e non è assegnato ad altri utenti, oppure nell’area utente se è assegnato a un altro utente.

   Per informazioni sul filtro delle informazioni nel Bilanciatore dei carichi di lavoro, vedere [Informazioni sul filtro nel Bilanciatore dei carichi di lavoro](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).
