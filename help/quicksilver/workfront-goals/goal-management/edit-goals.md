---
product-previous: workfront-goals
navigation-topic: goal-management
title: Modificare gli obiettivi in Obiettivi di Adobe Workfront
description: Puoi modificare gli obiettivi esistenti da qualsiasi periodo di tempo e in qualsiasi stato.
author: Alina
feature: Workfront Goals
exl-id: 74db534c-6897-40c2-bea9-a9d30a40f61c
source-git-commit: d7dd5ab4e3041a100b13c5bf169747f58db0ea39
workflow-type: tm+mt
source-wordcount: '631'
ht-degree: 1%

---

# Modificare gli obiettivi in Obiettivi di Adobe Workfront

Puoi modificare gli obiettivi esistenti da qualsiasi periodo di tempo e in qualsiasi stato.

## Requisiti di accesso

Devi avere i seguenti:

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> 
   <p>Per il nuovo piano e la nuova struttura delle licenze:
  <ul><li>Un piano Ultimate </li></ul>
   </p>
<p>Per il piano corrente e la struttura delle licenze: 
<ul><li> A Pro o superiore </li>
  <li>Una licenza Adobe Workfront Goals oltre a una licenza Workfront.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Licenza Adobe Workfront*</td>
 <td>
 <p>Nuova licenza: Collaboratore o versione successiva</p>
 Oppure
 <p>Licenza corrente: richiesta o successiva</p> <p>Per ulteriori informazioni, vedere <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Panoramica delle licenze di Adobe Workfront</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Prodotto*</td>
 <td>
 <p> Nuovo requisito del prodotto, uno dei seguenti: </p>
<ul>
<li>Un piano Select o Prime Adobe Workfront e un’ulteriore licenza Adobe Workfront Goals.</li>
<li>Un piano Workfront Ultimate che include gli obiettivi Workfront per impostazione predefinita. </li></ul>
 <p>Oppure</p>
 <p>Fabbisogno di prodotto corrente: un piano Workfront e una licenza aggiuntiva per gli obiettivi Adobe Workfront. </p> <p>Per informazioni, vedere <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requisiti per l'utilizzo degli obiettivi di Workfront</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Livello di accesso</td>
 <td> <p>Modifica accesso agli obiettivi</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Autorizzazioni oggetto</td>
 <td>
  <div>
  <p>Visualizza o autorizzazioni superiori per l’obiettivo per visualizzarlo</p>
  <p>Gestire le autorizzazioni per l’obiettivo per modificarlo</p>
  <p>Per informazioni sulla condivisione degli obiettivi, vedere <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Condividere un obiettivo in Obiettivi di Workfront</a>. </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>Modello di layout</p></td>
   <td> <p>A tutti gli utenti, inclusi gli amministratori di Workfront, deve essere assegnato un modello di layout che includa l’area Obiettivi nel menu principale. </p>  
</td>
  </tr>
</tbody>
</table>

*Per ulteriori informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **menu principale**, quindi fai clic su **Obiettivi**.\
   Viene visualizzato un elenco di obiettivi.
1. Fai clic su un obiettivo.\
   Viene visualizzata la pagina dell’obiettivo.

   ![](assets/goal-page-unshimmed.png)

1. Per modificare le informazioni per l&#39;obiettivo, effettuate una delle seguenti operazioni:
   * Fai clic sui campi visualizzati nell’intestazione dell’obiettivo per aggiornarli. Non tutti i campi nell’intestazione sono modificabili.
   * Fai clic sull&#39;icona **Altro** ![](assets/more-icon.png) a destra del nome dell&#39;obiettivo, quindi fai clic su **Modifica**.
   * Fai clic su **Dettagli obiettivo** nel pannello a sinistra, quindi fai clic sull&#39;icona **Modifica** ![](assets/edit-icon.png) in alto a destra, quindi fai clic su **Modifica tutto**. Inizia ad aggiornare i campi nella sezione Dettagli obiettivo.

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
