---
content-type: overview
product-area: projects
navigation-topic: manage-tasks
title: Panoramica del percorso critico del progetto
description: La determinazione del percorso critico di un progetto consente ad Adobe Workfront di contrassegnare automaticamente una sequenza di attività in un progetto che possono influire sulla tempistica del progetto. Le attività che possono influire sulla timeline del progetto sono contrassegnate come attività del percorso critico.
author: Alina
feature: Work Management
exl-id: 9cbc84bf-d02b-4bb7-8d5d-922554d1262e
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '684'
ht-degree: 0%

---

# Panoramica del percorso critico del progetto

<!-- Audited: 5/2025 -->

La determinazione del percorso critico di un progetto consente ad Adobe Workfront di contrassegnare automaticamente una sequenza di attività in un progetto che possono influire sulla tempistica del progetto. Le attività che possono influire sulla sequenza temporale del progetto vengono contrassegnate come attività Percorso critico.

Le seguenti funzioni possono influire sul Percorso critico di un progetto:

* Struttura funzionale del progetto.

  Per ulteriori informazioni, vedere [Determinare la struttura di suddivisione del lavoro in un progetto](../../../manage-work/projects/planning-a-project/determine-project-work-breakdown-structure.md).

* Tempo (durata) necessario per il completamento di ogni attività.
* Dipendenze tra le attività.

  Considera quanto segue:

   * Quando un&#39;attività sul percorso critico ha una relazione predecessore, i predecessori e i successori si trovano anche sul percorso critico se le modifiche alle date dei predecessori o successori influiscono direttamente sui rispettivi dipendenti.

     >[!TIP]
     >
     >Quando la data del successore di un&#39;attività non influisce direttamente sulla data delle attività dipendenti o sulle date del progetto, l&#39;attività successore non si trova nel percorso critico.
     >
     >
     >![](assets/successor-not-on-critical-path-350x150.png)     >
     >

   * Quando un&#39;attività secondaria viene identificata come attività Percorso critico, l&#39;attività padre viene identificata anche come attività Percorso critico se la data di inizio prevista e l&#39;ora dell&#39;attività padre corrispondono a quelle della sottoattività.

Tenendo conto di queste caratteristiche, il sistema calcola il percorso critico utilizzando il percorso più lungo tra l&#39;attività meno recente e l&#39;attività che determina la fine del progetto. Il calcolo del percorso critico tiene conto della data e dell&#39;ora in cui ogni attività può iniziare e finire senza prolungare il progetto. Questo processo determina quali attività sono &quot;critiche&quot; (e appartengono al percorso più lungo) e quali hanno &quot;fluttuazione totale&quot; (possono essere ritardate senza prolungare il progetto).

Qualsiasi ritardo nell’attività di un’attività sul percorso critico influisce direttamente sulla Data di completamento prevista del progetto (non esiste alcun valore mobile sul percorso critico).

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
   <td> 
   <p>Standard<p>
   <p>Lavoro o superiore</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Accesso alle attività di visualizzazione o superiore</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizzare o modificare le autorizzazioni per un'attività </p></td> 
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
   <td role="rowheader">Adobe Workfront license</td> 
   <td> 
   <p>New: Standard<p>
   <p>Or</p>
   <p>Current: Work or higher</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>View or higher access to Tasks</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions on a task </p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Visualizzare il percorso critico

È possibile visualizzare le attività che appartengono al percorso critico nelle seguenti aree dell&#39;applicazione Workfront:

* [Visualizza il percorso critico nel diagramma di Gantt](#view-the-critical-path-in-the-gantt-chart)
* [Visualizzare il percorso critico in un elenco di attività o in un report](#view-the-critical-path-in-a-task-list-or-report)

### Visualizzare il percorso critico nel diagramma di Gantt {#view-the-critical-path-in-the-gantt-chart}

Per visualizzare le attività sul Percorso critico nel diagramma di Gantt:

{{step1-to-projects}}

1. Nell’elenco Progetto, seleziona un progetto.

1. Nel pannello a sinistra, fai clic su **Attività**. Viene visualizzata la scheda **Attività**.

1. Nell&#39;angolo superiore destro dell&#39;elenco attività fare clic sull&#39;icona **Grafico di Gantt**.

   ![icona_grafico_gantt__1_.png](assets/gantt-icon.png)

1. Nell&#39;angolo superiore destro della sezione del grafico Gantt fare clic sull&#39;icona **Opzioni** ![Opzioni](assets/options-icon.png), quindi selezionare l&#39;opzione **Percorso critico** nell&#39;elenco a discesa visualizzato. Le attività che si trovano sul Percorso Critico ora presentano una linea rossa sopra la timeline.

   ![percorso_critico_su_gantt__1_.png](assets/crtitical-path-on-gantt--1--350x137.png)

### Visualizzare il percorso critico in un elenco di attività o in un report {#view-the-critical-path-in-a-task-list-or-report}

Per visualizzare quali attività si trovano nel percorso critico in un elenco di attività:

{{step1-to-projects}}

1. Nell’elenco Progetto, seleziona un progetto.

1. Nel pannello a sinistra, fai clic su **Attività**. Viene visualizzata la scheda **Attività**.

1. Fai clic sull&#39;icona **Visualizza** ![Visualizza icona](assets/view-icon.png), quindi seleziona **Stato**. Le attività presenti nel percorso critico visualizzano un flag **Percorso critico** nella colonna **Flag** dell&#39;elenco.

   Oppure

   Fai clic sull&#39;icona **Filtro** ![Icona Filtri](assets/filters-icon.png), quindi seleziona **+ Nuovo filtro**.
1. Nel primo campo, digita *È critico*, quindi selezionalo quando viene visualizzato nella sezione **Attività** dell&#39;elenco.

   ![L&#39;attività è un filtro critico](assets/task-is-critical.png)

1. Verificare che **Is true** sia selezionato nel secondo menu a discesa.

   ![Elenco a discesa vero](assets/critical-path-filter.png)

1. Chiudete il pannello Filtri. Nell&#39;elenco delle attività vengono ora visualizzate solo le attività che si trovano nel Percorso critico.
