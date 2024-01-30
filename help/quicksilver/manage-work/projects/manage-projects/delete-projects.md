---
title: Elimina progetti
product-area: projects
navigation-topic: manage-projects
description: Puoi eliminare un progetto se il progetto e i relativi dati non sono più necessari. In alternativa all’eliminazione di un progetto, è consigliabile modificare il progetto e cambiare lo stato su Completato o Inattivo. Questa operazione rimuove tutte le attività correnti correlate al progetto dall'elenco delle attività di un utente, ma salva tutti i dati associati al progetto.
author: Alina
feature: Work Management
exl-id: a0e80c4d-29a8-4bf8-aa19-0c2d493236c6
recommendations: noDisplay, noCatalog
source-git-commit: dda00a43c5122a233ce2849d828d2e5e4555d2d9
workflow-type: tm+mt
source-wordcount: '884'
ht-degree: 1%

---

# Elimina progetti

<!--Audited: 01/2024-->

Puoi eliminare un progetto se il progetto e i relativi dati non sono più necessari.

In alternativa all’eliminazione di un progetto, è consigliabile modificare il progetto e cambiare lo stato su Completato o Inattivo. Questa operazione rimuove tutte le attività correnti correlate al progetto dall&#39;elenco delle attività di un utente, ma salva tutti i dati associati al progetto.

Puoi eliminare un progetto in un elenco di progetti o a livello di progetto.

## Requisiti di accesso

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>piano Adobe Workfront</p> </td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td> <p>Licenza Adobe Workfront*</p> </td> 
   <td> <p>Licenza corrente: Piano </p> 
   Oppure
   <p>Nuova licenza: Standard </p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Configurazione del livello di accesso</td> 
   <td> <p>Modificare l’accesso ai progetti con la possibilità di creare ed eliminare progetti</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Autorizzazioni oggetto </p> </td> 
   <td> <p>Modifica l'accesso a Progetti, Attività, Problemi con la possibilità di eliminare progetti, attività e problemi</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni sulla pianificazione, il tipo di licenza o l&#39;accesso disponibili, contattare l&#39;amministratore Workfront. Per ulteriori informazioni sui requisiti di accesso, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Comprendere il processo di eliminazione dei progetti

* [Limitazioni per l’eliminazione di progetti](#limitations-for-deleting-projects)
* [Impatto dell’eliminazione di progetti](#the-impact-of-deleting-projects)

### Limitazioni per l’eliminazione di progetti  {#limitations-for-deleting-projects}

* Gli elementi eliminati vengono spostati nel Cestino per 30 giorni e possono essere recuperati solo dall&#39;amministratore di Workfront.

  Per ulteriori informazioni sul ripristino degli oggetti, vedere l&#39;articolo [Ripristina elementi eliminati](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

* Se il progetto presenta attività o problemi con ore registrate, l’amministratore di Workfront o del gruppo deve consentire l’eliminazione di tali attività configurando le Preferenze attività e problemi nell’istanza Workfront per consentire l’eliminazione del progetto che contiene le attività.

  Per ulteriori informazioni sull’eliminazione di attività, problemi o progetti in cui sono registrate ore, consulta la sezione &quot;Eliminazione&quot; in [Configurare le preferenze per attività e problemi a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">(NOTE: this bullet stays in NWE only forever)</p>
  -->

### Impatto dell’eliminazione di progetti {#the-impact-of-deleting-projects}

* L’eliminazione di un progetto ha un impatto su altri oggetti collegati al progetto.

  Quando si elimina un progetto, vengono eliminati anche i seguenti oggetti allegati a un progetto:

   * Documenti

     Non è possibile eliminare un progetto a cui è associato un documento estratto. Per ulteriori informazioni sull&#39;estrazione di documenti, vedere [Estrai documenti](../../../documents/managing-documents/check-out-documents.md).

   * Attività
   * Sottoattività
   * Problemi
   * Aggiornamenti
   * Approvazioni
   * Spese
   * Rischi
   * Linee di base
   * Informazioni sul Business Case
   * Informazioni dettagli coda
   * Tariffe di fatturazione
   * Record fatturazione

     Non puoi eliminare un progetto con Record fatturazione con lo stato Fatturato. Per ulteriori informazioni, consulta [Crea record fatturazione](../../projects/project-finances/create-billing-records.md).

* A seconda del modo in cui l’amministratore di Workfront configura le preferenze per l’eliminazione di progetti, attività o problemi nelle preferenze per le schede orario e le ore dell’istanza di Workfront, le ore registrate per le attività, i problemi o il progetto vengono gestite in uno dei seguenti modi durante l’eliminazione del progetto:

   * Le ore rimangono nella scheda orario come orario generale.
   * Le ore vengono eliminate e verranno ripristinate se il progetto viene ripristinato.

  Per ulteriori informazioni sulla configurazione delle preferenze di eliminazione per le ore collegate a problemi, consulta [Configurare le preferenze di orario e scheda orario](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

* Se il progetto eliminato è collegato a un’iniziativa nella Pianificazione scenario di Workfront:

   * L&#39;iniziativa rimane sul piano, ma il collegamento al progetto viene rimosso.
   * Se il progetto eliminato è collegato all’unica iniziativa pubblicata da un piano, viene rimossa anche l’indicazione che il piano è stato pubblicato.
   * Se recuperi un progetto eliminato, il progetto viene recuperato, ma il relativo collegamento all’iniziativa non viene ripristinato e l’area Pianificazione scenario non viene più visualizzata in Dettagli progetto.

     Scenario Planner richiede una licenza aggiuntiva. Per informazioni su Workfront Scenario Planner, consulta [Panoramica sulla pianificazione degli scenari](../../../scenario-planner/scenario-planner-overview.md).

     Per informazioni sui progetti collegati alle iniziative nella Pianificazione scenario, consulta [Aggiornare o creare progetti pubblicando iniziative nella Pianificazione scenario](../../../scenario-planner/publish-scenarios-update-projects.md).

* Se il progetto è anche un’attività per un obiettivo in Obiettivi Workfront:

   * Il progetto viene eliminato dall’obiettivo. Viene rimosso anche lo stato di avanzamento indicato sull’obiettivo dal progetto.

   * Se recuperi il progetto eliminato, viene ripristinato anche il progetto come attività dell’obiettivo.

     È necessaria una licenza aggiuntiva. Per informazioni sugli obiettivi di Workfront, consulta [Panoramica sugli obiettivi di Adobe Workfront](../../../workfront-goals/goal-management/wf-goals-overview.md).

     Per informazioni sull’associazione dei progetti agli obiettivi, consulta [Aggiungere progetti agli obiettivi in Obiettivi di Adobe Workfront](../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).

## Eliminare un progetto da un elenco

Puoi eliminare i progetti da un elenco di progetti.

1. Consente di passare a un elenco di progetti o a un report di progetti.
1. Seleziona il progetto o i progetti da eliminare, quindi fai clic su **Elimina** icona ![](assets/delete-icon.png) nella parte superiore dell’elenco.

1. Clic **Sì, elimina** per confermare l’eliminazione.

   I progetti vengono eliminati e memorizzati nel Cestino per 30 giorni. Durante questo periodo, l’amministratore di Workfront può ripristinare i progetti eliminati dal Cestino.

## Eliminare un progetto a livello di progetto

1. Vai al progetto che desideri eliminare.
1. Fai clic su **Altro** icona ![](assets/qs-more-menu.png) a destra del nome del progetto, quindi fai clic su **Elimina progetto**.

   ![](assets/more-icon-expanded-delete-project-highlighted.png)

1. Clic **Sì, elimina**.

   Il progetto viene eliminato e memorizzato nel Cestino per 30 giorni. L&#39;amministratore di Workfront può ripristinarlo dal Cestino in questo periodo di tempo.

## Ripristino di progetti eliminati

Un amministratore di sistema o di gruppo può ripristinare i progetti entro 30 giorni dalla loro eliminazione, come descritto nell’articolo [Ripristina elementi eliminati](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).
