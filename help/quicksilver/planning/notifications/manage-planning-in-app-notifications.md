---
title: Gestione delle notifiche in-app di Adobe Workfront Planning
description: Quando qualcuno assegna un tag a te o ai tuoi team in un commento del record, ricevi una notifica e-mail per quel tag.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: a6eb8c7c-a34d-4c84-a45c-7e7f050a4302
source-git-commit: e26a3d0e283182e08902c263252c8d067838c23a
workflow-type: tm+mt
source-wordcount: '365'
ht-degree: 0%

---


# Gestione delle notifiche in-app di Adobe Workfront Planning

{{planning-important-intro}}

È possibile ricevere notifiche in-app da Workfront Planning quando si verificano i seguenti scenari:

* Qualcuno assegna un tag a te o ai tuoi team in un commento record

  Per informazioni sull&#39;assegnazione di tag ad altri utenti in un commento record, vedere [Gestire i commenti record](/help/quicksilver/planning/records/manage-record-comments.md).
* Qualcuno richiede l’autorizzazione per accedere a una vista o a un’area di lavoro
* Qualcuno conferma che l&#39;accesso è stato concesso per una visualizzazione o un&#39;area di lavoro <!--Isk confirmed there is no notification for denying permissions - did not test-->

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
<p>Qualsiasi pacchetto Workfront e Planning</p> <p>Qualsiasi flusso di lavoro e qualsiasi pacchetto di Planning</p>
<p>Per ulteriori informazioni su ciò che è incluso in ogni pacchetto Workfront Planning, contattare il rappresentante del proprio account Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Licenza Adobe Workfront</p></td> 
   <td><p>Chiaro o superiore</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorizzazioni oggetto</p></td> 
   <td>   <p>Visualizza o autorizzazioni superiori per un'area di lavoro</a> </p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p> </td> 
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


<!--
OLD:

+++ Expand to view access requirements. 

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
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience.</p> 
<p>The users in your organization receive notifications from Workfront Planning only when your organization is onboarded to the Adobe Unified Experience. </p>
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
   <td>   <p>View or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> Users with a Light or Contributor license must be assigned a layout template that includes Planning.
   <p>Standard users and System Administrators have the Planning areas enabled by default.</p></div></li></ul>
</td>
  </tr>
</tbody> 
</table> 

+++
-->

## Gestire le notifiche in-app quando qualcuno ti assegna i tag in un commento

1. (Condizionale) Dopo che un utente ha aggiunto un tag a te o ai tuoi team in un commento su un record, passa all&#39;icona **Notifiche** in-app ![Icona notifiche Experience Cloud](assets/experience-cloud-notifications-icon.png) in Adobe Experience Cloud.

   ![Esempio di notifica in-app](assets/in-app-notification-example.png)

1. Fai clic sulla notifica.

   La pagina dei dettagli del record viene visualizzata in Workfront Planning. È possibile aggiornare il record o rispondere al commento.

1. (Facoltativo) Fai clic su **Segna tutto come letto** per indicare che hai letto tutte le notifiche.
1. (Facoltativo) Fai clic su **Visualizza tutto** per passare alla pagina **Notifiche** in Adobe Experience Cloud.

## Gestire le notifiche in-app quando si richiedono e si concedono le autorizzazioni

Ricevi notifiche in-app quando qualcuno ti richiede o ti concede autorizzazioni per una visualizzazione o un’area di lavoro.

Per informazioni sulla richiesta, la concessione o il rifiuto delle autorizzazioni per una visualizzazione o un&#39;area di lavoro, vedere [Richiedere le autorizzazioni per una visualizzazione o un&#39;area di lavoro](/help/quicksilver/planning/access/request-permissions.md).

Per informazioni sulla gestione delle notifiche di Workfront Planning, vedere [Gestione preferenze di notifica di Adobe Workfront Planning](/help/quicksilver/planning/notifications/manage-notification-preferences.md).
