---
content-type: reference
product-area: documents;workfront-integrations
navigation-topic: adobe-cloud-drive
title: Risolvere i problemi relativi a Adobe Cloud Drive
description: Rivedi limitazioni, considerazioni sulle prestazioni e soluzioni ai problemi più comuni con Adobe Cloud Drive su Mac e Windows.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 6ad89f8d00dd3a06eb160863c3213a9f80b1a44b
workflow-type: tm+mt
source-wordcount: 928
ht-degree: 0%

---

# Risolvere i problemi relativi a Adobe Cloud Drive

Questo articolo descrive le limitazioni di Adobe Cloud Drive, considerazioni sulle prestazioni da tenere presenti e soluzioni ai problemi comuni che potresti riscontrare.

Per informazioni sull&#39;utilizzo di Adobe Cloud Drive, vedi [Utilizzare Adobe Cloud Drive](/help/quicksilver/documents/adobe-cloud-drive/use-adobe-cloud-drive.md).

## Limitazioni

### Operazioni su file e cartelle

* Le cartelle di progetto sono di sola lettura al livello superiore. Non è possibile rinominarli, eliminarli o spostarli da Adobe Cloud Drive. Per creare, rinominare o eliminare un progetto, utilizza l’interfaccia web di Workfront.
* Le operazioni su file e cartelle all’interno di una cartella di progetto sono completamente supportate.

### Limiti di file e percorsi

* I nomi di file non possono superare i 255 caratteri su qualsiasi piattaforma.
* Il percorso completo del file (tutti i nomi delle cartelle più il nome del file) non può superare i 1024 caratteri. I file con percorsi più lunghi di questo limite non vengono visualizzati in Adobe Cloud Drive, anche se sono visibili nell’interfaccia web di Workfront.
* Se in un file viene visualizzato un errore **Percorso completo troppo lungo**, ridurre i nomi delle cartelle o la profondità di nidificazione delle cartelle per riportare il percorso entro il limite.

### Archiviazione

* I file salvati in Adobe Cloud Drive in locale utilizzano lo spazio su disco del dispositivo.
* I file solo cloud non utilizzano l’archiviazione locale.
* Rimuovere l&#39;accesso offline per i file non più necessari. Per ulteriori informazioni, vedere [Rimuovere l&#39;accesso offline per liberare spazio](/help/quicksilver/documents/adobe-cloud-drive/use-adobe-cloud-drive.md#remove-offline-access-to-free-up-space) in [Utilizzare Adobe Cloud Drive](/help/quicksilver/documents/adobe-cloud-drive/use-adobe-cloud-drive.md).

## Considerazioni sulle prestazioni

* **Dimensione file:** Il tempo necessario per la sincronizzazione dipende dalle dimensioni del file. I file più grandi in genere richiedono più tempo.
* **Velocità di rete:** connessioni più veloci offrono prestazioni di sincronizzazione migliori. La sincronizzazione riprende automaticamente dopo un&#39;interruzione.
* **Primo accesso:** i file vengono scaricati su richiesta la prima volta che si accede a tali file. L’accesso successivo è più veloce perché il file è memorizzato nella cache locale.

## Problemi comuni

### Adobe Cloud Drive non viene visualizzato

**Possibili cause:**

* Adobe Cloud Drive non è installato.
* Installazione non completata correttamente.
* La tua organizzazione non utilizza una versione di Workfront che supporta l’archiviazione cloud di Adobe.

**Soluzioni:**

* Verifica che Adobe Cloud Drive sia installato. Controllare **Applicazioni** (Mac) o **Programmi** (Windows).
* Avvia Adobe Cloud Drive manualmente.
* Contatta l’amministratore di Workfront per verificare che la tua organizzazione utilizzi una versione di Workfront che supporta l’archiviazione cloud di Adobe.
* Se necessario, reinstalla Adobe Cloud Drive. Per ulteriori informazioni, vedere [Installare Adobe Cloud Drive](/help/quicksilver/documents/adobe-cloud-drive/install-adobe-cloud-drive.md).

### L&#39;icona Adobe Cloud Drive non è visibile nella barra dei menu o nella barra delle applicazioni

**Possibili cause:**

* La barra dei menu (Mac) o l&#39;area di notifica (Windows) non dispone di spazio sufficiente per visualizzare l&#39;icona.

**Soluzioni:**

* **Mac:** tieni premuto Cmd e trascina le icone della barra dei menu esistenti per ridisporle o rimuoverle, creando spazio per l&#39;icona di Adobe Cloud Drive.
* **Windows:** Fare clic sulla freccia su (**Mostra icone nascoste**) nella barra delle applicazioni per trovare l&#39;icona di Adobe Cloud Drive, quindi trascinarla nell&#39;area visibile.

### I progetti non vengono visualizzati o mancano alcuni progetti

**Possibili cause:**

* Non hai accesso ad alcun progetto.
* Sincronizzazione non completata.
* Si è verificato un problema di connettività di rete.

**Soluzioni:**

* Verifica l’accesso al progetto nell’interfaccia web di Workfront.
* Verifica la connessione di rete.
* Esci da Adobe Cloud Drive e accedi di nuovo.

### I file non vengono sincronizzati

**Possibili cause:**

* Si è verificato un problema di connettività di rete.
* Errore di sincronizzazione nel file o nella cartella.
* Spazio su disco insufficiente.

**Soluzioni:**

* Controlla la tua connessione Internet.
* Verificare che lo spazio su disco sia sufficiente.
* Verificare la presenza di errori di sincronizzazione negli indicatori di stato del file. Per ulteriori informazioni, vedere [Indicatori di stato dei file](/help/quicksilver/documents/adobe-cloud-drive/use-adobe-cloud-drive.md#file-status-indicators) in [Utilizzare Adobe Cloud Drive](/help/quicksilver/documents/adobe-cloud-drive/use-adobe-cloud-drive.md).
* Riavvia Adobe Cloud Drive.
* Controlla lo stato di Adobe Cloud Drive nella barra delle applicazioni (Windows) o nella barra dei menu (Mac).

### Impossibile aprire un file

**Possibili cause:**

* Il file è solo cloud e il download non è riuscito.
* L&#39;applicazione necessaria per aprire il file non è installata.
* Il file è danneggiato.

**Soluzioni:**

* Controllare l&#39;indicatore di stato del file.
* Verificare che l&#39;applicazione richiesta sia installata.
* Fare clic con il pulsante destro del mouse sul file, selezionare **Mantieni sempre il dispositivo**, quindi riprovare ad aprirlo.
* Verificare che il file non sia danneggiato nell&#39;interfaccia Web di Workfront.

### Sincronizzazione lenta

**Possibili cause:**

* Il file è grande.
* Connessione di rete lenta.
* Molti file vengono sincronizzati contemporaneamente.

**Soluzioni:**

* Siate pazienti con file di grandi dimensioni. La sincronizzazione è ripristinabile, quindi riprende da dove si è interrotta dopo un’interruzione.
* Controllare la velocità di rete.
* Limita il numero di operazioni simultanee sui file.
* Mantieni i file di grandi dimensioni solo nel cloud, a meno che non sia necessario l’accesso offline.

### Lo spazio occupato dai file non in linea è eccessivo

**Soluzioni:**

* Fare clic con il pulsante destro del mouse su file non in linea e selezionare **Spazio disponibile**.
* Controllare regolarmente lo spazio su disco.
* Mantieni i file di grandi dimensioni a cui accedi raramente in modalità solo cloud.

### Impossibile creare, modificare o eliminare file o cartelle

**Possibili cause:**

* Si sta tentando di creare, rinominare o eliminare una cartella di progetto. Le cartelle di progetto sono di sola lettura al livello superiore.
* Il progetto è di sola lettura, pertanto non è possibile creare, modificare o eliminare file o cartelle al suo interno.

**Soluzioni:**

* Per creare, rinominare o eliminare un progetto, utilizza l’interfaccia web di Workfront.
* Chiedi al proprietario del progetto di condividerlo con te con l’accesso di modifica.

## Ottieni aiuto

Per domande sulla licenza, problemi di accesso al progetto o configurazione specifica dell’organizzazione, contatta l’amministratore Workfront.

Per condividere i registri con il supporto di Adobe, segui i passaggi descritti in [Eseguire lo strumento Raccolta registri di Adobe](https://helpx.adobe.com/it/creative-cloud/apps/troubleshoot/diagnostics-repair-tools/run-log-collector-tool.html).

## Best practice

* **Pianifica lavoro offline.** Scarica i file prima di viaggiare o lavorare in aree con scarsa connettività.
* **Monitoraggio dello stato di sincronizzazione.** Controllare gli indicatori dei file prima di chiudere le applicazioni.
* **Segui la struttura di cartelle del progetto.** Organizza i file all’interno delle cartelle di progetto secondo le intenzioni del proprietario del progetto.
* **Utilizzare nomi di file descrittivi.** Aiutare i membri del team a trovare ciò di cui hanno bisogno.
* **Evita di creare duplicati.** Non creare copie non necessarie dei file.
