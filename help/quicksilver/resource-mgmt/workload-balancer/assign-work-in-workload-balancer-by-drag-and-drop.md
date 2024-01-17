---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Assegnare il lavoro nel Bilanciatore dei carichi di lavoro trascinandolo
description: È possibile assegnare gli elementi di lavoro utilizzando il Bilanciatore dei carichi di lavoro di Adobe Workfront trascinandoli per gli utenti corretti.
author: Lisa
feature: Resource Management
exl-id: caffcde8-3953-44a4-b945-76f2de84f4c6
source-git-commit: 2c4fe48ef969741ba792e37c28adba86ffdcba9a
workflow-type: tm+mt
source-wordcount: '901'
ht-degree: 0%

---

# Assegnare il lavoro nel Bilanciatore dei carichi di lavoro trascinandolo

<!--remove production and preview preferences at release-->

È possibile assegnare gli elementi di lavoro utilizzando il Bilanciatore dei carichi di lavoro di Adobe Workfront trascinandoli per gli utenti corretti.

Per informazioni generali sull’assegnazione di lavoro agli utenti tramite il Bilanciatore dei carichi di lavoro, consulta [Panoramica sull’assegnazione del lavoro nel Bilanciatore dei carichi di lavoro](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Pianificare, per assegnare il lavoro nel Bilanciatore dei carichi di lavoro nell'area Risorse</p>
   <p>Lavoro, per assegnare il lavoro nel Bilanciatore dei carichi di lavoro di un team o di un progetto</p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Livello di accesso*</td> 
   <td> <p>Modifica accesso a:</p> 
    <ul> 
     <li> <p>Gestione risorse</p> </li> 
     <li> <p>Progetti</p> </li> 
     <li> <p>Attività</p> </li> 
     <li> <p>Problemi</p> </li> 
    </ul> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Autorizzazioni di Contribute o superiori per i progetti, le attività e i problemi che includono Assegnazioni</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

## Assegnare un elemento trascinandolo

È possibile assegnare un elemento dall&#39;area Lavoro non assegnato a un utente oppure riassegnare un elemento già assegnato a un altro utente nell&#39;area Lavoro assegnato.

1. Andare al Bilanciatore dei carichi di lavoro nel punto in cui si desidera assegnare il lavoro.

   È possibile assegnare il lavoro agli utenti utilizzando il Bilanciatore dei carichi di lavoro nell&#39;area Risorse, a livello di progetto o di team. Per ulteriori informazioni sulla posizione del Bilanciatore dei carichi di lavoro in Workfront, consulta [Individuare il Bilanciatore dei carichi di lavoro](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

1. (Facoltativo) Vai al **Lavoro non assegnato** e applica un filtro per visualizzare attività e problemi non assegnati agli utenti

   Oppure

   Vai a **Lavoro assegnato** ed espandere il nome di un utente per visualizzare gli elementi di lavoro assegnati, se si desidera riassegnare i relativi elementi.

1. (Condizionale) Nel Bilanciatore dei carichi di lavoro di un progetto, fai clic su **Mostra tutti gli utenti** icona ![](assets/show-all-users-icon-project-workload-balancer.png) per visualizzare tutti gli utenti di Workfront.

   In questo modo vengono visualizzati tutti gli utenti a cui hai accesso.

   Gli utenti che fanno anche parte del team del progetto e sono già assegnati agli elementi del progetto hanno l’icona del progetto a destra del loro nome nell’area Lavoro assegnato.

   ![](assets/user-on-the-project-indicator-highlighted-project-workload-balancer.png)


   >[!TIP]
   >
   >* L’opzione Mostra tutti gli utenti è disponibile solo nel Bilanciatore dei carichi di lavoro di un progetto.
   >* Utilizza i filtri per visualizzare solo gli utenti che ti interessano. Ad esempio, utilizza un filtro per visualizzare solo gli utenti dei tuoi team o gruppi.



1. Fare clic sulla barra di un elemento di lavoro che indica la sequenza temporale pianificata o prevista e trascinarla sul nome di un utente nella **Assegnato** area.

   L’utente su cui passi il cursore del mouse per rilasciare l’elemento di lavoro viene evidenziato.

   >[!TIP]
   >
   >Le ore pianificate per l’utente che stai passando il cursore vengono aggiornate in tempo reale con il numero di ore pianificate giornaliere dall’elemento di lavoro, per indicare quale potrebbe essere l’impatto dell’aggiunta di un nuovo elemento sulla loro allocazione complessiva.

   ![](assets/drag-drop-item-from-unassigned-to-assigned-wb-nwe-350x152.png)

1. Quando si è pronti, rilasciare l&#39;elemento di lavoro selezionato nella stessa riga del nome dell&#39;utente nell&#39;area assegnata. L&#39;articolo viene assegnato e le ore pianificate allocate vengono aggiornate per l&#39;utente con le nuove ore dell&#39;elemento di lavoro.

   Se l&#39;elemento è stato assegnato a una mansione che l&#39;utente non può svolgere, l&#39;elemento viene visualizzato sotto il nome dell&#39;utente nell&#39;area Lavoro assegnato e rimane anche nell&#39;area Lavoro non assegnato per indicare che la mansione associata non è stata ancora sostituita da un utente.

   >[!TIP]
   >
   >* Se hai attivato Raggruppa per progetto nell’area Impostazioni, l’attività assegnata viene visualizzata sotto il progetto corrispondente. Se l&#39;impostazione è disabilitata, l&#39;attività assegnata viene visualizzata nell&#39;area utente.
   >
   >
   >     L’elemento viene visualizzato in base ai criteri del Bilanciatore dei carichi di lavoro per l’ordinamento degli elementi di lavoro. Per ulteriori informazioni, consulta [Navigare nel Bilanciatore dei carichi di lavoro](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).
   >
   >
   >* Se hai attivato Mostra tutti gli utenti nel Bilanciatore dei carichi di lavoro di un progetto e hai assegnato gli elementi a utenti che non erano stati precedentemente assegnati a elementi del progetto, gli utenti vengono aggiunti al Team del progetto. Per ulteriori informazioni, consulta [Gestisci team di progetto](../../manage-work/projects/planning-a-project/manage-project-team.md).


1. (Facoltativo) Fai clic sulla barra di un elemento di lavoro sotto il nome di un utente nell’area Lavoro assegnato, trascinala e rilasciala sull’area Lavoro non assegnato per annullarne l’assegnazione. L’elemento non è stato assegnato dall’utente, ma potrebbe ancora essere assegnato a una mansione nel qual caso viene visualizzato nell’area Lavoro non assegnato. Se l’elemento è assegnato a un altro utente, rimane nell’area Lavoro assegnato sotto il nome dell’utente ancora assegnato.
1. (Facoltativo) Fai clic su **Mostra icona allocazioni** ![](assets/show-allocations-icon-small.png), quindi fare clic su **Menu Altro** ![](assets/qs-more-menu.png) > **Modifica allocazioni**.

   <!--
   (make sure these are still called this, and that the icon has not changed)
   -->
   Oppure

   Fare doppio clic su un&#39;allocazione giornaliera o settimanale per modificare la quantità di tempo assegnata all&#39;elemento di lavoro.

   Per informazioni sulla modifica delle allocazioni utente nel Bilanciatore dei carichi di lavoro, vedi la sezione &quot;Modifica allocazioni utente&quot; nell’articolo [Gestire le allocazioni utente nel Bilanciatore dei carichi di lavoro](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

   Per informazioni sulla rimozione delle assegnazioni da un elemento di lavoro tramite il Bilanciatore dei carichi di lavoro, vedere [Revoca assegnazione lavoro nel Bilanciatore dei carichi di lavoro](../../resource-mgmt/workload-balancer/unassign-work-in-workload-balancer.md).

