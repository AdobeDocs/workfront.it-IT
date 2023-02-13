---
title: Moduli CloudConvert
description: Moduli CloudConvert
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: e21ef8a0-bec0-43fc-a495-c00b4023a273
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2993'
ht-degree: 0%

---

# [!DNL CloudConvert] moduli

In uno scenario Adobe Workfront Fusion, è possibile automatizzare i flussi di lavoro che utilizzano CloudConvert e collegarli a più applicazioni e servizi di terze parti. La [!DNL CloudConvert] I moduli consentono di monitorare e gestire processi, attività e importare ed esportare file nei [!DNL CloudConvert] conto.

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

## Connetti [!DNL CloudConvert] a [!DNL Workfront Fusion] {#connect-cloudconvert-to-workfront-fusion}

Per collegare il [!DNL CloudConvert] account a [!DNL Workfront Fusion], devi ottenere la chiave API dalla [!DNL CloudConvert] conto.

1. Accedi al tuo [!DNL CloudConvert] e aprire il tuo account [!UICONTROL Dashboard].
1. Apri **[!UICONTROL Autorizzazione] > [!UICONTROL Chiavi API]** sezione .
1. Fai clic su **[!UICONTROL Creare una nuova chiave API]**.
1. Immetti il nome della chiave API, abilita gli ambiti che desideri utilizzare, quindi fai clic su **[!UICONTROL Crea]**.
1. Copia il token fornito e archivialo in un luogo sicuro.
1. In [!DNL Workfront Fusion], inizia a creare uno scenario e apri la [!DNL CloudConvert] del modulo **[!UICONTROL Creare una connessione]** finestra di dialogo.

   Per istruzioni, consulta [Crea uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. Inserisci il token salvato nel passaggio 5, quindi fai clic su **[!UICONTROL Continua]** stabilire il collegamento.

## [!DNL CloudConvert] moduli e relativi campi {#cloudconvert-modules-and-their-fields}

Quando si configura [!DNL CloudConvert] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL CloudConvert] potrebbero essere visualizzati, a seconda di fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se trovi il pulsante mappa sopra un campo o una funzione, puoi utilizzarlo per impostare variabili e funzioni per quel campo. Per ulteriori informazioni, consulta [Mappare informazioni da un modulo a un altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Attività comuni](#common-tasks)
* [Lavori](#jobs)
* [Attività](#tasks)
* [Altro](#other)

### Attività comuni

* [Acquisire un sito web](#capture-a-website)
* [[!UICONTROL Convertire un file]](#convert-a-file)
* [Creare un archivio](#create-an-archive)
* [Unisci file](#merge-files)
* [Ottimizzare un file](#optimize-a-file)

#### [!UICONTROL Acquisire un sito web]

Questo modulo di azione acquisisce un sito Web specifico e lo salva in formato PDF, JPG o PNG.

Puoi specificare l’URL del sito web e altre informazioni, ad esempio dove memorizzare le informazioni.

Il modulo restituisce l’ID del file e di tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL CloudConvert] account a [!DNL Workfront Fusion], vedi <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connetti [!DNL CloudConvert] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Inserisci l’URL del sito web da acquisire. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output Format] </td> 
   <td>Seleziona se salvare il sito web acquisito in formato PNG, JPG o PDF. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File Name] </td> 
   <td>Immetti un nome file (inclusa l’estensione) per il file di output di destinazione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers] </td> 
   <td> <p>(Facoltativo) Definisci le intestazioni di richiesta. </p> <p>Questa funzione è utile, ad esempio, quando l’URL specificato richiede l’autorizzazione. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conversione e opzioni specifiche del motore] </p> </td> 
   <td>Specifica le opzioni di conversione e di motore. Per visualizzare le opzioni disponibili, consulta la sezione <a href="https://cloudconvert.com/api/v2/convert#convert-tasks">[!DNL CloudConvert] API</a> documentazione per <code>input_format</code> e <code>output_format</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scaricare un file] </td> 
   <td> <p>Abilita questa opzione se desideri includere anche i dati del file nell’output del modulo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Convertire un file]

Converte un file in un formato di output selezionato.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL CloudConvert] account a [!DNL Workfront Fusion], vedi <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connetti [!DNL CloudConvert] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File di input]</td> 
   <td>Seleziona se caricare un file utilizzando [!DNL Workfront Fusion] oppure fornisci l’URL da cui verrà caricato il file.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Caricare un file]</td> 
   <td> <p>Selezionare un file di origine da un modulo precedente o mappare il nome e i dati del file di origine.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importare un file dall’URL]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL URL]</strong> </p> <p>Immetti l’URL del file da convertire.</p> </li> 
     <li> <p><strong>[!UICONTROL Headers]</strong></p> <p>Definire le intestazioni di richiesta (facoltativo). Questa funzione è utile, ad esempio, quando l’URL specificato richiede l’autorizzazione.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Formato]</td> 
   <td>Selezionare se si desidera specificare il formato di input del file che si desidera convertire. Se non viene specificato, l'estensione del file di input viene utilizzata come formato di input.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Input Format]</td> 
   <td>Selezionare il formato corrente del file.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Output Format]</td> 
   <td>Selezionare il formato di file di destinazione in cui si desidera convertire il file.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL File Name]</td> 
   <td>Scegli un nome file (inclusa l’estensione) per il file di output di destinazione.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Conversione e opzioni specifiche del motore] </p> </td> 
   <td>Specifica le opzioni di conversione e di motore. Per visualizzare le opzioni disponibili, consulta la sezione <a href="https://cloudconvert.com/api/v2/convert#convert-tasks">[!DNL CloudConvert] API</a> documentazione per <code>input_format</code> e <code>output_format</code>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Scaricare un file] </td> 
   <td> <p>Abilita questa opzione se desideri includere anche i dati del file nell’output del modulo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Creare un archivio]

Consente di aggiungere uno o più file all&#39;archivio ZIP, RAR, 7Z, TAR, TAR.GZ o TAR.BZ2.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL CloudConvert] account a [!DNL Workfront Fusion], vedi <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connetti [!DNL CloudConvert] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL File di input]</p> </td> 
   <td> <p>Specifica i file da aggiungere all’archivio.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Caricare un file]</td> 
   <td> <p>Selezionare un file di origine da un modulo precedente o mappare il nome e i dati del file di origine.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Importare un file dall’URL]</p> </td> 
   <td> <p><strong>[!UICONTROL URL]</strong> </p> <p>Inserisci l’URL del file da archiviare.</p> <p><strong>[!UICONTROL Headers]</strong> </p> <p>Definire le intestazioni di richiesta (facoltativo). Questa funzione è utile, ad esempio, quando l’URL specificato richiede l’autorizzazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output Format]</td> 
   <td> <p> Selezionare il formato di destinazione del file archiviato.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File name]</td> 
   <td> <p> Immetti il nome file (inclusa l’estensione) per il file di output di destinazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conversione e opzioni specifiche del motore] </td> 
   <td> <p>Specifica le opzioni di conversione e di motore. Per visualizzare le opzioni disponibili, consulta la sezione <a href="https://cloudconvert.com/api/v2/convert#convert-tasks">[!DNL CloudConvert] API</a> documentazione per <code>input_format</code> e <code>output_format</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scaricare un file]</td> 
   <td> <p>Abilita questa opzione se desideri includere anche i dati del file nell’output del modulo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Unisci file]

Unisce almeno due file in un PDF. Se i file di input non sono PDF, vengono automaticamente convertiti in PDF.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL CloudConvert] account a [!DNL Workfront Fusion], vedi <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connetti [!DNL CloudConvert] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL File di input]</p> </td> 
   <td> <p>Specificare i file da unire.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Caricare un file]</td> 
   <td> <p>Selezionare un file di origine da un modulo precedente o mappare il nome e i dati del file di origine.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Importare un file dall’URL]</p> </td> 
   <td> <p><strong>[!UICONTROL URL]</strong> </p> <p>Inserisci l’URL del file da archiviare.</p> <p><strong>[!UICONTROL Headers]</strong> </p> <p>Definire le intestazioni di richiesta (facoltativo). Questa funzione è utile, ad esempio, quando l’URL specificato richiede l’autorizzazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output Format]</td> 
   <td> <p> Selezionare il formato di destinazione del file unito.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File name]</td> 
   <td> <p> Immetti il nome file (inclusa l’estensione) per il file di output di destinazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conversione e opzioni specifiche del motore] </td> 
   <td> <p>Specifica le opzioni di conversione e di motore. Per visualizzare le opzioni disponibili, consulta la sezione <a href="https://cloudconvert.com/api/v2/convert#convert-tasks">[!DNL CloudConvert] API</a> documentazione per <code>input_format</code> e <code>output_format</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scaricare un file]</td> 
   <td> <p>Abilita questa opzione se desideri includere anche i dati del file nell’output del modulo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottimizzare un file]

Questo modulo di azione ottimizza e comprime un file in formato PDF, PNG o JPG.

È possibile specificare il file e i parametri per ottimizzarlo e archiviarlo.

Il modulo restituisce l’ID del file e di tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL CloudConvert] account a [!DNL Workfront Fusion], vedi <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connetti [!DNL CloudConvert] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File di input]</td> 
   <td>Seleziona se desideri caricare un file utilizzando Workfront Fusion o specifica l'URL da cui verrà caricato il file.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Caricare un file]</p> </td> 
   <td> <p>Selezionare un file di origine da un modulo precedente o mappare il nome e i dati del file di origine.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importare un file dall’URL] </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL URL]</strong>: Immetti l’URL del file da convertire.</li> 
     <li><strong>[!UICONTROL Headers]</strong>: (Facoltativo) Definisci le intestazioni di richiesta. Questa funzione è utile, ad esempio, quando l’URL specificato richiede l’autorizzazione.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Optimization for] </td> 
   <td> <p>Seleziona il profilo di ottimizzazione per specifiche esigenze di destinazione.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Web]</strong>: Ottimizzazione per il web (impostazione predefinita)</p> 
      <ul> 
       <li>Rimuovere i dati ridondanti e non necessari per il Web</li> 
       <li>Immagini compresse in modo intelligente, con immagini di esempio e clip</li> 
       <li>Unisci e sottoinsiemi di font</li> 
       <li>Convertire colori in RGB</li> 
      </ul> </li> 
    </ul> 
    <ul> 
     <li> <p><strong>[!UICONTROL Stampa]</strong>: Ottimizzazione per la stampa</p> 
      <ul> 
       <li> <p>Rimuovere i dati ridondanti e non necessari per la stampa</p> </li> 
       <li> <p>Immagini compresse in modo intelligente, con immagini di esempio e clip</p> </li> 
       <li> <p>Unisci e sottoinsiemi di font</p> </li> 
       <li> <p>Converti colori in CMYK</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Archive]</strong>: Ottimizzazione a scopo di archiviazione</p> 
      <ul> 
       <li> <p>Rimuovere i dati ridondanti e superflui per l'archiviazione</p> </li> 
       <li> <p>Comprimere le immagini in modo intelligente</p> </li> 
       <li> <p>Unisci e sottoinsiemi di font</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Immagini digitalizzate]</strong>: Ottimizzazione delle immagini digitalizzate</p> 
      <ul> 
       <li> <p>Profilo ottimizzato per PDF costituiti principalmente da immagini raster</p> </li> 
       <li> <p>Comprimere le immagini senza ridurre significativamente la qualità visiva</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL riduzione massima delle dimensioni]</strong>: Ottimizzazione per ridurre al massimo le dimensioni</p> 
      <ul> 
       <li> <p>Utilizzare la compressione massima possibile</p> </li> 
       <li> <p>Riduce la qualità visiva</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Formato di ingresso] </td> 
   <td>Selezionare il formato del file di input da ottimizzare. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File name]</td> 
   <td> <p>Immetti un nome file (inclusa l’estensione) per il file di output di destinazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conversione e opzioni specifiche del motore]</td> 
   <td> <p>Specifica le opzioni di conversione e di motore. Per visualizzare le opzioni disponibili, consulta la sezione <a href="https://cloudconvert.com/api/v2/convert#convert-tasks">[!DNL CloudConvert] API</a> documentazione per <code>input_format</code> e <code>output_format</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scaricare un file]</td> 
   <td> <p>Abilita questa opzione se desideri includere anche i dati del file nell’output del modulo.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Lavori

* [[!UICONTROL Creare un processo (avanzato)]](#create-a-job-advanced)
* [[!UICONTROL Nuovo evento di lavoro]](#new-job-event)
* [[!UICONTROL Elenca processi]](#list-jobs)
* [[!UICONTROL Ottieni un lavoro]](#get-a-job)
* [[!UICONTROL Eliminare un processo]](#delete-a-job)

#### [!UICONTROL Creare un processo (avanzato)]

Questo modulo crea un processo. Un processo può essere una o più attività identificate nel [!UICONTROL Nome] e collegati tra loro utilizzando [!UICONTROL Ingresso] campo .

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL CloudConvert] account a [!DNL Workfront Fusion], vedi <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connetti [!DNL CloudConvert] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File di input]</td> 
   <td> <p>Seleziona se caricare un file utilizzando [!DNL Workfront Fusion]oppure fornisci l’URL da cui verrà caricato il file.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Caricare un file]</td> 
   <td> <p>Selezionare un file di origine da un modulo precedente o mappare il nome e i dati del file di origine.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Importare un file dall’URL]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL URL]</strong>: Immetti l’URL del file da elaborare.</li> 
     <li><strong>[!UICONTROL Headers]</strong>: (Facoltativo) Definisci le intestazioni di richiesta. Questa funzione è utile, ad esempio, quando l’URL specificato richiede l’autorizzazione.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Tasks]</p> </td> 
   <td> <p>Aggiungi le attività che verranno eseguite all'interno del processo.</p> <p>La descrizione dei campi delle operazioni si trova nella sezione corrispondente.</p> 
    <ul> 
     <li><a href="#convert-a-file" class="MCXref xref">[!UICONTROL Convertire un file]</a> </li> 
     <li><a href="#capture-a-website" class="MCXref xref">[!UICONTROL Acquisire un sito web]e</a> </li> 
     <li><a href="#optimize-a-file" class="MCXref xref">[!UICONTROL Ottimizzare un file]</a> </li> 
     <li><a href="#create-an-archive" class="MCXref xref">[!UICONTROL Creare un archivio]</a> </li> 
     <li><a href="#merge-files" class="MCXref xref">[!UICONTROL Unisci file]</a> </li> 
    </ul> 
    <ul> 
     <li> <p><strong>[!UICONTROL Eseguire un comando]</strong> </p> <p>Per ulteriori informazioni sull'esecuzione di un comando, vedi <a href="https://cloudconvert.com/api/v2/command#command-tasks">[!DNL CloudConvert] Documentazione API</a>.</p> </li> 
     <li> <p><strong>[!UICONTROL Esporta un file in URL temporaneo]</strong> </p> <p> Specifica il nome dell’attività e il nome dell’attività di input (ad esempio Conversione).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Tag [!UICONTROL] </td> 
   <td> <p>Immetti un tag. I tag sono stringhe arbitrarie per identificare il processo. Non hanno alcun effetto e possono essere utilizzati per associare il processo a un ID.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminare un processo]

Questo modulo elimina un processo, inclusi tutte le attività e i dati.

>[!NOTE]
>
>I processi vengono eliminati automaticamente 24 ore dopo la loro scadenza.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL CloudConvert] account a [!DNL Workfront Fusion], vedi <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connetti [!DNL CloudConvert] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID processo [!UICONTROL]</td> 
   <td> <p>Immettere o mappare l'ID del processo da eliminare.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottieni un lavoro]

Questo modulo recupera i dettagli del processo.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL CloudConvert] account a [!DNL Workfront Fusion], vedi <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connetti [!DNL CloudConvert] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID processo [!UICONTROL]</td> 
   <td> <p>Immettere o mappare l'ID del processo di cui si desidera recuperare i dettagli.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Elenca processi]

Questo modulo recupera tutti i processi eseguiti nel tuo account.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL CloudConvert] account a [!DNL Workfront Fusion], vedi <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connetti [!DNL CloudConvert] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Status] </td> 
   <td> <p>Selezionare lo stato del processo per filtrare i processi restituiti in base a.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Imposta il numero di processi che Workfront Fusion 2.0 restituirà durante un ciclo di esecuzione.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Nuovo evento di lavoro]

Viene attivato quando viene creato un processo nell&#39;account o nell&#39;attività, termina o non riesce.

>[!NOTE]
>
>* Il processo creato da [!UICONTROL Creare un processo (avanzato)] il modulo è costituito da *diversi* compiti.
>* La [!UICONTROL Nuovo evento di lavoro] viene inoltre attivato quando un *individuale* attività creata, completata o non riuscita.
>


<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhhook name]</td> 
   <td>Inserisci il nome del webhook. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL CloudConvert] account a [!DNL Workfront Fusion], vedi <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connetti [!DNL CloudConvert] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output Format] </td> 
   <td>Seleziona se salvare il sito web acquisito in formato PNG, JPG o PDF. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Event]</td> 
   <td>Seleziona se il modulo viene attivato quando il processo o l'attività viene creato, terminato o non riesce.</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>* Se si lavora con l&#39;Aggregator Array (ad esempio si devono convertire molti file in formati diversi), utilizzare la **[!UICONTROL Non conosco il formato di input]** in [!UICONTROL Aggiungi un’attività] finestra di dialogo. In caso contrario, viene restituito l’errore .
>* Collegamento di attività all’interno del processo (nome > input, nome > input,...):
>
>  ![](assets/linking-name-across-jobs-350x808.png)>

### Attività

* [[!UICONTROL Ottieni attività]](#get-a-task)
* [[!UICONTROL Scaricare un file]](#download-a-file)
* [[!UICONTROL Attività elenco]](#list-tasks)
* [[!UICONTROL Riprova un&#39;attività]](#retry-a-task)
* [[!UICONTROL Annullare un’attività]](#cancel-a-task)
* [[!UICONTROL Eliminare un’attività]](#delete-a-task)

#### [!UICONTROL Annullare un’attività]

Questo modulo annulla un&#39;attività con stato di attesa o elaborazione.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL CloudConvert] account a [!DNL Workfront Fusion], vedi <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connetti [!DNL CloudConvert] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID attività]</td> 
   <td> <p> Immettere o mappare l'ID dell'attività che si desidera annullare.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminare un’attività]

Elimina un’attività, inclusi tutti i dati.

>[!NOTE]
>
>Le attività vengono eliminate automaticamente 24 ore dopo la loro scadenza.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL CloudConvert] account a [!DNL Workfront Fusion], vedi <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connetti [!DNL CloudConvert] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID attività]</td> 
   <td> <p> Immettere (mappare) l'ID dell'attività che si desidera eliminare.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Scaricare un file]

Questo modulo recupera il nome del file e i dati del file dall&#39;attività specificata.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL CloudConvert] account a [!DNL Workfront Fusion], vedi <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connetti [!DNL CloudConvert] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID attività]</td> 
   <td> <p> Immettere o mappare l'ID dell'attività da cui si desidera scaricare il file.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottieni un’attività]

Questo modulo recupera i dettagli dell&#39;attività.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL CloudConvert] account a [!DNL Workfront Fusion], vedi <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connetti [!DNL CloudConvert] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID attività]</td> 
   <td> <p>Immettere o mappare l'ID dell'attività di cui si desidera recuperare i dettagli.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Attività elenco]

Questo modulo recupera tutte le attività nell&#39;account in base alle impostazioni del filtro.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL CloudConvert] account a [!DNL Workfront Fusion], vedi <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connetti [!DNL CloudConvert] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Status] </td> 
   <td> <p>Selezionare lo stato dell'attività per filtrare le attività restituite in base a.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID processo [!UICONTROL] </td> 
   <td> <p>Immettere o mappare l'ID processo per restituire solo le attività all'interno del processo specificato.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Operation] </td> 
   <td> <p>Immettere il tipo di operazione per restituire solo le attività con l'operazione specificata. </p> <p>Nota: Utilizza il modulo [!UICONTROL List Possibile Operations] per recuperare le operazioni.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Immettere o mappare il numero massimo di record che si desidera restituire dal modulo durante ogni ciclo di esecuzione degli scenari.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Riprova un&#39;attività]

Questo modulo crea una nuova attività, in base alle impostazioni (payload) di un’altra attività.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL CloudConvert] account a [!DNL Workfront Fusion], vedi <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connetti [!DNL CloudConvert] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID attività]</td> 
   <td> <p> Immettere o mappare l'ID dell'attività da cui si desidera creare una nuova attività.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Altro

* [[!UICONTROL Ottieni informazioni personali]](#get-my-info)
* [[!UICONTROL Effettuare una chiamata API]](#make-an-api-call)

#### [!UICONTROL Ottieni informazioni personali]

Recupera i dettagli dell&#39;account autenticato relativi all&#39;utente corrente.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL CloudConvert] account a [!DNL Workfront Fusion], vedi <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connetti [!DNL CloudConvert] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Effettuare una chiamata API]

Ti consente di eseguire una chiamata API personalizzata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare il tuo account [Fusion App] a Workfront Fusion, vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione ad Adobe Workfront Fusion - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> <p>Immettere un percorso relativo a <code>https://api.cloudconvert.com/</code>. Ad esempio: <code>/v2/tasks</code></p> <p>Per l’elenco degli endpoint disponibili, consulta <a href="https://cloudconvert.com/api/v2">[!DNL CloudConvert] Documentazione API v2</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL, Metodo]</td> 
   td&gt; <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Aggiungi le intestazioni della richiesta sotto forma di un oggetto JSON standard.</p> <p>Ad esempio: <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion 2.0 aggiunge le intestazioni di autorizzazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>Aggiungi la query per la chiamata API sotto forma di un oggetto JSON standard.</p> <p>Ad esempio: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Aggiungi il contenuto del corpo della chiamata API sotto forma di un oggetto JSON standard. Quando utilizzi istruzioni condizionali come <code>if</code> nel JSON, inserisci le virgolette al di fuori dell’istruzione condizionale.<img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"></p> </td> 
  </tr> 
 </tbody> 
</table>

**Esempio:** Attività elenco

La seguente chiamata API restituisce tutte le attività dal tuo account CloudFront:

URL: `/v2/tasks`

Metodo: `GET`

![](assets/cloudconvert-api-example-input.png)

Le corrispondenze della ricerca si trovano nell&#39;Output del modulo in [!UICONTROL Bundle] > [!UICONTROL Corpo] > [!UICONTROL dati].

Nel nostro esempio sono state restituite 6 attività:

![](assets/cloudconvert-api-example-output.png)

## Risoluzione dei problemi {#troubleshooting}

Vedi la tabella seguente per eventuali errori e relative soluzioni:

<table style="table-layout:auto">
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Errore</p> </th> 
   <th>Passaggi successivi</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p><span style="font-weight: normal;">[!UICONTROL La dimensione del file di output supera il limite consentito per lo scenario.]</span> </p> </td> 
   <td> <p>Fai riferimento ai limiti di dimensione del file.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><span style="font-weight: normal;">[!UICONTROL Hai superato il tempo massimo di conversione.]</span> </p> </td> 
   <td> <p>Il libero [!DNL CloudConvert] Il piano offre 25 minuti di conversione al giorno. Se il tuo utilizzo supera il limite del piano gratuito, puoi passare a un pacchetto o a un abbonamento (prepagato).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><span style="font-weight: normal;">[!UICONTROL Impossibile leggere le dimensioni del frame: Impossibile cercare fino al 1508. � /output/JLIADSA00137P0.mp3: Argomento non valido.]</span> </p> </td> 
   <td> <p>Questo errore viene generato, ad esempio durante la conversione di file da MP3 a WAV. Assicurati di aver selezionato la regione corretta perché troverà riferimenti a file ma non solo al file corretto.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL RuntimeError:] </p> <p><span style="font-weight: normal;">[!UICONTROL Numero massimo di ripetizioni superate.]</span> </p> </td> 
   <td> <p>Individua il corrispondente [!DNL CloudConvert] lavoro [!DNL CloudConvert] elenco dei processi del dashboard e verifica la sua durata:</p> <p> <img src="assets/cloudconvert-duration-350x177.png" style="width: 350;height: 177;"> </p> <p>La [!DNL CloudConvert] &gt; Il timeout del modulo [!UICONTROL Convert a File] è impostato su 3 minuti. Se la durata del lavoro supera i 3 minuti (probabilmente a causa di un sovraccarico temporaneo del [!DNL CloudConvert] service), il modulo genera l'errore di cui sopra.</p> <p>In questo caso, considera una delle seguenti opzioni:</p> 
    <ul> 
     <li>Abilita la <strong>[!UICONTROL Consenti archiviazione esecuzioni incomplete]</strong> nelle impostazioni dello scenario per memorizzare le esecuzioni incomplete per una risoluzione manuale successiva. Facoltativamente è possibile allegare una route di gestione degli errori al [!DNL CloudConvert] modulo con la direttiva [!UICONTROL Break] per risolvere automaticamente le esecuzioni incomplete.</li> 
     <li>Disattiva la <strong>Opzione [!UICONTROL Scarica un file]</strong> in [!DNL CloudConvert] &gt; Modulo [!UICONTROL Converti un file]. In questo caso il modulo non attenderà il risultato della conversione. Per ottenere il risultato della conversione, crea un nuovo scenario e utilizza il [!DNL CloudConvert] &gt; trigger [!UICONTROL New Job Event].</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Esempio di flusso di lavoro per [!DNL CloudConvert] connettore

>[!INFO]
>
>**Esempio:** Conversione di un video da MOV a formato MP4
>
>1. Visita [https://cloudconvert.com/video-converter](https://>cloudconvert.com/video-converter)
>1. Fai clic su **[!UICONTROL Seleziona file]** e scegli il tuo file MOV campione.
>1. Fai clic sul menu a discesa accanto a **[!UICONTROL Converti in]** e scegli **[!UICONTROL MP4]**.
>
>1. Fai clic sul pulsante **[!UICONTROL chiave]** icona.
>1. Configura le impostazioni di compressione MP4 come vedi.
>1. Fai clic su **[!UICONTROL Converti]**.
>1. Al termine della conversione, fai clic su **[!UICONTROL Scarica]**.
>1. Rivedi il video convertito.
>1. Ripetere i passaggi da 1 a 8 finché non sono state trovate le impostazioni di conversione ottimali per il passaggio 5.
>1. Visita [https://cloudconvert.com/api/v2/convert#convert-tasks](https://cloudconvert.com/api/v2/convert#convert-tasks)
>1. Scegli **[!UICONTROL mov]** per **[!UICONTROL input_format]** campo .
>
>1. Scegli **[!UICONTROL mp4]** per **[!UICONTROL output_format]** campo .
>
>1. Un elenco di tutti i parametri possibili come video_codec, crf, ecc. apparirà.
>1. In Workfront Fusion 2.0, inserire il **[!UICONTROL CloudConvert]** > **[!UICONTROL Convertire un file]** nel tuo scenario.
>
>1. Apri le impostazioni del modulo.
>1. Configura il modulo come mostrato di seguito:

>
>   ![](assets/cloudconvert-mp4-example.png)
>
>1. Assicurati di includere tutte le impostazioni nel campo Opzioni conversione e specifiche del motore: per ciascuna impostazione del passaggio 5, individua il parametro corrispondente del passaggio 13 e il relativo valore.

