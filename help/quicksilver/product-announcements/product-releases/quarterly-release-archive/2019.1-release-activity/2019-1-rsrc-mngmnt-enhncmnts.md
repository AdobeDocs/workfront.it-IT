---
content-type: release-notes
navigation-topic: 2019-1-release-activity
title: Miglioramenti alla gestione delle risorse 2019.1
description: Questa pagina descrive tutti i miglioramenti alla gestione delle risorse inclusi nella versione 2019.1. Questa funzionalità è ora disponibile nell’ambiente di produzione.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6eed6023-96cc-45d7-8dae-a36d45e92068
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '953'
ht-degree: 0%

---

# Miglioramenti alla gestione delle risorse 2019.1

Questa pagina descrive tutti i miglioramenti alla gestione delle risorse inclusi nella versione 2019.1. Questa funzionalità è ora disponibile nell’ambiente di produzione.

Per un elenco di tutte le modifiche apportate in 2019.1, consulta [Panoramica delle attività sulla versione 2019.1](../../../../product-announcements/product-releases/quarterly-release-archive/2019.1-release-activity/2019-1-release-activity-overview.md).

## Filtro predefinito aggiornato nella pianificazione risorse

Il filtro predefinito nella Programmazione delle risorse non viene più filtrato in base al Gruppo del Progetto.

Quando si visualizza la Programmazione delle risorse, ora vengono visualizzati solo i progetti correnti e quelli con distinzione tra date per impostazione predefinita. Per impostazione predefinita sono incluse le informazioni dei seguenti progetti:

* Con una Data di completamento pianificata che si verifica dopo la prima data del mese corrente.
* Con una data di inizio pianificata che precede l&#39;ultima data del quarto mese a partire da oggi.
* Con lo stato Attuale o Pianificazione.

In precedenza, il filtro predefinito recuperava le informazioni dai seguenti progetti aggiuntivi:

* Con una Data di completamento pianificata che si verifica dopo la prima data del mese corrente.
* Con una data di inizio pianificata che precede l&#39;ultima data del quarto mese a partire da oggi.
* Con lo stato Attuale o Pianificazione.
* Con un gruppo che corrisponde al Gruppo Predefinito dell’utente connesso.

Per informazioni sull&#39;applicazione di filtri alla Programmazione delle risorse, vedere [Informazioni sui filtri nella Programmazione delle risorse](../../../../resource-mgmt/resource-planning/filter-resource-planner.md).

## Utilizzo dei caratteri jolly per i filtri di programmazione delle risorse

È ora possibile utilizzare i caratteri jolly per creare filtri nella Programmazione delle risorse. È ad esempio possibile utilizzare $$USER.ID per filtrare le informazioni sull&#39;utente connesso oppure $$USER.companyID per filtrare le informazioni su tutti gli utenti appartenenti alla stessa società dell&#39;utente connesso. Per un elenco completo delle variabili basate sugli utenti, vedere la sezione [Variabili filtro con caratteri jolly basate sugli utenti](../../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md#user-based-variables) in [Variabili filtro con caratteri jolly](../../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

In precedenza, i caratteri jolly non erano disponibili per i filtri di programmazione delle risorse.

Per informazioni sul filtro in Pianificazione risorse, vedere [Informazioni sul filtro in Pianificazione risorse](../../../../resource-mgmt/resource-planning/filter-resource-planner.md).

<!--
<iframe class="mt-media" src="assets/290697527?title=0&byline=0&portrait=0" width="640px" height="360px" frameborder="0" allowfullscreen></iframe>
-->

## Supporto per le variabili filtro con caratteri jolly basate sulla data nella pianificazione risorse

È ora possibile utilizzare qualsiasi versione della variabile di filtro con caratteri jolly $$TODAY quando si crea un filtro in Pianificazione risorse.

Prima di questo miglioramento, era possibile utilizzare solo variabili filtro con caratteri jolly basate sull’utente.

Per informazioni sul filtro in Pianificazione risorse, vedere [Informazioni sul filtro in Pianificazione risorse](../../../../resource-mgmt/resource-planning/filter-resource-planner.md).

Per informazioni sulle variabili filtro con caratteri jolly, vedere [Variabili filtro con caratteri jolly](../../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

## Opzioni di esportazione per la vista Ruolo nella Programmazione delle risorse

Nella visualizzazione Ruolo è ora possibile selezionare i livelli di informazioni da esportare dalla Programmazione delle risorse. È possibile esportare uno dei seguenti elementi:

* Solo ruoli
* Ruoli e Progetti
* Ruoli, progetti e utenti

Prima di questo miglioramento, tutti i livelli di informazioni venivano esportati nella vista Ruolo. Queste opzioni sono state introdotte nelle viste Progetto e Utente in una versione precedente.

Per informazioni sull&#39;esportazione di informazioni dalla Programmazione delle risorse, vedere [Esportare informazioni dalla Programmazione delle risorse](../../../../resource-mgmt/resource-planning/export-resource-planner.md).

## Opzioni di formattazione dei dati per l&#39;esportazione di Programmazione delle risorse

È ora possibile selezionare la modalità di visualizzazione delle informazioni nel file Excel quando vengono esportate dalla Programmazione delle risorse.

È possibile visualizzare la disponibilità e l&#39;allocazione delle informazioni esportate dalla Programmazione risorse nei modi seguenti:

* Separato dal nome degli oggetti a cui appartiene. In questo caso, i nomi degli oggetti a cui appartiene vengono visualizzati su ogni riga di dati. (opzione predefinita)
* Raggruppato per il nome degli oggetti a cui appartiene. In questo caso, le informazioni nel file esportato vengono visualizzate così come sono visualizzate in Workfront.

Prima di questo miglioramento, le informazioni nel file esportato venivano visualizzate come in Workfront.

Per informazioni sull&#39;esportazione di informazioni dalla Programmazione delle risorse, vedere [Esportare informazioni dalla Programmazione delle risorse](../../../../resource-mgmt/resource-planning/export-resource-planner.md).

## Timeline di programmazione persistente

>[!NOTE]
>
>Gli strumenti di pianificazione delle risorse sono stati dichiarati obsoleti e rimossi da Workfront con la versione 23.1. Per informazioni sulla pianificazione delle risorse tramite il Bilanciatore dei carichi di lavoro, vedere [Panoramica del Bilanciatore dei carichi di lavoro](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Le timeline di pianificazione ora mantengono l’intervallo temporale selezionato quando aggiorni la timeline o esci dalla pagina.

Prima di questo miglioramento, le timeline di pianificazione tornavano all’intervallo temporale predefinito quando si aggiornava la pagina o si usciva dalla pagina.

Questo miglioramento è disponibile nelle seguenti aree:

* Scheda Pianificazione nell’area Persone
* Scheda Team in funzione
* Scheda secondaria Pianificazione nella scheda Gestione del personale di un progetto

Per informazioni sull&#39;utilizzo della sequenza temporale nelle aree Programmazione risorse, vedere &quot;Introduzione alla programmazione delle risorse&quot;.

## Nuove opzioni di esportazione nella Programmazione delle risorse

È ora possibile selezionare i livelli di informazioni da esportare dalla Programmazione delle risorse. Nella vista Progetto, potete esportare uno dei seguenti elementi:

* Solo progetti
* Progetti e Ruoli
* Progetti, ruoli e utenti

Nella Vista utente, potete esportare uno dei seguenti elementi:

* Solo utenti
* Utenti e Progetti
* Utenti, progetti, ruoli, attività e problemi

Prima di questo miglioramento, per impostazione predefinita, tutti i livelli di informazioni venivano esportati in tutte le visualizzazioni del Programmatore risorse.

Per informazioni sull&#39;esportazione di informazioni dalla Programmazione delle risorse, vedere [Esportare informazioni dalla Programmazione delle risorse](../../../../resource-mgmt/resource-planning/export-resource-planner.md).

## Aggiornamento della Vista utente nella Programmazione delle risorse

Tutti gli utenti del sistema ora vengono visualizzati nella Vista utente della Programmazione delle risorse, ma solo gli utenti associati ai progetti filtrati mostrano anche le informazioni sulle ore.

Prima di questo aggiornamento, solo gli utenti assegnati agli elementi di lavoro sui progetti filtrati per vengono visualizzati nella Vista utente della Programmazione delle risorse.

È possibile utilizzare i filtri basati sugli utenti per ridurre il numero di utenti visualizzati nella Visualizzazione utente solo a quelli assegnati ai progetti che si desidera visualizzare.

Per informazioni sui filtri nella programmazione delle risorse, vedere [Informazioni sui filtri nella programmazione delle risorse](../../../../resource-mgmt/resource-planning/filter-resource-planner.md).
