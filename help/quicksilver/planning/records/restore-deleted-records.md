---
title: Ripristina record eliminati
description: È possibile recuperare i record eliminati dall'area Eliminati di recente in Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 8b6df633-eb05-4d3e-bfe6-76cedabdb76d
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/6F-GarlW1gY0gHEZIC-CgSiN75EMd2RcZZUGgyOgqxU
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 455
ht-degree: 3%

---

# Ripristinare i record eliminati


<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo i rilasci mensili in Produzione, le stesse funzioni sono disponibili nell’ambiente di Produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedere [Abilitare o disabilitare le versioni rapide per l&#39;organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

È possibile recuperare i record eliminati dall&#39;area Eliminati di recente in Adobe Workfront Planning.

Per informazioni sull&#39;eliminazione dei record, vedere [Elimina record](/help/quicksilver/planning/records/delete-records.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Pacchetto Adobe Workfront</p></td> 
   <td> 
<p>Qualsiasi pacchetto Workfront e Planning</p> <p>Qualsiasi flusso di lavoro e qualsiasi pacchetto di Planning</p>
<p>Per ulteriori informazioni su ciò che è incluso in ogni pacchetto Workfront Planning, contattare il rappresentante del proprio account Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Licenza di Adobe Workfront</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorizzazioni sugli oggetti</p></td> 
   <td>   <p>Autorizzazioni Contribute o superiori per un'area di lavoro, un tipo di record e <span class="preview">le autorizzazioni di gestione per un record</span> </p>    
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p> </td> 
  </tr>   
</tbody> 
</table>

Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

<!--
Old:
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard</p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Contribute or higher permissions to a workspace and record type</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
</tbody> 
</table>
-->

## Considerazioni sul recupero dei record eliminati

* È possibile ripristinare i record eliminati dall&#39;utente o da altri utenti.
* I record vengono memorizzati nel contenitore Eliminato di recente per 30 giorni. Dopo 30 giorni, i record vengono eliminati definitivamente da Workfront Planning.
* Se i record eliminati sono collegati ad altri record, i record collegati non vengono eliminati, ma vengono eliminate anche le informazioni del record eliminato. Il ripristino dei record eliminati ripristina le informazioni dai record connessi.
* È possibile ripristinare i record in blocco.
* Quando i record vengono eliminati, le seguenti informazioni vengono memorizzate nel contenitore Eliminato di recente:
   * **Nome**: queste sono le informazioni contenute nel campo Principale del record. Per ulteriori informazioni sui campi primari dei record, vedere [Panoramica sui campi primari](/help/quicksilver/planning/fields/primary-field-overview.md).
   * **Data di eliminazione**: l&#39;ora e la data in cui il record è stato eliminato.
   * **Ora in eliminata di recente**: ora dall&#39;eliminazione del record. I record eliminati più di 30 giorni prima della data corrente non vengono visualizzati nel contenitore Eliminati di recente.
   * **Eliminato da**: nome dell&#39;utente che ha eliminato il record.

## Ripristinare i record eliminati

1. Passare alla pagina del tipo di record in cui sono stati eliminati i record.
1. Fai clic sull&#39;icona **Annulla** ![Icona Annulla](assets/undo-icon.png) nell&#39;angolo superiore destro di qualsiasi visualizzazione pagina di tipo record, quindi fai clic su **Eliminato di recente**.

   Viene visualizzata la casella **Eliminato di recente**.

   ![Casella eliminata di recente](assets/recently-deleted-box.png)

1. Seleziona i record da eliminare, quindi fai clic su **Ripristina** > **Ripristina**. È possibile selezionare più record.

   Se il ripristino è stato eseguito correttamente, nella parte inferiore della schermata viene visualizzata una notifica di operazione riuscita.
1. Passare alla vista tabella ed esaminare i record ripristinati.
