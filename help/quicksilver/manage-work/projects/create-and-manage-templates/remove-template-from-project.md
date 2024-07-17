---
product-area: templates
navigation-topic: templates-navigation-topic
title: Rimuovere informazioni sul modello da un progetto
description: Impossibile rimuovere un modello da un progetto. È possibile rimuovere solo manualmente le informazioni aggiunte al progetto dopo che un modello è stato allegato al progetto. Per informazioni sull’associazione dei modelli, consulta Allegare un modello a un progetto.
author: Alina
feature: Work Management
exl-id: a8b6055a-7fac-4f9b-a880-10b2b85299b7
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '452'
ht-degree: 1%

---

# Rimuovere informazioni sul modello da un progetto

Impossibile rimuovere un modello da un progetto. È possibile rimuovere solo manualmente le informazioni aggiunte al progetto dopo che un modello è stato allegato al progetto. Per informazioni su come allegare i modelli, vedere [Allegare un modello a un progetto](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

## Requisiti di accesso

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
   <td> <p>Lavoro o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modifica l'accesso alle Attività</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire l’accesso alle attività </p> <p>Contribute o accesso successivo al progetto </p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

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

1. Seleziona tutte le attività identificate nel passaggio 2 come create da un modello, quindi fai clic su **icona Elimina****> Sì, elimina**. Per ulteriori informazioni, vedere [Elimina attività](../../../manage-work/tasks/manage-tasks/delete-tasks.md).
