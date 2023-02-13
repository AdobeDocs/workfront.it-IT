---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Visualizza: dati relativi ai compiti e ai progetti di origine"'
description: Quando un problema viene convertito in un'attività o in un progetto, viene stabilita una relazione di risoluzione tra l'attività o il progetto e il problema. In questa visualizzazione vengono visualizzati i seguenti campi del problema che vengono completati automaticamente al completamento dell'attività o del progetto - EDIT ME.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 5fefb174-3a18-408f-aa12-3f4aff23acfa
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 3%

---

# Visualizza: dati relativi ai compiti e ai progetti originari

Quando un problema viene convertito in un&#39;attività o in un progetto, viene stabilita una relazione di risoluzione tra l&#39;attività o il progetto e il problema. In questa visualizzazione vengono visualizzati i seguenti campi del problema che vengono completati automaticamente al completamento dell&#39;attività o del progetto:

* Nome
* Data inserimento
* Data di completamento Pianificata
* Data di completamento effettiva
* Tipo di richiesta
* Nome dell&#39;autore
* Assegnato all&#39;utente

![task_with_resolve_issue_fields.png](assets/task-with-resolving-issue-fields-350x38.png)

Per ulteriori informazioni, consulta anche [Visualizza: visualizzare le informazioni originali sul problema negli elenchi di attività e progetti](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-original-issue-info-task-project-list.md).

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
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Accesso a rapporti, dashboard, calendari</p> <p>Modificare l’accesso a Filtri, Visualizzazioni, Gruppi</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Visualizza i dettagli del problema di origine per attività e progetti

1. Passare a un elenco di attività o a un elenco di progetti.
1. Da **Visualizza** menu a discesa, seleziona **Nuova vista**.

1. In **Anteprima a colonne** eliminare tutte le colonne tranne una.
1. Fai clic sull’intestazione della colonna rimanente, quindi fai clic su **Passa alla modalità testo**.
1. Passa il puntatore del mouse sull’area della modalità testo e fai clic su **Fare clic per modificare il testo**.
1. Rimuovi il testo che trovi nella **Modalità testo** e sostituirlo con il seguente codice:

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

1. Fai clic su **Salva visualizzazione**.
