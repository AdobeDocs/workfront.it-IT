---
content-type: release-notes
navigation-topic: 2020-3-release-activity
title: 20.3 Miglioramenti alla gestione delle risorse
description: Questa pagina descrive tutti i miglioramenti alla gestione delle risorse apportati con la versione 20.3 all’ambiente di produzione. Questi miglioramenti sono stati resi disponibili nell’ambiente di produzione la settimana del 10 agosto 2020.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: a2c34117-e03c-4394-9b81-7c18433531d1
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '837'
ht-degree: 0%

---

# 20.3 Miglioramenti alla gestione delle risorse

Questa pagina descrive tutti i miglioramenti alla gestione delle risorse apportati con la versione 20.3 all’ambiente di produzione. Questi miglioramenti sono stati resi disponibili nell’ambiente di produzione la settimana del 10 agosto 2020.

Per un elenco di tutte le modifiche disponibili con la versione 20.3, consulta la [panoramica sulla versione 20.3](../../../product-announcements/product-releases/20.3-release-activity/20-3-release-overview.md).

## Includi ore da problemi nell’area Lavoro assegnato del Bilanciatore dei carichi di lavoro

Per consentirti di visualizzare un quadro completo di tutti i carichi di lavoro delle persone, abbiamo introdotto un’impostazione che consente di includere le ore dei problemi nell’area Lavoro assegnato del Bilanciatore dei carichi di lavoro.

Per informazioni sul funzionamento del Bilanciatore dei carichi di lavoro, vedere [Navigare nel Bilanciatore dei carichi di lavoro](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Regolare le allocazioni per i giorni non lavorativi nel Bilanciatore dei carichi di lavoro

È possibile regolare le allocazioni per le risorse per i giorni non lavorativi utilizzando il Bilanciatore dei carichi di lavoro.

Per informazioni sulla gestione delle allocazioni nel Bilanciatore dei carichi di lavoro, vedere [Gestione delle allocazioni utente nel Bilanciatore dei carichi di lavoro](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## Filtri per variabili disponibili nel Bilanciatore dei carichi di lavoro

Per migliorare la tua esperienza e darti maggiore flessibilità nella condivisione delle informazioni, ora abbiamo implementato filtri variabili per il Bilanciatore dei carichi di lavoro. I seguenti filtri sono stati aggiunti al Bilanciatore dei carichi di lavoro:

* &quot;Me&quot; (quando si filtra per utenti)
* &quot;Il mio ruolo principale&quot; (quando si filtra per ruoli)
* &quot;Il mio team predefinito&quot; o &quot;Tutti i miei team&quot; (quando si filtra per team).

Questi filtri sostituiscono le variabili di filtro con caratteri jolly di $$USER.ID, $$USER.roleID, $$USER.homeTeamID e $$USER.teamIDs

Quando applichi uno di questi filtri e condividi il Bilanciatore dei carichi di lavoro o lo inserisci in un dashboard, tutti gli altri utenti visualizzeranno le proprie informazioni.

Per informazioni sull&#39;applicazione dei filtri al Bilanciatore dei carichi di lavoro, vedere [Informazioni sui filtri nel Bilanciatore dei carichi di lavoro](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

## Nuovo ordinamento per i progetti nel Bilanciatore dei carichi di lavoro

Il Bilanciatore dei carichi di lavoro ora ordina i progetti in base alla prima Data inizio pianificata e in secondo luogo alla Data completamento pianificata più recente delle attività nel progetto che si verificano durante l’arco temporale visualizzato dall’utente. Questo consente di organizzare il lavoro in una gerarchia ad albero che consente di identificare più facilmente il lavoro per una giornata.

Per informazioni sulla visualizzazione dei progetti e degli elementi di lavoro nel Bilanciatore dei carichi di lavoro, vedere [Navigare nel Bilanciatore dei carichi di lavoro](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Visualizzare l’avanzamento del lavoro effettivo nel Bilanciatore dei carichi di lavoro

Per fornire una prospettiva accurata dell’avanzamento del carico di lavoro, nel Bilanciatore dei carichi di lavoro è stata introdotta una nuova impostazione che mostra la tempistica delle attività e dei problemi in base alle date previste. È possibile abilitare l&#39;impostazione Mostra date previste per visualizzare la sequenza temporale prevista dell&#39;elemento di lavoro oltre alla sequenza temporale pianificata.

Inoltre, con questo miglioramento, se un’attività o un problema viene completato prima della data di completamento pianificata, le ore allocate dai giorni rimanenti vengono completate per indicare che non vengono conteggiate nell’allocazione complessiva dell’utente.

Per informazioni su come navigare nel Bilanciatore dei carichi di lavoro e abilitare le impostazioni, vedere [Navigare nel Bilanciatore dei carichi di lavoro](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Funzioni del Bilanciatore dei carichi di lavoro precedentemente comunicate come rilascio con la versione 20.2

* [Regola l&#39;allocazione giornaliera e settimanale nel Bilanciatore dei carichi di lavoro](#adjust-daily-and-weekly-allocation-in-the-workload-balancer)
* [Aggiorna le ore pianificate per l&#39;attività nel Bilanciatore dei carichi di lavoro](#update-task-planned-hours-in-the-workload-balancer)
* [Un modo più pratico per aggiornare le allocazioni nel Bilanciatore dei carichi di lavoro](#a-more-convenient-way-to-update-allocations-in-the-workload-balancer)

### Regolare l’allocazione giornaliera e settimanale nel Bilanciatore dei carichi di lavoro {#adjust-daily-and-weekly-allocation-in-the-workload-balancer}

Per evitare il burnout delle risorse, ora puoi regolare l’allocazione giornaliera e settimanale degli utenti in modo che funzioni utilizzando il Bilanciatore dei carichi di lavoro.

Prima di questo miglioramento, questo era possibile solo utilizzando gli strumenti di pianificazione delle risorse.

Per informazioni sulla gestione delle allocazioni nel Bilanciatore dei carichi di lavoro, vedere [Gestione delle allocazioni utente nel Bilanciatore dei carichi di lavoro](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

**Disponibile in questi ambienti:**

* Adobe Workfront Classic
* La nuova esperienza Adobe Workfront

### Aggiornare le ore pianificate per l’attività nel Bilanciatore dei carichi di lavoro {#update-task-planned-hours-in-the-workload-balancer}

>[!NOTE]
>
>Questo miglioramento sarà disponibile in produzione subito dopo la versione 2020.2.

Una nuova opzione nell’area Gestione risorse del livello di accesso ora consente agli utenti con questo livello di accesso di modificare le Ore pianificate dal Bilanciatore dei carichi di lavoro. Quando si modificano le allocazioni nel Bilanciatore dei carichi di lavoro, il totale delle allocazioni giornaliere non deve necessariamente corrispondere al numero di ore pianificate delle attività. Una volta salvate le allocazioni, il totale delle ore di allocazione diventerà le ore pianificate dell&#39;attività. Ciò è possibile solo per le attività con un tipo di durata semplice.

Per informazioni sulla gestione delle allocazioni nel Bilanciatore dei carichi di lavoro, vedere [Gestione delle allocazioni utente nel Bilanciatore dei carichi di lavoro](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

Per informazioni sulla concessione dell&#39;accesso a Gestione risorse, vedere [Concedere l&#39;accesso a Gestione risorse](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).

### Un modo più pratico per aggiornare le allocazioni nel Bilanciatore dei carichi di lavoro {#a-more-convenient-way-to-update-allocations-in-the-workload-balancer}

Per semplificare la gestione delle allocazioni di un utente a un elemento di lavoro nel Bilanciatore dei carichi di lavoro, è ora possibile fare doppio clic sull’elemento di lavoro. È inoltre possibile utilizzare l&#39;opzione di menu Modifica allocazioni esistente. Inoltre, non è più necessario abilitare la visualizzazione delle allocazioni per poterle aggiornare.

Per informazioni sulla gestione delle allocazioni nel Bilanciatore dei carichi di lavoro, vedere [Gestione delle allocazioni utente nel Bilanciatore dei carichi di lavoro](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).
