---
title: Condividi aree di lavoro
description: Puoi condividere un’area di lavoro con altri utenti per garantire la collaborazione quando lavori in Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 475a519d-d3bd-4461-8099-0e296d556d34
source-git-commit: 11b72c797203dcf364281665bc60cf67d25c8b5d
workflow-type: tm+mt
source-wordcount: '898'
ht-degree: 3%

---

# Condividere le aree di lavoro

<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo i rilasci mensili in Produzione, le stesse funzioni sono disponibili nell’ambiente di Produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedere [Abilitare o disabilitare le versioni rapide per l&#39;organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Puoi condividere un’area di lavoro con altri utenti per garantire la collaborazione quando lavori in Adobe Workfront Planning.

<!--
This article describes how you can share a view with others. For information about requesting, granting, or denying permissions to a view, see [Request permissions to a view or a workspace](/help/quicksilver/planning/access/request-permissions.md). -->

>[!NOTE]
>
>La concessione di autorizzazioni a un&#39;area di lavoro non consente ad altri utenti di concedere autorizzazioni per le visualizzazioni nelle pagine dei tipi di record. È necessario concedere autorizzazioni alle singole visualizzazioni in una pagina di tipo record per condividerle con altri utenti. Per informazioni, vedere [Condividere una visualizzazione](/help/quicksilver/planning/access/share-views.md).


## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo. 

<!--at GA, check that the Workfront plans article linked below has Planning info-->

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Pacchetto Adobe Workfront</p></td> 
   <td> 
<p>Qualsiasi pacchetto Workfront e Planning</p> 
Oppure
<p>Qualsiasi pacchetto di Workflow e Planning</p> 
 </tr>
<tr> 
   <td role="rowheader"><p>Licenza di Adobe Workfront</p></td> 
   <td><p>Standard</p> 
  </td> 
  </tr>

<td role="rowheader"><p>Autorizzazioni sugli oggetti</p></td> 
   <td>  <p>Gestire le autorizzazioni per un’area di lavoro</p>  </td> 
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
<p>Your organization must be onboarded to the Adobe Unified Experience for users to be able to request and grant permissions to a workspace from a permission request. </p> 
<p>Users must be added to the Adobe Admin Console in order to gain permissions to Workfront Planning workspaces.</p>
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard </p>
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
   <td>  <p>Manage permissions to a workspace</p>  </td> 
  </tr> 

</tbody> 
</table> -->

## Considerazioni sulla condivisione delle aree di lavoro

* Per informazioni generali sulla condivisione di oggetti in Workfront Planning, vedere anche [Panoramica sulle autorizzazioni di condivisione in Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).
* Puoi condividere le aree di lavoro con utenti, team, ruoli, gruppi o aziende all’interno della tua organizzazione.
* Oltre a team, gruppi, aziende e ruoli, puoi condividere solo con gli utenti che sono stati aggiunti al Adobe Admin Console.
* Non è possibile condividere le aree di lavoro con utenti esterni all’organizzazione.
* Quando si condivide un&#39;area di lavoro, vengono condivisi anche tutti i tipi di record, i record e i campi associati alle aree di lavoro.
* Quando si condivide un&#39;area di lavoro, le visualizzazioni non vengono condivise. È necessario condividere le visualizzazioni separatamente.
* Le autorizzazioni di Workspace vengono visualizzate come autorizzazioni ereditate per i tipi di record.

## Condividere le autorizzazioni per un’area di lavoro

I seguenti utenti possono condividere un’area di lavoro con altri utenti:

* Gli amministratori di sistema possono condividere tutte le aree di lavoro, incluse quelle che non hanno creato.
* Tutti gli altri utenti possono condividere solo le aree di lavoro per le quali dispongono delle autorizzazioni di gestione.

Per condividere un’area di lavoro con altri utenti:

{{step1-to-planning}}

1. Apri l&#39;area di lavoro che desideri condividere, quindi fai clic su **Condividi** nell&#39;angolo superiore destro dello schermo. Viene visualizzata la casella Condivisione (Sharing).

   ![Pulsante Condividi nell&#39;area di lavoro in alto a destra](assets/share-button-on-workspace-top-right.png)


   <!--For Feb 26:1. <span class="preview">(Conditional) Depending on your access level, the following scenarios exist: </span>

      * <span class="preview">If you are a System Administrator, select from the following options:</span>

         <div class="preview">

         * **Only invited people can access**: You must select entities in the sharing box and choose their access to the workspace. This is the default selection. 
         * **Everyone in the system can view**: Everyone in the system with access to Planning can view the workspace in their **Workspaces** area in Planning.
         
         </div> 
         
      * <span class="preview">If you are a workspace manager with a Standard license, you can see one of the following selections but you cannot change them:</span>

         <div class="preview">
         
         * **Only invited people can access**
         * **Everyone in the system can view**
         
         </div>-->

1. Nel campo **Concedi l&#39;accesso a questa area di lavoro**, inizia a digitare il nome di un utente, un gruppo, un team, una società o una mansione e fai clic su di esso quando viene visualizzato nell&#39;elenco. <!--update screen shot at the release of system-wide permissions for workspaces-->

   ![Interfaccia utente condivisa con i gruppi](assets/sharing-ui-with-groups.png)

   >[!NOTE]
   >
   >* Oltre a team, gruppi, aziende e ruoli, puoi condividere solo con gli utenti che sono stati aggiunti al Adobe Admin Console. Non è possibile aggiungere utenti solo Workfront. Per informazioni, vedere [Gestione degli utenti in Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).
   >
   >* Quando condividi un&#39;area di lavoro con un utente, nel campo vengono visualizzati anche la mansione principale <span class="preview"> e l&#39;e-mail</span>. Per poter visualizzare l&#39;e-mail dell&#39;utente, è necessario che l&#39;impostazione Visualizza informazioni di contatto sia abilitata per l&#39;oggetto Users nel proprio livello di accesso.

1. Seleziona uno dei seguenti livelli di autorizzazione dal menu a discesa:
   * Visualizzazione
   * Contribuisci
   * Gestione

     Per informazioni sui livelli di autorizzazione e sulle azioni che gli utenti possono eseguire per ogni livello, vedere [Panoramica sulle autorizzazioni di condivisione in Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).
1. Fai clic su **Copia collegamento** per copiare un collegamento nell&#39;area di lavoro negli Appunti.
1. Condividi il collegamento copiato con altri utenti. Per poter accedere all’area di lavoro, gli utenti che ricevono il collegamento devono essere utenti attivi e accedere a Workfront.
1. Fai clic su **Salva**.

   Gli utenti che hanno condiviso l’area di lavoro con ricevono una notifica in-app e una notifica e-mail relativa alle autorizzazioni di accesso.

## Concedere autorizzazioni a un’area di lavoro da una richiesta di autorizzazione

Gli utenti che accedono a un collegamento a un’area di lavoro per la quale non dispongono di autorizzazioni possono richiedere le autorizzazioni per l’area di lavoro. Tutti gli utenti con autorizzazioni Gestisci per l&#39;area di lavoro ricevono la richiesta di autorizzazione e possono concedere o negare le autorizzazioni.

1. (Condizionale) Se sei il manager di un’area di lavoro, potresti ricevere una richiesta da un altro utente per accedere alla vista nelle seguenti aree:

   * Una notifica in-app
     ![Notifica in-app per la richiesta di accesso](assets/in-app-notification-for-access-request.png)
   * Una notifica e-mail
     ![Notifica e-mail per la richiesta di accesso](assets/email-notification-for-access-request.png)
1. (Condizionale) Dall’area di notifica in Workfront, fai clic sulla notifica in-app.
Oppure
Dalla notifica e-mail, fai clic su **Visualizza tutte le notifiche**, quindi fai clic sulla notifica nell&#39;elenco.

   Viene visualizzata la casella **Richieste di accesso in sospeso**.

   ![Casella di approvazione elenco notifiche](assets/notifications-list-approval-box.png)

1. (Facoltativo) Per l’utente di cui desideri approvare le autorizzazioni, seleziona una delle seguenti opzioni dal menu a discesa a destra del nome dell’utente:
   * **Visualizza**
   * **Contribuisci**
   * **Gestisci**
1. Selezionare l&#39;utente per il quale si desidera approvare o negare l&#39;autorizzazione, quindi fare clic su **Approva tutto** o **Rifiuta tutto**.
1. Fai clic sulla freccia rivolta a sinistra a sinistra di **Richieste di accesso in sospeso**, quindi fai clic su **Salva**.

   Se hai approvato la richiesta, gli utenti vengono aggiunti alla casella di condivisione dell’area di lavoro. L’utente che richiede l’autorizzazione riceve una conferma via e-mail che la sua richiesta è stata approvata. <!--will they also get an in-app notification??-->


## Rimuovere le autorizzazioni per un’area di lavoro


{{step1-to-planning}}

1. Apri l&#39;area di lavoro a cui vuoi rimuovere le autorizzazioni, quindi fai clic su **Condividi** nell&#39;angolo superiore destro dello schermo.
1. Fai clic sul menu a discesa a destra del nome di un&#39;entità con cui stai condividendo l&#39;area di lavoro, quindi fai clic su **Rimuovi**.
1. Fai clic su **Salva**.

   Gli utenti rimossi non hanno più accesso al workspace o ai relativi oggetti.

   Agli utenti rimossi dall’accesso all’area di lavoro non viene notificato di non disporre più di queste autorizzazioni.