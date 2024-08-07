---
product-area: projects;agile-and-teams
navigation-topic: manage-projects
title: Gestire un progetto nella visualizzazione Agile
description: Puoi sfruttare le funzionalità agili per il tuo progetto senza le problematiche amministrative che in genere accompagnano le procedure agili (come la gestione del backlog di un team o la creazione di iterazioni).
author: Alina and Lisa
feature: Work Management
exl-id: fc633fd6-35b4-4949-8045-22c775002436
source-git-commit: 84c5772d130be78d9f9b9aef342c57183d5ec985
workflow-type: tm+mt
source-wordcount: '1423'
ht-degree: 0%

---

# Gestire un progetto nella visualizzazione Agile

<!-- Audited: 2/2024 -->

Puoi sfruttare le funzionalità agili per il tuo progetto senza le problematiche amministrative che in genere accompagnano le procedure agili (come la gestione del backlog di un team o la creazione di iterazioni).

Se si desidera lavorare in un ambiente agile che utilizza un backlog team e consente di creare iterazioni dalle attività nel backlog, seguire le istruzioni in [Operazioni in un ambiente agile](../../../agile/work-in-an-agile-environment/work-in-an-agile-environment.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

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
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> <p>Corrente: revisione o versione successiva</p> 
   <p>Nuovo: Collaboratore o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazione del livello di accesso</td> 
   <td> <p>Modifica accesso alle seguenti aree:</p> 
    <ul> 
     <li> <p>Progetti</p> </li> 
     <li> <p>Report, dashboard, calendari</p> </li> 
     <li> <p>Filtri, Viste, Raggruppamenti</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizzare le autorizzazioni per il progetto</p>  </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Comprendere i progetti Agile

>[!NOTE]
>
>Questa sezione si applica solo alla vista Agile legacy, non alla vista bacheca di un progetto.

* [Funzionalità Agile in un progetto](#agile-functionality-in-a-project)
* [Differenze quando si utilizza la vista Agile su un progetto rispetto a un’iterazione](#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration)

### Funzionalità Agile in un progetto {#agile-functionality-in-a-project}

La seguente funzionalità agile è disponibile quando gestisci un progetto in una visualizzazione agile:

* Stato di completamento\
  Per informazioni più dettagliate sullo stato di completamento, vedere [Panoramica sullo stato di completamento dell&#39;iterazione](../../../agile/use-scrum-in-an-agile-team/burndown/iteration-completion-status-overview.md).

* Storyboard\
  Per informazioni più dettagliate sulla bacheca delle storie, consulta la sezione [Bacheca Scrum](../../../agile/use-scrum-in-an-agile-team/scrum-board/scrum-board.md).

Esistono alcune differenze quando si utilizzano visualizzazioni agili su un progetto anziché in un ambiente agile puro (con backlog e iterazioni). Per ulteriori informazioni, vedi [Differenze quando utilizzi la visualizzazione Agile su un progetto rispetto a un&#39;iterazione](#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration) in questo articolo.

### Differenze quando si utilizza la vista Agile su un progetto rispetto a un’iterazione {#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration}

* [Le attività e le sottoattività seguono regole di visualizzazione diverse in una visualizzazione Agile del progetto e nella bacheca delle storie di un&#39;iterazione](#tasks-and-subtasks-follow-different-display-rules-on-the-story-board)
* [Backlog e iterazioni non utilizzati nella visualizzazione Agile](#backlogs-and-iterations-are-not-used)
* [L&#39;ordine attività è mantenuto nella visualizzazione Agile e non può essere riordinato](#task-order-is-maintained-in-the-agile-view-and-cannot-be-reordered)
* [Le attività sono misurate solo nelle ore pianificate in un elenco di progetti](#tasks-are-measured-only-in-planned-hours)
* [Il team Agile non è utilizzato in una visualizzazione Agile](#the-agile-team-is-not-used)
* [Ogni utente del progetto può visualizzare il progetto in una visualizzazione Agile diversa](#each-user-on-the-project-can-view-the-project-in-a-different-agile-view)

#### Le attività e le sottoattività seguono regole di visualizzazione diverse in una visualizzazione Agile del progetto e nella bacheca delle storie di un&#39;iterazione {#tasks-and-subtasks-follow-different-display-rules-on-the-story-board}

* Le attività che non hanno né un&#39;attività padre né un&#39;attività secondaria vengono sempre visualizzate come una scheda a brano singolo nella bacheca delle storie della visualizzazione Agile.\
  Ad esempio, nella vista a elenco dei progetti vengono visualizzate le seguenti attività:

  ![Elenco progetti Agile - attività senza attività padre o sottoattività](assets/agile-project-single-list-nwe.png)

  Queste attività vengono visualizzate come segue nella visualizzazione agile del progetto:

  ![Visualizzazione agile progetto - attività senza attività padre o sottoattività](assets/agile-project-singlecard-nwe.png)

* Le attività padre con sottoattività vengono sempre visualizzate nella colonna **Storie** della bacheca delle storie della visualizzazione Agile. Le sottoattività vengono visualizzate nella corsia preferenziale dell&#39;attività padre.\
  Ad esempio, nella vista a elenco dei progetti vengono visualizzate le seguenti attività:

  ![Elenco progetti Agile - Attività con attività padre e sottoattività](assets/agile-project-parent-list-nwe.png)\
  Queste attività vengono visualizzate come segue nella visualizzazione agile del progetto:

  ![Visualizzazione progetto agile - attività con attività padre e sottoattività](assets/agile-project-parent-nwe.png)

* Le sottoattività di secondo livello (sottoattività delle sottoattività) vengono visualizzate come una scheda grigia sporgente rispetto all’attività padre immediata.
* Le sottoattività di terzo livello (sottoattività delle sottoattività delle sottoattività) non vengono mai visualizzate nella visualizzazione Agile.

#### I backlog e le iterazioni non vengono utilizzati nella visualizzazione Agile {#backlogs-and-iterations-are-not-used}

Quando si visualizza un progetto in una visualizzazione agile, i seguenti componenti agile non vengono utilizzati:

* **Backlog:** non viene utilizzato alcun backlog perché tutte le attività del progetto vengono visualizzate automaticamente come storie.
* **Iterazioni:** Anziché creare iterazioni per definire le date di completamento del lavoro, i giorni attualmente designati nella sequenza temporale del progetto diventano i giorni lavorativi.

#### L&#39;ordine delle attività viene mantenuto nella vista Agile e non può essere riordinato {#task-order-is-maintained-in-the-agile-view-and-cannot-be-reordered}

L&#39;ordine in cui le attività vengono visualizzate in un progetto viene mantenuto quando si visualizza il progetto in una bacheca delle storie agile.

Non è possibile riordinare le attività nel progetto quando si visualizza il progetto in una visualizzazione agile. Poiché la modifica dell&#39;ordine delle attività può influire su altre attività che potrebbero avere dipendenze, è necessario visualizzare il progetto in una visualizzazione standard per modificare l&#39;ordine delle attività.

#### Le attività vengono misurate solo nelle ore pianificate in un elenco di progetti {#tasks-are-measured-only-in-planned-hours}

Le attività di un progetto sono sempre misurate in Ore Pianificate.

In un’iterazione, le attività (storie) possono essere misurate in ore o punti.

#### Il team Agile non viene utilizzato in una visualizzazione Agile {#the-agile-team-is-not-used}

Poiché i team Agile completano il lavoro sulle iterazioni loro assegnate, non vengono utilizzati quando si visualizza un progetto in una visualizzazione Agile.

Invece, tutti gli utenti del progetto diventano essenzialmente il team agile di quel progetto.

#### Ogni utente del progetto può visualizzare il progetto in una visualizzazione Agile diversa {#each-user-on-the-project-can-view-the-project-in-a-different-agile-view}

A differenza di un’iterazione agile, gli utenti di un progetto possono personalizzare la visualizzazione agile autonomamente, mentre altri utenti utilizzano una visualizzazione agile diversa.

In un’iterazione Agile, le informazioni disponibili sullo storyboard Agile (come le colonne di stato disponibili) vengono determinate a livello di team.

Per informazioni su come personalizzare una visualizzazione Agile, vedere [Creare o personalizzare una visualizzazione Agile](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md#create-or-customize-an-agile-view) in [Creare o modificare le visualizzazioni in in Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

## Visualizzare un progetto nella visualizzazione Agile

1. Vai al progetto che desideri visualizzare in una visualizzazione agile, sull’elenco delle attività o sull’elenco dei problemi.
1. Fai clic sull&#39;icona **Vista bacheca** ![Icona bacheca](assets/board-icon-for-agile-view.png).

   La vista bacheca del progetto viene visualizzata per impostazione predefinita.

   ![Visualizzazione bacheca del progetto](assets/project-agile-board-view.png)

   <!--(Legacy agile view only) If you previously viewed the project in a custom agile view, the project is displayed in that view rather than in the default agile view.-->

1. (Facoltativo) Fai clic su **Configura** per impostare le opzioni per le colonne e le schede.

   Per ulteriori informazioni, vedere [Gestire le colonne della bacheca](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md) e [Personalizzare i campi visualizzati in una scheda](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md). Non è possibile definire i criteri di colonna nella vista bacheca di un progetto.

1. (Facoltativo) Fai clic su **Usa agile legacy** per utilizzare la visualizzazione agile legacy invece della visualizzazione bacheca.

1. (Facoltativo - solo vista agile legacy) Se hai creato una vista agile personalizzata o se un altro utente ha creato una vista agile personalizzata e l’ha condivisa con te, puoi visualizzarla al posto della vista agile predefinita.

   Fai clic sul menu a discesa **Visualizza**, quindi fai clic sulla visualizzazione agile personalizzata che desideri visualizzare.

   La visualizzazione agile personalizzata verrà utilizzata alla successiva selezione dell&#39;icona **Agile**.

   Per informazioni su come creare una nuova visualizzazione Agile, vedi [Creare e personalizzare le visualizzazioni Agile](#create-and-customize-agile-views), di seguito.

   Il progetto viene visualizzato nella visualizzazione agile personalizzata.

1. (Condizionale - solo per la visualizzazione agile legacy) Se le attività nel progetto utilizzano stati diversi da &quot;Nuovo&quot;, &quot;In corso&quot; o &quot;Completo&quot; (stati predefiniti per la visualizzazione agile), è necessario aggiungere gli stati aggiuntivi alla visualizzazione agile affinché vengano visualizzate tutte le attività con tali stati.

   Se le attività si trovano in uno stato che non viene visualizzato sullo storyboard Agile, l&#39;attività stessa non viene visualizzata sullo storyboard Agile (tuttavia, la percentuale di completamento di queste attività contribuisce ancora alla percentuale di completamento di tutte le attività padre e alla percentuale di completamento del progetto complessivo).

   Per aggiungere stati alla visualizzazione Agile, creare una nuova visualizzazione Agile o personalizzare una visualizzazione Agile esistente, come descritto in [Creare e personalizzare le visualizzazioni Agile](#create-and-customize-agile-views), di seguito.

1. (Facoltativo) Per tornare alla vista a elenco, fai clic sull&#39;icona **Elenco**.

## Creare e personalizzare viste Agile {#create-and-customize-agile-views}

>[!NOTE]
>
>Questa sezione si applica solo alla vista Agile legacy, non alla vista bacheca di un progetto.

Come per le viste standard in Workfront, puoi personalizzare le viste agili esistenti o crearne di nuove da zero. A differenza delle viste standard, non è possibile creare nuove viste agili basate su viste agili esistenti.

Per ulteriori informazioni sulla creazione e la personalizzazione delle visualizzazioni Agile, vedere la sezione [Creare o personalizzare una visualizzazione Agile](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md#create-or-customize-an-agile-view) nell&#39;articolo [Creare o modificare le visualizzazioni in in Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

## Condividere una visualizzazione Agile esistente

>[!NOTE]
>
>Questa sezione si applica solo alla vista Agile legacy, non alla vista bacheca di un progetto.

Puoi condividere una visualizzazione Agile creata o disporre delle autorizzazioni necessarie nello stesso modo in cui condividi qualsiasi altra visualizzazione, filtro o raggruppamento.

Per ulteriori informazioni, vedere [Condividere un filtro, una visualizzazione o un raggruppamento](../../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).

## Rimuovi una vista Agile esistente

>[!NOTE]
>
>Questa sezione si applica solo alla vista Agile legacy, non alla vista bacheca di un progetto.

È possibile rimuovere una visualizzazione Agile nello stesso modo in cui si rimuove qualsiasi altra visualizzazione, filtro o raggruppamento.

Per ulteriori informazioni, vedere [Rimuovere filtri, visualizzazioni e raggruppamenti](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/remove-filters-views-groupings.md).
