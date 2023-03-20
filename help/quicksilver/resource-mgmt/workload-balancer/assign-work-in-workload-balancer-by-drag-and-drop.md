---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Assegnare il lavoro nel bilanciamento del carico di lavoro trascinandolo e rilasciandolo
description: È possibile assegnare gli elementi di lavoro utilizzando il servizio di bilanciamento del carico di lavoro di Adobe Workfront trascinando e rilasciando gli elementi di lavoro agli utenti corretti.
author: Alina
feature: Resource Management
exl-id: caffcde8-3953-44a4-b945-76f2de84f4c6
source-git-commit: bbd99435bb07d68bf9058bcd3e8c6ef5d9df75a9
workflow-type: tm+mt
source-wordcount: '901'
ht-degree: 1%

---

# Assegnare il lavoro nel bilanciamento del carico di lavoro trascinandolo e rilasciandolo

<!--remove production and preview preferences at release-->

È possibile assegnare gli elementi di lavoro utilizzando il servizio di bilanciamento del carico di lavoro di Adobe Workfront trascinando e rilasciando gli elementi di lavoro agli utenti corretti.

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
   <td> <p>Pianificare, per assegnare il lavoro nel servizio di bilanciamento del carico di lavoro nell'area di determinazione origine</p>
   <p>Lavoro, per assegnare il lavoro nel servizio di bilanciamento del carico di lavoro di un team o di un progetto</p>
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

## Assegnare un elemento trascinandolo e rilasciandolo

È possibile assegnare un elemento dall&#39;area Lavoro non assegnato a un utente oppure riassegnare un elemento già assegnato a un altro utente nell&#39;area Lavoro assegnato.

1. Passa al servizio di bilanciamento del carico di lavoro in cui desideri assegnare il lavoro.

   È possibile assegnare il lavoro agli utenti utilizzando il servizio di bilanciamento del carico di lavoro nell&#39;area Origine, nel progetto o a livello di team. Per ulteriori informazioni sulla posizione del servizio di bilanciamento del carico di lavoro in Workfront, vedi [Individua il servizio di bilanciamento del carico di lavoro](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

1. (Facoltativo) Vai a **Lavoro non assegnato** e applica un filtro per visualizzare le attività e i problemi non assegnati agli utenti

   Oppure

   Vai a **Lavoro assegnato** espandere il nome di un utente per visualizzare gli elementi di lavoro assegnati, se si desidera riassegnarne gli elementi.

1. (Condizionale) Nel servizio di bilanciamento del carico di lavoro di un progetto, fai clic sul pulsante **Mostra tutti gli utenti** icona ![](assets/show-all-users-icon-project-workload-balancer.png) per visualizzare tutti gli utenti di Workfront.

   Vengono visualizzati tutti gli utenti a cui hai accesso.

   Gli utenti che fanno parte anche del team di progetto e sono già assegnati agli elementi del progetto hanno l’icona del progetto a destra del loro nome nell’area Lavoro assegnato .

   ![](assets/user-on-the-project-indicator-highlighted-project-workload-balancer.png)


   >[!TIP]
   >
   >* L’opzione Mostra tutti gli utenti è disponibile solo nel servizio di bilanciamento del carico di lavoro di un progetto.
   >* Utilizza i filtri per visualizzare solo gli utenti che sono importanti per te. Ad esempio, utilizza un filtro per visualizzare solo gli utenti dei team o dei gruppi.




1. Fare clic sulla barra di un elemento di lavoro che indica la timeline pianificata o proiettata e trascinarla sul nome di un utente nel **Assegnato** area.

   Viene evidenziato l’utente a cui si passa il puntatore del mouse per rilasciare l’elemento di lavoro.

   >[!TIP]
   >
   >Le ore pianificate per l&#39;utente a cui si passa il mouse sopra l&#39;aggiornamento in tempo reale con il numero di ore pianificate giornaliere dall&#39;elemento di lavoro, per indicare quale potrebbe essere l&#39;impatto dell&#39;aggiunta di un nuovo elemento sulla loro allocazione complessiva.

   ![](assets/drag-drop-item-from-unassigned-to-assigned-wb-nwe-350x152.png)

1. Quando sei pronto, rilascia l’elemento di lavoro selezionato nella stessa riga del nome dell’utente nell’area Assegnata. L&#39;articolo viene assegnato e l&#39;orario pianificato allocato viene aggiornato per l&#39;utente con le nuove ore dall&#39;elemento di lavoro.

   Se l&#39;elemento è stato assegnato a un ruolo di lavoro che l&#39;utente non è in grado di svolgere, l&#39;elemento viene visualizzato sotto il nome dell&#39;utente nell&#39;area Lavoro assegnato e rimane nell&#39;area Lavoro non assegnato per indicare che il ruolo di lavoro associato non è stato ancora sostituito da un utente.

   >[!TIP]
   >
   >* Se nell’area Impostazioni è stato abilitato Raggruppa per progetto , l’attività assegnata viene visualizzata sotto il progetto corrispondente. Se l’impostazione è disabilitata, l’attività assegnata viene visualizzata nell’area utente.
      >
      >
      >     L’elemento viene visualizzato in base ai criteri del servizio di bilanciamento del carico di lavoro per l’ordinamento degli elementi di lavoro. Per ulteriori informazioni, consulta [Naviga nel bilanciamento del carico di lavoro](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).
   >
   >
   >* Se hai abilitato Mostra tutti gli utenti nel servizio di bilanciamento del carico di lavoro di un progetto e hai assegnato gli elementi agli utenti che non erano stati precedentemente assegnati agli elementi del progetto, gli utenti verranno aggiunti al team del progetto. Per ulteriori informazioni, consulta [Gestione del team di progetto](../../manage-work/projects/planning-a-project/manage-project-team.md).



1. (Facoltativo) Fare clic sulla barra di un elemento di lavoro sotto il nome di un utente nell&#39;area Lavoro assegnato e trascinarlo sull&#39;area Lavoro non assegnato per annullarne l&#39;assegnazione. L&#39;elemento viene rimosso dall&#39;utente, ma potrebbe essere comunque assegnato a un ruolo di lavoro nel qual caso viene visualizzato nell&#39;area Lavoro non assegnato. Se l&#39;elemento viene assegnato a un altro utente, rimane nell&#39;area Lavoro assegnato con il nome dell&#39;utente che viene ancora assegnato.
1. (Facoltativo) Fai clic sul pulsante **Icona Mostra allocazioni** ![](assets/show-allocations-icon-small.png), quindi fai clic su **Menu Altro** ![](assets/qs-more-menu.png) > **Modifica allocazioni**.

   <!--
   (make sure these are still called this, and that the icon has not changed)
   -->
   Oppure

   Fare doppio clic su un&#39;allocazione giornaliera o settimanale per modificare il tempo assegnato dall&#39;utente all&#39;elemento di lavoro.

   Per informazioni sulla modifica delle allocazioni degli utenti nel load Balancer, consulta la sezione &quot;Modificare le allocazioni degli utenti&quot; nell’articolo [Gestire le allocazioni di utenti nel load balancer](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

   Per informazioni sulla rimozione delle assegnazioni da un elemento di lavoro utilizzando il servizio di bilanciamento del carico di lavoro, vedere [Annullare l’assegnazione del lavoro nel servizio di bilanciamento del carico di lavoro](../../resource-mgmt/workload-balancer/unassign-work-in-workload-balancer.md).

