---
content-type: overview
product-area: projects
navigation-topic: manage-tasks
title: Panoramica del progetto Percorso critico
description: La determinazione del percorso critico di un progetto è un modo automatico per Adobe Workfront di contrassegnare una sequenza di attività in un progetto che possono avere un impatto sulla timeline del progetto. Le attività che possono influenzare la cronologia del progetto vengono contrassegnate come attività di percorso critico.
author: Alina
feature: Work Management
exl-id: 9cbc84bf-d02b-4bb7-8d5d-922554d1262e
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '771'
ht-degree: 0%

---

# Panoramica del progetto Percorso critico

La determinazione del percorso critico di un progetto è un modo automatico per Adobe Workfront di contrassegnare una sequenza di attività in un progetto che possono avere un impatto sulla timeline del progetto. Le attività che possono influenzare la cronologia del progetto vengono contrassegnate come attività di percorso critico.

Le seguenti funzionalità possono influire sul percorso critico di un progetto:

* Struttura di suddivisione del lavoro del progetto.

   Per ulteriori informazioni sulla struttura di suddivisione del lavoro, consulta [Determinare la struttura di suddivisione del lavoro in un progetto](../../../manage-work/projects/planning-a-project/determine-project-work-breakdown-structure.md)

* Tempo (durata) necessario per completare ciascuna attività.
* Dipendenze tra le attività.

   Considera quanto segue:

   * Quando un&#39;attività sul percorso critico ha una relazione predecessore, i suoi predecessori e successori sono anche sul percorso critico se le modifiche alle date dei predecessori o dei successori influiscono direttamente sui loro dipendenti.

      >[!TIP]
      >
      >Quando la data del successore di un&#39;attività non influisce direttamente sulla data dei loro compiti dipendenti e non influisce sulle date del progetto, l&#39;attività successore non è nel percorso critico.
      >
      >
      >![](assets/successor-not-on-critical-path-350x150.png)     >

   * Quando un&#39;attività secondaria viene identificata come attività di percorso critico, l&#39;attività principale viene identificata anche come attività di percorso critico, se la data e l&#39;ora di inizio prevista dell&#39;attività principale sono uguali a quella dell&#39;attività secondaria.

Tenendo conto di queste funzioni, il sistema calcola il percorso critico utilizzando il percorso più lungo tra il primo task e il task che determina la fine del progetto. Il calcolo del percorso critico tiene conto del primo e ultimo momento in cui ogni attività può iniziare e terminare senza prolungare il progetto. Questo processo determina quali attività sono &quot;critiche&quot; (e appartengono al percorso più lungo) e quali hanno &quot;float totale&quot; (possono essere ritardate senza prolungare il progetto).

Qualsiasi ritardo nell&#39;attività di un&#39;attività sul percorso critico influisce direttamente sulla data di completamento prevista del progetto (non c&#39;è galleggiamento nel percorso critico).

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
   <td> <p>Visualizzazione o accesso superiore alle attività</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizza o autorizzazioni superiori per un'attività </p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Visualizza il percorso critico

È possibile visualizzare le attività che appartengono al Percorso critico nelle seguenti aree dell&#39;applicazione Workfront:

* [Visualizzare il percorso critico nel diagramma di Gantt](#view-the-critical-path-in-the-gantt-chart)
* [Visualizzare il percorso critico in un elenco di attività o in un report](#view-the-critical-path-in-a-task-list-or-report)

### Visualizzare il percorso critico nel diagramma di Gantt {#view-the-critical-path-in-the-gantt-chart}

Per visualizzare le attività nel percorso critico nel diagramma di Gantt:

1. Passa a un progetto per il quale desideri visualizzare il percorso critico.
1. Fai clic su **Attività** nel pannello a sinistra.
1. Fai clic sul pulsante **Diagramma di Gantt** nell&#39;angolo superiore destro dell&#39;elenco delle attività.

   ![gantt_graph_icon_1_.png](assets/gantt-chart-icon--1-.png)

1. Espandi la **Opzioni** quindi abilita il **Percorso critico** opzione .

   Le attività che si trovano nel percorso critico hanno una linea rossa sopra la propria linea temporale nel diagramma di Gantt.

   ![crtitical_path_on_gantt__1_.png](assets/crtitical-path-on-gantt--1--350x137.png)

### Visualizzare il percorso critico in un elenco di attività o in un report {#view-the-critical-path-in-a-task-list-or-report}

Per visualizzare quali attività si trovano nel percorso critico in un elenco di attività:

1. Passa a un progetto per il quale desideri visualizzare il percorso critico.
1. Fai clic su **Attività** nel pannello a sinistra.
1. Da **Visualizza** menu a discesa, seleziona **Stato**.

   Le attività che si trovano nel percorso critico hanno un **Percorso critico** la bandiera **Flag** della lista.

   È possibile applicare la stessa visualizzazione a un report attività.

   Per ulteriori informazioni sulla creazione di rapporti, consulta l’articolo [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

   Oppure

   Da **Filtro** menu a discesa, seleziona **Nuovo filtro**.

1. Fai clic su **Aggiungi regola filtro** e inizia a digitare **È critico** in **Mostrami solo le attività in cui ...** campo .

1. Selezionalo quando viene visualizzato nell’elenco.
1. Fai clic su **Salva filtro**.

   Nell&#39;elenco devono essere visualizzate solo le attività presenti nel percorso critico.
