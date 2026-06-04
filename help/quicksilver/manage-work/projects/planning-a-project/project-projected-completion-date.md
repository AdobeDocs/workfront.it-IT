---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Panoramica sulla data di completamento prevista per progetti, attività e problemi
description: La Data di completamento prevista è un indicatore calcolato in tempo reale del momento in cui il progetto, l’attività o il problema verrà completato. Quando il progetto, l’attività o il problema è contrassegnato come Completato, la Data di completamento prevista cambia in corrispondenza della Data di completamento effettiva.
author: Alina
feature: Work Management
exl-id: dde400e6-189f-4431-8f2f-7142ce424826
TQID: https://experienceleague.adobe.com/qpYXoo1C-GZi1B--dhKTGjzvSWdLxrQM3IqX4Q6GZt8
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b91c0848-76c4-4da4-8b81-3aade0518dd0id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 869
ht-degree: 5%

---

# Panoramica sulla data di completamento prevista per progetti, attività e problemi

<!-- Audited: 11/2025 -->

La Data di completamento prevista è un indicatore calcolato in tempo reale del momento in cui il progetto, l’attività o il problema verrà completato. Quando il progetto, l’attività o il problema è contrassegnato come Completato, la Data di completamento prevista cambia in corrispondenza della Data di completamento effettiva.

Le sezioni seguenti descrivono come e come individuare la Data di completamento prevista per progetti, attività e problemi.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo. 


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td> 
   <ul><li><p>Collaboratore o versione successiva per visualizzare la data di completamento prevista in un rapporto</p></li> <li><p>Una licenza Standard per creare un rapporto</p></li> </ul>
   Oppure
   <ul><li><p>Rivedi o più avanti per visualizzare la Data di completamento prevista in un rapporto</p></li> 
   <li><p>Una licenza Pianificazione per creare un report</p> </li></ul>
      </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Livello di accesso</td> 
   <td> <p>Accesso ai progetti di visualizzazione o superiore</p> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari per creare un rapporto</p> <p>Modificare l’accesso a Filtri, Viste, Raggruppamenti per creare un rapporto o modificare una vista a elenco</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
   <td> <p>Visualizzare o accedere ad autorizzazioni superiori per un progetto</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Come Adobe Workfront determina la data di completamento prevista

La Data di completamento prevista è un campo calcolato e non può essere modificata manualmente.

I criteri utilizzati per determinare la data di completamento prevista variano a seconda dell&#39;oggetto visualizzato:

* **Progetti:** la data di completamento prevista per i progetti è uguale alla data di completamento prevista dell&#39;ultima attività del progetto.

  Ad esempio, una percentuale di completamento più elevata sposta la data di completamento prevista dell&#39;attività più vicina al giorno corrente. Se lo stato dell&#39;attività è Nuovo e la data di completamento pianificata dell&#39;attività è vicina o è stata superata, la data di completamento prevista si sposta ulteriormente nel futuro.

* **Attività:** La data di completamento prevista per le attività è determinata in base ai seguenti criteri:

   * **Aggiornamenti dell&#39;avanzamento effettuati sull&#39;attività dall&#39;assegnatario dell&#39;attività:** Gli aggiornamenti dell&#39;avanzamento includono modifiche alla percentuale di completamento e modifiche allo stato dell&#39;attività.
   * **Data commit:** Se l&#39;assegnatario dell&#39;attività specifica una data di commit, la data di completamento prevista viene modificata in modo da corrispondere alla data di commit.

     Per ulteriori informazioni sulle date di conferma, vedere l&#39;articolo [Panoramica sulla data di conferma](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

   * **Predecessori:** Se non si verificano ritardi nelle attività predecessori, la Data di completamento prevista deve corrispondere alla Data di completamento pianificata. Quando si verificano ritardi, le attività dipendenti visualizzano una Data di completamento prevista successiva alla Data di completamento pianificata.

     Per ulteriori informazioni sulla data di completamento pianificata delle attività, vedere [Panoramica sulla data di completamento pianificata dell&#39;attività](../../../manage-work/tasks/task-information/task-planned-completion-date.md).

  >[!IMPORTANT]
  >
  >Quando il predecessore di un&#39;attività ha una data di completamento effettiva, le attività dipendenti ricevono una data di completamento prevista come descritto nel seguente scenario:
  >
  >
  >Se il progetto ha l&#39;Attività A, l&#39;Attività B e l&#39;Attività C e l&#39;Attività B è il successore dell&#39;Attività A, l&#39;Attività C è il successore dell&#39;Attività B e viene aggiunta una Data di completamento effettiva all&#39;Attività A, la Data di completamento prevista viene ricalcolata automaticamente per l&#39;Attività B (a condizione che il **Tipo di aggiornamento** del progetto sia impostato su Automatico e Su modifica), ma non verrà ricalcolata per l&#39;Attività C. Attualmente, Workfront calcola la Data di completamento prevista per le attività di un livello superiore o inferiore rispetto all&#39;Attività aggiornata, per motivi di prestazioni.

* **Problemi:** la data di completamento prevista del problema è inizialmente impostata per corrispondere alla data di completamento pianificata del problema.

  Se l’assegnatario del problema specifica una data di commit, sia la Data di completamento prevista che la Data di completamento pianificata vengono modificate in modo da corrispondere alla Data di commit.

  Per ulteriori informazioni sulle date di conferma, vedere l&#39;articolo [Panoramica sulla data di conferma](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

## Visualizza la data di completamento prevista

Puoi visualizzare la Data di completamento prevista dei progetti, delle attività e dei problemi nei rapporti. È possibile visualizzare la data di completamento prevista dei progetti e delle attività in altre aree di Workfront.

### Visualizzare la data di completamento prevista di un progetto {#view-the-projected-completion-date-of-a-project}

1. Vai al progetto in cui desideri visualizzare la Data di completamento prevista.
1. Fai clic su **Dettagli progetto** nel pannello a sinistra.
1. Individua il campo **Data di completamento prevista** nella sezione **Panoramica** > **Date progetto**.

### Visualizzare la data di completamento prevista di un&#39;attività {#view-the-projected-completion-date-of-a-task}

1. Passare all&#39;attività in cui si desidera visualizzare la data di completamento prevista.
1. Fai clic su **Dettagli attività** nel pannello a sinistra.
1. Individua il campo **Data di completamento prevista** nella sezione **Panoramica** > **Date attività e vincolo**.

### Visualizzare la data di completamento prevista di un problema {#view-the-projected-completion-date-of-an-issue}

È possibile visualizzare la Data di completamento prevista per i problemi solo in un report sui problemi o in una vista a elenco. La creazione di una vista a elenco è simile alla creazione della vista in un rapporto.

Per creare un report di problemi che includa la Data di completamento prevista:

1. Creare un rapporto sui problemi, come descritto nell&#39;articolo [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Selezionare la scheda **Colonne (visualizzazione)**.
1. Fai clic su **Aggiungi colonna** e inizia a digitare **Data di completamento prevista** nel campo **Mostra in questa colonna:**.

1. Selezionala quando viene visualizzata nell&#39;elenco, nell&#39;oggetto **Issue**.
1. Fai clic su **Salva e Chiudi**.

   ![Data di completamento prevista problema nella colonna del report](assets/issue-projected-completion-date-in-view-nwe-350x148.png)


   La colonna **Data di completamento prevista** nel report è compilata.


