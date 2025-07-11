---
title: Gestire le preferenze di notifica di Adobe Workfront Planning
description: È possibile gestire le preferenze di notifica per Adobe Workfront Planning. Questo articolo descrive come configurare le preferenze per le notifiche.
author: Alina
feature: Workfront Planning
role: User
recommendations: noDisplay, noCatalog
exl-id: ec549a61-095c-433f-80e2-1be5c0a05180
source-git-commit: d3d4a923dddb8685a981162918f34447300136cf
workflow-type: tm+mt
source-wordcount: '519'
ht-degree: 1%

---


# Gestire le preferenze di notifica di Adobe Workfront Planning

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

In Workfront Planning è possibile ricevere una notifica in-app o e-mail quando si verificano le seguenti azioni:

* Qualcuno aggiunge te o i tuoi team a un commento nella pagina del record
* Qualcuno chiede l&#39;autorizzazione per accedere a una vista o a un&#39;area di lavoro
* Qualcuno ti concede l&#39;autorizzazione per accedere a una visualizzazione o a un&#39;area di lavoro <!--I could not test this but Isk confirmed-->
* Inviare una richiesta di Workfront Planning.
* Qualcuno approva o rifiuta una richiesta di Workfront Planning inviata dall&#39;utente.
* Lo stato viene modificato in una richiesta di Workfront Planning sottomessa.

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
<p>L’istanza di Workfront della tua organizzazione deve essere integrata in Adobe Unified Experience.</p> 
<p>Gli utenti dell’organizzazione ricevono notifiche da Workfront Planning solo quando l’organizzazione è integrata in Adobe Unified Experience. </p>
<p>Per ulteriori informazioni, vedere <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Esperienza unificata Adobe per Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licenza Adobe Workfront*</p></td> 
   <td><p><p>Standard, Light o Contributor
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
   <td> <p>A tutti gli utenti, inclusi gli amministratori di Workfront, deve essere assegnato un modello di layout che includa l'area Planning nel menu principale. </p> </td> 
  </tr> 
</tbody> 
</table>

*Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

Per ulteriori informazioni sulle notifiche di Workfront Planning, vedere anche i seguenti articoli:

* Per informazioni sui commenti sui record, vedere [Gestisci commenti record](/help/quicksilver/planning/records/manage-record-comments.md).
* Per informazioni sulle notifiche in-app da Workfront Planning, vedere [Gestire le notifiche in-app per Adobe Workfront Planning](/help/quicksilver/planning/notifications/manage-planning-in-app-notifications.md).
* Per informazioni sulle notifiche e-mail da Workfront Planning, vedere [Gestire le notifiche e-mail per Adobe Workfront Planning](/help/quicksilver/planning/notifications/manage-planning-email-notifications.md).


## Gestire le preferenze di notifica

1. Accedi a Workfront con le credenziali Adobe Experience Cloud.
1. Fai clic sull&#39;icona del menu **account** ![icona del menu Account in Experience Cloud](assets/account-menu-icon-on-experience-cloud.png) in alto a destra dello schermo, quindi fai clic su **Preferenze**.
1. Nella sezione **Notifiche** fare clic su **Workfront**.
1. Seleziona le notifiche che desideri ricevere.
Oppure
Deseleziona le notifiche che desideri interrompere la ricezione.

   ![Pannello notifiche Adobe Experience Cloud per Workfront Planning](assets/adobe-experience-cloud-notifications-panel-for-workfront-planning.png)
1. Per Workfront sono disponibili le seguenti notifiche:

   * **Riferimenti**: si riceve una notifica quando un utente assegna un tag a te o al tuo team in un commento in Workfront Planning
   * **Richieste**: ricevi una notifica quando qualcuno effettua una delle seguenti operazioni:

      * Richiede o concede l&#39;autorizzazione per un oggetto Workfront Planning
      * Hai inviato una richiesta di Workfront Planning
      * Lo stato di una richiesta di Workfront Planning inviata è cambiato
      * Richiede, concede o rifiuta un&#39;approvazione per una richiesta di Workfront Planning

   Per ulteriori informazioni sulla gestione delle notifiche, vedere [Preferenze account e notifiche](https://experienceleague.adobe.com/en/docs/core-services/interface/features/account-preferences).

<!--OLD: notifications are not available to non-IMS customers: 

When someone adds you to a comment in the record page, you may receive an in-app as well as an email notification about the comment. 

The following scenarios exist:   

* Adobe Unified Experience customers receive both an in-app notification and an email notification. They can manage their in-app and email notification preferences in the Preferences area of their Adobe Experience Cloud profile for the Workfront product. 

    For more information, see [Account preferences and notifications](https://experienceleague.adobe.com/en/docs/core-services/interface/features/account-preferences).

* Customers who are not on the Adobe Unified Experience receive only an email notification. They cannot manage their email notifications preferences and will always receive an email when someone adds them to a comment on a record in Workfront Planning.   

-->
