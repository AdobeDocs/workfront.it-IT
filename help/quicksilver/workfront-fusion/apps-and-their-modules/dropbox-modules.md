---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli di Dropbox
description: In una [!DNL Adobe Workfront Fusion] è possibile automatizzare i flussi di lavoro che utilizzano il Dropbox, nonché collegarli a più applicazioni e servizi di terze parti.Questo consente di automatizzare attività quali monitoraggio, ricerca, recupero, inserimento, creazione e modifica di file e cartelle nel Dropbox.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: a35631d7-40ac-4e7f-9a37-ad3879c0b6a2
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '3013'
ht-degree: 0%

---

# [!DNL Dropbox] moduli

In un [!DNL Adobe Workfront Fusion] puoi automatizzare i flussi di lavoro che utilizzano [!UICONTROL Dropbox], nonché collegarlo a più applicazioni e servizi di terze parti.Questo consente di automatizzare attività come il monitoraggio, la ricerca, il recupero, l&#39;elenco, la creazione e la modifica di file e cartelle nel [!UICONTROL Dropbox].

Se hai bisogno di istruzioni su come creare uno scenario, vedi [Crea uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Per informazioni sui moduli, consulta [Moduli in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Requisiti di accesso

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td>
  <td> <p>[!UICONTROL Pro] o superiore</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licenza**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</td> 
  </tr> 
 </tbody> 
</table>

Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, vedi [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Prerequisiti

Per utilizzare [!DNL Dropbox] moduli, è necessario disporre di un [!DNL Dropbox] conto.

## [!DNL Dropbox] moduli e relativi campi

Quando si configura [!DNL Dropbox] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL Dropbox] potrebbero essere visualizzati, a seconda di fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se trovi il pulsante mappa sopra un campo o una funzione, puoi utilizzarlo per impostare variabili e funzioni per quel campo. Per ulteriori informazioni, consulta [Mappare informazioni da un modulo a un altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Moduli trigger](#trigger-modules)
* [Moduli per ottenere [!DNL Dropbox] file e cartelle](#modules-for-getting-dropbox-files-and-folders)
* [Moduli per la creazione e la modifica [!DNL Dropbox] file e cartelle](#modules-for-creating-and-editing-dropbox-files-and-folders)
* [Altri moduli](#other-modules)

### Moduli trigger

#### [!UICONTROL File di controllo]

Questo modulo di tipo Trigger restituisce i dettagli del file quando viene modificato il file in una cartella specificata.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Dropbox] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cartella] </td> 
   <td> <p>Seleziona la cartella da controllare per le modifiche.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch anche sottocartelle]</td> 
   <td> <p> Abilita questa opzione anche per monitorare le sottocartelle nella cartella selezionata per i file modificati.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit] </td> 
   <td> <p>Immettere o mappare il numero massimo di record che si desidera restituire dal modulo durante ogni ciclo di esecuzione degli scenari.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Moduli per ottenere [!DNL Dropbox] file e cartelle

* [[!UICONTROL Cerca file/cartelle]](#search-filesfolders)
* [[!UICONTROL Scaricare un file]](#download-a-file)
* [[!UICONTROL Ottieni metadati cartella]](#get-a-folder-metadata)
* [[!UICONTROL Elencare tutti i file/sottocartelle in una cartella]](#list-all-filessubfolders-in-a-folder)
* [[!UICONTROL Elenco revisioni dei file]](#list-file-revisions)

#### [!UICONTROL Cerca file/cartelle]

Questo modulo di ricerca cerca i record in un oggetto in [!DNL Dropbox] che corrispondono alla query di ricerca specificata.

Puoi mappare queste informazioni nei moduli successivi nello scenario .

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Dropbox] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Search] </td> 
   <td> <p>Inserisci il termine di ricerca.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cartella] </td> 
   <td> <p>Selezionare la cartella da cercare. Questo modulo cerca l'intero [!DNL Dropbox] se non si seleziona una cartella.</p> </td> 
  </tr> 
  <tr> 
   <td>Stato del file</td> 
   <td> <p> Selezionare lo stato del file per limitare la ricerca allo stato del file selezionato.</p> </td> 
  </tr> 
  <tr> 
   <td>Categorie di file</td> 
   <td> <p> Selezionare le categorie di file per limitare la ricerca alle categorie selezionate.</p> </td> 
  </tr> 
  <tr> 
   <td>Estensioni file</td> 
   <td> <p> Scegli le estensioni di file da cercare.</p> </td> 
  </tr> 
  <tr> 
   <td>Limite </td> 
   <td> <p>Immettere o mappare il numero massimo di record che si desidera restituire dal modulo durante ogni ciclo di esecuzione degli scenari.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Scaricare un file]

Questo modulo di azione scarica un file da una cartella.

Specificare il file e la relativa posizione.

Il modulo restituisce l’ID del file e di tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

>[!NOTE]
>
>Questo modulo è utile per fornire file ai moduli successivi.

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Dropbox] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>Modalità di selezione dei file</td> 
   <td> <p> Seleziona se mappare il percorso del file o se selezionare manualmente il file.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Percorso file / File</p> </td> 
   <td> <p style="font-weight: bold;">Percorso file</p> <p>Immetti o mappa il percorso di destinazione del file.</p> <p style="font-weight: bold;">File</p> <p>Selezionare il file dal menu.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottieni metadati cartella]

Questo modulo di azione recupera i dettagli della cartella condivisa.

Specifica l’ID della cartella.

Il modulo restituisce l’ID della cartella e di tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Dropbox] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>ID cartella condivisa</td> 
   <td> <p> Immetti o mappa l’ID della cartella di cui desideri recuperare i dettagli.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Elencare tutti i file/sottocartelle in una cartella]

Questo modulo di azione elenca i file o le cartelle in una particolare cartella.

Specifica l’ID della cartella.

Il modulo restituisce gli ID dei file o delle cartelle e di tutti i campi associati, nonché tutti i campi e i valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Dropbox] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>Lista </td> 
   <td> <p>Selezionare se si desidera recuperare file o cartelle.</p> </td> 
  </tr> 
  <tr> 
   <td>Mostra solo file scaricabili</td> 
   <td> <p> Abilita questa opzione per restituire solo i file scaricabili. Alcuni tipi di file, come i documenti Google, non sono scaricabili.</p> </td> 
  </tr> 
  <tr> 
   <td>Cartella </td> 
   <td> <p>Immettere o mappare la cartella da cui si desidera recuperare i file o le cartelle.</p> </td> 
  </tr> 
  <tr> 
   <td>Limite </td> 
   <td> <p>Immettere o mappare il numero massimo di record che si desidera elencare nel modulo durante ogni ciclo di esecuzione degli scenari.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Elenco revisioni dei file]

Questo modulo di azione recupera tutte le revisioni dei file (una cronologia delle versioni) di un particolare file.\
Specifica l’ID del file.

Il modulo restituisce tutti i campi standard associati al record, insieme a eventuali campi e valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Dropbox] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>Modalità di selezione dei file</td> 
   <td> <p> Seleziona se mappare il percorso del file o se selezionare manualmente il file.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Percorso file / File</p> </td> 
   <td> <p style="font-weight: bold;">Percorso file</p> <p>Immetti o mappa il percorso di destinazione del file.</p> <p style="font-weight: bold;">File</p> <p>Selezionare il file dal menu.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Limite</p> </td> 
   <td> <p>Immettere o mappare il numero massimo di record che si desidera elencare nel modulo durante ogni ciclo di esecuzione degli scenari.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Moduli per la creazione e la modifica [!DNL Dropbox] file e cartelle

* [[!UICONTROL Carica] un file](#upload-a-file)
* [[!UICONTROL Creare una cartella]](#create-a-folder)
* [[!UICONTROL Creare/sovrascrivere un file di testo]](#createoverwrite-a-text-file)
* [[!UICONTROL Creare/aggiornare un collegamento di condivisione]](#createupdate-a-share-link)
* [[!UICONTROL Ripristino di un file]](#restore-a-file)
* [[!UICONTROL Spostare un file o una cartella]](#move-a-filefolder)
* [[!UICONTROL Rinomina un file/cartella]](#rename-a-filefolder)
* [[!UICONTROL Eliminare un file/cartella]](#delete-a-filefolder)

#### [!UICONTROL Caricare un file]

Questo modulo di azione carica un file in una cartella.

Puoi specificare informazioni quali la posizione del file, il file da caricare e un nuovo nome facoltativo per il file.

Il modulo restituisce l’ID del file e di tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Dropbox] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cartella]</td> 
   <td> <p> Seleziona la cartella della [!DNL Dropbox] vuoi caricare il file in .</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL File di origine]</p> </td> 
   <td> <p>Immetti o mappa il file che desideri aggiungere al [!DNL Dropbox] cartella selezionata sopra.</p> <p style="font-weight: bold;">[!UICONTROL File name]</p> <p>Immetti o mappa il nome del file, inclusa l’estensione del file.</p> <p style="font-weight: bold;">[!UICONTROL File data]</p> <p>Immetti o mappa i dati del file (dal modulo precedente come [!UICONTROL Google Drive] &gt;[!UICONTROL Get a File)].</p> <p>Nota: La dimensione massima del file caricato è 150 MB.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sovrascrivi un file esistente]</td> 
   <td> <p> Abilita questa opzione per sostituire il file esistente con il nuovo file. Se questa opzione viene lasciata disabilitata, il file caricato viene rinominato.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Creare una cartella]

Questo modulo di azione crea una nuova cartella.

Specificare il percorso e un nome per la cartella.

Il modulo restituisce l’ID della cartella e di tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Dropbox] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome cartella] </td> 
   <td> <p>Immettere il nome della nuova cartella.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Cartella]</p> </td> 
   <td> <p>Immettere o mappare il percorso in cui si desidera creare una nuova cartella.</p> <p>Nota:   <p>Se utilizzi un [!DNL Dropbox Business] account (con spazi del team), è necessario rimuovere la barra <code>/</code>o non fare clic su <strong>[!UICONTROL Fai clic qui per scegliere la cartella</strong> per creare una cartella team nella directory principale.</p> <p>Se la barra non viene rimossa, viene visualizzato un errore <code>[409] path/malformed_path/..</code> viene restituito .</p> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Rinomina automatica]</td> 
   <td> <p> Se nel percorso di destinazione esiste già una cartella con lo stesso nome, abilitare questa opzione per rinominare la nuova cartella.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Creare/sovrascrivere un file di testo]

Questo modulo di azione crea un file DOC o sovrascrive il contenuto di un file esistente.

Specificare il file di origine e la cartella.

Il modulo restituisce l’ID della cartella e di tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Dropbox] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Seleziona per]</td> 
   <td> <p> Selezionare se si desidera creare o sovrascrivere un file DOC.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cartella] </td> 
   <td> <p>Selezionare la posizione di destinazione in cui si desidera creare un file.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL File di origine]</p> </td> 
   <td> <p>Immetti o mappa il file che desideri aggiungere al [!DNL Dropbox] cartella.</p> <p style="font-weight: bold;">Nome file</p> <p>Immettere il nome del file per il nuovo file DOC (senza estensione).</p> <p style="font-weight: bold;">Contenuto del file</p> <p>Immettere il contenuto testuale del file DOC.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Creare/aggiornare un collegamento di condivisione]

Questo modulo di azione crea un collegamento pubblico a un file.

Puoi specificare il file e le informazioni sul collegamento.

Il modulo restituisce l’ID del collegamento e di tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Dropbox] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Modalità di selezione dei file]</td> 
   <td> <p> Seleziona se mappare o immettere il percorso del file oppure seleziona manualmente il file.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL File Path / File]</p> </td> 
   <td> <p style="font-weight: bold;">[!UICONTROL File Path]</p> <p>Immetti o mappa il percorso di destinazione del file.</p> <p style="font-weight: bold;">[!UICONTROL File]</p> <p>Selezionare il file dal menu.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Visibilità richiesta]</p> </td> 
   <td> <p>Seleziona se il collegamento è pubblico, per il team o se la password è limitata.</p> <p>Nota: Le opzioni [!UICONTROL Team only] e [!UICONTROL Access with password] sono disponibili solo per gli utenti che hanno [!DNL Dropbox Pro] o versione successiva.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data di scadenza del collegamento]</td> 
   <td> <p> Immetti la data e l’ora in cui il collegamento scade e non sarà più accessibile. Se questo campo viene lasciato vuoto, il collegamento non scade. Per un elenco dei formati di data e ora supportati, consulta <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref" data-mc-variable-override="">Tipo di coercizione in [!DNL Adobe Workfront Fusion]</a>.</p> <p>Nota: Le opzioni [!UICONTROL Team] e [!UICONTROL Access with password] sono disponibili solo per gli utenti che dispongono di [!UICONTROL Dropbox Pro] o versioni successive.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Livello di accesso del collegamento</p> </td> 
   <td> <p>Imposta l'autorizzazione per il destinatario del collegamento.</p> <p><strong>[!UICONTROL Viewer]</strong> Gli utenti che utilizzano il collegamento possono visualizzare e commentare il contenuto.</p> <p><strong>[!UICONTROL Editor]</strong> Gli utenti che utilizzano il collegamento possono modificare, visualizzare e commentare il contenuto.</p> <p><strong>[!UICONTROL Max]</strong> Gli utenti che utilizzano il collegamento ricevono il livello di accesso massimo a cui puoi impostare il collegamento.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ripristino di un file]

Questo modulo di azione ripristina una versione precedente di un file.

Specificare il file e il numero della revisione desiderata.

Il modulo restituisce l’ID della versione e di tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Dropbox] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Modalità di selezione dei file]</td> 
   <td> <p> Seleziona se mappare o immettere il percorso del file oppure seleziona manualmente il file.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL File Path] / [!UICONTROL File]</p> </td> 
   <td> <p><strong>[!UICONTROL File Path]</strong> </p> <p>Immetti o mappa il percorso di destinazione del file.</p> <p><strong>[!UICONTROL File]</strong> </p> <p>Selezionare il file dal menu.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Revision]</p> </td> 
   <td> <p>Immettere o mappare il numero di revisione della revisione che si desidera ripristinare.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Spostare un file o una cartella]

Questo modulo di azione sposta un file o una cartella in un percorso diverso.

È possibile specificare il file o la cartella, nonché come e dove spostarlo.

Il modulo restituisce l’ID del file o della cartella e di tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Dropbox] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Modalità di selezione dei file] </td> 
   <td> <p>Seleziona se mappare o immettere il percorso del file oppure seleziona manualmente il file.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Percorso file/cartella] / [!UICONTROL File/Cartella]</p> </td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Percorso file/cartella]</p> <p>Immettere o mappare il percorso di destinazione al file o alla cartella.</p> <p style="font-weight: bold;">[!UICONTROL File/Cartella]</p> <p>Selezionare il file o la cartella dal menu.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL To Folder]</p> </td> 
   <td> <p>Immettere o mappare la posizione di destinazione del file o della cartella.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Nuovo Nome]</p> </td> 
   <td> <p>Immettere il nuovo nome del file o della cartella nella nuova posizione.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Auto Rinomina]</p> </td> 
   <td> <p>Abilita questa opzione per assicurarti che se esiste un file o una cartella con lo stesso nome, il modulo rinomini il nuovo file o la nuova cartella aggiungendo ([!UICONTROL NUMBER]) dopo il nome del file o della cartella. In caso contrario, il file o la cartella nella posizione di destinazione viene sovrascritto.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Consenti trasferimento proprietà]</p> </td> 
   <td> <p>Abilita questa opzione per consentire gli spostamenti in base al proprietario, anche se comporterebbe un trasferimento di proprietà per il contenuto in corso di spostamento.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Rinomina un file/cartella]

Questo modulo di azione rinomina un file o una cartella.

Specificare il file o la cartella e il nuovo nome.

Il modulo restituisce l’ID del file o della cartella e di tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Dropbox] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>Modalità di selezione dei file</td> 
   <td> <p> Seleziona se mappare o immettere il percorso del file oppure seleziona manualmente il file.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Percorso file/cartella / File/Cartella</p> </td> 
   <td> <p style="font-weight: bold;">Percorso file/cartella</p> <p>Immettere o mappare il percorso di destinazione al file o alla cartella.</p> <p style="font-weight: bold;">File/Cartella</p> <p>Selezionare il file o la cartella dal menu.</p> </td> 
  </tr> 
  <tr> 
   <td>Rinomina </td> 
   <td> <p>Immetti il [!UICONTROL target name] per il file, inclusa l'estensione del file.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminare un file/cartella]

Questo modulo di azione elimina un file o una cartella.

Specificare il file o la cartella.

Il modulo restituisce l’ID del record e di tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Dropbox] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Modalità di selezione dei file]</td> 
   <td> <p> Seleziona se mappare o immettere il percorso del file oppure seleziona manualmente il file.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL File Path] / [!UICONTROL File]</p> </td> 
   <td> <p style="font-weight: bold;">[!UICONTROL File Path]</p> <p>Immetti o mappa il percorso di destinazione del file.</p> <p style="font-weight: bold;">[!UICONTROL File]</p> <p>Selezionare il file dal menu.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Altri moduli

#### [!UICONTROL Effettuare una chiamata API]

Questo modulo di azione ti consente di effettuare una chiamata autenticata personalizzata al [!DNL Dropbox] API. In questo modo, puoi creare un’automazione del flusso di dati che non può essere eseguita dall’altro [!DNL Dropbox] moduli.

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Dropbox] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Immettere un percorso relativo a Immettere un percorso relativo a <code>https://api.dropboxapi.com</code>. Ad esempio: <code>/2/files/list_folder</code></p> <p>Nota: Per l’elenco degli endpoint disponibili, consulta <a href="https://www.dropbox.com/developers/documentation/http/documentation">Documentazione API di Dropbox v2</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL, Metodo]</p> </td> 
   <td> <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Headers] </td> 
   <td> <p>Immetti le intestazioni di richiesta desiderate. [!DNL Workfront Fusion] aggiunge automaticamente le intestazioni di autorizzazione.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Query String]</td> 
   <td> <p> Immetti la stringa di query della richiesta.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Body] </td> 
   <td> <p>Aggiungi il contenuto del corpo per la chiamata API sotto forma di un oggetto JSON standard.</p> <p>Nota:   <p>Quando si utilizzano istruzioni condizionali come <code>if</code> nel JSON, inserisci le virgolette al di fuori dell’istruzione condizionale.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Esempio:** La seguente chiamata API restituisce i primi 10 file dal [!DNL /Text files] nella cartella [!DNL Dropbox] account:
>
>URL: `/2/files/list_folder`
>
>Corpo:
> 
>`{`
>
>`"path": "/Text files",`
>
>`"limit": 10,`
>
>`"recursive": false,`
>
>`"include_deleted": false`
>
>`}`
>
>Le corrispondenze della ricerca si trovano nell&#39;Output del modulo in [!UICONTROL Bundle] > [!UICONTROL Corpo] > voci.
>
>Nel nostro esempio, sono stati restituiti 10 biglietti:

## Problemi comuni

* [Impossibile caricare o aggiornare un file](#unable-to-upload-or-update-a-file)
* [Il rendering dell&#39;immagine a cui si fa riferimento tramite un collegamento condiviso non viene eseguito](#image-referenced-via-a-shared-link-does-not-render)

### Impossibile caricare o aggiornare un file

Ci sono diverse situazioni in cui il caricamento o l’aggiornamento di un file non riesce:

* Il file caricato è troppo grande e supera la dimensione massima consentita per il tuo [!DNL Dropbox] o hai utilizzato tutti i tuoi [!DNL Dropbox] quota di archiviazione dell&#39;account. È necessario eliminare i file esistenti dal [!DNL Dropbox] account o aggiornamento del piano.
* La cartella selezionata in precedenza in cui viene caricato il file non esiste più. Lo scenario si arresta e devi selezionare nuovamente la cartella di destinazione.

### Il rendering dell&#39;immagine a cui si fa riferimento tramite un collegamento condiviso non viene eseguito

L’URL restituito da [!UICONTROL Dropbox] >[!UICONTROL Creare un collegamento condiviso] non si collega direttamente a un’immagine, ma a un [!DNL Dropbox] pagina. Per forzare il download dell&#39;immagine, sostituisci la versione finale `?dl=0` con `?dl=1`. Per forzare il rendering dell’immagine (ad esempio, in un browser Web o in Facebook Messenger), aggiungi `&raw=1` all’URL.

Se devi ottenere il collegamento diretto o non elaborato dell’immagine per il tuo sito web o per altri [!DNL Workfront Fusion] moduli, devi modificare l’URL condiviso iniziale nel modo seguente:

URL originale:

`https://www.dropbox.com/s/ia8qtvs20f3a5ux/Screen%20Shot%202018-10-15%20at%204.21.11%20PM.png?dl=0`

1. Sostituisci `www` con `dl`.
1. Rimuovi `?dl=0`.

URL finale:

`https://dl.dropbox.com/s/ia8qtvs20f3a5ux/Screen%20Shot%202018-10-15%20at%204.21.11%20PM.png`

Per modificare automaticamente l’URL, puoi utilizzare la funzione `replace()` due volte:

* Sostituisci www con dl

   ![](assets/www-to-dl-350x32.png)

* E rimuovere ?dl=0

   ![](assets/remove-dl0-350x33.png)

Per eseguire questa operazione in un unico passaggio, combina le seguenti funzioni:

![](assets/replace-both-350x47.png)

Puoi anche copiarlo e incollarlo nel campo . Sostituisci `1.url` con l’URL.

```
{{replace(replace(1.url; "?dl=0"; ""); "www"; "dl")}}
```
