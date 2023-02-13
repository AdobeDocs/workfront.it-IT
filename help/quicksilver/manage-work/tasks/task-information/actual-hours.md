---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Visualizza ore effettive
description: Le ore di accesso agli elementi di lavoro in Adobe Workfront sono considerate ore effettive.
author: Alina
feature: Work Management
exl-id: c4b0e431-1765-416d-89f5-6ac663ac1d4f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '796'
ht-degree: 0%

---

# Visualizza ore effettive

Le ore di accesso agli elementi di lavoro in Adobe Workfront sono considerate ore effettive.

Le ore effettive rappresentano il tempo effettivo necessario per completare un&#39;attività, un problema o un progetto.

È consigliabile che le ore siano registrate sugli elementi di lavoro, che sono attività e problemi.

Tuttavia, in qualità di amministratore di Workfront, puoi consentire anche agli utenti di eseguire l’accesso ai progetti, a seconda dei flussi di lavoro presenti nell’organizzazione.

Per ulteriori informazioni su come configurare il sistema per consentire agli utenti di eseguire l’accesso ai progetti, consulta [Configurare le preferenze relative a schede attività e ora](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

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
   <td> <p>Accesso o accesso più elevato a attività, progetti o problemi</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizza o autorizzazioni superiori per un'attività, un progetto o un problema</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Ore effettive su attività e problemi rispetto a Ore effettive sui progetti

Le ore effettive su attività e problemi rappresentano il numero di ore registrate direttamente sulle attività e sui problemi.

>[!NOTE]
>
>Le ore effettive dalle attività figlio vengono riportate fino alle ore effettive dell&#39;attività padre. La seguente formula si applica per le ore effettive di un&#39;attività padre:

```
Parent Task Actual Hours = All Tasks Actual Hours + Parent Task Actual Hours
```

Le ore effettive per i progetti rappresentano un totale di ore effettive per tutte le attività del progetto (incluse le ore registrate direttamente sulle attività padre), tutti i problemi del progetto e le ore effettive registrate sul progetto stesso.

La seguente formula si applica per le ore effettive di un progetto:

```
Project Actual Hours = All Tasks Actual Hours + All Issues Actual Hours + All Project Actual Hours
```

## Trova ore effettive

La ricerca del valore di Ore effettive per un articolo è identica per le attività, i progetti e i problemi.

È possibile trovare le informazioni Ore effettive sulle attività nelle posizioni seguenti:

* [Ore effettive nella sezione Dettagli](#actual-hours-in-the-details-section)
* [Ore effettive nella sezione Ore](#actual-hours-in-the-hours-section)
* [Ore effettive nei rapporti](#actual-hours-in-reports)
* [Ore effettive negli strumenti di gestione delle risorse](#actual-hours-in-resource-management-tools)

### Ore effettive nella sezione Dettagli {#actual-hours-in-the-details-section}

La ricerca delle ore effettive nella sezione Dettagli è identica per i progetti, le attività e i problemi.

Per individuare le ore effettive in Dettagli attività:

1. Passare a un&#39;attività per la quale si desidera rivedere l&#39;orario effettivo.
1. Fai clic su **Dettagli attività** nel pannello a sinistra.
1. Fai clic su **Panoramica** e notare **Ore effettive** valore.

   Totale delle ore di accesso all&#39;attività.

### Ore effettive nella sezione Ore {#actual-hours-in-the-hours-section}

La ricerca delle ore effettive nella sezione Ore è identica per i progetti, le attività e i problemi.

Per individuare le ore effettive nella sezione Ore :

1. Passare a un&#39;attività per la quale si desidera rivedere l&#39;orario effettivo.
1. Fai clic su **Ore** nel pannello a sinistra.

   A seconda della configurazione, la sezione Ore potrebbe essere elencata in **Mostra altro**.

   Viene visualizzato un elenco delle ore di accesso all’attività.

1. Assicurati che **Standard** visualizzazione e **Progetto** a questo elenco vengono applicati i raggruppamenti.

   Il numero visualizzato nella riga di raggruppamento per il **Ore** colonna indica il numero totale di ore effettive dell&#39;attività.

### Ore effettive nei rapporti {#actual-hours-in-reports}

Quando si creano rapporti relativi a attività, problemi o progetti, è possibile visualizzare il valore Ore effettive per ogni attività, problema o progetto del rapporto.

L&#39;aggiunta della colonna Ore effettive a una visualizzazione attività è simile alla creazione di una visualizzazione in un rapporto.

Per visualizzare le ore effettive in un rapporto delle attività:

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Workfront, quindi fai clic su **Rapporti**.
1. Fai clic su **Nuovo rapporto**, quindi scegli **Attività** come oggetto.

1. Fai clic su **Aggiungi colonna** e inizia a digitare **Ore effettive** quando **Mostra in questa colonna** viene visualizzato il campo a discesa . Selezionare il campo quando viene visualizzato nell’elenco.

1. Fai clic su **Salva e chiudi** per salvare il rapporto.

   La colonna Ore effettive mostra il numero di ore registrate per ogni attività.

### Ore effettive negli strumenti di gestione delle risorse {#actual-hours-in-resource-management-tools}

Se si desidera visualizzare l&#39;avanzamento del lavoro svolto dagli utenti sulle attività e sui problemi assegnati, è possibile visualizzarli nei seguenti strumenti di gestione delle risorse:

* Rapporto sull&#39;utilizzo.\
   Per informazioni sul rapporto di utilizzo, vedi [Panoramica del rapporto Utilizzo risorse](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

* Pianificazione risorse.

   Per informazioni sulla visualizzazione degli orari effettivi nel planner risorse, vedere [Visualizza Ore disponibili, pianificate e effettive o FTE nel planner risorse quando si utilizza la visualizzazione Utente](../../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md).

## Tempo di log

È possibile eseguire il log time su attività, problemi e progetti in diversi modi.

Per ulteriori informazioni sul tempo di accesso in Workfront, vedi [Tempo di log](../../../timesheets/create-and-manage-timesheets/log-time.md).
