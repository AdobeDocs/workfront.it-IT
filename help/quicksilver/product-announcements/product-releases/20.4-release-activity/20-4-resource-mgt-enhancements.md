---
title: 20.4 Miglioramenti alla gestione delle risorse
description: 20.4 Miglioramenti alla gestione delle risorse
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 9f660a38-4a59-4135-8178-0841088cc7d6
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '1042'
ht-degree: 0%

---

# 20.4 Miglioramenti alla gestione delle risorse

Questa pagina descrive tutti i miglioramenti alla gestione delle risorse apportati con la versione 20.4 all’ambiente di anteprima. Questi miglioramenti saranno resi disponibili nell’ambiente di produzione nella settimana del 9 novembre 2020.

Per un elenco di tutte le modifiche disponibili con la versione 20.4, consulta la [panoramica sulla versione 20.4](../../../product-announcements/product-releases/20.4-release-activity/20-4-release-overview.md).

## Pianificare il lavoro utilizzando l&#39;Impegno di lavoro invece delle Ore pianificate

Per offrire flessibilità nella pianificazione del lavoro sui progetti, è stato introdotto il nuovo concetto di Impegno di lavoro per le attività. È possibile stimare se l&#39;Impegno di lavoro per un&#39;attività è piccolo, medio o grande senza stimare manualmente le ore pianificate per l&#39;attività. Ogni livello di impegno viene calcolato in base a una percentuale di tempo dalle ore giornaliere tipiche configurate nell’istanza.

Con questa nuova funzione sono ora disponibili i seguenti miglioramenti:

* Abilita questa impostazione per progetti e modelli per renderla disponibile per le attività e i modelli
* Aggiorna questa impostazione per ogni attività con un tipo di durata semplice che aggiorna automaticamente le ore pianificate dell&#39;attività
* Disattiva questa impostazione utilizzando un modello di layout per gli utenti che preferiscono continuare a utilizzare le ore pianificate.
* Visualizza il valore di questo nuovo campo in un elenco di attività o in un report.

Per informazioni sull&#39;impegno di lavoro, vedere [Panoramica sull&#39;impegno di lavoro](../../../manage-work/tasks/task-information/work-effort.md).

Questa funzionalità è ora inclusa in [Planner Fundamentals, Part 2 learning path](https://experienceleague.adobe.com/en/docs/workfront/using/home) su Workfront One.

## Colori basati sullo stato del progetto per gli elementi di lavoro nel Bilanciatore dei carichi di lavoro

Per una migliore visibilità e una maggiore personalizzazione dell’esperienza nel Bilanciatore dei carichi di lavoro, ora puoi modificare i colori dei progetti e dei relativi elementi di lavoro in modo che corrispondano allo stato dei progetti. I colori corrispondono agli stati del progetto a livello di gruppo o di sistema. I colori visualizzati possono corrispondere sia allo stato del progetto di sistema che a quello personalizzato.

Per informazioni sulla personalizzazione della visualizzazione nel Bilanciatore dei carichi di lavoro, vedere [Navigare nel Bilanciatore dei carichi di lavoro](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Regolare l’allocazione degli utenti utilizzando i valori percentuali nel Bilanciatore dei carichi di lavoro

Ora puoi gestire le allocazioni degli utenti nel Bilanciatore dei carichi di lavoro utilizzando le percentuali anziché le ore.

Per informazioni sulla gestione delle allocazioni nel Bilanciatore dei carichi di lavoro, vedere [Gestione delle allocazioni utente nel Bilanciatore dei carichi di lavoro](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## Mostrare o nascondere il lavoro completato nel Bilanciatore dei carichi di lavoro

Una nuova impostazione ora consente di mostrare o nascondere gli elementi di lavoro completati nel Bilanciatore dei carichi di lavoro. L’impostazione è abilitata per impostazione predefinita e per gli elementi di lavoro completati che corrispondono ai criteri di filtro e all’intervallo di tempo selezionato, vengono visualizzati nel Bilanciatore dei carichi di lavoro.

Prima di questo miglioramento, gli elementi di lavoro completati venivano sempre visualizzati nel Bilanciatore dei carichi di lavoro.

Per ulteriori informazioni sulla regolazione delle impostazioni nel Bilanciatore dei carichi di lavoro, vedi [Navigare nel Bilanciatore dei carichi di lavoro](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Miglioramenti a livello di usabilità nel Bilanciatore dei carichi di lavoro

Per garantire un’esperienza semplificata e di facile utilizzo quando gestisci le risorse nel Bilanciatore dei carichi di lavoro, sono ora disponibili i seguenti miglioramenti a livello di usabilità:

* Ora puoi aprire il Riepilogo per problemi e attività dall’icona Riepilogo invece che dal menu Altro. Questa esperienza è ora coerente con quella degli elenchi.

  >[!NOTE]
  >
  >Questa opzione è disponibile solo nella nuova esperienza Adobe Workfront.

* È possibile accedere al menu Altro a sinistra della barra degli oggetti anziché alla fine della barra degli oggetti. In questo modo è più facile trovare gli oggetti che durano per un lungo periodo di tempo.
* È possibile accedere alle funzioni di assegnazione con una scelta rapida da tastiera. In precedenza, era disponibile solo dal menu Altro.
* È possibile caricare tutti gli elementi rimanenti con il nome di un utente invece dei 20 elementi seguenti facendo clic su Carica altro.

Per ulteriori informazioni sulla navigazione nel Bilanciatore dei carichi di lavoro, vedere [Navigare nel Bilanciatore dei carichi di lavoro](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Grafico di allocazione utente nel Bilanciatore dei carichi di lavoro

Per consentire una rappresentazione visiva di alto livello dell’allocazione degli utenti in un determinato intervallo di tempo, una nuova impostazione ora abilita una visualizzazione grafico per la modalità di visualizzazione delle allocazioni nel Bilanciatore dei carichi di lavoro. Abilitando questa impostazione, l&#39;allocazione degli utenti viene visualizzata in un grafico a linee che indica le sovrassegnazioni in blocchi di colore rosso e le sottoallocazioni in blu.

Per ulteriori informazioni sulla configurazione delle impostazioni nel Bilanciatore dei carichi di lavoro, vedere [Navigare nel Bilanciatore dei carichi di lavoro](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Visualizzare il lavoro completato nel Bilanciatore dei carichi di lavoro

Per consentire di identificare facilmente il lavoro già completato e gestire correttamente le assegnazioni degli utenti, è stato attivato un indicatore visivo nel Bilanciatore dei carichi di lavoro che mostra quando gli elementi di un intervallo di tempo selezionato sono stati completati. È ora possibile visualizzare un segno di spunta verde per le attività, i problemi quando vengono completati. Il progetto visualizza inoltre il segno di spunta verde quando sullo schermo sono visualizzati elementi di lavoro completati durante l&#39;intervallo di tempo.

Per informazioni sulla visualizzazione delle informazioni nel Bilanciatore dei carichi di lavoro, vedere [Navigare nel Bilanciatore dei carichi di lavoro](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Nuovo filtro predefinito per l’area Lavoro assegnato nel Bilanciatore dei carichi di lavoro

Il filtro Predefinito per l’area Lavoro assegnato nel Bilanciatore dei carichi di lavoro ora visualizza solo gli utenti membri di tutti i team a cui sei associato come utente connesso. Il nuovo filtro visualizza ora le informazioni più rilevanti, per impostazione predefinita.

Prima di questo miglioramento, in quest’area venivano visualizzati tutti gli utenti a cui avevi accesso.

Per informazioni sull&#39;utilizzo dei filtri nel Bilanciatore dei carichi di lavoro, vedere [Gestione dei filtri nel Bilanciatore dei carichi di lavoro](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

## Nuova icona per passare da valori di ore a valori di percentuale o tempo allocato e rimanente nel Bilanciatore dei carichi di lavoro

È stata aggiunta una nuova impostazione che consente di passare da un’ora all’altra e viceversa, mentre si visualizza il Bilanciatore dei carichi di lavoro. Con questa nuova icona, è stata eliminata anche la sezione Carico di lavoro utente nel pannello Impostazioni. Il Bilanciatore dei carichi di lavoro mostra il tempo allocato per impostazione predefinita e l’impostazione Ore rimanenti è stata spostata sulla nuova icona Percentuale o Ore.

Questo miglioramento elimina i clic e rende più semplice ed efficiente la navigazione nel Bilanciatore dei carichi di lavoro.

Per informazioni sulla gestione delle impostazioni per il Bilanciatore dei carichi di lavoro, vedere [Navigare nel Bilanciatore dei carichi di lavoro](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Un nuovo filtro integrato per il Bilanciatore dei carichi di lavoro: Utenti sui progetti

Per rendere più efficiente l’esperienza di filtro nel Bilanciatore dei carichi di lavoro, è stato aggiunto un nuovo filtro integrato nell’area Lavoro assegnato. Ora puoi applicare il filtro Utenti su progetti, che mostra gli utenti assegnati alle attività e ai problemi nei progetti specificati.

Per informazioni sull&#39;utilizzo dei filtri nel Bilanciatore dei carichi di lavoro, vedere [Informazioni sui filtri nel Bilanciatore dei carichi di lavoro](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

