---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;agile-and-teams;user-management
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli di Google Team Drive
description: I  [!DNL Adobe Workfront Fusion Google Team Drive] moduli ti consentono di monitorare, caricare, aggiornare, copiare, eliminare o recuperare file e creare cartelle nell'unità [!DNL Google Shared] .
author: Becky
feature: Workfront Fusion
exl-id: 8b4c057f-bb98-44d1-9b71-cbeaa402a1c3
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '1297'
ht-degree: 0%

---

# [!DNL Google Team Drive] moduli

I moduli [!DNL Adobe Workfront Fusion] [!DNL Google Team Drive] consentono di monitorare, caricare, aggiornare, copiare, eliminare o recuperare file e creare cartelle in [!DNL Google Shared Drive].

Per utilizzare [!DNL Google Team Drive] con [!DNL Adobe Workfront Fusion], è necessario disporre di un account [!DNL Google Workspace]. In caso contrario, è possibile creare un account [!DNL Google Workspace] nel [[!DNL Google Workspace] sito per l&#39;iscrizione](https://workspace.google.com/business/signup/welcome).

In uno scenario [!DNL Adobe Workfront Fusion], è possibile automatizzare i flussi di lavoro che utilizzano [!DNL Google Team Drive] e collegarlo a più applicazioni e servizi di terze parti.

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
   <p>Fabbisogno prodotto corrente: se disponi del piano [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront], la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo. [!DNL Workfront Fusion] è incluso nel piano [!UICONTROL Ultimate] [!DNL Workfront].</p>
   <p>Oppure</p>
   <p>Requisiti del prodotto legacy: la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Per conoscere il piano, il tipo di licenza o l&#39;accesso disponibili, contattare l&#39;amministratore [!DNL Workfront].

Per informazioni sulle [!DNL Adobe Workfront Fusion] licenze, vedere [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Prerequisiti

Per utilizzare i moduli [!DNL Google Team Drive], è necessario disporre di [!DNL Google Team Drive].

## [!DNL Google Team Drive] moduli e relativi campi

Quando configuri [!DNL Google Team Drive] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Insieme a questi, potrebbero essere visualizzati ulteriori campi di [!DNL Google Team Drive], a seconda di fattori quali il livello di accesso nell&#39;app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

I campi della finestra di dialogo del modulo visualizzati in **bold** (nello scenario [!DNL Workfront Fusion], **not** in questo articolo della documentazione) sono obbligatori.

Se viene visualizzato il pulsante Mappa sopra un campo o una funzione, è possibile utilizzarlo per impostare variabili e funzioni per tale campo. Per ulteriori informazioni, vedere [Mappare le informazioni da un modulo all&#39;altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Triggers

#### [!UICONTROL File di controllo]

Restituisce i dettagli del file quando un nuovo file viene aggiunto e/o modificato nella cartella specificata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Google Team Drive] a [!DNL Workfront Fusion], vedere <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Unità Team]</td> 
   <td> <p> Selezionare l'unità condivisa che si desidera controllare.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Selezionare la cartella nell'unità condivisa.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Quali file guardare]</td> 
   <td> <p> Selezionare il tipo di file che si desidera controllare.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converti [!DNL Google Documents] file in formato] </td> 
   <td> <p>Selezionare il formato in cui convertire i file [!DNL Google Documents] controllati.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converti [!DNL Google Sheets] file in formato] </td> 
   <td> <p>Selezionare il formato in cui convertire i file [!DNL Google Sheets] controllati.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converti [!DNL Google Slides] file in formato] </td> 
   <td> <p>Selezionare il formato in cui convertire i file [!DNL Google Slides] controllati.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converti [!DNL Google Drawings] file in formato] </td> 
   <td> <p>Selezionare il formato in cui convertire i file [!DNL Google Drawings] controllati.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td> <p> Specificare se si desidera monitorare la cartella per i file nuovi e modificati o solo per i nuovi file.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Numero massimo di file scaricati]</td> 
   <td> <p> Impostare il numero massimo di file restituiti [!DNL Workfront Fusion] durante un ciclo di esecuzione.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Azioni

* [[!UICONTROL Carica un file]](#upload-a-file)
* [[!UICONTROL Aggiorna un file]](#update-a-file)
* [[!UICONTROL Copia un file]](#copy-a-file)
* [[!UICONTROL Elimina un file]](#delete-a-file)
* [[!UICONTROL Sposta un file nel cestino]](#move-a-file-to-trash)
* [[!UICONTROL Ottieni un file]](#get-a-file)
* [[!UICONTROL Ottieni elenco file]](#get-a-file-list)
* [[!UICONTROL Crea una cartella]](#create-a-folder)

#### [!UICONTROL Carica un file]

Carica un file nell&#39;unità condivisa specificata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Google Team Drive] a [!DNL Workfront Fusion], vedere <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Unità Team] </td> 
   <td> <p>Selezionare l'unità condivisa in cui si desidera caricare un file.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Selezionare la cartella nell'unità condivisa.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Source File]</p> </td> 
   <td> <p>Specificare il file da caricare nell'unità condivisa.</p> <p>Mappa il file che desideri caricare dal modulo precedente (ad es. [!UICONTROL HTTP] &gt;[!UICONTROL Ottieni un file] o [!UICONTROL Dropbox] &gt;[!UICONTROL Ottieni un file)] oppure immettere manualmente il nome del file e i dati del file.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Title]</td> 
   <td> <p> Immettere il titolo del file che verrà visualizzato nella cartella condivisa.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converti un file]</td> 
   <td> <p> Abilita questa opzione per convertire il file nel formato Google corrispondente nella cartella condivisa.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggiorna un file]

Consente di modificare il nome e/o il contenuto del file.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Google Team Drive] a [!DNL Workfront Fusion], vedere <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Unità Team]</td> 
   <td> <p> Selezionare l'unità condivisa contenente il file che si desidera aggiornare.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Selezionare la cartella nell'unità condivisa.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID file]</td> 
   <td> <p> Immetti (mappa) l’ID del file da aggiornare.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Source File]</p> </td> 
   <td>Selezionare un file di origine da un modulo precedente o mappare il nome e i dati del file di origine.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Title] </td> 
   <td> <p>Immettere il nuovo titolo del file aggiornato.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converti un file]</td> 
   <td> <p> Abilita questa opzione per convertire il file nel formato [!DNL Google] corrispondente nella cartella condivisa.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Copia un file]

Copia un file specificato nella cartella selezionata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Google Team Drive] a [!DNL Workfront Fusion], vedere <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Unità Team]</td> 
   <td> <p> Selezionare l'unità condivisa contenente il file da copiare.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Selezionare la cartella di destinazione in cui copiare il file.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID file]</td> 
   <td> <p> Immetti (mappa) l’ID del file da copiare.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Nome del file di copia]</p> </td> 
   <td> <p>Immettere il nuovo nome del file se si desidera modificarlo nella posizione di destinazione.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Elimina un file]

Elimina un file specificato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Google Team Drive] a [!DNL Workfront Fusion], vedere <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID file]</td> 
   <td> <p> Immetti o mappa l’ID del file da eliminare.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Sposta un file nel cestino]

Sposta un file specificato nel cestino.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Google Team Drive] a [!DNL Workfront Fusion], vedere <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID file]</td> 
   <td> <p> Immetti o mappa l’ID del file da spostare nel cestino.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottieni un file]

Recupera i dettagli del file specificato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Google Team Drive] a [!DNL Workfront Fusion], vedere <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converti [!DNL Google Documents] file in formato] </td> 
   <td> <p>Selezionare il formato in cui convertire i file [!DNL Google Documents].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converti [!DNL Google Sheets] file in formato] </td> 
   <td> <p>Selezionare il formato in cui convertire i file [!DNL Google Sheets].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converti [!DNL Google Slides] file in formato] </td> 
   <td> <p>Selezionare il formato in cui convertire i file [!DNL Google Slides].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converti [!DNL Google Drawings] file in formato] </td> 
   <td> <p>Selezionare il formato in cui convertire i file [!DNL Google Drawings].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID file]</td> 
   <td> <p> Immetti o mappa l’ID del file da recuperare.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottieni elenco file]

Recupera i dettagli dei file e/o delle cartelle in base al termine di ricerca.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Google Team Drive] a [!DNL Workfront Fusion], vedere <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Unità Team]</td> 
   <td> <p> Selezionare l'unità condivisa da cui elencare i file.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Selezionare la cartella da cui si desidera elencare i file.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL - Ricerca] </td> 
   <td> <p>Seleziona il tipo di ricerca da eseguire - vedi di seguito.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Query]</p> </td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>[!UICONTROL Cerca nei nomi di file]</p> <p style="font-weight: normal;">Immettere il nome del file (inclusa l'estensione) quando l'opzione [!UICONTROL Cerca il termine esatto Cerca] è selezionata oppure immettere la parte del nome quando l'opzione [!UICONTROL Cerca i nomi contenenti il termine cercato] è selezionata.</p> </li> 
     <li> <p style="font-weight: bold;">[!UICONTROL Ricerca full-text]</p> <p>Immettere il termine di ricerca per eseguire ricerche nei nomi, nelle descrizioni e nei contenuti dei file.</p> </li> 
     <li> <p style="font-weight: bold;">[!UICONTROL Query di ricerca personalizzata]</p> <p>Immettere il termine della query di ricerca [!DNL Google]. Per ulteriori dettagli, fare riferimento alla <a href="https://developers.google.com/drive/api/v2/ref-search-terms">documentazione di ricerca query</a> di [!DNL Google]. Esempio: <code>fullText contains '"Hello world"'</code></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Retrieve]</td> 
   <td>Seleziona se desideri recuperare i file, la cartella o entrambi.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Numero massimo di risultati restituiti]</td> 
   <td> <p> Impostare il numero massimo di file o cartelle [!DNL Workfront Fusion] restituiti durante un ciclo di esecuzione.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crea una cartella]

Crea una nuova cartella.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Google Team Drive] a [!DNL Workfront Fusion], vedere <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Unità Team]</td> 
   <td> <p> Selezionare l'unità condivisa in cui si desidera creare una cartella.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Seleziona la cartella in cui desideri creare una cartella.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome della nuova cartella]</td> 
   <td> <p> Immettere il nome della nuova cartella.</p> </td> 
  </tr> 
 </tbody> 
</table>
