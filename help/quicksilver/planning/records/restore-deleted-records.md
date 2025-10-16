---
title: Ripristina record eliminati
description: È possibile recuperare i record eliminati dall'area Eliminati di recente in Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 8b6df633-eb05-4d3e-bfe6-76cedabdb76d
source-git-commit: 8546311acf722c0f4d47d4663b02ff701416894a
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

# Ripristina record eliminati

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span> -->

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
<ul> 
<li><p>Qualsiasi pacchetto Workfront e Planning</p></li>
Oppure
<li><p>Qualsiasi flusso di lavoro e qualsiasi pacchetto di Planning</p></li></ul>
<p>Per ulteriori informazioni su ciò che è incluso in ogni pacchetto Workfront Planning, contattare il rappresentante del proprio account Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Licenza Adobe Workfront</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorizzazioni oggetto</p></td> 
   <td>   <p>Contribuire o concedere autorizzazioni superiori a un’area di lavoro e a un tipo di record  </p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p> </td> 
  </tr>   
</tbody> 
</table>

Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

<!--Old:
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
</table> -->

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

## Ripristina record eliminati

1. Passare alla pagina del tipo di record in cui sono stati eliminati i record.
1. Fai clic sull&#39;icona **Annulla** ![Icona Annulla](assets/undo-icon.png) nell&#39;angolo superiore destro di qualsiasi visualizzazione pagina di tipo record, quindi fai clic su **Eliminato di recente**.

   Viene visualizzata la casella **Eliminato di recente**.

   ![Casella eliminata di recente](assets/recently-deleted-box.png)

1. Seleziona i record da eliminare, quindi fai clic su **Ripristina** > **Ripristina**. È possibile selezionare più record.

   Se il ripristino è stato eseguito correttamente, nella parte inferiore della schermata viene visualizzata una notifica di operazione riuscita.
1. Passare alla vista tabella ed esaminare i record ripristinati.
