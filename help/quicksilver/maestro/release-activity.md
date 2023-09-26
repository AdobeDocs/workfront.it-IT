---
title: Attività di rilascio Adobe Maestro
description: Utilizza Maestro per creare oggetti, campi e aree di lavoro personalizzati.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 28602d66b43ec4c30a9f13cff43157b978439d99
workflow-type: tm+mt
source-wordcount: '1458'
ht-degree: 0%

---


# Attività di rilascio Adobe Maestro

>[!IMPORTANT]
>
>Attualmente, Adobe Maestro fa parte di un programma beta aperto a un numero limitato di clienti.
>
>Contatta il rappresentante del tuo account per ulteriori informazioni su come partecipare al programma beta per Maestro.
>
>Per informazioni, consulta [Panoramica di Adobe Maestro](../maestro/maestro-overview.md).

Questo articolo elenca le funzionalità rilasciate dopo il lancio del programma beta chiuso Maestro, il 22 maggio 2023.

Le funzioni rilasciate sono elencate in ordine di rilascio, a partire da quelle più recenti. I clienti che partecipano al programma Maestro closed beta possono accedere a tutte le funzioni nei loro ambienti di anteprima e produzione.

>[!IMPORTANT]
>
>La documentazione a cui si fa riferimento nelle sezioni seguenti sarà disponibile un po’ di tempo dopo il rilascio delle funzioni in produzione.

In questa sezione sono elencate le funzioni e le patch rilasciate dopo il lancio del programma beta chiuso Maestro, il 22 maggio 2023.

Le funzioni vengono rilasciate settimanalmente e sono elencate in ordine di rilascio, con la prima più recente. I clienti che partecipano al programma Maestro closed beta possono accedere a tutte le funzioni nei loro ambienti di anteprima e produzione.

## Settimana del 18 settembre 2023

### Riordina righe

Anteprima e produzione: 20 settembre 2023

È ora possibile riordinare una o più righe (o record) nella visualizzazione Tabella di una pagina del tipo di record.

## Settimana del 4 settembre 2023

### Collegare i record Maestro alle aziende e ai gruppi Workfront

Anteprima e produzione: 5 settembre 2023

Ora è possibile collegare un record Maestro con aziende e gruppi Workfront. È innanzitutto necessario creare una connessione tra un tipo di record Maestro e i tipi di oggetto Società e gruppi di Workfront. Quindi puoi collegare un singolo record Maestro del tipo di record selezionato a singole aziende e gruppi Workfront.

Considera quanto segue:

* È necessario creare una connessione tra i tipi di record Maestro e i tipi di oggetto Società Workfront e Gruppo per ogni area di lavoro.

* Non è possibile collegare tipi di record di tassonomia con tipi di oggetto Workfront.

* È possibile collegare più record Maestro alla stessa società o gruppo Workfront e più aziende o gruppi allo stesso record Maestro.

* Non è possibile modificare aziende o gruppi in Maestro. Tutte le modifiche di società o gruppi eseguite in Workfront sono visibili in Maestro, quando si esaminano i record collegati a Maestro.

  Per ulteriori informazioni, consulta i seguenti articoli:

   * [Connetti tipi di record](../maestro/architecture-and-fields/connect-record-types.md)
   * [Collega record](../maestro/records/connect-records.md)

### Supporto URL per campi di testo a riga singola

Anteprima e produzione: 7 settembre 2023

Per una migliore visibilità quando si lavora con i collegamenti nella vista Tabella, è stato aggiunto il supporto per gli URL nei campi di testo a riga singola. L’utilizzo degli URL per altri siti web o unità esterne durante l’aggiornamento di un campo di testo a riga singola, ora li identifica come collegamenti e consente di fare clic su di essi dalla tabella. Prima di questo miglioramento, i collegamenti venivano visualizzati come testo.

## Settimana del 28 agosto 2023

### Menu di visibilità dei campi per la barra degli strumenti Vista tabella

Anteprima e produzione: 31 agosto 2023

Per visualizzare le informazioni corrette su un determinato set di record, in particolare se si desidera condividere la visualizzazione con altri utenti che devono visualizzare alcuni campi di un tipo di record, ma non tutti, è ora possibile selezionare i campi o le colonne da visualizzare e quelli da nascondere nella visualizzazione Tabella.

È possibile nascondere o visualizzare singoli campi da ogni intestazione delle colonne dei campi oppure gestire tutti i campi del tipo di record da un&#39;impostazione nella barra degli strumenti della visualizzazione tabella.

Per ulteriori informazioni, consulta [Gestire la vista tabella](../maestro/views/manage-the-table-view.md).

## Settimana del 21 agosto 2023

### Collegare i record Maestro a programmi e portafogli

Anteprima e produzione: 24 agosto 2023

Ora è possibile collegare un record Maestro con i programmi e i portfolio Workfront. È necessario creare una connessione tra un tipo di record Maestro e un programma o un portfolio che crea un campo connesso. È quindi possibile collegare qualsiasi record Maestro di tutti gli altri tipi di record all&#39;interno della stessa area di lavoro a programmi e portfolio specifici che creano un tipo di record di Portfolio Workfront Program o Workfront di sola lettura nella stessa area di lavoro. Considera quanto segue:

* I tipi di record del connettore Workfront sono univoci per ogni area di lavoro.
* È possibile collegare più record Maestro allo stesso programma o portfolio Workfront e più programmi e portfolio allo stesso record Maestro.
* Non è possibile modificare programmi e portafogli in Maestro. Tutte le modifiche al programma e al portfolio eseguite in Workfront sono visibili in Maestro durante la revisione dei record collegati.

### Nuova funzionalità di ordinamento per la vista tabella

Anteprima e produzione: 24 agosto 2023

È ora possibile ordinare i record nella vista tabella di una pagina del tipo di record.
Sono ora disponibili le seguenti funzionalità:

* Ordinamento a livello di tabella, in cui è possibile ordinare più campi contemporaneamente.
* Ordinamento a livello di colonna o di campo, in cui è possibile ordinare per singolo campo alla volta.

### Miglioramenti alla vista timeline: nuovo look-and-feel dei raggruppamenti e switch di visualizzazione Compatto/Standard

Anteprima e produzione: 24 agosto 2023

Sono stati introdotti i seguenti miglioramenti alla vista timeline:

* Ora potete visualizzare la vista timeline nelle seguenti modalità:

   * Standard: visualizza i record in righe separate.
   * Compatta: visualizza i record le cui date non si intersecano sulla stessa riga.

* È stato modificato l’aspetto delle linee di raggruppamento nella vista timeline in modo che vengano visualizzate sopra la timeline dei record in esse contenuti. Prima di questo miglioramento, le linee di raggruppamento venivano visualizzate sull&#39;intera lunghezza della timeline.

## Settimana del 14 agosto 2023

### Riordinare le colonne nella vista tabella

È ora possibile riordinare le colonne nella vista tabella Maestro. Quando riordinate le colonne, tenete presente quanto segue:

* Il campo Nome è sempre il primo campo nella visualizzazione tabella di una pagina di tipo record

* Impossibile spostare il campo Nome in un&#39;altra posizione

* Il campo Nome è bloccato e non fa parte dello scorrimento orizzontale.

### Scorrimento orizzontale per la visualizzazione della timeline

Ora è possibile scorrere orizzontalmente nella visualizzazione timeline di un tipo di record.

## Settimana del 7 agosto 2023

### Importare tipi di record da un file di Excel

Anteprima e produzione: 10 agosto 2023

È ora possibile importare un file Excel per creare tipi di record in un&#39;area di lavoro. I fogli del file diventano i tipi di record e le colonne del file diventano i rispettivi campi.

### Esperienza migliorata per la connessione di tipi di record e progetti

Anteprima e produzione: 10 agosto 2023

È stata migliorata la modalità di connessione dei tipi di record, inclusa la connessione ai progetti Workfront. Come parte di questo miglioramento, sono state apportate le seguenti modifiche quando si aggiunge un campo per un tipo di record dalla vista tabella:

* È stato rimosso il campo Tipo di relazione dalla scheda &quot;Nuovo campo&quot;.

* Aggiungere una scheda &quot;Nuova connessione&quot; in cui è possibile selezionare direttamente il record o il tipo di oggetto a cui si desidera connettersi, eliminando la necessità di un campo di tipo Relazione.

## Settimana del 10 luglio 2023

### Aggiornare l&#39;aspetto di un tipo di record

Anteprima e produzione: 13 luglio 2023

È ora possibile selezionare un&#39;icona personalizzata per un tipo di record e un colore personalizzato per l&#39;icona del tipo di record.

### Nuovo tipo di campo Casella di controllo

Anteprima e produzione: 13 luglio 2023

Ora puoi aggiungere un tipo di campo Casella di controllo ai tipi di record Maestro. È possibile utilizzare un campo di tipo Casella di controllo per aggiungere una singola opzione a un record. È possibile utilizzare questo campo per indicare un attributo o uno stato specifico per quel record specifico. È ad esempio possibile utilizzarlo come flag per tenere traccia di completamento, approvazione o qualsiasi altro attributo binario per ogni record.

## Settimana del 26 giugno 2023

### Attivazione rapida del menu contestuale in una tabella

Anteprima e produzione: 28 giugno 2023

È stata abilitata la possibilità di attivare il menu contestuale facendo clic con il pulsante destro del mouse in un punto qualsiasi di una riga di record quando si visualizzano i record nella vista tabella o in un tipo di record. È ora possibile visualizzare, eliminare o copiare rapidamente un collegamento alla pagina Dettagli del record quando si accede al menu contestuale da un punto qualsiasi della vista tabella di un tipo di record. Prima di questo miglioramento, il menu contestuale era accessibile solo dal menu Altro nella colonna Nome di un record.

## Settimana del 19 giugno 2023

### I nomi dei campi record sono univoci

Ora è stato introdotto un requisito per cui i nomi dei campi di un tipo di record Maestro devono avere nomi univoci. I campi che appartengono a tipi di record diversi non devono avere nomi univoci.

## Settimana del 5 giugno 2023

### Collegare i record Maestro con i progetti Workfront

Anteprima e produzione: 5 giugno 2023

Ora puoi collegare un record Maestro a progetti Workfront. È necessario creare un tipo di record Connector Maestro per stabilire la connessione tra i record Maestro e i progetti Workfront. Quindi, puoi collegare qualsiasi record Maestro da tutti gli altri tipi di record al record del connettore utilizzando il campo Relazione. Considera quanto segue:

* È necessario disporre di un tipo di record connettore per Workfront per ogni area di lavoro.
* È possibile collegare più record Maestro allo stesso progetto Workfront e più progetti allo stesso record Maestro.
* Non è possibile modificare i progetti in Maestro. Tutte le modifiche al progetto eseguite in Workfront sono visibili in Maestro durante la revisione dei record collegati.

## Settimana del 29 maggio 2023

### Requisito di due date per la creazione di una vista Timeline

Anteprima e produzione: 31 maggio 2023

Per creare una visualizzazione Sequenza temporale, è necessario avere almeno due campi data associati a un tipo di record.