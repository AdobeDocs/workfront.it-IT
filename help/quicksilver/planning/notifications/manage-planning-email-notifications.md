---
title: Gestione delle notifiche e-mail di Adobe Workfront Planning
description: Quando qualcuno assegna un tag a te o ai tuoi team in un commento del record in Adobe Workfront Planning, ricevi una notifica e-mail per quel tag.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 3c505b3a-cda7-4e7b-b497-28b820e9bb8f
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '679'
ht-degree: 1%

---


# Gestire le notifiche e-mail di Adobe Workfront Planning

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

È possibile ricevere notifiche e-mail da Workfront Planning quando si verificano i seguenti scenari:

* Qualcuno assegna un tag a te o ai tuoi team in un commento record

  Per informazioni sull&#39;assegnazione di tag ad altri utenti in un commento record, vedere [Gestire i commenti record](/help/quicksilver/planning/records/manage-record-comments.md).
* Qualcuno richiede l’autorizzazione per accedere a una vista o a un’area di lavoro
* Qualcuno conferma che l&#39;accesso è stato concesso per una visualizzazione o un&#39;area di lavoro <!--Isk confirmed that there is nno email for denying access but did not test-->
* Inviare una richiesta di Workfront Planning. Per informazioni, vedere [Creare e gestire un modulo di richiesta in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md)
* Qualcuno approva o rifiuta una richiesta di Workfront Planning inviata dall&#39;utente. Per informazioni, vedere [Approvare una richiesta in Adobe Workfront Planning](/help/quicksilver/planning/requests/approve-request.md)
* Lo stato viene modificato in una richiesta di Workfront Planning sottomessa.

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
<p>L’istanza di Workfront della tua organizzazione deve essere integrata in Adobe Unified Experience.</p> 
<p>Gli utenti dell’organizzazione ricevono notifiche da Workfront Planning solo quando l’organizzazione è integrata in Adobe Unified Experience. </p>
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

*Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
OLD: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> 
   <p>In order to receive notifications from Workfront Planning and manage notification preferences, your organization's instance of Workfront must be onboarded to the Adobe Unified Experience. For information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>.</p></td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access level controls in Workfront Planning. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>View or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>
 </tbody>
</table>
-->


## Gestisci le notifiche e-mail quando qualcuno ti assegna i tag in un commento

1. (Condizionale e facoltativo) Dopo che un utente ha aggiunto un tag a te o al tuo team in un commento di un record, vai alla notifica e-mail che ti informa del tag e del commento. Il mittente dell’e-mail è Adobe Experience Cloud.

   ![Esempio di notifiche e-mail](assets/email-notification-example.png)

1. (Facoltativo) Fai clic sul messaggio nella casella **Workfront** all&#39;interno dell&#39;e-mail.

   La pagina dei dettagli del record viene visualizzata in Workfront. È possibile aggiornare il record o rispondere al commento.

1. (Condizionale) Se disponibile, fare clic su **Visualizza tutte le notifiche**. <!--check with Lilit - do non-IMS users have this button??-->
La pagina **Notifiche** viene aperta in Adobe Experience Cloud. Vengono visualizzate tutte le notifiche provenienti da tutte le applicazioni Adobe Experience Cloud.

## Gestire le notifiche e-mail quando si richiedono e si concedono le autorizzazioni

1. (Condizionale e facoltativo) Dopo che qualcuno ti ha richiesto o concesso le autorizzazioni per accedere a una visualizzazione o a un’area di lavoro, vai all’e-mail che ti informa della richiesta di autorizzazione. Il mittente dell’e-mail è Adobe Experience Cloud.

1. (Facoltativo) Fai clic sul messaggio nella casella **Workfront** all&#39;interno dell&#39;e-mail.

   La pagina dei dettagli del record viene visualizzata in Workfront. È possibile aggiornare il record o rispondere al commento.

1. (Condizionale) Se disponibile, fare clic su **Visualizza tutte le notifiche**.
La pagina **Notifiche** viene aperta in Adobe Experience Cloud. Vengono visualizzate tutte le notifiche provenienti da tutte le applicazioni Adobe Experience Cloud.


Per informazioni sulla richiesta, la concessione o il rifiuto delle autorizzazioni per una visualizzazione o un&#39;area di lavoro, vedere [Richiedere le autorizzazioni per una visualizzazione o un&#39;area di lavoro](/help/quicksilver/planning/access/request-permissions.md).

Per informazioni sulla gestione delle notifiche di Workfront Planning, vedere [Gestione preferenze di notifica di Adobe Workfront Planning](/help/quicksilver/planning/notifications/manage-notification-preferences.md).

## Gestire le notifiche e-mail relative all&#39;invio, all&#39;approvazione o al rifiuto di richieste di Workfront Planning

1. (Facoltativo) Vai all’e-mail che ti invia Workfront
dopo aver inviato una richiesta o dopo che una richiesta inviata è stata approvata o rifiutata. Il mittente dell’e-mail è Adobe Workfront.

1. (Facoltativo) Fai clic su **Apri richiesta**. Verrà aperta la richiesta in Workfront Planning.

1. Fai clic sull&#39;icona **Notifiche** ![Icona area Notifiche Unified Shell](assets/notifications-area-icon-unified-shell.png) nell&#39;angolo superiore destro della schermata per accedere alla pagina **Notifiche**.

   Per informazioni sulla gestione delle notifiche di Workfront Planning, vedere [Gestione preferenze di notifica di Adobe Workfront Planning](/help/quicksilver/planning/notifications/manage-notification-preferences.md).
