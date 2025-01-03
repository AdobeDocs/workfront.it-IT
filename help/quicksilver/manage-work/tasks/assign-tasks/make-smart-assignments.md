---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Effettua assegnazioni intelligenti
description: È possibile utilizzare le assegnazioni avanzate per identificare l'utente migliore per completare il lavoro. Le assegnazioni intelligenti sono suggerimenti per utenti, ruoli o team presentati da Adobe Workfront quando si assegnano elementi di lavoro alle risorse in base a un algoritmo che determina la risorsa più appropriata per il processo. Per informazioni sulle assegnazioni Smart, vedere Cenni preliminari sulle assegnazioni Smart.
author: Alina
feature: Work Management
exl-id: 073a3234-3156-4b4f-a3e1-dbb32d61068a
source-git-commit: 412645a802bdf9057bb61a5a96df257daa1c3948
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%

---

# Effettua assegnazioni intelligenti

<!--Audited: 07/2024-->

<!--keep the yellow around the Rate card job roles and the Preview intro for those-->

<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono alle funzionalità disponibili solo nell&#39;ambiente di produzione per i clienti che hanno abilitato le versioni rapide.</span>

<span class="preview">Per informazioni sulle versioni rapide, vedi [Abilitare o disabilitare le versioni rapide per la tua organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview"> Questa funzionalità verrà rimossa dall&#39;ambiente di produzione per i clienti che hanno abilitato la versione rapida con la versione 25.1 a gennaio 2025. Per informazioni sulla versione 25.1, consulta [Panoramica sulla versione del primo trimestre 2025](/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-release-overview.md).

È possibile utilizzare le assegnazioni avanzate per identificare l&#39;utente migliore per completare il lavoro.

Le assegnazioni intelligenti sono suggerimenti per utenti, ruoli o team che Adobe Workfront presenta quando si assegnano elementi di lavoro alle risorse. Workfront basa i suoi suggerimenti su un algoritmo che determina la risorsa più appropriata per il processo.

<span class="preview">In Workfront sono presenti due algoritmi distinti che calcolano le assegnazioni intelligenti che funzionano in modo diverso per le attività e per i problemi.</span>

Per ulteriori informazioni sui criteri utilizzati per determinare le assegnazioni Smart, vedere [Panoramica assegnazioni Smart](/help/quicksilver/manage-work/tasks/assign-tasks/smart-assignments.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Nuovo: Standard</p>
      Oppure
      <p>Corrente: Lavoro o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica l'accesso ad Attività e Issues</p> <p>Accesso ai progetti di visualizzazione o superiore</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Autorizzazioni Contribute o superiori con la possibilità di effettuare assegnazioni su attività e problemi</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Effettua assegnazioni intelligenti

Le assegnazioni intelligenti sono disponibili nella maggior parte delle posizioni in cui è possibile effettuare assegnazioni in Workfront.

1. Vai alle seguenti aree e fai clic sul campo **Assegnazioni** o **Assegna a**:

   * Un elenco di attività o problemi o un rapporto
   * Un’intestazione di attività o problema
   * Pannello Riepilogo dell’attività o del problema
   * <span class="preview">Una nuova attività</span> o una nuova casella Problema, quando si aggiunge <span class="preview">una nuova attività</span> o un problema a un progetto
   * Un’attività o un problema nel Bilanciatore dei carichi di lavoro

1. Posizionare il cursore nel campo Assegnazioni e attendere due secondi.

   Per i problemi, le assegnazioni intelligenti vengono visualizzate nelle sezioni seguenti:

   * **Utenti e team**
   * **Ruoli**

   ![](assets/smart-assignments-issue-header.png)

   Per le attività, le assegnazioni intelligenti vengono visualizzate nelle sezioni seguenti, a seconda della fase di calcolo dell&#39;algoritmo che ha identificato le assegnazioni:

   * <span class="preview">**Assegnazioni suggerite**: visualizza le assegnazioni identificate nella prima fase dell&#39;algoritmo di assegnazione intelligente delle attività.</span>
   * **Utenti e team**, **Ruoli** o <span class="preview">**Ruoli con scheda di valutazione**</span>: assegnazioni identificate nella seconda fase del calcolo dell&#39;algoritmo dell&#39;assegnazione intelligente dell&#39;attività.

   <span class="preview">![](assets/smart-assignments-task-list.png)</span>

   Per ulteriori informazioni, vedere [Panoramica assegnazioni avanzate](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

1. Seleziona la risorsa nell’elenco dei consigli facendo clic sul nome.

1. (Facoltativo) Fai clic su **Assegna a me** per assegnare l&#39;elemento di lavoro a te stesso.

   >[!TIP]
   >
   >Se non sono presenti suggerimenti, l&#39;elenco dei suggerimenti non viene aperto.

1. (Facoltativo) Se non desideri utilizzare uno degli utenti consigliati dall’elenco Assegnazioni avanzate, inizia a digitare il nome della risorsa desiderata e selezionalo quando viene visualizzato nell’elenco.
1. Fai clic su **Invio** per effettuare l&#39;assegnazione.

   L’utente selezionato è assegnato all’attività o al problema.
