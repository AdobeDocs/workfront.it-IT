---
title: Approvare una richiesta in Adobe Workfront Planning
description: Quando un utente invia una richiesta a un modulo di richiesta associato a un’approvazione in Adobe Workfront Planning, gli approvatori ricevono una notifica e un messaggio e-mail relativi all’approvazione in sospeso. È necessario approvare la richiesta prima che Workfront Planning crei un oggetto.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 9b5ba629fa2f50f0425f4afbfd4faa891d917845
workflow-type: tm+mt
source-wordcount: '945'
ht-degree: 1%

---


# Approvare una richiesta in Adobe Workfront Planning

<!--take Preview and Production references at Production time-->

<!-- do you need to add that only workspace owners can view the Submitted/ Planning tab?? - asking team in slack-->

<span class="preview">Le informazioni contenute in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo i rilasci mensili in Produzione, le stesse funzioni sono disponibili nell’ambiente di Produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedere [Abilitare o disabilitare le versioni rapide per l&#39;organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Quando un utente invia una richiesta a un modulo di richiesta associato a un’approvazione in Adobe Workfront Planning, gli approvatori ricevono una notifica e un messaggio e-mail relativi all’approvazione in sospeso. È necessario approvare la richiesta prima che Workfront Planning crei un oggetto.

In questo articolo viene descritto come un responsabile dell&#39;area di lavoro può approvare una richiesta inviata per la creazione di un record in Workfront Planning.

Si consiglia inoltre di visualizzare i seguenti articoli:

* [Creazione e gestione di un modulo di richiesta in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md)
* [Inviare richieste di Adobe Workfront Planning per creare record](/help/quicksilver/planning/requests/submit-requests.md)
* [Aggiungere un’approvazione a un modulo di richiesta](/help/quicksilver/planning/requests/add-approval-to-request-form.md)

## Considerazioni sull’approvazione delle richieste e sugli stati delle richieste

Le richieste inviate vengono visualizzate nella scheda Pianificazione della sezione Inviate dell&#39;area Richieste di Workfront con uno dei seguenti stati di richiesta:

* **Revisione in sospeso**: questo stato viene visualizzato quando nessuno degli approvatori ha aperto l&#39;oggetto della richiesta.
* **In revisione**: lo stato **In attesa di revisione** diventa **In revisione** quando almeno un approvatore apre l&#39;oggetto della richiesta. Lo stato della richiesta rimane **In revisione** fino a quando tutti gli approvatori non avranno approvato la richiesta.
* **Approvato**: quando un approvatore approva l&#39;oggetto della richiesta, il suo stato individuale diventa **Approvato**, ma lo stato complessivo dell&#39;oggetto rimane **In revisione** fino a quando tutti gli approvatori non avranno preso le loro decisioni. Quando tutti gli approvatori approvano una richiesta, lo stato diventa **Approvato**.
* **Completato**: se tutti gli approvatori approvano l&#39;oggetto della richiesta, lo stato cambia in **Completato** oppure se la richiesta non ha bisogno di un&#39;approvazione.
* **Rifiutato**: se un approvatore rifiuta l&#39;oggetto della richiesta, lo stato diventa **Rifiutato**. Non viene creato alcun record ed è necessario inviare una nuova richiesta per creare il record.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

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
<p>Per ulteriori informazioni su quanto incluso in ogni piano di Workfront Planning, contattare l'account manager Workfront. </td>

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
   <td>
   <p>Standard</p>
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
   <td>
   <ul>
   <li><p>Gestire le autorizzazioni per un’area di lavoro</p></li>
    <li><p>Gli amministratori di sistema possono gestire le aree di lavoro che non hanno creato. </p></li>
    </ul>
   <p>Per informazioni sulle autorizzazioni di condivisione per gli oggetti di Workfront Planning, vedere  
   <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">Panoramica delle autorizzazioni di condivisione in Adobe Workfront Planning</a> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Modello di layout</p></td>
   <td> <p>A tutti gli utenti, inclusi gli amministratori di Workfront, deve essere assegnato un modello di layout che includa l'area Planning nel menu principale. </p>  
</td>
  </tr>
 </tbody>
</table>

*Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Approvare una richiesta per creare un record

Dopo che gli utenti aggiungono richieste a un modulo di richiesta di tipo record associato a un’approvazione, la richiesta viene inviata agli approvatori.

Gli approvatori ricevono le seguenti notifiche relative a una richiesta in attesa di approvazione:

* Una notifica in-app
* Una notifica e-mail

>[!NOTE]
>
>Per consentire agli utenti di ricevere notifiche e-mail e in-app, l’istanza di Workfront della tua organizzazione deve essere integrata in Adobe Unified Experience.

Per approvare una richiesta:

1. Esegui una delle operazioni seguenti:

   * Se hai accesso a Workfront Planning e puoi visualizzare almeno un&#39;area di lavoro, fai clic su **Menu principale** ![](assets/dots-menu.png) nell&#39;angolo superiore destro dello schermo o sul **Menu principale** ![](assets/lines-menu.png) nell&#39;angolo superiore sinistro, se disponibile, quindi fai clic su **Richieste** > **Inviate** > **Pianificazione** e fai clic sulla richiesta con lo stato di **Revisione in sospeso** o **In revisione**.

     >[!TIP]
     >
     >Se non disponi dell’accesso a Workfront Planning o se non disponi dell’accesso per visualizzare alcuna area di lavoro, puoi accedere a una richiesta per approvarla solo utilizzando l’e-mail o le notifiche in-app.

   * Fai clic sull&#39;icona ![](assets/notifications-area-icon-unified-shell.png) dell&#39;area **Notifiche** nell&#39;angolo superiore destro della schermata e fai clic sulla notifica di una richiesta in attesa della tua approvazione per aprire la richiesta.
   * Vai alla notifica e-mail nell&#39;e-mail che ti notifica una richiesta in attesa della tua approvazione, quindi fai clic su **Apri richiesta** per aprire la richiesta. <!--add the name of the button here, from the email-->

   La pagina della richiesta si apre in modalità di sola lettura.

   ![](assets/read-only-reqeust-page-in-review-status.png)

1. (Facoltativo) Fai clic sull&#39;icona **Approvazioni** ![](assets/approvals-icon.png) nell&#39;angolo superiore destro della richiesta per visualizzare gli approvatori.
1. Fai clic su **Rivedi e approva**, quindi scegli una delle seguenti opzioni: <!--did they fix the button and removed the &??-->

   * **Approva**: questa operazione approva la richiesta. Viene creato immediatamente un record per il tipo di record associato al modulo di richiesta dopo che tutti gli approvatori hanno approvato la richiesta.
   * **Rifiuta**: la richiesta viene rifiutata anche se l&#39;utente è l&#39;unico approvatore a rifiutarla. Non viene creato alcun record per il tipo di record associato al modulo di richiesta.

   L’utente che ha inviato la richiesta riceve un’e-mail e una notifica in un’app quando la richiesta viene approvata o rifiutata.

   Lo stato della richiesta cambia in base alla decisione di approvazione:

   * **Completato**: la richiesta è approvata.
   * **Rifiutata**: richiesta rifiutata.

   La richiesta rimane nella scheda Pianificazione della sezione Inviata nell&#39;area Richieste di Workfront.

