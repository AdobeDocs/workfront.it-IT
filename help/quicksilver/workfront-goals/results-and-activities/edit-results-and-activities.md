---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Modificare risultati e attività in Obiettivi di Adobe Workfront
description: Dopo che l’amministratore di Adobe Workfront ti ha concesso l’accesso corretto agli Obiettivi di Adobe Workfront, puoi creare e modificare obiettivi, risultati e attività.
author: Alina
feature: Workfront Goals
exl-id: 922a05f9-2995-4401-a6d2-e5a331270fd3
source-git-commit: d7dd5ab4e3041a100b13c5bf169747f58db0ea39
workflow-type: tm+mt
source-wordcount: '763'
ht-degree: 1%

---

# Modificare risultati e attività in Obiettivi di Adobe Workfront

Dopo che l’amministratore di Adobe Workfront ti ha concesso l’accesso corretto agli Obiettivi di Adobe Workfront, puoi creare e modificare obiettivi, risultati e attività.

Per informazioni sulla creazione di obiettivi, risultati e attività, consulta i seguenti articoli:

* [Crea obiettivi in Obiettivi Adobe Workfront](../../workfront-goals/goal-management/create-goals.md)
* [Guida introduttiva ai risultati e alle attività negli Obiettivi di Adobe Workfront](../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md)
* [Aggiungi risultati agli obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/results-and-activities/add-results-to-goals.md)
* [Aggiungere attività agli obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/results-and-activities/add-activities-to-goals.md)

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
 <td role="rowheader"><p>Livello di accesso</p></td>
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

## Considerazioni durante la modifica di risultati e attività

<!--
According to Vazgen, access levels will add more considerations.)
-->

* Puoi modificare i risultati e le attività che appartengono agli obiettivi creati o che disponi delle autorizzazioni necessarie per gestire.
* Non è possibile modificare l’avanzamento di progetti connessi a obiettivi come attività da Obiettivi di Workfront. L’avanzamento dei progetti viene aggiornato al completamento delle attività nel progetto. Puoi rimuovere i progetti dall’obiettivo disconnettendoli. Per ulteriori informazioni, vedere la sezione &quot;Disconnetti progetti&quot; nell&#39;articolo [Rimuovere risultati, attività e progetti dagli obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/results-and-activities/remove-results-activities-from-goals.md).

  >[!NOTE]
  >
  >Se le seguenti informazioni sul progetto vengono aggiornate a livello di progetto, Workfront Goals le aggiorna automaticamente a livello di obiettivo:
  >
  >   
  >   
  >   * Proprietario progetto
  >   * Nome progetto
  >   * Percentuale di completamento progetto
  >   
  >   
  >Per informazioni sulla connessione dei progetti agli obiettivi, vedere [Aggiungere progetti agli obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).

* Puoi eliminare i risultati e le attività dagli obiettivi quando non sono più rilevanti per il loro avanzamento. Non è possibile recuperare i risultati e le attività eliminati. Per informazioni sull&#39;eliminazione di risultati e attività, vedere [Rimuovere risultati, attività e progetti dagli obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/results-and-activities/remove-results-activities-from-goals.md).
* Puoi modificare i risultati e le attività associate agli obiettivi da qualsiasi periodo di tempo, incluso il passato.
* La modifica dei risultati e delle attività ne aggiorna le impostazioni e non lo stato di avanzamento. È necessario aggiornare l’avanzamento dei risultati e delle attività. Per informazioni sull&#39;aggiornamento dell&#39;avanzamento di obiettivi, risultati e attività, vedere [Aggiornare l&#39;avanzamento dell&#39;obiettivo in Obiettivi di Adobe Workfront](../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md).

## Modifica risultati

<!--
Editing results differs depending on which environment you use.

### Edit results in the Production environment

1. Go to the goal for which you want to edit a result and click the goal name to open the **Goal Details** panel.
1. Click **Results**.
1. Click the **gear icon** ![](assets/settings-gear-icon.png) to the right of the result you want to edit.

   ![](assets/results-gear-icon-options-350x85.png)

1. Click **Edit** to edit the following information:

   | Field |Description|
   |---|---|
   | Name |The name of the result. |
   | Owner |The owner of result.  |
   | Value |How you measure the progress of the result. |
   | Initial |The original value of the result. |
   | Target |The desired value when the result is completed. |

1. Click **Save**.
-->


1. Fai clic sul **menu principale** ![](assets/main-menu-icon.png), quindi su **Obiettivi**.
1. Nell&#39;elenco Obiettivo fare clic sul nome di un obiettivo per aprire la pagina obiettivo.
1. Fai clic su **Indicatori di avanzamento** nel pannello a sinistra.
1. Selezionare un risultato nell&#39;elenco Indicatori di avanzamento e fare clic sull&#39;icona **Modifica** ![](assets/edit-icon.png).

   Viene visualizzata la casella Modifica risultato (Edit Result).

   ![](assets/edit-result-box-unshimmed.png)

1. Modifica le seguenti informazioni:
   * **Nome risultato**: nome del risultato. Utilizza un nome descrittivo che illustra il risultato da ottenere per completare l’obiettivo.
   * **Proprietario risultato**: proprietario del risultato. Il proprietario deve essere un utente Workfront attivo.
   * **Tipo di valore**: come misurare l&#39;avanzamento del risultato.
   * **Valore iniziale**: il valore originale del risultato.
   * **Valore di destinazione**: il valore desiderato al completamento del risultato.
Per ulteriori informazioni sui campi dei risultati, vedere [Aggiungere risultati agli obiettivi](../results-and-activities/add-results-to-goals.md).
1. Fai clic su **Salva**.

## Modifica attività

<!--
Editing activities differs depending on which environment you use.

### Edit activities in the Production environment

>[!TIP]
>
>You cannot edit the Activity Type after you saved an activity on a goal.

1. Go to the goal for which you want to edit an activity and click the goal name to open the **Goal Details** panel.
1. Click **Activities**.
1. Click the **gear icon** ![](assets/settings-gear-icon.png) to the right of the activity you want to edit .

   ![](assets/activities-gear-icon-options-350x84.png)

1. Click **Edit** to edit the following information:

   | Field |Description |
   |---|---|
   | Name |The name of the activity. |
   | Owner |The owner of activity.  |

1. Click **Save**.
-->

1. Fai clic sul **menu principale** ![](assets/main-menu-icon.png), quindi su **Obiettivi**.
1. Nell&#39;elenco Obiettivo fare clic sul nome di un obiettivo per aprire la pagina obiettivo.
1. Fai clic su **Indicatori di avanzamento** nel pannello a sinistra.
1. Selezionare un&#39;attività nell&#39;elenco Indicatori di avanzamento e fare clic sull&#39;icona **Modifica** ![](assets/edit-icon.png).

   Viene visualizzata la casella Modifica attività.

   ![](assets/edit-activity-box-unshimmed.png)

1. Modifica le seguenti informazioni:
   * **Nome attività**: nome dell&#39;attività. Utilizza un nome descrittivo che illustra l’attività da eseguire per indicare che l’obiettivo è stato completato.
   * **Proprietario attività:** Proprietario dell&#39;attività. Il proprietario deve essere un utente Workfront attivo.\
     Per ulteriori informazioni sui campi attività, vedere [Aggiungere attività agli obiettivi](../results-and-activities/add-activities-to-goals.md).
1. Fai clic su **Salva**.


