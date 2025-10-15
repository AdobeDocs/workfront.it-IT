---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Accesso necessario per gestire le risorse nel Bilanciatore dei carichi di lavoro
description: Senza l'accesso o le autorizzazioni corrette, potrebbe non essere possibile visualizzare o gestire le assegnazioni di lavoro nel Bilanciatore dei carichi di lavoro.
author: Lisa
feature: Resource Management
exl-id: b3da9a62-481e-4503-8f27-136d6513262e
source-git-commit: 78d73d0d7bd0ffc00ae1afed0adb324501e0c310
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 0%

---

# Accesso necessario per gestire le risorse nel Bilanciatore dei carichi di lavoro

{{preview-fast-release-general}}

Senza l&#39;accesso o le autorizzazioni corrette, potrebbe non essere possibile visualizzare o gestire le assegnazioni di lavoro nel Bilanciatore dei carichi di lavoro.

È necessario disporre dell’accesso per visualizzare gli utenti di cui desideri visualizzare o gestire il carico di lavoro nel Bilanciatore dei carichi di lavoro. Inoltre, devi disporre del livello di accesso corretto e delle autorizzazioni corrette per i progetti a cui è associato il lavoro.

## Piano Adobe Workfront necessario per utilizzare il Bilanciatore dei carichi di lavoro per diverse aree

La tabella seguente illustra la connessione tra il piano Workfront di cui dispone la società e la posizione nel sistema in cui è possibile utilizzare il Bilanciatore dei carichi di lavoro:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p><b>Piano Workfront (corrente)</b></p></td> 
   <td> <p><b>Aree in cui è possibile accedere al Bilanciatore dei carichi di lavoro</b></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Team o versione successiva </td> 
   <td>Bilanciatore dei carichi di lavoro per un team o un progetto</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Pro o superiore</td> 
   <td>Bilanciatore dei carichi di lavoro per più progetti, a livello di sistema</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p><b>Piano Workfront (nuovo)</b></p></td> 
   <td> <p><b>Aree in cui è possibile accedere al Bilanciatore dei carichi di lavoro</b></p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">Qualsiasi </td> 
   <td>Accedere al Bilanciatore dei carichi di lavoro ovunque in Workfront</td> 
  </tr> 
 </tbody> 
</table>

Per informazioni sui piani di Workfront, vedere [I nostri piani](https://business.adobe.com/it/products/workfront/pricing.html).

Per informazioni su dove è possibile individuare il Bilanciatore dei carichi di lavoro in Workfront, vedere [Individuare il Bilanciatore dei carichi di lavoro](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

## Accesso necessario per visualizzare il Bilanciatore dei carichi di lavoro

Per visualizzare il Bilanciatore dei carichi di lavoro è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td><p>Nuovo: Standard</p>
       <p>oppure</p>
       <p>Corrente: piano, per visualizzare il Bilanciatore dei carichi di lavoro nell'area Risorse;</br>
       Utilizzare, per visualizzare il Bilanciatore dei carichi di lavoro di un team o di un progetto</p></td>
  </tr>  
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Accesso di visualizzazione o superiore a Gestione risorse</p> <p>Per informazioni sul livello di accesso Gestione risorse, vedere l'articolo <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md" class="MCXref xref">Concedere l'accesso a Gestione risorse</a>.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>È necessario disporre delle autorizzazioni di visualizzazione per il progetto di cui si desidera visualizzare le assegnazioni. </p> <p>Per informazioni sulle autorizzazioni del progetto, vedere l'articolo <a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Condividere un progetto in Adobe Workfront</a>.</p></td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<span class="preview">Tutti gli utenti hanno accesso alla visualizzazione del Bilanciatore dei carichi di lavoro sui propri profili. Questo non è limitato dalla licenza o dal livello di accesso. Il Bilanciatore dei carichi di lavoro in un profilo utente è di sola lettura e non è possibile modificare assegnazioni e allocazioni.</span>

## Accesso necessario per gestire le assegnazioni nel Bilanciatore dei carichi di lavoro

Per gestire il Bilanciatore dei carichi di lavoro è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td><p>Nuovo: Standard</p>
       <p>oppure</p>
       <p>Corrente: piano, per gestire le assegnazioni nel Bilanciatore dei carichi di lavoro nell'area Risorse;</br>
       Utilizzare, per gestire le assegnazioni nel Bilanciatore dei carichi di lavoro di un team o di un progetto</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica accesso a Gestione risorse</p> 
     <p>Per informazioni sul livello di accesso Gestione risorse, vedere l'articolo <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md" class="MCXref xref">Concedere l'accesso a Gestione risorse</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p> Autorizzazioni di Contribute o di livello superiore per il progetto di cui si desidera gestire le assegnazioni, che includono le autorizzazioni per effettuare assegnazioni. </p> <p>Per informazioni sulle autorizzazioni del progetto, vedere l'articolo <a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Condividere un progetto in Adobe Workfront</a>.</p></td>
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<!--these notes were inside the table: for the Edit access to Res Management
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">View or higher access to Financial Data, if you want to view information by cost (NOTE: this is not possible yet!)</p>    
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the Financial Data access level, see the article<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Grant access to financial data</a>. (NOTE: this is not possible yet!)</p>
    -->
