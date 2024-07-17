---
content-type: reference
navigation-topic: betas
title: '"Reporting Canvas beta: overview" (Reporting Canvas beta: panoramica)'
description: Informazioni sul programma beta per il prossimo strumento Reporting Canvas per Adobe Workfront
author: Nolan
feature: Product Announcements
hidefromtoc: true
hide: true
exl-id: 5767ef7d-1bc3-40d8-abeb-02b15166a0a3
source-git-commit: 535e9c8481ce0781ee0d35636bb6d56de4d1e102
workflow-type: tm+mt
source-wordcount: '1061'
ht-degree: 1%

---

# Reporting Canvas beta: panoramica

## Reporting Canvas

Una completa riprogettazione del reporting in Workfront, il nuovo strumento Reporting Canvas è attualmente in fase di sviluppo. Nella progettazione di Reporting Canvas, abbiamo lavorato sodo per fornire un’esperienza che offra la massima flessibilità associata a un design intuitivo e modulare, in modo che gli utenti come te possano sfruttare al meglio i tuoi dati nella creazione e nella condivisione di report. Grazie a un nuovo tipo di rapporto unificato che consente di trascinare quasi ogni elemento su un’area di lavoro illimitata, la creazione di un capolavoro di dati visivi sarà presto più semplice che mai.

Questo articolo contiene informazioni sulla versione beta privata corrente, limitata a clienti specifici. Nuove funzioni di Reporting Canvas vengono ora distribuite tramite i dashboard di Canvas. Per ulteriori informazioni, vedere **Piano di sviluppo** di seguito.

### Piano di sviluppo

Siamo nelle fasi finali della risoluzione di un problema di qualità dei dati che abbiamo osservato all’inizio della versione beta di Reporting Canvas. Presto riprenderemo a lavorare per fornire nuove visualizzazioni, espandere la selezione di oggetti Workfront da segnalare e migliorare le esperienze di creazione e distribuzione dei rapporti, tutte parti integranti nella realizzazione dei nostri obiettivi per Reporting Canvas (Area di lavoro di reporting).

Queste nuove esperienze verranno distribuite in modo incrementale, a partire dalla versione 23.2, tramite la nuova pagina Dashboard di Canvas, ora disponibile nell’ambiente di anteprima. Le dashboard di Canvas consentono di visualizzare i rapporti esistenti, insieme alle nuove funzionalità di reporting che stiamo creando, e fungeranno da ambiente principale per la distribuzione e il test delle nuove funzioni di Reporting Canvas. Per ulteriori informazioni sull&#39;attivazione e l&#39;utilizzo dei dashboard di Canvas, vedere [Panoramica dei dashboard di Canvas](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/canvas-dashboards-overview.md).

## Partecipare alla versione beta

>[!IMPORTANT]
>
>Le informazioni beta seguenti sono per gli amministratori che sono già stati inclusi nella versione beta dell’area di lavoro rapporti, che non accetta più nuovi partecipanti. Se desideri testare le nuove funzioni di Reporting Canvas man mano che vengono aggiunte, consulta **Piano di sviluppo** sopra per informazioni sull&#39;abilitazione di Canvas Dashboards.

### Disponibilità

La versione beta dell’Area di lavoro rapporti è disponibile per tutte le organizzazioni che si trovano su AWS, indipendentemente dalla regione.

### Partecipa alla versione beta

La versione beta di Reporting Canvas è completamente facoltativa, ma può essere accettata solo da un amministratore Workfront. Per fornire il consenso come amministratore di sistema:

1. Seleziona l&#39;icona **Reporting (beta)** nel menu principale dell&#39;istanza di Workfront.
1. Fai clic su **Accetta** per accettare i termini e le condizioni.
1. Consente di aggiungere i dati dell’organizzazione all’area di lavoro rapporti (l’operazione potrebbe richiedere alcune ore).
1. Inizia a utilizzare Reporting Canvas (Area di lavoro rapporti).

Dopo l’aggiunta dei dati dell’organizzazione all’area di lavoro rapporti, gli altri amministratori di sistema possono scegliere di partecipare singolarmente allo stesso modo (senza attendere che i dati vengano aggiunti nuovamente).

Per fornire il consenso ad altri utenti che non sono amministratori di Workfront:

1. Seleziona l&#39;icona **Reporting (beta)** nel menu principale dell&#39;istanza di Workfront.
1. Fai clic su **Autorizzazioni Reporting Canvas**.
1. Cerca e seleziona gli utenti specifici a cui desideri partecipare.

   >[!IMPORTANT]
   >
   >Gli utenti a cui si concede l&#39;accesso a Reporting Canvas avranno accesso a **tutti** i dati nel sistema in sola lettura, indipendentemente dalle autorizzazioni standard per la visualizzazione di tali dati.

1. Fai clic su **Salva**.
1. Aggiungi l&#39;icona **Generazione rapporti (versione beta)** nel modello di layout principale di ogni utente selezionato. Per ulteriori informazioni, vedere [Personalizzare il menu principale utilizzando un modello di layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).
1. Ogni utente deve quindi passare individualmente all&#39;icona **Reporting (beta)** nel menu principale e accettare i termini e le condizioni.

### Invia feedback

Per inviare un feedback sulla versione beta:

1. Nell&#39;area di lavoro Reporting di Workfront, fare clic sul pulsante **Invia feedback**.
1. Compila il modulo, quindi fai clic su **Invia**.

## Domande frequenti su Beta

+++Posso migrare i miei rapporti legacy all’area di lavoro di reporting?

In breve, la migrazione dei rapporti legacy non sarà disponibile durante la versione beta. Tuttavia, si tratta di una funzione pianificata (con alcune avvertenze descritte di seguito) per il lancio ufficiale.

Sebbene la barriera per la creazione di nuovi rapporti sia stata notevolmente ridotta con Reporting Canvas (Area di lavoro rapporti), il ripristino di alcuni dei rapporti e delle dashboard esistenti contribuirà ad accelerare il processo di adozione. Desideriamo quindi fornire gli strumenti e le risorse necessarie per assicurarti di poter trasferire tutti gli elementi legacy pertinenti in modo da iniziare con il piede giusto nell’area di lavoro Reporting. Tuttavia, poiché Reporting Canvas (Area di lavoro di reporting) rappresenta una modifica radicale nel modo in cui funziona il reporting corrente, sarebbe impossibile migrare ogni rapporto o dashboard esattamente come avviene attualmente.

La nostra strategia attuale per la migrazione nelle versioni ufficiali consente di effettuare le seguenti operazioni:

1. Identifica i rapporti e le dashboard pertinenti

   1. Consente di esportare un file CSV di tutti i rapporti e dashboard del sistema insieme a eventuali informazioni di tracciamento rilevanti (numero di visualizzazioni, quando e da chi).
   1. Fornisci un’esportazione dei rapporti configurati con le consegne pianificate insieme ai destinatari.

1. Seleziona i report e le dashboard di cui vuoi eseguire la migrazione, quindi fai clic su **Migra**

   Si tratta di una migrazione unidirezionale. Crea una copia dei report e delle dashboard selezionati nell’area di lavoro dei rapporti, lasciando intatto il report o la dashboard legacy nello strumento di reporting corrente.

   Puoi eseguire la migrazione dello stesso report o dashboard per il numero di volte desiderato.

1. In Reporting Canvas (Area di lavoro rapporti), accertati che tutti i rapporti e le dashboard selezionati siano stati migrati.
+++

+++Perché non è possibile visualizzare tutti gli oggetti che eseguo normalmente?

Per fornire la versione beta ai nostri clienti il prima possibile, l’abbiamo rilasciata solo con un sottoinsieme dei molti tipi di oggetti disponibili oggi in Workfront. Di seguito sono elencati i tipi di oggetto attualmente supportati nella versione beta:

* Assegnazione
* Documento
* Approvazione documento
* Spesa
* Ora
* Problema
* Nota
* Portfolio
* Progetto
* Programma
* Attività
* Scheda orario
* Elemento di lavoro
+++

+++Se si verifica un errore nell’area di lavoro di reporting durante la versione beta, i dati della mia organizzazione saranno interessati?

No. La versione beta utilizza una copia dei dati dell’organizzazione che viene inserita nell’area di lavoro dei rapporti. Anche se questo significa che sei sicuro di sperimentare durante la versione beta senza il rischio di influenzare i dati importanti, significa anche che la modifica in linea dei dati nell’Area di lavoro di reporting non sarà disponibile fino al lancio ufficiale.
+++

+++Posso rinunciare alla versione beta dopo l’iscrizione?

Un amministratore di Workfront non può rinunciare alla versione beta, ma può essere rimosso effettuando le seguenti operazioni:

1. Accedere come amministratore di sistema.
1. Passa a Reporting Canvas (Area di lavoro rapporti).
1. Fare clic su Reporting Canvas **autorizzazioni**.
1. Rimuovi dall’elenco gli utenti per i quali hai acconsentito la rinuncia alla versione beta.
1. Fai clic su **Salva**.
+++
