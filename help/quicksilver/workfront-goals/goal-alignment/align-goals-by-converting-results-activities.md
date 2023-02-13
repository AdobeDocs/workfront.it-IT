---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: Allineare gli obiettivi convertendo risultati e attività in obiettivi
description: Puoi allineare manualmente due obiettivi oppure convertire i risultati e le attività di un obiettivo esistente in un altro. Il risultato o l’attività convertiti diventa l’obiettivo secondario dell’obiettivo originale. Per informazioni sull’allineamento manuale di due obiettivi, consulta Allineare gli obiettivi collegandoli in Obiettivi di Adobe Workfront.
author: Alina
feature: Workfront Goals
exl-id: 48371389-952c-4732-b519-9774cd4d1b93
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '643'
ht-degree: 0%

---

# Allineare gli obiettivi convertendo risultati e attività in obiettivi

Puoi allineare manualmente due obiettivi oppure convertire i risultati e le attività di un obiettivo esistente in un altro. Il risultato o l’attività convertiti diventa l’obiettivo secondario dell’obiettivo originale.
Per informazioni sull&#39;allineamento manuale di due obiettivi, vedi [Allineare gli obiettivi collegandoli negli obiettivi di Adobe Workfront](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

## Requisiti di accesso


<!--drafted for P&P release: 

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
* Un obiettivo esistente con risultati e attività esistenti.

   Per informazioni sulla creazione degli obiettivi, vedi [Creare obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/goal-management/create-goals.md).

>[!IMPORTANT]
>
>Un obiettivo può contenere fino a 1000 indicatori di progresso.

<!--drafted for goal redesign: At PRODUCTION: update the sentence above to remove Production/ Preview references-->

## Considerazioni durante la conversione di risultati e attività in obiettivi

A volte, un risultato o un&#39;attività può avere un ambito più ampio del previsto e avrebbe più senso che diventassero obiettivi. Puoi convertire i risultati e le attività di un obiettivo esistente in un nuovo obiettivo. Questo è un approccio dal basso verso l&#39;alto per allineare gli obiettivi.

Quando converti risultati e attività in obiettivi, considera quanto segue:

* Il risultato o l’attività convertiti diventa l’obiettivo secondario dell’obiettivo originale e i due obiettivi diventano allineati.
* L&#39;obiettivo appena creato diventa l&#39;unico indicatore di avanzamento per l&#39;obiettivo originale, se non ci sono ulteriori risultati o attività sull&#39;obiettivo originale. Devi aggiungere risultati e attività all’obiettivo figlio per essere in grado di tracciare l’avanzamento su di esso.
* La conversione di un risultato o di un’attività in un obiettivo è irreversibile. Una volta convertito, il nuovo obiettivo figlio non può mai più diventare un risultato o un’attività per l’obiettivo principale.

## Convertire un risultato o un’attività in un obiettivo

<!--
<span class="preview">Converting results and activities differs depending on what environment you use. </span>

### Convert a result or activity to a goal in the Production environment

1. Go to a goal that has a result or an activity that you want to convert to a goal.
1. Click the name of the goal to open the **Goal Details** panel.
1. Expand the **Results** or **Activities** right-pointing arrows to see a list of results or activities for the goal. 

1. Click the **gear icon** ![](assets/settings-gear-icon.png) to the right of the result or activity name that you want to convert, then click **Convert into a Goal**.

   ![](assets/convert-to-goal-link-highlighted-350x191.png)

1. (Optional) Remove the name of the original activity or result owner from the **Goal Owner** field and replace it with another user, team, group, or your organization's name. By default, Workfront selects the owner of the result or the activity as the goal owner. 
1. Click **Convert**. The activity or result displays as an aligned goal in the Goal Details panel of the original goal and the original activity or result is removed from the original goal and transferred to the second goal. By default, the new goal has the same name as the original converted result or activity. 
1. (Optional) Click the name of the new goal to open the **Goal Details** panel and edit the name of the goal. For information about editing any information for an existing goal, see [Edit goals in Adobe Workfront Goals](../../workfront-goals/goal-management/edit-goals.md).
-->

1. Passa a un obiettivo con un risultato o un&#39;attività che desideri convertire in un obiettivo.
1. Dalla pagina dell’obiettivo, fai clic su **Indicatori di progresso** nel pannello a sinistra.
1. Seleziona un risultato o un’attività nell’elenco degli indicatori di avanzamento, quindi fai clic sul pulsante **Converti in obiettivo** icona ![](assets/convert-to-goal-icon-unshimmed.png) nella parte superiore dell’elenco degli indicatori di avanzamento. Viene visualizzata la casella Converti in obiettivo.

   ![](assets/convert-to-goal-box-unshimmed.png)
1. Aggiorna le seguenti informazioni:
   * **Nome dell&#39;obiettivo**: Per impostazione predefinita, il nuovo obiettivo ha lo stesso nome del risultato o dell’attività originale.
   * **Punto**: Per impostazione predefinita, il periodo del nuovo obiettivo è il trimestre corrente. È possibile selezionare la **Abilita date personalizzate** impostazione per definire un periodo di tempo personalizzato per il nuovo obiettivo.
   * **Proprietario dell&#39;obiettivo**: Per impostazione predefinita, il nuovo proprietario dell’obiettivo è il proprietario del risultato o dell’attività originale.
   * **Descrizione**: Aggiungi ulteriori informazioni sul nuovo obiettivo.
1. Fai clic su **Salva**

   Il risultato o l’attività viene ora convertito in un obiettivo figlio dell’obiettivo originale. È elencato come obiettivo nell&#39;elenco degli indicatori di avanzamento dell&#39;obiettivo originale.



