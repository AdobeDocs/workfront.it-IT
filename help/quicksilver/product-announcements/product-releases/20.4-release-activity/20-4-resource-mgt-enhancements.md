---
title: 20.4 Miglioramenti alla gestione delle risorse
description: 20.4 Miglioramenti alla gestione delle risorse
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 9f660a38-4a59-4135-8178-0841088cc7d6
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '1043'
ht-degree: 0%

---

# 20.4 Miglioramenti alla gestione delle risorse

Questa pagina descrive tutti i miglioramenti apportati alla gestione delle risorse con la versione 20.4 nell’ambiente di anteprima. Questi miglioramenti saranno resi disponibili nell&#39;ambiente di produzione la settimana del 9 novembre 2020.

Per un elenco di tutte le modifiche disponibili con la versione 20.4, vedi [Panoramica sulla versione 20.4](../../../product-announcements/product-releases/20.4-release-activity/20-4-release-overview.md).

## Pianificare il lavoro utilizzando lo sforzo di lavoro anziché le ore pianificate

Per offrirti flessibilità nella pianificazione dei progetti, abbiamo introdotto il nuovo concetto di impegno di lavoro per le attività. È possibile stimare se lo sforzo di lavoro per un&#39;attività è piccolo, medio o grande senza stimare manualmente le ore pianificate per l&#39;attività. Ogni livello di sforzo viene calcolato in base a una percentuale di tempo a partire dalle ore giornaliere tipiche, come configurato nella tua istanza.

Con questa nuova funzione sono ora disponibili i seguenti miglioramenti:

* Abilita questa impostazione per progetti e modelli per renderla disponibile per attività e attività modello
* Aggiorna questa impostazione per ogni attività con un tipo di durata semplice che aggiorna automaticamente l&#39;orario pianificato dell&#39;attività
* Disattiva questa impostazione utilizzando un modello di layout per gli utenti che preferiscono continuare a utilizzare le ore pianificate.
* Visualizza il valore del nuovo campo in un elenco di attività o in un report.

Per informazioni sullo sforzo di lavoro, vedi [Panoramica sullo sforzo di lavoro](../../../manage-work/tasks/task-information/work-effort.md).

Questa funzione è ora inclusa nella [Nozioni di base del planner, percorso di apprendimento parte 2](https://one.workfront.com/s/learningpath3/planner-fundamentals-for-the-new-workfront-experience-part-2-plan-a-project-20Y0z000000bm79EAA) su Workfront One.

## Colori basati sullo stato del progetto per gli elementi di lavoro nel bilanciamento del carico di lavoro

Per una migliore visibilità e una maggiore personalizzazione dell’esperienza nel servizio di bilanciamento del carico di lavoro, ora puoi modificare i colori dei progetti e dei relativi elementi di lavoro per adattarli allo stato del progetto. I colori corrispondono allo stato del progetto a livello di gruppo o di sistema. I colori visualizzati possono corrispondere sia allo stato del sistema che a quello del progetto personalizzato.

Per informazioni su come personalizzare la visualizzazione nel bilanciamento del carico di lavoro, vedi [Naviga nel bilanciamento del carico di lavoro](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Regolare l’allocazione degli utenti utilizzando i valori percentuali nel bilanciamento del carico di lavoro

Ora puoi gestire le allocazioni degli utenti nel servizio di bilanciamento del carico di lavoro utilizzando le percentuali invece che le ore.

Per informazioni sulla gestione delle allocazioni nel servizio di bilanciamento del carico di lavoro, vedi [Gestire le allocazioni di utenti nel load balancer](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## Mostra o nasconde il lavoro completato nel servizio di bilanciamento del carico di lavoro

Una nuova impostazione consente ora di mostrare o nascondere gli elementi di lavoro completati nel servizio di bilanciamento del carico di lavoro. L&#39;impostazione è abilitata per impostazione predefinita e gli elementi di lavoro completati che corrispondono ai criteri di filtro e all&#39;intervallo di tempo selezionato vengono visualizzati nel servizio di bilanciamento del carico di lavoro.

Prima di questo miglioramento, gli elementi di lavoro completati vengono sempre visualizzati nel servizio di bilanciamento del carico di lavoro.

Per ulteriori informazioni sulla regolazione delle impostazioni nel bilanciamento del carico di lavoro, vedi [Naviga nel bilanciamento del carico di lavoro](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Miglioramenti a livello di usabilità nel servizio di bilanciamento del carico di lavoro

Per garantire un’esperienza semplificata e semplice da usare quando gestisci le risorse nel workload Balancer, sono ora disponibili i seguenti miglioramenti a livello di usabilità:

* È ora possibile aprire il Riepilogo per i problemi e le attività dall&#39;icona Riepilogo anziché dal menu Altro. Questa esperienza è ora coerente con quella degli elenchi.

   >[!NOTE]
   >
   >Questa opzione è disponibile solo nella nuova esperienza Adobe Workfront.

* È possibile accedere al menu Altro a sinistra della barra degli oggetti anziché alla fine di una barra degli oggetti. Questo facilita la ricerca quando gli oggetti si estendono per un lungo periodo di tempo.
* È possibile accedere alle funzioni di assegnazione tramite una scelta rapida da tastiera. In precedenza, era disponibile solo dal menu Altro.
* È possibile caricare tutti gli elementi rimanenti sotto il nome di un utente invece dei 20 elementi seguenti facendo clic su Carica altro.

Per ulteriori informazioni sulla navigazione nel servizio di bilanciamento del carico di lavoro, consulta [Naviga nel bilanciamento del carico di lavoro](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Grafico di allocazione utente nel load balancer

Per consentire una rappresentazione visiva di alto livello dell’allocazione degli utenti in un determinato intervallo di tempo, una nuova impostazione ora consente una visualizzazione grafico della modalità di visualizzazione delle allocazioni nel load balancer. Se abiliti questa impostazione, l’allocazione degli utenti viene visualizzata in un grafico a linee che indica le sovrassegnazioni in blocchi rossi e le sottoallocazioni in blu.

Per ulteriori informazioni sulla configurazione delle impostazioni nel servizio di bilanciamento del carico di lavoro, vedi [Naviga nel bilanciamento del carico di lavoro](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Visualizza il lavoro completato nel servizio di bilanciamento del carico di lavoro

Per consentire di identificare facilmente il lavoro già completato in modo da poter gestire correttamente le assegnazioni utente, è stato abilitato un indicatore visivo nel servizio di bilanciamento del carico di lavoro che mostra quando sono stati completati gli elementi per un intervallo di tempo selezionato. È ora possibile visualizzare un segno di spunta verde per le attività, i problemi al termine del processo. Il progetto visualizza anche il segno di spunta verde quando sono presenti elementi di lavoro completati durante l’intervallo di tempo visualizzato sullo schermo.

Per informazioni sulla visualizzazione delle informazioni nel servizio di bilanciamento del carico di lavoro, vedi [Naviga nel bilanciamento del carico di lavoro](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Nuovo filtro predefinito per l&#39;area Lavoro assegnato nel bilanciamento del carico di lavoro

Il filtro Predefinito per l&#39;area Lavoro assegnato nel servizio di bilanciamento del carico di lavoro ora visualizza solo gli utenti membri di tutti i team a cui l&#39;utente connesso è associato. Per impostazione predefinita, il nuovo filtro ora visualizza le informazioni più rilevanti.

Prima di questo miglioramento, venivano visualizzati in quest’area tutti gli utenti a cui si aveva accesso per la visualizzazione.

Per informazioni sull&#39;utilizzo dei filtri nel load balancer, vedi [Gestire i filtri nel servizio di bilanciamento del carico di lavoro](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

## Nuova icona per passare da valori orari a valori percentuali o tempo allocato e rimanente nel servizio di bilanciamento del carico di lavoro

È stata aggiunta una nuova impostazione che consente di passare da Ore e Percentuali allocate quando si visualizza il servizio di bilanciamento del carico di lavoro. Con questa nuova icona, abbiamo eliminato anche la sezione User Workload nel pannello Impostazioni . Il servizio di bilanciamento del carico di lavoro mostra il tempo allocato per impostazione predefinita e abbiamo spostato l&#39;impostazione Ore rimanenti sulla nuova icona Percentuale o Ore.

Questo miglioramento elimina i clic e rende la navigazione del load Balancer più semplice ed efficiente.

Per informazioni sulla gestione delle impostazioni per il bilanciamento del carico di lavoro, vedi [Naviga nel bilanciamento del carico di lavoro](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Un nuovo filtro integrato per il load balancer: Utenti di progetti

Per rendere più efficiente l’esperienza di filtraggio nel servizio di bilanciamento del carico di lavoro, nell’area Lavoro assegnato è stato aggiunto un nuovo filtro incorporato. È ora possibile applicare il filtro Utenti su progetti per visualizzare gli utenti assegnati a attività e problemi nei progetti specificati.

Per informazioni sull&#39;utilizzo dei filtri nel load balancer, vedi [Filtrare le informazioni nel servizio di bilanciamento del carico di lavoro](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

