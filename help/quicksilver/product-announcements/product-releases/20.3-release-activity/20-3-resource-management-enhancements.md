---
content-type: release-notes
navigation-topic: 2020-3-release-activity
title: 20.3 Miglioramenti alla gestione delle risorse
description: Questa pagina descrive tutti i miglioramenti apportati alla gestione delle risorse con la versione 20.3 nell’ambiente di produzione. Questi miglioramenti sono stati resi disponibili nell’ambiente di produzione la settimana del 10 agosto 2020.
author: Luke
feature: Product Announcements
exl-id: a2c34117-e03c-4394-9b81-7c18433531d1
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '829'
ht-degree: 0%

---

# 20.3 Miglioramenti alla gestione delle risorse

Questa pagina descrive tutti i miglioramenti apportati alla gestione delle risorse con la versione 20.3 nell’ambiente di produzione. Questi miglioramenti sono stati resi disponibili nell’ambiente di produzione la settimana del 10 agosto 2020.

Per un elenco di tutte le modifiche disponibili con la versione 20.3, vedi [Panoramica sulla versione 20.3](../../../product-announcements/product-releases/20.3-release-activity/20.3-release-overview.md).

## Includi ore dai problemi nell&#39;area Lavoro assegnato del servizio di bilanciamento del carico di lavoro

Per visualizzare un quadro completo dei carichi di lavoro delle persone, è stata introdotta un’impostazione che consente di includere ore dai problemi nell’area Lavoro assegnato del servizio di bilanciamento del carico di lavoro.

Per informazioni sull&#39;utilizzo del servizio di bilanciamento del carico di lavoro, vedi [Naviga nel bilanciamento del carico di lavoro](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Regolare le allocazioni per i giorni non lavorativi nel bilanciamento del carico di lavoro

È possibile modificare le allocazioni per le risorse per i giorni non lavorativi utilizzando il servizio di bilanciamento del carico di lavoro.

Per informazioni sulla gestione delle allocazioni nel servizio di bilanciamento del carico di lavoro, vedi [Gestire le allocazioni di utenti nel load balancer](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## Filtri variabili disponibili nel servizio di bilanciamento del carico di lavoro

Per migliorare la tua esperienza e offrirti maggiore flessibilità quando condividi informazioni, ora abbiamo implementato filtri variabili per il servizio di bilanciamento del carico di lavoro. I seguenti filtri sono stati aggiunti al servizio di bilanciamento del carico di lavoro:

* &quot;Me&quot; (quando si filtra per utenti)
* &quot;Il mio ruolo principale&quot; (quando si filtra per ruoli)
* &quot;My Home Team&quot; o &quot;All My Teams&quot; (quando si filtra per team).

Questi filtri sostituiscono le variabili del filtro jolly $$USER.ID, $$USER.roleID, $$USER.homeTeamID e $$USER.teamIDs

Quando applichi uno di questi filtri e condividi il servizio di bilanciamento del carico di lavoro o lo inserisci in un dashboard, tutti gli altri utenti visualizzeranno le loro informazioni.

Per informazioni sull&#39;applicazione di filtri al load balancer, vedi [Filtrare le informazioni nel servizio di bilanciamento del carico di lavoro](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

## Nuovo ordinamento per i progetti nel servizio di bilanciamento del carico di lavoro

Il servizio di bilanciamento del carico di lavoro ora ordina i progetti in base alla prima data di inizio pianificata e, in secondo luogo, alla data di completamento pianificata più recente delle attività del progetto che si verificano durante l&#39;intervallo di tempo visualizzato dall&#39;utente sullo schermo. Questo consente di organizzare il lavoro in una gerarchia ad albero che consente di identificare più facilmente il lavoro per un giorno.

Per informazioni sulla visualizzazione di progetti e elementi di lavoro nel servizio di bilanciamento del carico di lavoro, vedi [Naviga nel bilanciamento del carico di lavoro](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Visualizza l&#39;avanzamento effettivo del lavoro nel servizio di bilanciamento del carico di lavoro

Per fornire una prospettiva accurata dell&#39;avanzamento del carico di lavoro, abbiamo introdotto una nuova impostazione nel servizio di bilanciamento del carico di lavoro che mostra la cronologia delle attività e dei problemi in base alle rispettive date previste. È possibile abilitare l&#39;impostazione Mostra date previste per visualizzare la timeline proiettata dell&#39;elemento di lavoro oltre alla timeline pianificata.

Inoltre, con questo miglioramento, se un&#39;attività o un problema viene completato prima della data di completamento pianificata, le ore assegnate dai giorni rimanenti vengono rilevate per indicare che non vengono conteggiate per l&#39;allocazione complessiva dell&#39;utente.

Per informazioni sulla navigazione nel load balancer e sull’abilitazione delle impostazioni, consulta [Naviga nel bilanciamento del carico di lavoro](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Funzioni del servizio di bilanciamento del carico di lavoro precedentemente comunicate come rilasciate con la versione 20.2

* [Regolare l’allocazione giornaliera e settimanale nel bilanciamento del carico di lavoro](#adjust-daily-and-weekly-allocation-in-the-workload-balancer)
* [Aggiorna orario pianificato attività nel servizio di bilanciamento del carico di lavoro](#update-task-planned-hours-in-the-workload-balancer)
* [Un modo più conveniente per aggiornare le allocazioni nel load Balancer](#a-more-convenient-way-to-update-allocations-in-the-workload-balancer)

### Regolare l’allocazione giornaliera e settimanale nel bilanciamento del carico di lavoro {#adjust-daily-and-weekly-allocation-in-the-workload-balancer}

Per evitare il esaurimento delle risorse, ora puoi regolare l’allocazione giornaliera e settimanale degli utenti in modo che funzioni utilizzando il servizio di bilanciamento del carico di lavoro.

Prima di questo miglioramento, era possibile utilizzare solo gli strumenti di pianificazione delle risorse.

Per informazioni sulla gestione delle allocazioni nel servizio di bilanciamento del carico di lavoro, vedi [Gestire le allocazioni di utenti nel load balancer](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

**Disponibile nei seguenti ambienti:**

* Adobe Workfront Classic
* La nuova esperienza Adobe Workfront

### Aggiorna orario pianificato attività nel servizio di bilanciamento del carico di lavoro {#update-task-planned-hours-in-the-workload-balancer}

>[!NOTE]
>
>Questo miglioramento sarà disponibile in Produzione subito dopo la versione 2020.2.

Una nuova opzione nell’area Gestione risorse del livello di accesso ora consente agli utenti con questo accesso di modificare le ore pianificate dal servizio di bilanciamento del carico di lavoro. Quando si modificano le allocazioni nel servizio di bilanciamento del carico di lavoro, il totale delle allocazioni giornaliere non deve corrispondere al numero di ore pianificate delle attività. Una volta salvate le allocazioni, il totale delle ore di allocazione diventerà l&#39;orario pianificato dell&#39;attività. Questo è possibile solo per le attività con un tipo di durata semplice.

Per informazioni sulla gestione delle allocazioni nel servizio di bilanciamento del carico di lavoro, vedi [Gestire le allocazioni di utenti nel load balancer](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

Per informazioni sulla concessione dell&#39;accesso a Gestione risorse, vedere [Concedere l’accesso a Gestione risorse](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).

### Un modo più conveniente per aggiornare le allocazioni nel load Balancer {#a-more-convenient-way-to-update-allocations-in-the-workload-balancer}

Per semplificare la gestione delle allocazioni di un utente a un elemento di lavoro nel servizio di bilanciamento del carico di lavoro, è ora possibile fare doppio clic sull&#39;elemento di lavoro. È inoltre possibile utilizzare l&#39;opzione di menu Modifica allocazioni esistente. Inoltre, non è più necessario abilitare la visualizzazione delle allocazioni per poterle aggiornare.

Per informazioni sulla gestione delle allocazioni nel servizio di bilanciamento del carico di lavoro, vedi [Gestire le allocazioni di utenti nel load balancer](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).
