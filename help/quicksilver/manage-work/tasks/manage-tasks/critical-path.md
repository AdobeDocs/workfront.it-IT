---
content-type: overview
product-area: projects
navigation-topic: manage-tasks
title: Panoramica del percorso critico del progetto
description: La determinazione del percorso critico di un progetto consente ad Adobe Workfront di contrassegnare automaticamente una sequenza di attività in un progetto che possono influire sulla tempistica del progetto. Le attività che possono influire sulla timeline del progetto sono contrassegnate come attività del percorso critico.
author: Alina
feature: Work Management
exl-id: 9cbc84bf-d02b-4bb7-8d5d-922554d1262e
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '764'
ht-degree: 0%

---

# Panoramica del percorso critico del progetto

La determinazione del percorso critico di un progetto consente ad Adobe Workfront di contrassegnare automaticamente una sequenza di attività in un progetto che possono influire sulla tempistica del progetto. Le attività che possono influire sulla timeline del progetto sono contrassegnate come attività del percorso critico.

Le seguenti funzioni possono influire sul Percorso critico di un progetto:

* Struttura funzionale del progetto.

  Per ulteriori informazioni sulla struttura funzionale, vedere [Determinare la struttura funzionale in un progetto](../../../manage-work/projects/planning-a-project/determine-project-work-breakdown-structure.md)

* Tempo (durata) necessario per il completamento di ogni attività.
* Dipendenze tra le attività.

  Considera quanto segue:

   * Quando un&#39;attività sul percorso critico ha una relazione predecessore, i predecessori e i successori si trovano anche sul percorso critico se le modifiche alle date dei predecessori o dei successori influiscono direttamente sui rispettivi dipendenti.

     >[!TIP]
     >
     >Quando la data del successore di un&#39;attività non influisce direttamente sulla data delle attività dipendenti e non influisce sulle date del progetto, l&#39;attività successore non si trova nel Percorso Critico.
     >
     >
     >![](assets/successor-not-on-critical-path-350x150.png)     >
     >

   * Quando un&#39;attività secondaria viene identificata come attività Percorso critico, l&#39;attività padre viene identificata anche come attività Percorso critico, se la data e l&#39;ora di inizio previste dell&#39;attività padre corrispondono a quelle della sottoattività.

Tenendo conto di queste caratteristiche, il sistema calcola il percorso critico utilizzando il percorso più lungo tra l&#39;attività meno recente e l&#39;attività che determina la fine del progetto. Il calcolo del percorso critico tiene conto della data e dell&#39;ora in cui ogni attività può iniziare e finire senza prolungare il progetto. Questo processo determina quali attività sono &quot;critiche&quot; (e appartengono al percorso più lungo) e quali hanno &quot;fluttuazione totale&quot; (possono essere ritardate senza prolungare il progetto).

Qualsiasi ritardo nell’attività di un’attività sul percorso critico influisce direttamente sulla Data di completamento prevista del progetto (non esiste alcun valore mobile sul percorso critico).

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
   <td> <p>Accesso alle attività di visualizzazione o superiore</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizzare o modificare le autorizzazioni per un'attività </p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

## Visualizzare il percorso critico

È possibile visualizzare le attività che appartengono al percorso critico nelle seguenti aree dell&#39;applicazione Workfront:

* [Visualizza il percorso critico nel diagramma di Gantt](#view-the-critical-path-in-the-gantt-chart)
* [Visualizzare il percorso critico in un elenco di attività o in un report](#view-the-critical-path-in-a-task-list-or-report)

### Visualizzare il percorso critico nel diagramma di Gantt {#view-the-critical-path-in-the-gantt-chart}

Per visualizzare le attività sul Percorso critico nel diagramma di Gantt:

1. Passare a un progetto per il quale si desidera visualizzare il percorso critico.
1. Fai clic su **Attività** nel pannello a sinistra.
1. Fai clic sull&#39;icona **Grafico di Gantt** nell&#39;angolo superiore destro dell&#39;elenco delle attività.

   ![icona_grafico_gantt__1_.png](assets/gantt-chart-icon--1-.png)

1. Espandi il menu **Opzioni**, quindi abilita l&#39;opzione **Percorso critico**.

   Le attività che si trovano nel Percorso critico presentano una linea rossa sopra la linea temporale nel diagramma di Gantt.

   ![percorso_critico_su_gantt__1_.png](assets/crtitical-path-on-gantt--1--350x137.png)

### Visualizzare il percorso critico in un elenco di attività o in un report {#view-the-critical-path-in-a-task-list-or-report}

Per visualizzare quali attività si trovano nel percorso critico in un elenco di attività:

1. Passare a un progetto per il quale si desidera visualizzare il percorso critico.
1. Fai clic su **Attività** nel pannello a sinistra.
1. Dal menu a discesa **Visualizza**, selezionare **Stato**.

   Le attività presenti nel percorso critico hanno un flag **Percorso critico** nella colonna **Flag** dell&#39;elenco.

   È possibile applicare la stessa visualizzazione a un report attività.

   Per ulteriori informazioni sulla creazione di report, vedere l&#39;articolo [Creare un report personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

   Oppure

   Dal menu a discesa **Filtro**, selezionare **Nuovo filtro**.

1. Fai clic su **Aggiungi regola filtro** e inizia a digitare **È critico** in **Mostra solo le attività in cui il campo ...**.

1. Selezionala quando viene visualizzata nell’elenco.
1. Fai clic su **Salva filtro**.

   Nell&#39;elenco devono essere visualizzate solo le attività presenti nel percorso critico.
