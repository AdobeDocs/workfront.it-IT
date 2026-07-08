---
product-area: documents;workfront-integrations
navigation-topic: adobe-cloud-drive
title: Usa Adobe Cloud Drive
description: Lavora con i tuoi progetti di archiviazione cloud Adobe direttamente da Finder o Esplora file utilizzando Adobe Cloud Drive. Aprire e modificare i file in qualsiasi applicazione, lavorare offline e risolvere i conflitti.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: d5dd769447e81d5d95b4907f8a01016b118f2322
workflow-type: tm+mt
source-wordcount: 1723
ht-degree: 2%

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
