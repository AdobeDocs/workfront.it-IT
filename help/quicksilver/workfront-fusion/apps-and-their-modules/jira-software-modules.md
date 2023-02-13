---
title: Moduli software Jira
description: In un [!DNL Adobe Workfront Fusion] puoi automatizzare i flussi di lavoro che utilizzano [!DNL Jira] Software e collegarlo a più applicazioni e servizi di terze parti.
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 6437fe98-2c2b-4b49-97e2-f94b23da93fd
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2039'
ht-degree: 1%

---

# [!DNL Jira Software] moduli

In un [!DNL Adobe Workfront Fusion] puoi automatizzare i flussi di lavoro che utilizzano [!DNL Jira Software], nonché collegarlo a più applicazioni e servizi di terze parti.

Se hai bisogno di istruzioni su come creare uno scenario, vedi [Crea uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Per informazioni sui moduli, consulta [Moduli in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

<!-- Bob Fix this compared to original -->

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
   <td> <p>[!UICONTROL Workfront Fusion for Work Automation and Integration] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</td> 
  </tr> 
 </tbody> 
</table>

Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, vedi [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Prerequisiti

Per utilizzare [!DNL Jira] moduli è necessario disporre di un [!DNL Jira] conto.

## Connetti [!DNL Jira Software] a [!DNL Workfront Fusion]

Il metodo di connessione si basa sull&#39;utilizzo o meno di [!DNL Jira Cloud] o [!DNL Jira Server].

* [Connetti [!DNL Jira Cloud] a Workfront Fusion](#connect-jira-cloud-to-workfront-fusion)
* [Connetti [!DNL Jira Server] a [!DNL Workfront Fusion]](#connect-jira-server-to-workfront-fusion)

### Connetti [!DNL Jira Cloud] a [!DNL Workfront Fusion]

Connetti [!DNL Jira Cloud] a [!DNL Workfront Fusion]

Connessione [!DNL Jira Software] a [!DNL Workfront Fusion], devi creare un token API e inserirlo insieme all’URL del servizio e al nome utente nel [!UICONTROL Creare una connessione] campo [!DNL Workfront Fusion].

#### Crea un token API in [!DNL Jira]

1. Vai a [https://id.atlassian.com/manage/api-tokens](https://id.atlassian.com/manage/api-tokens) e accedi.
1. Fai clic su **[!UICONTROL Crea token API]**.
1. Digita un nome per il token, ad esempio *Workfront Fusion*.
1. Copia il token utilizzando **[!UICONTROL Copia negli Appunti]** pulsante .

   >[!IMPORTANT]
   >
   >Dopo la chiusura di questa finestra di dialogo, non puoi visualizzare nuovamente il token.
1. Memorizza il token generato in un luogo sicuro.
1. Continua con [Configura le [!DNL Jira] Token API in [!DNL Workfront Fusion]](#configure-the-jira-api-token-in-workfront-fusion).

#### Configura le [!DNL Jira] Token API in [!DNL Workfront Fusion]

1. In [!DNL Workfront Fusion], aggiungi un [!DNL Jira] in uno scenario per aprire **[!UICONTROL Creare una connessione]** scatola.
1. Specifica le seguenti informazioni:

   * **[!UICONTROL URL servizio]**
   * **[!UICONTROL Username]**
   * **[!UICONTROL Token API]:** Questo è il token API creato in [Crea un token API in [!DNL Jira]](#create-an-api-token-in-jira) sezione di questo articolo.

1. Fai clic su [!UICONTROL Continua] per creare la connessione e tornare al modulo .

### Connetti [!DNL Jira Server] a [!DNL Workfront Fusion]

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Becky: Find out and document how to find these things</p>
-->

Per autorizzare una connessione tra [!DNL Workfront Fusion] e [!DNL Jira Server], devi disporre della tua chiave consumer, della chiave privata e dell’URL del servizio. Potrebbe essere necessario contattare il tuo [!DNL Jira] amministratore per queste informazioni.

* [Genera chiavi pubbliche e private per la tua [!DNL Jira] connection](#generate-public-and-private-keys-for-your-jira-connection)
* [Configura l’app client come consumer in [!DNL Jira]](#configure-the-client-app-as-a-consumer-in-jira)
* [Creare una connessione a [!DNL Jira] Centro dati server o Jira in [!DNL Workfront Fusion]](#create-a-connection-to-jira-server-or-jira-data-center-in-workfront-fusion)

#### Genera chiavi pubbliche e private per la tua [!DNL Jira] connection

Per acquisire una chiave privata per la [!DNL Workfront Fusion Jira] connessione, è necessario generare chiavi pubbliche e private.

1. Nel terminale, esegui quanto segue `openssl` comandi.

   * `openssl genrsa -out jira_privatekey.pem 1024`

      Questo comando genera una chiave privata a 1024 bit.

   * `openssl req -newkey rsa:1024 -x509 -key jira_privatekey.pem -out jira_publickey.cer -days 365`

      Questo comando crea un certificato X509.

   * `openssl pkcs8 -topk8 -nocrypt -in jira_privatekey.pem -out jira_privatekey.pcks8`

      Questo comando estrae la chiave privata (formato PKCS8) `jira_privatekey.pcks8`
file.

   * `openssl x509 -pubkey -noout -in jira_publickey.cer  > jira_publickey.pem`

      Questo comando estrae la chiave pubblica dal certificato al `jira_publickey.pem` file.

      >[!NOTE]
      >
      >Se si utilizza Windows, potrebbe essere necessario salvare la chiave pubblica nel `jira_publickey.pem` file manualmente:
      >
      >1. Nel terminale, esegui il seguente comando:
      >   
      >   `openssl x509 -pubkey -noout -in jira_publickey.cer`
      >   
      >1. Copia l&#39;uscita del terminale (incluso `-------BEGIN PUBLIC KEY--------` e `-------END PUBLIC KEY--------`
      >   
      >1. Incolla l’output del terminale in un file denominato `jira_publickey.pem`.



1. Continua a [Configura l’app client come consumer in [!DNL Jira]](#configure-the-client-app-as-a-consumer-in-jira)

#### Configura l’app client come consumer in [!DNL Jira]

1. Accedi al tuo [!DNL Jira] istanza.
1. Nel pannello di navigazione a sinistra, fai clic su **[!UICONTROL [!DNL Jira]Impostazioni]** ![](assets/jira-settings-icon.png) > **[!UICONTROL Applicazioni]**> **[!UICONTROL Collegamenti alle applicazioni]**.
1. In **[!UICONTROL Immettere l&#39;URL dell&#39;applicazione da collegare]** campo, immettere

   ```
   https://app.workfrontfusion.com/oauth/cb/workfront-jiraserver-oauth1
   ```

1. Fai clic su **[!UICONTROL Crea nuovo collegamento]**. Ignora il messaggio di errore &quot;Nessuna risposta ricevuta dall&#39;URL inserito&quot;.
1. In **[!UICONTROL Applicazioni di collegamento]** immetti valori nella finestra **[!UICONTROL Chiave del consumatore]** e **[!UICONTROL Segreto condiviso]** campi.

   È possibile scegliere i valori per questi campi.

1. Copia i valori del **[!UICONTROL Chiave del consumatore]** e **[!UICONTROL Segreto condiviso]** campi in una posizione sicura.

   Questi valori saranno necessari successivamente nel processo di configurazione.

1. Compila i campi URL come segue:

   | Campo | Descrizione |
   |---|---|
   | [!UICONTROL URL token di richiesta] | `<Jira base url>/plugins/servlet/oauth/request-token` |
   | [!UICONTROL URL autorizzazione] | `<Jira base url>/plugins/servlet/oauth/authorize` |
   | [!UICONTROL URL token di accesso] | `<Jira base url>/plugins/servlet/oauth/access-token` |

1. Seleziona la **[!UICONTROL Crea collegamento in entrata]** casella di controllo.
1. Fai clic su **[!UICONTROL Continua]**.
1. In **[!UICONTROL Applicazioni di collegamento]** , compila i campi seguenti:

   <table style="table-layout:auto"> 
    <col data-mc-conditions=""> 
    <col data-mc-conditions=""> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Consumer Key]</p> </td> 
      <td> Incolla la chiave del consumatore copiata in un percorso protetto.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome consumatore]</td> 
      <td>Inserisci un nome a tua scelta. Questo nome è per il tuo riferimento.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Chiave pubblica]</td> 
      <td>Incolla la chiave pubblica dalla <code>[!DNL jira_publickey.pem]</code> file.</td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **[!UICONTROL Continua]**.
1. Continua a [Creare una connessione a [!DNL Jira Server] o [!DNL Jira Data Center] in [!DNL Workfront Fusion]](#create-a-connection-to-jira-server-or-jira-data-center-in-workfront-fusion)

#### Creare una connessione a [!DNL Jira Server] o [!DNL Jira Data Center] in [!DNL Workfront Fusion]

>[!NOTE]
>
>Utilizza la [!DNL Jira Server] app a cui connettersi [!DNL Jira Server] o [!DNL Jira Data Center].
1. In qualsiasi [!DNL Jira Server] modulo in [!DNL Workfront Fusion], fai clic su **[!UICONTROL Aggiungi]** accanto al [!UICONTROL connection] campo .
1. In [!UICONTROL Creare una connessione] , compila i campi seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Nome connessione]</p> </td> 
      <td> <p>Immettere un nome per la connessione</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Consumer Key]</td> 
      <td>Incolla la chiave del consumatore copiata in un percorso protetto in <a href="#configure-the-client-app-as-a-consumer-in-jira" class="MCXref xref">Configura l’app client come consumer in [!DNL Jira]</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Private Key]</td> 
      <td>Incolla nella chiave privata dal <code>[!DNL jira_privatekey.pcks8]</code> file creato in <a href="#generate-public-and-private-keys-for-your-jira-connection" class="MCXref xref">Genera chiavi pubbliche e private per la tua [!DNL Jira] connection</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Service URL]</td> 
      <td>Inserisci il tuo [!DNL Jira] URL dell'istanza. </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **[!UICONTROL Continua]** per creare la connessione e tornare al modulo .

## [!DNL Jira Software] moduli e relativi campi

Quando si configura [!DNL Jira Software] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL Jira Software] potrebbero essere visualizzati, a seconda di fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se trovi il pulsante mappa sopra un campo o una funzione, puoi utilizzarlo per impostare variabili e funzioni per quel campo. Per ulteriori informazioni, consulta [Mappare informazioni da un modulo a un altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Azioni](#actions)
* [Ricerche](#searches)

### Triggers

#### [!UICONTROL Controlla i record]

Questo modulo di attivazione avvia uno scenario in cui un record viene aggiunto, aggiornato o eliminato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>Selezionare il webhook che si desidera utilizzare per controllare i record. </p> <p>Per aggiungere un nuovo webhook:</p> 
    <ol> 
     <li value="1">Fai clic su <strong>[!UICONTROL Aggiungi]</strong></li> 
     <li value="2">Immettere un nome per il webhook.</li> 
     <li value="3"> <p>Selezionare la connessione che si desidera utilizzare per il webhook. </p> <p>Per istruzioni su come collegare le [!DNL Jira Software] account a [!DNL Workfront Fusion], vedi <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connetti [!DNL Jira Software] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </li> 
     <li value="4"> <p>Selezionare il tipo di record per il quale si desidera che il software controlli:</p> 
      <ul> 
       <li>[!UICONTROL Commento] </li> 
       <li>[!UICONTROL Problema]</li> 
       <li>[!UICONTROL Project] </li> 
       <li>[!UICONTROL Sprint]</li> 
      </ul> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### Azioni

* [[!UICONTROL Aggiungi il problema allo sprint]](#add-issue-to-sprint)
* [[!UICONTROL Chiamata API personalizzata]](#custom-api-call)
* [[!UICONTROL Creare un record]](#create-a-record)
* [[!UICONTROL Eliminare un record]](#delete-a-record)
* [[!UICONTROL Scaricare un allegato]](#download-an-attachment)
* [[!UICONTROL Leggi un record]](#read-a-record)
* [[!UICONTROL Aggiornare un record]](#update-a-record)

#### [!UICONTROL Aggiungi il problema allo sprint]

Questo modulo di azione aggiunge uno o più problemi a uno sprint.

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Jira Software] account a [!DNL Workfront Fusion], vedi <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connetti [!DNL Jira Software] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sprint ID]</td> 
   <td>Immetti o mappa l’ID di stampa dello sprint a cui desideri aggiungere un problema.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID o chiavi del problema [!UICONTROL]</td> 
   <td>Aggiungi un ID o una chiave del problema da aggiungere allo sprint.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Creare un record]

Questo modulo di azione crea un nuovo record in Jira.

Il modulo restituisce tutti i campi standard associati al record, insieme a eventuali campi e valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Jira Software] account a [!DNL Workfront Fusion], vedi <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connetti [!DNL Jira Software] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td> <p>Selezionare il tipo di record che si desidera creare nel modulo. Quando selezioni un tipo di record, nel modulo vengono visualizzati altri campi specifici per tale tipo di record.</p> 
    <ul> 
     <li>Allegato [!UICONTROL]</li> 
     <li>[!UICONTROL Commento]</li> 
     <li>[!UICONTROL Problema]</li> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Sprint] </li> 
     <li>[!UICONTROL Worklog]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Chiamata API personalizzata]

Questo modulo di azione ti consente di effettuare una chiamata autenticata personalizzata al [!DNL Jira Software] API. In questo modo, puoi creare un’automazione del flusso di dati che non può essere eseguita dall’altro [!DNL Jira Software] moduli.

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Jira Software] account a [!DNL Workfront Fusion], vedi <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connetti [!DNL Jira Software] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Immettere un percorso relativo a<code>&lt;Instance URL>/rest/api/2/ </code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL, Metodo]</td> 
   td&gt; <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Aggiungi le intestazioni della richiesta sotto forma di un oggetto JSON standard.</p> <p>Ad esempio: <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] aggiunge le intestazioni di autorizzazione per te.</p> </td> 
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

#### [!UICONTROL Eliminare un record]

Questo modulo di azione elimina un record specifico.

Specifica l&#39;ID del record.

Il modulo restituisce l’ID del record e di tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Jira Software] account a [!DNL Workfront Fusion], vedi <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connetti [!DNL Jira Software] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td> <p>Selezionare il tipo di record che si desidera eliminare dal modulo. </p> 
    <ul> 
     <li>Allegato [!UICONTROL]</li> 
     <li>[!UICONTROL Commento]</li> 
     <li>[!UICONTROL Problema]</li> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Sprint] </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID o chiave]</td> 
   <td>Immettere o mappare l'ID o la chiave del record che si desidera eliminare.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Scaricare un allegato]

Questo modulo di azione scarica un allegato specifico.

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Jira Software] account a [!DNL Workfront Fusion], vedi <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connetti [!DNL Jira Software] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Immettere o mappare l'ID dell'allegato che si desidera scaricare.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Leggi un record]

Questo modulo di azione legge i dati da un singolo record in [!DNL Jira Software].

Specifica l&#39;ID del record.

Il modulo restituisce tutti i campi standard associati al record, insieme a eventuali campi e valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Jira Software] account a [!DNL Workfront Fusion], vedi <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connetti [!DNL Jira Software] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td> <p>Seleziona il tipo di [!DNL Jira] record che si desidera leggere nel modulo.</p> 
    <ul> 
     <li>Allegato [!UICONTROL]</li> 
     <li>[!UICONTROL Problema]</li> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Sprint] </li> 
     <li>[!UICONTROL Utente]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Uscite]</td> 
   <td>Seleziona gli output da ricevere. Le opzioni di output sono disponibili in base al tipo di record selezionato nel campo "[!UICONTROL Record Type]".</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td> <p>Immetti o mappa l'univoco [!DNL Jira Software] ID del record che si desidera leggere nel modulo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggiornare un record]

Questo modulo di azione aggiorna un record esistente, ad esempio un problema o un progetto.

Specifica l&#39;ID del record.

Il modulo restituisce l’ID del record e di tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Jira Software] account a [!DNL Workfront Fusion], vedi <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connetti [!DNL Jira Software] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td> <p>Selezionare il tipo di record che si desidera aggiornare nel modulo. Quando selezioni un tipo di record, nel modulo vengono visualizzati altri campi specifici per tale tipo di record.</p> 
    <ul> 
     <li>[!UICONTROL Commento]</li> 
     <li>[!UICONTROL Problema]</li> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Sprint] </li> 
     <li>[!UICONTROL Problema di transizione]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID o chiave]</td> 
   <td>Immettere o mappare l'ID o la chiave del record che si desidera aggiornare.</td> 
  </tr> 
 </tbody> 
</table>

### Ricerche

* [[!UICONTROL Elencare record]](#list-records)
* [[!UICONTROL Cerca record]](#search-for-records)

#### [!UICONTROL Elencare record]

Questo modulo di ricerca recupera tutti gli elementi di un tipo specifico che corrispondono alla query di ricerca

Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Jira Software] account a [!DNL Workfront Fusion], vedi <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connetti [!DNL Jira Software] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td> <p>Selezionare il tipo di record da elencare nel modulo. Quando selezioni un tipo di record, nel modulo vengono visualizzati altri campi specifici per tale tipo di record.</p> 
    <ul> 
     <li>[!UICONTROL Commento]</li> 
     <li>[!UICONTROL Problema]</li> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Problema di stampa]</li> 
     <li>[!UICONTROL Worklog]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Max Results]</p> </td> 
   <td> <p>Immettere o mappare il numero massimo di record che si desidera recuperare dal modulo durante ogni ciclo di esecuzione degli scenari.</p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Offset</td> 
    <td> Enter or map the ID of the first item you want to retrieve details for. This is a way to paginate the records. If you enter the 5000th item as the offset, the module would return items 5000-9999.</td> 
   </tr>
  --> 
 </tbody> 
</table>

#### [!UICONTROL Cerca record]

Questo modulo di ricerca cerca i record in un oggetto in [!DNL Jira Software] che corrispondono alla query di ricerca specificata.

Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Jira Software] account a [!DNL Workfront Fusion], vedi <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connetti [!DNL Jira Software] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td> <p>Selezionare il tipo di record che si desidera cercare nel modulo. Quando selezioni un tipo di record, nel modulo vengono visualizzati altri campi specifici per tale tipo di record.</p> 
    <ul> 
     <li>[!UICONTROL Issues]</li> 
     <li> <p>[!UICONTROL Issues by JQL (Jira Query Language)] </p> <p>Per ulteriori informazioni su JQL, vedi <a href="https://www.atlassian.com/blog/jira-software/jql-the-most-flexible-way-to-search-jira-14#:~:text=JQLstandsforJiraQuery,projectmanagers%2Candbusinessusers.">JQL</a> presso il sito di aiuto Atlassian. </p> </li> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Progetto per problema]</li> 
     <li>[!UICONTROL Utente]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
