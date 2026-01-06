---
product-previous: workfront-goals
navigation-topic: goal-management
title: Modificare gli obiettivi in Obiettivi di Adobe Workfront
description: Puoi modificare gli obiettivi esistenti da qualsiasi periodo di tempo e in qualsiasi stato.
author: Alina
feature: Workfront Goals
exl-id: 74db534c-6897-40c2-bea9-a9d30a40f61c
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '563'
ht-degree: 3%

---

# Modificare gli obiettivi in Obiettivi di Adobe Workfront

<!--Audited for P&P only: 10/2025-->

Puoi modificare gli obiettivi esistenti da qualsiasi periodo di tempo e in qualsiasi stato.

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
 <tr>
 <td role="rowheader">Adobe Workfront license*</td>
 <td>
 <p>New license: Contributor or higher</p>
 Or
 <p>Current license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Product*</td>
 <td>
  <p> New product requirement: Workfront</p>
 <p>Or</p>
  <p>Current product requirement: In addition to a Workfront license, you must purchase a license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
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

## Considerazioni sulla modifica degli obiettivi

* Non è possibile modificare gli obiettivi con lo stato Chiuso.
* Puoi modificare gli obiettivi da qualsiasi periodo di tempo.

  Per un obiettivo passato, puoi modificare le seguenti informazioni:

   * Nome
   * Periodo temporale
   * Stato

     >[!TIP]
     >
     >Se l&#39;obiettivo è Chiuso, la riapertura ricalcola la percentuale di completamento dell&#39;avanzamento. Non è possibile modificare un obiettivo chiuso.

   * Descrizione
   * Risultati e attività

## Modifica obiettivi

<!--
Editing goals differs depending on what environment you use.

### Edit goals in the Production environment

1. Go to a goal that you want to edit and click the goal name to open the **Goal Details** panel. 
1. Click the **More icon** ![More icon](assets/more-icon.png), then click **Edit**.

   ![Edit goal](assets/edit-goal-highlighted.png)

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

{{step1-to-goals}}

Viene visualizzato un elenco di obiettivi.

1. Fai clic su un obiettivo.\
   Viene visualizzata la pagina dell’obiettivo.

   ![Pagina obiettivo](assets/goal-page-unshimmed.png)

1. Per modificare le informazioni per l&#39;obiettivo, effettuate una delle seguenti operazioni:
   * Fai clic sui campi visualizzati nell’intestazione dell’obiettivo per aggiornarli. Non tutti i campi nell’intestazione sono modificabili.
   * Fai clic sull&#39;icona **Altro** ![Altro icona](assets/more-icon.png) a destra del nome dell&#39;obiettivo, quindi fai clic su **Modifica**.
   * Fai clic su **Dettagli obiettivo** nel pannello a sinistra, quindi fai clic sull&#39;icona **Modifica** ![Modifica](assets/edit-icon.png) nell&#39;angolo superiore destro, quindi fai clic su **Modifica tutto**. Inizia ad aggiornare i campi nella sezione Dettagli obiettivo.

     >[!IMPORTANT]
     >
     >Non tutti i campi visualizzati nelle aree sopra indicate possono essere modificati. In Workfront alcuni campi vengono calcolati e sono di sola lettura.

1. (Condizionale) A seconda di quanto selezionato nel passaggio precedente, aggiorna le seguenti informazioni sull’obiettivo:

   * Aggiorna le seguenti informazioni nell’intestazione dell’obiettivo, quindi premi Invio per salvare le modifiche:
      * **Nome obiettivo**: fare clic sul nome dell&#39;obiettivo e iniziare a digitare un nuovo nome.
      * **Proprietario**: fare clic sul nome del proprietario e iniziare a digitare il nome di un utente, team, gruppo o società, quindi selezionarlo quando viene visualizzato nell&#39;elenco. Puoi avere un solo proprietario per un obiettivo.
   * Aggiorna le seguenti informazioni nella casella Modifica obiettivo, quindi fai clic su **Salva**:
      * **Nome obiettivo**
      * **Periodo**: fare clic per aggiornare il periodo di tempo per l&#39;obiettivo\
        Oppure\
        Seleziona **Abilita date personalizzate** per specificare le date di **Inizio** e **Fine** dell&#39;obiettivo.

        >[!TIP]
        >
        >Deseleziona **Abilita date personalizzate** per tornare al periodo di tempo originale per l&#39;obiettivo.

      * **Proprietario obiettivo**
      * **Descrizione**: aggiungi o aggiorna le informazioni sull&#39;obiettivo.
   * Aggiorna o rivedi le informazioni nella sezione Dettagli obiettivo. Per ulteriori informazioni, consulta [Aggiornare gli obiettivi nella sezione Dettagli obiettivo in Obiettivi di Adobe Workfront](../goal-management/update-goals-in-goal-details-panel.md).

   <!-- (should you update the title here after changing it at production??? - change it to Update goals in the goal Details section)-->

1. (Facoltativo) Fai clic su **Indicatori di avanzamento** nel pannello a sinistra per aggiungere risultati, attività o progetti all&#39;obiettivo. Aggiungendo gli indicatori di progresso, potrai tenere traccia dell’avanzamento dell’obiettivo.
Per ulteriori informazioni, consulta i seguenti articoli:
   * [Aggiungere attività agli obiettivi in Obiettivi di Adobe Workfront](../results-and-activities/add-activities-to-goals.md)
   * [Aggiungi risultati agli obiettivi in Obiettivi di Adobe Workfront](../results-and-activities/add-results-to-goals.md).
   * [Aggiungi progetti agli obiettivi in Obiettivi di Adobe Workfront](../results-and-activities/connect-projects-to-goals-overview.md).

</div>
