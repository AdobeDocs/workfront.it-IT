---
title: Moduli software Jira
description: In un [!DNL Adobe Workfront Fusion] scenario, puoi automatizzare i flussi di lavoro che utilizzano [!DNL Jira] e collegarlo a più applicazioni e servizi di terze parti.
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 6437fe98-2c2b-4b49-97e2-f94b23da93fd
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '2085'
ht-degree: 1%

---

# [!DNL Jira Software] moduli

In un [!DNL Adobe Workfront Fusion] scenario, puoi automatizzare i flussi di lavoro che utilizzano [!DNL Jira Software], oltre a collegarlo a più applicazioni e servizi di terze parti.

Per istruzioni sulla creazione di uno scenario, consulta [Creare uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

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

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, consulta [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Prerequisiti

Da utilizzare [!DNL Jira] moduli è necessario disporre di [!DNL Jira] account.

## Connetti [!DNL Jira Software] a [!DNL Workfront Fusion]

Il metodo di connessione si basa sull&#39;utilizzo o meno di [!DNL Jira Cloud] o [!DNL Jira Server].

* [Connetti [!DNL Jira Cloud] a Workfront Fusion](#connect-jira-cloud-to-workfront-fusion)
* [Connetti [!DNL Jira Server] a [!DNL Workfront Fusion]](#connect-jira-server-to-workfront-fusion)

### Connetti [!DNL Jira Cloud] a [!DNL Workfront Fusion]

Connetti [!DNL Jira Cloud] a [!DNL Workfront Fusion]

Per connettersi [!DNL Jira Software] a [!DNL Workfront Fusion], devi creare un token API e inserirlo insieme all’URL del servizio e al nome utente nella [!UICONTROL Creare una connessione] campo in [!DNL Workfront Fusion].

#### Creare un token API in [!DNL Jira]

1. Vai a [https://id.atlassian.com/manage/api-tokens](https://id.atlassian.com/manage/api-tokens) e accedi.
1. Clic **[!UICONTROL Crea token API]**.
1. Digita un nome per il token, ad esempio *Workfront Fusion*.
1. Copia il token utilizzando **[!UICONTROL Copia negli Appunti]** pulsante.

   >[!IMPORTANT]
   >
   >Impossibile visualizzare di nuovo il token dopo aver chiuso questa finestra di dialogo.
1. Memorizza il token generato in un luogo sicuro.
1. Continua con [Configurare [!DNL Jira] Token API in [!DNL Workfront Fusion]](#configure-the-jira-api-token-in-workfront-fusion).

#### Configurare [!DNL Jira] Token API in [!DNL Workfront Fusion]

1. In entrata [!DNL Workfront Fusion], aggiungi un [!DNL Jira] modulo a uno scenario per aprire **[!UICONTROL Creare una connessione]** casella.
1. Specifica le seguenti informazioni:

   * **[!UICONTROL URL servizio]**
   * **[!UICONTROL Username]**
   * **[!UICONTROL Token API]:** Questo è il token API creato in [Creare un token API in [!DNL Jira]](#create-an-api-token-in-jira) sezione di questo articolo.

1. Clic [!UICONTROL Continua] per creare la connessione e tornare al modulo.

### Connetti [!DNL Jira Server] a [!DNL Workfront Fusion]

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Becky: Find out and document how to find these things</p>
-->

Per autorizzare una connessione tra [!DNL Workfront Fusion] e [!DNL Jira Server], sono necessari la chiave consumer, la chiave privata e l’URL del servizio. Potrebbe essere necessario contattare il [!DNL Jira] per queste informazioni.

* [Genera chiavi pubbliche e private per il tuo [!DNL Jira] connessione](#generate-public-and-private-keys-for-your-jira-connection)
* [Configurare l’app client come consumatore in [!DNL Jira]](#configure-the-client-app-as-a-consumer-in-jira)
* [Creare una connessione a [!DNL Jira] Server o Jira Data Center in [!DNL Workfront Fusion]](#create-a-connection-to-jira-server-or-jira-data-center-in-workfront-fusion)

#### Genera chiavi pubbliche e private per il tuo [!DNL Jira] connessione

Per acquisire una chiave privata per il [!DNL Workfront Fusion Jira] connessione, devi generare chiavi pubbliche e private.

1. Nel terminale, eseguire le operazioni seguenti `openssl` comandi.

   * `openssl genrsa -out jira_privatekey.pem 1024`

     Questo comando genera una chiave privata a 1024 bit.

   * `openssl req -newkey rsa:1024 -x509 -key jira_privatekey.pem -out jira_publickey.cer -days 365`

     Questo comando crea un certificato X509.

   * `openssl pkcs8 -topk8 -nocrypt -in jira_privatekey.pem -out jira_privatekey.pcks8`

     Questo comando estrae la chiave privata (formato PKCS8) nel `jira_privatekey.pcks8`
file.

   * `openssl x509 -pubkey -noout -in jira_publickey.cer  > jira_publickey.pem`

     Questo comando estrae la chiave pubblica dal certificato al `jira_publickey.pem` file.

     >[!NOTE]
     >
     >Se utilizzi Windows, potrebbe essere necessario salvare la chiave pubblica nel `jira_publickey.pem` file manualmente:
     >
     >1. Nel terminale, eseguire il comando seguente:
     >   
     >   `openssl x509 -pubkey -noout -in jira_publickey.cer`
     >   
     >1. Copiare l&#39;uscita del terminale (compresa `-------BEGIN PUBLIC KEY--------` e `-------END PUBLIC KEY--------`
     >   
     >1. Incolla l’output del terminale in un file denominato `jira_publickey.pem`.


1. Continua con [Configurare l’app client come consumatore in [!DNL Jira]](#configure-the-client-app-as-a-consumer-in-jira)

#### Configurare l’app client come consumatore in [!DNL Jira]

1. Accedi al tuo [!DNL Jira] dell&#39;istanza.
1. Nel pannello di navigazione a sinistra, fai clic su **[!UICONTROL [!DNL Jira]Impostazioni]** ![](assets/jira-settings-icon.png) > **[!UICONTROL Applicazioni]**> **[!UICONTROL Collegamenti applicazione]**.
1. In **[!UICONTROL Immettere l&#39;URL dell&#39;applicazione da collegare]** campo, immetti

   ```
   https://app.workfrontfusion.com/oauth/cb/workfront-jiraserver-oauth1
   ```

1. Clic **[!UICONTROL Crea nuovo collegamento]**. Ignora il messaggio di errore &quot;Nessuna risposta ricevuta dall’URL immesso&quot;.
1. In **[!UICONTROL Collegare le applicazioni]** , immettere i valori nella finestra **[!UICONTROL Chiave consumer]** e **[!UICONTROL Segreto condiviso]** campi.

   È possibile scegliere i valori per questi campi.

1. Copia i valori di **[!UICONTROL Chiave consumer]** e **[!UICONTROL Segreto condiviso]** campi in una posizione sicura.

   Questi valori saranno necessari più avanti nel processo di configurazione.

1. Compila i campi URL come segue:

   | Campo | Descrizione |
   |---|---|
   | [!UICONTROL URL token di richiesta] | `<Jira base url>/plugins/servlet/oauth/request-token` |
   | [!UICONTROL URL autorizzazione] | `<Jira base url>/plugins/servlet/oauth/authorize` |
   | [!UICONTROL URL token di accesso] | `<Jira base url>/plugins/servlet/oauth/access-token` |

1. Seleziona la **[!UICONTROL Crea collegamento in ingresso]** casella di controllo.
1. Clic **[!UICONTROL Continua]**.
1. In **[!UICONTROL Collegare le applicazioni]** , compilare i campi seguenti:

   <table style="table-layout:auto"> 
    <col data-mc-conditions=""> 
    <col data-mc-conditions=""> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Chiave consumer]</p> </td> 
      <td> Incolla la chiave consumer copiata in un percorso sicuro.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome consumer]</td> 
      <td>Immettere un nome a scelta. Questo nome serve come riferimento.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Public Key]</td> 
      <td>Incolla la chiave pubblica dal tuo <code>[!DNL jira_publickey.pem]</code> file.</td> 
     </tr> 
    </tbody> 
   </table>

1. Clic **[!UICONTROL Continua]**.
1. Continua con [Creare una connessione a [!DNL Jira Server] o [!DNL Jira Data Center] in [!DNL Workfront Fusion]](#create-a-connection-to-jira-server-or-jira-data-center-in-workfront-fusion)

#### Creare una connessione a [!DNL Jira Server] o [!DNL Jira Data Center] in [!DNL Workfront Fusion]

>[!NOTE]
>
>Utilizza il [!DNL Jira Server] app a cui connettersi [!DNL Jira Server] o [!DNL Jira Data Center].
1. In qualsiasi [!DNL Jira Server] modulo in [!DNL Workfront Fusion], fai clic su **[!UICONTROL Aggiungi]** accanto al [!UICONTROL connessione] campo.
1. In [!UICONTROL Creare una connessione] , compilare i campi seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Nome connessione]</p> </td> 
      <td> <p>Immetti un nome per la connessione</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Chiave consumer]</td> 
      <td>Incolla la chiave del consumatore che hai copiato in una posizione sicura in <a href="#configure-the-client-app-as-a-consumer-in-jira" class="MCXref xref">Configurare l’app client come consumatore in [!DNL Jira]</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Private Key]</td> 
      <td>Incolla la chiave privata da <code>[!DNL jira_privatekey.pcks8]</code> file creato in <a href="#generate-public-and-private-keys-for-your-jira-connection" class="MCXref xref">Genera chiavi pubbliche e private per il tuo [!DNL Jira] connessione</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Service URL]</td> 
      <td>Immetti il [!DNL Jira] URL dell’istanza. </td> 
     </tr> 
    </tbody> 
   </table>

1. Clic **[!UICONTROL Continua]** per creare la connessione e tornare al modulo.

## [!DNL Jira Software] moduli e relativi campi

Quando si configura [!DNL Jira Software] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL Jira Software] I campi potrebbero essere visualizzati in base a fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se viene visualizzato il pulsante Mappa sopra un campo o una funzione, è possibile utilizzarlo per impostare variabili e funzioni per tale campo. Per ulteriori informazioni, consulta [Mappare le informazioni da un modulo all’altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Azioni](#actions)
* [Ricerche](#searches)

### Triggers

#### [!UICONTROL Controlla i record]

Questo modulo di attivazione avvia uno scenario quando viene aggiunto, aggiornato o eliminato un record.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>Selezionare il webhook che si desidera utilizzare per controllare i record. </p> <p>Per aggiungere un nuovo webhook:</p> 
    <ol> 
     <li value="1">Clic <strong>[!UICONTROL Add]</strong></li> 
     <li value="2">Immettere un nome per il webhook.</li> 
     <li value="3"> <p>Seleziona la connessione da utilizzare per il webhook. </p> <p>Per istruzioni sulla connessione [!DNL Jira Software] account a [!DNL Workfront Fusion], vedi <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connetti [!DNL Jira Software] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </li> 
     <li value="4"> <p>Selezionare il tipo di record che si desidera che venga controllato dal software:</p> 
      <ul> 
       <li>[!UICONTROL Comment] </li> 
       <li>[!UICONTROL Issue]</li> 
       <li>Progetto [!UICONTROL] </li> 
       <li>[!UICONTROL Sprint]</li> 
      </ul> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### Azioni

* [[!UICONTROL Aggiungi problema a sprint]](#add-issue-to-sprint)
* [[!UICONTROL Chiamata API personalizzata]](#custom-api-call)
* [[!UICONTROL Crea un record]](#create-a-record)
* [[!UICONTROL Eliminare un record]](#delete-a-record)
* [[!UICONTROL Scaricare un allegato]](#download-an-attachment)
* [[!UICONTROL Leggi un record]](#read-a-record)
* [[!UICONTROL Aggiornare un record]](#update-a-record)

#### [!UICONTROL Aggiungi problema a sprint]

Questo modulo di azione aggiunge uno o più problemi a uno sprint.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Jira Software] account a [!DNL Workfront Fusion], vedi <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connetti [!DNL Jira Software] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sprint ID]</td> 
   <td>Immetti o mappa l’ID Sprint dello sprint a cui desideri aggiungere un problema.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID problema o chiavi]</td> 
   <td>Aggiungi un ID problema o una chiave per ogni problema che desideri aggiungere allo sprint.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crea un record]

Questo modulo di azione crea un nuovo record in Jira.

Il modulo restituisce tutti i campi standard associati al record, insieme a tutti i campi e i valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Jira Software] account a [!DNL Workfront Fusion], vedi <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connetti [!DNL Jira Software] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td> <p>Selezionare il tipo di record che si desidera venga creato dal modulo. Quando si seleziona un tipo di record, nel modulo vengono visualizzati altri campi specifici per tale tipo di record.</p> 
    <ul> 
     <li>[!UICONTROL Attachment]</li> 
     <li>[!UICONTROL Comment]</li> 
     <li>[!UICONTROL Issue]</li> 
     <li>Progetto [!UICONTROL]</li> 
     <li>[!UICONTROL Sprint] </li> 
     <li>[!UICONTROL Worklog]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Chiamata API personalizzata]

Questo modulo di azione consente di effettuare una chiamata autenticata personalizzata al [!DNL Jira Software] API. In questo modo, puoi creare un’automazione del flusso di dati che non può essere eseguita dall’altro [!DNL Jira Software] moduli.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Jira Software] account a [!DNL Workfront Fusion], vedi <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connetti [!DNL Jira Software] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Inserisci un percorso relativo a<code>&lt;Instance URL>/rest/api/2/ </code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   td&gt; <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Aggiungi le intestazioni della richiesta sotto forma di oggetto JSON standard.</p> <p>Ad esempio: <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] aggiunge le intestazioni di autorizzazione.</p> </td> 
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

#### [!UICONTROL Eliminare un record]

Questo modulo di azione elimina un record specifico.

Specifica l’ID del record.

Il modulo restituisce l’ID del record ed eventuali campi associati, insieme a eventuali campi e valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Jira Software] account a [!DNL Workfront Fusion], vedi <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connetti [!DNL Jira Software] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td> <p>Selezionare il tipo di record da eliminare dal modulo. </p> 
    <ul> 
     <li>[!UICONTROL Attachment]</li> 
     <li>[!UICONTROL Comment]</li> 
     <li>[!UICONTROL Issue]</li> 
     <li>Progetto [!UICONTROL]</li> 
     <li>[!UICONTROL Sprint] </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID o chiave]</td> 
   <td>Immetti o mappa l’ID o la chiave del record da eliminare.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Scaricare un allegato]

Questo modulo di azione scarica un particolare allegato.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Jira Software] account a [!DNL Workfront Fusion], vedi <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connetti [!DNL Jira Software] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Immetti o mappa l’ID dell’allegato da scaricare.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Leggi un record]

Questo modulo di azione legge i dati da un singolo record in [!DNL Jira Software].

Specifica l’ID del record.

Il modulo restituisce tutti i campi standard associati al record, insieme a tutti i campi e i valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Jira Software] account a [!DNL Workfront Fusion], vedi <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connetti [!DNL Jira Software] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td> <p>Seleziona il tipo di [!DNL Jira] record che si desidera leggere nel modulo.</p> 
    <ul> 
     <li>[!UICONTROL Attachment]</li> 
     <li>[!UICONTROL Issue]</li> 
     <li>Progetto [!UICONTROL]</li> 
     <li>[!UICONTROL Sprint] </li> 
     <li>[!UICONTROL Utente]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output]</td> 
   <td>Selezionare gli output che si desidera ricevere. Le opzioni di output sono disponibili in base al tipo di record selezionato nel campo "[!UICONTROL Tipo di record]".</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td> <p>Inserisci o mappa l’univoco [!DNL Jira Software] ID del record che desideri che il modulo legga.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggiornare un record]

Questo modulo di azione aggiorna un record esistente, ad esempio un problema o un progetto.

Specifica l’ID del record.

Il modulo restituisce l’ID del record ed eventuali campi associati, insieme a eventuali campi e valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Jira Software] account a [!DNL Workfront Fusion], vedi <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connetti [!DNL Jira Software] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td> <p>Selezionare il tipo di record da aggiornare nel modulo. Quando si seleziona un tipo di record, nel modulo vengono visualizzati altri campi specifici per tale tipo di record.</p> 
    <ul> 
     <li>[!UICONTROL Comment]</li> 
     <li>[!UICONTROL Issue]</li> 
     <li>Progetto [!UICONTROL]</li> 
     <li>[!UICONTROL Sprint] </li> 
     <li>[!UICONTROL Problema di transizione]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID o chiave]</td> 
   <td>Immetti o mappa l’ID o la chiave del record da aggiornare.</td> 
  </tr> 
 </tbody> 
</table>

### Ricerche

* [[!UICONTROL Elencare record]](#list-records)
* [[!UICONTROL Cerca record]](#search-for-records)

#### [!UICONTROL Elencare record]

Questo modulo di ricerca recupera tutti gli elementi di un tipo specifico che corrispondono alla query di ricerca

Puoi mappare queste informazioni nei moduli successivi nello scenario.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Jira Software] account a [!DNL Workfront Fusion], vedi <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connetti [!DNL Jira Software] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td> <p>Selezionare il tipo di record che si desidera elencare nel modulo. Quando si seleziona un tipo di record, nel modulo vengono visualizzati altri campi specifici per tale tipo di record.</p> 
    <ul> 
     <li>[!UICONTROL Comment]</li> 
     <li>[!UICONTROL Issue]</li> 
     <li>Progetto [!UICONTROL]</li> 
     <li>[!UICONTROL Problema Sprint]</li> 
     <li>[!UICONTROL Worklog]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Max Results]</p> </td> 
   <td> <p>Immettere o mappare il numero massimo di record che il modulo deve recuperare durante ogni ciclo di esecuzione dello scenario.</p> </td> 
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

Puoi mappare queste informazioni nei moduli successivi nello scenario.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Jira Software] account a [!DNL Workfront Fusion], vedi <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connetti [!DNL Jira Software] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td> <p>Selezionare il tipo di record da cercare nel modulo. Quando si seleziona un tipo di record, nel modulo vengono visualizzati altri campi specifici per tale tipo di record.</p> 
    <ul> 
     <li>[!UICONTROL Issues]</li> 
     <li> <p>[!UICONTROL Issues by JQL (Jira Query Language)] </p> <p>Per ulteriori informazioni su JQL, vedi <a href="https://www.atlassian.com/blog/jira-software/jql-the-most-flexible-way-to-search-jira-14#:~:text=JQLstandsforJiraQuery,projectmanagers%2Candbusinessusers.">JQL</a> sul sito di aiuto di Atlassian. </p> </li> 
     <li>Progetto [!UICONTROL]</li> 
     <li>[!UICONTROL Progetto per problema]</li> 
     <li>[!UICONTROL Utente]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
