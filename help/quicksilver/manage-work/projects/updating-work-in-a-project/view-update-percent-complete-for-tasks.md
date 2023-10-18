---
product-area: projects
navigation-topic: update-work-in-a-project
title: Visualizza e aggiorna la percentuale di completamento per le attività
description: È possibile aggiornare la percentuale di completamento di un'attività per indicare lo stato di avanzamento dell'attività verso il completamento.
author: Alina
feature: Work Management
exl-id: e53bca4d-1ed3-4e4d-8a35-217529a246dc
source-git-commit: b02c81873d84946f8db54bcf9a1a464de38781de
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 0%

---

# Visualizza e aggiorna la percentuale di completamento per le attività

È possibile aggiornare la percentuale di completamento di un&#39;attività per indicare lo stato di avanzamento dell&#39;attività verso il completamento.

## Requisiti di accesso

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard</p> 
   Or
   <p>Legacy license: Work or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the task</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Per aggiornare manualmente le attività, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Lavoro o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modifica l'accesso alle Attività</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per l’attività</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.


## Aree in cui è possibile aggiornare la percentuale di completamento di un&#39;attività

È possibile aggiornare la percentuale di completamento di un&#39;attività in una delle seguenti aree:

* **In un elenco di attività**: è possibile aggiornare la percentuale di completamento di un’attività quando viene visualizzata la colonna Percentuale di completamento.\
  Per ulteriori informazioni sulla modifica in linea, consulta [Modifica in linea di elementi in un elenco in Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md).

* **Nella vista Milestone (Attività cardine)**: è possibile aggiornare la percentuale di completamento di un’attività utilizzando la vista Milestone (Attività cardine) in un elenco di progetti o in un rapporto di progetto. Per ulteriori informazioni, consulta [Utilizzare la vista Milestone](../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md).

* **Quando si aggiorna l&#39;attività**: è possibile aggiornare l’opzione percentuale di completamento di un’attività quando si aggiunge un aggiornamento all’attività.

  >[!IMPORTANT]
  >
  >Questa opzione viene visualizzata solo dopo aver attivato l&#39;opzione Mostra percentuale completata.\
  >Per attivare la barra di aggiornamento della percentuale di completamento per le attività, effettuare le seguenti operazioni:
  >
  >1. Vai a **Principale** menu>nome>**Altro** accanto al tuo nome >**Modifica** > seleziona **Mostra la percentuale di completamento dello stato di aggiornamento**.\
  >![](assets/show-percent-complete-toggle-in-user-profile-350x243.png)  >

* **Nell’intestazione dell’attività**: è possibile aggiornare la percentuale di completamento di un’attività nell’intestazione dell’attività. Per informazioni, consulta [Modifica attività](../../tasks/manage-tasks/edit-tasks.md).

  ![](assets/nwe-updatetaskpercentinheader-350x54.png)


## Considerazioni sull&#39;aggiornamento della percentuale di completamento di un&#39;attività

* Quando si contrassegna un&#39;attività come completata al 100%, lo Stato dell&#39;attività viene aggiornato a Completo.
* Esistono i seguenti scenari per le attività padre:
   * Non è possibile aggiornare al 100% la percentuale di completamento di un&#39;attività padre quando la modalità di completamento riepilogo del progetto è impostata su Automatico e le sottoattività non sono completate.
   * È possibile aggiornare al 100% la percentuale di completamento di un&#39;attività padre quando la modalità di completamento riepilogo del progetto è impostata su Manuale e le sottoattività sono completate o incomplete.

  Per ulteriori informazioni, consulta [Modifica progetti](../manage-projects/edit-projects.md).

## Aggiornare la percentuale di completamento di un&#39;attività

1. Vai a una delle seguenti aree in Workfront:

   * Un elenco di attività
   * Un elenco di progetti e applica la vista Milestone
   * Un’attività, accedendo alla pagina dell’attività
1. Individua il **Percentuale completamento** campo per l&#39;attività di cui si desidera aggiornare la percentuale di completamento.
1. Fare clic all&#39;interno del campo Percentuale di completamento e digitare un numero compreso tra 0 e 100

   Oppure

   Fai clic e trascina il file **Percentuale completamento** al numero necessario per indicare la quantità di attività completata.

   >[!NOTE]
   >
   >Quando si indica che il 100% dell&#39;attività è completato, lo stato dell&#39;attività viene aggiornato anche a Completato.


1. Premi Invio nella tastiera per salvare la percentuale di completamento.

