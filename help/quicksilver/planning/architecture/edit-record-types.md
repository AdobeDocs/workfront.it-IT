---
title: Modifica tipi di record
description: È possibile modificare i tipi di record dopo il salvataggio. I tipi di record sono i tipi di oggetto di Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7d6de742-9657-4286-968c-1fc78ebbb94e
source-git-commit: 2fb95d37c32984e248767993c4858038d27e0590
workflow-type: tm+mt
source-wordcount: '634'
ht-degree: 2%

---


# Modifica tipi di record

<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo i rilasci mensili in Produzione, le stesse funzioni sono disponibili nell’ambiente di Produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedere [Abilitare o disabilitare le versioni rapide per l&#39;organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

I tipi di record sono i tipi di oggetto di Adobe Workfront Planning. È possibile modificare l&#39;aspetto dei tipi di record creati dall&#39;utente o da qualsiasi altro utente. Per informazioni sulla creazione di tipi di record di Workfront Planning, vedere [Creare tipi di record](/help/quicksilver/planning/architecture/create-record-types.md).

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
<p>Qualsiasi pacchetto Workfront e Planning</p>
<p><b>NOTA</b></p>
<p>Per configurare i tipi di record collegabili: </p>
<ul> 
<li><p>Qualsiasi pacchetto Workfront e qualsiasi pacchetto Planning</p></li>
<p>Oppure</p>
<li><p>Qualsiasi flusso di lavoro e un pacchetto Planning Prime o Ultimate</p></li></ul>

<div class="preview">
<p>Per configurare i tipi di record globali:</p>

<ul> 
<li><p>Qualsiasi pacchetto Workfront e un pacchetto Planning Plus</p></li>
<p>Oppure</p>
<li><p>Qualsiasi flusso di lavoro e un pacchetto Planning Prime o Ultimate</p></li></ul>
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
</table> -->

## Modifica tipi di record

{{step1-to-planning}}

1. Fare clic sul workspace di cui si desidera modificare i tipi di record.

   Viene visualizzata la pagina dell&#39;area di lavoro e i tipi di record.
1. Esegui una delle operazioni seguenti:

   * Passa il puntatore del mouse sulla scheda di un tipo di record e fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) nell&#39;angolo superiore destro della scheda del tipo di record, quindi fai clic su **Modifica**
     <span class="preview">o **Impostazioni**</span>
Oppure
   * Fai clic su una scheda del tipo di record per aprire la pagina del tipo di record, fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) a destra del nome del tipo di record, quindi fai clic su **Modifica** <span class="preview">o **Impostazioni**</span>.

   <span class="preview">![Altre opzioni di menu dalla scheda del tipo di record con Impostazioni](assets/more-menu-options-from-record-type-card-with-settings-link.png)</span>

1. Nella casella **Modifica tipo di record**, per impostazione predefinita viene aperta la scheda **Aspetto**. <!--update screen shot below at production-->

   ![Modifica la scheda dell&#39;aspetto della casella del tipo di record ](assets/edit-record-type-box-appearance-tab.png)

   Aggiorna le seguenti informazioni nella scheda **Aspetto**:

   * Se necessario, modificare il nome del tipo di record. <!--did they add a field label for this?-->
   * **Descrizione**: modificare o aggiungere una descrizione per il tipo di record con ulteriori informazioni.
   * Modificare il colore e la forma dell&#39;icona associata al tipo di record. Effettua le seguenti operazioni:
      * Selezionare un colore per identificare il tipo di record. Colore dell&#39;icona del tipo di record.
      * Seleziona un’icona dall’elenco, oppure inizia a digitare il nome di un’icona per descrivere ciò che rappresenta, quindi selezionala quando viene visualizzata. Icona del tipo di record. Per impostazione predefinita, viene selezionata un&#39;icona di file.

1. (Facoltativo e condizionale) Se sei un amministratore di sistema, fai clic sulla scheda **Impostazioni avanzate** <span class="preview">o **Impostazioni per più aree di lavoro**</span> e aggiorna le informazioni sulle funzionalità per più aree di lavoro del tipo di record.

   Per ulteriori informazioni, vedere [Configurare le funzionalità tra aree di lavoro diverse per i tipi di record](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md). <!--update screen shot at production - Jan 2026-->

   ![Casella Modifica tipo di record con scheda Impostazioni avanzate](assets/edit-record-type-box-advanced-settings-tab.png)

1. Fai clic su **Salva**.

   Se hai selezionato di connettere questo record da altre aree di lavoro, l&#39;icona **Record collegabile** ![Icona Connetti da altri spazi](assets/connect-from-other-workspaces-icon.png) viene visualizzata sulla scheda record.

   <span class="preview">Se hai scelto di consentire l&#39;aggiunta di questo record ad altre aree di lavoro, l&#39;icona del **record globale** ![icona del tipo di record globale](assets/global-icon.png) viene visualizzata sulla scheda record. </span>

1. (Facoltativo) Fai clic sulla scheda del tipo di record nell’area di lavoro per aprire la pagina del tipo di record, quindi rinomina il tipo di record nell’intestazione.

1. (Facoltativo) Per modificare un altro tipo di record, dalla pagina tipo di record espandere la freccia rivolta verso il basso a destra del nome di un tipo di record, cercare un tipo di record e selezionarlo quando viene visualizzato nell&#39;elenco.

   ![Elenco a discesa del tipo di record nella pagina del tipo di record con casella di ricerca](assets/record-type-drop-down-on-record-type-page-with-search-box.png)
