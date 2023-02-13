---
product-area: projects;agile-and-teams
navigation-topic: manage-projects
title: Gestire un progetto nella vista Agile
description: Piani, tipi di licenza richiesti e accesso alle autorizzazioni Adobe Workfront Plan Team, Pro, Business o Enterprise Workfront License Type Review, Work o Plan nel modello di accesso Modifica l'accesso e la possibilità di creare report, dashboard e calendari
author: Alina
feature: Work Management
exl-id: fc633fd6-35b4-4949-8045-22c775002436
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '1311'
ht-degree: 0%

---

# Gestire un progetto nella vista Agile

Piani, tipi di licenza e accesso richiesti

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><a href="https://www.workfront.com/plans" target="_blank">Piano Adobe Workfront</a> </p> </td> 
   <td> <p>Team, Pro, Business o Enterprise </p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="https://one.workfront.com/s/article/Understanding-License-Types-906212506?language=en_US&amp;r=16&amp;ui-comm-runtime-components-aura-components-siteforce-qb.Quarterback.validateRoute=1&amp;ui-communities-components-aura-components-forceCommunity-breadcrumbs.Breadcrumbs.getAncestors=1&amp;ui-communities-components-aura-components-forceCommunity-seoAssistant.SeoAssistant.getSeoData=1&amp;ui-force-components-controllers-recordGlobalValueProvider.RecordGvp.getRecord=1&amp;ui-self-service-components-controller.ArticleTopicList.getTopics=1&amp;ui-self-service-components-controller.ArticleView.getArticleHeaderDetail=1" target="_blank">Tipo di licenza Workfront</a> </p> </td> 
   <td> <p>Revisione, lavoro o piano </p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> <p>Permissions in the access model</p> </td> 
    <td> <li>Edit access and ability to create reports, dashboards, and calendars</li> </td> 
   </tr>
  --> 
 </tbody> 
</table>

Puoi sfruttare la funzionalità agile per il tuo progetto

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(such as story boards and burndown charts)
</MadCap:conditionalText>
-->

 senza le problematiche amministrative che solitamente accompagnano le pratiche agili (ad esempio la gestione di un backlog del team o la creazione di iterazioni).

Se desideri lavorare in un ambiente agile che utilizza un backlog del team e ti consente di creare iterazioni dalle attività nel backlog, segui le istruzioni in [Lavorare in un ambiente agile](../../../agile/work-in-an-agile-environment/work-in-an-agile-environment.md).

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
   <td> <p>Revisione o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica l’accesso alle seguenti aree:</p> 
    <ul> 
     <li> <p>Progetti</p> </li> 
     <li> <p>Report, dashboard, calendari</p> </li> 
     <li> <p>Filtri, Visualizzazioni, Raggruppamenti</p> </li> 
    </ul> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizza le autorizzazioni per il progetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Comprendere i progetti Agile

* [Funzionalità di base in un progetto](#agile-functionality-in-a-project)
* [Differenze quando si utilizza la vista Agile su un progetto rispetto a un&#39;iterazione](#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration)

### Funzionalità di base in un progetto {#agile-functionality-in-a-project}

La seguente funzionalità agile è disponibile quando gestisci un progetto in una visualizzazione agile:

* Stato di completamento\
   Per informazioni più dettagliate sullo stato di completamento, vedi [Panoramica sullo stato di completamento dell&#39;iterazione](../../../agile/use-scrum-in-an-agile-team/burndown/iteration-completion-status-overview.md).

* Scheda di storia\
   Per informazioni più dettagliate sulla bacheca delle storie, consultate la [Scrum board](../../../agile/use-scrum-in-an-agile-team/scrum-board/scrum-board.md) sezione .

Esistono alcune differenze quando si utilizzano visualizzazioni agili su un progetto rispetto a quando si lavora in un ambiente agile puro (con backlog e iterazioni). Per ulteriori informazioni, consulta [Differenze quando si utilizza la vista Agile su un progetto rispetto a un&#39;iterazione](#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration) in questo articolo.

### Differenze quando si utilizza la vista Agile su un progetto rispetto a un&#39;iterazione {#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration}

* [Le attività e le sottoattività seguono diverse regole di visualizzazione nel pannello Story](#tasks-and-subtasks-follow-different-display-rules-on-the-story-board)
* [Backlog e iterazioni non utilizzati](#backlogs-and-iterations-are-not-used)
* [L&#39;ordine delle attività viene mantenuto nella visualizzazione Agile e non può essere riordinato](#task-order-is-maintained-in-the-agile-view-and-cannot-be-reordered)
* [Le attività vengono misurate solo in orari pianificati](#tasks-are-measured-only-in-planned-hours)
* [Agile Team non utilizzato](#the-agile-team-is-not-used)
* [Ogni utente del progetto può visualizzare il progetto in una visualizzazione Agile diversa](#each-user-on-the-project-can-view-the-project-in-a-different-agile-view)

#### Le attività e le sottoattività seguono diverse regole di visualizzazione nel pannello Story {#tasks-and-subtasks-follow-different-display-rules-on-the-story-board}

* Le attività che non hanno un&#39;attività padre né una sottoattività vengono sempre visualizzate come una singola scheda del brano sulla bacheca del racconto.\
   Ad esempio, queste attività vengono visualizzate come segue nella vista a elenco dei progetti:

   ![Elenco dei progetti Agile: attività prive di attività padre o secondarie](assets/agile-project-single-list-nwe.png) Queste attività vengono visualizzate come segue nella visualizzazione agile del progetto:

   ![Visualizzazione agile progetto: attività prive di attività padre o secondarie](assets/agile-project-singlecard-nwe.png)

* Le attività padre con sottoattività vengono sempre visualizzate nel **Storie** colonna della trama. Le sottoattività vengono visualizzate nel riquadro a tendina dell&#39;attività principale.\
   Ad esempio, queste attività vengono visualizzate come segue nella vista a elenco dei progetti:

   ![Elenco dei progetti Agile - Attività con elementi principali e secondari](assets/agile-project-parent-list-nwe.png)\
   Queste attività vengono visualizzate come segue nella visualizzazione agile del progetto:

   ![Visualizzazione del progetto Agile: attività con elementi principali e secondari](assets/agile-project-parent-nwe.png)

* Le sottoattività di secondo livello (sottoattività delle sottoattività) vengono visualizzate come una scheda grigia sporgente dell&#39;attività principale immediata.
* Le sottoattività di terzo livello (sottoattività delle sottoattività delle sottoattività) non vengono mai visualizzate nel storyboard.

#### Backlog e iterazioni non utilizzati {#backlogs-and-iterations-are-not-used}

Quando si visualizza un progetto in una visualizzazione agile, non vengono utilizzati i seguenti componenti agili:

* **Backlog:** Non viene utilizzato alcun backlog perché tutte le attività del progetto vengono visualizzate automaticamente come storie.
* **Iterazioni:** Invece di creare iterazioni per definire le date in cui verrà eseguito il lavoro, i giorni attualmente indicati nella timeline del progetto diventano i giorni lavorativi.

#### L&#39;ordine delle attività viene mantenuto nella visualizzazione Agile e non può essere riordinato {#task-order-is-maintained-in-the-agile-view-and-cannot-be-reordered}

L&#39;ordine in cui le attività vengono visualizzate in un progetto viene mantenuto quando si visualizza il progetto in una bacheca di storie agili.

Non è possibile riordinare le attività del progetto quando lo si visualizza in una visualizzazione agile. Poiché la modifica dell’ordine delle attività può influire su altre attività che potrebbero avere dipendenze, è necessario visualizzare il progetto in una visualizzazione standard per modificare l’ordine delle attività.

#### Le attività vengono misurate solo in orari pianificati {#tasks-are-measured-only-in-planned-hours}

Le attività di un progetto vengono sempre misurate in Orari pianificati.

In un&#39;iterazione, le attività (storie) possono essere misurate in ore o punti.

#### Agile Team non utilizzato {#the-agile-team-is-not-used}

Poiché i team agili completano il lavoro sulle iterazioni assegnate loro, i team agili non vengono utilizzati quando si visualizza un progetto in una visualizzazione agile.

Invece, tutti gli utenti del progetto diventano essenzialmente il team agile per quel progetto.

#### Ogni utente del progetto può visualizzare il progetto in una visualizzazione Agile diversa {#each-user-on-the-project-can-view-the-project-in-a-different-agile-view}

A differenza di un’iterazione agile, gli utenti di un progetto possono personalizzare autonomamente la visualizzazione agile, mentre altri utenti utilizzano una visualizzazione agile diversa.

In un&#39;iterazione agile, le informazioni disponibili sulla scheda di storia agile (ad esempio le colonne di stato disponibili) vengono determinate a livello di gruppo.

Per informazioni su come personalizzare una visualizzazione agile, consulta  [Creare o personalizzare una visualizzazione Agile](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-an-agile-view) in  [Panoramica delle visualizzazioni in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md). 

## Visualizzare un progetto nella vista Agile

1. Passa al progetto da visualizzare in una visualizzazione agile.
1. Fai clic sul pulsante **Agile** icona.\
   ![Icona Agile](assets/agile-icon-nwe.png)\
   Il progetto viene visualizzato nella visualizzazione agile predefinita.\
   Se in precedenza hai visualizzato il progetto in una visualizzazione agile personalizzata, il progetto viene visualizzato in tale visualizzazione anziché nella visualizzazione agile predefinita.

1. (Facoltativo) Se hai creato una visualizzazione agile personalizzata o se un altro utente ha creato una visualizzazione agile personalizzata e l&#39;ha condivisa con te, puoi visualizzarla invece della visualizzazione agile predefinita.\
   Fai clic sul pulsante **Visualizza** menu a discesa, quindi fare clic sulla visualizzazione agile personalizzata che si desidera visualizzare.

   La visualizzazione agile personalizzata viene utilizzata la prossima volta che fai clic sul pulsante **Agile** icona.\
   Per informazioni su come creare una nuova visualizzazione agile, vedi [Creare e personalizzare le visualizzazioni Agile](#create-and-customize-agile-views).\
   Il progetto viene visualizzato nella visualizzazione agile personalizzata.

1. (Condizionale) Se le attività del progetto utilizzano stati diversi da &quot;Nuovo&quot;, &quot;In corso&quot; o &quot;Completo&quot; (gli stati predefiniti per la visualizzazione Agile), è necessario aggiungere gli stati aggiuntivi alla visualizzazione agile per visualizzare eventuali attività in tali stati.\
   Se le attività si trovano in uno stato che non viene visualizzato nella tabella delle storie agili, l&#39;attività stessa non viene visualizzata nella tabella delle storie agili (tuttavia, la percentuale di completamento di queste attività contribuisce comunque alla percentuale di completamento di tutte le attività padre e alla percentuale di completamento del progetto complessivo).\
   Per aggiungere stati alla visualizzazione agile, crea una nuova visualizzazione agile o personalizza una visualizzazione agile esistente, come descritto nella sezione &quot;Crea o personalizza una visualizzazione Agile&quot; dell’articolo [Panoramica delle visualizzazioni in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. (Facoltativo) Per tornare alla vista Elenco, fai clic sul pulsante **Elenco** icona.\
   ![](assets/list-icon.png)

## Creare e personalizzare le visualizzazioni Agile {#create-and-customize-agile-views}

Come per le viste standard in Workfront, puoi personalizzare le visualizzazioni agili esistenti o creare nuove visualizzazioni agili da zero. A differenza delle viste standard, non è possibile creare nuove visualizzazioni agili basate sulle visualizzazioni agili esistenti.

Per ulteriori informazioni sulla creazione e la personalizzazione delle visualizzazioni agili, consulta la sezione &quot;Creare o personalizzare una visualizzazione Agile&quot; nell’articolo [Panoramica delle visualizzazioni in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md). 

## Condividere una visualizzazione Agile esistente

Per informazioni su come condividere una visualizzazione agile, vedi [Condividere un filtro, una visualizzazione o un raggruppamento](../../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).

## Rimuovere una visualizzazione Agile esistente

Per informazioni su come eliminare una visualizzazione, consulta la sezione &quot;Rimuovere una visualizzazione&quot; nell’articolo [Panoramica delle visualizzazioni in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md). 
