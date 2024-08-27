---
title: Condividi visualizzazioni
description: È possibile condividere una visualizzazione con altri utenti per garantire la collaborazione quando si utilizza Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 673dd888-3135-48b0-8198-c8d6d6706ddf
source-git-commit: c497276579c5d70c29fe961e43356e1ae603262d
workflow-type: tm+mt
source-wordcount: '1200'
ht-degree: 1%

---


# Condividere le visualizzazioni

{{planning-important-intro}}

È possibile condividere una visualizzazione con altri utenti per garantire la collaborazione durante l&#39;utilizzo dei record in Adobe Workfront Planning.

>[!IMPORTANT]
>
>* La concessione di autorizzazioni a un&#39;area di lavoro non consente ad altri utenti di concedere autorizzazioni per le visualizzazioni nelle pagine dei tipi di record. È necessario concedere autorizzazioni alle singole visualizzazioni in una pagina di tipo record per condividerle con altri utenti.
>
>* La concessione delle autorizzazioni a una visualizzazione non modifica le autorizzazioni per la visualizzazione dei record. Le autorizzazioni per i record vengono concesse condividendo le aree di lavoro.
>
>* Quando si condivide una visualizzazione, si concedono ad altri utenti le autorizzazioni necessarie per accedere a tutti gli elementi della visualizzazione. Ad esempio, quando si assegnano le autorizzazioni Gestione a una visualizzazione, è possibile modificare il raggruppamento, il filtro, l&#39;ordinamento o l&#39;aspetto della barra.


Potete condividere una vista con le seguenti entità:

* Internamente, con utenti e gruppi di Workfront
* Pubblicamente, con utenti esterni a Workfront

<!--
This article describes how you can share a view with others. For information about requesting, granting, or denying permissions to a view, see [Request permissions to a view or a workspace](/help/quicksilver/planning/access/request-permissions.md). -->

## Requisiti di accesso

+++ Espandere per visualizzare i requisiti di accesso per Workfront Planning.

<!--at GA, check that the Workfront plans article linked below has Planning info-->

Per accedere a Workfront Planning, è necessario disporre dei seguenti elementi:

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
   <td role="rowheader"><p>Piano di pianificazione Adobe Workfront*</p></td> 
   <td> 
<p>Qualsiasi </p> 
<p>Per ulteriori informazioni su ciò che è incluso in ogni piano di Workfront Planning, vedere <a href="https://business.adobe.com/products/workfront/pricing.html">Determinazione prezzi e packaging di Adobe Workfront</a>. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Piattaforma Adobe Workfront</p></td> 
   <td> 
<p>Per poter accedere a tutte le funzionalità di Workfront Planning, l’istanza di Workfront della tua organizzazione deve essere integrata in Adobe Unified Experience.</p> 
<p>Per ulteriori informazioni, vedere <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Esperienza unificata di Adobe per Workfront</a>. </p> 
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
   <td>  <p>Gestire le autorizzazioni per una visualizzazione</p>  
   <p>Solo gli utenti con le autorizzazioni di gestione di un’area di lavoro possono condividere una visualizzazione pubblicamente.</p></td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modello di layout</p></td> 
   <td> <p>A tutti gli utenti, inclusi gli amministratori di Workfront, deve essere assegnato un modello di layout che includa l'area Planning nel menu principale. </p> </td> 
  </tr> 
</tbody> 
</table>

*Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<!--OLD: 

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
   <p> Adobe Workfront</p> </td>
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
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p>
   Or
   <p>Current: Plan </p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> There are no access controls for Adobe Workfront Planning</p>  
</td>
  </tr>

  <tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a view</p>  
   <p>Only users with Manage permissions to a workspace can share a view publicly.</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Planning area in the Main Menu. </p> <p>For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p> 
</td>
  </tr>
 </tbody>
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).-->

+++

## Considerazioni durante la condivisione delle visualizzazioni

* È possibile assegnare le autorizzazioni Visualizzazione o Gestione a una visualizzazione agli utenti interni di Workfront.

* Gli utenti con le autorizzazioni Gestione possono modificare le impostazioni di visualizzazione, condividerle, duplicarle o eliminarle.

* Puoi condividere le visualizzazioni con persone esterne all’organizzazione tramite un collegamento pubblico.

* Quando condividi pubblicamente una visualizzazione, il collegamento è accessibile a chiunque non faccia parte della tua azienda per un periodo di tempo limitato, indicato dalla data di scadenza. Non è necessario effettuare l&#39;accesso per visualizzare la visualizzazione condivisa.

* Gli utenti esterni all&#39;organizzazione che dispongono dell&#39;accesso a una visualizzazione non possono creare altre visualizzazioni, modificare la visualizzazione condivisa o aggiungere, eliminare o modificare le informazioni del record nella visualizzazione.

## Condivisione interna delle autorizzazioni per una visualizzazione

Puoi condividere con utenti o gruppi in Workfront le viste che hai creato o le viste per le quali disponi delle autorizzazioni di gestione.

>[!NOTE]
>
>Gli amministratori di sistema non possono visualizzare o condividere viste che non hanno creato personalmente. Possono accedere o condividere solo le visualizzazioni condivise con loro.
>
>Gli amministratori di sistema possono disporre solo delle autorizzazioni di gestione per una visualizzazione.

{{step1-to-planning}}

1. Aprire l&#39;area di lavoro di cui si desidera condividere la visualizzazione, quindi fare clic su una scheda del tipo di record.

   Verrà aperta la pagina del tipo di record.

1. Dalla scheda Visualizza, passa il puntatore del mouse sulla visualizzazione da condividere e fai clic sul menu **Altro** ![](assets/more-menu.png) a destra del nome della visualizzazione, quindi fai clic su **Condividi**.

   ![](assets/more-menu-for-views-expanded-with-share-option.png)

   La scheda **Condivisione interna** deve essere selezionata per impostazione predefinita.

1. (Facoltativo) Nell&#39;area **Chi ha accesso**, selezionare una delle opzioni seguenti:

   * **L&#39;accesso è consentito solo alle persone invitate**: è necessario specificare gli utenti o i gruppi con cui si desidera condividere la visualizzazione. Questa è l&#39;opzione predefinita.
   * **Tutti gli utenti nell&#39;area di lavoro possono visualizzare**: tutti gli utenti che dispongono di autorizzazioni di visualizzazione o di livello superiore per le aree di lavoro possono accedere alla visualizzazione.

1. Nel campo **Concedi l&#39;accesso in visualizzazione a**, inizia a digitare il nome di un utente o di un gruppo, quindi fai clic su di esso quando viene visualizzato nell&#39;elenco.

   ![](assets/sharing-a-view-ui-with-groups.png)

1. Seleziona uno dei seguenti livelli di autorizzazione dal menu a discesa:
   * Visualizza
   * Gestire

     Per informazioni sui livelli di autorizzazione e sulle azioni che gli utenti possono eseguire per ogni livello, vedere [Panoramica sulle autorizzazioni di condivisione in Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

     Gli amministratori di sistema ricevono sempre le autorizzazioni di gestione per le visualizzazioni condivise con loro.

1. Fai clic su **Copia collegamento** per copiare un collegamento negli Appunti.
1. Fai clic su **Salva**.

   La visualizzazione viene aggiornata con l&#39;icona persone ![](assets/view-shared-with-others-people-icon.png) per indicare che la visualizzazione è ora condivisa con altri utenti.

   >[!TIP]
   >
   >Le visualizzazioni senza un utente o un&#39;icona globale sono visualizzazioni create dall&#39;utente e non sono condivise con altri utenti. Le viste non condivise sono visibili solo a te.

1. Condividi il collegamento copiato con altri utenti. Gli utenti che ricevono il collegamento devono essere utenti attivi e accedere a Workfront per poter accedere alla pagina del tipo di record e visualizzarla nella visualizzazione selezionata.

## Condivisione pubblica delle autorizzazioni per una visualizzazione

Puoi condividere le viste create o le viste per le quali disponi delle autorizzazioni di gestione con persone che non dispongono di una licenza Workfront e che potrebbero essere esterne alla tua organizzazione.

>[!IMPORTANT]
>
>Solo gli utenti con le autorizzazioni Gestione di un&#39;area di lavoro possono condividere pubblicamente le visualizzazioni dell&#39;area di lavoro.


Per condividere una visualizzazione pubblicamente in Workfront Planning:

{{step1-to-planning}}

1. Aprire l&#39;area di lavoro di cui si desidera condividere la visualizzazione, quindi fare clic su una scheda del tipo di record.

   Verrà aperta la pagina del tipo di record.

1. Dalla scheda Visualizza, passa il puntatore del mouse sulla visualizzazione da condividere e fai clic sul menu **Altro** ![](assets/more-menu.png) a destra del nome della visualizzazione, quindi fai clic su **Condividi**.

   ![](assets/more-menu-for-views-expanded-with-share-option.png)

1. Fai clic su **Condivisione pubblica**.

   ![](assets/public-sharing-tab-for-views.png)

1. Abilita l&#39;impostazione **Crea collegamento pubblico**.

   È disponibile un collegamento. Questo è un link pubblico. Quando è condiviso, chiunque disponga del collegamento, incluse persone esterne all&#39;organizzazione, può accedere alla pagina del tipo di record e visualizzare record e campi nella pagina.

1. Fai clic sull&#39;icona **Copia collegamento** ![](assets/copy-link-view.png) per copiare il collegamento negli Appunti.

1. Immetti manualmente una data o utilizza il calendario nel campo **Data di scadenza collegamento** per selezionare una data di scadenza per il collegamento pubblico. La visualizzazione della pagina record non sarà accessibile dopo la data selezionata.

1. Fai clic su **Salva**.

   La visualizzazione viene aggiornata con l&#39;icona globale ![](assets/public-shared-view-icon-highlighted.png) per indicare che è condivisa pubblicamente.

   >[!TIP]
   >
   >Le visualizzazioni senza un utente o un&#39;icona globale sono visualizzazioni create dall&#39;utente e non sono condivise con altri utenti. Le viste non condivise sono visibili solo a te.


1. (Facoltativo) Incolla il collegamento copiato in un messaggio e-mail, chat, documento o in un commento di Workfront per condividerlo con altri utenti.

<!--
## Grant permissions to a view from a permission request

Users who access a link to a view to which they do not have permissions can request permissions to the view. All users with Manage permissions to the view receive the permission request and can grant or deny the permissions. 

1. (Conditional) If you are are the manager of a view, you might receive a request from another user to access the view in the following areas:
   
   * An in-app notification
      ![](assets/in-app-notification-for-access-request-for-view.png)
   * An email notification
      ![](assets/in-app-notification-for-access-request-for-view.png)
1. (Conditional) From the notification area in Workfront, click the in-app notification
   Or
   From the email notification, click **View all notifications**, then click the notification in the list.

   The **Pending access requests** box displays. 

      ![](assets/notifications-list-approval-box.png)
1. Select the user for whom you want to approve or deny the permission, then click **Approve all** or **Deny all**. 
1. Click the left-pointing arrow to the left of **Pending access requests**, then click **Save**.

   If you approved the request, the users are added to the sharing box of the view. 
-->

## Rimuovere le autorizzazioni per una visualizzazione

{{step1-to-planning}}

1. Aprire l&#39;area di lavoro di cui si desidera interrompere la condivisione della visualizzazione, quindi fare clic su una scheda del tipo di record. Verrà aperta la pagina del tipo di record.
1. Passa il puntatore del mouse sul nome della scheda della visualizzazione da cui vuoi rimuovere la condivisione e fai clic sul menu **Altro** ![](assets/more-menu.png), quindi fai clic su **Condividi**.
1. Per rimuovere la condivisione interna di una vista, eseguire le operazioni seguenti:

   1. Verificare che la scheda **Condivisione interna** sia selezionata.
   1. Individuare l&#39;utente o il gruppo da rimuovere, espandere il menu a discesa delle autorizzazioni a destra del nome dell&#39;utente o del gruppo, quindi fare clic su **Rimuovi**.

1. Per rimuovere la condivisione pubblica di una visualizzazione, eseguire le operazioni seguenti:

   1. Fare clic sulla scheda **Condivisione pubblica**.
   1. Deseleziona l&#39;opzione **Crea collegamento pubblico**.

1. Fai clic su **Salva**.

   Le persone non hanno più accesso alla visualizzazione. Agli utenti che sono stati rimossi dall’accesso alla vista non viene notificato che non dispongono più di questo accesso.
