---
product-area: documents;workfront-integrations
navigation-topic: adobe-cloud-drive
title: Usa Adobe Cloud Drive
description: Lavora con i tuoi progetti di archiviazione cloud Adobe direttamente da Finder o Esplora file utilizzando Adobe Cloud Drive. Aprire e modificare i file in qualsiasi applicazione, lavorare offline e risolvere i conflitti.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
    internal-label: Integrations
  - id: a1f87682-0525-5459-aa06-3560bb4c3b2a
    internal-label: Workfront Integrations and Apps
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: c16dc2b8b508f71767999aec7029664f5d31f23f
workflow-type: tm+mt
source-wordcount: '3955'
ht-degree: 1%
---
# Usa Adobe Cloud Drive

Dopo aver installato Adobe Cloud Drive, puoi lavorare con i progetti di archiviazione cloud di Adobe direttamente da Finder o Esplora file. Puoi aprire e modificare i file in qualsiasi applicazione, lavorare offline e consentire ad Adobe Cloud Drive di sincronizzare le modifiche nel cloud.

Per informazioni sull&#39;installazione di Adobe Cloud Drive, vedere [Installare Adobe Cloud Drive](/help/quicksilver/documents/adobe-cloud-drive/install-adobe-cloud-drive.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Versione Adobe Workfront</td> 
   <td>Flusso di lavoro di Ultimate, con l'archiviazione cloud Adobe abilitata</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
   <td>
      <p>Visualizzare l’accesso a un progetto per visualizzarlo in Adobe Cloud Drive</p>
      <p>Modificare l'accesso a un progetto per aggiungere, modificare o eliminare file al suo interno</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Accedere ai progetti

1. Aprire Finder (Mac) o Esplora file (Windows).
1. Passa a **Adobe Cloud Drive**.
1. Sfoglia l’elenco dei progetti a cui hai accesso in Workfront. Aprire una cartella di progetto per visualizzarne i file e le sottocartelle.

   >[!NOTE]
   >
   >* Le cartelle di progetto sono di sola lettura al livello superiore. Non è possibile rinominare, eliminare o spostare le cartelle di progetto.
   >* È possibile utilizzare file e cartelle all&#39;interno di una cartella di progetto, ad esempio aprire, modificare, creare, eliminare e così via.
   >* I progetti Workfront precedenti non vengono visualizzati in Adobe Cloud Drive. Sono disponibili solo i progetti archiviati nell’archiviazione cloud di Adobe.

## Indicatori di stato del file

Adobe Cloud Drive utilizza indicatori visivi per mostrare lo stato di sincronizzazione dei file. Le icone sono diverse tra Windows e Mac.

### Indicatori di stato dei file in Windows

| Icona | Stato | Significato file | Significato cartella |
| --- | --- | --- | --- |
| ![Icona Solo online](assets/acd-windows-online-only.png) | Solo online | Il file è sincronizzato ma è disponibile solo online. | Tutti i file all&#39;interno di sono disponibili online. |
| ![Icona di sincronizzazione](assets/acd-windows-syncing.png) | Sincronizzazione | Gli ultimi aggiornamenti del file vengono sincronizzati nella cache locale o nell’archiviazione cloud di Adobe. | È in corso la sincronizzazione di almeno un file nella cartella. |
| ![Icona offline disponibile](assets/acd-windows-available-offline.png) | Disponibile offline | Il file è sincronizzato e disponibile offline. | Almeno un file nella cartella è disponibile offline. |
| ![Icona bloccata](assets/acd-windows-pinned.png) | Bloccato (Mantieni sempre sul dispositivo) | Il file viene sincronizzato e mantenuto sempre offline. Adobe Cloud Drive non elimina automaticamente i contenuti bloccati. | Tutti i file nella cartella si trovano nella cache locale e sono disponibili offline. |
| ![Icona di sola lettura](assets/acd-windows-read-only.png) | Sola lettura | File di sola lettura. | La cartella è di sola lettura. |
| ![Icona errore di sincronizzazione](assets/acd-windows-sync-error.png) | Errore di sincronizzazione | Impossibile sincronizzare il file. Passa il puntatore del mouse sull’icona per visualizzare i dettagli. | Impossibile sincronizzare la cartella. Passa il puntatore del mouse sull’icona per visualizzare i dettagli. |
| ![Icona Sincronizza esclusi](assets/acd-windows-sync-excluded.png) | Sincronizzazione esclusa | Impossibile sincronizzare il file. Tipo o nome non supportato. | Impossibile sincronizzare la cartella a causa di un nome non supportato. |

### Indicatori di stato dei file in Mac

| Icona | Stato | Significato file | Significato cartella |
| --- | --- | --- | --- |
| (Nessuna icona) | Disponibile offline | Il file è sincronizzato e disponibile offline. | Tutti i file sono disponibili offline. |
| ![Icona Solo online](assets/acd-mac-online-only.png) | Solo online | Il file è sincronizzato e disponibile solo online. | Almeno un file nella cartella è solo online. |
| ![Icona di sincronizzazione](assets/acd-mac-syncing.png) | Sincronizzazione | Gli ultimi aggiornamenti del file vengono sincronizzati nella cache locale o nell’archiviazione cloud di Adobe. | Contenuto della cartella in fase di sincronizzazione. |
| ![Icona errore di sincronizzazione](assets/acd-windows-sync-error.png) | Errore di sincronizzazione | Impossibile aggiornare o sincronizzare il file. Passa il puntatore del mouse sull’icona per visualizzare i dettagli. | Impossibile aggiornare o sincronizzare la cartella. Passa il puntatore del mouse sull’icona per visualizzare i dettagli. |
| ![Icona Sincronizza esclusi](assets/acd-windows-sync-excluded.png) | Sincronizzazione esclusa | File escluso dalla sincronizzazione. | La cartella è esclusa dalla sincronizzazione. |
| ![Icona di sola lettura](assets/acd-mac-read-only.png) | Sola lettura | File di sola lettura. | La cartella è di sola lettura. |
| ![Icona bloccata](assets/acd-windows-pinned.png) | Bloccato (Mantieni sempre sul dispositivo) | Il file è bloccato per essere disponibile offline. Adobe Cloud Drive non elimina automaticamente i contenuti bloccati. | La cartella è bloccata per essere disponibile offline. |

### Descrizioni errori

Quando si verifica un errore o un problema di sincronizzazione, passa il cursore sull’icona del file o della cartella per visualizzare una descrizione del problema.

| Categoria di errore | Descrizione comando | Significato |
|---|---|---|
| Sincronizzazione esclusa | Tipo di file non supportato | Il tipo di file non è supportato da Adobe Cloud Drive. |
| Sincronizzazione esclusa | Nome file non supportato | Il nome file non è supportato da Adobe Cloud Drive. |
| Sincronizzazione esclusa | Progetto principale eliminato | Il progetto Workfront principale è stato eliminato. |
| Sincronizzazione sospesa | Contenuto del file non supportato | Impossibile sincronizzare il contenuto del file (ad esempio, è stato rilevato un problema di sicurezza). |
| Sincronizzazione sospesa | Caratteri non validi nel nome file | Il nome del file contiene caratteri non validi. |
| Sincronizzazione sospesa | Percorso completo troppo lungo | Il percorso del file supera la lunghezza massima consentita. |
| Sincronizzazione sospesa | Nessuna autorizzazione di scrittura | L&#39;accesso in scrittura a questo file o progetto è stato revocato. |
| Errore di sincronizzazione | Problema di autenticazione | Si è verificato un problema con le credenziali di accesso. |
| Errore di sincronizzazione | Archiviazione cloud non disponibile | I servizi cloud Adobe non sono al momento disponibili. |
| Errore di sincronizzazione | Archiviazione cloud completa | La quota di archiviazione cloud è piena. |
| Errore di sincronizzazione | Disco locale pieno | Spazio su disco locale insufficiente. |
| Errore di sincronizzazione | Nessuna connessione Internet | Il dispositivo non è connesso a Internet. |
| Errore di sincronizzazione | Errore imprevisto | Errore imprevisto durante la sincronizzazione. |
| Errore di sincronizzazione | Account bloccato | L&#39;account è stato bloccato dal servizio. |

>[!NOTE]
>
>Gli errori a livello di sistema, ad esempio disconnesso, errore di autenticazione, rete non disponibile, disco locale pieno o archiviazione cloud piena, vengono visualizzati nella barra delle applicazioni (Windows) o nella barra dei menu (Mac), non in singoli file.

### Sincronizza elenco di esclusione

Adobe Cloud Drive esclude alcuni file generati dal sistema, temporanei e di blocco dalla sincronizzazione. Sono esclusi i seguenti tipi di file e pattern:

| Categoria | Tipi di file/pattern | Descrizione |
|---|---|---|
| File di sistema | `.DS_Store`, `Thumbs.db` | Metadati del sistema operativo e file della cache delle miniature. |
| File di sistema e di memoria virtuale | `*.sys` (ad esempio `hiberfil.sys`, `pagefile.sys`, `swapfile.sys`) | File di sistema di grandi dimensioni utilizzati per la memoria virtuale, la sospensione o altre funzioni del sistema operativo. |
| File di indicizzazione macOS | `.Spotlight-V100`, `.fseventsd` | File di indicizzazione degli eventi di macOS Spotlight e di tracciamento degli eventi del file system. |
| File temporanei e di backup | `*.tmp`, `*.swp`, `*~`, `*.bak` | File temporanei, temporanei o di backup generati dalle applicazioni. |

## Apri un file

1. In Adobe Cloud Drive, accedi al file.
1. Fare doppio clic sul file.

   Il file viene aperto nell&#39;applicazione predefinita.

Adobe Cloud Drive supporta qualsiasi tipo di file aperto da un&#39;applicazione installata nel computer, tra cui:

* Formati Adobe Creative Cloud (PSD, AI, INDD, PRPROJ, AEP e così via)
* Documenti di Microsoft Office (DOCX, XLSX, PPTX)
* Immagini (JPG, PNG, GIF e così via)
* File video (MP4, MOV e così via)

>[!NOTE]
>
>I formati dei documenti cloud (PSDC, AIDC e così via) si aprono come equivalenti standard (PSD, AI e così via) quando vi si accede tramite Adobe Cloud Drive.

## Modificare e salvare un file

1. Apri un file da Adobe Cloud Drive.
1. Apportare le modifiche nell&#39;applicazione.
1. Salvare il file selezionando **File** > **Salva** o premendo Ctrl+S (Windows) o Comando+S (Mac).

   Le modifiche vengono sincronizzate automaticamente con l&#39;archiviazione cloud Adobe.

>[!IMPORTANT]
>
>Salva i file utilizzando **File** > **Salva** o la scelta rapida da tastiera. Evitare di utilizzare **Salva con nome** per creare copie, poiché genera file duplicati nell&#39;unità.

## Crea o aggiungi un nuovo file

Puoi creare un nuovo file direttamente in un progetto o aggiungere un file esistente dall’archivio locale.

### Creare un nuovo file da un&#39;applicazione

1. Aprire l&#39;applicazione da utilizzare per creare il file.
1. Crea il file come si farebbe normalmente.
1. Quando salvi, scegli un percorso all’interno della cartella di un progetto Adobe Cloud Drive.

   Il file viene visualizzato in Adobe Cloud Drive e viene sincronizzato con l’archiviazione cloud Adobe.

### Aggiungere un file esistente a un progetto

1. In Finder (Mac) o Esplora file (Windows), apri la cartella del progetto in Adobe Cloud Drive.
1. Trascina o copia i file dall’archivio locale nella cartella del progetto.

   I file vengono sincronizzati automaticamente con l’archiviazione cloud di Adobe.

## Rendi file e cartelle disponibili offline

Quando un file o una cartella è disponibile in modalità non in linea, è possibile aprirlo e modificarlo senza una connessione Internet. I file offline utilizzano lo spazio su disco locale.

### Mantieni un file o una cartella sul dispositivo

1. Fare clic con il pulsante destro del mouse sul file o sulla cartella in Adobe Cloud Drive.
1. Seleziona **Mantieni Sempre Su Questo Dispositivo**.

   Il file o la cartella viene scaricato nella cache locale e puoi utilizzarlo anche quando sei offline.

### Rimuovi l&#39;accesso offline per liberare spazio

1. Fare clic con il pulsante destro del mouse sul file o sulla cartella non in linea.
1. Selezionare **Spazio disponibile**.

   Il file o la cartella rimane nell’archiviazione cloud, ma viene rimosso dalla cache locale.

>[!NOTE]
>
>I file e le cartelle non in linea utilizzano lo spazio su disco locale. Rimozione dell&#39;accesso offline per i file e le cartelle non è più necessario liberare spazio.

## Copiare un file nell&#39;archivio locale

Puoi copiare un file da Adobe Cloud Drive nell’unità locale. L’originale rimane in Adobe Cloud Drive e la copia diventa un file locale indipendente.

1. Fare clic con il pulsante destro del mouse sul file in Adobe Cloud Drive.
1. Seleziona **Copia**, quindi incolla il file nel percorso nell&#39;unità locale in cui lo desideri.

   Il file viene copiato nella destinazione. L’originale rimane in Adobe Cloud Drive.

>[!NOTE]
>
>I file copiati nell&#39;archivio locale sono copie indipendenti. Le modifiche apportate a una copia locale non vengono sincronizzate con l’archiviazione cloud di Adobe.

<!-- Courtney check me: New sections below (Upload to Cloud through Open in Workfront) added for Adobe Cloud Drive v1.2.0, per helpxNewFeature.pdf from Pulkit Goel. Verify content, placement, and heading order. -->

## Caricare file nel cloud (caricamento diretto) {#direct-upload}

<!-- Courtney check me: Source PDF calls this "Upload to Cloud (Direct Upload)". Confirm heading wording. -->

Il caricamento diretto invia i file dal computer direttamente all’archiviazione cloud di Adobe, senza prima copiarli nella cartella Adobe Cloud Drive.

<!-- Courtney check me: Removed folder mentions from the Direct Upload section (intro, heading, step 1, 500-file bullet, hidden files bullet, and the Sync Activity link text), per Pulkit: folder support isn't available yet. Confirm nothing else should change. -->

### Caricare i file

1. Fare clic con il pulsante destro del mouse su un file nel Finder (Mac) o in Esplora file (Windows).
1. Seleziona **Carica nel cloud**.
1. Nel selettore di destinazione, seleziona una posizione all&#39;interno di uno dei progetti in Adobe Cloud Drive, quindi fai clic su **Carica qui**.
1. Monitora l&#39;avanzamento nella sezione **Caricamento diretto** della finestra Attività di sincronizzazione.

### Aspetti da considerare per il caricamento diretto

* Il caricamento diretto copia l’elemento nel cloud. L&#39;elemento originale rimane nella posizione corrente.
* Puoi selezionare più elementi da caricare contemporaneamente.
* La sezione Caricamento diretto elenca solo i singoli file, fino a un massimo di 500.
* È possibile caricare elementi dalla home directory utente o da qualsiasi unità esterna collegata. Altre posizioni di archiviazione cloud, come iCloud Drive o `~/Library/CloudStorage`, non sono supportate.
* Devi effettuare l&#39;accesso con un account Adobe abilitato. Non è necessaria una connessione Internet per avviare un caricamento. Senza una connessione, i caricamenti rimangono in coda.
* La sospensione della sincronizzazione annulla i caricamenti in corso. I caricamenti in coda vengono ripresi automaticamente quando si riprende la sincronizzazione.
* Se esci da Adobe Cloud Drive durante un caricamento, i caricamenti in corso vengono contrassegnati come annullati. I caricamenti in coda riprendono automaticamente al riavvio dell&#39;app.
* I file nascosti, i collegamenti simbolici e gli alias non sono supportati.
* Adobe Cloud Drive controlla quanti caricamenti vengono eseguiti contemporaneamente. I caricamenti rimanenti rimangono in coda finché non diventa disponibile uno slot.
* Viene visualizzato un conteggio live dei caricamenti, inclusi quelli non riusciti, ad esempio &quot;3 file in caricamento&quot;. Quando tutti i caricamenti vengono completati correttamente, il conteggio cambia in un riepilogo come &quot;3 file caricati&quot;. Seleziona **Ignora** per rimuoverlo.

<!-- Courtney check me: "Pausing sync cancels uploads in progress" and the quit behavior are from the PDF. Confirm with dev that both are intended. -->

### Stato caricamento

<!-- Courtney check me: Icons extracted from the PDF (48x48 px, low resolution) and named by table order. Verify each icon matches its status and ask Pulkit's team for higher-resolution originals. Add alt text review too. -->

| Icona | Stato | Descrizione | Azioni disponibili |
| --- | --- | --- | --- |
| ![Icona in coda](assets/acd-upload-status-queued.png) | In coda | Il caricamento è in attesa di inizio. | **Annulla** annulla questo elemento. |
| ![Icona caricamento](assets/acd-upload-status-uploading.png) | Caricamento | Caricamento in corso. | **Annulla** annulla questo elemento. |
| ![Icona Completato](assets/acd-upload-status-completed.png) | Completato | Caricamento completato. | **Apri in Workfront** apre la risorsa nell&#39;interfaccia Web di Workfront. |
| ![Icona non riuscita](assets/acd-upload-status-failed.png) | Non riuscito | Impossibile completare il caricamento. | **Mostra file di origine** rivela il file originale. **Riprova** ritenta il caricamento. Il nuovo tentativo è disponibile solo per alcuni errori. |
| ![Icona annullata](assets/acd-upload-status-cancelled.png) | Annullato | Il caricamento è stato interrotto da te o dal sistema. | Nessuno. I caricamenti annullati non vengono ritentati. Devi avviare un nuovo caricamento. |

Per visualizzare il motivo di un errore, passa il cursore sull’elemento non riuscito.

### Gestire l’elenco di caricamento

Ogni azione è disponibile solo quando applicabile.

* **Annulla tutti i caricamenti:** Disponibile quando i caricamenti sono in coda o in corso. Cancella tutti.
* **Nuovi tentativi di caricamento non riusciti:** Sono disponibili caricamenti non riusciti che è possibile ritentare. Tenta di eseguire tutte le operazioni. I caricamenti che non possono essere ritentati rimangono invariati.
* **Cancella:** disponibile quando non sono presenti caricamenti in coda o in corso. Rimuove tutti gli elementi completati, non riusciti e annullati. I file locali e il contenuto già caricato non sono interessati.
* **Cancellazione automatica:** gli elementi completati, non riusciti e annullati vengono rimossi automaticamente 24 ore dopo l&#39;ultimo aggiornamento. Gli elementi in coda e in corso non vengono mai rimossi automaticamente.

## Sospendi e riprendi sincronizzazione {#pause-resume-sync}

È possibile mettere in pausa Adobe Cloud Drive quando non si desidera caricare o scaricare file, ad esempio con una connessione Internet lenta o a consumo. Quando la sincronizzazione è in pausa, le modifiche non vengono inviate al cloud e le modifiche dal cloud non vengono scaricate nel computer. La sincronizzazione rimane in pausa fino a quando non viene ripresa.

### Sospendi sincronizzazione

1. Fai clic sull’icona Adobe Cloud Drive nella barra delle applicazioni (Windows) o nella barra dei menu (Mac).
1. Fai clic sull&#39;icona **Menu** (≡) nell&#39;angolo in alto a destra della finestra di Adobe Cloud Drive.
1. Selezionare **Sospendi sincronizzazione**.

   >[!TIP]
   >
   >Con la finestra Adobe Cloud Drive aperta, puoi anche premere Ctrl+P (Windows) o Comando+P (Mac).

   Nella finestra di Adobe Cloud Drive viene visualizzato **Sincronizzazione sospesa** e il messaggio **I file non verranno sincronizzati fino alla ripresa**. Quando passi il cursore sull&#39;icona Adobe Cloud Drive, viene visualizzato **Adobe Cloud Drive (in pausa)**.

>[!NOTE]
>
>Sospendi sincronizzazione è disponibile solo quando hai effettuato l’accesso e Adobe Cloud Drive è connesso.

### Riprendi sincronizzazione

1. Fai clic sull’icona Adobe Cloud Drive nella barra delle applicazioni (Windows) o nella barra dei menu (Mac).
1. Esegui una delle operazioni seguenti:

   * Fare clic su **Riprendi**.
   * Fai clic sull&#39;icona **Menu** (≡), quindi seleziona **Riprendi sincronizzazione**. Con la finestra aperta, è anche possibile premere Ctrl+R (Windows) o Comando+R (Mac).

   Adobe Cloud Drive riavvia la sincronizzazione, incluse eventuali modifiche apportate durante la sospensione della sincronizzazione.

## Visualizzare e gestire la cronologia delle versioni {#version-history}

È possibile utilizzare Cronologia versioni in Adobe Cloud Drive per sfogliare le versioni salvate di un file supportato nel cloud, visualizzare i dettagli e le miniature delle versioni e ripristinare una versione precedente. Se disponi delle autorizzazioni necessarie, puoi anche modificare il nome e la descrizione di una versione.

### Visualizza cronologia versioni

1. Vai alla cartella Adobe Cloud Drive nel Finder o in Esplora file.
1. Seleziona un file supportato.
1. Fare clic con il pulsante destro del mouse sul file e selezionare **Cronologia versioni**.
1. Seleziona una versione per visualizzarne i dettagli e la miniatura disponibili.

   Se il file non contiene versioni precedenti, **Non sono presenti versioni precedenti**. Le miniature potrebbero non essere disponibili per tutti i file o le versioni.

### Modifica informazioni versione

1. Apri Cronologia versioni per il file.
1. Seleziona la versione da aggiornare.
1. Apri il menu delle opzioni della versione e seleziona **Modifica informazioni sulla versione**.
1. Immettere un nome di **versione** o una **descrizione**.
1. Seleziona **Salva**.

   Le informazioni aggiornate vengono salvate e visualizzate quando si riapre Cronologia versioni.

### Ripristina una versione precedente

1. Apri Cronologia versioni per il file.
1. Seleziona la versione da ripristinare.
1. Selezionare **Ripristina questa versione**, se disponibile.
1. Attendere il completamento della sincronizzazione.
1. Riapri il file per verificare che il contenuto della versione selezionata sia ora corrente.

## Gestione archiviazione locale {#manage-local-storage}

È possibile utilizzare Gestione archiviazione locale in Adobe Cloud Drive per monitorare l&#39;utilizzo del disco locale, impostare un limite di archiviazione e visualizzare i file contrassegnati come **Sempre su questo dispositivo**.

<!-- Courtney check me: PDF says "Always on this device" here but this article uses "Always Keep On This Device" for the right-click option. Confirm which label the UI shows in each place. -->

### Visualizzazione dell&#39;utilizzo dello storage locale

1. Seleziona l’icona Adobe Cloud Drive e apri il relativo menu delle opzioni.
1. Selezionare **Gestione archiviazione locale**.
1. Esaminare l&#39;utilizzo dello spazio di archiviazione corrente e l&#39;elenco dei file contrassegnati come **Sempre in questo dispositivo**.
1. Ordinare l&#39;elenco dei file in base a **Nome** o **Dimensione** per trovare file specifici.

### Modificare il limite di archiviazione locale

1. Apri **Gestisci archiviazione locale** dal menu delle opzioni di Adobe Cloud Drive.
1. Immetti il limite di archiviazione desiderato.
1. Seleziona **Salva** per applicare la modifica.

>[!NOTE]
>
>Quando si imposta il limite di archiviazione, assicurarsi che nel dispositivo sia disponibile spazio su disco sufficiente.

## Visualizza attività di sincronizzazione {#sync-activity}

L’attività di sincronizzazione mostra un’attività recente tra la cartella Adobe Cloud Drive sul computer e l’archiviazione cloud Adobe. Utilizzala per monitorare caricamenti e download, esaminare le modifiche completate e identificare gli elementi che non sono stati sincronizzati.

### Visualizza attività di sincronizzazione

1. Seleziona l’icona Adobe Cloud Drive nella barra dei menu (Mac) o nell’area di notifica (Windows).
1. Espandi la sezione dell’attività di sincronizzazione utilizzando la freccia accanto al riepilogo dello stato.
1. Esamina le voci elencate e i relativi indicatori di stato. Passa il puntatore del mouse su un indicatore di stato per visualizzare l’avanzamento del trasferimento, l’operazione completata o un messaggio di errore.
1. Seleziona il menu Azioni accanto a un elemento per visualizzare le azioni disponibili per tale elemento.

### Informazioni sull’attività di sincronizzazione

* La sincronizzazione normale tiene traccia delle modifiche apportate tramite la cartella Adobe Cloud Drive, inclusi caricamenti, download, creazioni, ridenominazioni, spostamenti ed eliminazioni.
* L&#39;elenco di sincronizzazione normale contiene fino a 500 voci recenti. Le voci nuove o aggiornate vengono visualizzate nella parte superiore. Le voci meno recenti potrebbero essere rimosse quando l&#39;elenco raggiunge il limite.
* Una voce può inizialmente visualizzare **Preparazione in corso...** durante la risoluzione del nome o dei metadati.
* Nel riepilogo viene visualizzato il numero di elementi attualmente sincronizzati. **Sincronizzazione completata** indica che non sono attualmente attivi elementi. Analizzare l&#39;elenco per gli elementi non riusciti o esclusi, anziché considerare questo riepilogo come una conferma del completamento di ogni elemento.
* I file e le cartelle esclusi dalla sincronizzazione possono essere visualizzati con un errore che spiega il nome non supportato, il tipo non supportato o un altro motivo di esclusione.
* L&#39;attività viene cancellata alla disconnessione. L’elenco è una visualizzazione dell’attività, non una cronologia di controllo permanente.

### Stato sincronizzazione

<!-- Courtney check me: The PDF has two sync status tables (page 7 with 4 statuses, page 8 with 3 statuses and icons). I used the page 8 icons with the page 7 descriptions where they overlap. Confirm and decide whether to keep both tables. -->

| Icona | Stato | Descrizione | Azioni disponibili |
| --- | --- | --- | --- |
| Indicatore di attesa | In attesa di sincronizzazione | L&#39;elemento è in attesa dell&#39;inizio dell&#39;operazione. | **Mostra nel Finder** (Mac) o **Mostra in Explorer** (Windows), se applicabile. |
| ![Icona caricamento](assets/acd-sync-status-uploading.png) | Caricamento/Download | È in corso il trasferimento del contenuto del file. Passa il cursore del mouse sull’indicatore per vedere la direzione e la percentuale di trasferimento, se disponibili. Al 100%, la descrizione comando potrebbe mostrare **Finalizzazione in corso...** fino al completamento dell&#39;elaborazione. | **Mostra nel Finder** o **Mostra in Explorer**, se applicabile. |
| ![Icona Completato](assets/acd-sync-status-completed.png) | Operazione sincronizzata/completata | Operazione completata. La descrizione comando può identificare caricato, scaricato, creato, rinominato, rinominato nel cloud, spostato, eliminato o eliminato nel cloud. | **Mostra nel Finder** o **Mostra in Explorer** per gli elementi non eliminati. **Apri in Workfront** per gli elementi idonei completati, non eliminati. |
| ![Icona non riuscita](assets/acd-sync-status-failed.png) | Sincronizzazione non riuscita/esclusa | L&#39;elemento non può essere sincronizzato o è escluso dalla sincronizzazione. Passa il cursore del mouse sull’indicatore del motivo. | **Mostra nel Finder** o **Mostra in Explorer**, se applicabile. Risolvi il problema segnalato prima di prevedere la sincronizzazione dell’elemento. |

Gli elementi eliminati non possono essere rivelati localmente o aperti in Workfront dalla voce della loro attività.

### Gestire l’elenco delle attività

| Azione | Descrizione |
| --- | --- |
| Espandi o comprimi | Utilizzare la freccia accanto al riepilogo di sincronizzazione per mostrare o nascondere singole voci. |
| Mostra nel Finder / Mostra in Explorer | Individua un elemento non eliminato nella cartella Adobe Cloud Drive. |
| Apri in Workfront | Apri un elemento idoneo completato in Workfront nel browser. Questa azione non è disponibile per le voci di sincronizzazione normale attive, non riuscite o eliminate. |
| Cancella | Disponibile quando non sono attivi elementi di sincronizzazione normale. Cancella le voci completate, incluse quelle non riuscite, dalla vista attività. La cronologia di cancellazione non elimina i file locali o il contenuto cloud e non risolve un errore di sincronizzazione. |
| Ignora | Dopo aver cancellato un batch completato, potrebbe essere visualizzato un riepilogo degli elementi sincronizzati. Seleziona il relativo pulsante Chiudi per ignorare il riepilogo. |

>[!NOTE]
>
>Le righe con sincronizzazione normale non forniscono le azioni **Riprova** o **Annulla** per elemento utilizzate dal caricamento diretto. Per informazioni sul caricamento diretto, vedere [Caricamento di file nel cloud (caricamento diretto)](#direct-upload).

## Apri un elemento in Workfront {#open-in-workfront}

Apri in Workfront consente di passare da un elemento in Adobe Cloud Drive alla posizione corrispondente in Workfront nel browser. Utilizzalo per continuare a lavorare con l’elemento cloud in Workfront senza cercarlo manualmente.

### Aprire un elemento dal Finder o da Esplora file

1. Apri la cartella Adobe Cloud Drive nel Finder (Mac) o in Esplora file (Windows).
1. Selezionare un singolo file o una singola cartella associata a un elemento di Workfront.
1. Fare clic con il pulsante destro del mouse sull&#39;elemento e selezionare **Apri in Workfront**.

   Il browser apre la posizione Workfront corrispondente. Se richiesto, accedi con un account che abbia accesso a tale elemento.

### Apri un elemento dall’attività di sincronizzazione

1. Seleziona l’icona Adobe Cloud Drive nella barra dei menu (Mac) o nell’area di notifica (Windows).
1. Espandi la sezione dell’attività di sincronizzazione.
1. Per un elemento idoneo completato e non eliminato, aprire il menu Azioni aggiuntive e selezionare **Apri in Workfront**.
1. Per un file caricato tramite Caricamento diretto, utilizza la stessa azione nella voce completata nella sezione **Caricamento diretto**.

### Informazioni su Open in Workfront

* Selezionare un solo elemento alla volta. L&#39;apertura di più elementi selezionati in Workfront non è supportata.
* In Esplora file, il comando è nascosto per gli elementi esterni alla cartella Adobe Cloud Drive e per la directory principale dell&#39;unità stessa. Viene disattivato quando si selezionano più elementi.
* Un elemento deve avere una posizione Workfront corrispondente. Alcune cartelle o altri elementi potrebbero non avere una mappatura Workfront, anche se sono visibili in Adobe Cloud Drive.
* È possibile che un nuovo elemento locale non ancora caricato non disponga di un collegamento Workfront. Prima di riprovare, attendi il completamento del caricamento.
* Nella normale attività di sincronizzazione, l’azione viene offerta solo per le voci completate idonee. Non è disponibile per le voci attive, non riuscite o eliminate.
* In Caricamento diretto, l’azione è disponibile per i caricamenti completati, non per le voci in coda, caricate, non riuscite o annullate.
* Devi aver effettuato l&#39;accesso ad Adobe Cloud Drive. Workfront potrebbe anche richiedere di accedere separatamente nel browser e le autorizzazioni Workfront sono ancora valide.
* Per recuperare un collegamento non memorizzato nella cache e accedere a Workfront è necessaria una connessione Internet. Un collegamento risolto in precedenza non fornisce accesso offline a Workfront.
* Questa azione apre Workfront in un browser. Il file non viene aperto nell&#39;applicazione desktop, non viene caricata un&#39;altra copia né viene modificata la disponibilità offline locale.

### Apri in disponibilità Workfront

| Elemento o stato | Apri in Workfront, comportamento | Cosa fare |
| --- | --- | --- |
| Singolo elemento idoneo in Adobe Cloud Drive | Apre la posizione Workfront corrispondente. | Seleziona **Apri in Workfront**. |
| Più elementi selezionati | L’apertura di più elementi non è supportata. Esplora file disattiva il comando. | Seleziona un singolo elemento. |
| Nuovo elemento ancora in caricamento | Il collegamento Workfront potrebbe non essere ancora disponibile. | Attendi il completamento del caricamento, quindi riprova. |
| Voce di sincronizzazione normale completata | Disponibile quando l&#39;elemento è idoneo e non è stato eliminato. | Utilizzare il menu Azioni aggiuntive della voce. |
| Voce di caricamento diretto completata | Disponibile al termine del caricamento. | Utilizzare il menu Azioni aggiuntive della voce. |
| Elemento senza mappatura Workfront | Un messaggio indica che l&#39;elemento non è disponibile in Workfront. | Controlla l’elemento direttamente in Workfront o scegli un altro elemento supportato. |
| Voce normale sincronizzata eliminata | Azione non disponibile. | Utilizza direttamente Workfront se devi analizzare l’elemento eliminato. |

## Esci da Adobe Cloud Drive

Se si esce da Adobe Cloud Drive, l&#39;unità rimane visibile nel Finder o in Esplora file. Tuttavia, le modifiche apportate all&#39;interno dell&#39;unità durante la disconnessione e quelle non sincronizzate prima della disconnessione non vengono sincronizzate con il cloud.

Ciò che accade dopo dipende dall’account con cui effettui di nuovo l’accesso.

### Accedi di nuovo con lo stesso account

Adobe Cloud Drive conserva la cartella montata locale alla disconnessione. Se effettui nuovamente l’accesso con le stesse credenziali:

* Adobe Cloud Drive riutilizza automaticamente il montaggio esistente.
* Tutte le modifiche non sincronizzate apportate prima della disconnessione vengono mantenute e vengono sincronizzate una volta ripristinata la connessione.
* Non è richiesta alcuna azione da parte tua.

### Accedi con un altro account

Se effettui l’accesso con un altro account Adobe dopo la disconnessione:

* La cartella attualmente montata viene automaticamente rinominata e sottoposta a backup. Il nome della cartella di backup utilizza questo formato: `Adobe Cloud Drive <usermail>_<short_guid> (backup yyyy-MM-dd HH-mm-ss)`.
* Adobe Cloud Drive mappato al nuovo account diventa disponibile nel Finder o in Esplora file come di consueto.
* È possibile ripristinare manualmente qualsiasi lavoro non sincronizzato dalla cartella di backup prima di rimuoverlo.

>[!NOTE]
>
>Le cartelle di backup vengono salvate in `~/Library/CloudStorage` su Mac e in `C:\Users\<user>\` su Windows. Se cambi account più volte, vengono create più cartelle di backup con marca temporale. Esaminare e pulire periodicamente i backup per liberare spazio su disco.

## Risolvi conflitti di file

I conflitti possono verificarsi in una delle seguenti situazioni:

* Più utenti modificano o eliminano lo stesso file contemporaneamente.
* Un file viene modificato mentre è aperto da un altro utente.
* Le interruzioni di rete causano problemi di sincronizzazione.

### Come Adobe Cloud Drive risolve i conflitti

Adobe Cloud Drive utilizza una strategia di duplicazione per i conflitti:

* **Nessun blocco file.** Più utenti possono modificare i file contemporaneamente.
* **Duplicazione automatica.** Quando Adobe Cloud Drive rileva un conflitto, mantiene entrambe le versioni.
* **Cancella denominazione.** I file in conflitto includono il nome utente e la marca temporale in questo formato: `filename (Conflicted copy from username on date_time).extension`. Ad esempio: `hero-banner (Conflicted copy from John on 2026-02-10_16-06-44).psd`.

### Risolvere manualmente un conflitto

1. Identificare il file in conflitto. Il nome del file contiene la dicitura &quot;Copia in conflitto&quot;.
1. Rivedi entrambe le versioni per determinare quale è corretta.
1. Mantieni la versione corretta ed elimina l’altra versione.
1. Assegnare al file conservato un nome appropriato.

>[!TIP]
>
>Per ridurre al minimo i conflitti:
>
>* Controllare lo stato di sincronizzazione prima di modificare i file.
>* Comunicare con i membri del team su chi sta modificando i file.
>* Salva di frequente in modo che le modifiche vengano sincronizzate tempestivamente.
>* Chiudere i file al termine della modifica.
