---
product-area: templates
navigation-topic: templates-navigation-topic
title: Rimuovere informazioni sul modello da un progetto
description: Impossibile rimuovere un modello da un progetto. È possibile rimuovere solo manualmente le informazioni aggiunte al progetto dopo che un modello è stato allegato al progetto. Per informazioni sull’associazione dei modelli, consulta Allegare un modello a un progetto.
author: Alina
feature: Work Management
exl-id: a8b6055a-7fac-4f9b-a880-10b2b85299b7
source-git-commit: d7600a55b3dffb242957234de9d85a0deb1ad2e3
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 1%

---

# Rimuovere informazioni sul modello da un progetto

Impossibile rimuovere un modello da un progetto. È possibile rimuovere solo manualmente le informazioni aggiunte al progetto dopo che un modello è stato allegato al progetto. Per informazioni su come allegare i modelli, vedere [Allegare un modello a un progetto](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> <p>Standard</p>
   <p>Lavoro o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica l'accesso alle Attività</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire l’accesso alle attività </p> <p>Contribuire o accedere più facilmente al progetto</p>  </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>New: Standard</p>
   <p>Current: Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Tasks</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage access to tasks </p> <p>Contribute or higher access to the project </p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## Opzioni per rimuovere le informazioni sul modello da un progetto

Per rimuovere le informazioni sul modello aggiunte al progetto, effettuate una delle seguenti operazioni:

* Rimuovi manualmente le informazioni dal progetto dopo aver allegato il modello.

  Per informazioni, vedere [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md).

* Elimina nel progetto le attività aggiunte con il modello.

  Per informazioni, vedere la sezione [Eliminare le attività create da un modello](#delete-tasks-created-from-a-template) in questo articolo.

* Elimina il modello da Workfront. L’eliminazione del modello da Workfront non comporta l’eliminazione delle attività aggiunte dal modello dai progetti.

  Per informazioni, vedere [Elimina modelli di progetto](../../../manage-work/projects/create-and-manage-templates/delete-templates.md).

## Eliminare le attività create da un modello {#delete-tasks-created-from-a-template}

1. Vai alla sezione **Attività** del progetto.
1. Esegui una delle operazioni seguenti:

   * Creare un filtro per l&#39;elenco di task per visualizzare solo i task creati da un modello utilizzando l&#39;istruzione seguente:

     ```
     Task >> Template Task ID >>Is Not Blank
     ```

     Per informazioni sulla creazione di un filtro, vedere [Creare o modificare filtri in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

     Quando si applica il filtro, nell’elenco vengono visualizzate solo le attività associate a un ID attività modello.

   * Crea una visualizzazione per l&#39;elenco attività per visualizzare i campi **ID attività modello** o **Nome attività modello** in una colonna.

     Quando si applica la visualizzazione, le attività che contengono informazioni nella colonna ID attività modello o Nome attività modello sono state create utilizzando un modello.

     Per informazioni sulla creazione di una visualizzazione, vedere [Panoramica delle visualizzazioni in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. Seleziona tutte le attività identificate nel passaggio 2 come create da un modello, quindi fai clic su **icona Elimina**&#x200B;**> Sì, elimina**. Per ulteriori informazioni, vedere [Elimina attività](../../../manage-work/tasks/manage-tasks/delete-tasks.md).
