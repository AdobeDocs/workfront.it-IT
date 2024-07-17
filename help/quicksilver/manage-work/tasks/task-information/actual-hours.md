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

Le ore effettive rappresentano il tempo effettivo impiegato per completare un&#39;attività, un problema o un progetto.

È consigliabile che le ore vengano registrate sugli elementi di lavoro, che sono attività e problemi.

Tuttavia, in qualità di amministratore di Workfront, puoi consentire agli utenti di accedere anche ai progetti in base al tipo di flusso di lavoro all’interno dell’organizzazione.

Per ulteriori informazioni su come configurare il sistema per consentire agli utenti di accedere ai progetti, vedere [Configurare le preferenze relative alle ore e alle schede orario](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

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
   <td> <p>Accesso di visualizzazione o accesso successivo ad attività, progetti o problemi</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizzare o accedere ad autorizzazioni superiori per un’attività, un progetto o un problema</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

## Ore effettive per attività e problemi rispetto alle ore effettive per i progetti

Le ore effettive per attività e problemi rappresentano il numero di ore registrate direttamente sulle attività e sui problemi.

>[!NOTE]
>
>Le ore effettive da attività figlio vengono riportate alle ore effettive dell&#39;attività padre. La formula seguente si applica alle ore effettive di un task padre:

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

È possibile trovare le informazioni sulle ore effettive relative alle attività nelle posizioni seguenti:

* [Ore effettive nella sezione Dettagli](#actual-hours-in-the-details-section)
* [Ore effettive nella sezione Ore](#actual-hours-in-the-hours-section)
* [Ore effettive nei report](#actual-hours-in-reports)
* [Ore effettive negli strumenti di gestione delle risorse](#actual-hours-in-resource-management-tools)

### Ore effettive nella sezione Dettagli {#actual-hours-in-the-details-section}

La ricerca delle ore effettive nella sezione Dettagli è identica per progetti, attività e problemi.

Per individuare le ore effettive in Dettagli attività:

1. Passare a un&#39;attività per la quale si desidera esaminare le ore effettive.
1. Fai clic su **Dettagli attività** nel pannello a sinistra.
1. Fai clic su **Panoramica** e osserva il valore **Ore effettive**.

   Totale delle ore registrate per l&#39;attività.

### Ore effettive nella sezione Ore {#actual-hours-in-the-hours-section}

La sezione Ricerca delle ore effettive è identica per progetti, attività e problemi.

Per individuare le ore effettive nella sezione Ore:

1. Passare a un&#39;attività per la quale si desidera esaminare le ore effettive.
1. Fai clic su **Ore** nel pannello a sinistra.

   A seconda della configurazione, la sezione Ore potrebbe essere elencata in **Mostra altro**.

   Viene visualizzato un elenco delle ore registrate per l&#39;attività.

1. Assicurati che la visualizzazione **Standard** e il raggruppamento **Progetto** siano applicati a questo elenco.

   Il numero visualizzato nella riga di raggruppamento per la colonna **Ore** corrisponde al numero totale di ore effettive dell&#39;attività.

### Ore effettive nei rapporti {#actual-hours-in-reports}

Quando si creano rapporti su attività, problemi o progetti, è possibile visualizzare il valore Ore effettive per ogni attività, problema o progetto nel rapporto.

L&#39;aggiunta della colonna Ore effettive a una visualizzazione delle attività è simile alla creazione di una visualizzazione in un report.

Per visualizzare le ore effettive in un rapporto attività:

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **menu principale** nell&#39;angolo superiore destro di Workfront, quindi fai clic su **Rapporti**.
1. Fai clic su **Nuovo rapporto**, quindi scegli **Attività** come oggetto.

1. Fai clic su **Aggiungi colonna** e inizia a digitare **Ore effettive** quando viene visualizzato il campo a discesa **Mostra in questa colonna**. Selezionare il campo quando viene visualizzato nell&#39;elenco.

1. Fare clic su **Salva + Chiudi** per salvare il report.

   La colonna Ore effettive mostra il numero di ore registrate per ogni attività.

### Ore effettive negli strumenti di gestione delle risorse {#actual-hours-in-resource-management-tools}

Se si desidera visualizzare l&#39;avanzamento del lavoro svolto dagli utenti sulle attività e sui problemi assegnati, è possibile utilizzare i seguenti strumenti di gestione delle risorse:

* Rapporto utilizzo.\
  Per informazioni sul report sull&#39;utilizzo, vedere [Panoramica del report sull&#39;utilizzo delle risorse](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

* Pianificazione risorse.

  Per informazioni sulla visualizzazione delle ore effettive nella Programmazione delle risorse, vedere [Visualizzazione delle ore disponibili, pianificate e effettive o FTE nella Programmazione delle risorse quando si utilizza la Visualizzazione utente](../../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md).

## Registra ore

È possibile registrare il tempo su attività, problemi e progetti in diversi modi.

Per ulteriori informazioni sull&#39;ora di accesso in Workfront, vedere [Ora di accesso](../../../timesheets/create-and-manage-timesheets/log-time.md).
