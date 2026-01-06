---
product-previous: workfront-goals
navigation-topic: workfront-goals-settings
title: Condividere un obiettivo in Obiettivi di Workfront
description: Quando condividi un obiettivo, assegni le autorizzazioni di gestione a un obiettivo a chi non lo ha creato.
author: Alina
feature: Workfront Goals
exl-id: 747449cf-9092-4b9f-9add-db2e7d3fab48
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '724'
ht-degree: 9%

---

# Condividere un obiettivo in Obiettivi di Adobe Workfront

Quando condividi un obiettivo, assegni le autorizzazioni di gestione a un obiettivo a chi non lo ha creato.

## Requisiti di accesso

>[!NOTE]
>
>La tua azienda potrebbe scegliere di continuare a utilizzare gli obiettivi di Adobe Workfront se ha acquistato questo pacchetto in passato. Per ulteriori dettagli, rivolgiti al rappresentante del tuo account.
>
>Adobe Workfront Goals non è più disponibile per l’acquisto.

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo. 

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr>
  <td> <p>Pacchetto Adobe Workfront</p> </td> 
   <td> 
   <p>Adobe Workfront Ultimate</p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Licenza Adobe Workfront</td>
 <td>
 <p>Collaboratore o versione successiva</p>
<p>Richiedi o superiore</p></td>
 </tr>
  <tr>
 <td role="rowheader">Configurazione del livello di accesso</td>
 <td> <p>Modifica accesso agli obiettivi</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Autorizzazioni oggetto</td>
 <td>
  <div>
  <p>Visualizza o autorizzazioni superiori per l’obiettivo per visualizzarlo</p>
  <p>Gestire le autorizzazioni per l’obiettivo per modificarlo</p>
  </div> </td>
 </tr>
<tr>
   <td role="rowheader"><p>Modello layout</p></td>
   <td> <p>A tutti gli utenti, inclusi gli amministratori di sistema, deve essere assegnato un modello di layout che includa l'area Obiettivi nel menu principale. </p>  
</td>
  </tr>
</tbody>
</table>

Per ulteriori informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


<!--Old:

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> 
   <p>For the new plan and license structure:
  <ul><li>An Ultimate plan </li></ul>
   </p>
<p>For the current plan and license structure: 
<ul><li> A Pro or higher </li>
  <li>An Adobe Workfront Goals license in addition to a Workfront license.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront license*</td>
 <td>
 <p>New license: Contributor or higher</p>
 Or
 <p>Current license: Request or higher</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Product*</td>
 <td>
 <p> New product requirement, one of the following: </p>
<ul>
<li>A Select or Prime Adobe Workfront plan and an additional Adobe Workfront Goals license.</li>
<li>An Ultimate Workfront plan which includes Workfront Goals by default. </li></ul>
 <p>Or</p>
 <p>Current product requirement: A Workfront plan and an additional license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Access level</td>
 <td> <p>Edit access to Goals</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Object permissions</td>
 <td>
  <div>
  <p>View or higher permissions to the goal to view it</p>
  <p>Manage permissions to the goal to edit it</p>
  <p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Workfront Goals</a>. </p>
  </div> </td>
 </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Goals area in the Main Menu. </p>  
</td>
  </tr>
</tbody>
</table>-->

## Considerazioni sulla condivisione degli obiettivi

* Gli utenti possono disporre delle seguenti autorizzazioni per un obiettivo:

  <table style="table-layout:auto"> 
   <col> 
   </col> 
   <col> 
   </col> 
   <tbody> 
   <tr> 
      <td role="rowheader"><p><b>Autorizzazioni obiettivo</b></p></td> 
      <td>
      <p><b>Descrizione</b></p> </td> 
   </tr> 
   <tr> 
      <td role="rowheader"><p>Visualizzazione</p></td> 
      <td>
      <p>Gli utenti dispongono delle autorizzazioni per visualizzare l’obiettivo, ma non possono modificare le informazioni per l’obiettivo, né aggiungere o modificare informazioni per i risultati o per le attività, aggiornare lo stato o eliminare l’obiettivo.</p>      
      <p>Per impostazione predefinita, tutti gli utenti con accesso agli obiettivi possono visualizzare tutti gli obiettivi nel sistema. Gli utenti possono copiare l’obiettivo se dispongono dell’accesso di modifica per gli obiettivi nel proprio livello di accesso.</p> </td> 
   </tr> 
   <tr> 
      <td role="rowheader"><p>Gestione</p></td> 
      <td> <p>Gli utenti possono modificare tutte le informazioni per l’obiettivo, inclusi i risultati, o le attività, inclusa la loro eliminazione.</p> 
      <p>Solo i creatori o gli utenti di un obiettivo a cui sono state specificatamente assegnate le autorizzazioni di gestione possono gestire un obiettivo.</p> 
      Solo gli utenti con le autorizzazioni di gestione di un obiettivo possono condividere l’obiettivo con altri utenti in modo da assegnare loro le autorizzazioni di gestione per l’obiettivo. </p> </td> 
   </tr> 
   </tbody> 
   </table>

* Puoi condividere con altri i seguenti tipi di obiettivi:

   * Un obiettivo che hai creato
   * Obiettivo creato da un altro utente a cui sono state assegnate le autorizzazioni di gestione.

* Se disponi delle autorizzazioni di gestione per un obiettivo, puoi modificare le autorizzazioni sull’obiettivo per il creatore dell’obiettivo. Per impostazione predefinita, quando creano l’obiettivo dispongono delle autorizzazioni di gestione, ma è possibile modificarne le autorizzazioni in Visualizza.

## Condividere un obiettivo

{{step1-to-goals}}

Viene visualizzato l’elenco Obiettivo.

1. Fai clic sul nome di un obiettivo nell’elenco. Viene visualizzata la pagina dell’obiettivo.

1. Fai clic sull&#39;icona **Altro** accanto al nome dell&#39;obiettivo, quindi fai clic su **Condividi**.

   ![Altro menu](assets/more-menu-highlighted-goal-details-panel-with-share-link-350x156.png)

   Viene visualizzata la casella Accesso obiettivo (Goal Access).

   ![Accesso obiettivo](assets/goal-access-sharing-box-manage-system-wide-deselected-350x400.png)

1. Esegui una delle operazioni seguenti:

   * Selezionare l&#39;impostazione **Gestisci a livello di sistema** per assegnare le autorizzazioni di gestione a tutti gli utenti del sistema che dispongono dell&#39;accesso di modifica agli obiettivi nel proprio livello di accesso. Questa opzione è deselezionata per impostazione predefinita per tutti i nuovi obiettivi.
   * Inizia a digitare il nome di un utente a cui desideri assegnare le autorizzazioni di gestione nella casella **Concedi accesso di gestione a**. Seleziona il nome quando viene visualizzato nel’elenco.

     >[!TIP]
     >
     >Puoi condividere un obiettivo solo con altri utenti. Non puoi condividere gli obiettivi con gruppi, team o la tua azienda.

1. Fai clic su **Condividi**.

   L&#39;obiettivo viene condiviso con gli utenti specificati. Un’etichetta &quot;a livello di sistema&quot; o il nome degli utenti che dispongono delle autorizzazioni di gestione per l’obiettivo vengono visualizzati nel campo Accesso a gestione del pannello Dettagli obiettivo.

## Opzioni di autorizzazione per obiettivo

Nella tabella seguente sono elencate le autorizzazioni che è possibile concedere durante la condivisione di un obiettivo. Per ulteriori informazioni sull&#39;accesso degli utenti in base alla licenza, vedere [Concedere l&#39;accesso agli obiettivi di Adobe Workfront](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <thead> 
  <tr> 
   <th> <p><strong>Azioni</strong> </p> </th> 
   <th> <p><strong>Gestisci</strong> </p> </th> 
   <th> <p><strong>Visualizza</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Visualizza obiettivo</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Visualizzare risultati o attività</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>Copia obiettivo* </td> 
   <td>✓ </td> 
   <td>✓</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Convertire risultati o attività in altri obiettivi*</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Visualizza progetti aggiunti come attività** </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Modifica obiettivo</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Modifica risultati o attività</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Aggiungere risultati o attività per l’obiettivo</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Associa un progetto come attività all’obiettivo**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Elimina obiettivo</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Eliminare risultati o attività</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>Disconnetti progetti dall’obiettivo</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

*Per convertire i risultati e le attività in obiettivi, è necessario disporre dell’accesso di modifica per gli obiettivi nel proprio livello di accesso.

**Devi avere accesso a Visualizza progetti e alle autorizzazioni di visualizzazione per i progetti aggiunti o che desideri aggiungere all’obiettivo per visualizzarli.

Per informazioni sul livello di accesso al progetto, vedere [Concedere l&#39;accesso ai progetti](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

Per informazioni sulle autorizzazioni del progetto, vedere [Condividere un progetto in Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).


