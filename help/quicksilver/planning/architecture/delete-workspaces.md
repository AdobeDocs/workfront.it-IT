---
title: Elimina aree di lavoro
description: È possibile eliminare le aree di lavoro quando non sono più rilevanti.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: adec4b8e-2964-479b-8cf0-79d3afa27b2a
source-git-commit: 1dc2791bed0dfada109ee102e09c25ae9a52e6b0
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 2%

---


# Eliminare le aree di lavoro

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

In Adobe Workfront Planning, le aree di lavoro sono posizioni centralizzate in cui i team possono pianificare il lavoro. Per ulteriori informazioni, vedere [Creare aree di lavoro](/help/quicksilver/planning/architecture/create-workspaces.md).

È possibile eliminare le aree di lavoro non più rilevanti.

È consigliabile ricreare alcuni o tutti i tipi di record, i record, i campi e le visualizzazioni associati all&#39;area di lavoro che si desidera eliminare in un&#39;altra area di lavoro prima di eliminarla.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

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
<p>Per poter accedere a tutte le funzionalità di Workfront Planning, l’istanza di Workfront della tua organizzazione deve essere integrata in Adobe Unified Experience.</p> 
<p>Per ulteriori informazioni, vedere <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Esperienza unificata Adobe per Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licenza Adobe Workfront*</p></td> 
   <td><p> Standard </p>
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
   <td>   <p>Gestione delle autorizzazioni per un'area di lavoro</a> </p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modello layout</p></td> 
   <td> <p>A tutti gli utenti, inclusi gli amministratori di Workfront, deve essere assegnato un modello di layout che includa l'area Planning nel menu principale. </p> </td> 
  </tr> 
</tbody> 
</table>

*Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--replace the layout template info in the table with this at release: 


<p>In the Production environment, all users including the System Administrators must be assigned to a layout template that includes the Planning areas.</p>
<p><span class="preview">In the Preview environment, Standard users and System Administrators have the Planning area enabled by default.</span></p>

-->

## Considerazioni sull’eliminazione delle aree di lavoro

* Quando si eliminano le aree di lavoro, vengono eliminati anche tutti i tipi di record, i record, i relativi campi e le visualizzazioni.
* Le aree di lavoro eliminate e le informazioni in esse contenute non possono essere recuperate.

## Eliminare un’area di lavoro

{{step1-to-planning}}

1. (Condizionale) Se sei un amministratore di Workfront, fai clic su **Aree di lavoro in cui sono presente** per accedere alle aree di lavoro create oppure su **Altre aree di lavoro** per accedere alle aree di lavoro condivise con te.

1. (Facoltativo) Fai clic su **Mostra tutto** per visualizzare altre aree di lavoro. Il collegamento **Mostra tutto** viene visualizzato solo se sono presenti più di due righe di schede dell&#39;area di lavoro.
1. (Facoltativo) Fai clic su **Mostra meno** per limitare il numero di aree di lavoro visualizzate sullo schermo.
1. Per eliminare un&#39;area di lavoro, effettuate una delle seguenti operazioni:

   * Passa il puntatore del mouse sulla scheda dell&#39;area di lavoro, quindi fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) nell&#39;angolo superiore destro della scheda
Oppure
   * Fai clic su una scheda dell&#39;area di lavoro per aprirla, quindi fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) a destra del nome dell&#39;area di lavoro.
1. Fare clic su **Elimina**.

   ![Conferma eliminazione definitiva area di lavoro](assets/permanently-delete-workspace-confirmation.png)

1. Digita &quot;**delete**&quot; nello spazio fornito, quindi fai clic su **Delete** definitivamente. Non fa distinzione tra maiuscole e minuscole.

   L’area di lavoro viene eliminata e non può essere recuperata. Verranno eliminati anche tutti i tipi di record, i record, i campi e le visualizzazioni ad essi associati. <!--ensure this is right at or before GA-->
