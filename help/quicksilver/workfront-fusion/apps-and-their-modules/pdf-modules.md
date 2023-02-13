---
title: Servizi Adobe PDF
description: Servizi Adobe PDF
author: Becky
draft: Probably
feature: Workfront Fusion, Digital Content and Documents
exl-id: e0a5736b-dbdb-43c6-83ff-e88a5625a5bf
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '3213'
ht-degree: 0%

---

# [!DNL Adobe PDF Services]

Con la [!DNL Adobe Workfront Fusion] [!DNL Adobe PDF Services], è possibile estrarre dati da un file PDF o generare un nuovo file PDF dai dati forniti. Inoltre, è possibile convertire diversi tipi di file in PDF o PDF in altri tipi di file. PDF Services consente inoltre di combinare, comprimere o leggere i metadati di un file PDF, nonché di controllare la protezione tramite password sul file.

Se hai bisogno di istruzioni su come creare uno scenario, vedi [Crea uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Per informazioni sui moduli, consulta [Moduli in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

Per informazioni sull’API utilizzata per PDF Services, consulta [API di generazione dei documenti di Adobe](https://www.adobe.io/apis/documentcloud/dcsdk/doc-generation.html).

## Considerazioni sull’utilizzo [!DNL Adobe PDF Services]

* [Non è necessario un [!DNL Adobe] account](#you-do-not-need-an-adobe-account)
* [[!DNL Workfront Fusion] non memorizza i file](#workfront-fusion-does-not-store-your-files)

### Non è necessario un [!DNL Adobe] account

Perché [!DNL Workfront Fusion] fa parte del [!DNL Adobe] suite di prodotti, non è necessario un [!DNL Adobe] per utilizzare questi strumenti. Ogni strumento accede [!DNL Adobe] Funzionalità di PDF senza utilizzare una connessione.

Nonostante [!DNL Workfront Fusion] non richiede un [!DNL Adobe] per utilizzare PDF Services, i moduli richiedono una connessione. Non sono presenti credenziali in questa connessione e viene fornito solo un nome per la connessione stessa.

### [!DNL Workfront Fusion] non memorizza i file

La [!DNL Adobe PDF Services] può leggere, convertire o modificare i file, ma non [!DNL Adobe] né [!DNL Workfront Fusion] archiviare i file o i dati. Ciò significa che:

* Mantenere il controllo sui file, inclusa la loro sicurezza
* Non è necessario avere un [!UICONTROL Adobe] account di archiviazione o cloud per utilizzare PDF Services.

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

## [!DNL Adobe PDF Services] moduli e relativi campi

Quando si configura [!DNL PDF Services], [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Insieme a questi, potrebbero essere visualizzati campi aggiuntivi, a seconda di fattori come il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se trovi il pulsante mappa sopra un campo o una funzione, puoi utilizzarlo per impostare variabili e funzioni per quel campo. Per ulteriori informazioni, consulta [Mappare informazioni da un modulo a un altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [[!UICONTROL Genera documento]](#generate-document)
* [[!UICONTROL Estrai testo/tabella]](#extract-text--table)
* [[!UICONTROL Combinare file PDF]](#combine-pdf-files)
* [[!UICONTROL Comprimi file PDF]](#compress-pdf-files)
* [[!UICONTROL Converti documento in file PDF]](#convert-document-to-pdf-file)
* [[!UICONTROL Converti file HTML in file PDF]](#convert-html-to-pdf-file)
* [[!UICONTROL Converti immagine in file PDF]](#convert-image-to-pdf-file)
* [[!UICONTROL Converti PDF in documento]](#convert-pdf-to-document)
* [[!UICONTROL Converti PDF in immagine]](#convert-pdf-to-image)
* [[!UICONTROL Linearizzare un file PDF]](#linearize-a-pdf-file)
* [[!UICONTROL OCR per file PDF]](#ocr-for-pdf-file)
* [[!UICONTROL Manipolazione della pagina in PDF]](#pdf-page-manipulation)
* [[!UICONTROL Proprietà dei file PDF]](#pdf-file-properties)
* [[!UICONTROL File Protect PDF]](#protect-pdf-file)
* [[!UICONTROL Rimuovere la protezione di un file PDF]](#remove-protection-of-a-pdf-file)

### [!UICONTROL Genera documento]

La [!UICONTROL Genera documento] Il modulo è un modo potente per creare un PDF che contiene i dati selezionati. È possibile formattarlo utilizzando un [!DNL Microsoft Word] o fornendo dati in formato JSON.

Per ulteriori informazioni sulla [!UICONTROL [!DNL Adobe PDF Services] Genera documento] funzionalità, vedi [Panoramica sulla generazione dei documenti](https://www.adobe.io/apis/documentcloud/dcsdk/docs.html) in [!DNL Adobe Document Services] documentazione.

* [Utilizza la [!UICONTROL Genera documento] modulo con un [!DNL Microsoft Word] template](#use-the-generate-document-module-with-a-microsoft-word-template)
* [Utilizza la [!UICONTROL Genera documento] modulo con JSON](#use-the-generate-document-module-with-json)

#### Utilizza la [!UICONTROL Genera documento] modulo con un [!DNL Microsoft Word] template

<!--
>[!NOTE]
>
>For a discussion of Microsoft Word templates, see [Microsoft Word Template modules](../../workfront-fusion/apps-and-their-modules/microsoft-word-templates-modules.md). 
>
>You do not need to use Microsoft Word template modules to use a Microsoft Word template with the PDF Services Generate document module.
-->

Per utilizzare [!UICONTROL Genera documento] modulo con un [!UICONTROL Microsoft Word] modello, devi prima creare il modello. Per istruzioni, cerca &quot;Crea un modello&quot; nella sezione [!DNL Microsoft Office] documentazione.

Compila il [!UICONTROL Genera documento] campi modulo come segue:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Selezionare la connessione da utilizzare per questo modulo.</p> <p>Non è necessario un [!DNL Adobe] per creare una connessione PDF Services. Per ulteriori informazioni, consulta <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">Non è necessario un [!DNL Adobe] account</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File di origine]</td> 
   <td> <p>Selezionare un file di origine da un modulo precedente o mappare il nome e i dati del file di origine.</p> <p>Il file di origine è [!DNL Microsoft Word ]modello utilizzato dal modulo per generare il nuovo PDF.</p> <p>È consigliabile creare un progetto in [!DNL Workfront] per [!DNL Microsoft Word] modelli utilizzati in [!DNL Workfront Fusion]. È quindi possibile utilizzare la [!DNL Workfront] &gt; Modulo [!UICONTROL Download document] per richiamare il modello appropriato nello scenario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output Format]</td> 
   <td> <p>Selezionare il formato del documento generato.</p> 
    <ul> 
     <li> <p>PDF</p> </li> 
     <li> <p>DOCX</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Dati per l'unione]</td> 
   <td> <p>Per ogni tag valore nel modello da sostituire con testo, compila quanto segue:</p> 
    <ul> 
     <li> <p>[!UICONTROL Key]</p> <p>Immetti una chiave. Nel modello, la chiave è il testo mostrato nel tag valore. Ad esempio, se desideri inserire del testo nel tag valore <code>&#123;&#123;name&#125;&#125;</code>, inserisci <code>name </code>nel campo chiave .</p> </li> 
     <li> <p>Tipo di valore</p> <p>Selezionare se i dati nel campo valore sono un valore, un oggetto o una matrice di oggetti.</p> </li> 
     <li> <p>[!UICONTROL Value]</p> <p>Immettere o mappare il testo che si desidera visualizzare nel documento generato al posto del tag valore.</p> </li> 
    </ul> <p> <img src="assets/generate-with-template-350x241.png" style="width: 350;height: 241;"> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### Utilizza la [!UICONTROL Genera documento] modulo con JSON

Per utilizzare [!UICONTROL Genera documento] modulo con JSON, compila i campi come segue:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Selezionare la connessione da utilizzare per questo modulo.</p> <p>Non è necessario un [!DNL Adobe] per creare una connessione PDF Services. Per ulteriori informazioni, consulta <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">Non è necessario un [!DNL Adobe] account</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File di origine]</td> 
   <td> <p>Selezionare un file di origine da un modulo precedente o mappare il nome e i dati del file di origine.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output Format]</td> 
   <td> <p>Selezionare il formato del documento generato.</p> 
    <ul> 
     <li> <p>PDF</p> </li> 
     <li> <p>DOCX</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Dati per l'unione]</td> 
   <td> <p>Per utilizzare JSON in questo modulo, devi abilitare la mappatura su questo campo.</p> <p>Immetti o mappa il JSON da cui generare il documento. </p> <p>Puoi digitare JSON direttamente in questo campo o mappare l’output JSON da un modulo JSON.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Estrai testo/tabella]

Questo modulo di azione ti consente di estrarre dati da un file PDF. Il modulo genera singoli elementi di testo, ad esempio un paragrafo o il testo in una singola cella di una tabella.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Selezionare la connessione da utilizzare per questo modulo.</p> <p>Non è necessario un [!DNL Adobe] per creare una connessione PDF Services. Per ulteriori informazioni, consulta <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">Non è necessario un [!DNL Adobe] account</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File di origine]</td> 
   <td>Selezionare un file di origine da un modulo precedente o mappare il nome e i dati del file di origine.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elementi che devono essere estratti come JSON]</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Testo]</p> </li> 
     <li> <p>[!UICONTROL Tabelle]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Estrarre le caselle di collegamento?]</td> 
   <td>Abilita questa opzione per estrarre i dati relativi al riquadro di delimitazione del testo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Includi informazioni sullo stile per l'output?]</td> 
   <td>Abilita questa opzione per aggiungere informazioni sullo stile al JSON di output.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Combinare file PDF]

Questo modulo di azione prende più file PDF e li combina in un singolo file PDF. Ad esempio, questo modulo può combinare tutti i documenti in un [!UICONTROL Workfront] proiettare in un unico PDF al termine del progetto.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Selezionare la connessione da utilizzare per questo modulo.</p> <p>Non è necessario un [!DNL Adobe] per creare una connessione PDF Services. Per ulteriori informazioni, consulta <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">Non è necessario un [!DNL Adobe] account</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Documents]</td> 
   <td> <p>È possibile utilizzare un modulo di aggregazione per raccogliere i documenti da combinare in PDF oppure aggiungere i documenti manualmente. </p> <p>È consigliabile utilizzare un modulo [!UICONTROL Array Aggregator] per aggregare l’output da un modulo precedente. Utilizzando un aggregatore, non è necessario conoscere i nomi, le posizioni o i numeri di file da combinare. L’utilizzo di un aggregatore è quindi molto più flessibile e scalabile rispetto all’immissione manuale dei documenti da combinare.</p> <p>Per utilizzare il modulo di file [!UICONTROL Combina PDF] con un aggregatore, è necessario abilitare la mappatura nel campo Documenti. </p> <p>In questo esempio, il modulo [!UICONTROL Read Related Records] identifica i documenti associati a un progetto e il modulo [!UICONTROL Download Documents] li scarica. Tutti i PDF vengono aggregati in un array, che viene passato nel modulo file [!UICONTROL Combina PDF].</p> <p> <img src="assets/combine-example-350x104.png" style="width: 350;height: 104;"> </p> <p>È inoltre possibile immettere i documenti manualmente.</p> <p>Per ogni documento da includere nel PDF combinato:</p> 
    <ol> 
     <li value="1"> <p>Fai clic su [!UICONTROL Aggiungi un documento]</p> </li> 
     <li value="2"> <p>Nel campo [!UICONTROL Source file] selezionare il modulo che genera il documento da includere o mappare il nome e i dati del file di origine. </p> </li> 
     <li value="3"> <p>(Facoltativo) Se si desidera includere solo alcune pagine dal file di origine, per ogni intervallo di pagine che si desidera aggiungere fare clic su <strong>[!UICONTROL Aggiungi elemento]</strong> nel campo [!UICONTROL Pages], immetti la prima e l’ultima pagina dell’intervallo di pagine da includere e fai clic su <strong>[!UICONTROL Aggiungi]</strong>. È possibile includere più di un intervallo di pagine da un singolo documento.</p> </li> 
     <li value="4"> <p>Fai clic su <strong>[!UICONTROL Aggiungi]</strong>. </p> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Comprimi file PDF]

Questo modulo di azione prende un file PDF e lo comprime. Può essere utile per conservare la larghezza di banda o la memoria.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Selezionare la connessione da utilizzare per questo modulo.</p> <p>Non è necessario un [!DNL Adobe] per creare una connessione PDF Services. Per ulteriori informazioni, consulta <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">Non è necessario un [!DNL Adobe] account</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File di origine]</td> 
   <td> <p>Selezionare un file di origine da un modulo precedente o mappare il nome e i dati del file di origine.</p> <p>Il file di origine deve essere in formato PDF. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Livello di compressione]</td> 
   <td>Selezionare il livello di compressione che si desidera utilizzare.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Converti documento in file PDF]

Questo strumento converte un documento in un file PDF. Il file di origine deve essere in uno dei seguenti formati di documento:

* DOC
* XLS
* PPT
* TXT
* RTF

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Selezionare la connessione da utilizzare per questo modulo.</p> <p>Non è necessario un [!DNL Adobe] per creare una connessione PDF Services. Per ulteriori informazioni, consulta <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">Non è necessario un [!DNL Adobe] account</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File di origine]</td> 
   <td> <p>Selezionare un file di origine da un modulo precedente o mappare il nome e i dati del file di origine.</p> <p>Il file di origine deve essere in uno dei seguenti formati:</p> 
    <ul> 
     <li> <p>DOC</p> </li> 
     <li> <p>XLS</p> </li> 
     <li> <p>PPT</p> </li> 
     <li> <p>TXT</p> </li> 
     <li> <p>RTF</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Language]</td> 
   <td> <p>Selezionare la lingua predefinita per il documento di origine. Questo consente al modulo di selezionare un font appropriato, se non è incluso nel file di origine.</p> <p>Seleziona una delle seguenti lingue:</p> 
    <ul> 
     <li> <p>en-US (predefinito): Inglese (Stati Uniti d'America)</p> </li> 
     <li> <p>ca-ES: Catalano (Spagna)</p> </li> 
     <li> <p>cs-CZ: Ceco (Repubblica ceca)</p> </li> 
     <li> <p>da-DK: Danese (Danimarca)</p> </li> 
     <li> <p>de-DE: Tedesco (Germania)</p> </li> 
     <li> <p>en-AE: Inglese (Emirati Arabi Uniti)</p> </li> 
     <li> <p>en-GB: Inglese (Regno Unito)</p> </li> 
     <li> <p>en-IL: Inglese (Israele)</p> </li> 
     <li> <p>IT: Inglese (Stati Uniti d'America)</p> </li> 
     <li> <p>es-ES: Spagnolo (Spagna)</p> </li> 
     <li> <p>es-MX: Spagnolo (Messico)</p> </li> 
     <li> <p>eu-ES: Basco (Spagna)</p> </li> 
     <li> <p>FI: Finlandese (Finlandia)</p> </li> 
     <li> <p>fr-CA: Francese (Canada)</p> </li> 
     <li> <p>fr-FR: Francese (Francia)</p> </li> 
     <li> <p>fr-MA: Francese (Marocco)</p> </li> 
     <li> <p>hr-HR: Croato (Croazia)</p> </li> 
     <li> <p>hu-HU: Ungherese (Ungheria)</p> </li> 
     <li> <p>IT: Italiano (Italia)</p> </li> 
     <li> <p>ja-JP: Giapponese (Giappone)</p> </li> 
     <li> <p>kr-KR: Coreano (Corea del Sud)</p> </li> 
     <li> <p>Nb-NO: Norvegese Bokmål (Norvegia)</p> </li> 
     <li> <p>nl-NL: Olandese (Paesi Bassi)</p> </li> 
     <li> <p>pl-PL: Polacco (Polonia)</p> </li> 
     <li> <p>pt-BR: Portoghese (Brasile)</p> </li> 
     <li> <p>pt-PT: Portoghese (Portogallo)</p> </li> 
     <li> <p>RO: Rumeno (Romania)</p> </li> 
     <li> <p>ru-RU: Russo (Russia)</p> </li> 
     <li> <p>sk-SK: Slovacco (Slovacchia)</p> </li> 
     <li> <p>sl-SI: Sloveno (Slovenia)</p> </li> 
     <li> <p>sv-SE: Svedese (Svezia)</p> </li> 
     <li> <p>tr-TR: Turco (Turchia)</p> </li> 
     <li> <p>uk-UA: Ucraino (Ucraina)</p> </li> 
     <li> <p>zh-CN: Cinese (Cina continentale)</p> </li> 
     <li> <p>zh-TW: Cinese (Taiwan)</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Converti file HTML in file PDF]

Questo strumento converte un file HTML in un file PDF.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Selezionare la connessione da utilizzare per questo modulo.</p> <p>Non è necessario un [!DNL Adobe] per creare una connessione PDF Services. Per ulteriori informazioni, consulta <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">Non è necessario un [!DNL Adobe] account</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File di origine]</td> 
   <td> <p>Selezionare un file di origine da un modulo precedente o mappare il nome e i dati del file di origine.</p> <p>Importante: Il file di origine deve essere in formato HTML o ZIP. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL JSON]</td> 
   <td> <p>Se il tuo HTML fa riferimento a variabili JavaScript, puoi includerle qui. </p> <p>Per ogni variabile, fai clic su <strong>[!UICONTROL Aggiungi elemento]</strong> e include la chiave e il valore della variabile.</p> <p>Nota:   
     <ul> 
      <li> <p>Quando crei un PDF da un file ZIP, la risorsa sorgente collaterale deve includere un elemento script come: <code> &lt;script src='./json.js' type='text/javascript'&gt;&lt;/script&gt;</code> </p> </li> 
      <li> <p>Durante la creazione di un PDF da un URL, il contenuto di questo oggetto JSON viene inserito nella VM del browser prima del rendering della pagina. </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Include header e footer]</td> 
   <td> <p>Abilitare questa opzione per creare intestazioni e piè di pagina per il documento PDF.</p> 
    <ul> 
     <li> <p>L’intestazione include una data e il titolo del documento.</p> </li> 
     <li> <p>Il piè di pagina include il nome del file e un numero di pagina.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Larghezza pagina]</td> 
   <td>Immettere la larghezza in pollici della carta. Il modulo utilizza queste informazioni per formattare le pagine nel file PDF creato.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Altezza pagina]</td> 
   <td>Immettere l'altezza della carta, in pollici. Il modulo utilizza queste informazioni per formattare le pagine nel file PDF creato.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Converti immagine in file PDF]

Questo strumento converte un’immagine in un file PDF.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Selezionare la connessione da utilizzare per questo modulo.</p> <p>Non è necessario un [!DNL Adobe] per creare una connessione PDF Services. Per ulteriori informazioni, consulta <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">Non è necessario un [!DNL Adobe] account</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File di origine]</td> 
   <td> <p>Selezionare un file di origine da un modulo precedente o mappare il nome e il file immagine del file di origine.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Converti PDF in documento]

Questo strumento converte un file PDF in un documento. È possibile selezionare uno dei seguenti formati per il file di output.

* DOC
* DOCX
* PPTX
* XLSX
* RTF

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Selezionare la connessione da utilizzare per questo modulo.</p> <p>Non è necessario un [!DNL Adobe] per creare una connessione PDF Services. Per ulteriori informazioni, consulta <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">Non è necessario un [!DNL Adobe] account</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File di origine]</td> 
   <td> <p>Selezionare un file di origine da un modulo precedente o mappare il nome e i dati del file di origine.</p> <p>Il file di origine deve essere in formato PDF. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Formato file di output]</td> 
   <td> <p>Selezionare il formato di output dei file:</p> 
    <ul> 
     <li> <p>DOC</p> </li> 
     <li> <p>DOCX</p> </li> 
     <li> <p>PPTX</p> </li> 
     <li> <p>XLSX</p> </li> 
     <li> <p>RTF</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Converti PDF in immagine]

Questo strumento converte un PDF in un&#39;immagine in formato PNG o JPEG., che viene quindi trasmesso come ZIP. Il PDF viene convertito in un’immagine per pagina e ogni immagine termina con il numero di pagina. I file immagine vengono quindi combinati in un file ZIP.

Ad esempio, un file denominato &quot;TestFile&quot; con 8 pagine produrrebbe 8 immagini, denominate &quot;TestFile_1&quot; in &quot;TestFile_8&quot;. L&#39;output del modulo è un file ZIP contenente le 8 immagini.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Selezionare la connessione da utilizzare per questo modulo.</p> <p>Non è necessario un [!DNL Adobe] per creare una connessione PDF Services. Per ulteriori informazioni, consulta <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">Non è necessario un [!DNL Adobe] account</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File di origine]</td> 
   <td> <p>Selezionare un file di origine da un modulo precedente o mappare il nome e i dati del file di origine.</p> <p>Il file di origine deve essere in formato PDF. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Formato file di output]</td> 
   <td> <p>Selezionare il formato di output dei file:</p> 
    <ul> 
     <li>PNG</li> 
     <li>JPEG</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Linearizzare un file PDF]

Questo strumento consente di linearizzare un documento PDF per creare un documento PDF ottimizzato per il Web. Un documento PDF linearizzato può essere visualizzato pagina per pagina senza dover scaricare l’intero documento.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Selezionare la connessione da utilizzare per questo modulo.</p> <p>Non è necessario un [!DNL Adobe] per creare una connessione PDF Services. Per ulteriori informazioni, consulta <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">Non è necessario un [!DNL Adobe] account</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File di origine]</td> 
   <td> <p>Selezionare un file di origine da un modulo precedente o mappare il nome e i dati del file di origine.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL OCR per file PDF]

Questo strumento esegue il riconoscimento ottico dei caratteri (OCR) su un file e produce un PDF.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Selezionare la connessione da utilizzare per questo modulo.</p> <p>Non è necessario un [!DNL Adobe] per creare una connessione PDF Services. Per ulteriori informazioni, consulta <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">Non è necessario un [!DNL Adobe] account</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File di origine]</td> 
   <td> <p>Selezionare un file di origine da un modulo precedente o mappare il nome e i dati del file di origine.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL tipo OCR]</td> 
   <td> 
    <ul> 
     <li> <p>Il tipo [!UICONTROL Modificato immagine originale] garantisce che il testo sia ricercabile e selezionabile, ma modifica l’immagine originale durante il processo di pulizia (ad esempio, lo desktop) prima di posizionarlo sopra un livello di testo invisibile. Questo tipo rimuove gli artefatti indesiderati e può causare un documento più leggibile in alcuni scenari. </p> </li> 
     <li> <p>Anche il tipo di immagine originale non modificata sovrappone un livello di testo ricercabile all'immagine originale, ma in questo caso l'immagine originale rimane invariata. Questo tipo produce la massima fedeltà all'immagine originale.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Language]</td> 
   <td>Selezionare la lingua del documento.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Manipolazione della pagina in PDF]

Questo modulo consente di ruotare o eliminare in modo selettivo le pagine di un documento PDF. Ad esempio, è possibile modificare la visualizzazione verticale in visualizzazione orizzontale o rimuovere alcune pagine dal documento di PDF.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Selezionare la connessione da utilizzare per questo modulo.</p> <p>Non è necessario un [!DNL Adobe] per creare una connessione PDF Services. Per ulteriori informazioni, consulta <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">Non è necessario un [!DNL Adobe] account</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File di origine]</td> 
   <td> <p>Selezionare un file di origine da un modulo precedente o mappare il nome e i dati del file di origine.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Action]</td> 
   <td> <p>Selezionare l’azione da eseguire sul file.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Elimina]</b> </p> <p>Selezionare questa opzione per eliminare le pagine dal documento.</p> </li> 
     <li> <p><b>[!UICONTROL Ruota]</b> </p> <p>Selezionate questa opzione per ruotare le pagine, quindi immettete l'angolo, in gradi in senso orario, che desiderate ruotare le pagine del documento rispetto all'orientamento iniziale.</p> <p>Per ruotare la pagina da verticale a orizzontale o viceversa, ruotarla di 90 o 270 gradi.</p> <p>Se una pagina è capovolta, ruotala di 180 gradi.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pages]</td> 
   <td> <p>Per ogni intervallo di pagine da eliminare, fai clic su <strong>[!UICONTROL Aggiungi]</strong> quindi immetti la prima e l’ultima pagina dell’intervallo di pagine. </p> <p>Nota:   
     <ul> 
      <li> <p>È possibile utilizzare numeri negativi per contare indietro dalla fine del documento. L'ultima pagina di un documento è -1, la seconda all'ultima pagina è -2 e così via.</p> </li> 
      <li> <p>Per eliminare una singola pagina, imposta lo stesso numero di pagina sia all’inizio che alla fine dell’intervallo.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Immettere o mappare il numero massimo di record con cui si desidera che il modulo funzioni durante ogni ciclo di esecuzione degli scenari.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Proprietà dei file PDF]

Questo strumento estrae informazioni di base sul documento, ad esempio:

* Numero di pagine
* Versione PDF
* Se il file è crittografato
* Se il file è linerarizzato
* Se il file contiene file incorporati

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Selezionare la connessione da utilizzare per questo modulo.</p> <p>Non è necessario un [!DNL Adobe] per creare una connessione PDF Services. Per ulteriori informazioni, consulta <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">Non è necessario un [!DNL Adobe] account</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File di origine]</td> 
   <td> <p>Selezionare un file di origine da un modulo precedente o mappare il nome e i dati del file di origine.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL File Protect PDF]

Questo strumento protegge un documento PDF con una password utente o proprietario. Inoltre, imposta restrizioni su alcune funzioni quali stampa, modifica e copia nel documento PDF. È possibile selezionare il tipo di contenuto da cifrare e l’algoritmo di cifratura.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Selezionare la connessione da utilizzare per questo modulo.</p> <p>Non è necessario un [!DNL Adobe] per creare una connessione PDF Services. Per ulteriori informazioni, consulta <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">Non è necessario un [!DNL Adobe] account</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File di origine]</td> 
   <td> <p>Selezionare un file di origine da un modulo precedente o mappare il nome e i dati del file di origine.</p> <p>Il file di origine deve essere in formato PDF. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Password Protection Type]</td> 
   <td> <p>Abilitare questa opzione per utilizzare le password per crittografare il documento di input PDF. Se si abilita questa opzione, è necessario specificare e immettere un valore per uno o entrambi i valori seguenti: </p> 
    <ul> 
     <li> <p>[!UICONTROL userPassword]</p> </li> 
     <li> <p>[!UICONTROL ownerPassword] </p> </li> 
    </ul> <p>Ogni password può contenere fino a 128 caratteri.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Algoritmo di crittografia [!UICONTROL]</td> 
   <td> <p>Seleziona l’algoritmo di cifratura. </p> 
    <ul> 
     <li> <p>[!UICONTROL AES-128 crittografia]</p> <p>La password supporta solo i caratteri LATIN-I. </p> </li> 
     <li> <p>[!UICONTROL Crittografia AES-256]</p> <p>La password supporta il set di caratteri Unicode</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contenuto da crittografare]</td> 
   <td> <p>Seleziona il tipo di contenuto da cifrare.</p> 
    <ul> 
     <li> <p>[!UICONTROL Tutto il contenuto]</p> </li> 
     <li> <p>[!UICONTROL Tutto il contenuto tranne i metadati]</p> </li> 
     <li> <p>[!UICONTROL Solo dati incorporati] </p> </li> 
    </ul> <p>Selezionando "[!UICONTROL Only embedded data]", tutte le autorizzazioni di accesso fornite vengono rese inefficaci.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni [!UICONTROL]</td> 
   <td> <p>Seleziona le autorizzazioni da includere per consentire la stampa, la modifica o la copia dei contenuti.</p> <p>Le impostazioni delle autorizzazioni vengono utilizzate solo se [!UICONTROL ownerPassword] è impostato nel campo [!UICONTROL Password Protection Type] (Tipo di protezione password).</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Rimuovere la protezione di un file PDF]

Questo strumento rimuove la protezione (protezione tramite password) da un documento PDF.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Selezionare la connessione da utilizzare per questo modulo.</p> <p>Non è necessario un [!DNL Adobe] per creare una connessione PDF Services. Per ulteriori informazioni, consulta <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">Non è necessario un [!DNL Adobe] account</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File di origine]</td> 
   <td> <p>Selezionare un file di origine da un modulo precedente o mappare il nome e i dati del file di origine.</p> <p>Il file di origine deve essere in formato PDF.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Password]</td> 
   <td>Immettere la password che attualmente protegge il file.</td> 
  </tr> 
 </tbody> 
</table>
