---
product-area: projects
navigation-topic: manage-issues
title: Modificare le assegnazioni utente per più problemi in un elenco
description: Modificare le assegnazioni utente per più problemi in un elenco
author: Lisa
feature: Work Management
exl-id: e1e75027-1847-44cf-afeb-b19394dc3ea5
source-git-commit: 0358e79bd606d0035959bba2a47256456b529b18
workflow-type: tm+mt
source-wordcount: '521'
ht-degree: 1%

---

# Modificare le assegnazioni utente per più problemi in un elenco

<!--Audited: 07/2024-->
<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: similar article exists for tasks)</p>
-->

<!--<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div> -->

È possibile modificare simultaneamente le assegnazioni degli utenti a più problemi. Per informazioni sulla modifica o l’assegnazione di problemi uno alla volta, consulta anche i seguenti articoli:

* [Modifica problemi](../../../manage-work/issues/manage-issues/edit-issues.md)
* [Assegna problemi](../../../manage-work/issues/manage-issues/assign-issues.md)

Per informazioni generali sull&#39;assegnazione dei problemi, vedere [Panoramica sulla modifica delle assegnazioni dei problemi](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

>[!NOTE]
>
>È necessario disporre almeno delle autorizzazioni Contribuisci a un problema per poter effettuare assegnazioni al problema.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td>Licenza Adobe Workfront</td> 
   <td> <p>Standard</p>
   <p>Richiedi o superiore</p> </td> 
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td> <p>Modifica l'accesso alle Issues</p> <p>Accesso di visualizzazione o superiore a progetti e attività per assegnare un problema</p> </td> 
  </tr> 
  <tr> 
   <td>Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per il problema</p> <p>Quando si assegnano più problemi, contribuire con autorizzazioni o versioni successive al progetto o all’attività in cui si trova il problema.</p>  </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>When to modify user assignments on issues</h2>
<p>(NOTE:  drafted and moved to the overview article: Modify issue assignments overview)</p>
<p>You might want to modify the user assignments for multiple issues for a variety of  reasons, including the following:</p>
<ul>
<li>Users join or leave  your team</li>
<li>A user takes a vacation that extends beyond the issue  due dates</li>
<li>A specific role or user is set as the assignee for multiple issues and you want to quickly modify all items to be assigned to a different user or role</li>
</ul>
</div>
-->

## Modificare le assegnazioni per più problemi

1. Passare all&#39;elenco dei problemi contenente i problemi di cui si desidera modificare le assegnazioni.
1. (Facoltativo) Crea un filtro per visualizzare solo i problemi assegnati all’assegnatario che desideri modificare.

   Ad esempio, puoi creare un filtro per visualizzare solo i problemi con un ruolo specifico come assegnatario.  Quindi, puoi sostituire il ruolo con un utente specifico. Effettua le seguenti operazioni:

   1. Fai clic sull&#39;elenco a discesa **Filtri**, quindi fai clic su **Nuovo filtro**.

   1. Nel primo campo, inizia a digitare **Ruoli assegnazione** e scegli **Ruoli assegnazione: Nome** dall&#39;elenco.
   1. Selezionare **Is any of** dal menu a discesa del modificatore, quindi iniziare a digitare il nome di un ruolo e selezionarlo quando viene visualizzato nell&#39;elenco. È possibile digitare più ruoli.

      >[!TIP]
      >
      >Non utilizzare **Assegnato a** perché questo campo fa riferimento solo al proprietario del problema e non a tutti gli assegnatari.

      L’elenco dei problemi filtra automaticamente in base ai criteri di filtro.
   1. (Facoltativo) Fai clic su **Salva come nuovo**, quindi su **Salva**.

1. Seleziona i problemi per i quali vuoi modificare le assegnazioni, quindi fai clic sull&#39;icona **Modifica** ![Icona Modifica](assets/qs-edit-icon.png).

   Viene visualizzato **Modifica problemi**. Il numero di elementi selezionati viene visualizzato nell&#39;angolo superiore sinistro della pagina.

1. Fai clic su **Assegnazioni** nel pannello a sinistra, quindi fai clic sull&#39;icona **x** accanto all&#39;assegnatario da rimuovere.

   >[!TIP]
   >
   >Solo gli assegnatari assegnati a tutti i problemi selezionati vengono visualizzati nell&#39;area **Assegnazioni**.

   ![Area assegnazioni in problemi di modifica in blocco](assets/assignments-area-on-bulk-edit-issues.png)

1. Inizia a digitare il nome di un utente, una mansione o un team per aggiungere gli assegnatari a tutti i problemi selezionati.

   >[!TIP]
   >
   >Puoi assegnare più utenti, mansioni o team. Puoi assegnare solo utenti attivi, mansioni e team.
   >
   >Se un utente, una mansione o un team è stato assegnato prima della disattivazione, rimane assegnato all&#39;elemento di lavoro. In questo caso, consigliamo quanto segue:
   >
   >* Riassegnare l&#39;elemento di lavoro alle risorse attive.
   >* Associare gli utenti di un team disattivato a un team attivo e riassegnare l&#39;elemento di lavoro al team attivo.

   Gli assegnatari aggiunti vengono aggiunti a quelli esistenti. Non sostituiscono quelli esistenti per ogni problema selezionato.

1. (Facoltativo) Fai clic su **Assegna a me** per assegnare tutti i problemi a te stesso.
1. Fai clic su **Salva**.


   <!--Old functionality for assignments for issues - before November 2025:
   1. (Conditional) In the Production environment, do the following: 
   1. Go to the **Assignments** section, then select **Assignee**.
      ![Assignments area](assets/classic-assignmens-area-on-edit-box-350x119.png)
   1. Do one of the following:
      1. To add a new assignee:
         1. Start typing the name of a user, role, or team, then select it when it displays in the list. The assignment is added and does not replace the current assignments on the selected issues.
         >[!TIP]
         >
         >You can assign multiple users, job roles, or teams. You can assign only active users, job roles, and teams.
         >
         >If a user, job role, or a team was assigned before they were deactivated, they remain assigned to the work item. In this case, we recommend the following:
         >
         >* Reassign the work item to active resources.
         >* Associate the users in a deactivated team with an active team and reassign the work item to the active team.
          Information that is common across all issues selected displays. For example, if the same user is assigned to all issues, that user displays in the **Assignee**  column. If information is not common across the issues selected, no information displays.
      1. To remove individual assignees:
         1. Click the **X icon** next to the name of the assignee that you want to remove if the assignee displays in the Assignments list.
            Or
            If the assignee that you want to remove does not display in the Assignments section because the assignee is assigned to only some of the issues that you have selected, click **Remove Assignee** and start typing the name of the assignee that you want to remove, then click the name when it appears in the drop-down list.
         1. Click  **Remove Assignee** again to add another assignee to remove.
      1. To remove all existing assignees:
         1. Click **Remove All Existing Assignees**, then click **Yes, Delete All Assignees**.
            This removes not only common assignees (assignees that are displayed in the edit  dialog box), but also all assignees on all the selected issues.
         1. (Optional) Modify any of the following options for the assignees you selected to associate with the issues:
          * **Issue Owner:**  Select the radio button to indicate which assignee is designated as the Issues Owner. If left unselected, Adobe Workfront designates the first assignee as the Issue Owner. This is not available for team assignments. 
            * **Assignee's Role**: Select a role from the drop-down list. If left unselected, Workfront automatically selects the Primary Role of the user.
      1. Click **Save Changes**.-->




