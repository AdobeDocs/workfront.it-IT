---
content-type: overview;how-to-procedural
product-area: projects
keywords: analisi,metriche,progetto,attività,assegnatario,completo,stato,scaduto,in arrivo
navigation-topic: manage-projects
title: Comprendere le metriche del progetto
description: Le metriche del progetto forniscono una visualizzazione di ciò che accade in un progetto, consentendo di valutare rapidamente le esigenze e lo stato di un progetto. Scopri come interpretare l’area Metriche nel pannello a sinistra di un progetto.
author: Alina
feature: Work Management
exl-id: 54c2a59d-9f6b-4126-9526-5169aeda8517
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '1161'
ht-degree: 0%

---

# Comprendere le metriche del progetto

Le metriche di progetto forniscono una visualizzazione generale in formato grafico delle prestazioni di un progetto.

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
   <td> <p>Chiaro o superiore</p>
   <p>Revisione o successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Accesso ai progetti in visualizzazione</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizzare le autorizzazioni per un progetto</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per ulteriori informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront license*</td> 
   <td> <p>New: Light or higher </p>
   <p>Current: Review or higher </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configuration</td> 
   <td> <p>View access to Projects</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to a project</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Prerequisiti

Per accedere all’area Metriche dal pannello a sinistra di un progetto, devi:

* Abilitare l’opzione Metriche del pannello sinistro nell’area Progetti del modello di layout.

  Per informazioni su come un amministratore di Workfront o un amministratore di gruppi può personalizzare il pannello sinistro con un modello di layout, vedere [Personalizzare il pannello sinistro utilizzando un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md).

## Panoramica dell’area Metriche del progetto

Le metriche del progetto forniscono una visualizzazione di ciò che accade in un progetto, consentendo di valutare rapidamente le esigenze e lo stato di un progetto.

![](assets/project-metrics-full-screen-350x238.png)

Nell’area Metriche puoi vedere lo stato complessivo di un progetto e:

* Dove il lavoro è attivo o bloccato
* A chi sono assegnati elementi di lavoro aperti
* Dettagli sulle attività o sui problemi scaduti o prossimi alla Data di completamento pianificata

È inoltre possibile espandere ogni grafico per esaminare più da vicino le attività o i problemi relativi a una categoria specifica.

Per ulteriori informazioni su come esaminare queste attività o questi problemi, consulta [Visualizza dettagli metriche](#view-metrics-details).

<!--this was deprecated: 
>[!TIP]
>
>To see metrics at a higher level for a group of projects within a program, portfolio, etc., navigate to the Enhanced analytics area.  
>To learn more about Enhanced analytics, see [Enhanced analytics overview](../../../enhanced-analytics/enhanced-analytics-overview.md).-->

## KPI progetto

Gli indicatori di prestazioni chiave (KPI, Key Performance Indicators) vengono visualizzati nella parte superiore dell’area Metriche.

![](assets/project-metrics-kpis-350x52.png)

Questi KPI sono suddivisi nelle seguenti categorie:

| Attività completate | **Attività completate** mostra il numero di attività in stato Completato. Questo numero include anche le attività con uno stato personalizzato che equivale a Completato. |
|---|---|
| Attività non completate | **Attività non completate** mostra il numero di attività che non sono in stato Completato o Chiuso o che sono in stato Completato. |
| Attività in ritardo | **Attività scadute** mostra il numero di attività che hanno superato la data di completamento pianificata e che non sono in stato Completato o Chiuso o che sono in uno stato che equivale a Completato o Chiuso. |
| Attività totali | **Attività totali** mostra il numero totale di attività nel progetto. |

>[!TIP]
>
>Per visualizzare un elenco di elementi di lavoro per un indicatore KPI specifico, fare clic su di esso. Nell&#39;elenco è possibile fare clic su un elemento di lavoro specifico per visualizzare ulteriori dettagli in una nuova scheda.\
>![](assets/completed-tasks-dialog-350x75.png)\
>Per ulteriori informazioni, vedere [Visualizza dettagli metriche](#view-metrics-details).

## Grafico a barre attività o problemi

Nel grafico a barre visualizzato sotto i KPI del progetto è possibile esaminare lo stato o la priorità degli elementi di lavoro del progetto. La visualizzazione delle attività è selezionata per impostazione predefinita.

Quando lo stato è selezionato in questo grafico, è possibile visualizzare tutti gli stati delle attività o dei problemi di un progetto. Ogni stato è raggruppato in una barra nel grafico. In questo grafico vengono visualizzati tutti gli stati di sistema predefiniti e gli stati personalizzati.

![](assets/project-metrics-task-issue-by-status-350x120.png)

Quando la priorità è selezionata in questo grafico, puoi visualizzare tutte le priorità delle attività o dei problemi di un progetto.

![](assets/project-metrics-task-issue-by-priority-350x121.png)

>[!TIP]
>
>Per visualizzare un elenco di elementi di lavoro con uno stato o una priorità specifica, fare clic su una barra nel grafico. Nell&#39;elenco è possibile fare clic su un elemento di lavoro specifico per visualizzare ulteriori dettagli in una nuova scheda.\
>![](assets/completed-tasks-dialog-350x75.png)\
>Per ulteriori informazioni, vedere [Visualizza dettagli metriche](#view-metrics-details).

## Grafico ad anello

Il grafico ad anello sotto i KPI del progetto consente di esaminare il rapporto tra elementi di lavoro completati e elementi di lavoro incompleti in un progetto.

![](assets/tasks-issues-by-complete-status-350x250.png)

Nel menu a discesa sopra il grafico, puoi selezionare:

| Tutte le attività | Selezionando **attività** puoi visualizzare il numero totale di attività nel progetto e il rapporto tra le attività completate e quelle incomplete. |
|---|---|
| Tutti i problemi | Selezionando **problemi** puoi vedere il numero totale di problemi nel progetto e il rapporto tra problemi completati e incompleti. |

>[!TIP]
>
>Per visualizzare un elenco degli elementi di lavoro completati o incompleti, fare clic su tale sezione nel grafico ad anello. Nell&#39;elenco è possibile fare clic su un elemento di lavoro specifico per visualizzare ulteriori dettagli in una nuova scheda.\
>![](assets/completed-tasks-dialog-350x75.png)\
>Per ulteriori informazioni, vedere [Visualizza dettagli metriche](#view-metrics-details).

## Grafico a barre assegnatario

Il grafico a barre assegnatario mostra il numero di attività assegnate a ogni persona nel progetto. Questo numero varia in base alla categoria selezionata dal menu a discesa.

![](assets/tasks-issues-by-assignee-350x104.png)

È possibile scegliere di esaminare le assegnazioni di attività per un progetto nelle seguenti categorie:

| Completato | Selezionando **Completa** viene visualizzato il numero di attività assegnate a ogni utente che sono state completate. |
|---|---|
| Incompleto | Selezionando **Incompleto** viene visualizzato il numero di attività assegnate a ogni utente che non sono ancora state completate. |
| In arrivo | Selezionando **In arrivo** viene visualizzato il numero di attività assegnate a ogni utente che non hanno ancora raggiunto la data di inizio pianificata. |
| In ritardo | Selezionando **Scaduto** viene visualizzato il numero di attività assegnate a ogni utente che sono passate oltre la data di completamento pianificata e non sono ancora state completate. |

>[!TIP]
>
>Per visualizzare un elenco degli elementi di lavoro della categoria selezionata assegnati a un utente specifico, fare clic sulla barra accanto al nome dell&#39;utente nel grafico. Nell&#39;elenco è possibile fare clic su un elemento di lavoro specifico per visualizzare ulteriori dettagli in una nuova scheda.\
>![](assets/completed-tasks-dialog-350x75.png)\
>Per ulteriori informazioni, vedere [Visualizza dettagli metriche](#view-metrics-details).

## Visualizzare i dettagli delle metriche {#view-metrics-details}

È possibile interagire con i grafici nell&#39;area Metriche per esaminare i diversi aspetti di un grafico oppure esaminare più da vicino le attività e i problemi relativi a un grafico.

1. Vai al progetto per il quale vuoi visualizzare le metriche.
1. Nel pannello a sinistra, fai clic su **Metriche**.\
   Per impostazione predefinita, i grafici nell’area Metriche visualizzano le informazioni relative alle attività.\
   ![](assets/metrics-section-350x298.png)

1. (Condizionale) Se in un grafico viene visualizzata una freccia a discesa, fare clic sull&#39;icona **della** freccia a discesa![](assets/dropdown-arrow.png) nel grafico e selezionare l&#39;opzione desiderata dal menu.\
   Per informazioni sulle opzioni visualizzate nei menu di ciascun grafico, vedere la sezione corrispondente precedente.

1. (Facoltativo) Per esaminare più da vicino le attività o i problemi relativi a qualsiasi metrica della pagina, effettua le seguenti operazioni:

   1. Fare clic sull&#39;elemento, ad esempio le attività assegnate a un utente specifico, i problemi con priorità alta o tutte le attività scadute, per il quale si desidera visualizzare i dettagli.

      Viene visualizzato un elenco di attività o problemi.

      ![](assets/completed-tasks-dialog-350x75.png)

   1. Utilizza le frecce nella parte inferiore dell’elenco per individuare l’attività o il problema che desideri esaminare.

      Oppure

      Selezionare un numero specifico per visualizzare le attività o i problemi relativi a una pagina specifica.

      ![](assets/pagination-300x152.png)

   1. Seleziona un’attività o un problema per visualizzare ulteriori dettagli.

      L’attività o il problema viene aperto in una nuova scheda.

1. (Facoltativo) Per esportare il dashboard delle metriche del progetto in un file con estensione png, fai clic sull&#39;icona **Esporta** ![](assets/export.png), quindi seleziona **Esporta come PNG** dal menu a discesa.

   >[!TIP]
   >
   >Quando esportate la dashboard, il file esportato include solo ciò che viene visualizzato nella finestra della vista. Per includere alcuni elementi nel file esportato, potrebbe essere necessario scorrere la pagina verso l&#39;alto o verso il basso oppure regolare le impostazioni di zoom del browser.
