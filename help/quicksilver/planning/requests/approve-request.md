---
title: Approvare una richiesta in Adobe Workfront Planning
description: Quando un utente invia una richiesta a un modulo di richiesta associato a un’approvazione in Adobe Workfront Planning, gli approvatori ricevono una notifica e un messaggio e-mail relativi all’approvazione in sospeso. È necessario approvare la richiesta prima che Workfront Planning crei un oggetto.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: aca9b313-3420-43f6-8f6c-dd74888bd120
source-git-commit: 66d59467e7e9857ca5573b819d51da839ddbd4f7
workflow-type: tm+mt
source-wordcount: '1103'
ht-degree: 1%

---

# Approvare una richiesta in Adobe Workfront Planning

<!--take Preview and Production references at Production time-->

<!-- do you need to add that only workspace owners can view the Submitted/ Planning tab?? - asking team in slack-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Quando un utente invia una richiesta a un modulo di richiesta associato a un’approvazione in Adobe Workfront Planning, gli approvatori ricevono una notifica e un messaggio e-mail relativi all’approvazione in sospeso. È necessario approvare la richiesta prima che Workfront Planning crei un oggetto.

In questo articolo viene descritto come un responsabile dell&#39;area di lavoro può approvare una richiesta inviata per la creazione di un record in Workfront Planning.

Si consiglia inoltre di visualizzare i seguenti articoli:

* [Creazione e gestione di un modulo di richiesta in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md)
* [Inviare richieste di Adobe Workfront Planning per creare record](/help/quicksilver/planning/requests/submit-requests.md)
* [Aggiungere un’approvazione a un modulo di richiesta](/help/quicksilver/planning/requests/add-approval-to-request-form.md)

## Considerazioni sull’approvazione delle richieste

* Le richieste inviate vengono visualizzate nell’area Richieste di Workfront con uno dei seguenti stati di richiesta:

   * **Revisione in sospeso**: questo stato viene visualizzato quando nessuno degli approvatori ha aperto l&#39;oggetto della richiesta.
   * **In revisione**: lo stato **In attesa di revisione** diventa **In revisione** quando almeno un approvatore apre l&#39;oggetto della richiesta. Lo stato della richiesta rimane **In revisione** fino a quando tutti gli approvatori non avranno approvato la richiesta.
   * **Approvato**: quando un approvatore approva l&#39;oggetto della richiesta, il suo stato individuale diventa **Approvato**, ma lo stato complessivo dell&#39;oggetto rimane **In revisione** fino a quando tutti gli approvatori non avranno preso le loro decisioni. Quando tutti gli approvatori approvano una richiesta, lo stato diventa **Approvato**.
   * **Completato**: se tutti gli approvatori approvano l&#39;oggetto della richiesta, lo stato cambia in **Completato** oppure se la richiesta non ha bisogno di un&#39;approvazione.
   * **Rifiutato**: se un approvatore rifiuta l&#39;oggetto della richiesta, lo stato diventa **Rifiutato**. Non viene creato alcun record ed è necessario inviare una nuova richiesta per creare il record.

* È possibile visualizzare le informazioni sull&#39;approvazione in un record creato inviando un modulo di richiesta nei campi Approvato da e Data approvata. Per informazioni, vedere [Creare i campi](/help/quicksilver/planning/fields/create-fields.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Pacchetti Adobe Workfront</p></td> 
   <td> 
<p>Qualsiasi pacchetto Workfront e qualsiasi pacchetto Planning</p>
Oppure
<p>Qualsiasi pacchetto del flusso di lavoro e qualsiasi pacchetto Planning</p>
<p>Per ulteriori informazioni su ciò che è incluso in ogni pacchetto Workfront Planning, contattare il rappresentante del proprio account Workfront.</p>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Licenza Adobe Workfront</p></td> 
   <td><p>Qualsiasi</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorizzazioni oggetto</p></td> 
   <td>   <p>Gestione delle autorizzazioni per un'area di lavoro e tipo di record</a> </p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p>  </td> 
  </tr>  
</tbody> 
</table>

Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Approvare una richiesta per creare un record

Dopo che gli utenti aggiungono richieste a un modulo di richiesta di tipo record associato a un’approvazione, la richiesta viene inviata agli approvatori.

Gli approvatori ricevono le seguenti notifiche relative a una richiesta in attesa di approvazione:

* Una notifica in-app
* Una notifica e-mail

>[!NOTE]
>
>Per consentire agli utenti di ricevere notifiche e-mail e in-app, l’istanza di Workfront della tua organizzazione deve essere integrata in Adobe Unified Experience.

È possibile approvare le richieste per la creazione di record dalla richiesta stessa, <span class="preview">o dal widget Approvazioni personali nella Home.</span>

* [Approvare una richiesta dalla richiesta in Workfront Planning](#approve-a-request-from-the-request-in-workfront-planning)
* [Approvare una richiesta dal widget Le mie approvazioni nella Home](#approve-a-request-from-the-my-approvals-widget-in-home)

### Approvare una richiesta dalla richiesta in Workfront Planning

1. (Condizionale) Se utilizzi l’esperienza di richiesta legacy in Workfront, apri la richiesta effettuando una delle seguenti operazioni:

   * Se hai accesso a Workfront Planning e puoi visualizzare almeno un&#39;area di lavoro, fai clic su **Main Menu** ![Dots main menu](assets/dots-menu.png) nell&#39;angolo superiore destro della schermata o sul **Main Menu** ![Lines main menu](assets/lines-menu.png) nell&#39;angolo superiore sinistro, se disponibile, quindi fai clic su **Requests** > **Submitted** > **Planning** e fai clic sulla richiesta con lo stato di **Pending review** o **In review**.

     >[!TIP]
     >
     >Se non disponi dell’accesso a Workfront Planning o se non disponi dell’accesso per visualizzare alcuna area di lavoro, puoi accedere a una richiesta per approvarla solo utilizzando l’e-mail o le notifiche in-app.

   * Fai clic sull&#39;icona dell&#39;area **Notifications** ![Notifications area icon in Unified Shell](assets/notifications-area-icon-unified-shell.png) nell&#39;angolo superiore destro della schermata e fai clic sulla notifica relativa a una richiesta in attesa della tua approvazione per aprire la richiesta.
   * Vai alla notifica e-mail nell&#39;e-mail che ti notifica una richiesta in attesa della tua approvazione, quindi fai clic su **Apri richiesta** per aprire la richiesta. <!--add the name of the button here, from the email-->

   La pagina della richiesta si apre in modalità di sola lettura.

   ![Pagina richiesta di sola lettura in stato di revisione](assets/read-only-reqeust-page-in-review-status.png)
1. Se utilizzi la nuova esperienza di richiesta in Workfront, fai clic su **Menu principale** ![Menu principale punti](assets/dots-menu.png) nell&#39;angolo superiore destro dello schermo o sul **Menu principale** ![Menu principale righe](assets/lines-menu.png) nell&#39;angolo superiore sinistro, se disponibile, quindi fai clic su **Richieste** e fai clic sulla richiesta che desideri approvare con lo stato di **Revisione in sospeso**.
1. (Facoltativo) Fai clic sull&#39;icona **Approvazioni** ![Approvazioni](assets/approvals-icon.png) nell&#39;angolo superiore destro della richiesta per visualizzare gli approvatori.
1. Fai clic su **Rivedi e approva**, quindi scegli una delle seguenti opzioni:

   * **Approva**: questa operazione approva la richiesta. Viene creato immediatamente un record per il tipo di record associato al modulo di richiesta dopo che tutti gli approvatori hanno approvato la richiesta.
   * **Rifiuta**: la richiesta viene rifiutata anche se l&#39;utente è l&#39;unico approvatore a rifiutarla. Non viene creato alcun record per il tipo di record associato al modulo di richiesta.

   L’utente che ha inviato la richiesta riceve un’e-mail e una notifica in un’app quando la richiesta viene approvata o rifiutata.

   Lo stato della richiesta cambia in base alla decisione di approvazione:

   * **Completato**: la richiesta è approvata.
   * **Rifiutata**: richiesta rifiutata.

   La richiesta rimane nell’area Richieste di Workfront.

<div class="preview">

### Approvare una richiesta dal widget Le mie approvazioni nella Home

1. Fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon.png) nell&#39;angolo superiore destro di Adobe Workfront oppure, se disponibile, fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) nell&#39;angolo superiore sinistro, quindi fai clic su **[!UICONTROL Home]**.

   Oppure

   Fai clic sull&#39;icona [!UICONTROL Home] ![Home icon](/help/_includes/assets/home-icon-30x29.png) nell&#39;angolo superiore sinistro di Adobe Workfront, quindi individua il widget Approvazioni personali.

1. Individuare l&#39;oggetto che si desidera approvare o rifiutare.

1. (Facoltativo) Per aggiungere un commento, fai clic sulla freccia a discesa accanto a Approva o Rifiuta, digita la nota e fai clic su Aggiungi.

1. Scegliere una delle opzioni seguenti:

   * **Approva**: questa operazione approva la richiesta. Viene creato immediatamente un record per il tipo di record associato al modulo di richiesta dopo che tutti gli approvatori hanno approvato la richiesta.
   * **Rifiuta**: la richiesta viene rifiutata anche se l&#39;utente è l&#39;unico approvatore a rifiutarla. Non viene creato alcun record per il tipo di record associato al modulo di richiesta.

   L’utente che ha inviato la richiesta riceve un’e-mail e una notifica in un’app quando la richiesta viene approvata o rifiutata.

   Lo stato della richiesta cambia in base alla decisione di approvazione:

   * **Completato**: la richiesta è approvata.
   * **Rifiutata**: richiesta rifiutata.

</div>
