---
title: Moduli DocuSign
description: La [!DNL Adobe Workfront Fusion DocuSign] i moduli consentono di monitorare e recuperare lo stato dell'inviluppo, cercare e recuperare le buste o scaricare e inviare un documento per accedere [!DNL DocuSign] conto.
author: Becky
draft: Probably
feature: Workfront Fusion, Digital Content and Documents
exl-id: a6ebfe6f-dc3f-41f7-8129-bbc5775cff33
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1911'
ht-degree: 0%

---

# Moduli DocuSign

La [!DNL Adobe Workfront Fusion] [!DNL DocuSign] i moduli consentono di monitorare e recuperare lo stato dell&#39;inviluppo, cercare e recuperare le buste o scaricare e inviare un documento per accedere [!DNL DocuSign] conto.

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

Per utilizzare [!DNL DocuSign] moduli, è necessario disporre di un [!DNL DocuSign] conto.

## Connetti [!DNL DocuSign] a [!DNL Workfront Fusion] {#connect-docusign-to-workfront-fusion}

Per creare una connessione per [!DNL DocuSign] moduli:

1. Fai clic su **[!UICONTROL Aggiungi]** accanto al [!UICONTROL Connessione] quando si inizia a configurare il primo [!DNL DocuSign] modulo .
1. Immetti quanto segue:

<table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Nome connessione]</p> </td> 
      <td>Immettere un nome per il nuovo [!DNL DocuSign] connection</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tipo di account]</td> 
      <td>Seleziona se l'account a cui desideri connetterti è un account di produzione o demo.</td> 
     </tr> 
    </tbody> 
   </table>

1. Continua come descritto in [Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base](../../workfront-fusion/connections/connect-to-fusion-general.md#connect).

## [!DNL DocuSign] moduli e relativi campi

Quando si configura [!DNL DocuSign] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL DocuSign] potrebbero essere visualizzati, a seconda di fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se trovi il pulsante mappa sopra un campo o una funzione, puoi utilizzarlo per impostare variabili e funzioni per quel campo. Per ulteriori informazioni, consulta [Mappare informazioni da un modulo a un altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Azioni](#actions)

### Triggers

#### [!UICONTROL Buste di controllo]

Questo modulo di attivazione avvia uno scenario in cui una busta viene inviata, consegnata, firmata, completata o rifiutata.

<table style="table-layout:auto">
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL DocuSign] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Collega l’app o il servizio Web del modulo a [!DNL Workfront Fusion]</a> nell'articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crea uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Account] </td> 
   <td> <p>Selezionare l'account contenente i record che si desidera controllare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo evento]</td> 
   <td> <p> Seleziona il tipo di evento da visualizzare.</p> 
    <ul> 
     <li>[!UICONTROL Documento completato]</li> 
     <li>[!UICONTROL Documento rifiutato]</li> 
     <li>[!UICONTROL Documento inviato]</li> 
     <li>[!UICONTROL Documento firmato]</li> 
     <li>[!UICONTROL Nuovo documento in Posta in arrivo]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Campi di output]</p> </td> 
   <td> <p>Selezionare i campi che si desidera includere nell'output del modulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Immettere o mappare il numero massimo di record con cui si desidera che il modulo funzioni durante ogni ciclo di esecuzione degli scenari.</td> 
  </tr> 
 </tbody> 
</table>

### Azioni

* [[!UICONTROL Chiamata API personalizzata]](#custom-api-call)
* [[!UICONTROL Scaricare un documento]](#download-a-document)
* [[!UICONTROL Leggi una busta]](#read-an-envelope)
* [[!UICONTROL Caricare un file in un inviluppo]](#upload-a-file-to-an-envelope)
* [[!UICONTROL Crea una nuova busta]](#create-a-new-envelope)
* [[!UICONTROL Aggiungi destinatario a busta]](#add-recipient-to-envelope)
* [[!UICONTROL Aggiungi campo personalizzato]](#add-custom-field)
* [[!UICONTROL Modifica campo personalizzato]](#modify-custom-field)
* [[!UICONTROL Invia busta]](#send-envelope)

#### [!UICONTROL Chiamata API personalizzata]

Questo modulo di azione ti consente di eseguire una chiamata API personalizzata.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL DocuSign] account a [!DNL Workfront Fusion], vedi <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connetti [!DNL DocuSign] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Account]</td> 
   <td>Immettere o mappare l'account che si desidera utilizzare per accedere al [!DNL DocuSign] API.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL URL]</td> 
   <td> <p>Digita l’indirizzo sul server web con cui desideri interagire il modulo.</p> <p>Puoi digitare un URL relativo, il che significa che non devi includere il protocollo (ad esempio <code>http://</code>) all'inizio. Questo suggerisce al server web di verificare che l'interazione si verifichi sul server.</p> <p>Ad esempio: <code>[!DNL /api/conversations].create</code></p> <p>Suggerimento: Per un elenco degli endpoint disponibili, consulta <a href="https://developers.docusign.com/esign-rest-api/reference">[!DNL DocuSign] Riferimento API</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL, Metodo]</td> 
   td&gt; <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Headers]</td> 
   <td> <p>Aggiungi le intestazioni della richiesta sotto forma di un oggetto JSON standard. Questo determina il tipo di contenuto della richiesta.</p> <p>Ad esempio:<code> {"Content-type":"application/json"}</code></p> <p>Nota: Se ricevi errori ed è difficile determinarne l’origine, considera la possibilità di modificare le intestazioni in base al [!DNL Workfront] documentazione. Se la chiamata API personalizzata restituisce un errore di richiesta HTTP 422, prova a utilizzare un’intestazione "Content-Type":"text/plain".</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Query String]</td> 
   <td> <p>Aggiungi la query per la chiamata API sotto forma di un oggetto JSON standard.</p> <p>Ad esempio: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Body]</td> 
   <td> <p>Aggiungi il contenuto del corpo per la chiamata API sotto forma di un oggetto JSON standard.</p> <p>Nota:  <p>Quando si utilizzano istruzioni condizionali come <code>if</code> nel JSON, inserisci le virgolette al di fuori dell’istruzione condizionale.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td>Immettere o mappare il numero massimo di risultati con cui lavorare durante un ciclo di esecuzione.</td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Esempio:** Buste elenco
>
>La seguente chiamata API restituisce buste dalla data specificata nel [!DNL DocuSign] account:
>
>**URL**: `/v2.1/accounts/{accountId}/envelopes/`
>
>**Metodo**: `GET`
>
>**Stringa query**:
>
>* **Chiave**: `from_date`
>
>* **Valore**: `YYYY-MM-DD`
>
>Specifica quando la richiesta inizia a verificare la presenza di modifiche di stato per le buste nell&#39;account.
>
>![](assets/example-docusign-setup-350x770.png)
>
>Il risultato si trova in Output del modulo in Bundle > Corpo > buste.
>
>Nel nostro esempio, sono state restituite 6 buste:
>
>![](assets/docusign-example-output-350x677.png)

#### [!UICONTROL Scaricare un documento]

Questo modulo di azione scarica un singolo documento.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL DocuSign] account a [!DNL Workfront Fusion], vedi <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connetti [!DNL DocuSign] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Account] </td> 
   <td> <p>Selezionare l'account contenente il documento da scaricare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID Busta</td> 
   <td> <p> Immetti o mappa l’ID della busta da scaricare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Document ID]</p> </td> 
   <td> <p>Immettere o mappare l'ID del documento che si desidera scaricare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Certificate]</td> 
   <td>Seleziona <strong>[!UICONTROL Sì]</strong> per includere il certificato di firma della busta nel download.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Documenti per ID utente]</td> 
   <td>Seleziona <strong>[!UICONTROL Sì]</strong> se desideri consentire ai destinatari di recuperare i documenti per ID utente. Ad esempio, se un utente è incluso in due ordini di indirizzamento diversi con diverse visibilità, l'utilizzo di questa opzione restituisce tutti i documenti di entrambi i cicli.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encrypt]</td> 
   <td>Seleziona <strong>[!UICONTROL Sì]</strong> se desideri che i byte di PDF restituiti nella risposta siano crittografati per tutti i key manager configurati sul tuo [!DNL DocuSign] conto.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Language]</td> 
   <td>Seleziona la lingua.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mostra modifiche]</td> 
   <td>Quando è impostato su <strong>[!UICONTROL Sì]</strong>, tutti i campi modificati per il PDF restituito sono evidenziati in giallo e le firme o le iniziali facoltative sono evidenziate in rosso.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watermark]</td> 
   <td> <p>Seleziona <strong>[!UICONTROL No]</strong> per rimuovere la filigrana dai documenti PDF.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Leggi una busta]

Questo modulo di azione legge informazioni su un&#39;inviluppo in [!DNL DocuSign] utilizzando l&#39;ID busta.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL DocuSign] account a [!DNL Workfront Fusion], vedi <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connetti [!DNL DocuSign] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Account] </td> 
   <td> <p>Selezionare l'account contenente il documento da cui si desidera leggere le informazioni.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID Busta</td> 
   <td> <p> Immettere o mappare l'ID contenente il documento da cui si desidera leggere le informazioni.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Uscite]</td> 
   <td>Selezionare le proprietà che si desidera visualizzare nell'output del modulo. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Caricare un file in un inviluppo]

Questo modulo carica un file specificato in un inviluppo esistente in DocuSign.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL DocuSign] account a [!DNL Workfront Fusion], vedi <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connetti [!DNL DocuSign] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Account] </td> 
   <td> <p>Seleziona l’account che contiene la busta in cui desideri caricare un file.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID Busta</td> 
   <td> <p> Immetti o mappa l’ID della busta in cui desideri caricare un file.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File di origine]</td> 
   <td>Selezionare un file di origine da un modulo precedente oppure immettere il nome e i dati del file di origine.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crea una nuova busta]

Questo modulo di azione crea una nuova busta da un modello. Restituisce l’ID della nuova busta e lo stato della nuova busta.

<table style="table-layout:auto">
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td>

<td> <p>Per istruzioni su come collegare il tuo account DocuSign a Workfront Fusion, vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Collegare l'app o il servizio Web del modulo a Workfront Fusion</a> nell'articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Creare uno scenario in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Account] </td>
   <td> <p>Seleziona l’account che contiene la busta in cui desideri caricare un file.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Template]</td>
   <td> <p> Selezionare il modello da cui si desidera creare la nuova busta. I modelli sono disponibili in base all’ [!UICONTROL Account] selezionato.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">
     [!UICONTROL Dopo la creazione]
   </td> 
   <td> <p>Selezionare se salvare la busta come bozza o inviarla per la firma.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Destinatari del modello]</td>
    <td>Selezionare il destinatario della busta</td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggiungi destinatario a busta]

Questo modulo di azione aggiunge uno o più destinatari a una busta esistente. Se la busta è già stata inviata, al destinatario viene inviato un messaggio e-mail. Questo modulo non è valido per le buste già completate.

<table style="table-layout:auto">
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr data-mc-conditions=""> 
    <td>[!UICONTROL Connection] </td>
   <td> <p>Per istruzioni su come collegare il tuo account DocuSign a Workfront Fusion, vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Collegare l'app o il servizio Web del modulo a Workfront Fusion</a> nell'articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Creare uno scenario in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="">
    <td>[!UICONTROL Account] </td>
   <td> <p>Seleziona l’account che contiene la busta in cui desideri aggiungere i destinatari.</p> </td> 
  </tr> 
  <tr> 
    <td>ID Busta</td>
    <td>Seleziona o mappa l’ID della busta in cui desideri aggiungere il destinatario.</td>
  </tr> 
  <tr data-mc-conditions="">
    <td role="rowheader">[!UICONTROL Tipo di destinatario]</td>
   <td> <p> Selezionare il tipo di destinatario che si desidera aggiungere all'inviluppo.</p> 
    <ul> 
     <li> <p>[!UICONTROL Agent]</p> </li> 
     <li> <p>[!UICONTROL Carbon copy]</p> </li> 
     <li> <p>[!UICONTROL Certified delivery]</p> </li> 
     <li> <p>[!UICONTROL Firmatario di persona]</p> </li> 
     <li> <p>[!UICONTROL Intermediario]</p> </li> 
     <li> <p>[!UICONTROL Signer]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td>E-MAIL [!UICONTROL]</td>
   <td> <p>Inserisci o mappa l’indirizzo e-mail del destinatario che desideri aggiungere alla busta.</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Name]</td>
   <td>Immettere o mappare il nome del destinatario che si desidera aggiungere alla busta.</td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Ordine di routing]</td>
   <td> <p>Immettere o mappare il numero di indirizzamento del destinatario. Il numero di indirizzamento determina l’ordine in cui i destinatari ricevono e firmano i documenti.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL E-mail body]</td>
   <td>Inserisci o mappa il corpo (contenuto) dell’e-mail che viene inviato al destinatario.</td> 
  </tr> 
  <tr>
    <td role="rowheader">[!UICONTROL Oggetto e-mail]</td>
   <td>Immetti o mappa l’oggetto dell’e-mail inviata al destinatario.</td> 
  </tr> 
    <td role="rowheader">[!UICONTROL Messaggio privato]</td>
   <td> <li> <p>Solo il destinatario selezionato vede il messaggio privato e il messaggio generale. Il messaggio privato è limitato a 1000 caratteri.</p> </li> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Authentication]</td> 
   <td> <p>Seleziona il metodo di autenticazione da utilizzare per confermare l’identità del destinatario.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nessuno]</strong> </p> </li> 
     <li> <p><strong>[!UICONTROL Codice di accesso]</strong> </p> <p>Immetti o mappa il codice di accesso.</p> </li> 
     <li> <p><strong>[!UICONTROL Phone]</strong> </p> <p>Immettere o mappare il numero di telefono</p> </li> 
     <li> <p><strong>[!UICONTROL SMS]</strong> </p> <p>Immettere o mappare il numero di telefono</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggiungi campo personalizzato]

Questo modulo di azione aggiunge un campo personalizzato al documento

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL DocuSign] account a [!DNL Workfront Fusion], vedi <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connetti [!DNL DocuSign] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Account] </td> 
   <td> <p>Selezionare l'account contenente il documento in cui si desidera aggiungere un campo personalizzato.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID Busta</td> 
   <td> <p> Immettere o mappare l'ID della busta contenente il documento in cui si desidera aggiungere un campo personalizzato.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome campo]</td> 
   <td>Immettere o mappare un nome per il nuovo campo che si desidera aggiungere.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Obbligatorio]</td> 
   <td>Abilita questa opzione se desideri che il campo aggiunto sia un campo obbligatorio.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mostra campo]</td> 
   <td>Abilita questa opzione se desideri che il campo sia visibile.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Value]</td> 
   <td>Immetti o mappa il valore (contenuto) del campo aggiunto. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Modifica campo personalizzato]

Questo modulo di azione modifica un campo personalizzato utilizzando il nome del campo.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL DocuSign] account a [!DNL Workfront Fusion], vedi <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connetti [!DNL DocuSign] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Account] </td> 
   <td> <p>Selezionare l'account contenente il documento in cui si desidera modificare un campo personalizzato.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID Busta</td> 
   <td> <p> Immettere o mappare l'ID della busta contenente il documento in cui si desidera modificare un campo personalizzato.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Field ID]</td> 
   <td>Immetti o mappa l’ID del campo da modificare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome campo]</td> 
   <td>Immettere o mappare il nome del campo che si desidera modificare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Obbligatorio]</td> 
   <td>Abilita questa opzione se desideri che il campo modificato sia un campo obbligatorio.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mostra campo]</td> 
   <td>Abilita questa opzione se desideri che il campo sia visibile.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Value]</td> 
   <td>Immetti o mappa il valore (contenuto) del campo modificato. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Invia busta]

Questo modulo di azione invia una bozza di busta ai relativi destinatari.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL DocuSign] account a [!DNL Workfront Fusion], vedi <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connetti [!DNL DocuSign] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Account] </td> 
   <td> <p>Seleziona l’account che contiene la bozza di busta da inviare ai relativi destinatari.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID Busta</td> 
   <td> <p> Immetti o mappa l'ID della bozza di busta che desideri inviare ai relativi destinatari.</p> </td> 
  </tr> 
 </tbody> 
</table>
