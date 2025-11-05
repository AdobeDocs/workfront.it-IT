---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Gestire la percentuale di allocazione di utenti o ruoli nelle attività
description: La percentuale di allocazione rappresenta la quantità di tempo in cui una risorsa assegnata deve lavorare su un'attività in un giorno. Rappresenta la percentuale di un giorno lavorativo (in base alla programmazione dell'utente o del progetto) in cui una risorsa viene allocata per l'intera durata dell'attività.
author: Lisa
feature: Work Management
exl-id: 82238dff-b95e-42e4-8e72-6247934b504d
source-git-commit: ac24b2486b9fc5a0b8c2944a6ec240140238b908
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 1%

---

# Gestire la percentuale di allocazione di utenti o ruoli sulle attività

<!--
<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with  a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div> 
-->

La percentuale di allocazione rappresenta la quantità di tempo in cui una risorsa assegnata deve lavorare su un&#39;attività in un giorno. Rappresenta la percentuale di un giorno lavorativo (in base alla programmazione dell&#39;utente o del progetto) in cui una risorsa viene allocata per l&#39;intera durata dell&#39;attività.

>[!NOTE]
>
>Quando si assegnano gli utenti al lavoro, la loro disponibilità in base alle loro pianificazioni influisce sulle date pianificate e previste delle attività e dei problemi. Per informazioni sulle pianificazioni, vedere [Creare una pianificazione](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

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
   <p>Lavoro o superiore</p>
   </td> 
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td>Modifica l'accesso alle Attività</td> 
  </tr> 
  <tr> 
   <td>Autorizzazioni oggetto</td>
   <td><p>Autorizzazioni di contribuzione o di livello superiore per l'attività</p>
   <p>Modificare le autorizzazioni per aggiornare la percentuale di allocazione nella casella Modifica attività</p></td>
  </tr>
 </tbody>
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
Change this sentence in the table when unshimmming assignments on Edit task:
<p>Edit permissions to update allocation percentage in the Edit Task box</p>
To this:
<p>Edit permissions to update allocation percentage in the Edit Task box when editing tasks using the old experience. <span class="preview">You can no longer manage allocation percentage in the Edit task box when editing tasks in the new experience.</span></p> <p>For information, see <a href="/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md">Edit tasks</a></p>.
-->

## Considerazioni sulla modifica delle allocazioni percentuali per le attività

* Per impostazione predefinita, agli utenti viene assegnata una percentuale di tempo uguale per le attività a cui sono assegnati.
* È possibile modificare manualmente la percentuale di allocazione per gli utenti e i ruoli assegnati alle attività solo quando il tipo di durata dell&#39;attività è Lavoro calcolato o Basato sulle risorse.

  Per informazioni, vedere [Panoramica sulla durata e sul tipo di durata dell&#39;attività](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

* Non è possibile modificare la percentuale di allocazione per i team assegnati alle attività.
* Non puoi modificare la percentuale di allocazione per utenti e mansioni assegnati ai problemi.

## Modificare l&#39;allocazione percentuale di utenti o ruoli per un&#39;attività

1. Passare a un&#39;attività per la quale si desidera modificare la percentuale di allocazione delle risorse.
1. Fai clic sul menu **Altro** ![](assets/qs-more-icon-on-an-object.png) accanto al nome dell&#39;attività, quindi fai clic su **Modifica**.

   Oppure

   Fai clic sull&#39;area **Assegnazioni** nell&#39;intestazione dell&#39;attività, quindi fai clic su **Avanzate**.

1. Assicurati che il **Tipo di durata** dell&#39;attività sia uno dei seguenti:

   * Lavoro Calcolato
   * Impegno Aggiuntivo

   >[!TIP]
   >
   >* Per il tipo di durata dell&#39;assegnazione calcolata, Workfront utilizza la formula seguente per calcolare la percentuale di allocazione di ciascun assegnatario: `Allocation Percentage = (Work Required / Number of days in the Duration) / Number of hours per work day / Number of assignees`.
   >* Per il tipo di durata semplice, è possibile stimare le ore assegnate a ciascuna risorsa, non la percentuale di allocazione.

1. Fai clic su **Assegnazioni**, quindi modifica le **Allocazioni** per ogni assegnatario dell&#39;attività.

   È possibile modificare solo la percentuale di allocazione per le assegnazioni utente e ruolo.

   Non è possibile modificare la percentuale di allocazione per un team assegnato a un&#39;attività.

   ![Modifica percentuale di allocazione](assets/advanced-assignments-allocation-percentage.png)

1. Fai clic su **Salva**.
