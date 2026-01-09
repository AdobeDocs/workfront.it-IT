---
title: Configurare l’area Impostazioni di un tipo di record
description: Oltre a modificare un tipo di record nella casella Modifica tipo di record, è possibile modificare anche i tipi di record nella pagina Impostazioni.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 40891b0e960e38c4fca55eec428a4e3a6397b316
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 3%

---


# Configurare l’area Impostazioni di un tipo di record

<span class="preview">Le informazioni contenute in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo i rilasci mensili in Produzione, le stesse funzioni sono disponibili nell’ambiente di Produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedere [Abilitare o disabilitare le versioni rapide per l&#39;organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

È possibile configurare ulteriori impostazioni per un tipo di record dopo averle salvate in Adobe Workfront Planning.

A seconda delle funzionalità che si desidera definire per un tipo di record, è possibile configurare ulteriori impostazioni eseguendo una delle operazioni seguenti:

<!--the above will need to be reworded when we add automations and manage request forms to this area-->

* Modificarli

  Per informazioni, vedere [Modifica tipi di record](/help/quicksilver/planning/architecture/edit-record-types.md).

* Configurazione della pagina Impostazioni di un tipo di record.

  Questo articolo descrive come modificare un tipo di record configurandone la pagina Impostazioni.

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
<p>Qualsiasi pacchetto Workfront e Planning</p>
<p>Qualsiasi pacchetto di Workflow e Planning</p>

<p><b>NOTA</b></p>

<p>Per configurare i tipi di record collegabili:</p>

<ul> 
<li><p>Qualsiasi pacchetto Workfront e Planning</p></li>
Oppure
<li><p>Qualsiasi pacchetto Workflow e un pacchetto Planning Prime o Ultimate</p></li></ul>

<div class="preview">

<p>Per configurare i tipi di record globali:</p>

<ul> 
<li><p>Qualsiasi pacchetto Workfront e un pacchetto Planning Plus</p></li>
Oppure
<li><p>Qualsiasi pacchetto Workflow e un pacchetto Planning Prime o Ultimate</p></li></ul>
<p>Per ulteriori informazioni su ciò che è incluso in ogni pacchetto Workfront Planning, contattare il rappresentante del proprio account Workfront. </p> 
</div>
   </td> </tr>
  <tr> 
   <td role="rowheader"><p>Licenza Adobe Workfront</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorizzazioni oggetto</p></td> 
   <td>   <p>Gestire le autorizzazioni per un’area di lavoro</p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p>  </td> 
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
   <td><p> Standard </p>
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
   <td>   <p>Manage permissions to a workspace and record type </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
   <p>Only system administrators can enable record types to connect from other workspaces</p> </td> 
  </tr> 

</tbody> 
</table> 

-->

## Configurare le informazioni sul tipo di record nella pagina Impostazioni

Puoi definire le funzionalità tra aree di lavoro diverse per un tipo di record configurando le informazioni nella relativa pagina Impostazioni.

<!--the intro above will change when we can configure more in this area -->

{{step1-to-planning}}

1. Fare clic sull&#39;area di lavoro di cui si desidera modificare i tipi di record.

   Viene visualizzata la pagina dell&#39;area di lavoro e i tipi di record.
1. Esegui una delle operazioni seguenti:

   * Passa il puntatore del mouse sulla scheda di un tipo di record e fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) nell&#39;angolo superiore destro della scheda del tipo di record, quindi fai clic su **Impostazioni**

     ![Altre opzioni di menu dalla scheda del tipo di record](assets/more-menu-options-from-record-type-card-with-settings-link.png)

     Oppure

   * Fai clic su una scheda del tipo di record per aprire la pagina del tipo di record, fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) a destra del nome del tipo di record, quindi fai clic su **Impostazioni**.

   <!--update screen shot at prod??-->

   ![Impostazioni per più aree di lavoro nella pagina Impostazioni](assets/settings-page-cross-workspace-settings.png)

1. La sezione **Impostazioni tra aree di lavoro** è selezionata per impostazione predefinita.
1. Attiva o disattiva una delle seguenti impostazioni:

   * **Consente di aggiungere questo tipo di record ad altre aree di lavoro** per indicare che si tratta di un tipo di record globale
   * **Consenti la connessione a questo tipo di record in altre aree di lavoro** per indicare che si tratta di un tipo di record collegabile.

   Le impostazioni sono disattivate per impostazione predefinita.

   Per ulteriori informazioni, vedere [Configurare le funzionalità tra aree di lavoro diverse per i tipi di record](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)