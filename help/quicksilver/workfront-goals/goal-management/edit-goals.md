---
product-previous: workfront-goals
navigation-topic: goal-management
title: Modificare gli obiettivi in Obiettivi di Adobe Workfront
description: Puoi modificare gli obiettivi esistenti da qualsiasi periodo di tempo e in qualsiasi stato.
author: Alina
feature: Workfront Goals
exl-id: 74db534c-6897-40c2-bea9-a9d30a40f61c
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 1%

---

# Modificare gli obiettivi in Obiettivi di Adobe Workfront

Puoi modificare gli obiettivi esistenti da qualsiasi periodo di tempo e in qualsiasi stato.

## Requisiti di accesso

<!--drafted - for P&P releases: 

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
   <td> <p>Modificare l’accesso a Obiettivi o versioni successive</p> <p><b>NOTA</b>

<p>Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta:</p> 
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
     <p>Per informazioni sulla condivisione degli obiettivi, vedi <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Condividere un obiettivo in Obiettivi di Workfront</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*Per sapere quale piano, tipo di licenza o accesso si dispone, contattare l&#39;amministratore Workfront.

## Prerequisiti

È necessario disporre dei seguenti elementi prima di poter iniziare:

* Modello di layout che include l’area Obiettivi del menu principale.
* Hai creato gli obiettivi che desideri modificare oppure disponi delle autorizzazioni di gestione per tali obiettivi.

## Considerazioni sulla modifica degli obiettivi

* Non è possibile modificare gli obiettivi con lo stato Chiuso.
* Puoi modificare gli obiettivi da qualsiasi periodo di tempo.

   È possibile modificare le seguenti informazioni per un obiettivo precedente:

   * Nome
   * Periodo di tempo
   * Stato

      >[!TIP]
      >
      >Se l&#39;obiettivo è Chiuso, riaprirlo ricalcola percentuale di avanzamento completato. Non è possibile modificare un obiettivo chiuso.

   * Descrizione
   * Risultati e attività

## Modificare gli obiettivi

<!--
Editing goals differs depending on what environment you use.

### Edit goals in the Production environment

1. Go to a goal that you want to edit and click the goal name to open the **Goal Details** panel. 
1. Click the **More icon** ![](assets/more-icon.png), then click **Edit**.

   ![](assets/edit-goal-highlighted.png)

1. Update the name of the goal in the **Goal** field. 
1. Select a time period when the goal should be completed.

   Select from the following predefined options:

   * The current year
   * The quarters of the current year
   * The next two years
   * The quarters of the next two years

   Or

   Click **Define custom dates** to select a custom time frame. 

1. (Conditional) Select a start and an end date for your goal, if you clicked **Define custom dates**.

   
   <p>(NOTE: these fields don't yet have a name) </p>
   

   >[!CAUTION]
   >
   >You cannot create a goal with custom dates in the past.

1. (Optional) Click **Reset custom dates** to return to the predefined options.

   >[!TIP]
   >
   >We recommend that everyone in your organization selects the same time frames for similar goals or goals that are aligned. This provides better alignment between goals and ensures that everyone's work supports your larger organization-wide strategy.

1. Click the **Owner** field and select a new owner for the goal, if you want to indicate someone else as the owner of the goal. 
1. (Conditional) Start typing the name of a user, team, group, or the name of your organization in the **Owner** field, then select it when it displays in the list. You can have only one owner for a goal. 
1. Update the **Description** of the goal, then click **Save**.

-->

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png), quindi fai clic su **Obiettivi**.\
   Viene visualizzato un elenco di obiettivi.
1. Fai clic su un obiettivo.\
   Viene visualizzata la pagina dell’obiettivo.

   ![](assets/goal-page-unshimmed.png)

1. Effettua una delle seguenti operazioni per modificare le informazioni per l’obiettivo:
   * Fai clic sui campi che vengono visualizzati nell’intestazione dell’obiettivo per aggiornarli. Non tutti i campi nell’intestazione sono modificabili.
   * Fai clic sul pulsante **Icona Altro** ![](assets/more-icon.png) a destra del nome dell&#39;obiettivo, quindi fai clic su **Modifica**.
   * Fai clic su **Dettagli obiettivo** nel pannello a sinistra e fai clic su **Icona Modifica** ![](assets/edit-icon.png) nell&#39;angolo in alto a destra, quindi fai clic su **Modifica tutto**. Inizia ad aggiornare i campi nella sezione Dettagli obiettivo .

      >[!IMPORTANT]
      >
      >Non è possibile modificare tutti i campi visualizzati nelle aree sopra menzionate. Workfront calcola alcuni campi e sono di sola lettura.

1. (Condizionale) A seconda di quanto selezionato nel passaggio precedente, aggiorna le seguenti informazioni sull’obiettivo:

   * Aggiorna le seguenti informazioni nell&#39;intestazione dell&#39;obiettivo, quindi premi Invio per salvare le modifiche:
      * **Nome dell&#39;obiettivo**: Fare clic sul nome dell&#39;obiettivo e iniziare a digitare un nuovo nome.
      * **Proprietario**: Fai clic sul nome del proprietario e inizia a digitare il nome di un utente, di un team, di un gruppo o della società, quindi selezionalo quando viene visualizzato nell’elenco. Puoi avere un solo proprietario per un obiettivo.
   * Aggiornare le seguenti informazioni nella casella Modifica obiettivo, quindi fare clic su **Salva**:
      * **Nome obiettivo**
      * **Punto**: Fai clic su per aggiornare il periodo di tempo per l&#39;obiettivo\
         Oppure\
         Seleziona **Abilita date personalizzate** per specificare le date dell&#39;obiettivo **Inizio** e **Date di fine**.

         >[!TIP]
         >
         >Deseleziona **Abilita date personalizzate** per tornare al periodo di tempo originale per l&#39;obiettivo.

      * **Proprietario obiettivo**
      * **Descrizione**: Aggiungi o aggiorna informazioni sull&#39;obiettivo.
   * Aggiorna o rivedi le informazioni nella sezione Dettagli obiettivo . Per ulteriori informazioni, consulta [Aggiornare gli obiettivi nella sezione Dettagli obiettivo in Obiettivi di Adobe Workfront](../goal-management/update-goals-in-goal-details-panel.md).

   <!-- (should you update the title here after changing it at production??? - change it to Update goals in the goal Details section)-->

1. (Facoltativo) Fai clic su **Indicatori di avanzamento** nel pannello a sinistra per aggiungere risultati, attività o progetti all’obiettivo. Aggiungendo degli indicatori di avanzamento, potrai tenere traccia dell’avanzamento dell’obiettivo.
Per ulteriori informazioni, consulta i seguenti articoli:
   * [Aggiungere attività agli obiettivi in Obiettivi di Adobe Workfront](../results-and-activities/add-activities-to-goals.md)
   * [Aggiungere risultati agli obiettivi in Obiettivi di Adobe Workfront](../results-and-activities/add-results-to-goals.md).
   * [Aggiungere progetti agli obiettivi in Obiettivi di Adobe Workfront](../results-and-activities/connect-projects-to-goals-overview.md).

</div>
