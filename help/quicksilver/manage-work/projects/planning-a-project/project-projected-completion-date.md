---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Panoramica della data di completamento prevista per progetti, attività e problemi
description: La data di completamento prevista è un indicatore calcolato in tempo reale che indica quando il progetto, l'attività o il problema verrà completato. Quando il progetto, l'attività o il problema sono contrassegnati come Completato, la data di completamento prevista viene modificata in base alla data di completamento effettivo.
author: Alina
feature: Work Management
exl-id: dde400e6-189f-4431-8f2f-7142ce424826
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '876'
ht-degree: 0%

---

# Panoramica della data di completamento prevista per progetti, attività e problemi

La data di completamento prevista è un indicatore calcolato in tempo reale che indica quando il progetto, l&#39;attività o il problema verrà completato. Quando il progetto, l&#39;attività o il problema sono contrassegnati come Completato, la data di completamento prevista viene modificata in base alla data di completamento effettivo.

Nelle sezioni seguenti viene descritto come viene determinata la data di completamento prevista per i progetti, le attività e i problemi e come individuarla.

## Requisiti di accesso

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> 
   <p>For current licenses: 
   <ul><li><p>Contributor or higher to view the Projected Completion Date in a report</p></li> <li><p>A Standard license to create a report</p></li> </ul>
   
   <p>For legacy licenses: 
   <ul><li><p>Review or higher to view the Projected Completion Date in a report</p></li> 
   <li><p>A Plan license to create a report</p> </li></ul>
      </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects</p> <p>You must have Edit access to Reports, Dashboards, Calendars to create a report</p> <p>You must have Edit access to Filters, Views, Groupings to create a report or modify a list view</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

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
   <td> <p>Rivedi o una versione successiva per visualizzare la data di completamento prevista in un rapporto</p> <p>Una licenza di piano per creare un report</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Visualizzare o accedere in modo più rapido ai progetti</p> <p>Per creare un rapporto è necessario disporre dell’accesso Modifica a Report, Dashboard, Calendari</p> <p>Per creare un rapporto o modificare una vista a elenco è necessario disporre dell’accesso Modifica a Filtri, Viste e Gruppi</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizzare o concedere autorizzazioni superiori a un progetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Come Adobe Workfront determina la data di completamento prevista

La data di completamento prevista è un campo calcolato e non può essere modificato manualmente.

I criteri utilizzati per determinare la data di completamento prevista variano a seconda dell&#39;oggetto visualizzato:

* **Progetti:** La data di completamento prevista per i progetti corrisponde alla data di completamento prevista dell&#39;ultima attività del progetto.
* **Attività:** La data di completamento prevista per le attività viene determinata in base ai seguenti criteri:

   * **Avanzamento degli aggiornamenti apportati all&#39;attività dall&#39;assegnatario:** Gli aggiornamenti dell&#39;avanzamento includono le modifiche alla percentuale di completamento e lo stato dell&#39;attività.
   * **Data commit:** Se l&#39;assegnatario dell&#39;attività specifica una data di commit, la data di completamento prevista viene modificata per corrispondere alla data di commit.

      Per ulteriori informazioni sulle date di commit, consulta l’articolo [Panoramica sulla data del commit](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

   * **Predecessori:** Se non si verificano ritardi nelle attività precedenti, la data di completamento prevista deve corrispondere alla data di completamento pianificata. Quando si verificano dei ritardi, le attività dipendenti presentano una data di completamento prevista maggiore della data di completamento pianificata.

      Per ulteriori informazioni sulla data di completamento pianificata delle attività, vedere [Panoramica dell&#39;attività Data completamento pianificata](../../../manage-work/tasks/task-information/task-planned-completion-date.md).
   >[!IMPORTANT]
   >
   >Quando il predecessore di un&#39;attività ha una data di completamento effettiva, i task dipendenti ricevono una data di completamento prevista come descritto nello scenario seguente:
   >
   >
   >Se il progetto ha l&#39;attività A, l&#39;attività B e l&#39;attività C e l&#39;attività B è il successore dell&#39;attività A, l&#39;attività C è il successore dell&#39;attività B e viene aggiunta una data di completamento effettiva all&#39;attività A, la data di completamento prevista viene automaticamente ricalcolata per l&#39;attività B (a condizione che l&#39;opzione **Tipo di aggiornamento** del progetto è impostato su Automatico e In caso di modifica), ma non verrà ricalcolato per l&#39;attività C. Al momento, Workfront calcola la data di completamento prevista per le attività che sono di un livello superiore o inferiore rispetto all&#39;attività aggiornata, per motivi di prestazioni. 

* **Problemi:**la data di completamento prevista del problema viene inizialmente impostata in modo che corrisponda alla data di completamento pianificata del problema.

   Se l&#39;assegnatario del problema specifica una data di commit, sia la data di completamento prevista che la data di completamento pianificata cambiano in modo che corrispondano alla data di commit.

   Per ulteriori informazioni sulle date di commit, consulta l’articolo [Panoramica sulla data del commit](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

## Visualizza la data di completamento prevista

È possibile visualizzare la data di completamento prevista di progetti, attività e problemi nei rapporti. È possibile visualizzare la data di completamento prevista dei progetti e delle attività in altre aree di Workfront. 

* [Visualizza la data di completamento prevista di un progetto](#view-the-projected-completion-date-of-a-project)
* [Visualizza la data di completamento prevista di un&#39;attività](#view-the-projected-completion-date-of-a-task)
* [Visualizza la data di completamento prevista di un problema](#view-the-projected-completion-date-of-an-issue)

### Visualizza la data di completamento prevista di un progetto {#view-the-projected-completion-date-of-a-project}

1. Passare al progetto in cui si desidera visualizzare la data di completamento prevista.
1. Fai clic su **Dettagli progetto** nel pannello a sinistra.
1. Individua il **Data di completamento prevista** nel campo **Panoramica** sezione .

### Visualizza la data di completamento prevista di un&#39;attività {#view-the-projected-completion-date-of-a-task}

1. Passare all&#39;attività in cui si desidera visualizzare la data di completamento prevista.
1. Fai clic su **Dettagli attività** nel pannello a sinistra.
1. Individua il **Data di completamento prevista** nel campo **Panoramica** sezione .

### Visualizza la data di completamento prevista di un problema {#view-the-projected-completion-date-of-an-issue}

È possibile visualizzare la data di completamento prevista per i problemi solo in un report dei problemi o in una visualizzazione a elenco. La creazione di una vista a elenco è simile alla creazione di una vista in un rapporto.

Per creare un rapporto sul problema che include la data di completamento prevista:

1. Crea un rapporto sul problema, come descritto nell’articolo [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Seleziona la **Colonne (visualizzazione)** scheda .
1. Fai clic su **Aggiungi colonna** e inizia a digitare **Data di completamento prevista** in **Mostra in questa colonna:** campo .

1. Selezionalo quando viene visualizzato nell’elenco, sotto la sezione **Problema** oggetto. 
1. Fai clic su **Salva e chiudi**.

   La **Data di completamento prevista** nel rapporto viene compilata la colonna . 

   ![](assets/issue-projected-completion-date-in-view-nwe-350x148.png)
