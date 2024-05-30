---
product-area: projects
navigation-topic: update-work-in-a-project
title: Aggiorna le date di conferma per attività e problemi
description: Puoi aggiornare manualmente la data di conferma di un’attività o di un problema che ti è stato assegnato. Per ulteriori informazioni sulle date di conferma in Adobe Workfront, consulta Panoramica sulla data di conferma.
author: Alina
feature: Work Management
exl-id: 003c52c7-baf3-4316-bb4b-83b600172d48
source-git-commit: 49335ec86057e4985477034558a271bf4efcab5e
workflow-type: tm+mt
source-wordcount: '574'
ht-degree: 0%

---


# Aggiorna le date di conferma per attività e problemi

{{highlighted-preview}}

Puoi aggiornare manualmente la data di conferma di un’attività o di un problema che ti è stato assegnato. Per ulteriori informazioni sulle date di conferma in Adobe Workfront, consulta [Panoramica sulla data di conferma](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

## Requisiti di accesso

<!--Audited: 01/2024-->

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

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
   <td> 
   Per le nuove licenze:
   <ul>
   <li><p>Standard per le attività</p> </li>
   <li><p>Collaboratore o versione successiva per i problemi</p></li>
   </ul>
   Per le licenze correnti:
<ul>
   <li><p>Lavoro o superiore per le attività</p></li> 
   <li><p>Richiedi o superiore per problemi</p></li>
</ul>

</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica l'accesso ad Attività e Issues</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per l’attività o il problema</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni sulla pianificazione, il tipo di licenza o l&#39;accesso disponibili, contattare l&#39;amministratore Workfront. Per ulteriori informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Prerequisiti

Prima di poter modificare la Data di conferma di un’attività o di un problema, è necessario essere assegnati all’attività o al problema di cui è necessario aggiornare la Data di conferma.

## Aggiorna le date di conferma per attività e problemi


Puoi aggiornare la Data di conferma di un’attività o di un problema nelle seguenti aree di Workfront:

* La sezione Dettagli di un’attività o di un problema
* <span class="preview">Intestazione dell’attività o del problema</span>

  <span class="preview">L’amministratore del Workfront o del gruppo deve aggiungere la Data di conferma all’intestazione dell’attività o del problema del modello di layout per visualizzarla dalla pagina dell’attività o del problema.
Per informazioni, consulta [Personalizzare le intestazioni degli oggetti utilizzando un modello di layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).</span>

L’aggiornamento della data di conferma è identico per attività e problemi.

>[!NOTE]
>
>È possibile chiedere all&#39;amministratore del sistema o del gruppo di aggiungere il campo Data conferma al pannello Riepilogo per semplificarne l&#39;aggiornamento in varie aree di Workfront.
>
>Per ulteriori informazioni, consulta i seguenti articoli:
>
>* [Panoramica di riepilogo](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)
>* [Personalizzare Home e Riepilogo utilizzando un modello di layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).


1. Vai a un&#39;attività o a un problema che ti è stato assegnato come **Proprietario**.

   Per ulteriori informazioni su come individuare il proprietario dell’attività per un problema o un’attività, consulta la sezione [Modifica attività](../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments) nell’articolo [Modifica attività](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

1. <span class="preview">(Condizionale e facoltativo) Se l’amministratore del Workfront o del gruppo ha aggiunto la Data conferma all’intestazione dell’attività o del problema, fai clic su **Conferma data** nell’intestazione, quindi seleziona una data dal calendario. Se la Data del commit non è nell&#39;intestazione, procedere come segue. </span>

   <span class="preview">![](assets/commit-date-task-header.png)</span>

1. Clic **Dettagli Attività** o **Dettagli problema** nel pannello a sinistra.
1. Clic **Panoramica** per espanderlo.
1. Aggiornare il **Conferma data** campo.

   ![](assets/task-commit-date-edit-highlighted-details-page.png)

1. Fai clic su **Salva modifiche**.

   Dopo aver apportato questa modifica, si verifica quanto segue:

   * La data di conferma e la data di completamento pianificata dell’attività o del problema non coincidono più.

     Invece, la Data impegno e la Data completamento prevista dell’attività o del problema diventano le stesse.

     ![](assets/task-projected-completion-date-in-details-highlighted-nwe-350x230.png)

   * In una notifica in-app Workfront, il proprietario del progetto riceve una notifica che informa che hai suggerito una nuova Data di conferma per l’attività o il problema.
   * Nella sezione Aggiornamenti, il proprietario del progetto viene informato che hai suggerito una nuova Data di conferma e che può, in questo momento, aggiornare la Data di completamento pianificata dell’attività o del problema in modo che corrisponda alla Data di conferma suggerita.

     ![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline.png)


     <!--![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline-highlighted-nwe-350x139.png)-->

     Per informazioni sulle notifiche e sugli aggiornamenti attivati da questa modifica, consulta la sezione &quot;Notifiche e aggiornamenti attivati dalla modifica della data di conferma&quot; nell’articolo [Panoramica sulla data di conferma](/help/quicksilver/manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

<!--at the Production update stream when removing legacy - replace the last bullet with: The Project Owner is notified in the Systems Activity and the All tabs of the Updates section that you have suggested a new Commit Date. They can then update the Planned Completion Date accordingly by editing the task or the issue.-->