---
content-type: reference
product-area: resource-management
keywords: carico di lavoro, bilanciamento
navigation-topic: resource-management-overview
title: Strumenti di pianificazione delle risorse obsoleti in Adobe Workfront
description: Al momento stiamo deprecando tutti gli strumenti di pianificazione da Adobe Workfront e li sostituiremo con il servizio di bilanciamento del carico di lavoro.
author: Alina
feature: Resource Management
exl-id: 7fa644cd-cf6a-40f8-ae28-bf222bb45d3f
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '873'
ht-degree: 0%

---

# Strumenti di pianificazione delle risorse obsoleti in Adobe Workfront

>[!IMPORTANT]
>  
><span class="preview">La funzionalità di pianificazione descritta in questo articolo è stata rimossa e rimossa da Adobe Workfront a partire dalla versione 23.1 di gennaio 2023.   </span>
>  
> <span class="preview"> Questo articolo verrà rimosso anche poco dopo la versione 23.1, all’inizio del 2023. Al momento, è consigliabile aggiornare di conseguenza tutti i segnalibri. </span>
> 
><span class="preview"> Ora puoi utilizzare il servizio di bilanciamento del carico di lavoro per pianificare il lavoro per le risorse. </span>
>  
> <span class="preview">Per informazioni sulla pianificazione delle risorse tramite il servizio di bilanciamento del carico di lavoro, consulta la sezione . [Il servizio di bilanciamento del carico di lavoro](../../resource-mgmt/workload-balancer/workload-balancer.md). </span>

<!--
We are currently in the process of removing all Scheduling tools from Adobe Workfront and replacing them with the Workload Balancer.

>[!IMPORTANT]
>
>We are no longer implementing new feature functionality for the current Scheduling solution and we no longer consider nor prioritize defects for a fix in this area of Adobe Workfront.

This article describes the timeline for this deprecation and it compares the functionality of the Scheduling tools and that of the Workload Balancer to indicate which Scheduling capabilities are already supported in the Workload Balancer. 

We have been announcing a more exact timeline through the Announcement Center at key milestones during the deprecation process and this article has been updated as this process continues.

>[!NOTE]
>
>The changes described in this article do not affect any other resource management tools. For example, they do not affect the [!UICONTROL Resource Planner] or the [!UICONTROL Utilization] report.
-->

## Come preparare

Per informazioni dettagliate su come preparare la transizione tra Pianificazione e il bilanciamento del carico di lavoro, vedi [Migrazione da Resource Scheduling al load Balancer](../../resource-mgmt/resource-mgmt-overview/migrate-resource-scheduling-to-workload-balancer.md).

Se al momento utilizzi gli strumenti di pianificazione, ti consigliamo di interromperli e iniziare a utilizzare il servizio di bilanciamento del carico di lavoro.

![Area di programmazione delle risorse globale](assets/resource-scheduler-global-350x127.png)

Quasi tutte le funzionalità precedentemente disponibili nelle aree di pianificazione sono ora disponibili nel servizio di bilanciamento del carico di lavoro. Per informazioni, consulta la sezione . [Disponibilità delle funzioni](#feature-availability) in questo articolo. Puoi continuare a pianificare le tue risorse per lavorare esclusivamente nel servizio di bilanciamento del carico di lavoro.

![Area di bilanciamento del carico di lavoro globale](assets/workload-balancer-pti-350x111.png)

## Informazioni che non verranno trasferite al servizio di bilanciamento del carico di lavoro

Le seguenti informazioni non verranno trasferite dagli strumenti di programmazione al servizio di bilanciamento del carico di lavoro:

* **Allocazione giornaliera per gli utenti**: Non utilizzare contemporaneamente entrambi i programmi e il servizio di bilanciamento del carico di lavoro per regolare le stesse allocazioni utente. Se negli strumenti di programmazione sono state gestite le allocazioni utente, le allocazioni giornaliere corrette non vengono trasferite al servizio di bilanciamento del carico di lavoro. Analogamente, se le allocazioni utente sono state modificate nel load Balancer, non vengono trasferite agli strumenti di programmazione. Ti invitiamo caldamente a garantire che le allocazioni giornaliere siano accurate nel servizio di bilanciamento del carico di lavoro per prepararti a questa transizione. Per informazioni, consulta [Gestire le allocazioni di utenti nel load balancer](../workload-balancer/manage-user-allocations-workload-balancer.md).
* **Filtri**: Se hai salvato i filtri nelle aree di programmazione, non vengono trasferiti al servizio di bilanciamento del carico di lavoro. È necessario ricreare i filtri nel servizio di bilanciamento del carico di lavoro. Per informazioni, consulta [Filtrare le informazioni nel servizio di bilanciamento del carico di lavoro](../workload-balancer/filter-information-workload-balancer.md).

## Elementi di rilievo della timeline obsoleta

>[!IMPORTANT]
>
>Utilizza questo articolo per conoscere la timeline più recente per la deprecazione degli strumenti di pianificazione. Eventuali aggiornamenti a questa timeline verranno comunicati in questo articolo e nei messaggi di Centro annunci .

Di seguito è riportata una cronologia del processo di deprecazione degli strumenti di pianificazione delle risorse:

* [Versione 2020.4 (novembre 2020)](#2020-4-release-november-2020)
* [Versione 2021.4 (ottobre 2021)](#2021-4-release-october-2021)
* [Versioni 2022.4 - 2023.1 (ottobre 2022 - gennaio 2023)](#2022-4-2023-1-releases)

### Versione 2020.4 (novembre 2020) {#2020-4-release-november-2020}

* La nuova funzionalità non è più implementata per la soluzione di programmazione
* Solo i difetti di gravità alta e critica avranno priorità per una correzione
* Nuove funzionalità di bilanciamento del carico di lavoro aggiunte a Workfront

### Versione 2021.4 (ottobre 2021) {#2021-4-release-october-2021}

* Il servizio di bilanciamento del carico di lavoro è impostato come predefinito per qualsiasi nuovo utente di Workfront
* Filtri migliorati che possono essere condivisi e includere campi aggiuntivi

### Versioni 2022.4 - 2023.1 (ottobre 2022 - gennaio 2023) {#2022-4-2023-1-releases}

* Nessun difetto verrà attribuito la priorità a una correzione durante e dopo le versioni 2022.4 o 2023.1
* Tutte le aree di programmazione vengono rimosse dall&#39;ambiente di anteprima (**20 ottobre 2022**)
* Tutte le aree di programmazione vengono rimosse dall&#39;ambiente di produzione (**Gennaio 2023**)
* Il servizio di bilanciamento del carico di lavoro è l’unico strumento di pianificazione delle risorse disponibile in Workfront (dopo **Gennaio 2023**)

## Disponibilità delle funzioni {#feature-availability}

Se non diversamente specificato, tutte le funzionalità di pianificazione delle risorse sono state o saranno disponibili nel servizio di bilanciamento del carico di lavoro. Per informazioni sul bilanciamento del carico di lavoro, vedi [Panoramica del servizio di bilanciamento del carico di lavoro](../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Oltre alle funzioni esistenti, il servizio di bilanciamento del carico di lavoro dispone o disporrà di nuove funzionalità che non esistevano negli strumenti di programmazione delle risorse, come illustrato nella tabella seguente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td rowspan="2"><span style="font-weight: normal;"><b>Funzioni</b></span> </td> 
   <td rowspan="2"> <b>Disponibilità della funzionalità degli strumenti di pianificazione delle risorse</b></td> 
   <td colspan="3"><b>Disponibilità della funzione di bilanciamento del carico di lavoro</b></td> 
  </tr> 
  <tr> 
   <td><b>Disponibile ora</b></td> 
   <td><b>Disponibile a breve</b></td> 
   <td><b>Non pianificato</b></td> 
  </tr> 
  <tr> 
   <td> <p>Strumento di accesso dall'area Risorse</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Aree separate per il lavoro non assegnato e assegnato</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Applicazione e creazione di filtri per lavoro non assegnato e assegnato</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Accedere agli elementi di lavoro direttamente dallo strumento</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Assegnazione o annullamento manuale di attività e problemi</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Regolare le singole allocazioni</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Includi ora del problema</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Visualizza date previste </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Visualizza lavoro completato</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Mostra le eccezioni di orario utente, fine settimana e pianificazione</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>Assegnazione rapida degli utenti in base ai ruoli*</span> </td> 
   <td>✓</td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>Sostituzione rapida degli utenti*</span> </td> 
   <td>✓</td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>Disassegnazione rapida degli utenti*</span> </td> 
   <td>✓</td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><span>Accesso a uno strumento da un team</span> </td> 
   <td>✓</td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><span>Accesso a uno strumento da un progetto</span> </td> 
   <td>✓</td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr>
   <td>Gli utenti con licenza di lavoro possono regolare le allocazioni degli utenti quando accedono al servizio di bilanciamento del carico di lavoro da un progetto </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td></td> 
   <td></td> 
  </tr> 
  <tr> 
   <td>Problemi di visualizzazione nell'area di lavoro non assegnata</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td></td> 
   <td></td> 
  </tr> 
  <tr> 
   <td><span>Assegnare e annullare l’assegnazione di attività e problemi mediante trascinamento*</span> </td> 
   <td>✓</td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Visibile a tutti gli utenti del piano, senza essere designato come Resource Manager per il progetto.</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Raggruppa informazioni per progetto</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Condivisione del servizio di bilanciamento del carico di lavoro con utenti senza accesso all'area di determinazione origine</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Visualizza e regola le allocazioni per settimana</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Accedere agli utenti direttamente dallo strumento</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Accedere a ulteriori informazioni sugli elementi di lavoro senza spostarsi all'interno del pannello Riepilogo*</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Visualizza e regola l'allocazione come valore percentuale </td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Visualizza la differenza tra il tempo disponibile e quello allocato</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Visualizzazione della disponibilità degli utenti in un grafico</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Codice colore per elementi di lavoro e progetti in base allo stato del progetto</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Aggiorna automaticamente le ore pianificate durante la regolazione dell'allocazione utente (per le attività con un tipo di durata semplice)</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><span>Suggerire le assegnazioni in base al modello di assegnazione dell'utente, alle assegnazioni esistenti di Ruolo o Team</span> </td> 
   <td> </td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Filtri migliorati che possono essere condivisi e includere campi aggiuntivi</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><span>Esecuzione di assegnazioni avanzate</span> </td> 
   <td> </td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td> 
  </tr>

<tr> 
   <td><span>Codice colore degli elementi di lavoro in base ai progetti e allo stato del progetto</span> </td> 
   <td> </td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td>

<tr> 
   <td>Aggiungi utenti al team del progetto (reindirizzati al <b>Persone</b> scheda del progetto) </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td></td> 
   <td> </td>

</tr>
   <tr> 
   <td>Assegnazione automatica di attività e problemi</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr>

</tbody> 
</table>

*Queste funzioni sono disponibili solo nella nuova esperienza Adobe Workfront.
