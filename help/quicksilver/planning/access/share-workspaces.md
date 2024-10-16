---
title: Condividi aree di lavoro
description: Puoi condividere un’area di lavoro con altri utenti per garantire la collaborazione quando lavori in Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 475a519d-d3bd-4461-8099-0e296d556d34
source-git-commit: 9debb7c6d9df0f9f4962f3e66f146e5f605d20f0
workflow-type: tm+mt
source-wordcount: '724'
ht-degree: 2%

---

# Condividere le aree di lavoro

{{planning-important-intro}}

Puoi condividere un’area di lavoro con altri utenti per garantire la collaborazione quando lavori in Adobe Workfront Planning.

<!--
This article describes how you can share a view with others. For information about requesting, granting, or denying permissions to a view, see [Request permissions to a view or a workspace](/help/quicksilver/planning/access/request-permissions.md). -->

>[!NOTE]
>
>La concessione di autorizzazioni a un&#39;area di lavoro non consente ad altri utenti di concedere autorizzazioni per le visualizzazioni nelle pagine dei tipi di record. È necessario concedere autorizzazioni alle singole visualizzazioni in una pagina di tipo record per condividerle con altri utenti. Per informazioni, vedere [Condividere una visualizzazione](/help/quicksilver/planning/access/share-views.md).


## Requisiti di accesso

+++ Espandere per visualizzare i requisiti di accesso per Workfront Planning.

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
   <td role="rowheader"><p>Piano di pianificazione Adobe Workfront*</p></td> 
   <td> 
<p>Qualsiasi </p> 
<p>Per ulteriori informazioni su quanto incluso in ogni piano di Workfront Planning, contattare l'account manager Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Piattaforma Adobe Workfront</p></td> 
   <td> 
<p>Per poter accedere a tutte le funzionalità di Workfront Planning, l’istanza di Workfront della tua organizzazione deve essere integrata in Adobe Unified Experience.</p>
<p>Per consentire agli utenti di richiedere e concedere autorizzazioni per un’area di lavoro da una richiesta di autorizzazione, la tua organizzazione deve essere integrata nell’esperienza unificata di Adobe. </p> 
<p>Per ulteriori informazioni, vedere <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Esperienza unificata di Adobe per Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licenza Adobe Workfront*</p></td> 
   <td><p> Standard </p>
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
   <td>  <p>Gestire le autorizzazioni per un’area di lavoro</p>  </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modello di layout</p></td> 
   <td> <p>A tutti gli utenti, inclusi gli amministratori di Workfront, deve essere assegnato un modello di layout che includa l'area Planning nel menu principale. </p> </td> 
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
   <td> <p>Manage permissions to a workspace</p>  
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



## Condividere le autorizzazioni per un’area di lavoro

I seguenti utenti possono condividere un’area di lavoro con altri utenti:

* Gli amministratori di sistema possono condividere tutte le aree di lavoro, incluse quelle che non hanno creato.
* Tutti gli altri utenti possono condividere solo le aree di lavoro per le quali dispongono delle autorizzazioni di gestione.

Per condividere un’area di lavoro con altri utenti:

{{step1-to-planning}}

1. Apri l&#39;area di lavoro che desideri condividere, quindi fai clic su **Condividi** nell&#39;angolo superiore destro dello schermo.

   ![](assets/share-button-on-workspace-top-right.png)

1. Nel campo **Concedi l&#39;accesso all&#39;area di lavoro a**, inizia a digitare il nome di un utente o di un gruppo, quindi fai clic su di esso quando viene visualizzato nell&#39;elenco.

   ![](assets/sharing-ui-with-groups.png)

1. Seleziona uno dei seguenti livelli di autorizzazione dal menu a discesa:
   * Visualizza
   * Contribuisci
   * Gestire

     Per informazioni sui livelli di autorizzazione e sulle azioni che gli utenti possono eseguire per ogni livello, vedere [Panoramica sulle autorizzazioni di condivisione in Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).
1. Fai clic su **Copia collegamento** per copiare un collegamento nell&#39;area di lavoro negli Appunti.
1. Condividi il collegamento copiato con altri utenti. Per poter accedere all’area di lavoro, gli utenti che ricevono il collegamento devono essere utenti attivi e accedere a Workfront.
1. Fai clic su **Salva**.

## Concedere autorizzazioni a un’area di lavoro da una richiesta di autorizzazione

Gli utenti che accedono a un collegamento a un’area di lavoro per la quale non dispongono di autorizzazioni possono richiedere le autorizzazioni per l’area di lavoro. Tutti gli utenti con autorizzazioni Gestisci per l&#39;area di lavoro ricevono la richiesta di autorizzazione e possono concedere o negare le autorizzazioni.

1. (Condizionale) Se sei il manager di un’area di lavoro, potresti ricevere una richiesta da un altro utente per accedere alla vista nelle seguenti aree:

   * Una notifica in-app
     ![](assets/in-app-notification-for-access-request.png)
   * Una notifica e-mail
     ![](assets/email-notification-for-access-request.png)
1. (Condizionale) Dall’area di notifica in Workfront, fai clic sulla notifica in-app.
Oppure
Dalla notifica e-mail, fai clic su **Visualizza tutte le notifiche**, quindi fai clic sulla notifica nell&#39;elenco.

   Viene visualizzata la casella **Richieste di accesso in sospeso**.

   ![](assets/notifications-list-approval-box.png)

1. (Facoltativo) Per l’utente di cui desideri approvare le autorizzazioni, seleziona una delle seguenti opzioni dal menu a discesa a destra del nome dell’utente:
   * **Visualizza**
   * **Contribute**
   * **Gestisci**
1. Selezionare l&#39;utente per il quale si desidera approvare o negare l&#39;autorizzazione, quindi fare clic su **Approva tutto** o **Rifiuta tutto**.
1. Fai clic sulla freccia rivolta a sinistra a sinistra di **Richieste di accesso in sospeso**, quindi fai clic su **Salva**.

   Se hai approvato la richiesta, gli utenti vengono aggiunti alla casella di condivisione dell’area di lavoro. L’utente che richiede l’autorizzazione riceve una conferma via e-mail che la sua richiesta è stata approvata. <!--will they also get an in-app notification??-->


## Rimuovere le autorizzazioni per un’area di lavoro


{{step1-to-planning}}

1. Apri l&#39;area di lavoro a cui vuoi rimuovere le autorizzazioni, quindi fai clic su **Condividi** nell&#39;angolo superiore destro dello schermo.
1. Fai clic sul menu a discesa a destra del nome di un utente o di un gruppo, quindi fai clic su **Rimuovi**.
1. Fai clic su **Salva**.

   L&#39;utente o gli utenti che appartengono al gruppo rimosso non hanno più accesso al workspace o ai relativi oggetti.
