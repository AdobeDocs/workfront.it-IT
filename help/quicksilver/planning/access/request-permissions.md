---
title: Richiedere le autorizzazioni per una visualizzazione o un Workspace
description: Quando qualcuno condivide un collegamento a una visualizzazione o a un'area di lavoro a cui non hai accesso, puoi richiedere le autorizzazioni necessarie per aprirlo. In questo articolo vengono illustrati i passaggi necessari per richiedere l'accesso a una visualizzazione o a un'area di lavoro quando si verifica un collegamento condiviso che non è possibile aprire.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 94dfa36a-801a-4eef-bcf5-4a3fecc5a3d0
source-git-commit: c879d06cfe7ba76df3e974c160a7349f1503f17f
workflow-type: tm+mt
source-wordcount: '519'
ht-degree: 0%

---

# Richiedere le autorizzazioni per una visualizzazione o un’area di lavoro

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

>[!IMPORTANT]
>
>La funzionalità descritta in questo articolo è disponibile solo quando l’organizzazione è stata integrata in Adobe Unified Experience.
>
>Per ulteriori informazioni, vedere [Esperienza unificata Adobe per Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).


È possibile richiedere le autorizzazioni per una visualizzazione o un&#39;area di lavoro quando qualcuno condivide con te un collegamento alla visualizzazione o all&#39;area di lavoro a cui non hai accesso.

La richiesta delle autorizzazioni per una visualizzazione è simile alla richiesta delle autorizzazioni per un&#39;area di lavoro.

In questo articolo viene descritto come richiedere l&#39;accesso a una visualizzazione o a un&#39;area di lavoro quando un utente condivide un collegamento con l&#39;utente e non è possibile accedere alla pagina condivisa.

Per informazioni sulla concessione di autorizzazioni per visualizzazioni e aree di lavoro, vedere gli articoli seguenti:

* [Condividere le visualizzazioni](/help/quicksilver/planning/access/share-views.md)
* [Condividere le aree di lavoro](/help/quicksilver/planning/access/share-workspaces.md)


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
   <td role="rowheader"><p>Pacchetto Adobe Workfront</p></td> 
   <td> 
<p>Qualsiasi pacchetto Workfront e Planning</p> 
Oppure
<p>Qualsiasi pacchetto di Workflow e Planning</p> 
 </tr>

<tr> 
   <td role="rowheader"><p>Licenza Adobe Workfront</p></td> 
   <td><p>Qualsiasi</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configurazione del livello di accesso</p></td> 
   <td> <p>Nessun controllo del livello di accesso per Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Autorizzazioni oggetto</p></td> 
   <td>  <p>Dopo aver concesso la richiesta di autorizzazione, puoi ottenere le seguenti autorizzazioni:</p>
   <ul><li><p>Visualizzare o gestire una visualizzazione</p></li>
   <li><p>Visualizzare, contribuire o gestire per un'area di lavoro</p></li></ul>  
   <p>Solo gli utenti con le autorizzazioni di gestione per un’area di lavoro e una visualizzazione possono condividere una visualizzazione pubblicamente.</p></td> 
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
<p><b>IMPORTANT</b></p>
<p>The users in your organization can request permissions for views and workspaces only when your organization is onboarded to the Adobe Unified Experience. </p>
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard, Light, or Contributor</p>
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
   <td>  <p>After your request for permission is granted, you could gain the following permissions:</p>
   <ul><li><p>View or Manage for a view</p></li>
   <li><p>View, Contribute, or Manage to a workspace</p></li></ul>  
   <p>Only users with Manage permissions to a workspace and a view can share a view publicly.</p></td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> Users with a Light or Contributor license must be assigned a layout template that includes Planning.
   <p>Standard users and System Administrators have the Planning areas enabled by default.</p></div></li></ul>
  
</td>
  </tr>
 
</tbody> 
</table> -->


## Richiedere le autorizzazioni per una visualizzazione o un’area di lavoro

La richiesta di autorizzazioni per una visualizzazione è simile alla richiesta di autorizzazioni per un&#39;area di lavoro.

Quando qualcuno condivide con te un collegamento a un’area di lavoro o a una visualizzazione a cui non hai accesso:

1. Fai clic sul collegamento condiviso con te per la visualizzazione o l’area di lavoro.

   Viene visualizzata una pagina di **Accesso negato** per informare che non si dispone dell&#39;accesso alla visualizzazione o all&#39;area di lavoro.

   ![Richiedi accesso alla visualizzazione](assets/request-access-to-view.png)

1. (Condizionale) Se il collegamento condiviso è per una visualizzazione di un&#39;area di lavoro a cui hai accesso, fai clic su **Apri con visualizzazione esistente**. Se si dispone delle autorizzazioni di accesso all&#39;area di lavoro, la pagina del tipo di record viene visualizzata nella visualizzazione predefinita.

1. (Facoltativo e condizionale) Se non disponi delle autorizzazioni necessarie per visualizzare l&#39;area di lavoro, aggiungi un messaggio personalizzato nella casella disponibile, quindi fai clic su **Richiedi accesso**.

   Tutti gli utenti con autorizzazioni di gestione per la visualizzazione o l’area di lavoro ricevono le notifiche seguenti per la richiesta di accesso:
   * Una notifica in-app
     ![Notifica in-app per la richiesta di accesso](assets/in-app-notification-for-access-request.png)
   * Una notifica e-mail
     ![Notifica e-mail per la richiesta di accesso](assets/email-notification-for-access-request.png)

1. (Facoltativo) Quando il gestore della visualizzazione o dell’area di lavoro ti concede le autorizzazioni per la visualizzazione o l’area di lavoro, ricevi una notifica e-mail e una notifica in-app con la conferma che l’autorizzazione è stata concessa. <!--check this - I was not able to test this, but Isk confirmed.-->
