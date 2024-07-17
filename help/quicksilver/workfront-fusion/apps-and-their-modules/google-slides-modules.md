---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli diapositive di Google
description: I moduli delle diapositive di Adobe Workfront Fusion Google consentono di creare, aggiornare, elencare e/o eliminare presentazioni e caricare immagini nelle presentazioni nel proprio account Google Slides.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 680a5328-1d50-4434-beda-7a4670a6e458
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1618'
ht-degree: 0%

---

# [!DNL Google Slides] moduli

I moduli [!DNL Adobe Workfront Fusion] [!DNL Google Slides] ti consentono di creare, aggiornare, elencare e/o eliminare presentazioni e caricare immagini nelle presentazioni nel tuo account [!DNL Google Slides].

Per utilizzare [!DNL Google Slides] con [!DNL Workfront Fusion], è necessario disporre di un account [!DNL Google]. Se non si dispone ancora di un account [!DNL Google], è possibile crearne uno nella pagina della guida dell&#39;account [!DNL Google].

È inoltre necessario [!DNL Google Slides] in [!DNL Google Drive].

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

## Prerequisiti

Per utilizzare i moduli [!DNL Google Slides], è necessario disporre di un account [!DNL Google].

## [!DNL Google Slides] moduli e relativi campi

Quando si configurano [!DNL Google Slides] moduli, in Workfront Fusion vengono visualizzati i campi elencati di seguito. Insieme a questi, potrebbero essere visualizzati ulteriori campi di [!DNL Google Slides], a seconda di fattori quali il livello di accesso nell&#39;app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se viene visualizzato il pulsante Mappa sopra un campo o una funzione, è possibile utilizzarlo per impostare variabili e funzioni per tale campo. Per ulteriori informazioni, vedere [Mappare le informazioni da un modulo all&#39;altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Presentazione](#presentation)
* [Altro](#other)

### Presentazione

* [[!UICONTROL Guarda Presentations]](#watch-presentations)
* [[!UICONTROL Elenca Presentations]](#list-presentations)
* [[!UICONTROL Ottieni una presentazione]](#get-a-presentation)
* [[!UICONTROL Ottieni pagina/miniatura]](#get-a-pagethumbnail)
* [[!UICONTROL Crea una presentazione da un modello]](#create-a-presentation-from-a-template)
* [[!UICONTROL Carica un&#39;immagine in una presentazione]](#upload-an-image-to-a-presentation)
* [[!UICONTROL Aggiorna grafico]](#refresh-a-chart)
* [[!UICONTROL Aggiungi/Elimina diapositiva]](#adddelete-a-slide)

#### [!UICONTROL Guarda Presentations]

Si attiva quando viene creata o aggiornata una nuova presentazione.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Google Slides] a [!DNL Workfront Fusion], vedere <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch] </td> 
   <td> <p>Seleziona l’opzione per guardare le presentazioni:</p> 
    <ul> 
     <li> <p>[!UICONTROL Data di creazione]</p> </li> 
     <li> <p>[!UICONTROL Modified Date]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Il numero massimo di presentazioni che Workfront Fusion deve restituire durante un ciclo di esecuzione di uno scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Elenca Presentations]

Recupera un elenco di tutte le presentazioni.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Google Slides] a [!DNL Workfront Fusion], vedere <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scegli un percorso unità]</td> 
   <td> <p>Selezionare [!DNL Google Drive] dove si trovano le presentazioni da elencare:</p> 
    <ul> 
     <li>[!UICONTROL Unità]</li> 
     <li>[!UICONTROL condiviso con me]</li> 
     <li>[!UICONTROL [!DNL Google] unità condivisa]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID cartella]</td> 
   <td> <p>Scegliere il percorso della cartella delle presentazioni da elencare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Il numero massimo di presentazioni [!DNL Workfront Fusion] deve essere restituito durante un ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottieni una presentazione]

Ottiene la versione più recente di una presentazione specificata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Google Slides] a [!DNL Workfront Fusion], vedere <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scegli un'unità]</td> 
   <td> <p>Selezionare [!DNL Google Drive] dove si trovano le presentazioni da elencare:</p> 
    <ul> 
     <li>[!UICONTROL Unità]</li> 
     <li>[!UICONTROL condiviso con me]</li> 
     <li>[!UICONTROL [!DNL Google] unità condivisa]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID presentazione]</td> 
   <td> <p> Selezionare la presentazione che si desidera recuperare.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottieni pagina/miniatura]

Ottiene la versione più recente della pagina specificata o della miniatura di una pagina nella presentazione.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Google Slides] a [!DNL Workfront Fusion], vedere <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID presentazione]</td> 
   <td> <p> Seleziona l’ID presentazione da recuperare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID oggetto pagina]</td> 
   <td> <p> Selezionare la diapositiva per la quale si desidera visualizzare i dettagli dell'oggetto pagina.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mostra miniatura pagina]</td> 
   <td> <p> Selezionare la casella di controllo se si desidera visualizzare le informazioni sulle miniature della pagina.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crea una presentazione da un modello]

Crea una nuova presentazione sostituendo tutti i tag come `{{Name}}`, `{{Email}}` in un modello con i dati forniti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Google Slides] a [!DNL Workfront Fusion], vedere <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Title] </td> 
   <td> <p>Immettere un nome per la nuova presentazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Copia presentazione]</td> 
   <td> <p> Selezionare l'opzione se si sta copiando una presentazione esistente:</p> 
    <ul> 
     <li>[!UICONTROL Per Mappatura]</li> 
     <li>[!UICONTROL Per Elenco A Discesa]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Copia dell'ID presentazione esistente]</td> 
   <td> <p> Immettere il Percorso o l'ID presentazione di una presentazione esistente che si desidera copiare. Questo campo viene visualizzato se si sta creando la presentazione [!UICONTROL By Mapping].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scegli un'unità]</td> 
   <td> <p>Selezionare [!DNL Google Drive] dove si trovano le presentazioni da elencare:</p> 
    <ul> 
     <li>[!UICONTROL Unità]</li> 
     <li>[!UICONTROL condiviso con me]</li> 
     <li>[!UICONTROL [!DNL Google] unità condivisa]</li> 
    </ul> <p>Questo campo viene visualizzato se si sta creando la presentazione [!UICONTROL Per elenco a discesa].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID presentazione]</td> 
   <td> <p> Selezionare l'ID presentazione della presentazione che si desidera utilizzare come modello.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Values] </td> 
   <td> <p>Aggiungi i valori:</p> 
    <ul> 
     <li><strong>[!UICONTROL Tag]</strong>: immettere il tag che si desidera sostituire nella presentazione. Ad esempio: <code>&#123;&#123;Name&#125;&#125;</code></li> 
     <li><strong>[!UICONTROL Replaced Value]</strong>: immetti il valore con cui sostituire il tag esistente. Ad esempio, se una stringa <tr><ul><tr><tr><tr><code>&#123;&#123;Name&#125;&#125;/code> in the presentation and the replaced value is Sample, then the <code>&#123;&#123;Name}}</code> will be replaced by <code>Sample</code>.</li> 
    </ul> </td> 
  </tr> 
   
   <td role="rowheader">[!UICONTROL New Drive Location]</td> 
   <td> <p>Select the [!DNL Google Drive] where you want to store or add the new presentation:</p> 
     
     <li>[!UICONTROL My Drive]</li> 
     <li>[!UICONTROL Shared With Me]</li> 
     <li>[!UICONTROL [!DNL Google] Shared Drive]</li> 
    </ul> </td> 
  </tr> 
   
   <td role="rowheader"> <p>[!UICONTROL New Document's Location]</p> </td> 
   <td> <p>Select the folder where you want to store or add the presentation.</p> </td> 
  </tr> 
   
   <td role="rowheader">[!UICONTROL Shared] </td> 
   <td> <p>Select if you want to share the presentation.</p> </td> 
  </tr> 
   
   <td role="rowheader">[!UICONTROL Sharing with Other's Email Address]</td> 
   <td> <p> Enter the email address with whom you want to share the presentation. If you are not entering an email address and selecting only shared field, the presentation is shareable to anyone.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Carica un&#39;immagine in una presentazione]

Carica un’immagine con i dati forniti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Google Slides] a [!DNL Workfront Fusion], vedere <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scegli presentazione]</td> 
   <td> <p>Scegliere come selezionare la presentazione in cui si sta caricando un'immagine.</p> 
    <ul> 
     <li>[!UICONTROL Per Mappatura]</li> 
     <li>[!DNL By Dropdown]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scegli un'unità]</td> 
   <td> <p>Selezionare [!DNL Google Drive] dove si trovano le presentazioni da elencare:</p> 
    <ul> 
     <li>[!UICONTROL Unità]</li> 
     <li>[!UICONTROL condiviso con me]</li> 
     <li>[!UICONTROL [!DNL Google] unità condivisa]</li> 
    </ul> <p>Questo campo viene visualizzato se si sta creando la presentazione [!UICONTROL Per elenco a discesa].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID presentazione]</td> 
   <td> <p> Seleziona l’ID presentazione della presentazione in cui stai caricando un’immagine.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Values]</td> 
   <td> <p>Valori Aggiungi i valori:</p> 
    <ul> 
     <li><strong>[!UICONTROL Tag]</strong>: immettere il tag a cui si desidera aggiungere l'URL.</li> 
     <li><strong>[!UICONTROL URL immagine]</strong>: immettere il percorso o l'URL dell'immagine da caricare.</li> 
    </ul> <p>Nota: le dimensioni delle immagini devono essere inferiori a 50 MB, non devono superare i 25 megapixel e devono essere in formato PNG, JPEG o GIF.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggiorna grafico]

Aggiorna i dati del grafico memorizzati in una presentazione specificata dall&#39;ID.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Google Slides] a [!DNL Workfront Fusion], vedere <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scegli un'unità]</td> 
   <td> <p>Selezionare [!DNL Google Drive] dove si trovano le presentazioni da elencare:</p> 
    <ul> 
     <li>[!UICONTROL Unità]</li> 
     <li>[!UICONTROL condiviso con me]</li> 
     <li>[!UICONTROL [!DNL Google] unità condivisa]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID presentazione]</td> 
   <td> <p>Selezionare l'ID presentazione della presentazione che include il grafico da aggiornare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID oggetto grafico]</td> 
   <td> <p> Selezionare il grafico da aggiornare.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggiungi/Elimina diapositiva]

Crea una diapositiva vuota o elimina una diapositiva esistente nella presentazione specificata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Google Slides] a [!DNL Workfront Fusion], vedere <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Selezionare il metodo]</td> 
   <td> <p>Scegliere se si desidera aggiungere una nuova diapositiva o eliminarla.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Presentation ID]</td> 
   <td> <p>Selezionare l'ID presentazione della presentazione per la quale si desidera aggiungere o eliminare una diapositiva.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di layout predefinito]</td> 
   <td> <p> Selezionare il layout di diapositiva predefinito che si desidera utilizzare per la diapositiva aggiunta. Specificare i valori per eventuali campi aggiuntivi, ad esempio [!UICONTROL Title].</p> 
    <ul> 
     <li>[!UICONTROL Layout vuoto, senza segnaposto]</li> 
     <li>[!UICONTROL Layout con una didascalia in basso]</li> 
     <li>[!UICONTROL Layout con titolo e sottotitolo]</li> 
     <li>[!UICONTROL Layout con titolo e corpo]</li> 
     <li>[!UICONTROL Layout con titolo e due colonne]</li> 
     <li>[!UICONTROL Layout con solo un titolo]</li> 
     <li>[!UICONTROL Layout con titolo sezione]</li> 
     <li>[!UICONTROL Layout con titolo e sottotitolo su un lato e descrizione sull'altro]</li> 
     <li>[!UICONTROL Layout con un titolo e un corpo, disposti in una singola colonna]</li> 
     <li>[!UICONTROL Layout con un punto principale]</li> 
     <li>[!DNL Layout with a big number heading]</li> 
    </ul> <p>Questo campo è disponibile se si è selezionato di aggiungere una diapositiva.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Altro

* [[!UICONTROL Effettuare una chiamata API]](#make-an-api-call)
* [[!UICONTROL Inserire collegamenti in una presentazione]](#insert-links-in-a-presentation)

#### [!UICONTROL Effettuare una chiamata API]

Esegue una chiamata API autorizzata arbitraria.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Google Slides] a [!DNL Workfront Fusion], vedere <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> <p>Immetti un percorso relativo a https://developers.google.com/slides/. Ad es. Presentazione.</p> <p>Per l'elenco degli endpoint disponibili, fare riferimento alla documentazione API <a href="https://developers.google.com/slides/reference/rest">[!DNL Google Slides]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, vedere <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Inserisci le intestazioni di richiesta desiderate. Non è necessario aggiungere intestazioni di autorizzazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Stringa Di Query]</td> 
   <td> <p> Immettere la stringa di query richiesta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Aggiungi il contenuto body per la chiamata API sotto forma di oggetto JSON standard.</p> <p>Nota:  <p>Quando si utilizzano istruzioni condizionali come <code>if</code> nel JSON, inserire le virgolette al di fuori dell'istruzione condizionale.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Esempio:** utilizzando una chiamata API è possibile ottenere i dettagli della presentazione per l&#39;ID presentazione immesso. È possibile trovare l&#39;ID presentazione nell&#39;URL quando si apre la presentazione in [!DNL Google Slides].
>
>![](assets/api-call-350x13.png)
>
>La seguente chiamata API restituisce i dettagli della presentazione:
>
>![](assets/presentation-details.png)
>
>Le corrispondenze della ricerca si trovano nell&#39;output del modulo in [!UICONTROL Bundle] > [!UICONTROL Body] > [!UICONTROL presentationId].
>
>Nel nostro esempio, sono stati restituiti i dettagli della presentazione richiesti:
>
>![](assets/presentation-details-2.png)

#### [!UICONTROL Inserire collegamenti in una presentazione]

Questo modulo rende selezionabili tutti i collegamenti di una presentazione o inserisce un collegamento in tutti i testi di input corrispondenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Google Slides] a [!DNL Workfront Fusion], vedere <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scegli presentazione]</td> 
   <td> <p>Scegliere come selezionare la presentazione in cui si sta caricando un'immagine.</p> 
    <ul> 
     <li>[!UICONTROL Per Mappatura]</li> 
     <li>[!UICONTROL Per Elenco A Discesa]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scegli un'unità]</td> 
   <td> <p>Selezionare [!DNL Google Drive] dove si trovano le presentazioni da elencare:</p> 
    <ul> 
     <li>[!UICONTROL Unità]</li> 
     <li>[!UICONTROL condiviso con me]</li> 
     <li>[!UICONTROL [!DNL Google] unità condivisa]</li> 
    </ul> <p>Questo campo viene visualizzato se si sta creando la presentazione [!UICONTROL Per elenco a discesa].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID presentazione]</td> 
   <td> <p>Scegliere il percorso della cartella delle presentazioni da elencare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select]</td> 
   <td> <p>Selezionare se si desidera rendere selezionabili tutti i collegamenti di una presentazione o se si desidera inserire un collegamento in tutti i testi di input corrispondenti.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Input Testo]</td> 
   <td>Per ogni elemento di testo per il quale si desidera aggiungere un collegamento, aggiungere all'elenco l'elemento e il relativo collegamento associato. Ogni volta che l'elemento viene visualizzato nella presentazione, verrà automaticamente collegato al sito specificato.</td> 
  </tr> 
 </tbody> 
</table>
