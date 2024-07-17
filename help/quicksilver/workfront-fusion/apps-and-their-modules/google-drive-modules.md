---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli unità Google
description: I  [!DNL Adobe Workfront Fusion Google Drive] moduli ti consentono di monitorare, cercare, creare, aggiornare, eliminare e gestire i tuoi file, cartelle o unità condivise nel tuo [!DNL Google Drive].
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 7d620c93-d1bf-4451-9f76-1d6fd850cec9
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '2941'
ht-degree: 0%

---

# [!DNL Google Drive] moduli

I moduli [!DNL Adobe Workfront Fusion] [!DNL Google Drive] consentono di monitorare, cercare, creare, aggiornare, eliminare e gestire i file, la cartella o le unità condivise in [!DNL Google Drive].

In uno scenario [!DNL Adobe Workfront Fusion], è possibile collegare l&#39;account [!DNL Google Drive] a più applicazioni e servizi di terze parti.

Se hai bisogno di istruzioni per la creazione di uno scenario, consulta [Creare uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Per informazioni sui moduli, vedere [Moduli in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Requisiti di accesso

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td>
  <td> <p>[!UICONTROL Pro] o versione successiva</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licenza**</td> 
   <td>
   <p>Requisiti di licenza correnti: nessun requisito di licenza [!DNL Workfront Fusion].</p>
   <p>Oppure</p>
   <p>Requisito licenza legacy: [!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>
   <p>Fabbisogno prodotto corrente: se si dispone del piano [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront], l'organizzazione deve acquistare [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo. [!DNL Workfront Fusion] è incluso nel piano [!UICONTROL Ultimate] [!DNL Workfront].</p>
   <p>Oppure</p>
   <p>Requisiti del prodotto legacy: la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Per conoscere il piano, il tipo di licenza o l&#39;accesso disponibili, contattare l&#39;amministratore [!DNL Workfront].

Per informazioni sulle [!DNL Adobe Workfront Fusion] licenze, vedere [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).



## Connessione di [!DNL Google Drive] a [!DNL Workfront Fusion]

Se sei [!DNL @gmail.com] o [!DNL @googlemail.com] utente devi creare un client OAuth su [the [!DNL Google Cloud Platform]](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) per ottenere [!UICONTROL ID client] e [!UICONTROL Segreto client].

Per istruzioni dettagliate su come creare il client OAuth (e ottenere [!UICONTROL ID client] e [!UICONTROL Segreto client]), vedi [Connetti [!DNL Adobe Workfront Fusion] a [!DNL Google Services] utilizzando un client OAuth personalizzato](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

Per istruzioni sulla connessione dell&#39;account [!DNL Google Drive] a [!UICONTROL Workfront Fusion], vedere [Creare una connessione a [!UICONTROL Adobe Workfront Fusion] - Istruzioni di base](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!DNL Google Drive] moduli e relativi campi

Quando configuri [!DNL Google Drive] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Insieme a questi, potrebbero essere visualizzati ulteriori campi di [!DNL Google Drive], a seconda di fattori quali il livello di accesso nell&#39;app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se viene visualizzato il pulsante Mappa sopra un campo o una funzione, è possibile utilizzarlo per impostare variabili e funzioni per tale campo. Per ulteriori informazioni, vedere [Mappare le informazioni da un modulo all&#39;altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)



* [Triggers](#triggers)
* [Azioni](#actions)

### Triggers

* [[!UICONTROL Guarda I File Nella Cartella]](#watch-files-in-folder)
* [[!UICONTROL Guarda tutti i file]](#watch-all-files)
* [[!UICONTROL Guarda i file condivisi]](#watch-shared-files)
* [[!UICONTROL Osserva commenti]](#watch-comments)

#### [!UICONTROL Guarda I File Nella Cartella]

Recupera i dettagli del file quando un file viene aggiunto o modificato nella cartella specificata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Connection] </td>
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Google Drive] a [!DNL Workfront Fusion], vedere <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Connessione di [!DNL Google Drive] a [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Seleziona la cartella da controllare]</td>
    <td >Selezionare nell'unità la cartella in cui si desidera visualizzare i file.</td>
  </tr> 
  <tr> 
    <td>[!UICONTROL Quali file guardare]</td>
   <td> <p>Selezionare il tipo di file che si desidera visualizzare.</p> 
    <ul> 
     <li>[!UICONTROL Tutto]</li> 
     <li>[!DNL Google Documents]</li> 
     <li>[!DNL Google Spreadsheets]</li> 
     <li>[!DNL Google Slides]</li> 
     <li>[!DNL Google Drawings]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td >[!UICONTROL Converti [!DNL Google Documents] file in formato]</td>
    <td>Selezionare il formato di file in cui convertire [!DNL Google Documents].</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Converti [!DNL Google Spreadsheets] file in formato]</td>
    <td>Selezionare il formato di file in cui convertire [!DNL Google Spreadsheets].</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Converti [!DNL Google Slides] file in formato]</td>
    <td>Selezionare il formato di file in cui convertire [!DNL Google Slides].</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Converti [!DNL Google Drawings] file in formato]</td>
    <td>Selezionare il formato di file in cui convertire [!DNL Google Drawings].</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Watch]</td>
    <td>Selezionare se si desidera visualizzare i nuovi file e tutte le modifiche o solo i nuovi file.</td>
  </tr> 
  <tr> 
    <td>[!UICONTROL Numero massimo di file scaricati]</td>
    <td>Impostare il numero massimo di risultati che [!DNL Workfront Fusion] scaricherà durante un ciclo (il numero di ripetizioni per esecuzione dello scenario).</td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Guarda tutti i file]

Recupera i dettagli del file quando un file in [!DNL Google Drive] viene aggiunto o modificato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Google Drive] a [!DNL Workfront Fusion], vedere <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Connessione di [!DNL Google Drive] a [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Quali file guardare]</td> 
   <td> <p>Selezionare il tipo di file che si desidera visualizzare.</p> 
    <ul> 
     <li>[!UICONTROL Tutto]</li> 
     <li>[!DNL Google Documents]</li> 
     <li>[!DNL Google Spreadsheets]</li> 
     <li>[!DNL Google Slides]</li> 
     <li>[!DNL Google Drawings]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td >[!UICONTROL Converti [!DNL Google Documents] file in formato]</td>
    <td>Selezionare il formato di file in cui convertire [!DNL Google Documents].</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Converti [!DNL Google Spreadsheets] file in formato]</td>
    <td>Selezionare il formato di file in cui convertire [!DNL Google Spreadsheets].</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Converti [!DNL Google Slides] file in formato]</td>
    <td>Selezionare il formato di file in cui convertire [!DNL Google Slides].</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Converti [!DNL Google Drawings] file in formato]</td>
    <td>Selezionare il formato di file in cui convertire [!DNL Google Drawings].</td>
  </tr>  
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td>Selezionare se si desidera visualizzare i nuovi file e tutte le modifiche o solo i nuovi file.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Numero massimo di file scaricati]</td> 
   <td>Impostare il numero massimo di risultati che [!DNL Workfront Fusion] scaricherà durante un ciclo (il numero di ripetizioni per esecuzione dello scenario).</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Guarda i file condivisi]

Si attiva quando viene condiviso un nuovo file o viene aggiornato un file condiviso esistente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Google Drive] a [!DNL Workfront Fusion], vedere <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Connessione di [!DNL Google Drive] a [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Seleziona la cartella da controllare]</td> 
   <td>Seleziona la cartella condivisa in cui desideri guardare i file.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Quali file guardare]</td> 
   <td> <p>Selezionare il tipo di file che si desidera visualizzare.</p> 
    <ul> 
     <li>[!UICONTROL Tutto]</li> 
     <li>[!DNL Google Documents]</li> 
     <li>[!DNL Google Spreadsheets]</li> 
     <li>[!DNL Google Slides]</li> 
     <li>[!DNL Google Drawings]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td >[!UICONTROL Converti [!DNL Google Documents] file in formato]</td>
    <td>Selezionare il formato di file in cui convertire [!DNL Google Documents].</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Converti [!DNL Google Spreadsheets] file in formato]</td>
    <td>Selezionare il formato di file in cui convertire [!DNL Google Spreadsheets].</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Converti [!DNL Google Slides] file in formato]</td>
    <td>Selezionare il formato di file in cui convertire [!DNL Google Slides].</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Converti [!DNL Google Drawings] file in formato]</td>
    <td>Selezionare il formato di file in cui convertire [!DNL Google Drawings].</td>
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td>Selezionare se si desidera visualizzare i nuovi file e tutte le modifiche o solo i nuovi file.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Numero massimo di file scaricati]</td> 
   <td>Impostare il numero massimo di risultati che [!DNL Workfront Fusion] scaricherà durante un ciclo (il numero di ripetizioni per esecuzione dello scenario).</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Osserva commenti]

Si attiva quando un commento viene aggiunto o modificato nel file selezionato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Google Drive] a [!DNL Workfront Fusion], vedere <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Connessione di [!DNL Google Drive] a [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File]</td> 
   <td>Selezionare il file da controllare per i commenti.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td>Seleziona se desideri controllare tutte le modifiche o solo i nuovi commenti</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Numero massimo di commenti restituiti]</td> 
   <td>Impostare il numero massimo di commenti che [!DNL Workfront Fusion] restituirà durante un ciclo (il numero di ripetizioni per esecuzione dello scenario).</td> 
  </tr> 
 </tbody> 
</table>

### Azioni

* [[!UICONTROL Carica un file]](#upload-a-file)
* [[!UICONTROL Aggiorna un file]](#update-a-file)
* [[!UICONTROL Copia un file]](#copy-a-file)
* [[!UICONTROL Elimina un file]](#delete-a-file)
* [[!UICONTROL Sposta un file o una cartella nel cestino]](#move-a-filefolder-to-trash)
* [[!UICONTROL Ottieni un file]](#get-a-file)
* [[!UICONTROL Cerca file/cartelle]](#search-for-filesfolders)
* [[!UICONTROL Crea una cartella]](#create-a-folder)
* [[!UICONTROL Ottieni un collegamento di condivisione]](#get-a-share-link)

#### [!UICONTROL Carica un file]

Carica un file in [!DNL Google Drive].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Google Drive] a [!DNL Workfront Fusion], vedere <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Connessione di [!DNL Google Drive] a [!UICONTROL Workfront Fusion]</a></p> </td> 
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
   <td>[!UICONTROL Cartella di destinazione]</td> 
   <td>Selezionare la cartella in cui si desidera caricare un file. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source file]</td> 
   <td>Seleziona se desideri utilizzare un file trasmesso da un modulo precedente o se desideri mappare il file manualmente.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome file]</td> 
   <td>Selezionare il nome del file. Questa opzione è disponibile se si seleziona "[!UICONTROL Map]" nel campo [!UICONTROL source file].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data]</td> 
   <td>Seleziona il file di dati da caricare. Questa opzione è disponibile se si seleziona "[!UICONTROL Map]" nel campo [!UICONTROL source file].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Title]</td> 
   <td>Immettere un titolo per il nuovo file.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converti un file]</td> 
   <td>L'attivazione di questa opzione consente al modulo di convertire i file nel formato [!DNL Google] corrispondente.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggiorna un file]

Aggiorna i metadati o il contenuto di un file.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Google Drive] a [!DNL Workfront Fusion], vedere <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Connessione di [!DNL Google Drive] a [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Destination]</td> 
   <td> <p>Seleziona la destinazione in cui desideri caricare un file.</p> 
    <ul> 
     <li>[!UICONTROL Unità]</li> 
     <li>[!UICONTROL condiviso con me]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sposta in una cartella]</td> 
   <td>Se si desidera spostare il file in una cartella diversa, selezionare la cartella in cui si desidera spostare il file.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID file]</td> 
   <td>Mappa l’ID del file da aggiornare.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Title]</td> 
   <td>Immetti un titolo per il file aggiornato.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Modificare il contenuto di un file]</td> 
   <td>Seleziona se desideri sostituire il contenuto del file.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source file]</td> 
   <td>Seleziona se desideri utilizzare un file trasmesso da un modulo precedente o se desideri mappare il file manualmente. Questo campo è disponibile se si è scelto di modificare il contenuto del file nel campo precedente.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome file]</td> 
   <td>Selezionare il nome del file. Questa opzione è disponibile se si seleziona "[!UICONTROL Map]" nel campo [!UICONTROL source file].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data]</td> 
   <td>Seleziona il file di dati da caricare. Questa opzione è disponibile se si seleziona "[!UICONTROL Map]" nel campo [!UICONTROL source file].</td> 
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
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Google Drive] a [!DNL Workfront Fusion], vedere <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Connessione di [!DNL Google Drive] a [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Destination]</td> 
   <td> <p>Seleziona la destinazione in cui desideri caricare un file.</p> 
    <ul> 
     <li>[!UICONTROL Unità]</li> 
     <li>[!UICONTROL condiviso con me]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cartella di destinazione]</td> 
   <td>Selezionare la cartella in cui si trova il file che si desidera copiare/</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID file]</td> 
   <td>Mappa l’ID del file da aggiornare.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Il nome della copia]</td> 
   <td>Immettere un titolo per il nuovo file. Lasciare vuoto questo campo se non si desidera modificare il nome del file originale.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Elimina un file]

Elimina definitivamente un file o una cartella.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Google Drive] a [!DNL Workfront Fusion], vedere <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Connessione di [!DNL Google Drive] a [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID file]</td> 
   <td>Mappa l’ID del file da eliminare.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Sposta un file o una cartella nel cestino]

Sposta un file o una cartella nel cestino.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Google Drive] a [!DNL Workfront Fusion], vedere <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Connessione di [!DNL Google Drive] a [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID file]</td> 
   <td>Mappa l’ID del file da spostare nel cestino.</td> 
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
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Google Drive] a [!DNL Workfront Fusion], vedere <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Connessione di [!DNL Google Drive] a [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converti [!DNL Google Documents] file in formato]</td> 
   <td>Selezionare il formato di file in cui convertire [!DNL Google Documents].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converti [!DNL Google Spreadsheets] file in formato]</td> 
   <td>Selezionare il formato di file in cui convertire [!DNL Google Spreadsheets].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converti [!DNL Google Slides] file in formato]</td> 
   <td>Selezionare il formato di file in cui convertire [!DNL Google Slides].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converti [!DNL Google Drawings] file in formato]</td> 
   <td>Selezionare il formato di file in cui convertire [!DNL Google Drawings].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID file]</td> 
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
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Google Drive] a [!DNL Workfront Fusion], vedere <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Connessione di [!DNL Google Drive] a [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Destination]</td> 
   <td> <p>Seleziona la destinazione in cui desideri eseguire la ricerca.</p> 
    <ul> 
     <li>[!UICONTROL Unità]</li> 
     <li>[!UICONTROL condiviso con me]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Elenca una cartella]</td> 
   <td>Passare alla cartella in cui si desidera cercare i file o le cartelle.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Retrieve]</td> 
   <td> <p> Seleziona se desideri cercare file, cartelle o entrambi.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL - Ricerca]</p> </td> 
   <td> <p>Selezionare il tipo di ricerca che si desidera eseguire.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Cerca nei nomi di file/cartelle]</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Query]</strong> </p> <p>Immettere una parte del nome o del nome completo del file (compreso il suffisso) che si desidera cercare.</p> </li> 
       <li> <p><strong>[!UICONTROL Opzioni di ricerca]</strong> </p> <p>Selezionare se si desidera cercare il termine esatto o se si desidera cercare nomi contenenti il termine di ricerca.</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Fulltext] ricerca</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Query]</strong> </p> <p>Immettere un termine di ricerca da cercare in [!DNL Google Drive].</p> </li> 
      </ul> </li> 
     <li> <p><strong>Immettere una query di ricerca personalizzata</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Query]</strong> </p> <p>Immettere la query di ricerca personalizzata. Per ulteriori informazioni, consulta la sezione [!UICONTROL Search for Files] di questo articolo.</p> </li> 
       <li> <p><strong>Aggiungi la cartella selezionata in precedenza alla query</strong> </p> <p>Cerca la cartella nell'insieme parent. In questo modo vengono trovati tutti i file e le cartelle che si trovano direttamente nella cartella selezionata in precedenza.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Numero massimo di risultati restituiti]</td> 
   <td>Impostare il numero massimo di file o cartelle [!DNL Workfront Fusion] restituiti durante un ciclo di esecuzione.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Continua l'esecuzione della route anche se il modulo non restituisce alcun risultato]</td> 
   <td>Abilita questa opzione per garantire che lo scenario non venga interrotto se il modulo non restituisce alcun risultato.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crea una cartella]

Crea una cartella nel percorso specificato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Google Drive] a [!DNL Workfront Fusion], vedere <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Connessione di [!DNL Google Drive] a [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Destination]</td> 
   <td> <p>Seleziona la destinazione in cui desideri caricare un file.</p> 
    <ul> 
     <li>[!UICONTROL Unità]</li> 
     <li>[!UICONTROL condiviso con me]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nuovo percorso cartella]</td> 
   <td>Passa alla posizione in cui desideri creare una nuova cartella.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome della nuova cartella]</td> 
   <td>Immettere un nome per la cartella che si sta creando.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Condividi cartella]</td> 
   <td>Selezionare questa opzione se si desidera condividere la cartella con altri utenti tramite il collegamento [!UICONTROL Share]. In caso contrario, il collegamento di condivisione è solo per il proprietario.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottieni un collegamento di condivisione]

Recupera il collegamento di condivisione per un file in Google Drive.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Google Drive] a [!DNL Workfront Fusion], vedere <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Connessione di [!DNL Google Drive] a [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID file]</td> 
   <td>Mappa l’ID del file per il quale desideri ottenere il collegamento di condivisione.</td> 
  </tr> 
 </tbody> 
</table>

## Risoluzione dei problemi

### Impossibile caricare o aggiornare un file

Esistono diverse situazioni in cui il caricamento o l’aggiornamento di un file non riesce:

* Il file caricato è troppo grande e supera la dimensione massima consentita per il piano [!DNL Google Drive] oppure hai superato il limite di archiviazione di [!DNL Google Drive]. È possibile aggiornare il piano di archiviazione o eliminare i file esistenti dal servizio [!DNL Google Drive].
* La cartella selezionata in cui doveva essere caricato il file non esiste più. Lo scenario si interrompe ed è quindi necessario selezionare nuovamente una cartella di destinazione.

## Cerca file

Nel modulo Elenca i file in una cartella è possibile utilizzare una query personalizzata costituita dalle seguenti parti:

* **[!UICONTROL Campo]** - Attributo del file in cui viene eseguita la ricerca, ad esempio l&#39;attributo `name` del file.

* **[!UICONTROL Operatore]** - Test eseguito sui dati per fornire una corrispondenza, ad esempio `contains`.

* **[!UICONTROL Valore]** - Contenuto dell&#39;attributo testato, ad esempio il nome del file `My cool document`.

Combinare le clausole con le congiunzioni `and` o `or` e negare la query con `not`.

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
   <td>stringa</td> 
   <td><code>contains</code><sup>1</sup>, <code>=</code>, <code>!=</code></td> 
   <td> <p> Nome del file.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL fullText]</code> </td> 
   <td>stringa </td> 
   <td><code>contains</code><sup>2, 3</sup> </td> 
   <td> <p> Testo completo del file con nome, descrizione, contenuto e testo indicizzabile.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL mimeType]</code> </td> 
   <td> stringa</td> 
   <td><code>contains</code>, <code>=</code>, <code>!=</code></td> 
   <td> <p> Tipo MIME del file.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL modifiedDate]</code> </td> 
   <td> data<sup>4</sup></td> 
   <td><code> &lt;=</code>, <code>&lt;</code>, <code>=</code>, <code>!=</code>, <code>></code>, <code>>=</code></td> 
   <td> <p> Data dell’ultima modifica apportata al file.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL lastViewedByMeDate]</code> </td> 
   <td> data<sup>4</sup></td> 
   <td><code>&lt;=</code>, <code>&lt;</code>, <code>=</code>, <code>!=</code>, <code>></code>, <code>>=</code></td> 
   <td> <p> Data dell’ultima visualizzazione di un file da parte dell’utente.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL trashed]</code></td> 
   <td>booleano </td> 
   <td><code>=</code>, <code>!=</code></td> 
   <td> <p> Indica se il file si trova o meno nel cestino.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL starred]</code></td> 
   <td>booleano </td> 
   <td><code>=</code>, <code>!=</code></td> 
   <td> <p>Indica se il file è interpretato o meno.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL parents]</code></td> 
   <td>raccolta </td> 
   <td><code>in </code> </td> 
   <td> <p>Specifica se l'insieme padre [!UICONTROL] contiene l'ID specificato.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL owners]</code></td> 
   <td>raccolta </td> 
   <td><code>in </code> </td> 
   <td> <p>Utenti proprietari del file.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL writers]</code></td> 
   <td>raccolta </td> 
   <td><code>in </code> </td> 
   <td> <p>Utenti che dispongono dell'autorizzazione per modificare il file.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL readers] </code> </td> 
   <td>raccolta </td> 
   <td><code>in </code> </td> 
   <td> <p>Utenti che dispongono dell'autorizzazione per la lettura del file.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL sharedWithMe]</code> </td> 
   <td>booleano </td> 
   <td><code>=</code>, <code>!=</code></td> 
   <td> <p> File inclusi nella raccolta "Condivisi con me" dell'utente.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL properties] </code> </td> 
   <td>raccolta</td> 
   <td><code>has </code> </td> 
   <td> <p> Proprietà personalizzate del file pubblico.</p> </td> 
  </tr> 
 </tbody> 
</table>

Considera quanto segue sugli operatori in questi campi:

* L&#39;operatore `contains` esegue solo la corrispondenza del prefisso per un `title`.

  Ad esempio, il titolo &quot;HelloWorld&quot; corrisponde a `title contains 'Hello'` ma non a `title contains 'World'`.

* L&#39;operatore `contains` esegue la corrispondenza solo su token di stringa interi per `fullText`.

  Ad esempio, se il testo completo di un documento contiene la stringa &quot;HelloWorld&quot;, solo la query `fullText contains 'HelloWorld'` restituisce un risultato. Query come `fullText contains 'Hello'` non restituirebbero risultati in questo scenario.

* L&#39;operatore `contains` corrisponde a una frase alfanumerica esatta se è racchiuso tra virgolette doppie.

  Ad esempio, se il `fullText` di un documento contiene la stringa &quot;Hello there world&quot;, la query `fullText contains '"Hello there"'` restituisce un risultato, ma la query `fullText contains '"Hello world"'` no.

  Inoltre, poiché la ricerca è alfanumerica, se il `fullText` di un documento contiene la stringa &quot;Hello_world&quot;, la query `fullText contains '"Hello world"'` restituisce un risultato.

* I campi con data `type` non sono attualmente confrontabili tra loro, ma solo con date costanti.

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
   <td> <p>Racchiudi tra virgolette singole '. Eliminare le virgolette singole nelle query con <code>\'</code>, ad esempio <code> 'Valentine\'s Day'</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>Booleano </td> 
   <td> <p><code>true </code>o <code>false</code>.</p> </td> 
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
   <td> <p>Il contenuto di una stringa è presente nell’altra.</p> </td> 
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
   <td> <p> Una data è precedente a un’altra.</p> </td> 
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
   <td> <p>Un elemento è contenuto in una raccolta.</p> </td> 
  </tr> 
  <tr> 
   <td><code>and </code> </td> 
   <td> <p>Restituire i file che corrispondono a entrambe le clausole.</p> </td> 
  </tr> 
  <tr> 
   <td><code>or </code> </td> 
   <td> <p>Restituire i file che corrispondono a una delle due clausole.</p> </td> 
  </tr> 
  <tr> 
   <td><code>not </code> </td> 
   <td> <p>Nega una clausola di ricerca.</p> </td> 
  </tr> 
  <tr> 
   <td><code>has </code> </td> 
   <td> <p>Una raccolta contiene un elemento che corrisponde ai parametri.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per le clausole composte è possibile utilizzare le parentesi per raggruppare le clausole. Ad esempio:
`modifiedDate > '2012-06-04T12:00:00' and (mimeType contains 'image/' or mimeType contains 'video/')` Questa ricerca restituisce tutti i file con un tipo MIME immagine o video la cui ultima modifica è successiva al 4 giugno 2012. Poiché gli operatori `and` e `or` vengono valutati da sinistra a destra, senza parentesi, nell&#39;esempio precedente verranno restituite solo le immagini modificate dopo il 4 giugno 2012, ma tutti i video verranno restituiti anche prima del 4 giugno 2012.

### Esempi

Tutti gli esempi in questa pagina mostrano il parametro `<q>q</q>` non codificato, dove `title = 'hello'` è codificato come `title+%3d+%27hello%27`. Le librerie client gestiscono automaticamente questa codifica.

* Cerca file con nome &quot;hello&quot;
  <pre>title = 'ciao'</pre>
* Cerca le cartelle utilizzando il tipo MIME specifico per la cartella
  <pre>mimeType = 'application/vnd.google-apps.folder'</pre>
* Cerca file che non sono cartelle
  <pre>mimeType!= 'application/vnd.google-apps.folder'</pre>
* Cerca i file con un nome contenente le parole &quot;hello&quot; e &quot;bye&quot;
  <pre>il titolo contiene 'hello' e [!UICONTROL name] contiene 'goodbye'</pre>
* Cerca file con un nome che non contiene la parola &quot;hello&quot;
  <pre>il titolo non contiene 'hello'</pre>
* Cerca i file che contengono la parola &quot;hello&quot; nel contenuto
  <pre>fullText contiene 'hello'</pre>
* Cerca i file che non contengono la parola &quot;hello&quot; nel contenuto
  <pre>fullText non contiene 'hello'</pre>
* Cerca i file che contengono la frase esatta &quot;hello world&quot; nel contenuto
  <pre>fullText contiene '"hello world"'fullText contiene '"hello_world"'</pre>
* Cercare i file con una query contenente il carattere &quot;\&quot; (ad esempio, &quot;\authors&quot;)
  <pre>fullText contiene "\\authors"</pre>
* Cerca file scrivibili dall&#39;utente &quot;test@example.org&quot;
  <pre>'test@example.org' in [!DNL writers]</pre>
* Cercare l&#39;ID `1234567` nella raccolta `parents`. Verranno trovati tutti i file e le cartelle che si trovano direttamente nella cartella con ID `1234567`.
  <pre>'1234567' in [!UICONTROL parent]</pre>
* Cercare l&#39;ID alias `appDataFolder` nella raccolta `parents`. Questo consente di trovare tutti i file e le cartelle che si trovano direttamente nella [cartella Dati applicazioni](https://developers.google.com/drive/api/v2/appdata).
  <pre>'appDataFolder' negli elementi padre</pre>
* Cerca file scrivibili dagli utenti &quot;test@example.org&quot; e &quot;test2@example.org&quot;
  <pre>'test@example.org' negli autori e 'test2@example.org' negli autori</pre>
* Cerca i file che contengono il testo &quot;importante&quot; nel cestino
  <pre>fullText contiene 'important' e cestino = true</pre>
* Cerca i file modificati dopo il 4 giugno 2012
  <pre>modifiedDate &gt; '2012-06-04T12:00:00' // fuso orario predefinito: UTC</pre><pre>modifiedDate &gt; '2012-06-04T12:00:00-08:00'</pre>
* Cerca i file condivisi con l’utente autorizzato con &quot;hello&quot; nel nome
  <pre>sharedWithMe e il titolo contiene 'hello'</pre>
* Cercare i file con una [proprietà di file personalizzata](https://developers.google.com/drive/api/v2/properties) denominata `additionalID` con il valore `8e8aceg2af2ge72e78`.
  <pre>proprietà con { key='additionalID' e value='8e8aceg2af2ge72e78' e visibility='PRIVATE' }</pre>

Il Source di questa guida è [[!DNL Google Drive] documentazione](https://developers.google.com/drive/api/v2/search-shareddrives).
