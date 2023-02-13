---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli Microsoft OneDrive
description: In un [!DNL Adobe Workfront Fusion] In questo caso, è possibile automatizzare i flussi di lavoro che utilizzano OneDrive e collegarli a più applicazioni e servizi di terze parti.
author: Becky
feature: Workfront Fusion
exl-id: 13a25c6c-bdf1-467d-bd90-ebd763c59235
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '3934'
ht-degree: 0%

---

# [!DNL Microsoft OneDrive] moduli

In un [!DNL Adobe Workfront Fusion] puoi automatizzare i flussi di lavoro che utilizzano [!DNL OneDrive], nonché collegarlo a più applicazioni e servizi di terze parti.

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

Per utilizzare [!DNL OneDrive] moduli, è necessario disporre di un [!DNL Microsoft OneDrive] conto.

## Collegamento della [!DNL OneDrive] servizio a [!DNL Workfront Fusion]

Per istruzioni su come collegare le [!DNL OneDrive] account a [!UICONTROL Workfront Fusion], vedi [Creare una connessione a [!UICONTROL Adobe Workfront Fusion] - Istruzioni di base](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!DNL Microsoft OneDrive] moduli e relativi campi

Quando si configura [!DNL OneDrive] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL OneDrive] potrebbero essere visualizzati, a seconda di fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se trovi il pulsante mappa sopra un campo o una funzione, puoi utilizzarlo per impostare variabili e funzioni per quel campo. Per ulteriori informazioni, consulta [Mappare informazioni da un modulo a un altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [File/Cartella](#filefolder)
* [Altro](#other)

### File/Cartella

* [[!UICONTROL Visualizza file/cartelle]](#watch-filesfolders)
* [[!UICONTROL Cerca file/cartelle]](#search-filesfolders)
* [[!UICONTROL Ottieni un file]](#get-a-file)
* [[!UICONTROL Scaricare un file]](#download-a-file)
* [[!UICONTROL Caricare un file]](#upload-a-file)
* [[!UICONTROL Creare una cartella]](#create-a-folder)
* [[!UICONTROL Ottieni collegamento condivisione]](#get-a-share-link)
* [[!UICONTROL Spostare un file o una cartella]](#move-a-filefolder)
* [[!UICONTROL Copia un file]](#copy-a-file)
* [[!UICONTROL Eliminare un file/cartella]](#delete-a-filefolder)

#### [!UICONTROL Visualizza file/cartelle]

Questo modulo di attivazione avvia uno scenario in cui viene creato o aggiornato un file o una cartella.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Per istruzioni su come collegare le [!DNL OneDrive] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Guarda file/cartelle]</td> 
   <td> <p>Selezionare la modalità di controllo dei file o delle cartelle:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Per Ora Di Creazione]</b> </p> <p>Cerca nuovi file o cartelle.</p> </li> 
     <li> <p><b>[!UICONTROL Per Ora Di Aggiornamento]</b> </p> <p>Cerca file o cartelle esistenti aggiornati.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scegli la tua [!DNL OneDrive] ubicazione]</td> 
   <td> <p>Seleziona la posizione da guardare:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>Seleziona se abilitare il modulo per immettere un ID unità.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sì]</b> </p> <p>Immettere l'ID dell'unità che si desidera controllare nel modulo.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> <p>Passa alla cartella che desideri controllare nel modulo. È inoltre possibile immettere una query per filtrare i risultati restituiti.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Condiviso Con Me]</b> </p> <p>Il modulo controlla i file che sono stati condivisi con il proprietario dell'unità.</p> </li> 
     <li> <p><b>Unità del sito</b> </p> <p>Seleziona il sito SharePoint da controllare nel modulo. I siti disponibili sono Sites seguiti dall’utente connesso.</p> </li> 
     <li> <p><b>Unità del gruppo [!UICONTROL]</b> </p> <p>Selezionare il gruppo di cui si desidera controllare l'unità del modulo.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scegli un tipo di articolo]</td> 
   <td> <p>Selezionare se si desidera guardare file, cartelle o entrambi.</p> <p>Nota: Non è possibile cercare le cartelle in un'unità [!UICONTROL Shared With Me].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Immettere o mappare il numero massimo di record che si desidera restituire dal modulo durante ogni ciclo di esecuzione degli scenari.</p> </td> 
  </tr> 
 </tbody> 
</table>



#### [!UICONTROL Cerca file/cartelle]

Questo modulo di ricerca restituisce file e cartelle in base ai criteri impostati.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Per istruzioni su come collegare le [!DNL OneDrive] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scegli la tua [!DNL OneDrive] ubicazione]</td> 
   <td> <p>Seleziona il percorso da cercare:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>Seleziona se abilitare il modulo per immettere un ID unità.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sì]</b> </p> <p>Immettere l'ID dell'unità in cui si desidera eseguire la ricerca nel modulo.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> <p>Passa alla cartella in cui desideri eseguire la ricerca del modulo. È inoltre possibile immettere una query per filtrare i risultati restituiti.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Condiviso Con Me]</b> </p> <p>Il modulo cerca i file condivisi con il proprietario dell'unità.</p> </li> 
     <li> <p><b>Unità del sito</b> </p> <p>Seleziona la [!DNL SharePoint] Sito in cui si desidera eseguire la ricerca nel modulo. I siti disponibili sono Sites seguiti dall’utente connesso.</p> </li> 
     <li> <p><b>Unità del gruppo [!UICONTROL]</b> </p> <p>Selezionare il gruppo di cui si desidera eseguire la ricerca nel modulo.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scegli un tipo di articolo]</td> 
   <td> <p>Selezionare se si desidera cercare file, cartelle o entrambi.</p> <p>Nota: Non è possibile cercare cartelle in un'unità [!UICONTROL Shared With Me].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Immettere o mappare il numero massimo di record che si desidera restituire dal modulo durante ogni ciclo di esecuzione degli scenari.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottieni un file]

Questo modulo di azione ottiene i metadati di un file specificato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Per istruzioni su come collegare le [!DNL OneDrive] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Invio (ID file e percorso file)]</td> 
   <td>Selezionare se si desidera identificare il file per ID file o per percorso file.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inserisci un ID file] / [!UICONTROL File Path]</td> 
   <td> <p>Selezionare la modalità di immissione dell'ID file o del percorso file:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Invio manuale]</b> </p> <p>Seleziona questa opzione se desideri immettere direttamente l’ID o il percorso oppure mapparlo da un modulo precedente.</p> </li> 
     <li> <p><b>[!UICONTROL Seleziona da un elenco]</b> </p> <p>Selezionare questa opzione se si desidera selezionare da un elenco di file o percorsi disponibili. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scegli la tua [!DNL OneDrive] ubicazione]</td> 
   <td> <p>Seleziona il percorso da cercare:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>Seleziona se abilitare il modulo per immettere un ID unità.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sì]</b> </p> <p>Immettere l'ID dell'unità contenente il file che si desidera ottenere.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>Unità del sito</b> </p> <p>Selezionare il sito SharePoint contenente il file che si desidera ottenere. I siti disponibili sono Sites seguiti dall’utente connesso.</p> </li> 
     <li> <p><b>Unità del gruppo [!UICONTROL]</b> </p> <p>Selezionare il gruppo di cui l'unità contiene il file che si desidera ottenere.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID unità]</td> 
   <td> <p>Selezionare o mappare l'unità contenente il file che si desidera ottenere. Questo campo non è disponibile se hai selezionato [!UICONTROL No] nel campo [!UICONTROL Abilita per immettere un ID unità].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File] / [!UICONTROL File ID] / [!UICONTROL File Path]</td> 
   <td> <p>Se hai selezionato [!UICONTROL Invio manuale], immetti o mappa l’ID file o il percorso del file che desideri ottenere.</p> <p>Se hai selezionato [!UICONTROL Seleziona dall’elenco], seleziona il file da ottenere.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Scaricare un file]

Questo modulo di azione scarica il file specificato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Per istruzioni su come collegare le [!DNL OneDrive] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Invio (ID file e percorso file)]</td> 
   <td>Selezionare se si desidera identificare il file per ID file o per percorso file.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Immettere un ID file/percorso file</td> 
   <td> <p>Selezionare la modalità di immissione dell'ID file o del percorso file:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Invio manuale]</b> </p> <p>Seleziona questa opzione se desideri immettere direttamente l’ID o il percorso oppure mapparlo da un modulo precedente.</p> </li> 
     <li> <p><b>[!UICONTROL Seleziona da un elenco]</b> </p> <p>Selezionare questa opzione se si desidera selezionare da un elenco di file o percorsi disponibili. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scegli la tua [!DNL OneDrive] ubicazione]</td> 
   <td> <p>Seleziona il percorso in cui desideri inserire il file da scaricare:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>Seleziona se abilitare il modulo per immettere un ID unità.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sì]</b> </p> <p>Immettere l'ID dell'unità contenente il file da scaricare.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>Unità del sito</b> </p> <p>Selezionare il sito SharePoint contenente il file da scaricare. I siti disponibili sono Sites seguiti dall’utente connesso.</p> </li> 
     <li> <p><b>Unità del gruppo [!UICONTROL]</b> </p> <p>Selezionare il gruppo di cui l'unità contiene il file da scaricare.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID unità]</td> 
   <td> <p>Selezionare o mappare l'unità contenente il file che si desidera scaricare. Questo campo non è disponibile se hai selezionato [!UICONTROL No] nel campo [!UICONTROL Abilita per immettere un ID unità].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File] / [!UICONTROL File ID] / [!UICONTROL File Path]</td>
   <td> <p>Se hai selezionato [!UICONTROL Invio manuale], immetti o mappa l’ID file o il percorso del file da scaricare.</p> <p>Se hai selezionato [!UICONTROL Seleziona dall’elenco], seleziona il file da scaricare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Converti in PDF]</td> 
   <td> <p>Abilitare questa opzione per convertire il file in un file PDF. Puoi convertire i seguenti tipi di file:</p> 
    <table style="table-layout:auto"> 
     <col> 
     <col> 
     <col> 
     <tbody> 
      <tr> 
       <td> 
        <ul> 
         <li> <p> <p>CSV</p> </p> </li> 
         <li> <p> <p>DOC</p> </p> </li> 
         <li> <p> <p>DOCX</p> </p> </li> 
         <li> <p> <p>ODP</p> </p> </li> 
         <li> <p> <p>ODS</p> </p> </li> 
         <li> <p> <p>ODT</p> </p> </li> 
        </ul> </td> 
       <td> 
        <ul> 
         <li> <p> <p>STAZIONE</p> </p> </li> 
         <li> <p> <p>POTM</p> </p> </li> 
         <li> <p> <p>POTX</p> </p> </li> 
         <li> <p> <p>PPS</p> </p> </li> 
         <li> <p> <p>PPSX</p> </p> </li> 
         <li> <p> <p>PPSXM</p> </p> </li> 
        </ul> </td> 
       <td> 
        <ul> 
         <li> <p>PPT</p> </li> 
         <li> <p>PPTM</p> </li> 
         <li> <p>PPTX</p> </li> 
         <li> <p>RTF</p> </li> 
         <li> <p>XLS</p> </li> 
         <li> <p>XLSX</p> </li> 
        </ul> </td> 
      </tr> 
     </tbody> 
    </table> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Caricare un file]

Questo modulo di azione carica un file nella cartella specificata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Per istruzioni su come collegare le [!DNL OneDrive] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Invio (ID posizione cartella e percorso)</td> 
   <td>Seleziona se identificare la cartella di destinazione per ID o per percorso.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scegli la tua [!DNL OneDrive] ubicazione]</td> 
   <td> <p>Seleziona il percorso in cui vuoi caricare un file:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>Seleziona se abilitare il modulo per immettere un ID unità.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sì]</b> </p> <p>Selezionare l'unità contenente il file che si desidera ottenere.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>Unità del sito</b> </p> <p>Seleziona la [!DNL SharePoint] Sito contenente la cartella in cui desideri caricare un file. I siti disponibili sono Sites seguiti dall’utente connesso.</p> </li> 
     <li> <p><b>Unità del gruppo [!UICONTROL]</b> </p> <p>Selezionare il gruppo di cui l'unità contiene la cartella in cui si desidera caricare un file.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID unità]</td> 
   <td> <p>Selezionare l'unità che contiene la cartella in cui si desidera caricare un file. Questo campo non è disponibile se hai selezionato [!UICONTROL No] nel campo [!UICONTROL Abilita per immettere un ID unità].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File di origine]</td> 
   <td> <p>Selezionare un file di origine da un modulo precedente o mappare il nome e i dati del file di origine.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Se esiste un file con lo stesso nome]</td> 
   <td>Selezionare la procedura da seguire se esiste già un file con lo stesso nome.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Descrizione]</td> 
   <td>Aggiungi una descrizione al file caricato.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Creare una cartella]

Questo modulo di azione crea una nuova cartella nell&#39;unità specificata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Per istruzioni su come collegare le [!DNL OneDrive] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scegli la tua [!DNL OneDrive] ubicazione]</td> 
   <td> <p>Selezionare il percorso in cui si desidera creare una cartella:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>Seleziona se abilitare il modulo per immettere un ID unità.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sì]</b> </p> <p>Selezionare l'unità in cui si desidera creare una cartella.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>Unità del sito</b> </p> <p>Seleziona la [!DNL SharePoint] Sito in cui si desidera creare una cartella. I siti disponibili sono Sites seguiti dall’utente connesso.</p> </li> 
     <li> <p><b>Unità del gruppo [!UICONTROL]</b> </p> <p>Selezionare il gruppo proprietario dell'unità in cui si desidera creare una cartella.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID unità]</td> 
   <td> <p>Selezionare l'unità in cui si desidera creare una cartella. Questo campo non è disponibile se hai selezionato [!UICONTROL No] nel campo [!UICONTROL Abilita per immettere un ID unità].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cartella]</td> 
   <td>Se desideri che la nuova cartella sia una sottocartella, passa alla cartella in cui desideri che sia una sottocartella.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nuovo Nome Cartella]</td> 
   <td> <p>Immettere o mappare un nome per la nuova cartella.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Se esiste una cartella con lo stesso nome]</td> 
   <td>Selezionare la procedura da seguire se esiste già un file con lo stesso nome.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottieni collegamento condivisione]

Questo modulo di azione restituisce un collegamento di condivisione per il file specificato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Per istruzioni su come collegare le [!DNL OneDrive] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Invio (ID file e percorso file)]</td> 
   <td>Selezionare se si desidera identificare il file per ID file o per percorso file.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inserisci un ID file] / [!UICONTROL File Path]</td> 
   <td> <p>Selezionare la modalità di immissione dell'ID file o del percorso file:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Invio manuale]</b> </p> <p>Seleziona questa opzione se desideri immettere direttamente l’ID o il percorso oppure mapparlo da un modulo precedente.</p> </li> 
     <li> <p><b>[!UICONTROL Seleziona da un elenco]</b> </p> <p>Selezionare questa opzione se si desidera selezionare da un elenco di file o percorsi disponibili. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scegli la tua [!DNL OneDrive] ubicazione]</td> 
   <td> <p>Seleziona la posizione per la quale desideri recuperare un collegamento di condivisione per:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>Seleziona se abilitare il modulo per immettere un ID unità.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sì]</b> </p> <p>Immettere l'ID dell'unità contenente il file per il quale si desidera recuperare un collegamento di condivisione.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>Unità del sito</b> </p> <p>Selezionare il sito SharePoint contenente il file per il quale si desidera recuperare un collegamento di condivisione. I siti disponibili sono Sites seguiti dall’utente connesso.</p> </li> 
     <li> <p><b>Unità del gruppo [!UICONTROL]</b> </p> <p>Selezionare il gruppo di cui l'unità contiene il file per il quale si desidera recuperare un collegamento di condivisione.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID unità]</td> 
   <td> <p>Selezionare o mappare l'unità contenente il file per il quale si desidera recuperare un collegamento di condivisione. Questo campo non è disponibile se hai selezionato [!UICONTROL No] nel campo [!UICONTROL Abilita per immettere un ID unità].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File] / [!UICONTROL File ID] / [!UICONTROL File Path]</td> 
   <td> <p>Se hai selezionato [!UICONTROL Invio manuale], immetti o mappa l’ID file o il percorso del file per il quale desideri recuperare un collegamento di condivisione.</p> <p>Se hai selezionato [!UICONTROL Select] dall'elenco, seleziona il file per il quale desideri recuperare un collegamento di condivisione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Permission Type]</td> 
   <td> <p>Seleziona se vuoi che gli utenti con il collegamento siano in grado di leggere e scrivere sul file o di leggere solo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ambito [!UICONTROL]</td> 
   <td>Seleziona se rendere il file disponibile a chiunque disponga del collegamento o solo ai membri della tua organizzazione che lo dispongono.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Spostare un file o una cartella]

Questo modulo di azione sposta un file o una cartella in una nuova posizione di cartella

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Per istruzioni su come collegare le [!DNL OneDrive] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Invio (ID file e percorso file)]</td> 
   <td>Selezionare se si desidera identificare il file per ID file o per percorso file.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inserisci un ID file / Percorso file]</td> 
   <td> <p>Selezionare la modalità di immissione dell'ID file o del percorso file:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Invio manuale]</b> </p> <p>Seleziona questa opzione se desideri immettere direttamente l’ID o il percorso oppure mapparlo da un modulo precedente.</p> </li> 
     <li> <p><b>[!UICONTROL Seleziona da un elenco]</b> </p> <p>Selezionare questa opzione se si desidera selezionare da un elenco di file o percorsi disponibili. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scegli la tua [!DNL OneDrive] ubicazione]</td> 
   <td> <p>Selezionare il percorso contenente il file o la cartella che si desidera spostare:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>Seleziona se abilitare il modulo per immettere un ID unità.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sì]</b> </p> <p>Immettere l'ID dell'unità contenente il file o la cartella che si desidera spostare.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>Unità del sito</b> </p> <p>Seleziona la [!DNL SharePoint] Sito contenente il file o la cartella da spostare. I siti disponibili sono Sites seguiti dall’utente connesso.</p> </li> 
     <li> <p><b>Unità del gruppo [!UICONTROL]</b> </p> <p>Selezionare il gruppo di cui l'unità contiene il file o la cartella che si desidera spostare.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID unità]</td> 
   <td> <p>Selezionare o mappare l'unità contenente il file o la cartella che si desidera spostare. Questo campo non è disponibile se hai selezionato [!UICONTROL No] nel campo [!UICONTROL Abilita per immettere un ID unità].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Seleziona [!UICONTROL File/Cartella]</td> 
   <td>Selezionare se si desidera spostare un file o una cartella.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!UICONTROL File] / [!UICONTROL File ID] / [!UICONTROL File Path]</p> <p role="rowheader">[!UICONTROL Folder] / [!UICONTROL Folder ID] / [!UICONTROL Folder Path]</p> </td> 
   <td> <p>Se hai selezionato [!UICONTROL Invio manuale], immetti o mappa l’ID o il percorso del file o della cartella da spostare.</p> <p>Se hai selezionato [!UICONTROL Select] dall’elenco, seleziona il file o la cartella da spostare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inserisci una nuova posizione cartella]</td> 
   <td> <p>Selezionare la posizione in cui si desidera inserire il percorso in cui si desidera spostare il file o la cartella:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Invio manuale]</b> </p> <p>Seleziona questa opzione se desideri immettere direttamente l’ID o il percorso oppure mapparlo da un modulo precedente.</p> </li> 
     <li> <p><b>[!UICONTROL Seleziona da un elenco]</b> </p> <p>Selezionare questa opzione se si desidera selezionare da un elenco di file o percorsi disponibili. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scegli la tua [!DNL OneDrive] ubicazione]</td> 
   <td> <p>Selezionare il percorso in cui si desidera spostare il file o la cartella:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>Seleziona se abilitare il modulo per immettere un ID unità.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sì]</b> </p> <p>Immettere l'ID dell'unità in cui si desidera spostare il file o la cartella.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>Unità del sito</b> </p> <p>Seleziona la [!DNL SharePoint] Sito in cui si desidera spostare il file o la cartella. I siti disponibili sono Sites seguiti dall’utente connesso.</p> </li> 
     <li> <p><b>Unità del gruppo [!UICONTROL]</b> </p> <p>Selezionare il gruppo in cui si desidera spostare il file o la cartella.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID unità]</td> 
   <td> <p>Selezionare o mappare l'unità contenente la cartella in cui si desidera spostare il file o la cartella. Questo campo non è disponibile se hai selezionato [!UICONTROL No] nel campo [!UICONTROL Abilita per immettere un ID unità].</p> <p>Se si lascia vuoto questo campo, il file o la cartella possono essere spostati solo all'interno della stessa [!DNL OneDrive].</p> <p>Puoi spostare file e cartelle da [!UICONTROL My Drive] a un'unità del sito o a un'unità del gruppo. </p> <p>È possibile spostare i file da un'unità del sito solo alla stessa unità nello stesso sito.</p> <p>È possibile spostare i file da un'unità di un gruppo solo alla stessa unità nello stesso gruppo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cartella]</td> 
   <td>Immettere o mappare la cartella in cui si desidera spostare il file o la cartella.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Copia un file]

Questo modulo di azione copia un file in una nuova posizione di cartella

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Per istruzioni su come collegare le [!DNL OneDrive] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Invio (ID file e percorso file)]</td> 
   <td>Selezionare se si desidera identificare il file per ID file o per percorso file.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inserisci un ID file] / [!UICONTROL File Path]</td> 
   <td> <p>Selezionare la modalità di immissione dell'ID file o del percorso file:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Invio manuale]</b> </p> <p>Seleziona questa opzione se desideri immettere direttamente l’ID o il percorso oppure mapparlo da un modulo precedente.</p> </li> 
     <li> <p><b>[!UICONTROL Seleziona da un elenco]</b> </p> <p>Selezionare questa opzione se si desidera selezionare da un elenco di file o percorsi disponibili. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scegli la tua [!DNL OneDrive] ubicazione]</td> 
   <td> <p>Selezionare il percorso contenente il file da copiare:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>Seleziona se abilitare il modulo per immettere un ID unità.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sì]</b> </p> <p>Immettere l'ID dell'unità contenente il file o la cartella che si desidera copiare.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>Unità del sito</b> </p> <p>Selezionare il sito SharePoint contenente il file da spostare. I siti disponibili sono Sites seguiti dall’utente connesso.</p> </li> 
     <li> <p><b>Unità del gruppo [!UICONTROL]</b> </p> <p>Selezionare il gruppo di cui l'unità contiene il file da copiare.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID unità]</td> 
   <td> <p>Selezionare o mappare l'unità contenente il file che si desidera copiare. Questo campo non è disponibile se hai selezionato [!UICONTROL No] nel campo [!UICONTROL Abilita per immettere un ID unità].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!UICONTROL File] / [!UICONTROL File ID] / [!UICONTROL File Path]</p> </td> 
   <td> <p>Se hai selezionato [!UICONTROL Invio manuale], immetti o mappa l’ID o il percorso del file da copiare.</p> <p>Se hai selezionato [!UICONTROL Select] dall’elenco, seleziona il file da copiare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inserisci una nuova posizione cartella]</td> 
   <td> <p>Selezionare la modalità di immissione del percorso in cui si desidera copiare il file o:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Invio manuale]</b> </p> <p>Seleziona questa opzione se desideri immettere direttamente l’ID o il percorso oppure mapparlo da un modulo precedente.</p> </li> 
     <li> <p><b>[!UICONTROL Seleziona da un elenco]</b> </p> <p>Selezionare questa opzione se si desidera selezionare da un elenco di cartelle disponibili. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nuovo percorso OneDrive]</td> 
   <td> <p>Selezionare la posizione in cui si desidera copiare il filtro. Questa opzione è disponibile se si sceglie di selezionare il nuovo percorso della cartella da un elenco.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>Seleziona se abilitare il modulo per immettere un ID unità.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sì]</b> </p> <p>Immettere l'ID dell'unità in cui si desidera copiare il file.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>Unità del sito</b> </p> <p>Seleziona la [!DNL SharePoint] Sito in cui si desidera copiare il file. I siti disponibili sono Sites seguiti dall’utente connesso.</p> </li> 
     <li> <p><b>Unità del gruppo [!UICONTROL]</b> </p> <p>Selezionare il gruppo in cui si desidera copiare il file.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID unità]</td> 
   <td> <p>Selezionare o mappare l'unità contenente la cartella in cui si desidera copiare il file. Questo campo non è disponibile se hai selezionato [!UICONTROL No] nel campo [!UICONTROL Abilita per immettere un ID unità].</p> <p>Se lasci questo vuoto, il file o la cartella possono essere copiati solo all'interno dello stesso [!UICONTROL OneDrive].</p> <p>Puoi copiare file e cartelle da [!UICONTROL My Drive] a un'unità del sito o a un'unità del gruppo. </p> <p>È possibile copiare i file da un'unità del sito solo nella stessa unità nello stesso sito.</p> <p>È possibile copiare i file da un'unità di un gruppo solo nella stessa unità nello stesso gruppo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cartella]</td> 
   <td>Immettere o mappare la cartella in cui si desidera spostare la copia o la cartella.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nuovo Nome File Copiato]</td> 
   <td> <p>Immettere o mappare un nome per la nuova copia del file. È possibile lasciare vuoto questo campo se non si desidera modificare il nome del file originale.</p> <p>Il nome deve includere l’estensione del file. Esempio:<code> file.txt</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminare un file/cartella]

Questo modulo di azione elimina il file selezionato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Per istruzioni su come collegare le [!DNL OneDrive] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Invio (ID e percorso file/cartelle)]</td> 
   <td>Selezionare se si desidera identificare il file per ID file o per percorso file.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inserisci un ID file/cartella /Inserisci un percorso file/cartella]</td> 
   <td> <p>Selezionare la modalità di immissione dell'ID file o del percorso file:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Invio manuale]</b> </p> <p>Seleziona questa opzione se desideri immettere direttamente l’ID o il percorso oppure mapparlo da un modulo precedente.</p> </li> 
     <li> <p><b>[!UICONTROL Seleziona da un elenco]</b> </p> <p>Selezionare questa opzione se si desidera selezionare da un elenco di file o percorsi disponibili. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scegli la tua [!DNL OneDrive] ubicazione]</td> 
   <td> <p>Seleziona il percorso da cercare:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>Seleziona se abilitare il modulo per immettere un ID unità.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sì]</b> </p> <p>Immettere l'ID dell'unità contenente il file o la cartella che si desidera eliminare.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>Unità del sito</b> </p> <p>Seleziona la [!DNL SharePoint] Sito contenente il file o la cartella da eliminare. I siti disponibili sono Sites seguiti dall’utente connesso.</p> </li> 
     <li> <p><b>Unità del gruppo [!UICONTROL]</b> </p> <p>Selezionare il gruppo di cui l'unità contiene il file o la cartella che si desidera eliminare.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID unità]</td> 
   <td> <p>Selezionare o mappare l'unità contenente il file o la cartella che si desidera eliminare. Questo campo non è disponibile se hai selezionato [!UICONTROL No] nel campo [!UICONTROL Abilita per immettere un ID unità].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Seleziona [!UICONTROL File/Cartella]</td> 
   <td>Selezionare se si desidera eliminare un file o una cartella.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File] / [!UICONTROL File ID] / [!UICONTROL File Path]</td>
   <td> <p>Se hai selezionato [!UICONTROL Invio manuale], immetti o mappa l’ID file o il percorso del file da eliminare.</p> <p>Se hai selezionato [!UICONTROL Select] dall’elenco, seleziona il file da eliminare.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Altro

#### [!UICONTROL Effettuare una chiamata API]

Questo modulo esegue una chiamata API personalizzata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Per istruzioni su come collegare le [!DNL OneDrive] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Immettere un percorso relativo a <code>https://graph.microsoft.com</code>. Esempio:<code> /v1.0/me/drive/root/children</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL, Metodo]</td> 
   td&gt; <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Aggiungi le intestazioni della richiesta sotto forma di un oggetto JSON standard.</p> <p>Ad esempio: <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion aggiunge le intestazioni di autorizzazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>Aggiungi la query per la chiamata API sotto forma di un oggetto JSON standard.</p> <p>Ad esempio: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Aggiungi il contenuto del corpo per la chiamata API sotto forma di un oggetto JSON standard.</p> <p>Nota:  <p>Quando si utilizzano istruzioni condizionali come <code>if</code> nel JSON, inserisci le virgolette al di fuori dell’istruzione condizionale.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>



## Se non riesci a caricare o aggiornare un file

Ci sono diversi possibili problemi quando il caricamento o l’aggiornamento di un file non riesce:

* Il file caricato è troppo grande e supera il limite massimo di dimensione del file per il tuo [!DNL OneDrive] pianifica o hai utilizzato tutti i tuoi [!DNL OneDrive] quota di archiviazione dell&#39;account. Per ottenere più spazio di archiviazione, elimina i file esistenti da [!DNL OneDrive] o aggiornare il [!DNL OneDrive] conto.
* OneDrive non consente di caricare due file con lo stesso nome in un&#39;unica cartella. Se la cartella di destinazione contiene un file con lo stesso nome del file caricato, l’esecuzione dello scenario termina con un errore. La soluzione consiste nel rinominare semplicemente il file caricato. Se lo scopo è quello di aggiornare un file, utilizza il [!UICONTROL Aggiornare un file] azione.
* La cartella selezionata in precedenza, in cui viene caricato il file, non esiste più. Lo scenario si interrompe e dovrai selezionare nuovamente la cartella di destinazione.
