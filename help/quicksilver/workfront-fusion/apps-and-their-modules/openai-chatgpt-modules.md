---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli OpenAI (ChatGPT)
description: In uno scenario Adobe Workfront Fusion, puoi automatizzare i flussi di lavoro che utilizzano OpenAIT(ChatGPT), nonché collegarlo a più applicazioni e servizi di terze parti.
author: Becky
feature: Workfront Fusion
source-git-commit: a8bc882f393dcf17bca80da86c25c053272e27c9
workflow-type: tm+mt
source-wordcount: '1395'
ht-degree: 0%

---

# [!DNL OpenAI (ChatGPT & DALL-E)] moduli

In un [!DNL Adobe Workfront Fusion] scenario, puoi automatizzare i flussi di lavoro che utilizzano [!DNL OpenAI (ChatGPT & DALL-E)], oltre a collegarlo a più applicazioni e servizi di terze parti.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] per l'automazione e l'integrazione del lavoro] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare la funzionalità descritta in questo articolo.</td> 
  </tr> 
 </tbody> 
</table>

Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, consulta [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Prerequisiti

Da utilizzare [!DNL OpenAI (ChatGPT & DALL-E)] moduli, è necessario disporre di un [!DNL OpenAI] , inclusa una chiave API e un ID organizzazione.

## Connessione [!DNL OpenAI (ChatGPT & DALL-E)] a [!DNL Workfront Fusion]

Puoi creare una connessione al tuo [!DNL OpenAI (ChatGPT & DALL-E)] account direttamente da un [!DNL OpenAI (ChatGPT & DALL-E)] modulo.

1. In qualsiasi [!DNL OpenAI (ChatGPT & DALL-E)] modulo, fai clic su **[!UICONTROL Aggiungi]** accanto al [!UICONTROL Connessione] campo.
1. Immettere le seguenti informazioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Nome connessione]</p> </td> 
      <td> <p>Immettere un nome per la nuova connessione.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL API Key]</td> 
      <td>Puoi individuare la tua chiave API nelle impostazioni utente di OpenAI.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL ID organizzazione] </td> 
      <td>Puoi individuare il tuo ID organizzazione nella pagina Impostazioni organizzazione in OpenAI.</td> 
     </tr> 
    </tbody> 
   </table>

1. Clic **[!UICONTROL Continua]** per creare la connessione e tornare al modulo.


## [!DNL OpenAI (ChatGPT & DALL-E)] moduli e relativi campi

Quando si configura [!DNL OpenAI (ChatGPT & DALL-E)] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL OpenAI (ChatGPT & DALL-E)] I campi potrebbero essere visualizzati in base a fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se viene visualizzato il pulsante Mappa sopra un campo o una funzione, è possibile utilizzarlo per impostare variabili e funzioni per tale campo. Per ulteriori informazioni, consulta [Mappare le informazioni da un modulo all’altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Creare un completamento

Questo modulo di azione crea un completamento per il prompt o la chat forniti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL OpenAI (ChatGPT & DALL-E)] account a Workfront Fusion, vedi <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Connessione [!DNL OpenAI (ChatGPT & DALL-E)] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Model]</td> 
   <td> Inserisci o mappa l’ID del modello da utilizzare. Puoi utilizzare il modulo Ottieni modelli per visualizzare tutti i modelli disponibili. </td> 
  </tr> 
  <!--<tr> 
   <td role="rowheader">[!UICONTROL Temperature]</td> 
   <td> This value must be between 0 and 2, and determines the randomness of the output. Higher values produce output that is more random, while lower values produce more focused output. </td> 
  </tr> -->
  <tr> 
   <td role="rowheader">[!UICONTROL Impostazioni avanzate]</td> 
   <td> <p>Per informazioni sulle impostazioni avanzate facoltative in questo modulo, vedere le informazioni sulla creazione di completamenti in <a href="https://platform.openai.com/docs/api-reference/completions/create" class="MCXref xref">Documentazione API OpenAI</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Crea moderazione

Questo modulo di azione determina se il testo viola il criterio del contenuto di OpenAI.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL OpenAI (ChatGPT & DALL-E)] account a Workfront Fusion, vedi <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Connessione [!DNL OpenAI (ChatGPT & DALL-E)] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Input]</td> 
   <td> Per ogni esempio di testo che si desidera includere, fare clic su <b>Aggiungi elemento</b> e immetti o mappa il testo. Includere l'intero testo di esempio.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Model]</td> 
   <td> Inserisci o mappa l’ID del modello da utilizzare. Puoi utilizzare il modulo Ottieni modelli per visualizzare tutti i modelli disponibili. </td> 
  </tr> 
 </tbody> 
</table>

### Creare una modifica

Questo modulo di azione restituisce una versione modificata di un prompt fornito, seguendo le istruzioni.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL OpenAI (ChatGPT & DALL-E)] account a Workfront Fusion, vedi <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Connessione [!DNL OpenAI (ChatGPT & DALL-E)] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Model]</td> 
   <td> Inserisci o mappa l’ID del modello da utilizzare. Puoi utilizzare il modulo Ottieni modelli per visualizzare tutti i modelli disponibili. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Input]</td> 
   <td> Immettere o mappare il testo da modificare. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Istruzione [!UICONTROL]</td> 
   <td> Immetti o mappa le istruzioni per la modifica. Esempio: "Correggi gli errori di ortografia". </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Impostazioni avanzate]</td> 
   <td> <p>Per informazioni sulle impostazioni avanzate facoltative in questo modulo, consulta le informazioni sulla creazione di modifiche in <a href="https://platform.openai.com/docs/api-reference/edits/create" class="MCXref xref">Documentazione API OpenAI</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Creare un’incorporazione

Questo modulo di azione crea un vettore di incorporamento che rappresenta il testo di input.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL OpenAI (ChatGPT & DALL-E)] account a Workfront Fusion, vedi <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Connessione [!DNL OpenAI (ChatGPT & DALL-E)] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Model]</td> 
   <td> Inserisci o mappa l’ID del modello da utilizzare. Puoi utilizzare il modulo Ottieni modelli per visualizzare tutti i modelli disponibili. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Testo di input da incorporare]</td> 
   <td> Inserisci o mappa il testo da incorporare. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID utente]</td> 
   <td> Inserisci o mappa un identificatore univoco che rappresenta l’utente finale, per consentire a OpenAI di monitorare e rilevare eventuali abusi </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> Immettere o mappare il numero massimo di modifiche con cui si desidera lavorare il modulo durante ogni ciclo di esecuzione dello scenario.</td> 
  </tr> 
 </tbody> 
</table>

### Crea completamento chat

Dato un elenco di messaggi che descrivono una conversazione, questo modulo di azione restituisce una risposta.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL OpenAI (ChatGPT & DALL-E)] account a Workfront Fusion, vedi <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Connessione [!DNL OpenAI (ChatGPT & DALL-E)] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Model]</td> 
   <td> Inserisci o mappa l’ID del modello da utilizzare. Puoi utilizzare il modulo Ottieni modelli per visualizzare tutti i modelli disponibili. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Messages]</td> 
   <td>I messaggi descrivono la conversazione fino ad ora. Per ogni messaggio che desideri aggiungere, fai clic su <b>Aggiungi elemento</b> e compila quanto segue:
   <ul>
   <li> <b>Ruolo</b>: seleziona il ruolo dell’autore del messaggio.</li>
   <li> <b>Contenuto</b>: inserisci o mappa il contenuto di questo messaggio.</li>
   <li> <b>Nome</b>: immetti o mappa il nome dell’autore del messaggio. Il nome può contenere lettere maiuscole e minuscole, numeri e trattini bassi. La lunghezza massima per il nome è di 64 caratteri.</li>
   </ul>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Impostazioni avanzate]</td> 
   <td> <p>Per informazioni sulle impostazioni avanzate facoltative in questo modulo, vedere le informazioni sulla creazione di completamenti chat in <a href="https://platform.openai.com/docs/api-reference/chat/create" class="MCXref xref">Documentazione API OpenAI</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--

### Edit image

This action module makes edits or creates variations of existing images.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL OpenAI (ChatGPT & DALL-E)] account to Workfront Fusion, see <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Connecting [!DNL OpenAI (ChatGPT & DALL-E)] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select the operation]</td> 
   <td> Select whether you want to create edits or variations of the image.
   <p>NOTE: Images must be a valid PNG file, less than 4MB, and square. If mask is not provided, the image must have transparency, which will be used as the mask.</p> 
 </td> 
  </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td>Select a source file from a previous module, or map the source file's name and data.</td> 
  </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Text description of desired image]</td> 
   <td> <p>If editing an image, enter or map a description of the edits you want to create. Maximum length is 1000 characters.</p> </td> 
  </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Advanced settings]</td> 
   <td> <p>For information about the optional advanced settings in this module, see the information about creating image edits or variations in the <a href="https://platform.openai.com/docs/api-reference/images/createEdit" class="MCXref xref">OpenAI API documentation</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

### Genera immagini

Questo modulo di azione genera o modifica immagini con modelli Dall-E.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL OpenAI (ChatGPT & DALL-E)] account a Workfront Fusion, vedi <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Connessione [!DNL OpenAI (ChatGPT & DALL-E)] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Descrizione testo dell'immagine desiderata]</td> 
   <td> Inserisci o mappa una descrizione dell’immagine desiderata. La lunghezza massima della descrizione è di 1000 caratteri. 
 </td> 
  </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Impostazioni avanzate]</td> 
   <td> <p>Per informazioni sulle impostazioni avanzate facoltative di questo modulo, vedere le informazioni sulla creazione di immagini in <a href="https://platform.openai.com/docs/api-reference/images/create" class="MCXref xref">Documentazione API OpenAI</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Ottieni modelli

Questo modulo elenca e descrive i vari modelli disponibili nell’API OpenAI.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL OpenAI (ChatGPT & DALL-E)] account a Workfront Fusion, vedi <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Connessione [!DNL OpenAI (ChatGPT & DALL-E)] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Action]</td> 
   <td> Seleziona se desideri ottenere un elenco di tutti i modelli o recuperare un modello specifico.
    <ul>
    <li><p><b>Modelli di elenco </b></p><p>Questa azione elenca i modelli attualmente disponibili e fornisce informazioni di base su ciascuno di essi, ad esempio il proprietario e la disponibilità.</p></li>
    <li><p><b>Recupera modello </b></p><p>Inserisci o mappa l’ID del modello da recuperare. </p></li>
   </ul>
 </td> 
 </tbody> 
</table>

### Effettuare una chiamata API personalizzata

Questa azione invia una richiesta HTTP personalizzata all’API OpenAI.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL OpenAI (ChatGPT & DALL-E)] account a Workfront Fusion, vedi <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Connessione [!DNL OpenAI (ChatGPT & DALL-E)] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> <p>Inserisci un percorso relativo a <code>https://api.openai.com/v1/</code> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
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

<!--

### Manage Audio

This action modules converts audio to text.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL OpenAI (ChatGPT & DALL-E)] account to Workfront Fusion, see <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Connecting [!DNL OpenAI (ChatGPT & DALL-E)] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select the operation]</td> 
   <td> Select whether you want to transcribe the audio into the input language, or into English.
   <p>If transcribing into the input language, you can select the language in this module's advanced settings. </td> 
  </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td>Select a source file from a previous module, or map the source file's name and data.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> Enter or map the maximum number of edits you want the module to work with during each scenario execution cycle.</td> 
   <tr> 
   <td role="rowheader">[!UICONTROL Advanced settings]</td> 
   <td> <p>For information about the optional advanced settings in this module, see the information about creating transcriptions in the <a href="https://platform.openai.com/docs/api-reference/audio/createTranscription" class="MCXref xref">OpenAI API documentation</a>.</p> </td> 
  </tr> 
  </tr> 
 </tbody> 
</table>

-->

### Gestione file

Questo modulo di azione elenca, elimina o recupera file o contenuto di file.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL OpenAI (ChatGPT & DALL-E)] account a Workfront Fusion, vedi <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Connessione [!DNL OpenAI (ChatGPT & DALL-E)] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Action]</td> 
   <td> Seleziona l’azione da eseguire. 
  </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL ID file]</td> 
   <td> Se si elimina un file o si recupera il relativo contenuto, immettere o mappare l'ID del file. 
  </tr> 
</tbody>
</table>

### Gestione ottimizzazioni

Gestisci i processi di ottimizzazione per adattare un modello ai tuoi dati di formazione specifici.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL OpenAI (ChatGPT & DALL-E)] account a Workfront Fusion, vedi <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Connessione [!DNL OpenAI (ChatGPT & DALL-E)] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seleziona l'operazione]</td> 
   <td> Seleziona l’azione da eseguire.
   <ul>
   <li><p>Ottimizzare un modello da un set di dati</p><p>Immettere o mappare una descrizione per l'immagine desiderata.</p>
     <li><p>Ottenere informazioni su un processo di ottimizzazione</p><p>Inserisci o mappa l’ID del processo.</p>
   <li><p>Annullare un processo di ottimizzazione</p><p>Inserisci o mappa l’ID del processo.</p>
   <li><p>Annullare un processo di ottimizzazione</p><p>Inserisci o mappa l’ID del processo.</p>
   <li><p>Ottenere aggiornamenti dello stato per un processo di ottimizzazione</p><p>Inserisci o mappa l’ID del processo e seleziona se desideri inviare questi aggiornamenti in streaming.</p>
   <li><p>Eliminare un modello ottimizzato</p><p>Inserisci o mappa l’ID del modello da eliminare.</p>
 </ul> 
  </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL ID file]</td> 
   <td> Se si elimina un file o si recupera il relativo contenuto, immettere o mappare l'ID del file. 
  </tr> 
</tbody>

