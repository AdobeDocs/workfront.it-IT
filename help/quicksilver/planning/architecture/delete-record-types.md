---
title: Cancella Tipi di Record
description: È possibile eliminare i tipi di record quando non sono più rilevanti. L'eliminazione dei tipi di record comporta anche l'eliminazione di tutte le informazioni associate ai tipi di record, ad esempio record, campi e visualizzazioni.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 70fd3887-3871-45b5-9c21-f57da63662aa
source-git-commit: 2fb95d37c32984e248767993c4858038d27e0590
workflow-type: tm+mt
source-wordcount: '1062'
ht-degree: 0%

---


<!--keep the global record type reference in yellow till January 2026-->

# Elimina tipi di record

<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo i rilasci mensili in Produzione, le stesse funzioni sono disponibili nell’ambiente di Produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedere [Abilitare o disabilitare le versioni rapide per l&#39;organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

È possibile eliminare i tipi di record quando non sono più rilevanti.

Tuttavia, l&#39;eliminazione dei tipi di record comporta anche l&#39;eliminazione di tutte le informazioni associate ai tipi di record. Per ulteriori informazioni, vedere la sezione [Considerazioni durante l&#39;eliminazione dei tipi di record](#considerations-when-deleting-record-types) in questo articolo.

Per informazioni sui tipi di record, vedere [Panoramica sui tipi di record](/help/quicksilver/planning/architecture/overview-of-record-types.md).

<!-- last sentence might need to be deleted when we can recover or replace deleted record types-->

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
<p>Oppure</p>
<li><p>Qualsiasi flusso di lavoro e qualsiasi pacchetto di Planning</p></li></ul>
<div class="preview">
<p>Per eliminare i tipi di record globali:</p>
<ul><li><p>Qualsiasi pacchetto Workfront e un pacchetto Planning Plus</p></li>
<p>Oppure</p>
<li><p>Qualsiasi flusso di lavoro e un pacchetto Planning Prime o Ultimate</p></li></ul>
</div>
<p>Per ulteriori informazioni su ciò che è incluso in ogni pacchetto Workfront Planning, contattare il rappresentante del proprio account Workfront. </p> 
   </td> 
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
   <td>   <p>Manage permissions to a workspace and record type</p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p></td> 
  </tr> 
</tbody> 
</table> 
-->


## Considerazioni durante l’eliminazione dei tipi di record

<!--check this and ensure these are still true - some things might change with / after closed beta-->

* È possibile eliminare solo i tipi di record dalle aree di lavoro per le quali si dispone delle autorizzazioni Gestione.
* L&#39;eliminazione dei tipi di record comporta la rimozione delle seguenti informazioni ad essi associate:

   * Tutti i record di quel tipo.
   * Tutti i campi associati al tipo di record.
   * Tutte le visualizzazioni (inclusi filtri, raggruppamenti e criteri di ordinamento) del tipo di record.
* Il tipo di record viene rimosso da tutti gli utenti che accedono all’area di lavoro.
* Non è possibile recuperare i tipi di record eliminati o le relative informazioni.
* È consigliabile ricreare i campi e i record associati al tipo di record che si desidera eliminare in un altro tipo di record prima di eliminarli.

<div class="preview">

* Non è possibile eliminare un tipo di record globale aggiunto ad altre aree di lavoro.

  Per ulteriori informazioni, vedere la sezione [Eliminare i tipi di record globali](#delete-global-record-types) in questo articolo.

</div>

## Elimina tipi di record

{{step1-to-planning}}

1. Fare clic sull&#39;area di lavoro di cui si desidera eliminare i tipi di record.

   Oppure

   Da un workspace, espandere la freccia rivolta verso il basso a destra del nome di un workspace esistente, cercare un workspace e selezionarlo quando viene visualizzato nell&#39;elenco.

   Viene aperto il workspace e vengono visualizzati i tipi di record.
1. Esegui una delle operazioni seguenti:

   * Passa il puntatore del mouse sulla scheda del tipo di record, fai clic sul menu **Altro**, quindi su **Elimina**.
   * Fare clic sulla scheda del tipo di record che si desidera eliminare e nella pagina del tipo di record fare clic sul menu **Altro** ![Altro menu](assets/more-menu.png) a destra del nome del tipo di record, quindi fare clic su **Elimina**.

   ![Conferma eliminazione definitiva tipo di record](assets/permanently-delete-record-type-confirmation.png)


1. Digita **delete** nella casella di conferma, quindi fai clic su **Delete** definitivamente. Non fa distinzione tra maiuscole e minuscole.

   Il tipo di record selezionato, insieme ai relativi campi, record associati e viste, viene eliminato e non può essere recuperato.

<div class="preview">

## Elimina tipi di record globali

Durante l&#39;eliminazione dei tipi di record globali sono presenti i seguenti scenari:

* Se un tipo di record configurato come globale non è stato ancora aggiunto a un&#39;altra area di lavoro, è possibile eliminarlo dall&#39;area di lavoro originale.

* Se un tipo di record configurato come tipo di record globale è stato aggiunto ad almeno un&#39;altra area di lavoro, non è possibile eliminarlo dall&#39;area di lavoro originale. È innanzitutto necessario rimuovere (eliminando) i tipi di record globali dalle aree di lavoro secondarie in cui sono stati aggiunti, quindi è possibile eliminare definitivamente il tipo di record globale dall&#39;area di lavoro originale.

### Eliminare un tipo di record globale dal workspace originale

È possibile eliminare un tipo di record dall&#39;area di lavoro originale se non è più rilevante.

1. Passare al tipo di record globale nell&#39;area di lavoro originale.

1. (Condizionale) Effettuare una delle operazioni seguenti, a seconda che il tipo di record globale sia stato aggiunto o meno alle aree di lavoro secondarie:

   * Se il tipo di record non è stato aggiunto a un&#39;area di lavoro secondaria, fare clic sul menu **Altro** ![Altro menu](assets/more-menu.png) sulla scheda del tipo di record o a destra del nome del tipo di record nella relativa pagina, quindi fare clic su **Elimina**.
   * Se il tipo di record è stato aggiunto ad almeno un&#39;altra area di lavoro secondaria, passare innanzitutto all&#39;area di lavoro secondaria ed eliminare il record globale da tale spazio.

     Per informazioni, vedere la sezione [Eliminare un tipo di record globale da un&#39;area di lavoro secondaria](#delete-a-global-record-type-from-a-secondary-workspace) in questo articolo.

1. (Condizionale) Continuare a eliminare il tipo di record, come descritto nella sezione [Eliminare i tipi di record](#delete-record-types-1) in questo articolo.

   Si verificano le seguenti situazioni:

   * Il tipo di record globale viene rimosso dall’area di lavoro originale e non è possibile recuperare il tipo di record, i relativi record e campi.
   * Vengono rimossi anche tutti i tipi di record globali dalle aree di lavoro secondarie e dai relativi record.

### Eliminare un tipo di record globale da un workspace secondario

Se non è più necessario, è possibile eliminare un tipo di record aggiunto da un&#39;altra area di lavoro.

Considera quanto segue:

* Se si elimina un tipo di record globale da un workspace secondario, questo verrà rimosso solo dal workspace secondario. Il tipo di record rimane nell&#39;area di lavoro originale.

* Quando si elimina un tipo di record globale da un&#39;area di lavoro secondaria, vengono eliminati anche i seguenti elementi:

   * Record aggiunti dall&#39;area di lavoro secondaria.

  <!--Coming later: * The fields added from the secondary workspace.-->

* Non è possibile recuperare i tipi di record globali eliminati dalle aree di lavoro secondarie.

* Il tipo di record originale rimane nell&#39;area di lavoro originale e in altre aree di lavoro in cui è stato aggiunto.

Per eliminare un tipo di record globale da un&#39;area di lavoro secondaria:

1. Passare al tipo di record globale nell&#39;area di lavoro secondaria.

1. (Facoltativo) Fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) sulla scheda del tipo di record o a destra del nome del tipo di record nella relativa pagina, quindi fai clic su **Elimina**.
1. (Condizionale) Digita **delete** nel campo fornito, quindi fai clic su **Delete** definitivamente.

   ![Casella di conferma Elimina tipo di record globale secondario](assets/delete-secondary-global-record-type.png)

   Si verificano le seguenti situazioni:

   * Il tipo di record creato da un tipo di record globale viene rimosso dall&#39;area di lavoro selezionata.
   * Il tipo di record originale con i relativi campi rimane nell&#39;area di lavoro originale.
   * Il tipo di record rimane in tutte le altre aree di lavoro in cui è stato aggiunto.
   * I record <!--and fields--> aggiunti al tipo di record dall&#39;area di lavoro corrente vengono eliminati. Tutti gli altri record aggiunti da aree di lavoro aggiuntive in cui è stato aggiunto il tipo di record globale vengono conservati nelle rispettive aree di lavoro e nell&#39;area di lavoro originale. &lt;!- I campi vengono conservati nelle aree di lavoro in cui sono stati aggiunti.

</div>
