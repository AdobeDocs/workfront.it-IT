---
product-previous: workfront-goals
navigation-topic: workfront-goals-settings
title: Condividere un obiettivo in Obiettivi di Workfront
description: Quando condividi un obiettivo, assegna le autorizzazioni di gestione a un obiettivo a un utente che non lo ha creato.
author: Alina
feature: Workfront Goals
exl-id: 747449cf-9092-4b9f-9add-db2e7d3fab48
source-git-commit: afc2124a7fd0d9d52c04be1c174fdba314beec7a
workflow-type: tm+mt
source-wordcount: '754'
ht-degree: 2%

---

# Condividere un obiettivo in Obiettivi di Adobe Workfront

Quando condividi un obiettivo, assegna le autorizzazioni di gestione a un obiettivo a un utente che non lo ha creato.

## Requisiti di accesso

<!--drafted - replace the table below with this one when P&P releases: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
  <tr>
   <td role="rowheader">Adobe Workfront plan*</td>
   <td>
   <p>Current plan: Select or higher</p>
   Or
   <p>Legacy plan: Pro or higher</p>
   
   </td>
  </tr>
  <tr>
   <td role="rowheader">Adobe Workfront license*</td>
   <td>
   <p>Current license: Contributor or higher</p>
   Or
   <p>Legacy license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Product</td>
   <td>
   <p> Current product requirement: If you have the Select or Prime Adobe Workfront plan, you must also buy an additional Adobe Workfront Goals license.  Workfront Goals are included in the Ultimate Workfront Plan.</p>
   Or
   <p>Legacy product requirement: You must purchase an additional license for the Adobe Workfront Goals to access functionality described in this article. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
  </tr>
  <tr>
   <td role="rowheader">Access level*</td>
   <td> <p>Edit access to Goals</p> <p><b>NOTE</b><p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see:</p>
     <ul>
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a> </p> </li>
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Grant access to Adobe Workfront Goals</a></span> </p> </li>
     </ul> </p> </td>
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
 </tbody>
</table>
-->

Devi disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Pro o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Richiesta o superiore</p> <p>Per ulteriori informazioni, consulta <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Panoramica sulle licenze di Adobe Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td> <p>Devi acquistare una licenza aggiuntiva per la funzionalità Obiettivi di Adobe Workfront per accedere alla descritta in questo articolo. </p> <p>Per informazioni, consulta <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requisiti per l'utilizzo degli obiettivi di Workfront</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modificare l’accesso a Obiettivi o versioni successive</p> <p><b>NOTA</b><p>Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta:</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Concedere l’accesso agli obiettivi di Adobe Workfront</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> 
    <div> 
     <p>Gestione delle autorizzazioni per l'obiettivo</p> 
     <p>Per informazioni sulla condivisione degli obiettivi, vedi <a href="#" class="MCXref xref selected">Condividere un obiettivo in Obiettivi di Workfront</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*Per sapere quale piano, tipo di licenza o accesso si dispone, contattare l&#39;amministratore Workfront.

## Prerequisiti

Prima di iniziare, è necessario disporre dei seguenti elementi:

* Modello di layout che include l’area Obiettivi del menu principale.

## Considerazioni sulla condivisione degli obiettivi

* Gli utenti possono disporre delle seguenti autorizzazioni per un obiettivo:

   <table style="table-layout:auto"> 
   <col> 
   </col> 
   <col> 
   </col> 
   <tbody> 
   <tr> 
      <td role="rowheader"><p><b>Autorizzazioni per gli obiettivi</b></p></td> 
      <td>
      <p><b>Descrizione</b></p> </td> 
   </tr> 
   <tr> 
      <td role="rowheader"><p>Visualizza</p></td> 
      <td>
      <p>Gli utenti dispongono delle autorizzazioni necessarie per visualizzare l’obiettivo, ma non possono modificare le informazioni relative all’obiettivo, non possono aggiungere o modificare informazioni per risultati o attività, aggiornare lo stato o eliminare l’obiettivo.</p>      
      <p>Per impostazione predefinita, tutti gli utenti con accesso a Obiettivi possono visualizzare tutti gli obiettivi nel sistema. Gli utenti possono copiare l’obiettivo se hanno accesso a Modifica obiettivi nel loro livello di accesso.</p> </td> 
   </tr> 
   <tr> 
      <td role="rowheader"><p>Gestisci</p></td> 
      <td> <p>Gli utenti possono modificare tutte le informazioni per l’obiettivo, inclusi i risultati, o le attività, compresa l’eliminazione.</p> 
      <p>Solo i creatori di obiettivi o gli utenti ai quali sono state assegnate autorizzazioni di gestione a un obiettivo possono gestire un obiettivo.</p> 
      Solo gli utenti con autorizzazioni di gestione per un obiettivo possono condividere l'obiettivo con altri per assegnare loro le autorizzazioni di gestione per l'obiettivo. </p> </td> 
   </tr> 
   </tbody> 
   </table>

* Puoi condividere con altri i seguenti tipi di obiettivi:

   * Un obiettivo creato
   * Un obiettivo creato da un altro utente a cui sono state assegnate le autorizzazioni per la gestione.

* Se disponi di autorizzazioni di gestione per un obiettivo, puoi modificare le autorizzazioni per l’obiettivo per il creatore di obiettivo. Per impostazione predefinita, dispongono delle autorizzazioni di gestione quando creano l&#39;obiettivo, ma puoi modificarne le autorizzazioni in Visualizza.

## Condividere un obiettivo

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) > **Obiettivi** nell&#39;angolo in alto a destra.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../workfront-goals-settings/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   Viene visualizzato l’Elenco obiettivi.

1. Fai clic sul nome di un obiettivo nell’elenco. Viene visualizzata la pagina dell’obiettivo.

1. Fai clic sul pulsante **Icona Altro** accanto al nome dell&#39;obiettivo, quindi fai clic su **Condividi**.

   ![](assets/more-menu-highlighted-goal-details-panel-with-share-link-350x156.png)

   Viene visualizzata la casella Accesso obiettivo.

   ![](assets/goal-access-sharing-box-manage-system-wide-deselected-350x400.png)

1. Esegui una delle operazioni seguenti:

   * Seleziona la **Gestione a livello di sistema** impostazione per assegnare le autorizzazioni Manage a tutti gli utenti del sistema che hanno accesso Edit to Goals nel loro livello di accesso. Questa opzione è deselezionata per impostazione predefinita per tutti i nuovi obiettivi.
   * Inizia a digitare il nome di un utente a cui desideri assegnare le autorizzazioni di gestione nel **Assegna a Gestisci l&#39;accesso a** scatola. Selezionare il nome quando viene visualizzato nell&#39;elenco.

      >[!TIP]
      >
      >Puoi condividere un obiettivo solo con altri utenti. Non puoi condividere obiettivi con gruppi, team o con la tua azienda.

1. Fai clic su **Condividi**.

   L&#39;obiettivo viene condiviso con gli utenti specificati. Un’etichetta &quot;a livello di sistema&quot; o il nome degli utenti che dispongono delle autorizzazioni di gestione per l’obiettivo vengono visualizzati nel campo Accesso alla gestione nel pannello Dettagli obiettivo .

## Opzioni di autorizzazione per l’obiettivo

Nella tabella seguente sono elencate le autorizzazioni che puoi concedere quando condividi un obiettivo. Per ulteriori informazioni sull&#39;accesso che gli utenti ottengono in base alla propria licenza, vedi [Concedere l’accesso agli obiettivi di Adobe Workfront](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).

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
   <td> <p>Visualizza risultati o attività</p> </td> 
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
   <td>Modificare risultati o attività</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Aggiungi risultati o attività per l’obiettivo</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Associa un progetto come attività all’obiettivo**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Elimina obiettivo</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Eliminare risultati o attività</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>Scollegare progetti dall'obiettivo</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

*È necessario disporre dell&#39;accesso Modifica agli obiettivi nel livello di accesso per poter convertire i risultati e le attività in obiettivi.

**Per visualizzarli è necessario disporre dell’autorizzazione Visualizza progetti e Visualizza progetti aggiunti o che si desidera aggiungere all’obiettivo.

Per informazioni sul livello di accesso al progetto, consulta [Concedere l’accesso ai progetti](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

Per informazioni sulle autorizzazioni del progetto, consulta [Condivisione di un progetto in Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

 
