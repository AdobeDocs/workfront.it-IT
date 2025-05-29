---
title: Miglioramenti al progetto del terzo trimestre 2025
description: Miglioramenti al progetto del terzo trimestre 2025
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
hide: true
hidefromtoc: true
exl-id: 33fa5a61-5300-402c-9f80-f2701f7999a8
source-git-commit: a5a61045bad5a97fb1413fac4a5a2666b753fa83
workflow-type: tm+mt
source-wordcount: '488'
ht-degree: 0%

---

# Miglioramenti al progetto del terzo trimestre 2025

Questa pagina descrive i miglioramenti apportati all’ambiente di anteprima con la versione del terzo trimestre 2025. Questi miglioramenti saranno resi disponibili nell’ambiente di produzione come indicato.

Per un elenco di tutte le modifiche disponibili al momento nel ciclo di rilascio del terzo trimestre 2025, consulta [Panoramica sulla versione del terzo trimestre 2025](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-release-overview.md).

## Modifica della modalità di memorizzazione delle ore effettive nel database per le chiamate API

>[!NOTE]
>
>* Anteprima: 27 maggio 2025
>* Versione rapida di produzione: 27 maggio 2025
>* Produzione per tutti i clienti: 27 maggio 2025

Questo aggiornamento introduce una modifica nel modo in cui le ore effettive per progetti, attività e problemi vengono memorizzate nel database. A partire da questo aggiornamento, le ore effettive utilizzeranno un valore di `actualWorkRequiredDouble` (con un valore in ore).

Prima di questo aggiornamento, le ore effettive erano memorizzate con un valore di `actualWorkRequired` (con un valore in minuti). Questo aggiornamento garantirà un conteggio più accurato delle ore effettive quando vengono calcolate utilizzando una chiamata API.

A causa di questa modifica, potrebbe essere necessario aggiornare eventuali chiamate API che fanno riferimento al campo del valore originale. Non apportare modifiche se si utilizza un valuefield di `actualWorkRequiredExpression` nelle chiamate API.

Questo aggiornamento non modifica i calcoli delle ore effettive per progetti, attività e problemi nelle colonne dei campi personalizzati calcolati.

## Aggiornamento in utilizzando il cursore Percentuale di completamento nell’intestazione di un’attività o di un problema

>[!NOTE]
>
>* Anteprima: 27 maggio 2025
>* Versione rapida di produzione: 27 maggio 2025
>* Produzione per tutti i clienti: 27 maggio 2025

Abbiamo aggiornato il funzionamento del cursore della percentuale di completamento per le attività e i problemi.

Sono ora disponibili le seguenti funzionalità:

* Quando fai scorrere la bolla blu &quot;Percentuale di completamento&quot; nell’intestazione di un’attività o di un problema, la percentuale di completamento dell’attività o del problema viene ora aggiornata con incrementi di cinque punti. Prima di questo aggiornamento, facendo scorrere la bolla blu Percentuale di completamento, le attività o i problemi venivano aggiornati con incrementi di un punto.

* Puoi fare doppio clic sulla bolla blu e aggiornarla manualmente con qualsiasi numero desiderato senza utilizzare il cursore. Questa funzionalità non è stata modificata.

Non sono state introdotte altre modifiche per aggiornare la percentuale di completamento di attività e problemi in altre aree di Workfront.

Per informazioni, vedere [Visualizzare e aggiornare la percentuale di completamento per le attività](/help/quicksilver/manage-work/projects/updating-work-in-a-project/view-update-percent-complete-for-tasks.md).

## Maggiore trasparenza nell’utilizzo dell’Assistente IA per progetti, attività e problemi

>[!NOTE]
>
>* Anteprima: 19 maggio 2025
>* Versione rapida di produzione: 19 maggio 2025
>* Produzione per tutti i clienti: 19 maggio 2025

Per chiarire in che modo l’Assistente per l’intelligenza artificiale individua le risposte a domande su progetti, attività e problemi di Workfront, abbiamo aggiunto queste informazioni alla risposta alla domanda. Ora, l’Assistente AI include le informazioni di ricerca nell’output. Puoi utilizzare queste informazioni per verificare che l’Assistente AI abbia identificato correttamente la domanda che ti stai ponendo e per comprendere il contesto della risposta.

In precedenza, queste informazioni non erano disponibili nella risposta dell’Assistente IA.

Per informazioni sull&#39;utilizzo dell&#39;Assistente IA per ottenere informazioni sugli elementi di Workfront, vedere [Utilizzare l&#39;Assistente IA per lavorare con progetti, attività e problemi](/help/quicksilver/workfront-basics/ai-assistant/work-with-pti-through-ai-assisant.md).
