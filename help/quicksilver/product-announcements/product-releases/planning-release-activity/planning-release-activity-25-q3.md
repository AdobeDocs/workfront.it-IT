---
content-type: release-notes
title: Attività della versione del terzo trimestre 2025 per Adobe Workfront Planning
description: Questa è l’attività di rilascio per il prodotto Adobe Workfront Planning per il terzo trimestre 2025.
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
exl-id: 6761f5af-2501-4487-8114-2751f1e4fe69
source-git-commit: 686db6004d1a64279080ab3ba311c172a6a24d1f
workflow-type: tm+mt
source-wordcount: '1308'
ht-degree: 0%

---

# Attività della versione del terzo trimestre 2025 per Adobe Workfront Planning

Questo articolo descrive le funzioni rilasciate per Workfront Planning durante la versione del terzo trimestre 2025.

<!--keep the sentence below for all future quarterly release pages-->

Per un elenco di tutte le funzionalità rilasciate per Adobe Workfront Planning, vedere [Attività di rilascio di Adobe Workfront Planning: indice articolo](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).

## Filtri, colonne e campi aggiuntivi aggiunti alla scheda Pianificazione nell’area Richieste

>[!NOTE]
>
>* Anteprima: 29 maggio 2025
>* Versione rapida di produzione: 12 giugno 2025
>* Produzione per tutti i clienti: 17 luglio 2025

Sono state aggiunte le seguenti funzionalità a un elenco di richieste nella scheda Pianificazione dell’area Richieste:

* Nella colonna Inserito da è indicata la persona che ha aggiunto una richiesta
* Filtri per limitare il numero di richieste visualizzate nella scheda Pianificazione. Puoi filtrare l’elenco in base ai seguenti elementi:

   * Workspace da cui proviene il modulo di richiesta
   * tipo di record associato al modulo di richiesta
   * la data di ingresso della richiesta
   * il nome del modulo di richiesta
   * lo stato delle richieste
   * il nome della persona che ha inserito la richiesta.

* Le colonne consentono di visualizzare o nascondere i campi o le colonne dell&#39;elenco delle richieste di Planning.

Per informazioni, vedere [Inviare le richieste di Adobe Workfront Planning per la creazione di record](/help/quicksilver/planning/requests/submit-requests.md).

## Nuova esperienza nella suddivisione dei record in modalità Compatta nella visualizzazione timeline

>[!NOTE]
>
>* Anteprima: 22 maggio 2025
>* Versione rapida di produzione: 12 giugno 2025
>* Produzione per tutti i clienti: 17 luglio 2025

È stata modificata l’esperienza di suddivisione dei record nella visualizzazione timeline ed è stata applicata la visualizzazione Compatta.
Con il nuovo aggiornamento, quando si definiscono gli oggetti di suddivisione durante la visualizzazione della timeline in modalità Compatta, viene richiesto di passare alla visualizzazione Standard al termine della configurazione delle condizioni di suddivisione.

Prima di questo miglioramento, non era possibile definire le condizioni di raggruppamento durante la visualizzazione della timeline in modalità Compatta.

Con questo aggiornamento, l’opzione Standard è la scelta predefinita. In precedenza, la modalità Compatta era quella predefinita.

Per informazioni, vedere [Gestire la visualizzazione della sequenza temporale](/help/quicksilver/planning/views/manage-the-timeline-view.md).

## Aggiornare le impostazioni della vista timeline per definire l&#39;aspetto delle barre dei record collegati quando si utilizza l&#39;opzione Raggruppamento

>[!NOTE]
>
>* Anteprima: 15 maggio 2025
>* Versione rapida di produzione: 12 giugno 2025
>* Produzione per tutti i clienti: 17 luglio 2025

È ora possibile formattare l&#39;aspetto delle barre dei record nella visualizzazione timeline per i record del raggruppamento. È possibile aggiornare le seguenti impostazioni per le barre di questi record:

* Stile barra
* Colore

Prima di questo miglioramento, era possibile formattare solo le barre dei record principali così come vengono visualizzate nella visualizzazione timeline e non era possibile formattare le barre dei record collegati.\
 
Per informazioni, vedere [Gestire la visualizzazione della sequenza temporale](/help/quicksilver/planning/views/manage-the-timeline-view.md).  

## Esportare la vista tabella in un file CSV o Excel 

>[!NOTE]
>
>* Anteprima: 15 maggio 2025
>* Versione rapida di produzione: 12 giugno 2025
>* Produzione per tutti i clienti: 17 luglio 2025

È stata aggiunta una nuova funzionalità a Workfront Planning che consente di esportare le informazioni visibili nella vista a tabella in un file CSV o Excel.  

Quando esportate informazioni dalla vista tabella, tenete presente quanto segue:  

* Le informazioni esportate tengono conto dei filtri, dei raggruppamenti e degli ordinamenti applicati alla vista tabella in Workfront Planning.
* Le miniature e i colori di riga personalizzati non sono supportati nel file esportato.  
* Vengono esportati solo i campi resi visibili nell’interfaccia di Workfront. I campi nascosti non vengono esportati.  

Per ulteriori informazioni, vedere [Gestire la visualizzazione della tabella](/help/quicksilver/planning/views/manage-the-table-view.md). 

## I campi connessi di Workfront Planning sono ora supportati quando si importano record utilizzando un file CSV o Excel

>[!NOTE]
>
>* Anteprima: 15 maggio 2025
>* Versione rapida di produzione: 12 giugno 2025
>* Produzione per tutti i clienti: 17 luglio 2025

È ora possibile popolare i valori dei campi collegati quando si aggiungono record a un tipo di record utilizzando un file CSV o Excel.  Sono supportati solo i campi dei record di Planning connessi. I campi che visualizzano connessioni ad altre applicazioni non sono supportati.

Questa modifica è supportata quando si importa un file CSV ed Excel per creare sia un tipo di record che record per un tipo di record esistente.

Prima di questo miglioramento, non era possibile compilare i campi di connessione al momento dell’importazione dei record.

Per informazioni, vedere i seguenti articoli:

* [Creare record importando informazioni da un file CSV o Excel](/help/quicksilver/planning/records/import-file-to-create-records.md).

* [Creare tipi di record importando informazioni da un file CSV o Excel](/help/quicksilver/planning/architecture/import-file-to-create-record-types.md).

## Modifica in linea nella pagina Record connessi di un record

>[!NOTE]
>
>* Anteprima: 30 aprile 2025
>* Versione rapida di produzione: 15 maggio 2025
>* Produzione per tutti i clienti: 17 luglio 2025

È ora possibile modificare i record nella pagina Record collegati di un record. Con questo aggiornamento, abbiamo introdotto quanto segue:

* Il nome della pagina è stato modificato da &quot;Visualizzazione connessione&quot; a &quot;Pagina record connessi&quot;.
* I record collegati visualizzati in questa pagina sono modificabili in linea nella vista a tabella. Gli oggetti Workfront connessi continuano a essere visualizzati in una tabella di sola lettura.

Prima di questo miglioramento, la tabella della pagina di visualizzazione Connessione era di sola lettura per le connessioni record.

Per informazioni, vedere [Gestire il layout della pagina record](/help/quicksilver/planning/records/manage-the-record-page.md).

## Area di pianificazione visibile per impostazione predefinita nel menu principale per gli utenti con licenza Standard

>[!NOTE]
>
>* Anteprima: 30 aprile 2025
>* Versione rapida di produzione: 15 maggio 2025
>* Produzione per tutti i clienti: 17 luglio 2025

Gli utenti Standard e System Administrator possono ora trovare l&#39;area Planning nel menu principale per impostazione predefinita, senza essere assegnati a un modello di layout che lo include. Tutti gli altri utenti devono disporre di un modello di layout che includa l&#39;area Planning loro assegnata per poter accedere ad essa.

Prima di questo miglioramento, gli utenti con tutti i livelli di licenza dovevano essere assegnati al modello di layout modificato per includere l’area Planning nel menu principale per accedere a quest’area.

>[!NOTE]
>
>Questa modifica sarà visibile per tutti gli utenti nuovi ed esistenti con una licenza Amministratore di sistema e Standard.
>&#x200B;>Gli utenti esistenti assegnati a un modello di layout continueranno a visualizzare tutto in base alle impostazioni definite nel modello di layout.

Per informazioni, vedere [Panoramica di Adobe Workfront Planning](/help/quicksilver/planning/access/access-overview.md).

## Formattazione del colore a livello di riga nella vista tabella

>[!NOTE]
>
>* Anteprima: 30 aprile 2025
>* Versione rapida di produzione: 15 maggio 2025
>* Produzione per tutti i clienti: 17 luglio 2025

Per una migliore visibilità delle informazioni importanti dei record, è stata introdotta la formattazione del colore a livello di riga per la visualizzazione per tabella. È ora possibile scegliere un colore per ogni riga dopo aver definito le condizioni per ciascuna scelta.  Questa è una nuova funzionalità che non esisteva prima di questo aggiornamento.

Per informazioni, vedere [Gestire la visualizzazione della tabella](/help/quicksilver/planning/views/manage-the-table-view.md).

## Nuova impostazione per troncare i nomi dei record lunghi nella vista Timeline standard

>[!NOTE]
>
>* Anteprima: 23 aprile 2025
>* Versione rapida di produzione: 15 maggio 2025
>* Produzione per tutti i clienti: 17 luglio 2025

È ora possibile attivare un&#39;impostazione nella scheda Stile barra della casella Impostazioni di una visualizzazione timeline per troncare i nomi dei record più lunghi quando vengono visualizzati nella visualizzazione Standard. L&#39;impostazione è disattivata per impostazione predefinita e può essere attivata solo quando si visualizza la vista timeline in modalità Standard. Poiché questa impostazione è disabilitata, per impostazione predefinita le informazioni sulle barre dei record vengono visualizzate espanse. Prima di questo miglioramento, le informazioni sulle barre dei record venivano troncate per impostazione predefinita.

Per informazioni, vedere [Gestire la visualizzazione della sequenza temporale](/help/quicksilver/planning/views/manage-the-timeline-view.md).

## Autorizzazioni di condivisione per i tipi di record


>[!NOTE]
>
>* Anteprima: 17 aprile 2025
>* Versione rapida di produzione: 12 giugno 2025
>* Produzione per tutti i clienti: 17 luglio 2025

Per controllare meglio chi può visualizzare o gestire i record in ogni tipo di record e garantire che solo le persone autorizzate possano gestire le informazioni di ogni tipo di record in base ai loro ruoli e responsabilità, sono state introdotte le autorizzazioni a livello di tipo di record.

Prima di questo miglioramento, era possibile condividere solo le aree di lavoro con altri utenti e l’autorizzazione concessa a un’area di lavoro veniva applicata a tutti i tipi di record nell’area di lavoro.

Sono stati introdotti i seguenti aggiornamenti:

* Le autorizzazioni di Workspace vengono condivise automaticamente con tutti i tipi di record nell’area di lavoro.
* Il livello di autorizzazioni concesse per l&#39;area di lavoro viene visualizzato come Autorizzazioni ereditate per il tipo di record.
* Non è possibile condividere un tipo di record con un livello di autorizzazione superiore a quello degli utenti nell&#39;area di lavoro.
* È possibile disabilitare le autorizzazioni ereditate sul tipo di record per renderlo di sola lettura per tutte le persone nell&#39;area di lavoro. Successivamente, è possibile aggiungere singoli utenti, team, gruppi, società o ruoli e concedere loro l&#39;autorizzazione Contribuisci al tipo di record.

Per ulteriori informazioni, vedere [Condividi tipi di record](/help/quicksilver/planning/access/share-record-types.md).


