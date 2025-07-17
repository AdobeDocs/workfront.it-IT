---
title: Cancella Tipi di Record
description: È possibile eliminare i tipi di record quando non sono più rilevanti. L'eliminazione dei tipi di record comporta anche l'eliminazione di tutte le informazioni associate ai tipi di record, ad esempio record, campi e visualizzazioni.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 70fd3887-3871-45b5-9c21-f57da63662aa
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 2%

---


# Elimina tipi di record

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

È possibile eliminare i tipi di record quando non sono più rilevanti.

Tuttavia, l&#39;eliminazione dei tipi di record comporta anche l&#39;eliminazione di tutte le informazioni associate ai tipi di record. Per ulteriori informazioni, vedere la sezione [Considerazioni durante l&#39;eliminazione dei tipi di record](#considerations-when-deleting-record-types) in questo articolo.

Per informazioni sui tipi di record, vedere [Panoramica sui tipi di record](/help/quicksilver/planning/architecture/overview-of-record-types.md).

<!-- last sentence might need to be deleted when we can recover or replace deleted record types-->

## Requisiti di accesso

+++ Espandere per visualizzare i requisiti di accesso.

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Prodotti</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Piano Adobe Workfront*</p></td> 
   <td> 
<p>Uno dei seguenti piani di Workfront:</p> 
<ul><li>Seleziona</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning non è disponibile per i piani Workfront legacy</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Pacchetto Adobe Workfront Planning*</p></td> 
   <td> 
<p>Qualsiasi </p> 
<p>Per ulteriori informazioni su quanto incluso in ogni piano di Workfront Planning, contattare l'account manager Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Piattaforma Adobe Workfront</p></td> 
   <td> 
<p>Per poter accedere a Workfront Planning, l’istanza di Workfront della tua organizzazione deve essere integrata in Adobe Unified Experience.</p> 
<p>Per ulteriori informazioni, vedere <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Esperienza unificata Adobe per Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licenza Adobe Workfront*</p></td> 
   <td><p> Standard</p>
   <p>Workfront Planning non è disponibile per le licenze Workfront legacy</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configurazione del livello di accesso</p></td> 
   <td> <p>Nessun controllo del livello di accesso per Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Autorizzazioni oggetto</p></td> 
   <td>   <p>Gestire le autorizzazioni per un’area di lavoro e un tipo di record</p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p></td> 
  </tr> 
</tbody> 
</table>

*Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


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
