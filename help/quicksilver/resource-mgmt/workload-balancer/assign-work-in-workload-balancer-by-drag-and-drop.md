---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Assegnare il lavoro nel Bilanciatore dei carichi di lavoro trascinandolo e rilasciandolo
description: È possibile assegnare gli elementi di lavoro utilizzando il Bilanciatore dei carichi di lavoro di Adobe Workfront trascinandoli per gli utenti corretti.
author: Lisa
feature: Resource Management
exl-id: caffcde8-3953-44a4-b945-76f2de84f4c6
source-git-commit: 69ac06c36440d9fbbf0c8c9f3e019374da2e2f91
workflow-type: tm+mt
source-wordcount: '991'
ht-degree: 0%

---

# Assegnare il lavoro nel Bilanciatore dei carichi di lavoro trascinandolo

{{preview-fast-release-general}}

È possibile assegnare gli elementi di lavoro utilizzando il Bilanciatore dei carichi di lavoro di Adobe Workfront trascinandoli per gli utenti corretti.

Per informazioni generali sull&#39;assegnazione del lavoro agli utenti che utilizzano il Bilanciatore dei carichi di lavoro, vedere [Panoramica sull&#39;assegnazione del lavoro nel Bilanciatore dei carichi di lavoro](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

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
       <p>Corrente: piano, per assegnare il lavoro nel Bilanciatore dei carichi di lavoro nell'area Risorse;</br>
       Lavoro, per assegnare il lavoro nel Bilanciatore dei carichi di lavoro di un team o di un progetto</p></td>
  </tr>
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
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
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td>Autorizzazioni di Contribute o superiori per i progetti, le attività e i problemi che includono Assegnazioni</td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Assegnare un elemento trascinandolo

È possibile assegnare un elemento dall&#39;area Lavoro non assegnato a un utente oppure riassegnare un elemento già assegnato a un altro utente nell&#39;area Lavoro assegnato.

1. Andare al Bilanciatore dei carichi di lavoro nel punto in cui si desidera assegnare il lavoro.

   È possibile assegnare il lavoro agli utenti utilizzando il Bilanciatore dei carichi di lavoro nell&#39;area Risorse, a livello di progetto o di team. Per ulteriori informazioni sulla posizione del Bilanciatore dei carichi di lavoro in Workfront, vedere [Individuare il Bilanciatore dei carichi di lavoro](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

1. (Facoltativo) Vai all&#39;area **Lavoro non assegnato** e applica un filtro per visualizzare le attività, i problemi, <span class="preview">e le assegnazioni di ruolo</span> non assegnati agli utenti

   Oppure

   Passare all&#39;area **Lavoro assegnato** ed espandere il nome di un utente per visualizzare gli elementi di lavoro assegnati, se si desidera riassegnare i relativi elementi.

   >[!NOTE]
   >
   ><span class="preview">Le assegnazioni di ruolo vengono visualizzate in elementi di lavoro nell&#39;area Lavoro non assegnato quando l&#39;impostazione Mostra assegnazioni di ruolo è abilitata. Per ulteriori informazioni, vedere [Personalizzare la visualizzazione](/help/quicksilver/resource-mgmt/workload-balancer/navigate-the-workload-balancer.md#customize-the-view) in [Navigare nel Bilanciatore dei carichi di lavoro](/help/quicksilver/resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).</span>

1. (Condizionale) Nel Bilanciatore dei carichi di lavoro di un progetto, fai clic sull&#39;icona **Mostra tutti gli utenti** ![Mostra tutti gli utenti](assets/show-all-users-icon-project-workload-balancer.png) per visualizzare tutti gli utenti di Workfront.

   In questo modo vengono visualizzati tutti gli utenti a cui hai accesso.

   Gli utenti che fanno anche parte del team del progetto e sono già assegnati agli elementi del progetto hanno l’icona del progetto a destra del loro nome nell’area Lavoro assegnato.

   ![Utente nel progetto](assets/user-on-the-project-indicator-highlighted-project-workload-balancer.png)

   >[!TIP]
   >
   >* L’opzione Mostra tutti gli utenti è disponibile solo nel Bilanciatore dei carichi di lavoro di un progetto.
   >* Utilizza i filtri per visualizzare solo gli utenti che ti interessano. Ad esempio, utilizza un filtro per visualizzare solo gli utenti dei tuoi team o gruppi.

1. Fare clic sulla barra di un elemento di lavoro <span class="preview">o di un&#39;assegnazione di ruolo</span> che indica la sequenza temporale pianificata o prevista e trascinarla sul nome di un utente nell&#39;area **Assegnato**.

   L’utente su cui passi il cursore del mouse per rilasciare l’elemento di lavoro viene evidenziato.

   <span class="preview">Quando si trascinano e si rilasciano assegnazioni di ruolo, l&#39;utente viene evidenziato in arancione se il ruolo corrente non corrisponde all&#39;assegnazione di ruolo. È comunque possibile assegnare il lavoro all&#39;utente quando i ruoli non corrispondono.</span>

   >[!TIP]
   >
   >Le ore pianificate per l’utente che stai passando il cursore vengono aggiornate in tempo reale con il numero di ore pianificate giornaliere dall’elemento di lavoro, per indicare quale potrebbe essere l’impatto dell’aggiunta di un nuovo elemento sulla loro allocazione complessiva.

   <span class="preview">Immagine di esempio nell&#39;ambiente di anteprima:</span>
   ![Elimina elemento da assegnare a un utente](assets/wb-drag-drop-role-or-task-to-user.png)

   Immagine di esempio nell’ambiente di produzione:
   ![Elimina elemento da assegnare a un utente](assets/drag-drop-item-from-unassigned-to-assigned-wb-nwe-350x152.png)

1. Quando sei pronto, rilascia l&#39;elemento di lavoro selezionato <span class="preview">o l&#39;assegnazione di ruolo</span> nella stessa riga del nome dell&#39;utente nell&#39;area assegnata. L&#39;articolo viene assegnato e le ore pianificate allocate vengono aggiornate per l&#39;utente con le nuove ore dell&#39;elemento di lavoro.

   <span class="preview">Se l&#39;impostazione Mostra assegnazioni ruolo non è abilitata</span> e l&#39;elemento di lavoro è stato assegnato a una mansione che l&#39;utente non può svolgere, l&#39;elemento viene visualizzato sotto il nome dell&#39;utente nell&#39;area Lavoro assegnato. Inoltre, rimane nell’area Lavoro non assegnato per indicare che il ruolo lavorativo associato non è stato ancora sostituito da un utente.

   >[!TIP]
   >
   >* Se hai attivato Raggruppa per progetto nell’area Impostazioni, l’attività assegnata viene visualizzata sotto il progetto corrispondente. Se l&#39;impostazione è disabilitata, l&#39;attività assegnata viene visualizzata nell&#39;area utente.
   >
   >
   >     L’elemento viene visualizzato in base ai criteri del Bilanciatore dei carichi di lavoro per l’ordinamento degli elementi di lavoro. Per ulteriori informazioni, vedere [Navigare nel Bilanciatore dei carichi di lavoro](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).
   >
   >
   >* Se hai attivato Mostra tutti gli utenti nel Bilanciatore dei carichi di lavoro di un progetto e hai assegnato gli elementi a utenti che non erano stati precedentemente assegnati a elementi del progetto, gli utenti vengono aggiunti al Team del progetto. Per ulteriori informazioni, vedere [Gestione team di progetto](../../manage-work/projects/planning-a-project/manage-project-team.md).


1. (Facoltativo) Fai clic sulla barra di un elemento di lavoro sotto il nome di un utente nell’area Lavoro assegnato, trascinala e rilasciala sull’area Lavoro non assegnato per annullarne l’assegnazione. L’elemento non è stato assegnato dall’utente, ma potrebbe ancora essere assegnato a una mansione nel qual caso viene visualizzato nell’area Lavoro non assegnato. Se l’elemento è assegnato a un altro utente, rimane nell’area Lavoro assegnato sotto il nome dell’utente ancora assegnato.
1. (Facoltativo) Fai clic sull&#39;icona **Mostra allocazioni** ![Mostra allocazioni](assets/show-allocations-icon-small.png), quindi fai clic sul **Altro menu** ![Altro menu](assets/qs-more-menu.png) > **Modifica allocazioni**.

   <!--
   (make sure these are still called this, and that the icon has not changed)
   -->
   Oppure

   Fare doppio clic su un&#39;allocazione giornaliera o settimanale per modificare la quantità di tempo assegnata all&#39;elemento di lavoro.

   Per informazioni sulla modifica delle allocazioni utente nel Bilanciatore dei carichi di lavoro, vedere la sezione &quot;Modifica allocazioni utente&quot; nell&#39;articolo [Gestione delle allocazioni utente nel Bilanciatore dei carichi di lavoro](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

   Per informazioni sulla rimozione delle assegnazioni da un elemento di lavoro tramite il Bilanciatore dei carichi di lavoro, vedere [Annullamento dell&#39;assegnazione del lavoro nel Bilanciatore dei carichi di lavoro](../../resource-mgmt/workload-balancer/unassign-work-in-workload-balancer.md).

