---
title: Eliminare progetti
product-area: projects
navigation-topic: manage-projects
description: Se il progetto e i relativi dati non sono più necessari, puoi eliminare un progetto.
author: Alina
feature: Work Management
exl-id: a0e80c4d-29a8-4bf8-aa19-0c2d493236c6
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '854'
ht-degree: 0%

---

# Eliminare progetti

Se il progetto e i relativi dati non sono più necessari, puoi eliminare un progetto.

Invece di eliminare un progetto, consigliamo di modificarlo e di impostarlo su Completato o Morto. In questo modo vengono rimosse tutte le attività correnti correlate al progetto dall’elenco delle attività di un utente, ma vengono salvati tutti i dati associati al progetto.

## Requisiti di accesso

<!-- drafted for P&P:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront plan*</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront license*</p> </td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Access level configurations*</strong> </td> 
   <td> <p>Edit access to Projects with ability to Create <span>and Delete</span> projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Object permissions</strong> </p> </td> 
   <td> <p>Edit access to Projects, Tasks,&nbsp;Issues with ability to Delete projects, tasks, and issues</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica l’accesso a Progetti, Attività, Problemi con la possibilità di eliminare progetti, attività e problemi</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestisci le autorizzazioni per il progetto, le attività e i problemi del progetto con la possibilità di eliminare il progetto, le attività e i problemi. </p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.
Puoi eliminare un progetto in un elenco di progetti o a livello di progetto.

## Comprendere il processo di eliminazione dei progetti

* [Limitazioni per l’eliminazione dei progetti](#limitations-for-deleting-projects)
* [L’impatto dell’eliminazione dei progetti](#the-impact-of-deleting-projects)

### Limitazioni per l’eliminazione dei progetti  {#limitations-for-deleting-projects}

* Gli elementi eliminati vengono spostati nel Cestino per 30 giorni e possono essere recuperati solo dall&#39;amministratore Workfront.

   Per ulteriori informazioni sul ripristino degli oggetti, vedere l’articolo [Ripristina elementi eliminati](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

* Se il progetto ha attività o problemi con le ore registrate, l’amministratore di Workfront o di gruppo deve consentire l’eliminazione di tali attività configurando le Preferenze attività e problemi nell’istanza Workfront per poter eliminare il progetto che contiene le attività.

   Per ulteriori informazioni sull’abilitazione dell’eliminazione di attività, problemi o progetti in cui vengono registrate ore, consulta la sezione &quot;Eliminazione&quot; in [Configurare le preferenze relative alle attività e ai problemi a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">(NOTE: this bullet stays in NWE only forever)</p>
  -->

### L’impatto dell’eliminazione dei progetti {#the-impact-of-deleting-projects}

* Quando si elimina un progetto, vengono interessati anche altri oggetti collegati al progetto.

   Quando elimini un progetto vengono eliminati anche i seguenti oggetti associati a un progetto:

   * Documenti

      Non è possibile eliminare un progetto con un documento allegato estratto. Per ulteriori informazioni sull&#39;estrazione dei documenti, vedere [Estrarre documenti](../../../documents/managing-documents/check-out-documents.md).

   * Attività
   * Sottoattività
   * Problemi
   * Note
   * Approvazioni
   * Spese

* A seconda della modalità di configurazione delle preferenze di eliminazione di progetti, attività o problemi nelle preferenze della scheda attività e ora dell’istanza Workfront, le ore registrate per le attività, i problemi o il progetto vengono gestiti in uno dei modi seguenti durante l’eliminazione del progetto:

   * Le ore rimangono sulla scheda attività come ora generale.
   * Le ore vengono eliminate e verranno ripristinate se il progetto viene ripristinato.

   Per ulteriori informazioni sulla configurazione delle preferenze di eliminazione per le ore di accesso ai problemi, vedi [Configurare le preferenze relative a schede attività e ora](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

* Se il progetto eliminato è collegato a un&#39;iniziativa in Workfront Scenario Planner:

   * L&#39;iniziativa rimane in programma, ma il collegamento al progetto viene rimosso.
   * Se il progetto eliminato è collegato all’unica iniziativa pubblicata da un piano, viene eliminata anche l’indicazione che il piano è stato pubblicato.
   * Se si recupera un progetto eliminato, il progetto viene recuperato, ma il relativo collegamento all’iniziativa non viene ripristinato e l’area Planner scenario non viene più visualizzata in Dettagli progetto.

      Il planner scenario è disponibile solo nella nuova esperienza Adobe Workfront e richiede una licenza aggiuntiva. Per informazioni su Workfront Scenario Planner, vedi [Panoramica di Scenario Planner](../../../scenario-planner/scenario-planner-overview.md).

      Per informazioni sui progetti collegati alle iniziative nel Planner scenario, vedi [Aggiornare o creare progetti pubblicando iniziative nel Planner scenario](../../../scenario-planner/publish-scenarios-update-projects.md).

* Se il progetto è anche un’attività per un obiettivo in Obiettivi di Workfront:

   * Il progetto viene eliminato dall’obiettivo. Vengono rimossi anche i progressi indicati nell’obiettivo dal progetto.

   * Se recuperi il progetto eliminato, anche il progetto viene ripristinato come attività dell’obiettivo.

      Questo richiede una licenza aggiuntiva. Per informazioni sugli obiettivi di Workfront, vedi [Panoramica sugli obiettivi di Adobe Workfront](../../../workfront-goals/goal-management/wf-goals-overview.md).

      Per informazioni sull’associazione di progetti con obiettivi, consulta [Aggiungere progetti agli obiettivi in Obiettivi di Adobe Workfront](../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).

## Eliminare un progetto da un elenco

È possibile eliminare i progetti da un elenco di progetti.

1. Passa a un elenco di progetti o a un rapporto di progetto.
1. Seleziona il progetto da eliminare, quindi fai clic su **Elimina** in cima all&#39;elenco.

1. Fai clic su **Sì, Elimina** per confermare l’eliminazione.

   Il progetto viene eliminato e memorizzato nel Cestino per 30 giorni. L&#39;amministratore Workfront può ripristinarlo dal Cestino in questo momento.

## Eliminare un progetto a livello di progetto

1. Passa al progetto da eliminare.
1. Fai clic sul pulsante **Altro** icona ![](assets/qs-more-menu.png).

1. Fai clic su **Elimina progetto**.

1. Fai clic su **Sì, eliminalo**.

   Il progetto viene eliminato e memorizzato nel Cestino per 30 giorni. L&#39;amministratore Workfront può ripristinarlo dal Cestino in questo momento.

## Ripristino dei progetti eliminati

Un amministratore di sistema o di gruppo può ripristinare i progetti entro 30 giorni dalla loro eliminazione, come descritto nell’articolo [Ripristina elementi eliminati](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).
