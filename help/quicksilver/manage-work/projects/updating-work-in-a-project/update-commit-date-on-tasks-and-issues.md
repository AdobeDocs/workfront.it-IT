---
product-area: projects
navigation-topic: update-work-in-a-project
title: Aggiorna le date di conferma per attività e problemi
description: Puoi aggiornare manualmente la data di conferma di un’attività o di un problema che ti è stato assegnato. Per ulteriori informazioni sulle date di conferma in Adobe Workfront, consulta Panoramica sulla data di conferma.
author: Alina
feature: Work Management
exl-id: 003c52c7-baf3-4316-bb4b-83b600172d48
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 0%

---

# Aggiorna le date di conferma per attività e problemi

Puoi aggiornare manualmente la data di conferma di un’attività o di un problema che ti è stato assegnato. Per ulteriori informazioni sulle date di conferma in Adobe Workfront, consulta [Panoramica sulla data di conferma](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

## Requisiti di accesso

<!--Audited: 01/2024-->

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

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

Prima di iniziare, devi essere assegnato all’attività o al problema per il quale devi aggiornare la Data di conferma.

## Aggiorna le date di conferma per attività e problemi

L’aggiornamento della data di conferma è identico per attività e problemi.

1. Vai a un&#39;attività o a un problema che ti è stato assegnato come **Proprietario**.

   Per ulteriori informazioni su come individuare il proprietario dell’attività per un problema o un’attività, consulta la sezione [Modifica attività](../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments) nell’articolo [Modifica attività](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

1. Clic **Dettagli Attività** o **Dettagli problema** nel pannello a sinistra.
1. Clic **Panoramica** per espanderlo.
1. Aggiornare il **Conferma data** campo.

   ![](assets/task-commit-date-edit-highlighted-details-page.png)

1. Clic **Salva modifiche**.

   Dopo aver apportato questa modifica, si verifica quanto segue: 

   * La data di conferma e la data di completamento pianificata dell’attività o del problema non coincidono più.

     Invece, la Data impegno e la Data completamento prevista dell’attività o del problema diventano le stesse.

     ![](assets/task-projected-completion-date-in-details-highlighted-nwe-350x230.png)

   * Se utilizzi l’area Aggiornamenti precedenti, al proprietario del progetto viene notificato che hai suggerito una nuova Data di conferma per l’attività o il problema e che puoi, in questo momento, aggiornare la Data di completamento pianificata dell’attività o del problema in modo che corrisponda alla Data di conferma suggerita. Questa funzionalità non è supportata nella nuova esperienza di aggiunta di commenti. Per informazioni, consulta [La nuova esperienza di commento](/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

     ![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline-highlighted-nwe-350x139.png)

     Per informazioni sulle notifiche e sugli aggiornamenti attivati da questa modifica, consulta la sezione [Notifiche e aggiornamenti attivati dalla modifica della data di conferma](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md#notifica) nell’articolo [Panoramica sulla data di conferma](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).
