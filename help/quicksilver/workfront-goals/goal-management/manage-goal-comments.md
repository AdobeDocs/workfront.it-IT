---
product-previous: workfront-goals
navigation-topic: goal-management
title: Gestire i commenti sugli obiettivi in Obiettivi di Adobe Workfront
description: Puoi aggiungere commenti a tutti gli obiettivi che puoi visualizzare in Obiettivi di Adobe Workfront.
author: Alina
feature: Workfront Goals
exl-id: 6cf2d2d2-5ba5-40f2-a803-01359c338541
source-git-commit: 6e2e337969fccba88ea7089fe9a6d9db605343f7
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 1%

---

# Gestire i commenti sugli obiettivi in Obiettivi di Adobe Workfront

<!--Audited for P&P only: 04/2025-->

<!--consider retiring this article when goals and all objects are in parity and we remove the legacy commenting from the system. From then on, there is just ONE way to comment and that will be documented in the Update Work article-->

<!--take "legacy" and "new commenting" references out when we remove the legacy - April 2024???-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. </span>

<span class="preview">For information about the current release schedule, see [First Quarter 2024 release overview](../../product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).</span>-->

<!--
After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>  
<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)</span>  
-->

Puoi aggiungere commenti a tutti gli obiettivi che puoi visualizzare in Obiettivi di Adobe Workfront.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire le azioni descritte in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> 
   <p>Per il nuovo piano e la nuova struttura delle licenze:
  <ul><li>Un piano Ultimate </li></ul>
   </p>
<p>Per il piano corrente e la struttura delle licenze: 
<ul><li> A Pro o superiore </li>
  <li>Una licenza Adobe Workfront Goals oltre a una licenza Workfront.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Licenza Adobe Workfront</td>
 <td>
 <p>Qualsiasi</td>
 </tr>
 <tr>
 <td role="rowheader">Prodotto*</td>
 <td>
 <p> Nuovo requisito prodotto: Workfront</p>
 Oppure
 <p>Requisiti attuali del prodotto: oltre a una licenza Workfront, è necessario acquistare una licenza per gli obiettivi Adobe Workfront. </p> <p>Per informazioni, vedere <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requisiti per l'utilizzo degli obiettivi di Workfront</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Configurazione del livello di accesso</td>
 <td> <p>Visualizzare o accedere più facilmente agli obiettivi</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Autorizzazioni oggetto</td>
 <td>
  <div>
  <p>Visualizza o autorizzazioni superiori per l’obiettivo</p>
  <p>Per impostazione predefinita, gli utenti non hanno accesso agli obiettivi </p>
 <p>Per informazioni sulla condivisione degli obiettivi, vedere <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Condividere un obiettivo in Obiettivi di Workfront</a>. </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>Modello layout</p></td>
   <td> <p>A tutti gli utenti, inclusi gli amministratori di Workfront, deve essere assegnato un modello di layout che includa l’area Obiettivi nel menu principale. </p>  
</td>
  </tr>
</tbody>
</table>

*Per ulteriori informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Gestisci commenti obiettivo

Puoi aggiungere commenti agli obiettivi nella sezione Aggiornamenti della pagina di un obiettivo.

1. Fai clic sull&#39;icona **Main Menu** ![Main Menu icon](assets/main-menu-icon.png) nell&#39;angolo superiore destro o sull&#39;icona **Main Menu** ![Main Menu lines](assets/lines-main-menu.png) nell&#39;angolo superiore sinistro, se disponibile, quindi fai clic su **Goals**.
Verrà aperto l&#39;elenco degli obiettivi.
1. Individua l’obiettivo a cui desideri aggiungere commenti, quindi fai clic sul nome per aprire la pagina dell’obiettivo.
1. Fai clic su **Aggiornamenti** nel pannello a sinistra.

   Per ulteriori informazioni sulla gestione dei commenti per gli oggetti Workfront, vedere [Aggiorna lavoro](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

<!--   
1. (Optional) To locate an existing comment, start typing a keyword (*****or a user's name********) in the **Search** box in the upper-right corner of the **Comments** tab. 
   
   ![Search field](assets/search-field-in-updates-tab-goals.png)

   The keyword (****or user****) you searched for is highlighted and the comments that contain it display at the top of the Updates section. 


      >[!NOTE]
      >
      >You must search for a word included in a comment or reply. You cannot search for a tagged user or team.
   
   For more information, see [Update work](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

1. Click the **x** icon in the search field to clear the search results and return to the complete update.
1. Click the **Comments** tab in the upper-left corner of the Updates area.
1. Start entering a comment in the **New comment** box.
         
   ![Comment box](assets/comment-box-empty-unshimmed.png)

   >[!TIP]
   >
   >Navigating away from the Updates section before you finish typing and submitting a comment keeps the comment on the page in draft mode even after you log off and log back on. Drafts are saved for 7 days after which they are discarded and cannot be recovered. Drafted comments are only visible to the user entering them.

1. (Optional) To undo or redo a change, use the following shortcut keys:
      * CTRL + Z (⌘+z for Mac) to undo a change 
      * CTRL + Y (⌘+y for Mac) to redo a change 
1. (Optional) To add rich-text formatting to your update, a hyperlink, or an emoji, use any options on the Rich Text toolbar or the icons adjacent to it. For more information, see [Update work](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). 
1. (Optional) In the **Tag people or teams** area, start typing the name or the email of a user, or a team that you would like to include in this comment, then select it when it displays in the list. 
1. Select the **Private to my company** toggle to make the comment visible only to people in your company. 

      >[!TIP]
      >
      >You must have a Company specified in your profile to have this option available in the Updates area. 

1. Click **Submit**. 

      >[!TIP]
      >
      >If another user submits a comment to the same item you are updating, there will be a red line with a "New" indicator to inform you of the newer comments, as well as a blue notification at the bottom of the screen indicating the number of new comments. 
      >
      >The indicator only displays only after the comment was submitted on the item, and not when the comment is still composed. 
      >![Real time new red indicator](assets/real-time-new-red-indicator-unified-commenting-copy.png)
      
1. (Optional) To edit a comment, click the **More** menu ![More icon](assets/more-icon.png) to the right of the Like icon, then click **Edit**. 
1. Edit the information in the comment or remove any of the tagged users. 
   You can edit your comment within 15 minutes from submitting it. An "edited" indicator is added to the left of the date stamp that displays when the comment was updated.

   ![Edited tag on comment](assets/edited-tag-on-comment-unified-commenting.png)

   >[!TIP]
   >
   > * An email is generated to notify users of your update only when you submit the original update. No email is generated after you edited your update.
   >
   > * The date stamp is the date of the original comment and not the date of the latest update. 

1. (Optional) Click the **More** menu ![More icon](assets/more-icon.png), then click any of the following options to copy information from a comment to the clipboard or into a new reply:

      * **Copy link** to copy the link of an update, without the replies.
      * **Copy body text** to copy the text of an update. 
      * **Quote reply** to open a new comment box where the original comment is quoted in a new reply and is marked as a block quote.

         For more information, see [Update work](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). 

1. (Optional) Click the **More** menu ![More icon](assets/more-icon.png) to the right of a comment, then click **Delete** to delete a comment you added. For more information, see [Update work](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. (Optional) Click **Reply** to reply to an existing comment, then follow the steps 5-9 above. For more information about replying to updates, see [Reply to updates](../../workfront-basics/updating-work-items-and-viewing-updates/reply-to-updates.md). (**********insure this stays accurate*********)
1. (Conditional and optional) If other users have added comments that display outside of the visible area in the Updates section, click **View** inside the blue **new comments banner** at the bottom of the screen  to display these comments.
   
   ![Blue comments banner](assets/blue-new-comments-banner-with-view-button.png)
   
   Additional comments display at the bottom of the screen.
1. (Optional) Click the **Like** icon![Like icon](assets/like-icon.png) to like a comment that someone else added. The icon updates with the number of likes.

1. (Optional) Click the **System Activity** tab to view updates logged by the system. When a goal is updated, Workfront generates a note about that update that and displays it in the System Activity tab. Workfront also records a system update when a result, activity, or project is added to the goal or when it is updated. (*********ensure the casing on the tab has not changed**********)-->


