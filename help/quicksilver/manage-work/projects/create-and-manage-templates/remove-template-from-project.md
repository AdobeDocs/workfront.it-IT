---
product-area: templates
navigation-topic: templates-navigation-topic
title: Rimuovere informazioni sul modello da un progetto
description: Non è possibile rimuovere un modello da un progetto. Puoi rimuovere manualmente solo le informazioni aggiunte al progetto dopo l’aggiunta di un modello al progetto. Per informazioni sull’associazione dei modelli, consulta Allegare un modello a un progetto.
author: Alina
feature: Work Management
exl-id: a8b6055a-7fac-4f9b-a880-10b2b85299b7
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 1%

---

# Rimuovere informazioni sul modello da un progetto

Non è possibile rimuovere un modello da un progetto. Puoi rimuovere manualmente solo le informazioni aggiunte al progetto dopo l’aggiunta di un modello al progetto. Per informazioni sull&#39;associazione dei modelli, consulta [Allegare un modello a un progetto](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Lavoro o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica accesso alle attività</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestione dell’accesso alle attività </p> <p>Contribuire o un accesso più elevato al progetto </p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Opzioni per rimuovere le informazioni sui modelli da un progetto

Per rimuovere le informazioni sui modelli aggiunte al progetto, puoi effettuare una delle seguenti operazioni:

* Rimuovi manualmente le informazioni dal progetto dopo che il modello è stato allegato.

   Per informazioni, consulta [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md).

* Elimina le attività nel progetto aggiunte con il modello.

   Per informazioni, consulta la sezione [Eliminare le attività create da un modello](#delete-tasks-created-from-a-template) in questo articolo.

* Elimina il modello da Workfront. L’eliminazione del modello da Workfront non comporta l’eliminazione delle attività aggiunte dal modello dai progetti.

   Per informazioni, consulta [Eliminare i modelli di progetto](../../../manage-work/projects/create-and-manage-templates/delete-templates.md).

## Eliminare le attività create da un modello {#delete-tasks-created-from-a-template}

1. Vai a **Attività** sezione del progetto.
1. Esegui una delle operazioni seguenti:

   * Creare un filtro per l&#39;elenco delle attività per visualizzare solo le attività create da un modello utilizzando l&#39;istruzione seguente:

      ```
      Task >> Template Task ID >>Is Not Blank
      ```

      Per informazioni sulla creazione di un filtro, consulta [Creare o modificare filtri in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

      Quando si applica il filtro, nell’elenco vengono visualizzate solo le attività associate a un ID attività modello.

   * Crea una visualizzazione per l&#39;elenco delle attività per visualizzare il **ID attività modello** o **Nome attività modello** in una colonna.

      Quando si applica la visualizzazione, le attività che contengono informazioni nella colonna ID attività modello o nome attività modello sono state create utilizzando un modello.

      Per informazioni sulla creazione di una visualizzazione, vedi [Panoramica delle visualizzazioni in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. Seleziona tutte le attività identificate nel Passaggio 2 come create da un modello, quindi fai clic su **Icona Elimina****> Sì, Elimina**. Per ulteriori informazioni, consulta [Elimina attività](../../../manage-work/tasks/manage-tasks/delete-tasks.md).
