---
product-area: projects
navigation-topic: manage-tasks
title: Associa attività cardine ad attività
description: È possibile associare le attività cardine alle attività per indicare quando si raggiungono passaggi importanti nel corso della durata del progetto. È necessario associare un percorso milestone a un progetto prima di associare le milestone alle attività del progetto.
author: Alina
feature: Work Management
exl-id: 56410640-fde4-417f-8ea0-f089315476f7
source-git-commit: e896d156854c6729e5ea0a82dcbc641fbfa9415e
workflow-type: tm+mt
source-wordcount: '424'
ht-degree: 0%

---

# Associa attività cardine ad attività

<!--Audited: 01/2024-->

È possibile associare le attività cardine alle attività per indicare quando si raggiungono passaggi importanti nel corso della durata del progetto.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

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
   <td> <p>Nuova licenza: Standard</p> 
   <p>Licenza corrente: Lavoro o versione successiva</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modifica l'accesso alle Attività</p> <p><b>NOTA</b>

Se non disponi dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per l’attività</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

+++

## Prerequisiti

Prima di associare un&#39;attività cardine a un&#39;attività, è necessario che siano presenti le condizioni seguenti:

* L&#39;amministratore di Workfront deve creare un percorso milestone, come descritto in [Creare un percorso milestone](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md).

* È necessario associare un Percorso milestone a un progetto.

  Per informazioni, vedere [Modifica progetti](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md).

* Per associare un percorso milestone a un progetto, il progetto deve trovarsi nello stato Pianificazione o Corrente.

  >[!TIP]
  >
  >Per ottenere una panoramica ottimale dell&#39;avanzamento dei milestone nei progetti utilizzando la vista Milestone, è necessario creare attività padre e associarle a ogni fase principale del progetto. Quindi, associa queste attività padre a ciascuna delle attività cardine del percorso milestone.

## Associare un&#39;attività cardine a un&#39;attività

Dopo aver associato un percorso milestone a un progetto, alle attività può essere assegnata una milestone.

1. Vai a un&#39;attività, quindi fai clic sull&#39;icona **Altro** ![](assets/more-icon.png) a destra del nome dell&#39;attività, quindi su **Modifica**.

   Le attività e le Milestone hanno una relazione 1:1. Impossibile associare la stessa milestone a più attività. È possibile collegare ogni attività a un&#39;unica attività cardine oppure associare ogni attività cardine a un&#39;unica attività.

1. Fai clic su **Impostazioni**, quindi seleziona una milestone nel campo **Milestone** per l&#39;attività.
1. Fai clic su **Salva**.
1. (Facoltativo) In un elenco di attività, aggiungi la colonna **Icone di stato** per identificare le attività cardine. Nella colonna Icone di stato viene visualizzato l&#39;indicatore del rombo di Milestone.

   Per informazioni, vedere [Creare o modificare le visualizzazioni in Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

   ![](assets/amwt3.png)

1. (Facoltativo) Vai a un elenco di progetti, seleziona la visualizzazione **Milestone** per identificare l&#39;avanzamento delle attività milestone.

   ![](assets/milestone-view-project-list.png)
