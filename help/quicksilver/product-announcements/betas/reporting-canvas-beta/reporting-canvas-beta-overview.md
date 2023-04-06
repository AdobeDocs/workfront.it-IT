---
content-type: reference
navigation-topic: betas
title: '''Reporting Canvas beta: panoramica"'
description: Informazioni sul programma beta per il prossimo strumento Reporting Canvas per Adobe Workfront
author: Nolan
feature: Product Announcements
exl-id: cc0adf28-08ab-4330-b901-219ab687f02f
source-git-commit: d738ef3f6642d5b1a646f58896575a2971bbc06a
workflow-type: tm+mt
source-wordcount: '1060'
ht-degree: 1%

---


# Reporting Canvas beta: panoramica

## Area di lavoro di reporting

Una completa reimmaginazione del reporting in Workfront, il nuovo strumento Area di reporting è attualmente in fase di sviluppo. Nella progettazione di Reporting Canvas, abbiamo lavorato sodo per fornire un’esperienza che offra la massima flessibilità abbinata a un design intuitivo e modulare, in modo che gli utenti come voi possano sfruttare al meglio i vostri dati per creare e condividere rapporti. Grazie a un nuovo tipo di rapporto unificato che consente di trascinare quasi tutti gli elementi su un&#39;area di lavoro senza limiti, la creazione di un capolavoro di dati visivi sarà presto più semplice che mai.

Questo articolo contiene informazioni sull’attuale versione beta privata, limitata a clienti specifici. Le nuove funzioni Area di lavoro di reporting vengono ora implementate tramite dashboard di Canvas. Vedi **Piano di sviluppo** qui sotto per ulteriori informazioni.

### Piano di sviluppo

Siamo nelle fasi finali di risoluzione di un problema di qualità dei dati che abbiamo osservato all&#39;inizio nella versione beta di Reporting Canvas. Presto riprenderemo il lavoro per fornire nuove visualizzazioni, espandere la selezione di oggetti Workfront segnalabili e migliorare le esperienze di creazione e distribuzione dei rapporti, tutte parte integrante della realizzazione dei nostri obiettivi per Reporting Canvas.

A partire dalla versione 23.2, distribuiremo queste nuove esperienze in modo incrementale tramite la nuova pagina Dashboard di Canvas che è ora disponibile nel tuo ambiente di anteprima. I dashboard di Canvas consentono di visualizzare i rapporti esistenti insieme alle nuove funzionalità di reporting che stiamo creando e fungeranno da ambiente principale per la distribuzione e il test delle nuove funzionalità per Area di lavoro di reporting. Per ulteriori informazioni sull’abilitazione e l’utilizzo delle dashboard di Canvas, consulta [Panoramica delle dashboard di Canvas](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/canvas-dashboards-overview.md).

## Partecipa alla versione beta

>[!IMPORTANT]
>
>Le informazioni beta riportate di seguito sono per gli amministratori che sono già stati inclusi nella versione beta di Reporting Canvas, che non accetta più nuovi partecipanti. Se desideri testare le nuove funzioni di Area di lavoro rapporti man mano che vengono aggiunte, consulta **Piano di sviluppo** per informazioni sull’abilitazione delle dashboard di Canvas.

### Disponibilità

La versione beta di Reporting Canvas è disponibile per tutte le organizzazioni che si trovano su AWS, indipendentemente dall’area geografica.

### Unisciti alla versione beta

La versione beta di Reporting Canvas è completamente facoltativa, ma può essere utilizzata solo da un amministratore Workfront. Per effettuare il consenso come amministratore di sistema:

1. Seleziona la **Reporting (beta)** nel menu Principale dell’istanza Workfront.
1. Fai clic su **Accetta** accettare i termini e le condizioni.
1. Consenti l’aggiunta dei dati della tua organizzazione all’Area di lavoro rapporti (l’operazione potrebbe richiedere fino a poche ore).
1. Iniziare a utilizzare Area di lavoro rapporti.

Dopo aver aggiunto i dati della tua organizzazione a Reporting Canvas, altri amministratori di sistema possono scegliere di partecipare individualmente allo stesso modo (senza attendere che i dati vengano aggiunti nuovamente).

Per accettare altri utenti che non sono amministratori di Workfront:

1. Seleziona la **Reporting (beta)** nel menu Principale dell’istanza Workfront.
1. Fai clic su **Autorizzazioni di Reporting Canvas**.
1. Cerca e seleziona gli utenti specifici a cui vuoi partecipare.

   >[!IMPORTANT]
   >
   >Gli utenti a cui si concede l’accesso a Reporting Canvas avranno accesso a **tutto** i dati presenti nel sistema con capacità di sola lettura, indipendentemente dalle autorizzazioni standard per visualizzare tali dati.

1. Fai clic su **Salva**.
1. Aggiungi il **Reporting (beta)** nel modello di layout principale di ogni utente selezionato. Per ulteriori informazioni, consulta [Personalizzare il menu principale utilizzando un modello di layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).
1. Ogni utente deve quindi navigare individualmente fino al **Reporting (beta)** nel menu principale e accettare i termini e le condizioni.

### Invia feedback

Per inviare un feedback sulla versione beta:

1. In Area di reporting in Workfront, fai clic sul pulsante **Invia feedback** pulsante .
1. Compila il modulo, quindi fai clic su **Invia**.

## Domande frequenti su Beta

+++Posso migrare i miei rapporti legacy in Reporting Canvas?

In breve, la migrazione dei rapporti legacy non sarà disponibile durante la versione beta. Tuttavia, si tratta di una funzione pianificata (con alcuni avvertimenti descritti di seguito) per il lancio ufficiale.

Sebbene la barriera alla creazione di nuovi report sia stata notevolmente ridotta con Reporting Canvas, sappiamo che la presenza di alcuni dei tuoi report e dashboard esistenti contribuirà ad accelerare il processo di adozione. In quanto tale, vogliamo fornire gli strumenti e le risorse necessari per assicurarci che tu possa portare con sé tutti gli elementi legacy rilevanti per assicurarti di iniziare con il piede giusto in Reporting Canvas. Dato che Reporting Canvas è un cambiamento così radicale nel modo in cui funziona il reporting attuale, tuttavia, sarebbe impossibile migrare ogni report o dashboard esattamente come è oggi.

La nostra attuale strategia di migrazione nelle versioni ufficiali ti permette di:

1. Identificare i report e le dashboard pertinenti

   1. Consente di esportare un CSV di tutti i rapporti e le dashboard del sistema, insieme a qualsiasi informazione di tracciamento pertinente (numero di visualizzazioni, quando e da chi).
   1. Fornisci un’esportazione di rapporti configurati con consegne programmate insieme ai destinatari.

1. Seleziona i report e le dashboard di cui vuoi eseguire la migrazione, quindi fai clic su **Migrare**

   Questa è una migrazione a senso unico. Crea una copia dei rapporti e delle dashboard selezionati in Area di lavoro rapporti, lasciando intatto il rapporto o il dashboard legacy nello strumento di reporting corrente.

   Puoi eseguire la migrazione dello stesso report o dashboard il numero di volte desiderato.

1. In Area di lavoro rapporti , accertati che tutti i rapporti e le dashboard selezionati siano stati migrati.
+++

+++Perché non riesco a vedere tutti gli oggetti che faccio normalmente?

Al fine di fornire la versione beta ai nostri clienti il prima possibile, l’abbiamo rilasciata con solo un sottoinsieme dei molti tipi di oggetti disponibili in Workfront oggi. Di seguito sono elencati i tipi di oggetti attualmente supportati nella versione beta:

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

++ Se qualcosa va storto in Reporting Canvas durante la versione beta, i dati della mia organizzazione saranno interessati?

No. La versione beta utilizza una copia dei dati dell’organizzazione che viene compilata in Area di lavoro rapporti. Anche se questo significa che puoi sperimentare in tutta sicurezza durante la versione beta senza rischi di influire su dati importanti, significa anche che la modifica in linea dei dati in Reporting Canvas non sarà disponibile fino al lancio ufficiale.
+++

+++Posso rinunciare alla versione beta dopo l’iscrizione?

Un amministratore Workfront non può rinunciare alla versione beta; tuttavia, è possibile rimuovere gli amministratori non di sistema eseguendo le operazioni seguenti:

1. Accedi come amministratore di sistema.
1. Passa a Area di lavoro rapporti.
1. Fai clic su Area di lavoro rapporti **permissions**.
1. Rimuovi dall’elenco degli utenti per i quali desideri rinunciare alla versione beta.
1. Fai clic su **Salva**.
+++
