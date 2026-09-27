---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Aggiungere un’attività secondaria a una storia esistente nel Kanban Board
description: Leggi questo articolo per scoprire come creare sottoattività per i brani esistenti sulla bacheca Kanban.
author: Courtney
feature: Agile
exl-id: c6610616-80e5-4ded-9d23-63f15536e45c
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: 'https://experienceleague.adobe.com/Wbiao1UjwOzItIGJkh1E9A81RcUfLDJqgYjRDL46qvQ'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
subfeature_v2:
  - id: be65ef36-43e4-48e1-a062-caa3778e15be
    internal-label: Agile
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '305'
ht-degree: 14%
---
# Aggiungere un’attività secondaria a una storia esistente nella bacheca Kanban

Quando create sottoattività per i brani esistenti, tenete presente quanto segue:

**Quando l&#39;impostazione [!UICONTROL Modalità di completamento riepilogo] per il progetto è impostata su [!UICONTROL Manuale]:**

* Puoi spostare una storia padre con sottoattività in [!UICONTROL Completo], che aggiorna la storia padre al 100% e lo [!UICONTROL Stato] in [!UICONTROL Completo]. Le sottoattività non vengono aggiornate.
* Per aggiornare la [!UICONTROL Percentuale completata] per la storia, è necessario aggiornarla dalla scheda [!UICONTROL Storie] o dalla pagina [!UICONTROL Dettagli] dell&#39;oggetto.

**Quando l&#39;impostazione [!UICONTROL Modalità di completamento riepilogo] per il progetto è impostata su [!UICONTROL Automatica]:**

* Non potete spostare la storia principale in senso orizzontale. Per aggiornare [!UICONTROL Percent Complete] per la storia, è necessario aggiornare [!UICONTROL Percent Complete] per le sottoattività. La [!UICONTROL Percentuale completata] per il brano viene calcolata in base alla [!UICONTROL Percentuale completata] di tutte le sottoattività.
* Se si sposta una storia padre con sottoattività in [!UICONTROL Complete], la storia padre viene aggiornata al 100% e lo stato [!UICONTROL Status] in [!UICONTROL Complete]. Anche le sottoattività vengono aggiornate al 100% e lo [!UICONTROL Stato] viene aggiornato a [!UICONTROL Completo].

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

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
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td> <p>Standard</p> 
   <p>Work o successiva</p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
   <td>Contribuire o gestire l'accesso all'attività su cui si trova la sottoattività</td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Aggiungi un&#39;attività secondaria a una storia esistente nella bacheca [!UICONTROL Kanban]

1. Vai alla bacheca [!UICONTROL Kanban] contenente la storia in cui desideri aggiungere un&#39;attività secondaria.
1. Fai clic sul nome dell&#39;attività nel riquadro del brano sulla bacheca [!UICONTROL Kanban].
1. Aggiungere un&#39;attività secondaria all&#39;attività come si farebbe in qualsiasi altro elenco di attività in [!DNL Workfront], come descritto in [Creare attività secondarie](../../manage-work/tasks/create-tasks/create-subtasks.md).
