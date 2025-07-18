---
title: Richiedere le autorizzazioni per una visualizzazione o un Workspace
description: Quando qualcuno condivide un collegamento a una visualizzazione o a un'area di lavoro a cui non hai accesso, puoi richiedere le autorizzazioni necessarie per aprirlo. In questo articolo vengono illustrati i passaggi necessari per richiedere l'accesso a una visualizzazione o a un'area di lavoro quando si verifica un collegamento condiviso che non è possibile aprire.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 94dfa36a-801a-4eef-bcf5-4a3fecc5a3d0
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '629'
ht-degree: 1%

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

+++ Espandere per visualizzare i requisiti di accesso.

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
<p>Per poter accedere a Workfront Planning, l’istanza di Workfront della tua organizzazione deve essere integrata in Adobe Unified Experience.</p> 
<p><b>IMPORTANTE</b></p>
<p>Gli utenti dell’organizzazione possono richiedere autorizzazioni per visualizzazioni e aree di lavoro solo quando l’organizzazione è integrata in Adobe Unified Experience. </p>
<p>Per ulteriori informazioni, vedere <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Esperienza unificata Adobe per Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licenza Adobe Workfront*</p></td> 
   <td><p> Standard, Light o Contributor</p>
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
   <td>  <p>Dopo aver concesso la richiesta di autorizzazione, puoi ottenere le seguenti autorizzazioni:</p>
   <ul><li><p>Visualizzare o gestire una visualizzazione</p></li>
   <li><p>Visualizzare, contribuire o gestire in un'area di lavoro</p></li></ul>  
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

*Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


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
