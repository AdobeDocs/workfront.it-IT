---
title: Esporta record dalla vista tabella
description: È possibile esportare i record e le relative informazioni dalla vista tabella in un file CSV o Excel.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: d8ac4d94-28b5-41d6-acb8-259696897c8a
source-git-commit: 8546311acf722c0f4d47d4663b02ff701416894a
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 1%

---

# Esporta record dalla vista tabella

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

È possibile esportare i record e le relative informazioni dalla vista tabella in un file Excel o CSV in Adobe Workfront Planning.

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
   <td><p>Chiaro o superiore</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorizzazioni oggetto</p></td> 
   <td> <p>Visualizzare o modificare le autorizzazioni per un'area di lavoro e un tipo di record</p>   
   <p>Visualizzare o autorizzazioni superiori per una visualizzazione</p>

</td> 
  </tr> 
  <tr>
   <td role="rowheader"><p>Modello layout</p></td>
   <td> Agli utenti con una licenza Light o Contributor deve essere assegnato un modello di layout che includa Planning.
   <p>Per impostazione predefinita, le aree Pianificazione sono attivate dagli utenti standard e dagli amministratori di sistema.</p></div></li></ul>
</td>
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
   <td><p> Light or higher </p>
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
   <td>   <p>View or higher permissions to a view</p>  
   </td> 
  </tr> 
</tbody> 
</table> -->


## Esporta record dalla vista tabella

Quando esportate la vista tabella, tenete presente quanto segue:

* Le informazioni esportate in un file di Excel mantengono i filtri, i raggruppamenti e gli ordinamenti applicati alla vista tabella in Workfront Planning. I raggruppamenti non sono visibili nel file CSV.

* Le miniature e i colori di riga personalizzati non sono supportati nei file esportati.

* Vengono esportati solo i campi resi visibili nell’interfaccia di Workfront. I campi nascosti non vengono esportati.

Per esportare informazioni dalla vista tabella o da un tipo di record:

1. Passare a una pagina del tipo di record e fare clic su una scheda della vista tabella.
1. Esegui una delle operazioni seguenti:

   * Passa il puntatore del mouse sul nome della scheda di visualizzazione della tabella, quindi fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) a destra del nome della visualizzazione, quindi fai clic su **Esporta**.

   ![Altro menu in una visualizzazione](assets/view-more-menu-with-duplicate-option.png)

   * Fai clic su **Condividi** > **Esporta la visualizzazione corrente**. Questa opzione è disponibile solo quando viene visualizzata la vista tabella.

   ![Pulsante Condividi con tipo di record e opzioni di condivisione della visualizzazione](assets/share-button-with-record-type-and-view-sharing-options.png)

1. Selezionare uno dei formati seguenti:

   * **Excel**
   * **CSV**

   >[!IMPORTANT]
   >
   >Non è possibile esportare informazioni dalla vista tabella quando si visualizza una vista diversa sullo schermo. Per accedere all&#39;opzione Esporta nel menu Altro, è necessario visualizzare la vista tabella che si desidera esportare.

   Il file viene scaricato nel computer.

1. (Facoltativo) Vai alla cartella dei download sul tuo computer e trova il file scaricato.

   Il nome del file esportato è nel seguente formato:

   `Name of the view - name of the record type`

   Ad esempio, una visualizzazione tabella per il tipo di record Campagne genera un file denominato `Table view - Campaigns`.

   Nel file vengono visualizzate le seguenti informazioni:

   * Le intestazioni di colonna sono evidenziate in nero nel file Excel
   * Tutti i campi visibili nell’interfaccia di Workfront, ordinati e filtrati in base agli stessi criteri
   * I raggruppamenti vengono mantenuti nel file di Excel

   È ora possibile condividere i file esportati con altri utenti o allegarli a qualsiasi comunicazione.

</div>
