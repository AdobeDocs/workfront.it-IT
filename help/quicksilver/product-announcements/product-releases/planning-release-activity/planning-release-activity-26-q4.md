---
content-type: release-notes
title: Attività della versione del quarto trimestre 2026 per Adobe Workfront Planning
description: Questa è l’attività di rilascio per il prodotto Adobe Workfront Planning per il quarto trimestre del 2026.
author: Becky
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: 3f0a939e9de6436117fcb8242449793dcef73205
workflow-type: tm+mt
source-wordcount: '1770'
ht-degree: 1%

---

# Attività della versione del quarto trimestre 2026 per Adobe Workfront Planning

Questo articolo descrive le funzioni rilasciate per Workfront Planning durante la versione del quarto trimestre 2026.

Per un elenco di tutte le funzionalità rilasciate per Adobe Workfront Planning, vedere [Attività di rilascio di Adobe Workfront Planning: indice articolo](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).

## Consente di gestire la visibilità delle miniature e dei colori dei record dalla colonna del campo principale nella vista tabella

>[!NOTE]
>
>Anteprima: 3 settembre 2026
>Versione rapida di produzione: 17 settembre 2026
>Produzione per tutti: 15 ottobre 2026

È ora possibile gestire la visibilità delle miniature e dei colori dei record durante la modifica della colonna del campo principale nella vista tabella.

Con questo aggiornamento, le impostazioni Miniatura e Colore verranno rimosse dall&#39;icona Campi nella barra degli strumenti della vista tabella.

Per informazioni, vedere [Gestire la visualizzazione della tabella](/help/quicksilver/planning/views/manage-the-table-view.md).

## Creare regole business per i tipi di record

>[!NOTE]
>
>Anteprima: 3 settembre 2026
>Versione rapida di produzione: 17 settembre 2026
>Produzione per tutti: 15 ottobre 2026

In qualità di responsabile dell&#39;area di lavoro, è ora possibile impostare regole business per i tipi di record che in seguito rifletteranno sulla gestione dei record di quel tipo. È possibile definire regole che consentono agli utenti di modificare o eliminare record solo quando vengono soddisfatte determinate condizioni o quando vengono compilati determinati campi.

È possibile creare una condizione per la regola business che faccia riferimento a tutti i tipi di campo ad eccezione dei seguenti:

* Campi formula
* Campi di ricerca
* Campi di riferimento

Non è possibile aggiungere regole business ai tipi di record globali.

Per ulteriori informazioni, vedere [Configurare le regole business dei tipi di record](/help/quicksilver/planning/architecture/configure-business-rules.md).

>[!NOTE]
>
>Con questo aggiornamento, sono state aggiornate anche le seguenti opzioni di menu nel menu Altro di un tipo di record:
>
>* **Crea moduli di richiesta** e **Gestisci moduli di richiesta** è stato modificato in **Moduli di richiesta**
>* **Gestione automazioni** è stato modificato in **Automazioni**

## Introduzione di settimane personalizzate per la visualizzazione timeline

>[!NOTE]
>
>Anteprima: 3 settembre 2026
>Versione rapida di produzione: 17 settembre 2026
>Produzione per tutti: 15 ottobre 2026

In qualità di amministratore di Workfront, ora puoi configurare settimane personalizzate, oltre ai trimestri personalizzati. Le settimane e i trimestri personalizzati sono visibili dalla vista timeline di Workfront Planning. Workfront genera settimane sequenziali a partire dalla Settimana 1 all’inizio del Trimestre personalizzato 1.

È possibile personalizzare le etichette delle settimane visibili nella visualizzazione timeline. È possibile scegliere un formato predefinito o immetterne uno personalizzato.

Le settimane personalizzate non sono visibili in Workfront. Sono visibili solo nella vista timeline di Workfront Planning.

Per informazioni, vedere [Abilitare i trimestri personalizzati](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md).

## Filtri per i campi record collegati dipendenti

>[!NOTE]
>
>Anteprima: 3 settembre 2026
>Versione rapida di produzione: 17 settembre 2026
>Produzione per tutti: 15 ottobre 2026

È ora possibile filtrare determinati tipi di record che soddisfano un criterio di filtro quando si aggiungono connessioni dipendenti in Planning.

Anziché tutti i tipi di record disponibili nei campi collegati dipendenti, verranno visualizzati solo quelli che soddisfano i criteri di filtro specificati.

Per questa funzione è stata aggiunta una nuova opzione Regole filtro record nella scheda Nuova connessione durante la connessione di tipi di record.

Per informazioni, vedere [Gestire le connessioni dipendenti](/help/quicksilver/planning/architecture/manage-dependent-connections.md).

## Comprimi ed espandi tutti i raggruppamenti nella vista timeline

>[!NOTE]
>
>Anteprima: 27 agosto 2026
>Versione rapida di produzione: 17 settembre 2026
>Produzione per tutti: 15 ottobre 2026

Le viste Timeline ora includono Comprimi tutto ed Espandi tutte le opzioni per le timeline raggruppate. In questo modo è più semplice spostarsi tra le viste della roadmap di grandi dimensioni: è possibile ridurre rapidamente la vista raggruppando le intestazioni, quindi espandere solo le sezioni che si desidera esaminare.

Per ulteriori informazioni, vedere [Gestire la visualizzazione della sequenza temporale](/help/quicksilver/planning/views/manage-the-timeline-view.md).

## Visualizzare i nomi dei gruppi completi e ridimensionare il pannello di raggruppamento nella vista Timeline

>[!NOTE]
>
>Anteprima: 27 agosto 2026
>Versione rapida di produzione: 17 settembre 2026
>Produzione per tutti: 15 ottobre 2026

Nella vista timeline, passando il cursore su un&#39;etichetta di gruppo troncata, ora viene visualizzato il testo completo in una descrizione comando, sia nella visualizzazione Corsia che in quella Raggruppamento in pila. Le etichette non troncate non mostrano descrizioni comandi.

Il pannello di raggruppamento a sinistra nella visualizzazione Corsia può essere ridimensionato trascinandone il divisore. La vista viene aggiornata in tempo reale, in linea con la vista tabella. La larghezza del pannello di ogni utente viene salvata nelle sessioni, con una larghezza predefinita per i nuovi utenti.

Per informazioni, consulta [Gestire la vista timeline](/help/quicksilver/planning/views/manage-the-timeline-view.md).

## Sono state migliorate le prestazioni del calendario per set di record di grandi dimensioni nella visualizzazione settimana

>[!NOTE]
>
>Anteprima: 27 agosto 2026
>Versione rapida di produzione: 17 settembre 2026
>Produzione per tutti: 15 ottobre 2026

Nella visualizzazione per settimana del calendario vengono ora visualizzati solo i primi 1.000 record del periodo di settimana visibile. Se sono presenti più record, nella parte inferiore del calendario viene visualizzato il seguente messaggio che indica che sono disponibili record aggiuntivi: &quot;Sono presenti più record. Carica di più.&quot;

Per informazioni, vedere [Gestire la visualizzazione del calendario](/help/quicksilver/planning/views/manage-the-calendar-view.md).

## Intestazioni di colonna aggiornate per i campi record collegati dipendenti

>[!NOTE]
>
>Anteprima: 20 agosto 2026
>Versione rapida di produzione: 17 settembre 2026
>Produzione per tutti: 15 ottobre 2026

Sono stati apportati miglioramenti visivi alle intestazioni di colonna per un campo record connesso dipendente nella visualizzazione per tabella.

Per informazioni, vedere [Gestire le connessioni dipendenti](/help/quicksilver/planning/architecture/manage-dependent-connections.md).

## Miglioramenti alla vista tabella quando si trascinano e rilasciano più righe

>[!NOTE]
>
>Anteprima: 13 agosto 2026
>Versione rapida di produzione: 13 agosto 2026
>Produzione per tutti: 15 ottobre 2026
>[!BADGE Fuori pianificazione]{type=Neutral}

Sono disponibili nuovi indicatori visivi quando si trascinano e rilasciano più righe nella vista tabella. Un segno più e un indicatore numerico più evidenti ora mostrano quante righe sono selezionate per l’azione di trascinamento della selezione.

Per informazioni, vedere [Gestire la visualizzazione della tabella](/help/quicksilver/planning/views/manage-the-table-view.md).

## Indirizza l&#39;oggetto richiesta inviato all&#39;area di lavoro corretta quando si utilizzano i tipi di record globali

>[!NOTE]
>
>Anteprima: 13 agosto 2026
>Versione rapida di produzione: 17 settembre 2026
>Produzione per tutti: 15 ottobre 2026

I record creati per i tipi di record globali mediante l&#39;invio di un modulo di richiesta vengono ora instradati automaticamente all&#39;area di lavoro da cui sono stati inviati.

I record creati inviando una richiesta da un&#39;area di lavoro secondaria di un tipo di record globale vengono aggiunti a tale area di lavoro secondaria. I record creati inviando una richiesta dall’area di lavoro originale o dall’area Richieste principale vengono aggiunti all’area di lavoro originale.

Se il modulo di assegnazione include un campo Workspace e l’utente seleziona un’area di lavoro prima dell’invio, la richiesta viene indirizzata all’area di lavoro selezionata indipendentemente da dove è stato avviato il modulo. In questo modo i record verranno organizzati nell&#39;area di lavoro desiderata dal momento della creazione.

Per informazioni, vedere [Inviare le richieste di Adobe Workfront Planning per la creazione di record](/help/quicksilver/planning/requests/submit-requests.md).

## Presentazione delle competenze di Workfront Planning Solution Architect

>[!NOTE]
>
>Anteprima: 10 agosto 2026
>Produzione: 10 agosto 2026

Stiamo rilasciando una nuova competenza, Workfront Planning Solution Architect, che porta a Claude una guida agentica e basata su best practice per Workfront Planning:

* **Configurare** nuove aree di lavoro di Planning da specificare, con il server Workfront MCP che esegue l&#39;installazione nell&#39;ambiente.
* **Controlla** le configurazioni esistenti per gli antipasti su larga scala.
* **Controllare l&#39;utilizzo** in base ai limiti consigliati (record, connessioni, profondità gerarchia).
* **Fai domande** su Planning in qualsiasi momento.

Oltre alla configurazione iniziale, l’abilità supporta la governance in corso rilevando la deriva della configurazione prima che causi attrito, segnalando i limiti in avvicinamento prima che diventino bloccanti, imponendo standard coerenti in ogni area di lavoro indipendentemente da chi la configura e fornendo risposte precise a chiunque nel team senza attendere uno specialista. Questo insieme copre l’intero ciclo di vita della corretta configurazione di un’area di lavoro e del suo mantenimento in questo modo con la crescita dell’utilizzo.

Per informazioni, consulta [Abilità disponibili per l&#39;installazione diretta](/help/quicksilver/workfront-basics/workfront-mcp-server/direct-skills.md).

## Trascinare le righe nella vista tabella

>[!NOTE]
>
>Anteprima: 30 luglio 2026
>Versione rapida di produzione: 13 agosto 2026
>Produzione per tutti: 15 ottobre 2026

L’esperienza di trascinamento e rilascio di righe nella vista tabella è stata migliorata visivamente.

Per informazioni, vedere [Gestire la visualizzazione della tabella](/help/quicksilver/planning/views/manage-the-table-view.md).


## Campi record connessi dipendenti

>[!NOTE]
>
>Anteprima: 30 luglio 2026
>Versione rapida di produzione: 13 agosto 2026
>Produzione per tutti: 15 ottobre 2026

Workspace Manager ora può definire le dipendenze tra i tipi di record collegati. Ad esempio, quando si verifica un campo Regione, vengono visualizzati solo i valori associati all’area geografica selezionata. Questa impostazione viene configurata direttamente nella configurazione del campo connessione: quando si aggiunge una connessione da un tipo di record Geo a un tipo di record dipendente (come Area), una nuova impostazione consente ai manager dell’area di lavoro di contrassegnarla come dipendente dal tipo di record Geo, utilizzando le relazioni già stabilite tra tali tipi di record.

Una volta configurato, qualsiasi tipo di record che fa riferimento a entrambi i campi (ad esempio una campagna) vedrà immediatamente l’effetto: la selezione di un valore Geo restringe il selettore Regione solo alle aree effettivamente collegate a tale Geo. In questo modo la struttura dei record viene applicata automaticamente, eliminando combinazioni non corrispondenti e riducendo la pulizia manuale.

Questo aggiornamento include le seguenti funzionalità:

* È stata aggiunta la nuova sezione Impostazioni connessione nella scheda Nuova connessione, durante la connessione dei tipi di record
* Nella nuova sezione è stata aggiunta l’impostazione Rendi la connessione dipendente


Per informazioni, vedere [Gestire le connessioni dipendenti](/help/quicksilver/planning/architecture/manage-dependent-connections.md).




## Mostra nuovo indicatore di commento per un record nella vista tabella

>[!NOTE]
>
>Anteprima: 30 luglio 2026
>Versione rapida di produzione: 13 agosto 2026
>Produzione per tutti: 15 ottobre 2026

È stato aggiunto un nuovo indicatore che indica quando in un record sono presenti commenti non letti. L&#39;indicatore viene visualizzato nell&#39;angolo superiore destro del campo principale del record nella visualizzazione tabella.

Per ulteriori informazioni, vedere [Gestire i commenti dei record](/help/quicksilver/planning/records/manage-record-comments.md).

## Personalizzazione del colore del record e codifica a colori basata sulla connessione

>[!NOTE]
> 
>Anteprima: 23 luglio 2026
>Versione rapida di produzione: 13 agosto 2026
>Produzione per tutti: 15 ottobre 2026

I record ora supportano palette di colori personalizzabili che consentono di aggiornare i colori assegnati automaticamente ai nuovi record a colori standard o personalizzati.

In questo miglioramento sono incluse le seguenti modifiche: 

* Abbiamo aggiunto l’opzione Colore alle seguenti aree:
  * L&#39;icona Campi nella vista tabella. 
  * La sezione Stile barra nell&#39;area Impostazioni di una timeline e di una vista calendario

    Quando l&#39;impostazione Colore è attivata, il colore assegnato a un nuovo record viene visualizzato ovunque in queste visualizzazioni. 

* Un cerchio di colori viene aggiunto alla pagina Dettagli del record. 
* È ora possibile aggiungere campi record a selezione singola, multipla e collegati alla codifica a colori delle barre nelle visualizzazioni Timeline e Calendario quando si effettua la colorazione in base ai valori di Campo. 
* È possibile attivare la visualizzazione del colore, oltre al nome e all&#39;immagine di un record quando si creano campi record connessi. 
* Anche la sezione Colore nell’area Impostazioni è stata razionalizzata rimuovendo l’opzione &quot;Nessuno&quot;.  

Per informazioni, vedere [Creare record](/help/quicksilver/planning/records/create-records.md). 

## Planning Designer ora richiede l&#39;accettazione del contratto Beta

>[!NOTE]
>Anteprima e produzione per tutti i clienti: 20 luglio 2026
>[!BADGE Fuori pianificazione]{type=Neutral}

Planning Designer ora richiede un contratto Beta accettato da utilizzare. La tua azienda non è tenuta a firmare un contratto di intelligenza artificiale. Questo è disponibile per tutti i clienti.

A questo scopo, nella sezione Configurazione della sezione Opt in AI Beta è stata spostata l’opzione Planning Designer.

Se si avvia Planning Designer senza un contratto Beta accettato, verrà richiesta l&#39;accettazione prima dell&#39;apertura del generatore di workspace.

Per informazioni, vedere [Introduzione ad Adobe Workfront Planning Designer](/help/quicksilver/planning/general/planning-ai-designer.md).
