---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: Allineare gli obiettivi convertendo risultati e attività in obiettivi
description: Puoi allineare manualmente due obiettivi oppure convertire i risultati e le attività di un obiettivo esistente in un altro obiettivo. Il risultato o l’attività convertiti diventano l’obiettivo secondario dell’obiettivo originale. Per informazioni sull’allineamento manuale di due obiettivi, consulta Allineare gli obiettivi collegandoli in Obiettivi di Adobe Workfront.
author: Alina
feature: Workfront Goals
exl-id: 48371389-952c-4732-b519-9774cd4d1b93
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '605'
ht-degree: 17%

---

# Allineare gli obiettivi convertendo risultati e attività in obiettivi

<!--Audited P&P only: 4/2025-->

Puoi allineare manualmente due obiettivi oppure convertire i risultati e le attività di un obiettivo esistente in un altro obiettivo. Il risultato o l’attività convertiti diventano l’obiettivo secondario dell’obiettivo originale.
Per informazioni sull&#39;allineamento manuale di due obiettivi, vedere [Allineare gli obiettivi collegandoli in Obiettivi di Adobe Workfront](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

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
 <p>Current license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
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

## Prerequisiti

Prima di iniziare, è necessario disporre dei seguenti elementi:

* Un obiettivo esistente con risultati e attività esistenti.

  Per informazioni sulla creazione degli obiettivi, vedere [Creare gli obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/goal-management/create-goals.md).

>[!IMPORTANT]
>
>Un obiettivo può avere fino a 1000 indicatori di progresso.

<!--drafted for goal redesign: At PRODUCTION: update the sentence above to remove Production/ Preview references-->

## Considerazioni durante la conversione di risultati e attività in obiettivi

A volte, un risultato o un’attività possono avere un ambito più ampio del previsto e avrebbe più senso che diventino obiettivi. Puoi convertire i risultati e le attività di un obiettivo esistente in un nuovo obiettivo. Si tratta di un approccio dal basso verso l’alto per allineare gli obiettivi.

Quando converti risultati e attività in obiettivi, tieni presente quanto segue:

* Il risultato o l’attività convertiti diventano l’obiettivo secondario dell’obiettivo originale e i due obiettivi vengono allineati.
* L’obiettivo appena creato diventa il singolo indicatore di progresso per l’obiettivo originale, se non sono presenti risultati o attività aggiuntivi sull’obiettivo originale. Per poter tenere traccia dell’avanzamento su di esso, aggiungi risultati e attività all’obiettivo secondario.
* La conversione di un risultato o di un’attività in un obiettivo è irreversibile. Una volta convertito, il nuovo obiettivo secondario non può più diventare un risultato o un’attività per l’obiettivo principale.

## Convertire un risultato o un’attività in un obiettivo

<!--
<span class="preview">Converting results and activities differs depending on what environment you use. </span>

### Convert a result or activity to a goal in the Production environment

1. Go to a goal that has a result or an activity that you want to convert to a goal.
1. Click the name of the goal to open the **Goal Details** panel.
1. Expand the **Results** or **Activities** right-pointing arrows to see a list of results or activities for the goal. 

1. Click the **gear icon** ![Gear icon](assets/settings-gear-icon.png) to the right of the result or activity name that you want to convert, then click **Convert into a Goal**.

   ![Convert to goal](assets/convert-to-goal-link-highlighted-350x191.png)

1. (Optional) Remove the name of the original activity or result owner from the **Goal Owner** field and replace it with another user, team, group, or your organization's name. By default, Workfront selects the owner of the result or the activity as the goal owner. 
1. Click **Convert**. The activity or result displays as an aligned goal in the Goal Details panel of the original goal and the original activity or result is removed from the original goal and transferred to the second goal. By default, the new goal has the same name as the original converted result or activity. 
1. (Optional) Click the name of the new goal to open the **Goal Details** panel and edit the name of the goal. For information about editing any information for an existing goal, see [Edit goals in Adobe Workfront Goals](../../workfront-goals/goal-management/edit-goals.md).
-->

1. Vai a un obiettivo che ha un risultato o un&#39;attività che desideri convertire in un obiettivo.
1. Dalla pagina dell&#39;obiettivo, fai clic su **Indicatori di avanzamento** nel pannello a sinistra.
1. Seleziona un risultato o un&#39;attività nell&#39;elenco degli indicatori di avanzamento, quindi fai clic sull&#39;icona **Converti in obiettivo** ![Converti in obiettivo](assets/convert-to-goal-icon-unshimmed.png) nella parte superiore dell&#39;elenco degli indicatori di avanzamento. Viene visualizzata la casella Converti in obiettivo (Convert to goal).

   ![Converti in casella obiettivo](assets/convert-to-goal-box-unshimmed.png)
1. Aggiorna le seguenti informazioni:
   * **Nome obiettivo**: per impostazione predefinita, il nuovo obiettivo ha lo stesso nome del risultato o dell&#39;attività originale.
   * **Periodo**: per impostazione predefinita, il periodo del nuovo obiettivo è il trimestre corrente. È possibile selezionare l&#39;impostazione **Abilita date personalizzate** per definire un periodo di tempo personalizzato per il nuovo obiettivo.
   * **Proprietario obiettivo**: per impostazione predefinita, il nuovo proprietario obiettivo è il proprietario del risultato o dell&#39;attività originale.
   * **Descrizione**: aggiungi ulteriori informazioni sul nuovo obiettivo.
1. Fai clic su **Salva**

   Il risultato o l’attività viene ora convertito in un obiettivo secondario dell’obiettivo originale. È elencato come obiettivo nell&#39;elenco degli indicatori di progresso dell&#39;obiettivo originale.



