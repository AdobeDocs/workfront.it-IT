---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;agile-and-teams;user-management
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli unità team Google
description: La [!DNL Adobe Workfront Fusion Google Team Drive] i moduli consentono di monitorare, caricare, aggiornare, copiare, eliminare o recuperare file e creare cartelle nelle [!DNL Google Shared] Guida.
author: Becky
feature: Workfront Fusion
exl-id: 8b4c057f-bb98-44d1-9b71-cbeaa402a1c3
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1258'
ht-degree: 0%

---

# [!DNL Google Team Drive] moduli

La [!DNL Adobe Workfront Fusion] [!DNL Google Team Drive] i moduli consentono di monitorare, caricare, aggiornare, copiare, eliminare o recuperare file e creare cartelle nelle [!DNL Google Shared Drive].

Per utilizzare [!DNL Google Team Drive] con [!DNL Adobe Workfront Fusion], è necessario disporre di un [!DNL G Suite] conto. Se non ne hai uno, puoi creare una [!DNL G Suite] al [[!DNL G Suite] sito di registrazione](https://gsuite.google.com/signup/businessstarter/welcome).

In un [!DNL Adobe Workfront Fusion] puoi automatizzare i flussi di lavoro che utilizzano [!DNL Google Team Drive], nonché collegarlo a più applicazioni e servizi di terze parti.

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

Per utilizzare [!DNL Google Team Drive] moduli, è necessario disporre di un [!DNL Google Team Drive].

## [!DNL Google Team Drive] moduli e relativi campi

Quando si configura [!DNL Google Team Drive] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL Google Team Drive] potrebbero essere visualizzati, a seconda di fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Campi di dialogo del modulo visualizzati in **audace** (in [!DNL Workfront Fusion] scenario, **not** in questo articolo della documentazione) sono obbligatori.

Se trovi il pulsante mappa sopra un campo o una funzione, puoi utilizzarlo per impostare variabili e funzioni per quel campo. Per ulteriori informazioni, consulta [Mappare informazioni da un modulo a un altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

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
   <td> <p>Per istruzioni su come collegare le [!DNL Google Team Drive] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Team Drive]</td> 
   <td> <p> Selezionare l'unità condivisa che si desidera controllare.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cartella] </td> 
   <td> <p>Selezionare la cartella all'interno dell'unità condivisa.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Quali file controllare]</td> 
   <td> <p> Selezionare il tipo di file che si desidera controllare.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converti [!DNL Google Documents] file da formattare] </td> 
   <td> <p>Selezionare il formato desiderato [!DNL Google Documents] file convertiti in.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converti [!DNL Google Sheets] file da formattare] </td> 
   <td> <p>Selezionare il formato desiderato [!DNL Google Sheets] file convertiti in.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converti [!DNL Google Slides] file da formattare] </td> 
   <td> <p>Selezionare il formato desiderato [!DNL Google Slides] file convertiti in.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converti [!DNL Google Drawings] file da formattare] </td> 
   <td> <p>Selezionare il formato desiderato [!DNL Google Drawings] file convertiti in.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td> <p> Seleziona se desideri monitorare la cartella per i file nuovi e modificati o solo per i nuovi file.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Numero massimo di file scaricati]</td> 
   <td> <p> Imposta il numero massimo di file [!DNL Workfront Fusion] tornerà durante un ciclo di esecuzione.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Azioni

* [[!UICONTROL Caricare un file]](#upload-a-file)
* [[!UICONTROL Aggiornare un file]](#update-a-file)
* [[!UICONTROL Copia un file]](#copy-a-file)
* [[!UICONTROL Eliminare un file]](#delete-a-file)
* [[!UICONTROL Sposta un file nel cestino]](#move-a-file-to-trash)
* [[!UICONTROL Ottieni un file]](#get-a-file)
* [[!UICONTROL Ottieni elenco file]](#get-a-file-list)
* [[!UICONTROL Creare una cartella]](#create-a-folder)

#### [!UICONTROL Caricare un file]

Carica un file sull&#39;unità condivisa specificata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google Team Drive] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Team Drive] </td> 
   <td> <p>Selezionare l'unità condivisa in cui si desidera caricare un file.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cartella] </td> 
   <td> <p>Selezionare la cartella all'interno dell'unità condivisa.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL File di origine]</p> </td> 
   <td> <p>Specifica il file da caricare nell'unità condivisa.</p> <p>Mappa il file da caricare dal modulo precedente (ad es. [!UICONTROL HTTP] &gt;[!UICONTROL Ottieni un file] o [!UICONTROL Dropbox] &gt;[!UICONTROL Ottieni un file)], oppure immetti manualmente il nome del file e i dati del file.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Title]</td> 
   <td> <p> Immetti il titolo del file che verrà visualizzato nella cartella condivisa.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convertire un file]</td> 
   <td> <p> Abilita questa opzione per convertire il file nel formato Google corrispondente nella cartella condivisa.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggiornare un file]

Consente di modificare il nome file e/o il contenuto del file.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google Team Drive] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Team Drive]</td> 
   <td> <p> Selezionare l'unità condivisa contenente il file da aggiornare.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cartella] </td> 
   <td> <p>Selezionare la cartella all'interno dell'unità condivisa.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File ID]</td> 
   <td> <p> Immetti (mappa) l’ID del file da aggiornare.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL File di origine]</p> </td> 
   <td>Selezionare un file di origine da un modulo precedente o mappare il nome e i dati del file di origine.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Title] </td> 
   <td> <p>Inserisci il nuovo titolo per il file aggiornato.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convertire un file]</td> 
   <td> <p> Abilita questa opzione per convertire il file nel corrispondente [!DNL Google] nella cartella condivisa.</p> </td> 
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
   <td> <p>Per istruzioni su come collegare le [!DNL Google Team Drive] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Team Drive]</td> 
   <td> <p> Selezionare l'unità condivisa contenente il file da copiare.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cartella] </td> 
   <td> <p>Selezionare la cartella di destinazione in cui si desidera copiare il file.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File ID]</td> 
   <td> <p> Immetti (mappa) l’ID del file da copiare.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Il nome del file di copia]</p> </td> 
   <td> <p>Immettere il nuovo nome file se si desidera modificarlo nel percorso di destinazione.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminare un file]

Elimina un file specificato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google Team Drive] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File ID]</td> 
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
   <td> <p>Per istruzioni su come collegare le [!DNL Google Team Drive] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File ID]</td> 
   <td> <p> Immetti o mappa l'ID del file da spostare nel cestino.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottieni un file]

Recupera i dettagli sul file specificato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google Team Drive] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converti [!DNL Google Documents] file da formattare] </td> 
   <td> <p>Seleziona il formato desiderato per la [!DNL Google Documents] file convertiti in.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converti [!DNL Google Sheets] file da formattare] </td> 
   <td> <p>Seleziona il formato desiderato per la [!DNL Google Sheets] file convertiti in.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converti [!DNL Google Slides] file da formattare] </td> 
   <td> <p>Seleziona il formato desiderato per la [!DNL Google Slides] file convertiti in.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converti [!DNL Google Drawings] file da formattare] </td> 
   <td> <p>Seleziona il formato desiderato per la [!DNL Google Drawings] file convertiti in.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File ID]</td> 
   <td> <p> Immetti o mappa l’ID del file da recuperare.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottieni elenco file]

Recupera i dettagli di file e/o cartelle in base al termine di ricerca.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google Team Drive] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Team Drive]</td> 
   <td> <p> Selezionare l'unità condivisa da cui si desidera elencare i file.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cartella] </td> 
   <td> <p>Selezionare la cartella da cui si desidera elencare i file.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Search] </td> 
   <td> <p>Seleziona il tipo di ricerca che desideri eseguire, vedi di seguito.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Query [!UICONTROL]</p> </td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>[!UICONTROL Cerca nei nomi dei file]</p> <p style="font-weight: normal;">Immetti il nome del file (inclusa l’estensione del file) quando l’opzione [!UICONTROL Cerca termine esatto Cerca] è selezionata o inserisci la parte del nome quando l’opzione [!UICONTROL Cerca nomi contenenti il termine ricercato] è selezionata.</p> </li> 
     <li> <p style="font-weight: bold;">[!UICONTROL Ricerca full-text]</p> <p>Immettere il termine di ricerca da cercare nei nomi, nelle descrizioni e nei contenuti dei file.</p> </li> 
     <li> <p style="font-weight: bold;">[!UICONTROL Query di ricerca personalizzata]</p> <p>Inserisci il [!DNL Google] termine della query di ricerca. Per maggiori dettagli, consulta [!DNL Google]s <a href="https://developers.google.com/drive/api/v2/ref-search-terms">Documentazione query di ricerca</a>. Esempio: <code>fullText contains '"Hello world"'</code></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Retrieve]</td> 
   <td>Seleziona se desideri recuperare file, cartelle o entrambi.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Numero massimo di risultati restituiti]</td> 
   <td> <p> Imposta il numero massimo di file o cartelle [!DNL Workfront Fusion] tornerà durante un ciclo di esecuzione.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Creare una cartella]

Crea una nuova cartella.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google Team Drive] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Team Drive]</td> 
   <td> <p> Selezionare l'unità condivisa in cui si desidera creare una cartella.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cartella] </td> 
   <td> <p>Selezionare la cartella in cui si desidera creare una cartella.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Il nome della nuova cartella]</td> 
   <td> <p> Immettere il nome della nuova cartella.</p> </td> 
  </tr> 
 </tbody> 
</table>
