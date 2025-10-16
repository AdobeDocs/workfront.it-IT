---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: Allineare gli obiettivi collegandoli negli obiettivi di Adobe Workfront
description: Se sei un singolo collaboratore con un obiettivo personale, potresti volerlo allineare agli obiettivi del tuo team per visualizzare in modo efficace l’avanzamento del tuo obiettivo nel contesto più ampio della strategia dell’organizzazione.
author: Alina
feature: Workfront Goals
exl-id: 4276f1c9-2ee9-4f74-b011-ae1e19fefe35
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '726'
ht-degree: 0%

---

# Allineare gli obiettivi collegandoli in Obiettivi di Adobe Workfront

<!--Audited P&P only: 10/2025-->

Se sei un singolo collaboratore con un obiettivo personale, potresti volerlo allineare agli obiettivi del tuo team per visualizzare in modo efficace l’avanzamento del tuo obiettivo nel contesto più ampio della strategia dell’organizzazione.

Quando tutti nella tua organizzazione hanno i loro obiettivi allineati agli obiettivi della tua organizzazione, possono vedere chiaramente in che modo i loro contributi individuali e gli sforzi del team aiutano a fare un grande passo avanti su priorità più grandi a livello aziendale. Per ulteriori informazioni sulle best practice per l&#39;allineamento degli obiettivi, vedere [Panoramica sull&#39;allineamento degli obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/goal-alignment/goal-alignment-overview.md).

Esistono due approcci per connettere gli obiettivi in Obiettivi di Adobe Workfront:

* Puoi creare l’allineamento tra gli obiettivi collegandoli tra loro.

* Puoi allineare manualmente due obiettivi oppure convertire i risultati e le attività di un obiettivo esistente in un altro obiettivo. Il risultato o l’attività convertiti diventano l’obiettivo secondario dell’obiettivo originale.

>[!IMPORTANT]
>
>Un obiettivo può avere un totale di 1000 indicatori di progresso.

Questo articolo descrive come allineare gli obiettivi collegandoli tra loro. Per informazioni sull&#39;allineamento degli obiettivi tramite la conversione dei risultati e delle attività in obiettivi, vedere [Allineare gli obiettivi tramite la conversione dei risultati e delle attività in obiettivi](../../workfront-goals/goal-alignment/align-goals-by-converting-results-activities.md).

## Requisiti di accesso

>[!NOTE]
>
>La tua azienda potrebbe scegliere di continuare a utilizzare gli obiettivi di Adobe Workfront se ha acquistato questo pacchetto in passato. Per ulteriori dettagli, rivolgiti al rappresentante del tuo account.
>
>Adobe Workfront Goals non è più disponibile per l’acquisto.

+++Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>

<td> <p>Pacchetto Adobe Workfront</p> </td> 
   <td> 
   <p>Adobe Workfront Ultimate</p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>Licenza Adobe Workfront</p> </td> 
   <td> <p>Collaboratore o versione successiva</p> 
     <p>Richiedente o versione successiva</p> </td> 
  </tr>

<td><p>Configurazioni del livello di accesso</p> </td> 
   <td> <p>Modifica accesso agli obiettivi</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Autorizzazioni oggetto </p> </td> 
   <td> <p>Gestire le autorizzazioni per un obiettivo</p>  </td> 
  </tr> 
  <tr>
   <td role="rowheader"><p>Modello layout</p></td>
   <td> <p>A tutti gli utenti, inclusi gli amministratori di sistema, deve essere assegnato un modello di layout che includa l'area Obiettivi nel menu principale. </p>  
</td>
  </tr>
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso alla documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
  <p> New product requirement: Workfront</p>
  Or
  <p>Current product requirement: In addition to a Workfront license, you must purchase a license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Access level</td>
 <td> <p>Edit access to Goals</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Object permissions</td>
 <td>
  
  <p>View or higher permissions to the goal to view it</p>
  <p>Manage permissions to the goal to edit it</p>
  <p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Workfront Goals</a>. </p>
   </td>
 </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Goals area in the Main Menu. </p>  
</td>
  </tr>
</tbody>
</table>-->

## Allineare gli obiettivi collegandoli tra loro

<!--
Aligning goals by connecting them differs depending on what environment you use. 

### Align goals by connecting them in the Production environment

1. Create two goals that you want to align. For information about creating goals, see [Create goals in Adobe Workfront Goals](../../workfront-goals/goal-management/create-goals.md).
1. (Optional) Activate the goals that you want to align. You can align goals that have a Draft, Active, or Inactive status. For information about activating goals, see [Activate goals in Adobe Workfront Goals](../../workfront-goals/goal-management/activate-goals.md).
1. Go to the goal that you want to align (child goal) to another goal (parent goal) and click its name to open the **Goal Details** panel.

   For example, if you want Goal 2 to influence the progress of Goal 1, you must go to Goal 2. 

1. Click **Align to another goal** in the upper-right corner of the right panel.

   ![Align to another goal](assets/align-to-another-goal-link-highlighted-350x128.png)

1. Start typing the name of an existing goal or the name of an owner in the **Align to another goal** field, then select it when it appears in the list. Only goals that are from the same or future periods display in the list. 
1. Click **Save**.

   The goal you started with (Goal 2) is now the child goal of the goal you aligned it with (Goal 1).   
   The aligned goals display connected in the Goal Alignment section with Goal 2 as secondary to Goal 1.

   ![Aligned cards](assets/goal-1-and-2-aligned-cards-350x427.png)

1. (Optional) To view the goals in the Goal Alignment section, do one of the following:

   * Click the Goal Alignment section in the left panel and find the goals by applying the correct filter. For information about filtering information in Workfront Goals, see [Filter information in Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md).
   * Click the Goal List, Check-in, or Pulse sections in the left panel and find one of the goals, then click the **Alignment icon** ![Align icon](assets/align-icon.png) next to the goal name to go directly to the goal in the Goal Alignment section.

   For information about the Goal Alignment section, see [Navigate the Goal Alignment section in Adobe Workfront Goals](../../workfront-goals/goal-alignment/navigate-goal-alignment-chart.md). 

1. (Optional) Add activities and results to either goal to indicate their progress. For information about adding activities and results, see the following articles:

   * [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md) 
   * [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md)

1. (Optional) Remove the alignment between two goals, when you consider that no longer is relevant to your organization's overall strategy For information about removing alignment between goals, see [Remove goal alignment in Adobe Workfront Goals](../../workfront-goals/goal-alignment/remove-goal-alignment.md).

-->
1. Creare due obiettivi da allineare. Per informazioni sulla creazione degli obiettivi, vedere [Creare gli obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/goal-management/create-goals.md).
1. (Facoltativo) Attiva gli obiettivi che desideri allineare. È possibile allineare gli obiettivi con stato Bozza, Attivo o Inattivo. Per informazioni sull&#39;attivazione degli obiettivi, vedere [Attivare gli obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/goal-management/activate-goals.md).
1. Vai all’obiettivo che desideri allineare (obiettivo figlio) a un altro obiettivo (obiettivo padre) e fai clic sul nome per aprire la pagina dell’obiettivo.

   >[!INFO]
   >
   >Ad esempio, se desideri che l&#39;obiettivo 2 influenzi l&#39;avanzamento dell&#39;obiettivo 1, devi passare all&#39;obiettivo 2.

1. Fai clic su **Dettagli obiettivo** nel pannello a sinistra.

1. Nell&#39;area **Informazioni obiettivo principale**, fare clic su **Aggiungi** nel campo **Obiettivo principale** se non è presente alcun obiettivo principale.

   Oppure

   Fai clic sul nome dell’obiettivo principale per sceglierne un altro.

1. Inizia a digitare il nome di un obiettivo esistente nel campo **Obiettivo principale**, quindi selezionalo quando viene visualizzato nell&#39;elenco. Nell’elenco vengono visualizzati solo gli obiettivi dello stesso periodo o di periodi futuri.

1. Fai clic su **Salva modifiche**.

   L’obiettivo con cui hai iniziato (Obiettivo 2) ora è l’obiettivo secondario dell’obiettivo principale con cui l’hai allineato (Obiettivo 1).\
   Gli obiettivi allineati vengono visualizzati connessi nella sezione Allineamento obiettivo con l’Obiettivo 2 secondario all’Obiettivo 1.
L’obiettivo secondario viene visualizzato nella sezione Indicatori di avanzamento dell’obiettivo principale mentre il suo avanzamento aggiorna l’avanzamento dell’obiettivo principale.

   ![Schede allineate](assets/goal-1-and-2-aligned-cards-350x427.png)

1. (Facoltativo) Per visualizzare gli obiettivi nella sezione Allineamento obiettivo, vai all&#39;area Obiettivi di Workfront, quindi fai clic sulla sezione **Allineamento obiettivo** nel pannello a sinistra. Per informazioni sulla sezione Allineamento obiettivo, vedere [Passare alla sezione Allineamento obiettivo in Obiettivi di Adobe Workfront](../../workfront-goals/goal-alignment/navigate-goal-alignment-chart.md).

1. (Facoltativo) Aggiungi attività e risultati a entrambi gli obiettivi per indicarne l’avanzamento. Per informazioni sull’aggiunta di attività e risultati, consulta i seguenti articoli:

   * [Aggiungi attività agli obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/results-and-activities/add-activities-to-goals.md)
   * [Aggiungere risultati agli obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/results-and-activities/add-results-to-goals.md)

1. (Facoltativo) Se ritieni che non sia più pertinente alla strategia complessiva della tua organizzazione, rimuovi l’allineamento tra due obiettivi. Per informazioni sulla rimozione dell&#39;allineamento tra gli obiettivi, vedere [Rimuovere l&#39;allineamento degli obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/goal-alignment/remove-goal-alignment.md).

