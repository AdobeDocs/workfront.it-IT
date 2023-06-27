---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli Microsoft OneDrive
description: In un [!DNL Adobe Workfront Fusion] scenario, è possibile automatizzare i flussi di lavoro che utilizzano OneDrive e collegarlo a più applicazioni e servizi di terze parti.
author: Becky
feature: Workfront Fusion
exl-id: 13a25c6c-bdf1-467d-bd90-ebd763c59235
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '3982'
ht-degree: 0%

---

# [!DNL Microsoft OneDrive] moduli

In un [!DNL Adobe Workfront Fusion] scenario, puoi automatizzare i flussi di lavoro che utilizzano [!DNL OneDrive], oltre a collegarlo a più applicazioni e servizi di terze parti.

Per istruzioni sulla creazione di uno scenario, consulta [Creare uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Per informazioni sui moduli, consulta [Moduli in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <p>Fabbisogno di licenza corrente: No [!DNL Workfront Fusion] requisito di licenza.</p>
   <p>Oppure</p>
   <p>Requisito licenza legacy: [!UICONTROL [!DNL Workfront Fusion] per l'automazione e l'integrazione del lavoro] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>
   <p>Fabbisogno prodotto corrente: se si dispone di [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront] Pianifica, la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare la funzionalità descritta in questo articolo. [!DNL Workfront Fusion] è incluso in [!UICONTROL Ultimate] [!DNL Workfront] piano.</p>
   <p>Oppure</p>
   <p>Requisiti del prodotto legacy: la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare la funzionalità descritta in questo articolo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, consulta [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Prerequisiti

Da utilizzare [!DNL OneDrive] moduli, è necessario disporre di un [!DNL Microsoft OneDrive] account.

## Collegamento di [!DNL OneDrive] servizio a [!DNL Workfront Fusion]

Per istruzioni sulla connessione [!DNL OneDrive] account a [!UICONTROL Workfront Fusion], vedi [Creare una connessione a [!UICONTROL Adobe Workfront Fusion] - Istruzioni di base](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!DNL Microsoft OneDrive] moduli e relativi campi

Quando si configura [!DNL OneDrive] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL OneDrive] I campi potrebbero essere visualizzati in base a fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se viene visualizzato il pulsante Mappa sopra un campo o una funzione, è possibile utilizzarlo per impostare variabili e funzioni per tale campo. Per ulteriori informazioni, consulta [Mappare le informazioni da un modulo all’altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [File/Cartella](#filefolder)
* [Altro](#other)

### File/Cartella

* [[!UICONTROL File/cartelle di controllo]](#watch-filesfolders)
* [[!UICONTROL Cerca file/cartelle]](#search-filesfolders)
* [[!UICONTROL Ottieni un file]](#get-a-file)
* [[!UICONTROL Scaricare un file]](#download-a-file)
* [[!UICONTROL Carica un file]](#upload-a-file)
* [[!UICONTROL Creare una cartella]](#create-a-folder)
* [[!UICONTROL Ottieni un collegamento di condivisione]](#get-a-share-link)
* [[!UICONTROL Spostare un file o una cartella]](#move-a-filefolder)
* [[!UICONTROL Copiare un file]](#copy-a-file)
* [[!UICONTROL Eliminare un file o una cartella]](#delete-a-filefolder)

#### [!UICONTROL File/cartelle di controllo]

Questo modulo di attivazione avvia uno scenario quando viene creato o aggiornato un file o una cartella.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Per istruzioni sulla connessione [!DNL OneDrive] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Guarda file/cartelle]</td> 
   <td> <p>Selezionare la modalità di visualizzazione di file o cartelle:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Per Ora Di Creazione]</b> </p> <p>Cerca nuovi file o cartelle.</p> </li> 
     <li> <p><b>[!UICONTROL Per Ora Di Aggiornamento]</b> </p> <p>Controlla i file o le cartelle esistenti aggiornati.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scegli il tuo [!DNL OneDrive] posizione]</td> 
   <td> <p>Seleziona la posizione da controllare:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Unità]</b> </p> <p>Selezionare se abilitare il modulo per immettere un ID unità.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sì]</b> </p> <p>Immettere l'ID dell'unità che si desidera controllare nel modulo.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> <p>Passare alla cartella che si desidera controllare nel modulo. Puoi anche inserire una query per filtrare i risultati restituiti.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL condiviso con me]</b> </p> <p>Il modulo controlla i file condivisi con il proprietario dell'unità.</p> </li> 
     <li> <p><b>[!UICONTROL Unità del sito]</b> </p> <p>Seleziona il sito SharePoint che desideri che il modulo controlli. I Siti disponibili sono Siti seguiti dall'utente connesso.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Selezionare il gruppo di cui si desidera controllare l'unità del modulo.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scegli un tipo di elemento]</td> 
   <td> <p>Seleziona se desideri guardare file, cartelle o entrambi.</p> <p>Nota: non è possibile controllare le cartelle in un'unità [!UICONTROL Shared With Me].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Immettere o mappare il numero massimo di record che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</p> </td> 
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
   <td>Per istruzioni sulla connessione [!DNL OneDrive] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scegli il tuo [!DNL OneDrive] posizione]</td> 
   <td> <p>Selezionare il percorso in cui si desidera eseguire la ricerca:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Unità]</b> </p> <p>Selezionare se abilitare il modulo per immettere un ID unità.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sì]</b> </p> <p>Immettere l'ID dell'unità in cui si desidera eseguire la ricerca nel modulo.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> <p>Passa alla cartella in cui desideri eseguire la ricerca nel modulo. Puoi anche inserire una query per filtrare i risultati restituiti.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL condiviso con me]</b> </p> <p>Il modulo cerca i file che sono stati condivisi con il proprietario dell'unità.</p> </li> 
     <li> <p><b>[!UICONTROL Unità del sito]</b> </p> <p>Seleziona la [!DNL SharePoint] Sito in cui si desidera eseguire la ricerca nel modulo. I Siti disponibili sono Siti seguiti dall'utente connesso.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Selezionare il gruppo di cui si desidera cercare l'unità del modulo.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scegli un tipo di elemento]</td> 
   <td> <p>Seleziona se desideri cercare file, cartelle o entrambi.</p> <p>Nota: non è possibile cercare cartelle in un'unità [!UICONTROL Shared With Me].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Immettere o mappare il numero massimo di record che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</p> </td> 
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
   <td>Per istruzioni sulla connessione [!DNL OneDrive] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Invio (ID file e percorso file)]</td> 
   <td>Specificare se si desidera identificare il file in base all'ID file o al percorso file.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Immettere un ID file] / [!UICONTROL Percorso file]</td> 
   <td> <p>Selezionare la modalità di immissione dell'ID o del percorso del file:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Immetti Manualmente]</b> </p> <p>Seleziona questa opzione se desideri immettere direttamente l’ID o il percorso oppure mapparlo da un modulo precedente.</p> </li> 
     <li> <p><b>[!UICONTROL Seleziona da elenco]</b> </p> <p>Selezionare questa opzione se si desidera effettuare una selezione da un elenco di file o percorsi disponibili. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scegli il tuo [!DNL OneDrive] posizione]</td> 
   <td> <p>Selezionare il percorso in cui si desidera eseguire la ricerca:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Unità]</b> </p> <p>Selezionare se abilitare il modulo per immettere un ID unità.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sì]</b> </p> <p>Immettere l'ID dell'unità che contiene il file che si desidera ottenere.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Unità del sito]</b> </p> <p>Selezionare il sito SharePoint contenente il file che si desidera ottenere. I Siti disponibili sono Siti seguiti dall'utente connesso.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Selezionare il gruppo la cui unità contiene il file che si desidera ottenere.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID unità]</td> 
   <td> <p>Selezionare o mappare l'unità contenente il file che si desidera ottenere. Questo campo non è disponibile se è stato selezionato [!UICONTROL No] nel campo [!UICONTROL Attiva per immettere un ID unità].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File] / [!UICONTROL File ID] / [!UICONTROL File Path]</td> 
   <td> <p>Se è stato selezionato [!UICONTROL Invio manuale], immettere o mappare l'ID file o il percorso del file che si desidera ottenere.</p> <p>Se è stato selezionato [!UICONTROL Seleziona dall'elenco], selezionare il file che si desidera ottenere.</p> </td> 
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
   <td>Per istruzioni sulla connessione [!DNL OneDrive] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Invio (ID file e percorso file)]</td> 
   <td>Specificare se si desidera identificare il file in base all'ID file o al percorso file.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Immetti un ID file/percorso file</td> 
   <td> <p>Selezionare la modalità di immissione dell'ID o del percorso del file:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Immetti Manualmente]</b> </p> <p>Seleziona questa opzione se desideri immettere direttamente l’ID o il percorso oppure mapparlo da un modulo precedente.</p> </li> 
     <li> <p><b>[!UICONTROL Seleziona da elenco]</b> </p> <p>Selezionare questa opzione se si desidera effettuare una selezione da un elenco di file o percorsi disponibili. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scegli il tuo [!DNL OneDrive] posizione]</td> 
   <td> <p>Selezionare il percorso che contiene il file da scaricare:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Unità]</b> </p> <p>Selezionare se abilitare il modulo per immettere un ID unità.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sì]</b> </p> <p>Immettere l'ID dell'unità che contiene il file da scaricare.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Unità del sito]</b> </p> <p>Selezionare il sito SharePoint contenente il file che si desidera scaricare. I Siti disponibili sono Siti seguiti dall'utente connesso.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Selezionare il gruppo la cui unità contiene il file da scaricare.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID unità]</td> 
   <td> <p>Selezionare o mappare l'unità contenente il file da scaricare. Questo campo non è disponibile se è stato selezionato [!UICONTROL No] nel campo [!UICONTROL Attiva per immettere un ID unità].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File] / [!UICONTROL File ID] / [!UICONTROL File Path]</td>
   <td> <p>Se è stato selezionato [!UICONTROL Invio manuale], immettere o mappare l'ID file o il percorso del file che si desidera scaricare.</p> <p>Se è stato selezionato [!UICONTROL Seleziona dall'elenco], selezionare il file che si desidera scaricare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Converti in PDF]</td> 
   <td> <p>Abilita questa opzione per convertire il file in un file PDF. È possibile eseguire la conversione dai seguenti tipi di file:</p> 
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
         <li> <p> <p>PENTOLA</p> </p> </li> 
         <li> <p> <p>POM</p> </p> </li> 
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

#### [!UICONTROL Carica un file]

Questo modulo di azione carica un file nella cartella specificata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Per istruzioni sulla connessione [!DNL OneDrive] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Invio (ID e percorso cartella)</td> 
   <td>Seleziona se desideri identificare la cartella di destinazione per ID o per percorso.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scegli il tuo [!DNL OneDrive] posizione]</td> 
   <td> <p>Selezionare il percorso in cui si desidera caricare un file:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Unità]</b> </p> <p>Selezionare se abilitare il modulo per immettere un ID unità.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sì]</b> </p> <p>Selezionare l'unità contenente il file che si desidera ottenere.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Unità del sito]</b> </p> <p>Seleziona la [!DNL SharePoint] Sito contenente la cartella in cui si desidera caricare un file. I Siti disponibili sono Siti seguiti dall'utente connesso.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Selezionare il gruppo la cui unità contiene la cartella in cui si desidera caricare un file.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID unità]</td> 
   <td> <p>Selezionare l'unità contenente la cartella in cui si desidera caricare un file. Questo campo non è disponibile se è stato selezionato [!UICONTROL No] nel campo [!UICONTROL Attiva per immettere un ID unità].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File di origine]</td> 
   <td> <p>Selezionare un file di origine da un modulo precedente o mappare il nome e i dati del file di origine.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Se il file con lo stesso nome esiste]</td> 
   <td>Selezionare come procedere se esiste già un file con lo stesso nome.</td> 
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
   <td>Per istruzioni sulla connessione [!DNL OneDrive] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scegli il tuo [!DNL OneDrive] posizione]</td> 
   <td> <p>Selezionare il percorso in cui si desidera creare una cartella:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Unità]</b> </p> <p>Selezionare se abilitare il modulo per immettere un ID unità.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sì]</b> </p> <p>Selezionare l'unità in cui si desidera creare una cartella.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Unità del sito]</b> </p> <p>Seleziona la [!DNL SharePoint] Sito in cui si desidera creare una cartella. I Siti disponibili sono Siti seguiti dall'utente connesso.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Selezionare il gruppo proprietario dell'unità in cui si desidera creare una cartella.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID unità]</td> 
   <td> <p>Selezionare l'unità in cui si desidera creare una cartella. Questo campo non è disponibile se è stato selezionato [!UICONTROL No] nel campo [!UICONTROL Attiva per immettere un ID unità].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td>Se si desidera che la nuova cartella sia una sottocartella, passare alla cartella in cui si desidera che sia una sottocartella.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome nuova cartella]</td> 
   <td> <p>Immettere o mappare un nome per la nuova cartella.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL se esiste una cartella con lo stesso nome]</td> 
   <td>Selezionare come procedere se esiste già un file con lo stesso nome.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottieni un collegamento di condivisione]

Questo modulo di azione restituisce un collegamento di condivisione per il file specificato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Per istruzioni sulla connessione [!DNL OneDrive] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Invio (ID file e percorso file)]</td> 
   <td>Specificare se si desidera identificare il file in base all'ID file o al percorso file.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Immettere un ID file] / [!UICONTROL Percorso file]</td> 
   <td> <p>Selezionare la modalità di immissione dell'ID o del percorso del file:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Immetti Manualmente]</b> </p> <p>Seleziona questa opzione se desideri immettere direttamente l’ID o il percorso oppure mapparlo da un modulo precedente.</p> </li> 
     <li> <p><b>[!UICONTROL Seleziona da elenco]</b> </p> <p>Selezionare questa opzione se si desidera effettuare una selezione da un elenco di file o percorsi disponibili. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scegli il tuo [!DNL OneDrive] posizione]</td> 
   <td> <p>Selezionare il percorso per il quale si desidera recuperare un collegamento di condivisione:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Unità]</b> </p> <p>Selezionare se abilitare il modulo per immettere un ID unità.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sì]</b> </p> <p>Immettere l'ID dell'unità contenente il file per il quale si desidera recuperare un collegamento di condivisione.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Unità del sito]</b> </p> <p>Selezionare il sito SharePoint contenente il file per il quale si desidera recuperare un collegamento di condivisione. I Siti disponibili sono Siti seguiti dall'utente connesso.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Selezionare il gruppo la cui unità contiene il file per il quale si desidera recuperare un collegamento di condivisione.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID unità]</td> 
   <td> <p>Selezionare o mappare l'unità contenente il file per il quale si desidera recuperare un collegamento di condivisione. Questo campo non è disponibile se è stato selezionato [!UICONTROL No] nel campo [!UICONTROL Attiva per immettere un ID unità].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File] / [!UICONTROL File ID] / [!UICONTROL File Path]</td> 
   <td> <p>Se è stato selezionato [!UICONTROL Invio manuale], immettere o mappare l'ID file o il percorso del file per il quale si desidera recuperare un collegamento di condivisione.</p> <p>Se si seleziona [!UICONTROL Select] dall'elenco, selezionare il file per il quale si desidera recuperare un collegamento di condivisione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di autorizzazione]</td> 
   <td> <p>Specificare se si desidera che gli utenti con il collegamento siano in grado di leggere e scrivere nel file o di sola lettura.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ambito]</td> 
   <td>Specificare se si desidera rendere disponibile il file a chiunque disponga del collegamento oppure solo ai membri dell'organizzazione che dispongono del collegamento.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Spostare un file o una cartella]

Questo modulo di azione sposta un file o una cartella in una nuova posizione

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Per istruzioni sulla connessione [!DNL OneDrive] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Invio (ID file e percorso file)]</td> 
   <td>Specificare se si desidera identificare il file in base all'ID file o al percorso file.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inserisci un ID file/percorso file]</td> 
   <td> <p>Selezionare la modalità di immissione dell'ID o del percorso del file:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Immetti Manualmente]</b> </p> <p>Seleziona questa opzione se desideri immettere direttamente l’ID o il percorso oppure mapparlo da un modulo precedente.</p> </li> 
     <li> <p><b>[!UICONTROL Seleziona da elenco]</b> </p> <p>Selezionare questa opzione se si desidera effettuare una selezione da un elenco di file o percorsi disponibili. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scegli il tuo [!DNL OneDrive] posizione]</td> 
   <td> <p>Selezionare il percorso contenente il file o la cartella che si desidera spostare:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Unità]</b> </p> <p>Selezionare se abilitare il modulo per immettere un ID unità.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sì]</b> </p> <p>Immettere l'ID dell'unità che contiene il file o la cartella che si desidera spostare.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Unità del sito]</b> </p> <p>Seleziona la [!DNL SharePoint] Sito contenente il file o la cartella che si desidera spostare. I Siti disponibili sono Siti seguiti dall'utente connesso.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Selezionare il gruppo la cui unità contiene il file o la cartella che si desidera spostare.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID unità]</td> 
   <td> <p>Selezionare o mappare l'unità contenente il file o la cartella che si desidera spostare. Questo campo non è disponibile se è stato selezionato [!UICONTROL No] nel campo [!UICONTROL Attiva per immettere un ID unità].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Seleziona [!UICONTROL File/Cartella]</td> 
   <td>Seleziona se desideri spostare un file o una cartella.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!UICONTROL File] / [!UICONTROL File ID] / [!UICONTROL File Path]</p> <p role="rowheader">[!UICONTROL Folder] / [!UICONTROL Folder ID] / [!UICONTROL Folder Path]</p> </td> 
   <td> <p>Se è stato selezionato [!UICONTROL Invio manuale], immettere o mappare l'ID o il percorso del file o della cartella che si desidera spostare.</p> <p>Se si seleziona [!UICONTROL Select] dall'elenco, selezionare il file o la cartella che si desidera spostare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inserisci un nuovo percorso cartella]</td> 
   <td> <p>Selezionare la modalità di immissione del percorso in cui si desidera spostare il file o la cartella:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Immetti Manualmente]</b> </p> <p>Seleziona questa opzione se desideri immettere direttamente l’ID o il percorso oppure mapparlo da un modulo precedente.</p> </li> 
     <li> <p><b>[!UICONTROL Seleziona da elenco]</b> </p> <p>Selezionare questa opzione se si desidera effettuare una selezione da un elenco di file o percorsi disponibili. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scegli il tuo [!DNL OneDrive] posizione]</td> 
   <td> <p>Selezionare il percorso in cui si desidera spostare il file o la cartella:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Unità]</b> </p> <p>Selezionare se abilitare il modulo per immettere un ID unità.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sì]</b> </p> <p>Immettere l'ID dell'unità in cui spostare il file o la cartella.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Unità del sito]</b> </p> <p>Seleziona la [!DNL SharePoint] Sito in cui spostare il file o la cartella. I Siti disponibili sono Siti seguiti dall'utente connesso.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Selezionare il gruppo di cui si desidera spostare il file o la cartella.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID unità]</td> 
   <td> <p>Selezionare o mappare l'unità contenente la cartella in cui si desidera spostare il file o la cartella. Questo campo non è disponibile se è stato selezionato [!UICONTROL No] nel campo [!UICONTROL Attiva per immettere un ID unità].</p> <p>Se si lascia vuoto questo campo, il file o la cartella può essere spostato solo all'interno dello stesso [!DNL OneDrive].</p> <p>È possibile spostare file e cartelle da [!UICONTROL Unità personale] a un'unità del sito [!UICONTROL Unità] o a un'unità del gruppo [!UICONTROL]. </p> <p>È possibile spostare i file da un'unità di un sito [!UICONTROL] solo nella stessa unità nello stesso sito.</p> <p>È possibile spostare i file dall'unità di un gruppo [!UICONTROL] solo alla stessa unità nello stesso gruppo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td>Immettere o mappare la cartella in cui spostare il file o la cartella.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Copiare un file]

Questo modulo di azione copia un file in un nuovo percorso di cartella

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Per istruzioni sulla connessione [!DNL OneDrive] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Invio (ID file e percorso file)]</td> 
   <td>Specificare se si desidera identificare il file in base all'ID file o al percorso file.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Immettere un ID file] / [!UICONTROL Percorso file]</td> 
   <td> <p>Selezionare la modalità di immissione dell'ID o del percorso del file:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Immetti Manualmente]</b> </p> <p>Seleziona questa opzione se desideri immettere direttamente l’ID o il percorso oppure mapparlo da un modulo precedente.</p> </li> 
     <li> <p><b>[!UICONTROL Seleziona da elenco]</b> </p> <p>Selezionare questa opzione se si desidera effettuare una selezione da un elenco di file o percorsi disponibili. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scegli il tuo [!DNL OneDrive] posizione]</td> 
   <td> <p>Selezionare il percorso contenente il file da copiare:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Unità]</b> </p> <p>Selezionare se abilitare il modulo per immettere un ID unità.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sì]</b> </p> <p>Immettere l'ID dell'unità che contiene il file o la cartella da copiare.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Unità del sito]</b> </p> <p>Selezionare il sito SharePoint contenente il file che si desidera spostare. I Siti disponibili sono Siti seguiti dall'utente connesso.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Selezionare il gruppo la cui unità contiene il file da copiare.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID unità]</td> 
   <td> <p>Selezionare o mappare l'unità contenente il file da copiare. Questo campo non è disponibile se è stato selezionato [!UICONTROL No] nel campo [!UICONTROL Attiva per immettere un ID unità].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!UICONTROL File] / [!UICONTROL File ID] / [!UICONTROL File Path]</p> </td> 
   <td> <p>Se è stato selezionato [!UICONTROL Invio manuale], immettere o mappare l'ID o il percorso del file da copiare.</p> <p>Se è stato selezionato [!UICONTROL Select] dall'elenco, selezionare il file che si desidera copiare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inserisci un nuovo percorso cartella]</td> 
   <td> <p>Selezionare la modalità di immissione del percorso in cui si desidera copiare il file o:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Immetti Manualmente]</b> </p> <p>Seleziona questa opzione se desideri immettere direttamente l’ID o il percorso oppure mapparlo da un modulo precedente.</p> </li> 
     <li> <p><b>[!UICONTROL Seleziona da elenco]</b> </p> <p>Seleziona questa opzione se desideri effettuare una selezione da un elenco di cartelle disponibili. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nuovo percorso OneDrive]</td> 
   <td> <p>Selezionare il percorso in cui si desidera copiare il filtro. Questa opzione è disponibile se si è scelto di selezionare il nuovo percorso di cartella da un elenco.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Unità]</b> </p> <p>Selezionare se abilitare il modulo per immettere un ID unità.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sì]</b> </p> <p>Immettere l'ID dell'unità in cui copiare il file.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Unità del sito]</b> </p> <p>Seleziona la [!DNL SharePoint] Sito in cui copiare il file. I Siti disponibili sono Siti seguiti dall'utente connesso.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Selezionare il gruppo di cui si desidera copiare il file.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID unità]</td> 
   <td> <p>Selezionare o mappare l'unità contenente la cartella in cui si desidera copiare il file. Questo campo non è disponibile se è stato selezionato [!UICONTROL No] nel campo [!UICONTROL Attiva per immettere un ID unità].</p> <p>Se si lascia vuoto questo campo, il file o la cartella può essere copiato solo nello stesso [!UICONTROL OneDrive].</p> <p>È possibile copiare file e cartelle da [!UICONTROL Unità personale] in un'unità del sito [!UICONTROL Unità del sito] o in un'unità del gruppo [!UICONTROL]. </p> <p>È possibile copiare i file da un'unità del sito [!UICONTROL] solo nella stessa unità nello stesso sito.</p> <p>È possibile copiare i file da un'unità del gruppo [!UICONTROL] solo nella stessa unità dello stesso gruppo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td>Immettere o mappare la cartella in cui si desidera spostare la copia o la cartella.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome nuovo file copiato]</td> 
   <td> <p>Immettere o mappare un nome per la nuova copia del file. È possibile lasciare vuoto questo campo se non si desidera modificare il nome del file originale.</p> <p>Il nome deve includere l’estensione del file. Esempio:<code> file.txt</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminare un file o una cartella]

Questo modulo di azione elimina il file selezionato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Per istruzioni sulla connessione [!DNL OneDrive] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Invio (ID file/cartella e percorso)]</td> 
   <td>Specificare se si desidera identificare il file in base all'ID file o al percorso file.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Immettere un ID file/cartella /Immettere un percorso file/cartella]</td> 
   <td> <p>Selezionare la modalità di immissione dell'ID o del percorso del file:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Immetti Manualmente]</b> </p> <p>Seleziona questa opzione se desideri immettere direttamente l’ID o il percorso oppure mapparlo da un modulo precedente.</p> </li> 
     <li> <p><b>[!UICONTROL Seleziona da elenco]</b> </p> <p>Selezionare questa opzione se si desidera effettuare una selezione da un elenco di file o percorsi disponibili. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scegli il tuo [!DNL OneDrive] posizione]</td> 
   <td> <p>Selezionare il percorso in cui si desidera eseguire la ricerca:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Unità]</b> </p> <p>Selezionare se abilitare il modulo per immettere un ID unità.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sì]</b> </p> <p>Immettere l'ID dell'unità che contiene il file o la cartella che si desidera eliminare.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Unità del sito]</b> </p> <p>Seleziona la [!DNL SharePoint] Sito contenente il file o la cartella da eliminare. I Siti disponibili sono Siti seguiti dall'utente connesso.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Selezionare il gruppo la cui unità contiene il file o la cartella che si desidera eliminare.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID unità]</td> 
   <td> <p>Selezionare o mappare l'unità contenente il file o la cartella che si desidera eliminare. Questo campo non è disponibile se è stato selezionato [!UICONTROL No] nel campo [!UICONTROL Attiva per immettere un ID unità].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Seleziona [!UICONTROL File/Cartella]</td> 
   <td>Seleziona se desideri eliminare un file o una cartella.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File] / [!UICONTROL File ID] / [!UICONTROL File Path]</td>
   <td> <p>Se è stato selezionato [!UICONTROL Invio manuale], immettere o mappare l'ID file o il percorso del file che si desidera eliminare.</p> <p>Se è stato selezionato [!UICONTROL Select] dall'elenco, selezionare il file che si desidera eliminare.</p> </td> 
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
   <td>Per istruzioni sulla connessione [!DNL OneDrive] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Inserisci un percorso relativo a <code>https://graph.microsoft.com</code>. Esempio:<code> /v1.0/me/drive/root/children</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   td&gt; <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Aggiungi le intestazioni della richiesta sotto forma di oggetto JSON standard.</p> <p>Ad esempio: <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion aggiunge automaticamente le intestazioni di autorizzazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Stringa Di Query]</td> 
   <td> <p>Aggiungi la query per la chiamata API sotto forma di oggetto JSON standard.</p> <p>Ad esempio: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Aggiungi il contenuto body per la chiamata API sotto forma di oggetto JSON standard.</p> <p>Nota:  <p>Quando si utilizzano istruzioni condizionali quali <code>if</code> nel JSON, inserisci le virgolette al di fuori dell’istruzione condizionale.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>



## Se non riesci a caricare o aggiornare un file

Quando si carica o si aggiorna un file con esito negativo, si possono verificare diversi problemi:

* Il file caricato è troppo grande e supera la dimensione massima consentita per il file [!DNL OneDrive] o ha utilizzato tutte le sue risorse [!DNL OneDrive] quota di archiviazione dell&#39;account. Per ottenere più spazio di archiviazione, elimina i file esistenti da [!DNL OneDrive] o aggiornare [!DNL OneDrive] account.
* OneDrive non consente di caricare due file con lo stesso nome in una singola cartella. Se la cartella di destinazione contiene un file con lo stesso nome del file che viene caricato, l’esecuzione dello scenario termina con un errore. La soluzione consiste semplicemente nel rinominare il file caricato. Se il tuo obiettivo è quello di aggiornare un file, utilizza [!UICONTROL Aggiornare un file] azione.
* La cartella selezionata in precedenza, in cui viene caricato il file, non esiste più. Lo scenario si interrompe e dovrai selezionare di nuovo la cartella di destinazione.
