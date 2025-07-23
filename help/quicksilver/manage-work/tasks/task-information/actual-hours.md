---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Visualizza ore effettive
description: Le ore di accesso agli elementi di lavoro in Adobe Workfront sono considerate ore effettive. Le ore effettive rappresentano il tempo effettivo impiegato per completare un'attività, un problema o un progetto.
author: Alina
feature: Work Management
exl-id: c4b0e431-1765-416d-89f5-6ac663ac1d4f
source-git-commit: de42974a9a5c4c346ef3ae1cce09968befd1381c
workflow-type: tm+mt
source-wordcount: '1178'
ht-degree: 0%

---

# Visualizza ore effettive

<!-- Audited: 5/2025 -->

Le ore di accesso agli elementi di lavoro in Adobe Workfront sono considerate ore effettive.

Le ore effettive rappresentano il tempo effettivo impiegato per completare un&#39;attività, un problema o un progetto.

È consigliabile che le ore vengano registrate sugli elementi di lavoro, che sono attività e problemi. Tuttavia, in qualità di amministratore di Workfront, puoi consentire agli utenti di accedere anche ai progetti in base ai flussi di lavoro dell’organizzazione.

Per ulteriori informazioni su come configurare il sistema per consentire agli utenti di accedere ai progetti, vedere [Configurare le preferenze relative alle ore e alle schede orario](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

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
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> 
   <p>Nuovo: Standard<p>
   <p>Oppure</p>
   <p>Corrente: Lavoro o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Accesso di visualizzazione o accesso successivo ad attività, progetti o problemi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizzare o accedere ad autorizzazioni superiori per un’attività, un progetto o un problema</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ore effettive rispetto alle ore effettive legacy

A seconda dell’area di Workfront da cui accedi alle ore effettive, potrebbe fare riferimento a una delle seguenti ore registrate:

* Nei report ed elenchi relativi a progetti, attività e problemi:

   * **Ore effettive**: ore registrate per progetto, attività o problemi dopo maggio 2021. Sono archiviati nel database di Workfront in ore e il valore del campo è `actualWorkRequiredDouble`.
   * **Ore effettive legacy**: ore registrate per progetti, attività o problemi in qualsiasi momento, anche prima di maggio 2021. Sono archiviati nel database di Workfront come minuti e il valore del campo è `actualWorkRequired`.

     >[!IMPORTANT]
     >
     >Il costo effettivo del progetto utilizza le ore effettive legacy per il calcolo.


* Nell’area Dettagli progetto, attività o problema:

   * **Ore effettive**: ore registrate per progetti, attività o problemi dopo maggio 2021. Sono archiviati nel database di Workfront in ore e il valore del campo è `actualWorkRequiredDouble`.
   * **Ore effettive**: quando si accede a tali dati utilizzando un campo personalizzato di riferimento di campo nativo in un modulo personalizzato per un progetto, un&#39;attività o un problema.

## Ore effettive per attività e problemi rispetto alle ore effettive per i progetti

Le ore effettive per attività e problemi rappresentano il numero di ore registrate direttamente sulle attività e sui problemi.

Le ore effettive da attività figlio vengono riportate alle ore effettive dell&#39;attività padre. La formula seguente si applica alle ore effettive di un task padre:

```
Parent Task Actual Hours = All Tasks Actual Hours + Parent Task Actual Hours
```

Le ore effettive per i progetti rappresentano un totale delle ore effettive di tutte le attività del progetto (comprese le ore registrate direttamente sulle attività padre), di tutte le Issues del progetto e delle ore effettive registrate sul progetto stesso.

La formula seguente si applica alle ore effettive di un progetto:

```
Project Actual Hours = All Tasks Actual Hours + All Issues Actual Hours + All Project Actual Hours
```

## Trova ore effettive

Il valore di Ore effettive per un elemento è identico per attività, progetti e problemi.

### Ore effettive nella sezione Dettagli {#actual-hours-in-the-details-section}

La ricerca delle ore effettive nella sezione Dettagli è identica per progetti, attività e problemi.

Per individuare le ore effettive in Dettagli attività:

1. Passare a un&#39;attività per la quale si desidera esaminare le ore effettive.
1. Nel pannello a sinistra, fai clic su **Dettagli attività**. Viene visualizzata la sezione **Panoramica**.
1. Individua il valore **Ore effettive** nella sezione **Orario di lavoro**. Totale delle ore registrate per l&#39;attività.
1. (Facoltativo e condizionale) Se il riferimento al campo Ore effettive nativo è stato aggiunto a un modulo personalizzato per un progetto, un’attività o un problema, vai al modulo personalizzato e individua le Ore effettive nel campo personalizzato. Totale delle ore registrate per l&#39;oggetto.

### Ore effettive nella sezione Ore {#actual-hours-in-the-hours-section}

La sezione Ricerca delle ore effettive è identica per progetti, attività e problemi.

Per individuare le ore effettive nella sezione Ore di un&#39;attività:

1. Passare a un&#39;attività per la quale si desidera esaminare le ore effettive.

1. Nel pannello a sinistra, fai clic su **Ore**. Viene visualizzato un elenco delle ore registrate per l&#39;attività, con la colonna **Ore** che mostra il numero totale di ore effettive per l&#39;attività.

1. Assicurati che la visualizzazione **Standard** e il raggruppamento **Progetto** siano applicati a questo elenco.
1. Le ore effettive per l&#39;attività vengono visualizzate nella riga di raggruppamento per la colonna **Ore effettive**.

### Ore effettive e ore effettive legacy nei rapporti

Quando si creano rapporti su attività, problemi o progetti, è possibile visualizzare le ore effettive e i valori delle ore effettive legacy per ogni attività, problema o progetto nel rapporto.

Per informazioni sulla differenza tra le ore effettive e le ore effettive precedenti, vedere la sezione [Ore effettive rispetto alle ore effettive precedenti](#actual-hours-vs-legacy-actual-hours) in questo articolo.

Per visualizzare le ore effettive e le ore effettive legacy in un rapporto attività:

{{step1-to-reports}}

1. Nella pagina **Report**, fai clic su **Nuovo report**, quindi scegli **Attività** come oggetto.
1. Nell&#39;angolo inferiore destro della pagina fare clic su **Aggiungi colonna**.
1. Nel campo a discesa **Mostra in questa colonna**, inizia a digitare **Ore effettive**, quindi seleziona il campo quando viene visualizzato nell&#39;elenco.
1. Ripeti il passaggio precedente per aggiungere al rapporto il campo **Ore effettive legacy**.

1. Nell&#39;angolo inferiore sinistro della pagina fare clic su **Salva + Chiudi** per salvare il report.

1. Nella finestra di dialogo **Denomina il report per salvarlo**, immetti un nuovo nome per il report, quindi fai clic su **Applica**.
1. Ripeti gli stessi passaggi per un progetto o un rapporto sui problemi.

### Ore effettive negli strumenti di gestione delle risorse {#actual-hours-in-resource-management-tools}

Se si desidera visualizzare l&#39;avanzamento del lavoro svolto dagli utenti sulle attività e sui problemi assegnati, è possibile utilizzare i seguenti strumenti di gestione delle risorse:

* Il Rapporto Utilizzo.\
  Per informazioni, vedere [Panoramica del report Utilizzo risorse](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

* La Programmazione delle risorse.

  Per informazioni, vedere [Visualizza ore disponibili, pianificate ed effettive o FTE nella pianificazione risorse quando si utilizza la visualizzazione utente](../../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md).


### Ore effettive nell’API Workfront

<!--this section was added as a result to this issue: https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/task/6810910e0001b932e0948336208e76f2/overview-->

La maggior parte dei campi di Workfront in cui sono memorizzate le ore viene salvata nel database di Workfront in pochi minuti. Il nome del campo Ore pianificate di un&#39;attività, ad esempio, è `workRequired` nel database di Workfront ed è memorizzato in minuti.

Devi tenere conto della conversione da minuti a ore quando accedi a questi campi nelle chiamate API o nei campi o nelle colonne personalizzati calcolati.

Le ore effettive registrate per progetti, attività o problemi sono attualmente memorizzate nel database di Workfront in minuti e il valore del campo è `actualWorkRequired`.

Con la seguente versione dell’API Workfront, che verrà rilasciata più avanti nel 2025, le ore effettive sono memorizzate nei campi e nelle unità seguenti nel database:

* **Ore effettive**: ore registrate per progetto, attività o problemi dopo maggio 2021. Sono archiviati nel database di Workfront in ore e il valore del campo è `actualWorkRequiredDouble`.
* **Ore effettive legacy**: ore registrate per progetti, attività o problemi in qualsiasi momento, anche prima di maggio 2021. Sono archiviati nel database di Workfront come minuti e il valore del campo è `actualWorkRequired`.

  >[!IMPORTANT]
  >
  >Il costo effettivo del progetto utilizza le ore effettive legacy per il calcolo.

  Per informazioni sull&#39;utilizzo delle ore effettive nelle colonne o nei campi calcolati, vedere [Domande frequenti sui report](/help/quicksilver/reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md).

## Registra ore

È possibile registrare il tempo su attività, problemi e progetti in diversi modi.

Per ulteriori informazioni, vedere [Tempo di connessione](../../../timesheets/create-and-manage-timesheets/log-time.md).
