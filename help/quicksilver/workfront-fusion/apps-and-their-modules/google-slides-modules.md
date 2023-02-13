---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli scorrevoli Google
description: I moduli Slides di Adobe Workfront Fusion Google consentono di creare, aggiornare, elencare e/o eliminare presentazioni e caricare immagini in presentazioni nel tuo account Slides Google.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 680a5328-1d50-4434-beda-7a4670a6e458
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1575'
ht-degree: 0%

---

# [!DNL Google Slides] moduli

La [!DNL Adobe Workfront Fusion] [!DNL Google Slides] i moduli consentono di creare, aggiornare, elencare e/o eliminare presentazioni e caricare immagini nelle presentazioni [!DNL Google Slides] conto.

Per utilizzare [!DNL Google Slides] con [!DNL Workfront Fusion], è necessario disporre di un [!DNL Google] conto. Se non hai un [!DNL Google] tuttavia, è possibile crearne una nella [!DNL Google] Pagina della guida dell’account.

Hai anche bisogno di [!DNL Google Slides] nel tuo [!DNL Google Drive].

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

Per utilizzare [!DNL Google Slides] moduli, è necessario disporre di un [!DNL Google] conto.

## [!DNL Google Slides] moduli e relativi campi

Quando si configura [!DNL Google Slides] Workfront Fusion visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL Google Slides] potrebbero essere visualizzati, a seconda di fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se trovi il pulsante mappa sopra un campo o una funzione, puoi utilizzarlo per impostare variabili e funzioni per quel campo. Per ulteriori informazioni, consulta [Mappare informazioni da un modulo a un altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Presentazione](#presentation)
* [Altro](#other)

### Presentazione

* [[!UICONTROL Guarda Presentations]](#watch-presentations)
* [[!UICONTROL Elenco Presentations]](#list-presentations)
* [[!UICONTROL Ottenere una presentazione]](#get-a-presentation)
* [[!UICONTROL Ottieni una pagina/miniatura]](#get-a-pagethumbnail)
* [[!UICONTROL Creare una presentazione da un modello]](#create-a-presentation-from-a-template)
* [[!UICONTROL Caricare un’immagine in una presentazione]](#upload-an-image-to-a-presentation)
* [[!UICONTROL Aggiornare un grafico]](#refresh-a-chart)
* [[!UICONTROL Aggiungere/eliminare una diapositiva]](#adddelete-a-slide)

#### [!UICONTROL Guarda Presentations]

Attiva quando viene creata o aggiornata una nuova presentazione.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google Slides] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch] </td> 
   <td> <p>Seleziona l’opzione per guardare le presentazioni:</p> 
    <ul> 
     <li> <p>[!UICONTROL Data di creazione]</p> </li> 
     <li> <p>[!UICONTROL Data di modifica]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Il numero massimo di presentazioni che Workfront Fusion deve restituire durante un ciclo di esecuzione di uno scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Elenco Presentations]

Recupera un elenco di tutte le presentazioni.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google Slides] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scegli una posizione dell'unità]</td> 
   <td> <p>Seleziona la [!DNL Google Drive] dove si trovano le presentazioni da elencare:</p> 
    <ul> 
     <li>[!UICONTROL My Drive]</li> 
     <li>[!UICONTROL Condiviso Con Me]</li> 
     <li>[!UICONTROL [!DNL Google] Unità condivisa]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID cartella [!UICONTROL]</td> 
   <td> <p>Scegli il percorso della cartella delle presentazioni da elencare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Numero massimo di presentazioni [!DNL Workfront Fusion] dovrebbe essere restituito durante un ciclo di esecuzione di uno scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottenere una presentazione]

Ottiene la versione più recente di una presentazione specificata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google Slides] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scegliere un'unità]</td> 
   <td> <p>Seleziona la [!DNL Google Drive] dove si trovano le presentazioni da elencare:</p> 
    <ul> 
     <li>[!UICONTROL My Drive]</li> 
     <li>[!UICONTROL Condiviso Con Me]</li> 
     <li>[!UICONTROL [!DNL Google] Unità condivisa]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID presentazione]</td> 
   <td> <p> Selezionare la presentazione da recuperare.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottieni una pagina/miniatura]

Ottiene la versione più recente della pagina specificata o della miniatura di una pagina nella presentazione.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google Slides] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID presentazione]</td> 
   <td> <p> Selezionare l'ID presentazione che si desidera recuperare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Page Object ID]</td> 
   <td> <p> Selezionare la diapositiva per la quale si desidera visualizzare i dettagli dell'oggetto pagina.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mostra miniatura pagina]</td> 
   <td> <p> Seleziona la casella di controllo se desideri visualizzare le informazioni sulle miniature della pagina.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Creare una presentazione da un modello]

Crea una nuova presentazione sostituendo tutti i tag come `{{Name}}`, `{{Email}}` in un modello con i dati forniti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google Slides] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Title] </td> 
   <td> <p>Immettere un nome per la nuova presentazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Copiare una presentazione]</td> 
   <td> <p> Selezionare l'opzione se si sta copiando una presentazione esistente:</p> 
    <ul> 
     <li>[!UICONTROL By Mapping]</li> 
     <li>[!UICONTROL By Dropdown]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Copia dell'ID presentazione esistente]</td> 
   <td> <p> Immettere l'ID percorso o presentazione di una presentazione esistente da copiare. Questo campo viene visualizzato se si sta creando la presentazione [!UICONTROL By Mapping].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scegliere un'unità]</td> 
   <td> <p>Seleziona la [!DNL Google Drive] dove si trovano le presentazioni da elencare:</p> 
    <ul> 
     <li>[!UICONTROL My Drive]</li> 
     <li>[!UICONTROL Condiviso Con Me]</li> 
     <li>[!UICONTROL [!DNL Google] Unità condivisa]</li> 
    </ul> <p>Questo campo viene visualizzato se si sta creando la presentazione [!UICONTROL By Dropdown].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID presentazione]</td> 
   <td> <p> Selezionare l'ID presentazione della presentazione che si desidera utilizzare come modello.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Values] </td> 
   <td> <p>Aggiungi i valori seguenti:</p> 
    <ul> 
     <li><strong>Tag [!UICONTROL]</strong>: Immettere il tag da sostituire nella presentazione. Ad esempio: <code>&#123;&#123;Name&#125;&#125;</code></li> 
     <li><strong>[!UICONTROL Valore Sostituito]</strong>: Immetti il valore con cui deve essere sostituito il tag esistente. Ad esempio, se una stringa <code>&#123;&#123;Name}}</code><code>Sample</code></li></ul></td></tr><tr><td role="rowheader"></td><td><p></p><ul><li></li><li></li><li></li></ul></td></tr><tr><td role="rowheader"><p></p></td><td><p></p></td></tr><tr><td role="rowheader"></td><td><p></p></td></tr><tr><td role="rowheader"></td><td><p></p></td></tr></tbody></table>

#### [!UICONTROL Caricare un’immagine in una presentazione]

Carica un’immagine con i dati specificati.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google Slides] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scegliere una presentazione]</td> 
   <td> <p>Scegli come selezionare la presentazione in cui si sta caricando un'immagine.</p> 
    <ul> 
     <li>[!UICONTROL By Mapping]</li> 
     <li>[!DNL By Dropdown]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scegliere un'unità]</td> 
   <td> <p>Seleziona la [!DNL Google Drive] dove si trovano le presentazioni da elencare:</p> 
    <ul> 
     <li>[!UICONTROL My Drive]</li> 
     <li>[!UICONTROL Condiviso Con Me]</li> 
     <li>[!UICONTROL [!DNL Google] Unità condivisa]</li> 
    </ul> <p>Questo campo viene visualizzato se si sta creando la presentazione [!UICONTROL By Dropdown].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID presentazione]</td> 
   <td> <p> Seleziona l'ID presentazione della presentazione in cui stai caricando un'immagine.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Values]</td> 
   <td> <p>Valori Aggiungi i valori seguenti:</p> 
    <ul> 
     <li><strong>Tag [!UICONTROL]</strong>: Inserisci il tag a cui desideri aggiungere l’URL.</li> 
     <li><strong>[!UICONTROL URL immagine]</strong>: Immetti il percorso o l’URL dell’immagine da caricare.</li> 
    </ul> <p>Nota: Le immagini devono avere dimensioni inferiori a 50 MB, non possono superare i 25 megapixel e devono essere in formato PNG, JPEG o GIF.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggiornare un grafico]

Aggiorna i dati del grafico memorizzati in una presentazione specificata dall&#39;ID.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google Slides] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scegliere un'unità]</td> 
   <td> <p>Seleziona la [!DNL Google Drive] dove si trovano le presentazioni da elencare:</p> 
    <ul> 
     <li>[!UICONTROL My Drive]</li> 
     <li>[!UICONTROL Condiviso Con Me]</li> 
     <li>[!UICONTROL [!DNL Google] Unità condivisa]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID presentazione]</td> 
   <td> <p>Selezionare l'ID presentazione della presentazione che include il grafico che si desidera aggiornare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Chart Object ID]</td> 
   <td> <p> Selezionare il grafico che si desidera aggiornare.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggiungere/eliminare una diapositiva]

Crea una diapositiva vuota o elimina una diapositiva esistente nella presentazione specificata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google Slides] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Selezionare il metodo]</td> 
   <td> <p>Scegliere se si desidera aggiungere una nuova diapositiva o eliminare una diapositiva.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Presentation ID]</td> 
   <td> <p>Selezionare l'ID presentazione della presentazione per la quale si desidera aggiungere o eliminare una diapositiva.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di layout predefinito]</td> 
   <td> <p> Selezionare il layout diapositiva predefinito che si desidera utilizzare per la diapositiva aggiunta. Specifica i valori per eventuali campi aggiuntivi, ad esempio [!UICONTROL Title].</p> 
    <ul> 
     <li>[!UICONTROL Layout vuoto, senza segnaposto]</li> 
     <li>[!UICONTROL Layout con una didascalia in basso]</li> 
     <li>[!UICONTROL Layout con titolo e sottotitolo]</li> 
     <li>[!UICONTROL Layout con titolo e corpo]</li> 
     <li>[!UICONTROL Layout con un titolo e due colonne]</li> 
     <li>[!UICONTROL Layout con un solo titolo]</li> 
     <li>[!UICONTROL Layout con un titolo di sezione]</li> 
     <li>[!UICONTROL Layout con titolo e sottotitolo da un lato e descrizione dall’altro]</li> 
     <li>[!UICONTROL Layout con un titolo e un corpo, disposti in una singola colonna]</li> 
     <li>[!UICONTROL Layout con un punto principale]</li> 
     <li>[!DNL Layout with a big number heading]</li> 
    </ul> <p>Questo campo è disponibile se è stato selezionato per aggiungere una diapositiva.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Altro

* [[!UICONTROL Effettuare una chiamata API]](#make-an-api-call)
* [[!UICONTROL Inserire collegamenti in una presentazione]](#insert-links-in-a-presentation)

#### [!UICONTROL Effettuare una chiamata API]

Esegue una chiamata API arbitraria autorizzata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google Slides] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> <p>Immetti un percorso relativo a https://developers.google.com/slides/. Ad esempio Presentazione.</p> <p>Per l’elenco degli endpoint disponibili, consulta <a href="https://developers.google.com/slides/reference/rest">[!DNL Google Slides] Documentazione API</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL, Metodo]</td> 
   <td> <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Immetti le intestazioni di richiesta desiderate. Non è necessario aggiungere intestazioni di autorizzazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p> Immetti la stringa di query della richiesta.</p> </td> 
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

>[!INFO]
>
>**Esempio:** Utilizzando una chiamata API puoi ottenere i dettagli della presentazione per l’ID presentazione immesso. Puoi trovare l’ID della presentazione nell’URL quando apri la presentazione in [!DNL Google Slides].
>
>![](assets/api-call-350x13.png)
>
>La seguente chiamata API restituisce i dettagli della presentazione:
>
>![](assets/presentation-details.png)
>
>Le corrispondenze della ricerca si trovano nell&#39;Output del modulo in [!UICONTROL Bundle] > [!UICONTROL Corpo] > [!UICONTROL presentazioneId].
>
>Nel nostro esempio, sono stati restituiti i dettagli di presentazione richiesti:
>
>![](assets/presentation-details-2.png)

#### [!UICONTROL Inserire collegamenti in una presentazione]

Questo modulo rende cliccabili tutti i collegamenti di una presentazione, o inserisce un collegamento in tutti i testi di input corrispondenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google Slides] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scegliere una presentazione]</td> 
   <td> <p>Scegli come selezionare la presentazione in cui si sta caricando un'immagine.</p> 
    <ul> 
     <li>[!UICONTROL By Mapping]</li> 
     <li>[!UICONTROL By Dropdown]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scegliere un'unità]</td> 
   <td> <p>Seleziona la [!DNL Google Drive] dove si trovano le presentazioni da elencare:</p> 
    <ul> 
     <li>[!UICONTROL My Drive]</li> 
     <li>[!UICONTROL Condiviso Con Me]</li> 
     <li>[!UICONTROL [!DNL Google] Unità condivisa]</li> 
    </ul> <p>Questo campo viene visualizzato se si sta creando la presentazione [!UICONTROL By Dropdown].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID presentazione]</td> 
   <td> <p>Scegli il percorso della cartella delle presentazioni da elencare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select]</td> 
   <td> <p>Selezionare se si desidera fare clic su tutti i collegamenti di una presentazione o se si desidera inserire un collegamento in tutti i testi di input corrispondenti.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Testo Ingressi]</td> 
   <td>Per ogni elemento di testo per il quale desideri aggiungere un collegamento, aggiungi all’elenco l’elemento e il relativo collegamento associato. Ogni volta che l'elemento viene visualizzato nella presentazione, viene automaticamente collegato al sito specificato.</td> 
  </tr> 
 </tbody> 
</table>
