---
title: Elimina aree di lavoro
description: È possibile eliminare le aree di lavoro quando non sono più rilevanti.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: adec4b8e-2964-479b-8cf0-79d3afa27b2a
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/yzpirNfY0Hsp0cbClQA8dFqhgqbpK8ZryIyeq4tBAgw
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 37be1f25fa54f3efd4113478496e95db3c8bce1c
workflow-type: tm+mt
source-wordcount: 499
ht-degree: 4%

---

# Eliminare le aree di lavoro

<span class="preview">Le informazioni contenute in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo il rilascio in anteprima, le stesse funzioni sono disponibili mensilmente nell’ambiente di produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedere [Abilitare o disabilitare le versioni rapide per l&#39;organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

In Adobe Workfront Planning, le aree di lavoro sono posizioni centralizzate in cui i team possono pianificare il lavoro. Per ulteriori informazioni, consulta [Creare aree di lavoro](/help/quicksilver/planning/architecture/create-workspaces.md).

È possibile eliminare le aree di lavoro non più rilevanti.

È consigliabile ricreare alcuni o tutti i tipi di record, i record, i campi e le visualizzazioni associati all&#39;area di lavoro che si desidera eliminare in un&#39;altra area di lavoro prima di eliminarla.

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
   <td role="rowheader"><p>Licenza di Adobe Workfront</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorizzazioni sugli oggetti</p></td> 
   <td>   <p>Gestire le autorizzazioni per un’area di lavoro</p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p>  </td> 
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
   <td>   <p>Manage permissions to a workspace</p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
</tbody> 
</table>
-->

## Considerazioni sull’eliminazione delle aree di lavoro

* Quando si eliminano le aree di lavoro, vengono eliminati anche tutti i tipi di record, i record, i relativi campi e le visualizzazioni.
* Le aree di lavoro eliminate e le informazioni in esse contenute non possono essere recuperate.

## Eliminare un’area di lavoro

{{step1-to-planning}}

1. (Condizionale) Se sei un amministratore di Workfront, fai clic su una delle seguenti opzioni:

   * **Aree di lavoro a cui partecipo** per accedere alle aree di lavoro create
   * **Tutte le aree di lavoro** per accedere alle aree di lavoro condivise con te o create dall&#39;utente

   >[!NOTE]
   >
   ><span class="preview">Impossibile eliminare le aree di lavoro nella scheda **Aree di lavoro di esempio**. È consigliabile utilizzare il bundle di modelli per più aree di lavoro per creare aree di lavoro simili a quelle disponibili nella scheda Area di lavoro di esempio. Per informazioni, vedere [Creare aree di lavoro](/help/quicksilver/planning/architecture/create-workspaces.md).</span>

1. (Facoltativo) Fai clic su **Mostra tutto** per visualizzare altre aree di lavoro. Il collegamento **Mostra tutto** viene visualizzato solo se sono presenti più di due righe di schede dell&#39;area di lavoro.
1. (Facoltativo) Fai clic su **Mostra meno** per limitare il numero di aree di lavoro visualizzate sullo schermo.
1. Per eliminare un&#39;area di lavoro, effettuate una delle seguenti operazioni:

   * Passa il puntatore del mouse sulla scheda dell&#39;area di lavoro, quindi fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) nell&#39;angolo superiore destro della scheda
Oppure
   * Fai clic sull&#39;icona **cerca** ![icona Cerca](assets/search-icon.png) nell&#39;angolo superiore destro della pagina Aree di lavoro per cercare un&#39;area di lavoro per nome e fai clic su una scheda dell&#39;area di lavoro per aprirla, quindi fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) a destra del nome dell&#39;area di lavoro.

   >[!TIP]
   >
   >È possibile utilizzare la seguente combinazione di tastiera per aprire la casella di ricerca globale da qualsiasi pagina di Workfront Planning e cercare le aree di lavoro:
   >
   >* CTRL+K per Windows
   >* ⌘+K per Mac

1. Fai clic su **Elimina**.

   ![Conferma eliminazione definitiva area di lavoro](assets/permanently-delete-workspace-confirmation.png)

1. Digita &quot;**delete**&quot; nello spazio fornito, quindi fai clic su **Delete** definitivamente. Non fa distinzione tra maiuscole e minuscole.

   L’area di lavoro viene eliminata e non può essere recuperata. Verranno eliminati anche tutti i tipi di record, i record, i campi e le visualizzazioni ad essi associati. <!--ensure this is right at or before GA-->


