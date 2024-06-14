---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Effettua assegnazioni intelligenti
description: È possibile utilizzare le assegnazioni avanzate per identificare l'utente migliore per completare il lavoro. Le assegnazioni intelligenti sono suggerimenti per utenti, ruoli o team presentati da Adobe Workfront quando si assegnano elementi di lavoro alle risorse in base a un algoritmo che determina la risorsa più appropriata per il processo. Per informazioni sulle assegnazioni Smart, vedere Cenni preliminari sulle assegnazioni Smart.
author: Alina
feature: Work Management
exl-id: 073a3234-3156-4b4f-a3e1-dbb32d61068a
source-git-commit: 02a47566acd0fff151656fe2c5b59a6679748b15
workflow-type: tm+mt
source-wordcount: '620'
ht-degree: 0%

---

# Effettua assegnazioni intelligenti

<!--keep the yellow around the Rate card job roles and the Preview intro for those-->

<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti oppure nell’ambiente di produzione per i clienti che hanno abilitato le versioni rapide.</span>

<span class="preview">Per informazioni sulle versioni rapide, consulta [Abilitare o disabilitare le versioni rapide per la tua organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">Per informazioni sulla versione corrente, consulta [Panoramica sulla versione del terzo trimestre 2024](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).</span>

È possibile utilizzare le assegnazioni avanzate per identificare l&#39;utente migliore per completare il lavoro.

Le assegnazioni intelligenti sono suggerimenti per utenti, ruoli o team che Adobe Workfront presenta quando si assegnano elementi di lavoro alle risorse. Workfront basa i suoi suggerimenti su un algoritmo che determina la risorsa più appropriata per il processo.

<span class="preview">In Workfront sono disponibili due algoritmi distinti che calcolano le assegnazioni intelligenti che funzionano in modo diverso per le attività e per i problemi. </span>

Per ulteriori informazioni sui criteri utilizzati per determinare le assegnazioni intelligenti, consulta [Panoramica delle assegnazioni intelligenti](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

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
   <td> <p>Autorizzazioni di tipo Contribuisci o più elevato con la possibilità di effettuare assegnazioni su attività e problemi</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni sulla pianificazione, il tipo di licenza o l&#39;accesso disponibili, contattare l&#39;amministratore Workfront. Per ulteriori informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Effettua assegnazioni intelligenti

Le assegnazioni intelligenti sono disponibili nella maggior parte delle posizioni in cui è possibile effettuare assegnazioni in Workfront.

1. Vai alle seguenti aree e fai clic su **Assegnazioni** o **Assegna a** campo:

   * Un elenco di attività o problemi o un rapporto
   * Un’intestazione di attività o problema
   * Pannello Riepilogo dell’attività o del problema
   * <span class="preview">Una casella Nuova attività o Nuovo problema quando si aggiunge una nuova attività o un nuovo problema a un progetto</span>
   * Il campo Assegnazioni per un elemento elencato nell&#39;area Home
   * Un’attività o un problema nel Bilanciatore dei carichi di lavoro

1. Posizionare il cursore nel campo Assegnazioni e attendere due secondi.

   <div class="preview">
   Vengono visualizzate una o più delle seguenti sezioni con suggerimenti di assegnazione intelligente:

   * **Assegnazioni suggerite**: viene visualizzata per le attività. <!--remove the note when we go to production with smarter assignments-->

     >[!TIP]
     >
     >   Viene visualizzata l’intestazione dell’elenco **Di seguito sono riportati alcuni consigli** invece di **Assegnazioni suggerite** nell’ambiente di produzione.
     >
   * **Utenti e team**: viene visualizzata per le attività e i problemi.
   * **Ruoli**: viene visualizzato per attività e problemi.
   * **Valuta ruoli scheda**: viene visualizzata per le attività. Per ulteriori informazioni, consulta [Gestire le schede delle tariffe](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).<!--check later with Lisa to see if this also came to issues?! - and always keep this in yellow-->
   </div>

   <span class="preview">![](assets/smart-assignments-task-header-nwe-350x302.png)</span>


   Per le attività, le assegnazioni intelligenti vengono visualizzate nelle sezioni seguenti, a seconda della fase di calcolo dell&#39;algoritmo che ha identificato le assegnazioni:

   * **Assegnazioni suggerite**: assegnazioni identificate nella prima fase del calcolo dell&#39;algoritmo dell&#39;assegnazione intelligente dell&#39;attività. <span class="preview">Questa sezione non è disponibile per i problemi.</span>
   * <span class="preview">**Utenti e team**, **Ruoli**, o **Valuta ruoli scheda**: assegnazioni identificate nella seconda fase del calcolo dell&#39;algoritmo dell&#39;assegnazione intelligente dell&#39;attività. <!--no longer valid: This section is not available for issues. --></span> <!--replace this with the new UI: "Other assignments"-->

   <span class="preview">![](assets/smart-assignments-task-list.png)</span>

   Per ulteriori informazioni, consulta [Panoramica delle assegnazioni intelligenti](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

1. Seleziona l’utente nell’elenco dei consigli facendo clic sul nome.

1. (Facoltativo) Fai clic su **Assegna a me** per assegnare l&#39;elemento di lavoro a se stessi.

   >[!TIP]
   >
   >Se non sono presenti suggerimenti, l&#39;elenco dei suggerimenti non viene aperto.

1. (Facoltativo) Se non desideri utilizzare uno degli utenti consigliati dall’elenco Assegnazioni avanzate, inizia a digitare il nome della risorsa desiderata e selezionalo quando viene visualizzato nell’elenco.
1. Clic **Invio** per effettuare l&#39;assegnazione.

   L’utente selezionato è assegnato all’attività o al problema.
