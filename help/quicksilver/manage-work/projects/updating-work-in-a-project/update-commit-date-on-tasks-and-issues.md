---
product-area: projects
navigation-topic: update-work-in-a-project
title: Aggiornare le date di conferma per attività e problemi
description: Puoi aggiornare manualmente la data di conferma di un’attività o di un problema che ti è stato assegnato. Per ulteriori informazioni sulle date di conferma in Adobe Workfront, consulta Panoramica sulla data di conferma.
author: Alina
feature: Work Management
exl-id: 003c52c7-baf3-4316-bb4b-83b600172d48
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 0%

---


# Aggiorna le date di conferma per attività e problemi

<!--Audited: 07/2024-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases.</span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release, see [Third Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).</span>-->

Puoi aggiornare manualmente la data di conferma di un’attività o di un problema che ti è stato assegnato. Per ulteriori informazioni su Conferma date in Adobe Workfront, consulta [Panoramica sulla conferma data](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

## Requisiti di accesso

<!--Audited: 01/2024-->

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

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
   Nuovo:
   <ul>
   <li><p>Standard per le attività</p> </li>
   <li><p>Collaboratore o versione successiva per i problemi</p></li>
   </ul>
   Corrente:
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
   <td> <p>Gestire le autorizzazioni per l’attività o il problema</p>
   <p> Per aggiornare la data del commit, devi essere assegnato all’attività o al problema </p>
    </td> 
  </tr> 
 </tbody> 
</table>

* Per ulteriori informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

Prima di poter modificare la Data di conferma di un’attività o di un problema, è necessario essere assegnati all’attività o al problema di cui è necessario aggiornare la Data di conferma.

## Aggiorna le date di conferma per attività e problemi


Puoi aggiornare la Data di conferma di un’attività o di un problema nelle seguenti aree di Workfront:

* La sezione Dettagli di un’attività o di un problema
* Intestazione dell’attività o del problema

  L’amministratore del Workfront o del gruppo deve aggiungere la Data di conferma all’intestazione dell’attività o del problema del modello di layout per visualizzarla dalla pagina dell’attività o del problema.
Per informazioni, vedere [Personalizzare le intestazioni degli oggetti utilizzando un modello di layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

L’aggiornamento della data di conferma è identico per attività e problemi.

>[!NOTE]
>
>È possibile chiedere all&#39;amministratore del sistema o del gruppo di aggiungere il campo Data conferma al pannello Riepilogo per semplificarne l&#39;aggiornamento in varie aree di Workfront.
>
>Per ulteriori informazioni, consulta i seguenti articoli:
>
>* [Panoramica di riepilogo](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)
>* [Personalizzare il pannello Riepilogo utilizzando un modello di layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).


1. Vai a un&#39;attività o a un problema a cui sei assegnato come **Proprietario**.

   Per ulteriori informazioni su come individuare il proprietario dell&#39;attività per un problema o un&#39;attività, vedere la sezione [Modifica attività](../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments) nell&#39;articolo [Modifica attività](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

1. (Condizionale e facoltativo) Se l&#39;amministratore del Workfront o del gruppo ha aggiunto la Data conferma all&#39;intestazione dell&#39;attività o del problema, fare clic sul campo **Data conferma** nell&#39;intestazione, quindi selezionare una data dal calendario. Se la Data del commit non è nell&#39;intestazione, procedere come segue.

   ![](assets/commit-date-task-header.png)

1. Fai clic su **Dettagli attività** o **Dettagli problema** nel pannello a sinistra.
1. Fai clic su **Panoramica** per espanderlo.
1. Aggiorna il campo **Commit Date**.

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

     Per informazioni sulle notifiche e sugli aggiornamenti attivati da questa modifica, vedere la sezione &quot;Notifiche e aggiornamenti attivati dalla modifica della data di conferma&quot; nell&#39;articolo [Panoramica sulla data di conferma](/help/quicksilver/manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

<!--at the Production update stream when removing legacy - replace the last bullet with: The Project Owner is notified in the Systems Activity and the All tabs of the Updates section that you have suggested a new Commit Date. They can then update the Planned Completion Date accordingly by editing the task or the issue.-->
