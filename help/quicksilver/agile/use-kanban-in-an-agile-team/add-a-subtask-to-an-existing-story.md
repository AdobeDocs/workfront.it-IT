---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Aggiungere un’attività secondaria a una storia esistente nel Kanban Board
description: Leggi questo articolo per scoprire come creare sottoattività per i brani esistenti sulla bacheca Kanban.
author: Jenny
feature: Agile
exl-id: c6610616-80e5-4ded-9d23-63f15536e45c
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 0%

---

# Aggiungi un’attività secondaria a un brano esistente nel Kanban Board

Quando create sottoattività per i brani esistenti, tenete presente quanto segue:

**Quando l&#39;impostazione [!UICONTROL Modalità di completamento riepilogo] per il progetto è impostata su [!UICONTROL Manuale]:**

* Puoi spostare una storia padre con sottoattività in [!UICONTROL Completo], che aggiorna la storia padre al 100% e lo [!UICONTROL Stato] in [!UICONTROL Completo]. Le sottoattività non vengono aggiornate.
* Per aggiornare la [!UICONTROL Percentuale completata] per la storia, è necessario aggiornarla dalla scheda [!UICONTROL Storie] o dalla pagina [!UICONTROL Dettagli] dell&#39;oggetto.

**Quando l&#39;impostazione [!UICONTROL Modalità di completamento riepilogo] per il progetto è impostata su [!UICONTROL Automatica]:**

* Non potete spostare la storia principale in senso orizzontale. Per aggiornare [!UICONTROL Percent Complete] per la storia, è necessario aggiornare [!UICONTROL Percent Complete] per le sottoattività. La [!UICONTROL Percentuale completata] per il brano viene calcolata in base alla [!UICONTROL Percentuale completata] di tutte le sottoattività.
* Se si sposta una storia padre con sottoattività in [!UICONTROL Complete], la storia padre viene aggiornata al 100% e lo stato [!UICONTROL Status] in [!UICONTROL Complete]. Anche le sottoattività vengono aggiornate al 100% e lo [!UICONTROL Stato] viene aggiornato a [!UICONTROL Completo].

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> <p>Standard</p> 
   <p>Lavoro o superiore</p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td>Contribuire o gestire l'accesso all'attività su cui si trova la sottoattività</td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Aggiungi un&#39;attività secondaria a una storia esistente nella bacheca [!UICONTROL Kanban]

1. Vai alla bacheca [!UICONTROL Kanban] contenente la storia in cui desideri aggiungere un&#39;attività secondaria.
1. Fai clic sul nome dell&#39;attività nel riquadro del brano sulla bacheca [!UICONTROL Kanban].
1. Aggiungere un&#39;attività secondaria all&#39;attività come si farebbe in qualsiasi altro elenco di attività in [!DNL Workfront], come descritto in [Creare attività secondarie](../../manage-work/tasks/create-tasks/create-subtasks.md).
