---
product-area: projects
navigation-topic: update-work-in-a-project
title: Visualizza e aggiorna percentuale di completamento per le attività
description: È possibile aggiornare la percentuale di completamento di un'attività per indicare lo stato di avanzamento dell'attività verso il completamento.
author: Alina
feature: Work Management
exl-id: e53bca4d-1ed3-4e4d-8a35-217529a246dc
source-git-commit: 1c2303fe2cea51e3339335c433d2be6475949cb1
workflow-type: tm+mt
source-wordcount: '553'
ht-degree: 0%

---

# Visualizza e aggiorna la percentuale di completamento per le attività

<!--Audited:01/2024-->

È possibile aggiornare la percentuale di completamento di un&#39;attività per indicare lo stato di avanzamento dell&#39;attività verso il completamento.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per aggiornare manualmente le attività, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Nuova licenza: Standard</p> 
   Oppure
   <p>Licenza corrente: Lavoro o versione successiva</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica l'accesso alle Attività</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per l’attività</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Aree in cui è possibile aggiornare la percentuale di completamento di un&#39;attività

È possibile aggiornare la percentuale di completamento di un&#39;attività in una delle seguenti aree:

* **In un elenco di attività**: è possibile aggiornare la percentuale di completamento di un&#39;attività quando viene visualizzata la colonna Percentuale di completamento.\
  Per ulteriori informazioni sulla modifica in linea, vedere [Elementi di modifica in linea in un elenco in Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md).

* **Nella vista Milestone**: è possibile aggiornare la percentuale di completamento di un&#39;attività quando si utilizza la vista Milestone in un elenco di progetti o in un report di progetti. Per ulteriori informazioni, vedere [Utilizzare la vista Milestone](../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md).

<!--only in legacy commenting: 
* **As you update the task**:  You can update the percent complete option of a task when adding an update to the task.

  >[!IMPORTANT]
  >
  >This option displays only after you enable the Show Percent Complete option.  
  >To enable the percent complete update bar for tasks, do the following:   
  >
  >1. Go to the **Main** menu>your name>**More** icon next to your name >**Edit** > select **Show percent complete on update status**.   
  >![](assets/show-percent-complete-toggle-in-user-profile-350x243.png)  >-->

* **Nell&#39;intestazione attività**: è possibile aggiornare la percentuale di completamento di un&#39;attività nell&#39;intestazione attività. Per informazioni, vedere [Modifica attività](../../tasks/manage-tasks/edit-tasks.md).

  ![](assets/nwe-updatetaskpercentinheader-350x54.png)

* **Nel pannello Riepilogo di un&#39;attività**: puoi aggiornare la percentuale di completamento di un&#39;attività nella parte superiore del pannello Riepilogo quando visualizzi l&#39;attività nelle seguenti aree:

   * Elenco o rapporto attività
   * Scheda orario
   * Bilanciatore dei carichi di lavoro

  ![](assets/update-percent-complete-in-task-summary-highlighted.png)

  Per ulteriori informazioni, vedere [Panoramica di riepilogo](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)

* **Home**: è possibile aggiornare la percentuale di completamento di un&#39;attività o di un problema dal pannello Riepilogo nell&#39;area Home o dal widget Il mio lavoro.

Per informazioni, vedere [Guida introduttiva alla Home](/help/quicksilver/workfront-basics/using-home/using-the-home-area/get-started-with-home.md).

## Considerazioni sull&#39;aggiornamento della percentuale di completamento di un&#39;attività

* Quando si contrassegna un&#39;attività come completata al 100%, lo Stato dell&#39;attività viene aggiornato a Completo.
* Esistono i seguenti scenari per le attività padre:
   * Non è possibile aggiornare al 100% la percentuale di completamento di un&#39;attività padre quando la modalità di completamento riepilogo del progetto è impostata su Automatico e le sottoattività non sono completate.
   * È possibile aggiornare al 100% la percentuale di completamento di un&#39;attività padre quando la modalità di completamento riepilogo del progetto è impostata su Manuale e le sottoattività sono completate o incomplete.

  Per ulteriori informazioni, vedere [Modifica progetti](../manage-projects/edit-projects.md).

## Aggiornare la percentuale di completamento di un&#39;attività

1. Vai a una delle seguenti aree in Workfront:

   * Un elenco di attività
   * Un elenco di progetti e applica la vista Milestone
   * Un’attività, accedendo alla pagina dell’attività
1. Individua il campo **Percentuale completata** per l&#39;attività di cui desideri aggiornare la percentuale di completamento.

   >[!TIP]
   >
   >  Il campo Percentuale di completamento viene sempre visualizzato nella parte superiore del pannello Riepilogo.


1. Fai clic nel campo **Percentuale completata** e digita un numero compreso tra 0 e 100

   Oppure

   Fai clic e trascina la barra **Percent Complete** (Percentuale di completamento) sul numero necessario per indicare la quantità di attività completata, se disponibile.

   >[!NOTE]
   >
   >Quando si indica che il 100% dell&#39;attività è completato, lo stato dell&#39;attività viene aggiornato anche a Completato.


1. Premi Invio nella tastiera per salvare la percentuale di completamento.

Anche la percentuale di completamento del progetto viene aggiornata automaticamente.

