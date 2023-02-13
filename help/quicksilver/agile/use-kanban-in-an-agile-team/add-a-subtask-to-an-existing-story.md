---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Aggiungere una sottoattività a una storia esistente sulla bacheca Kanban
description: Leggi questo articolo per scoprire come creare sottoattività per le storie esistenti sulla bacheca Kanban.
author: Lisa
feature: Agile
exl-id: c6610616-80e5-4ded-9d23-63f15536e45c
source-git-commit: 9da0c8234f563a0202cd15017b37a341476f7406
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 0%

---

# Aggiungere una sottoattività a una storia esistente sulla bacheca Kanban

Durante la creazione di sottoattività per i brani esistenti, tenere presente quanto segue:

**Quando il [!UICONTROL Modalità completamento riepilogo] per il progetto è impostata su [!UICONTROL Manuale]:**

* È possibile spostare un brano principale con sottoattività in [!UICONTROL Completa], che aggiorna il brano principale al 100% e al [!UICONTROL Stato] a [!UICONTROL Completa]. Le sottoattività non vengono aggiornate.
* Per aggiornare [!UICONTROL Percentuale completata] per la storia, devi aggiornarla dal [!UICONTROL Storie] o dalla scheda [!UICONTROL Dettagli] della pagina dell&#39;oggetto.

**Quando il [!UICONTROL Modalità completamento riepilogo] per il progetto è impostata su [!UICONTROL Automatico]:**

* Non è possibile spostare il brano principale. Per aggiornare [!UICONTROL Percentuale completata] per la storia, devi aggiornare il [!UICONTROL Percentuale completata] per tutte le sottoattività. La [!UICONTROL Percentuale completata] per la storia viene calcolata in base al [!UICONTROL Percentuale completata] di tutte le sottoattività.
* Spostamento di un brano principale con sottoattività in [!UICONTROL Completa] aggiorna il brano principale al 100% e la [!UICONTROL Stato] a [!UICONTROL Completa]. Le sottoattività vengono inoltre aggiornate al 100% e [!UICONTROL Stato] è stato aggiornato a [!UICONTROL Completa].

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
   <td> <p>[!UICONTROL Work] o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni a livello di accesso*</strong></td> 
   <td> <p>[!UICONTROL Worker] o superiore</p> <p>Nota: Se non hai ancora accesso, chiedi [!DNL Workfront] amministratore se imposta ulteriori restrizioni nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il livello di accesso, vedi <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorizzazioni oggetto</strong></td> 
   <td> <p>[!UICONTROL Contribute] o [!UICONTROL Gestisci] accesso all'attività su cui si trova la sottoattività</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

## Aggiungi una sottoattività a una storia esistente nella [!UICONTROL Kanban] bacheca

1. Vai a [!UICONTROL Kanban] bacheca che contiene il racconto in cui si desidera aggiungere una sottoattività.
1. Fai clic sul nome dell&#39;attività nella sezione della storia del [!UICONTROL Kanban] consiglio di amministrazione.
1. Aggiungere un sottotask all&#39;attività come si farebbe in qualsiasi altro elenco di attività all&#39;interno di [!DNL Workfront], come descritto in [Creare sottoattività](../../manage-work/tasks/create-tasks/create-subtasks.md).
