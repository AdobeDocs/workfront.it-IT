---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Aggiungi un’attività secondaria a un brano esistente nel Kanban Board
description: Leggi questo articolo per scoprire come creare sottoattività per i brani esistenti sulla bacheca Kanban.
author: Lisa
feature: Agile
exl-id: c6610616-80e5-4ded-9d23-63f15536e45c
source-git-commit: 9da0c8234f563a0202cd15017b37a341476f7406
workflow-type: tm+mt
source-wordcount: '366'
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

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] piano*</strong></td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licenza*</strong></td> 
   <td> <p>[!UICONTROL Work] o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni del livello di accesso*</strong></td> 
   <td> <p>[!UICONTROL Worker] o versione successiva</p> <p>Nota: se non disponi ancora dell'accesso, chiedi all'amministratore [!DNL Workfront] se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di [!DNL Workfront] può modificare il livello di accesso, vedere <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorizzazioni oggetto</strong></td> 
   <td> <p>Accesso [!UICONTROL Contribute] o [!UICONTROL Gestisci] all'attività su cui si trova la sottoattività</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore [!DNL Workfront].

## Aggiungi un&#39;attività secondaria a una storia esistente nella bacheca [!UICONTROL Kanban]

1. Vai alla bacheca [!UICONTROL Kanban] contenente la storia in cui desideri aggiungere un&#39;attività secondaria.
1. Fai clic sul nome dell&#39;attività nel riquadro del brano sulla bacheca [!UICONTROL Kanban].
1. Aggiungere un&#39;attività secondaria all&#39;attività come si farebbe in qualsiasi altro elenco di attività in [!DNL Workfront], come descritto in [Creare attività secondarie](../../manage-work/tasks/create-tasks/create-subtasks.md).
