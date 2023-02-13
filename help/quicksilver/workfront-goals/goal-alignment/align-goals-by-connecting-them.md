---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: Allineare gli obiettivi collegandoli negli obiettivi di Adobe Workfront
description: Se sei un collaboratore individuale con un obiettivo personale, puoi allinearlo agli obiettivi del tuo team per visualizzare in modo efficace il progresso del tuo obiettivo nel contesto più ampio della strategia della tua organizzazione.
author: Alina
feature: Workfront Goals
exl-id: 4276f1c9-2ee9-4f74-b011-ae1e19fefe35
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '770'
ht-degree: 0%

---

# Allineare gli obiettivi collegandoli negli obiettivi di Adobe Workfront


Se sei un collaboratore individuale con un obiettivo personale, puoi allinearlo agli obiettivi del tuo team per visualizzare in modo efficace il progresso del tuo obiettivo nel contesto più ampio della strategia della tua organizzazione.

Quando tutti i membri della tua organizzazione hanno i loro obiettivi allineati a quelli della tua organizzazione, possono vedere chiaramente in che modo i loro contributi individuali e gli sforzi del team aiutano a spostare l&#39;ago avanti su priorità a livello aziendale più grandi. Per ulteriori informazioni sulle best practice per l’allineamento degli obiettivi, consulta [Panoramica sull’allineamento degli obiettivi negli obiettivi di Adobe Workfront](../../workfront-goals/goal-alignment/goal-alignment-overview.md).

Esistono due approcci per collegare gli obiettivi in Obiettivi di Adobe Workfront:

* È possibile creare l&#39;allineamento tra gli obiettivi collegando gli obiettivi tra loro.

* Puoi allineare manualmente due obiettivi oppure convertire i risultati e le attività di un obiettivo esistente in un altro. Il risultato o l’attività convertiti diventa l’obiettivo secondario dell’obiettivo originale.

>[!IMPORTANT]
>
>Un obiettivo può avere un totale di 1000 indicatori di progresso.

Questo articolo descrive come allineare gli obiettivi collegandoli tra loro. Per informazioni sull’allineamento degli obiettivi mediante la conversione di risultati e attività in obiettivi, consulta [Allineare gli obiettivi convertendo risultati e attività in obiettivi](../../workfront-goals/goal-alignment/align-goals-by-converting-results-activities.md).

## Requisiti di accesso

<!--drfated for the P&P release: 

You must have the following:

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
   <td> <p>Modifica l'accesso agli obiettivi</p> <p><b>NOTA</b>

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

## Allineare gli obiettivi collegandoli tra loro

<!--
Aligning goals by connecting them differs depending on what environment you use. 

### Align goals by connecting them in the Production environment

1. Create two goals that you want to align. For information about creating goals, see [Create goals in Adobe Workfront Goals](../../workfront-goals/goal-management/create-goals.md).
1. (Optional) Activate the goals that you want to align. You can align goals that have a Draft, Active, or Inactive status. For information about activating goals, see [Activate goals in Adobe Workfront Goals](../../workfront-goals/goal-management/activate-goals.md).
1. Go to the goal that you want to align (child goal) to another goal (parent goal) and click its name to open the **Goal Details** panel.

   For example, if you want Goal 2 to influence the progress of Goal 1, you must go to Goal 2. 

1. Click **Align to another goal** in the upper-right corner of the right panel.

   ![](assets/align-to-another-goal-link-highlighted-350x128.png)

1. Start typing the name of an existing goal or the name of an owner in the **Align to another goal** field, then select it when it appears in the list. Only goals that are from the same or future periods display in the list. 
1. Click **Save**.

   The goal you started with (Goal 2) is now the child goal of the goal you aligned it with (Goal 1).   
   The aligned goals display connected in the Goal Alignment section with Goal 2 as secondary to Goal 1.

   ![](assets/goal-1-and-2-aligned-cards-350x427.png)

1. (Optional) To view the goals in the Goal Alignment section, do one of the following:

   * Click the Goal Alignment section in the left panel and find the goals by applying the correct filter. For information about filtering information in Workfront Goals, see [Filter information in Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md).
   * Click the Goal List, Check-in, or Pulse sections in the left panel and find one of the goals, then click the **Alignment icon** ![](assets/align-icon.png) next to the goal name to go directly to the goal in the Goal Alignment section.

   For information about the Goal Alignment section, see [Navigate the Goal Alignment section in Adobe Workfront Goals](../../workfront-goals/goal-alignment/navigate-goal-alignment-chart.md). 

1. (Optional) Add activities and results to either goal to indicate their progress. For information about adding activities and results, see the following articles:

   * [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md) 
   * [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md)

1. (Optional) Remove the alignment between two goals, when you consider that no longer is relevant to your organization's overall strategy For information about removing alignment between goals, see [Remove goal alignment in Adobe Workfront Goals](../../workfront-goals/goal-alignment/remove-goal-alignment.md).

-->
1. Crea due obiettivi da allineare. Per informazioni sulla creazione degli obiettivi, vedi [Creare obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/goal-management/create-goals.md).
1. (Facoltativo) Attiva gli obiettivi che desideri allineare. È possibile allineare gli obiettivi con stato Bozza, Attivo o Inattivo. Per informazioni sull’attivazione degli obiettivi, vedi [Attivare gli obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/goal-management/activate-goals.md).
1. Passa all’obiettivo da allineare (obiettivo figlio) a un altro obiettivo (obiettivo padre) e fai clic sul suo nome per aprire la pagina dell’obiettivo.

   >[!INFO]
   >
   >Ad esempio, se desideri che l’obiettivo 2 influisca sul progresso dell’obiettivo 1, devi andare all’obiettivo 2.

1. Fai clic su **Dettagli obiettivo** nel pannello a sinistra.

1. In **Informazioni sull&#39;obiettivo padre** area, fai clic su **Aggiungi** in **Obiettivo principale** campo se non esiste un obiettivo principale,

   Oppure

   Fai clic sul nome dell’obiettivo principale per sceglierne un altro.

1. Inizia a digitare il nome di un obiettivo esistente nella **Obiettivo principale** , quindi selezionalo quando viene visualizzato nell’elenco. Nell’elenco vengono visualizzati solo gli obiettivi dello stesso periodo o di periodi futuri.

1. Fai clic su **Salva modifiche**.

   L’obiettivo con cui hai iniziato (Obiettivo 2) è ora l’obiettivo secondario dell’obiettivo principale con cui l’hai allineato (Obiettivo 1).\
   Gli obiettivi allineati sono collegati nella sezione Allineamento obiettivo con Obiettivo 2 come secondario rispetto all&#39;Obiettivo 1.
L&#39;obiettivo figlio viene visualizzato nella sezione Indicatori di avanzamento dell&#39;obiettivo principale mentre l&#39;avanzamento dell&#39;obiettivo principale viene aggiornato.

   ![](assets/goal-1-and-2-aligned-cards-350x427.png)

1. (Facoltativo) Per visualizzare gli obiettivi nella sezione Allineamento obiettivo , vai all&#39;area Obiettivi di Workfront, quindi fai clic sul pulsante **Allineamento obiettivo** nel pannello a sinistra. Per informazioni sulla sezione Allineamento obiettivo, vedere [Naviga nella sezione Allineamento obiettivo in Obiettivi di Adobe Workfront](../../workfront-goals/goal-alignment/navigate-goal-alignment-chart.md).

1. (Facoltativo) Aggiungi attività e risultati a entrambi gli obiettivi per indicare il loro avanzamento. Per informazioni sull’aggiunta di attività e risultati, vedi i seguenti articoli:

   * [Aggiungere attività agli obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/results-and-activities/add-activities-to-goals.md)
   * [Aggiungere risultati agli obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/results-and-activities/add-results-to-goals.md)

1. (Facoltativo) Rimuovi l&#39;allineamento tra due obiettivi, se ritieni che non sia più rilevante per la strategia globale della tua organizzazione. Per informazioni sulla rimozione dell&#39;allineamento tra obiettivi, consulta [Rimuovere l’allineamento dell’obiettivo negli obiettivi di Adobe Workfront](../../workfront-goals/goal-alignment/remove-goal-alignment.md).

