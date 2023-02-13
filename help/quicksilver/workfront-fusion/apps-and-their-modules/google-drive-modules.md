---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli unità Google
description: La [!DNL Adobe Workfront Fusion Google Drive] I moduli consentono di monitorare, cercare, creare, aggiornare, eliminare e gestire i file, le cartelle o le unità condivise all'interno dell'utente [!DNL Google Drive].
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 7d620c93-d1bf-4451-9f76-1d6fd850cec9
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2908'
ht-degree: 0%

---

# [!DNL Google Drive] moduli

La [!DNL Adobe Workfront Fusion] [!DNL Google Drive] I moduli consentono di monitorare, cercare, creare, aggiornare, eliminare e gestire i file, le cartelle o le unità condivise all&#39;interno dell&#39;utente [!DNL Google Drive].

In una [!DNL Adobe Workfront Fusion] in uno scenario, è possibile collegare [!DNL Google Drive] account a più applicazioni e servizi di terze parti.

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



## Collegamento [!DNL Google Drive] a [!DNL Workfront Fusion]

Se sei [!DNL @gmail.com] o [!DNL @googlemail.com] utente necessario creare un client OAuth su [la [!DNL Google Cloud Platform]](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) per ottenere [!UICONTROL ID client] e [!UICONTROL Segreto client].

Per istruzioni dettagliate su come creare il client OAuth (e ottenere [!UICONTROL ID client] e [!UICONTROL Segreto client]), vedi [Connetti [!DNL Adobe Workfront Fusion] a [!DNL Google Services] utilizzo di un client OAuth personalizzato](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

Per istruzioni su come collegare le [!DNL Google Drive] account a [!UICONTROL Workfront Fusion], vedi [Creare una connessione a [!UICONTROL Adobe Workfront Fusion] - Istruzioni di base](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!DNL Google Drive] moduli e relativi campi

Quando si configura [!DNL Google Drive] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL Google Drive] potrebbero essere visualizzati, a seconda di fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se trovi il pulsante mappa sopra un campo o una funzione, puoi utilizzarlo per impostare variabili e funzioni per quel campo. Per ulteriori informazioni, consulta [Mappare informazioni da un modulo a un altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)



* [Triggers](#triggers)
* [Azioni](#actions)

### Triggers

* [[!UICONTROL Guarda i file nella cartella]](#watch-files-in-folder)
* [[!UICONTROL Guarda tutti i file]](#watch-all-files)
* [[!UICONTROL Guarda i file condivisi]](#watch-shared-files)
* [[!UICONTROL Osserva commenti]](#watch-comments)

#### [!UICONTROL Guarda i file nella cartella]

Recupera i dettagli del file quando un file viene aggiunto o modificato nella cartella specificata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Connection] </td>
   <td> <p>Per istruzioni su come collegare le [!DNL Google Drive] account a [!DNL Workfront Fusion], vedi <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Collegamento [!DNL Google Drive] a [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Seleziona la cartella da controllare]</td>
    <td >Selezionare la cartella dell'unità in cui si desidera visualizzare i file.</td>
  </tr> 
  <tr> 
    <td>[!UICONTROL Quali file controllare]</td>
   <td> <p>Selezionare il tipo di file da visualizzare.</p> 
    <ul> 
     <li>[!UICONTROL ALL]</li> 
     <li>[!DNL Google Documents]</li> 
     <li>[!DNL Google Spreadsheets]</li> 
     <li>[!DNL Google Slides]</li> 
     <li>[!DNL Google Drawings]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td >[!UICONTROL Converti [!DNL Google Documents] file da formattare]</td>
    <td>Selezionare il formato di file che si desidera convertire [!DNL Google Documents] a.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Converti [!DNL Google Spreadsheets] file da formattare]</td>
    <td>Selezionare il formato di file che si desidera convertire [!DNL Google Spreadsheets] a.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Converti [!DNL Google Slides] file da formattare]</td>
    <td>Selezionare il formato di file che si desidera convertire [!DNL Google Slides] a.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Converti [!DNL Google Drawings] file da formattare]</td>
    <td>Selezionare il formato di file che si desidera convertire [!DNL Google Drawings] a.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Watch]</td>
    <td>Selezionare se si desidera visualizzare i nuovi file e tutte le modifiche o solo i nuovi file.</td>
  </tr> 
  <tr> 
    <td>[!UICONTROL Numero massimo di file scaricati]</td>
    <td>Imposta il numero massimo di risultati che [!DNL Workfront Fusion] viene scaricato durante un ciclo (il numero di ripetizioni per esecuzione di scenari).</td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Guarda tutti i file]

Recupera i dettagli del file quando un file nel [!DNL Google Drive] viene aggiunto o modificato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google Drive] account a [!DNL Workfront Fusion], vedi <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Collegamento [!DNL Google Drive] a [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Quali file controllare]</td> 
   <td> <p>Selezionare il tipo di file da visualizzare.</p> 
    <ul> 
     <li>[!UICONTROL ALL]</li> 
     <li>[!DNL Google Documents]</li> 
     <li>[!DNL Google Spreadsheets]</li> 
     <li>[!DNL Google Slides]</li> 
     <li>[!DNL Google Drawings]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td >[!UICONTROL Converti [!DNL Google Documents] file da formattare]</td>
    <td>Selezionare il formato di file che si desidera convertire [!DNL Google Documents] a.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Converti [!DNL Google Spreadsheets] file da formattare]</td>
    <td>Selezionare il formato di file che si desidera convertire [!DNL Google Spreadsheets] a.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Converti [!DNL Google Slides] file da formattare]</td>
    <td>Selezionare il formato di file che si desidera convertire [!DNL Google Slides] a.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Converti [!DNL Google Drawings] file da formattare]</td>
    <td>Selezionare il formato di file che si desidera convertire [!DNL Google Drawings] a.</td>
  </tr>  
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td>Selezionare se si desidera visualizzare i nuovi file e tutte le modifiche o solo i nuovi file.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Numero massimo di file scaricati]</td> 
   <td>Imposta il numero massimo di risultati che [!DNL Workfront Fusion] viene scaricato durante un ciclo (il numero di ripetizioni per esecuzione di scenari).</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Guarda i file condivisi]

Attiva quando un nuovo file viene condiviso con te o un file condiviso esistente viene aggiornato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google Drive] account a [!DNL Workfront Fusion], vedi <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Collegamento [!DNL Google Drive] a [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Seleziona la cartella da controllare]</td> 
   <td>Selezionare la cartella condivisa in cui si desidera visualizzare i file.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Quali file controllare]</td> 
   <td> <p>Selezionare il tipo di file da visualizzare.</p> 
    <ul> 
     <li>[!UICONTROL ALL]</li> 
     <li>[!DNL Google Documents]</li> 
     <li>[!DNL Google Spreadsheets]</li> 
     <li>[!DNL Google Slides]</li> 
     <li>[!DNL Google Drawings]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td >[!UICONTROL Converti [!DNL Google Documents] file da formattare]</td>
    <td>Selezionare il formato di file che si desidera convertire [!DNL Google Documents] a.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Converti [!DNL Google Spreadsheets] file da formattare]</td>
    <td>Selezionare il formato di file che si desidera convertire [!DNL Google Spreadsheets] a.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Converti [!DNL Google Slides] file da formattare]</td>
    <td>Selezionare il formato di file che si desidera convertire [!DNL Google Slides] a.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Converti [!DNL Google Drawings] file da formattare]</td>
    <td>Selezionare il formato di file che si desidera convertire [!DNL Google Drawings] a.</td>
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td>Selezionare se si desidera visualizzare i nuovi file e tutte le modifiche o solo i nuovi file.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Numero massimo di file scaricati]</td> 
   <td>Imposta il numero massimo di risultati che [!DNL Workfront Fusion] viene scaricato durante un ciclo (il numero di ripetizioni per esecuzione di scenari).</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Osserva commenti]

Attiva quando un commento viene aggiunto o modificato nel file selezionato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google Drive] account a [!DNL Workfront Fusion], vedi <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Collegamento [!DNL Google Drive] a [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File]</td> 
   <td>Selezionare il file da controllare per i commenti.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td>Selezionare se si desidera controllare tutte le modifiche o solo i nuovi commenti</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Numero massimo di commenti restituiti]</td> 
   <td>Imposta il numero massimo di commenti che [!DNL Workfront Fusion] restituirà durante un ciclo (il numero di ripetizioni per esecuzione di scenari).</td> 
  </tr> 
 </tbody> 
</table>

### Azioni

* [[!UICONTROL Caricare un file]](#upload-a-file)
* [[!UICONTROL Aggiornare un file]](#update-a-file)
* [[!UICONTROL Copia un file]](#copy-a-file)
* [[!UICONTROL Eliminare un file]](#delete-a-file)
* [[!UICONTROL Spostare un file o una cartella nel cestino]](#move-a-filefolder-to-trash)
* [[!UICONTROL Ottieni un file]](#get-a-file)
* [[!UICONTROL Cerca file/cartelle]](#search-for-filesfolders)
* [[!UICONTROL Creare una cartella]](#create-a-folder)
* [[!UICONTROL Ottenere un collegamento di condivisione]](#get-a-share-link)

#### [!UICONTROL Caricare un file]

Carica un file sul tuo [!DNL Google Drive].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google Drive] account a [!DNL Workfront Fusion], vedi <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Collegamento [!DNL Google Drive] a [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Destination]</td> 
   <td> <p>Seleziona la destinazione in cui desideri caricare un file.</p> 
    <ul> 
     <li>[!DNL My Drive]</li> 
     <li>[!DNL Shared with Me]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cartella Target]</td> 
   <td>Seleziona la cartella in cui desideri caricare un file. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File di origine]</td> 
   <td>Seleziona se desideri utilizzare un file passato da un modulo precedente o se desideri mappare manualmente il file.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File name]</td> 
   <td>Selezionare il nome del file. Questa opzione è disponibile se si seleziona "[!UICONTROL Map]" nel campo [!UICONTROL file di origine].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data]</td> 
   <td>Seleziona il file di dati da caricare. Questa opzione è disponibile se si seleziona "[!UICONTROL Map]" nel campo [!UICONTROL file di origine].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Title]</td> 
   <td>Inserisci un titolo per il nuovo file.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convertire un file]</td> 
   <td>L’abilitazione di questa opzione consente al modulo di convertire i file nel corrispondente [!DNL Google] formato.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggiornare un file]

Aggiorna i metadati o il contenuto di un file.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google Drive] account a [!DNL Workfront Fusion], vedi <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Collegamento [!DNL Google Drive] a [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Destinazione]</td> 
   <td> <p>Seleziona la destinazione in cui desideri caricare un file.</p> 
    <ul> 
     <li>[!UICONTROL My Drive]</li> 
     <li>[!UICONTROL condiviso con me]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sposta in una cartella]</td> 
   <td>Se si desidera spostare il file in un'altra cartella, selezionare la cartella in cui si desidera spostare il file.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File ID]</td> 
   <td>Mappa l'ID del file da aggiornare.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Title]</td> 
   <td>Inserisci un titolo per il file aggiornato.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Modificare il contenuto di un file]</td> 
   <td>Seleziona se sostituire il contenuto del file.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File di origine]</td> 
   <td>Seleziona se desideri utilizzare un file passato da un modulo precedente o se desideri mappare manualmente il file. Questo campo è disponibile se è stato selezionato per modificare il contenuto del file nel campo precedente.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File name]</td> 
   <td>Selezionare il nome del file. Questa opzione è disponibile se si seleziona "[!UICONTROL Map]" nel campo [!UICONTROL file di origine].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data]</td> 
   <td>Seleziona il file di dati da caricare. Questa opzione è disponibile se si seleziona "[!UICONTROL Map]" nel campo [!UICONTROL file di origine].</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Copia un file]

Copia un file nella nuova posizione.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google Drive] account a [!DNL Workfront Fusion], vedi <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Collegamento [!DNL Google Drive] a [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Destinazione]</td> 
   <td> <p>Seleziona la destinazione in cui desideri caricare un file.</p> 
    <ul> 
     <li>[!UICONTROL My Drive]</li> 
     <li>[!UICONTROL condiviso con me]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cartella Target]</td> 
   <td>Selezionare la cartella in cui si trova il file da copiare/</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File ID]</td> 
   <td>Mappa l'ID del file da aggiornare.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Il nome della copia]</td> 
   <td>Inserisci un titolo per il nuovo file. Lasciare vuoto questo campo se non si desidera modificare il nome del file originale.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminare un file]

Elimina definitivamente un file o una cartella.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google Drive] account a [!DNL Workfront Fusion], vedi <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Collegamento [!DNL Google Drive] a [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File ID]</td> 
   <td>Mappa l’ID del file da eliminare.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Spostare un file o una cartella nel cestino]

Sposta un file o una cartella nel cestino.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google Drive] account a [!DNL Workfront Fusion], vedi <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Collegamento [!DNL Google Drive] a [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File ID]</td> 
   <td>Mappa l'ID del file da spostare nel cestino.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottieni un file]

Recupera il file con l’ID specificato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google Drive] account a [!DNL Workfront Fusion], vedi <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Collegamento [!DNL Google Drive] a [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converti [!DNL Google Documents] file da formattare]</td> 
   <td>Selezionare il formato di file che si desidera convertire [!DNL Google Documents] a.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converti [!DNL Google Spreadsheets] file da formattare]</td> 
   <td>Selezionare il formato di file che si desidera convertire [!DNL Google Spreadsheets] a.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converti [!DNL Google Slides] file da formattare]</td> 
   <td>Selezionare il formato di file che si desidera convertire [!DNL Google Slides] a.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converti [!DNL Google Drawings] file da formattare]</td> 
   <td>Selezionare il formato di file che si desidera convertire [!DNL Google Drawings] a.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File ID]</td> 
   <td>Mappa l’ID del file da recuperare.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Cerca file/cartelle]

Cerca file o cartelle in base ai criteri di ricerca.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google Drive] account a [!DNL Workfront Fusion], vedi <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Collegamento [!DNL Google Drive] a [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Destinazione]</td> 
   <td> <p>Seleziona la destinazione da cercare.</p> 
    <ul> 
     <li>[!UICONTROL My Drive]</li> 
     <li>[!UICONTROL condiviso con me]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Elencare una cartella]</td> 
   <td>Passa alla cartella in cui desideri cercare i file o le cartelle.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Retrieve]</td> 
   <td> <p> Selezionare se si desidera cercare file, cartelle o entrambi.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Search]</p> </td> 
   <td> <p>Selezionare il tipo di ricerca che si desidera eseguire.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Cerca nei nomi di file/cartelle]</strong> </p> 
      <ul> 
       <li> <p><strong>Query [!UICONTROL]</strong> </p> <p>Immettere una parte del nome file o del nome file completo (incluso il suffisso) da cercare.</p> </li> 
       <li> <p><strong>[!UICONTROL Opzioni di ricerca]</strong> </p> <p>Selezionare se si desidera cercare il termine esatto o se si desidera cercare i nomi contenenti il termine di ricerca.</p> </li> 
      </ul> </li> 
     <li> <p><strong>Ricerca di [!UICONTROL Fulltext]</strong> </p> 
      <ul> 
       <li> <p><strong>Query [!UICONTROL]</strong> </p> <p>Inserisci qualsiasi termine di ricerca che desideri cercare nel tuo [!DNL Google Drive].</p> </li> 
      </ul> </li> 
     <li> <p><strong>Immettere una query di ricerca personalizzata</strong> </p> 
      <ul> 
       <li> <p><strong>Query [!UICONTROL]</strong> </p> <p>Inserisci la query di ricerca personalizzata. Per ulteriori dettagli, consulta la sezione [!UICONTROL Search for Files] di questo articolo.</p> </li> 
       <li> <p><strong>Aggiungi alla query la cartella selezionata sopra</strong> </p> <p>Cerca la cartella nell'insieme parent. Questo trova tutti i file e le cartelle che si trovano direttamente nella cartella selezionata sopra.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Numero massimo di risultati restituiti]</td> 
   <td>Imposta il numero massimo di file o cartelle [!DNL Workfront Fusion] tornerà durante un ciclo di esecuzione.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Continua l’esecuzione del percorso anche se il modulo non restituisce risultati]</td> 
   <td>Abilita questa opzione per garantire che lo scenario non venga interrotto se il modulo non restituisce risultati.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Creare una cartella]

Crea una cartella nel percorso specificato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google Drive] account a [!DNL Workfront Fusion], vedi <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Collegamento [!DNL Google Drive] a [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Destinazione]</td> 
   <td> <p>Seleziona la destinazione in cui desideri caricare un file.</p> 
    <ul> 
     <li>[!UICONTROL My Drive]</li> 
     <li>[!UICONTROL condiviso con me]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nuovo percorso cartella]</td> 
   <td>Passa alla posizione in cui desideri creare una nuova cartella.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Il nome della nuova cartella]</td> 
   <td>Immettere un nome per la cartella che si sta creando.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Condividi cartella]</td> 
   <td>Seleziona questa opzione se desideri condividere la cartella con altri utenti con il collegamento [!UICONTROL Condividi]. In caso contrario, il collegamento di condivisione è solo per il proprietario.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottenere un collegamento di condivisione]

Recupera il collegamento di condivisione per un file in Google Drive.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google Drive] account a [!DNL Workfront Fusion], vedi <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Collegamento [!DNL Google Drive] a [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File ID]</td> 
   <td>Mappa l'ID del file per il quale vuoi ottenere il collegamento di condivisione.</td> 
  </tr> 
 </tbody> 
</table>

## Risoluzione dei problemi

### Impossibile caricare o aggiornare un file

Ci sono diverse situazioni in cui il caricamento o l’aggiornamento di un file non riesce:

* Il file caricato è troppo grande e supera il limite massimo di dimensione del file consentito per il tuo [!DNL Google Drive] pianifica o hai superato il tuo [!DNL Google Drive] limite di archiviazione. È possibile aggiornare il piano di storage o eliminare i file esistenti dal [!DNL Google Drive] servizio.
* La cartella selezionata in cui deve essere caricato il file non esiste più. Lo scenario si arresta e quindi è necessario selezionare di nuovo una cartella di destinazione.

## Cercare file

Nei file di elenco dei moduli in una cartella è possibile utilizzare una query personalizzata costituita da queste parti:

* **[!UICONTROL Campo]** - Attributo del file in corso di ricerca, ad esempio, l&#39;attributo `name` del file.

* **[!UICONTROL Operatore]** - Test eseguito sui dati per fornire una corrispondenza, ad esempio, `contains`.

* **[!UICONTROL Valore]** - Il contenuto dell&#39;attributo testato, ad esempio il nome del file `My cool document`.

Combinare clausole con le congiunzioni `and` o `or`e nega la query con `not`.

* [Campi](#fields)
* [Tipi di valore](#value-types)
* [Operatori](#operators)
* [Esempi](#examples)

### Campi

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Campo </th> 
   <th>Tipo di valore </th> 
   <th>Operatori</th> 
   <th> <p> Descrizione</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><code>[!UICONTROL title]</code></td> 
   <td>string</td> 
   <td><code>contains</code><sup>1</sup>, <code>=</code>, <code>!=</code></td> 
   <td> <p> Nome del file.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL fullText]</code> </td> 
   <td>string </td> 
   <td><code>contains</code><sup>2, 3</sup> </td> 
   <td> <p> Testo completo del file, compresi nome, descrizione, contenuto e testo indicizzabile.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL mimeType]</code> </td> 
   <td> string</td> 
   <td><code>contains</code>, <code>=</code>, <code>!=</code></td> 
   <td> <p> Tipo MIME del file.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL modifiedDate]</code> </td> 
   <td> date<sup>4</sup></td> 
   <td><code> &lt;=</code>, <code>&lt;</code>, <code>=</code>, <code>!=</code>, <code>></code>, <code>>=</code></td> 
   <td> <p> Data dell’ultima modifica apportata al file.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL lastViewedByMeDate]</code> </td> 
   <td> date<sup>4</sup></td> 
   <td><code>&lt;=</code>, <code>&lt;</code>, <code>=</code>, <code>!=</code>, <code>></code>, <code>>=</code></td> 
   <td> <p> Data dell’ultima visualizzazione di un file da parte dell’utente.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL trashed]</code></td> 
   <td>booleano </td> 
   <td><code>=</code>, <code>!=</code></td> 
   <td> <p> Se il file si trova nel cestino o no.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL starred]</code></td> 
   <td>booleano </td> 
   <td><code>=</code>, <code>!=</code></td> 
   <td> <p>Se il file viene avviato o meno.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL parents]</code></td> 
   <td>raccolta </td> 
   <td><code>in </code> </td> 
   <td> <p>Se l'insieme [!UICONTROL parent] contiene l'ID specificato.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL owners]</code></td> 
   <td>raccolta </td> 
   <td><code>in </code> </td> 
   <td> <p>Utenti titolari del file.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL writers]</code></td> 
   <td>raccolta </td> 
   <td><code>in </code> </td> 
   <td> <p>Utenti autorizzati a modificare il file.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL readers] </code> </td> 
   <td>raccolta </td> 
   <td><code>in </code> </td> 
   <td> <p>Utenti autorizzati a leggere il file.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL sharedWithMe]</code> </td> 
   <td>booleano </td> 
   <td><code>=</code>, <code>!=</code></td> 
   <td> <p> File presenti nell'insieme "Condivisi con me" dell'utente.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL properties] </code> </td> 
   <td>raccolta</td> 
   <td><code>has </code> </td> 
   <td> <p> Proprietà dei file personalizzati pubblici.</p> </td> 
  </tr> 
 </tbody> 
</table>

Considera quanto segue sugli operatori in questi campi:

* La `contains` esegue solo la corrispondenza del prefisso per un `title`.

   Ad esempio, il titolo &quot;HelloWorld&quot; corrisponde a `title contains 'Hello'` ma non `title contains 'World'`.

* La `contains` esegue solo la corrispondenza su token stringa interi per `fullText`.

   Ad esempio, se il testo completo di un documento contiene la stringa &quot;HelloWorld&quot; solo la query `fullText contains 'HelloWorld'` restituisce un risultato. Query quali `fullText contains 'Hello'` non restituisce risultati in questo scenario.

* La `contains` l’operatore corrisponde a una frase alfanumerica esatta se è circondato da virgolette doppie.

   Ad esempio, se `fullText` di un documento contiene la stringa &quot;Ciao a tutti&quot;, quindi la query `fullText contains '"Hello there"'` restituisce un risultato, ma la query `fullText contains '"Hello world"'` No.

   Inoltre, poiché la ricerca è alfanumerica, se la `fullText` di un documento contiene la stringa &quot;Hello_world&quot;, quindi la query `fullText contains '"Hello world"'` restituisce un risultato.

* Campi `type` Attualmente la data non è paragonabile tra loro, ma solo a date costanti.

### Tipi di valore

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo di valore</th> 
   <th> <p> Note</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Stringa </td> 
   <td> <p>Surround con virgolette singole '. Evita virgolette singole nelle query con <code>\'</code>ad esempio<code> 'Valentine\'s Day'</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>Booleano </td> 
   <td> <p><code>true </code>oppure <code>false</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>Data </td> 
   <td> <p>Formato RFC 3339, il fuso orario predefinito è UTC, ad esempio <code>2012-06-04T12:00:00-08:00</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Operatori

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Operatore </th> 
   <th> <p>Note</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><code>contains</code></td> 
   <td> <p>Il contenuto di una stringa è presente nell'altra.</p> </td> 
  </tr> 
  <tr> 
   <td><code>=</code> </td> 
   <td> <p> Il contenuto di una stringa o di un valore booleano è uguale all’altro.</p> </td> 
  </tr> 
  <tr> 
   <td><code>!=</code> </td> 
   <td> <p> Il contenuto di una stringa o di un valore booleano non è uguale all’altro.</p> </td> 
  </tr> 
  <tr> 
   <td><code>&lt;</code> </td> 
   <td> <p> Una data è precedente a un'altra.</p> </td> 
  </tr> 
  <tr> 
   <td><code>&lt;=</code> </td> 
   <td> <p> Una data è precedente o uguale a un'altra.</p> </td> 
  </tr> 
  <tr> 
   <td><code>></code> </td> 
   <td> <p> Una data è successiva a un'altra.</p> </td> 
  </tr> 
  <tr> 
   <td><code>>=</code> </td> 
   <td> <p> Una data è successiva o uguale a un’altra.</p> </td> 
  </tr> 
  <tr> 
   <td><code>in </code> </td> 
   <td> <p>Un elemento è contenuto all’interno di una raccolta.</p> </td> 
  </tr> 
  <tr> 
   <td><code>and </code> </td> 
   <td> <p>Restituisce file che corrispondono a entrambe le clausole.</p> </td> 
  </tr> 
  <tr> 
   <td><code>or </code> </td> 
   <td> <p>Restituisce file che corrispondono a una delle due clausole.</p> </td> 
  </tr> 
  <tr> 
   <td><code>not </code> </td> 
   <td> <p>Ignora una clausola di ricerca.</p> </td> 
  </tr> 
  <tr> 
   <td><code>has </code> </td> 
   <td> <p>Una raccolta contiene un elemento che corrisponde ai parametri.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per le clausole composte, è possibile utilizzare le parentesi per raggruppare le clausole. Ad esempio:
`modifiedDate > '2012-06-04T12:00:00' and (mimeType contains 'image/' or mimeType contains 'video/')` Questa ricerca restituisce tutti i file con un tipo MIME immagine o video che l’ultima modifica è stata apportata dopo il 4 giugno 2012. Perché `and` e `or` gli operatori vengono valutati da sinistra a destra, senza parentesi, l’esempio precedente restituirà solo le immagini modificate dopo il 4 giugno 2012, ma restituirà tutti i video, anche quelli precedenti al 4 giugno 2012.

### Esempi

Tutti gli esempi in questa pagina mostrano i dati non codificati `<q>q</q>` , dove `title = 'hello'` viene codificato come `title+%3d+%27hello%27`. Le librerie client gestiscono automaticamente questa codifica.

* Cerca file con il nome &quot;hello&quot;

   <pre>title = 'hello'</pre>
* Cerca cartelle utilizzando il tipo MIME specifico per la cartella

   <pre>mimeType = 'application/vnd.google-apps.folder'</pre>
* Cercare file che non sono cartelle

   <pre>mimeType != 'application/vnd.google-apps.folder'</pre>
* Cerca file con un nome contenente le parole &quot;hello&quot; e &quot;arrivederci&quot;

   <pre>il titolo contiene 'hello' e [!UICONTROL name] contiene 'arrivederci'</pre>
* Cerca file con un nome che non contenga la parola &quot;hello&quot;

   <pre>il titolo non contiene "hello"</pre>
* Cerca file contenenti la parola &quot;hello&quot; nel contenuto

   <pre>fullText contiene 'hello'</pre>
* Cerca file che non contengono la parola &quot;hello&quot; nel contenuto

   <pre>not fullText contiene 'hello'</pre>
* Cerca i file contenenti la frase esatta &quot;hello world&quot; nel contenuto

   <pre>fullText contiene '"hello world"'fullText contiene '"hello_world"</pre>
* Cerca file con una query contenente il carattere &quot;\&quot; (ad esempio, &quot;\authors&quot;)

   <pre>fullText contiene '\\authors'</pre>
* Cerca file scrivibili dall&#39;utente &quot;test@example.org&quot;

   <pre>"test@example.org" in [!DNL writers]</pre>
* Cerca l&#39;ID `1234567` in `parents` raccolta. In questo modo vengono trovati tutti i file e le cartelle che si trovano direttamente nella cartella il cui ID è `1234567`.

   <pre>'1234567' in [!UICONTROL parent]</pre>
* Cerca l’ID alias `appDataFolder` in `parents` raccolta. Questo trova tutti i file e le cartelle che si trovano direttamente sotto il [Cartella dati applicazione](https://developers.google.com/drive/api/v2/appdata).

   <pre>'appDataFolder' negli elementi principali</pre>
* Cerca file scrivibili dagli utenti &quot;test@example.org&quot; e &quot;test2@example.org&quot;

   <pre>"test@example.org" negli autori e "test2@example.org" negli autori</pre>
* Cerca i file contenenti il testo &quot;importante&quot; che si trovano nel cestino

   <pre>fullText contiene 'important' e cestato = true</pre>
* Cerca file modificati dopo il 4 giugno 2012

   <pre>modifiedDate &gt; '2012-06-04T12:00:00' // il fuso orario predefinito è UTC</pre><pre>modifiedDate &gt; '2012-06-04T12:00:00-08:00'</pre>
* Cerca file condivisi con l&#39;utente autorizzato con il nome &quot;hello&quot;

   <pre>sharedWithMe e title contengono 'hello'</pre>
* Cercare file con un [proprietà file personalizzata](https://developers.google.com/drive/api/v2/properties) denominato `additionalID` con il valore `8e8aceg2af2ge72e78`.

   <pre>le proprietà hanno { key='additionalID' e value='8e8aceg2af2ge72e78' e visibility='PRIVATE' }</pre>

Origine di questa guida [[!DNL Google Drive] documentazione](https://developers.google.com/drive/api/v2/search-shareddrives).
