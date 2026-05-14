---
product-area: documents
navigation-topic: approvals
title: Aggiornare gli scenari di Workfront Fusion per la revisione e l’approvazione unificate
description: Inventariare, classificare e correggere gli scenari Workfront Fusion basati su Workfront Proofing legacy mentre l'organizzazione adotta lo storage aziendale Adobe e la revisione e l'approvazione unificate.
author: Courtney
feature: Work Management, Digital Content and Documents
role: Admin
source-git-commit: 0a635f80338cef38dec7d32391596ca9ccd2fd6c
workflow-type: tm+mt
source-wordcount: '804'
ht-degree: 1%

---

# Aggiornare gli scenari di Workfront Fusion per la revisione e l’approvazione unificate

Gli scenari Workfront Fusion basati su versioni precedenti di Workfront Proofing non funzionano automaticamente con i progetti di storage aziendale Adobe. I moduli specifici della bozza, i webhook e gli endpoint API hanno equivalenti diretti in alcuni casi e cambiamenti significativi in altri. Questo articolo consente di inventariare gli scenari interessati, classificarli e decidere un percorso di correzione prima di inserire i team che dipendono da tali scenari nel rollout dello storage aziendale Adobe.

Gli scenari con ambito di progetti Workfront legacy continuano a funzionare come fanno attualmente. Il lavoro di correzione descritto in questo articolo si applica agli scenari che si intende eseguire sui progetti di storage aziendale Adobe.

I connettori di fusione con supporto nativo per revisione e approvazione unificate saranno disponibili nel terzo trimestre del 2026. Pianifica la ricostruzione ora, ma consigliamo di attendere i nuovi connettori prima di generare. Gli scenari saranno più semplici e affidabili di quelli che sostituiranno.

Linee guida dettagliate sull’automazione saranno pubblicate insieme alla versione del connettore Fusion Q3 2026. Utilizza questo articolo per fare l’inventario e classificare gli scenari ora in modo da essere pronti ad agire una volta che la guida sarà disponibile.

Per un riepilogo di alto livello delle modifiche apportate al passaggio dell&#39;organizzazione a Workfront su Adobe Enterprise Storage, vedere [Passare a Workfront su Adobe Enterprise Storage](/help/quicksilver/review-and-approve-work/workfront-storage.md).


## Quali sono le modifiche per Fusion sui progetti di storage aziendale Adobe

Gli scenari Fusion esistenti basati su Workfront Proof si basano su moduli specifici per le bozze, trigger di webhook ed endpoint API che non fanno parte del modello dati unificato di revisione e approvazione. La tabella seguente mappa i tipi di scenario comuni in base all’impatto previsto e al percorso futuro:

| Tipo di scenario | Impatto | Percorso in avanti |
|---|---|---|
| Creazione e instradamento delle bozze | Interruzioni | Rigenera utilizzando l’API di approvazione unificata nel terzo trimestre del 2026 |
| Webhook sullo stato della bozza | Interruzioni | Ricostruisci con nuovi trigger di evento di approvazione nel terzo trimestre 2026 |
| Trigger di caricamento documento | Parziale: è necessario ripetere il test | Audit e nuovo test dopo la migrazione nel terzo trimestre 2026 |
| Notifiche promemoria approvazione | Interruzioni | Sostituisci con scadenze modello di approvazione |
| Indirizzamento delle decisioni di approvazione | Interruzioni | Rigenera utilizzando i nuovi campi di stato delle decisioni |
| Rapporti di approvazione personalizzati | Parziale: i nomi dei campi possono cambiare | Mappa i campi legacy al nuovo schema |


## Classificare ogni scenario come Modifica, Ricostruisci o Ritira

Il lavoro che ogni scenario richiede dipende da ciò che fa e da ciò che è disponibile nella revisione e nell&#39;approvazione unificate. Utilizza le seguenti classificazioni:

* **Modifica**: l&#39;azione esistente relativa alla bozza ha un equivalente diretto in revisione e approvazione unificate ed è possibile aggiornare lo scenario per utilizzare la nuova azione.
* **Ricostruisci**: i passaggi sottostanti sono cambiati in modo significativo oppure sono presenti nuove funzionalità che lo scenario deve utilizzare, pertanto è necessario ricrearlo da zero.
* **Ritira**: la funzionalità di revisione e approvazione unificata nativa, ad esempio i modelli di approvazione in più fasi con promemoria di scadenza, sostituisce lo scenario creato per l&#39;esecuzione.

Esamina ogni scenario in base alla tua logica di business specifica per deciderne la classificazione.

## Approccio di risoluzione

Per pianificare ed eseguire la correzione di Fusion, utilizzare il seguente approccio:

1. **Inventario ora.** Recupera un elenco completo degli scenari di Fusion attivi e assegna i tag a tutti quelli che fanno riferimento alla creazione di bozze, allo stato della bozza, alle approvazioni di documenti o al routing di approvazione. Non attendere l&#39;attivazione dello storage aziendale Adobe.
1. **Classifica ogni scenario** come Modifica, Ricompila o Ritira in base ai criteri della sezione precedente.
1. **Sospendi gli scenari dipendenti dalla bozza** prima di inserire nel programma pilota per lo storage aziendale di Adobe i team che dipendono da essi. L’esecuzione di automazioni basate su bozze obsolete rispetto al nuovo modello può causare errori invisibili all’utente o azioni duplicate.
1. **Utilizzare i modelli di approvazione per sostituire la logica di routing semplice.** I modelli di approvazione nativi in più fasi con automazione delle scadenze possono gestire molti casi d’uso che in precedenza richiedevano Fusion. Per ulteriori informazioni, consulta [Creare un modello di approvazione per risorse e documenti](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).
1. **Attendere gli aggiornamenti del connettore Fusion per il terzo trimestre 2026 prima di ricompilare.** I connettori aggiornati espongono i moduli progettati appositamente per la revisione e l’approvazione unificate e rendono le ricostruzioni notevolmente più semplici e affidabili. Si sconsiglia di ricostruire a fronte della versione 22 dell’API di Workfront in anticipo. Se procedi per uno scenario critico dal punto di vista temporale, pianifica di rivedere tale lavoro una volta rilasciati i nuovi connettori.
1. **Verifica gli scenari ricostruiti end-to-end in un&#39;istanza sandbox** prima di abilitarli in produzione. Presta particolare attenzione ai payload di abbonamento agli eventi; i nomi dei campi e lo schema sono diversi dagli eventi di bozza precedenti.

>[!TIP]
>
>Molte organizzazioni hanno accumulato scenari di Fusion che sono stati una soluzione alternativa per le lacune nelle prove legacy. Le funzioni di revisione e approvazione unificate native, tra cui modelli di approvazione, promemoria di scadenza e instradamento in più fasi, eliminano completamente la necessità di alcuni di questi scenari. Quando classifichi ogni scenario, valuta se una funzione nativa può sostituirla. Ritirare uno scenario è spesso un risultato a lungo termine più pulito rispetto alla sua ricostruzione.

## Articoli correlati

* [Passare a Workfront sullo storage aziendale Adobe](/help/quicksilver/review-and-approve-work/workfront-storage.md)
* [Panoramica sulla revisione e sull’approvazione unificata](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)
* [Introduzione a revisione e approvazione unificate](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)
* [Creare un modello di approvazione per risorse e documenti](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)
