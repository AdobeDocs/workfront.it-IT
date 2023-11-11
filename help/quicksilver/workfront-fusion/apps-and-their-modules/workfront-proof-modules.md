---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli bozza di Workfront
description: In un [!DNL Adobe Workfront Fusion] scenario, puoi automatizzare i flussi di lavoro che utilizzano [!DNL Workfront Proof], oltre a collegarlo a più applicazioni e servizi di terze parti.
author: Becky
feature: Workfront Fusion, Workfront Proof, Digital Content and Documents
exl-id: f5c6fb08-880d-4432-aef1-57db13b3ecdb
source-git-commit: 5d7ff744ed0721ffa6d793a224226f28a76c57a0
workflow-type: tm+mt
source-wordcount: '2934'
ht-degree: 0%

---

# [!DNL Workfront Proof] moduli

In un [!DNL Adobe Workfront Fusion] scenario, puoi automatizzare i flussi di lavoro che utilizzano [!DNL Workfront Proof], oltre a collegarlo a più applicazioni e servizi di terze parti.

Questa opzione è utile se devi eseguire attività attualmente non supportate nella verifica in [!DNL Workfront] o in [!DNL Workfront Proof], ad esempio aggiornando le bozze in base a determinati eventi e cercando i destinatari di una bozza.

Il [!DNL Workfront Proof] il connettore non viene conteggiato rispetto al numero di app attive disponibili per l’organizzazione. Tutti gli scenari, anche se utilizzano solo [!DNL Workfront Proof] app, conteggio rispetto al conteggio totale degli scenari della tua organizzazione.

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
   <p>Requisito licenza legacy: [!UICONTROL [!DNL Workfront Fusion] per l'automazione e l'integrazione del lavoro], [!UICONTROL [!DNL Workfront Fusion] per automazione lavoro]</p>
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

## [!DNL Workfront Proof] moduli e relativi campi

Quando si configura [!DNL Workfront Proof] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL Workfront Proof] I campi potrebbero essere visualizzati in base a fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se viene visualizzato il pulsante Mappa sopra un campo o una funzione, è possibile utilizzarlo per impostare variabili e funzioni per tale campo. Per ulteriori informazioni, consulta [Mappare le informazioni da un modulo all’altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Azioni](#actions)
* [Ricerche](#searches)

### Triggers

* [Guarda le bozze](#watch-proofs)
* [Osserva riepilogo PDF](#watch-for-pdf-summary)
* [[!UICONTROL Guarda l’attività bozza]](#watch-proof-activity)

#### [!UICONTROL Guarda le bozze]

Questo modulo di attivazione pianificato esegue uno scenario quando un utente crea o prende una decisione su una bozza.

Il modulo restituisce un elenco di tutti i record trovati durante il periodo specificato, insieme ai relativi tipi. Restituisce anche i valori dei campi specificati. Se il modulo ha trovato decisioni prese sulla bozza, include sia i valori precedenti che quelli correnti in campi separati. Puoi mappare queste informazioni nei moduli successivi nello scenario.

Questo si verifica in un intervallo pianificato regolare specificato.

È necessario disporre di autorizzazioni sufficienti per accedere alla bozza o alle bozze in [!DNL Workfront Proof] per recuperare queste informazioni.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Workfront Proof] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Tipo di record</td> 
   <td>Seleziona il tipo di [!DNL Workfront Proof] registrare che si desidera che il modulo controlli.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Uscite</td> 
   <td> <p>Seleziona le informazioni da includere nel bundle di output per questo modulo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Limite</td> 
   <td> <p>Immettere o mappare il numero massimo di record che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Osserva riepilogo PDF]

Questo modulo di attivazione immediata esegue uno scenario quando un utente crea un riepilogo di PDF per una bozza.

In questo modulo è necessario un webhook.

Il modulo restituisce tutti i campi standard associati alla bozza, insieme a tutti i campi e i valori personalizzati a cui la connessione accede. Crea anche un nuovo abbonamento evento per i riepiloghi PDF e restituisce il contenuto dall’attributo &quot;pdf_url&quot; inviato nel payload. Puoi mappare queste informazioni nei moduli successivi nello scenario.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Workfront Proof] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Webhook]</td> 
   <td>Puoi selezionare un webhook esistente o crearne uno nuovo. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">Trigger istantanei (webhook) in [!DNL Adobe Workfront Fusion]</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td>Immettere o mappare il numero massimo di record che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Guarda l’attività bozza]

Questo modulo di attivazione esegue uno scenario quando si verifica un’attività specificata su una bozza di bozza.

Il modulo restituisce tutti i campi standard associati alla bozza, insieme a tutti i campi e i valori personalizzati a cui la connessione accede. Crea anche un nuovo abbonamento evento per i riepiloghi dei PDF e restituisce il contenuto dal `pdf_url` attributo inviato nel payload. Puoi mappare queste informazioni nei moduli successivi nello scenario.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Workfront Proof] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo di attività]</td> 
   <td>Seleziona se desideri controllare le nuove decisioni (comprese le modifiche di stato [!UICONTROL proof]) o solo le modifiche generali dello stato della bozza.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td>Immettere o mappare il numero massimo di record che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</td> 
  </tr> 
 </tbody> 
</table>

### Azioni

* [[!UICONTROL Crea bozza]](#create-proof)
* [[!UICONTROL Chiamata API personalizzata]](#custom-api-call)
* [[!UICONTROL Scarica bozza]](#download-proof)
* [[!UICONTROL Leggi un record]](#read-a-record)
* [[!UICONTROL Richiedi riepilogo PDF]](#request-pdf-summary)
* [[!UICONTROL Aggiorna bozza]](#update-proof)
* [[!UICONTROL Carica file]](#upload-file)

#### [!UICONTROL Crea bozza]

Questo modulo di azione crea una nuova bozza o una nuova versione di una bozza in [!DNL Workfront Proof].

Se crei una nuova versione, puoi specificare i parametri per la nuova bozza e la bozza sorgente.

Il modulo restituisce l’ID della nuova bozza o versione della bozza. È possibile mappare queste informazioni nei moduli successivi nello scenario.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Workfront Proof] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>Tipo di bozza [!UICONTROL]</td> 
   <td> <p>Specifica se la bozza creata deve avere un flusso di lavoro di base o un flusso di lavoro automatico [!UICONTROL].</p> <p>Compila quindi i campi visualizzati per il tipo di bozza scelto. Ad esempio, se hai scelto [!UICONTROL Automated Workflow], compila il <strong>[!UICONTROL Fasi flusso di lavoro]</strong> per configurare le fasi.</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Consenti il download del file originale]</td> 
   <td>Seleziona se desideri consentire il download del file originale da cui è stata creata la bozza.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Visualizzatore bozze di [!UICONTROL Classic]</td> 
   <td>Seleziona se utilizzi il visualizzatore di bozze classico.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Combina tutti i file in un'unica bozza]</td> 
   <td>Abilita questa opzione per combinare tutti i file in un’unica bozza multipagina.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Crea una nuova versione di bozza]</td> 
   <td>Seleziona questa opzione se desideri che il modulo crei una nuova versione di una bozza esistente. Quindi, nella <strong>[!UICONTROL ID bozza esistente]</strong> che visualizza, mappa o immetti l’ID univoco della bozza.</td> 
  </tr> 
  <tr> 
   <td>Etichetta collegamento personalizzato [!UICONTROL]</td> 
   <td>Inserisci o mappa un’etichetta per il collegamento della bozza personalizzata.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL URL collegamento personalizzato]</td> 
   <td>Inserisci o mappa l’URL del collegamento personalizzato.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Notifiche e-mail predefinite per gli abbonati]</td> 
   <td>Digita uno dei seguenti numeri per indicare quale delle seguenti impostazioni predefinite di notifica e-mail desideri utilizzare per la bozza creata.
    <ul>
     <li><strong>1</strong> - Tutti i nuovi commenti e risposte</li>
     <li><strong>2</strong> - Risposte alle mie osservazioni</li>
     <li><strong>3</strong> - Riepilogo giornaliero</li>
     <li><strong>4</strong> - Riepilogo orario</li>
     <li><strong>5</strong> - Solo decisioni</li>
     <li><strong>9</strong> - Disabilitato</li>
    </ul></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Disattiva riepilogo Excel]</td> 
   <td>Seleziona se vuoi disabilitare la possibilità di scaricare i commenti della bozza in un file Excel.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Disattiva Riepilogo PDF]</td> 
   <td>Seleziona se vuoi disabilitare la possibilità di scaricare i commenti della bozza in un file PDF.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Disattiva E-Mail Sottoscrizione]</td> 
   <td>Seleziona se vuoi disabilitare l’e-mail di abbonamento per questa bozza.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL - Abilita lettore incorporato]</td> 
   <td>Seleziona se desideri abilitare il lettore incorporato per questa bozza.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL - Abilita sottoscrizioni]</td> 
   <td>Seleziona se consentire agli utenti non partecipanti di abbonarsi alla bozza.<br>Se si seleziona questa opzione, è anche possibile selezionare il Ruolo predefinito per i sottoscrittori, come descritto in questa tabella.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Abilita convalida sottoscrizioni]</td> 
   <td>Specificare se si desidera abilitare la convalida e-mail dell'abbonamento. Se questa opzione è abilitata, l’abbonato deve fare clic su un collegamento in un messaggio e-mail per accedere a una bozza.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL - Abilita URL team]</td> 
   <td>Seleziona se desideri che la bozza creata nasconda o mostri l’URL del team.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Hash file] <span style="font-weight: normal;">o</span> [!UICONTROL Hash file]</td> 
   <td>Aggiungi l’ID del file o dei file da cui desideri creare una bozza o delle bozze.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Nomi File]</td> 
   <td>Aggiungi il nome o i nomi del file per la bozza creata Questo campo è obbligatorio.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Blocca la bozza quando vengono prese tutte le decisioni necessarie]</td> 
   <td>Specifica se desideri che la bozza creata venga bloccata dopo aver preso tutte le decisioni necessarie.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Notifica i destinatari relativamente a questa bozza]</td> 
   <td>Seleziona un’opzione per indicare se desideri che i destinatari ricevano una notifica al momento della creazione della bozza.&gt;</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome bozza]</td> 
   <td>Digita un nome per la bozza creata Questo è un campo obbligatorio. Utilizza un simbolo di barra verticale (|) per separare i nomi per più bozze.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID proprietario bozza]</td> 
   <td>Inserisci o mappa l’ID del proprietario della bozza. Se questo campo viene lasciato vuoto, il proprietario della bozza viene impostato sull’utente corrente.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID riferimento]</td> 
   <td>Immetti l’ID di riferimento per la bozza.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Richiedi firma elettronica]</td> 
   <td>Seleziona se desideri richiedere a chiunque prenda una decisione su una bozza di inviare una firma elettronica.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Require login]</td> 
   <td> <p>Specifica se la bozza creata deve richiedere l’accesso. </p> <p>Corrisponde all'impostazione [!UICONTROL Login Required] illustrata in <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">[!UICONTROL Configura impostazioni bozza] in [!DNL Workfront Proof]</a></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ID risoluzione]</td> 
   <td>Immetti l’ID della risoluzione da utilizzare per la bozza. Per un elenco degli ID risoluzione, vedi [!DNL Workfront Proof] <a href="https://api.proofhq.com/home/objects/soapworkflowproofobject.html">Documentazione API</a>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL SWF]</td> 
   <td>Immetti il tipo di bozza SWF.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Show] [elemento]</td> 
   <td>Per ogni elemento, seleziona se desideri visualizzarlo nella bozza.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ID area di lavoro]</td> 
   <td>Immetti l’ID dell’area di lavoro in cui desideri creare la bozza. </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Destinatari]</td> 
   <td>Aggiungi gli indirizzi e-mail dei destinatari desiderati per la bozza creata.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Scadenza]</td> 
   <td> <p>Specifica la scadenza desiderata per la bozza creata. Utilizza il seguente formato data:</p> <p><code>YYYY-MM-DD hh:mm</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Chiamata API personalizzata]

Questo modulo di azione consente di effettuare una chiamata autenticata personalizzata al [!DNL Workfront Proof] API. In questo modo, puoi creare un’automazione del flusso di dati che non può essere eseguita dall’altro [!DNL Workfront Proof] moduli.

Il modulo restituisce il codice di stato, le intestazioni e il corpo. Puoi mappare queste informazioni nei moduli successivi nello scenario.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Workfront Proof] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Method]</td> 
   <td>Imposta l’azione per la chiamata API. Per informazioni sulle azioni disponibili, vedere <a href="http://api.proofhq.com/">Documentazione API di bozza</a>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Body (XML)]</td> 
   <td> <p>Aggiungi il contenuto body per la chiamata API sotto forma di oggetto JSON standard.</p> <p>Nota:  <p>Quando si utilizzano istruzioni condizionali quali <code>if</code> nel JSON, inserisci le virgolette al di fuori dell’istruzione condizionale.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Esempio:**
>
>![](assets/wfp-api-module-example-350x586.png)

#### [!UICONTROL Scarica bozza]

Questo modulo di azione scarica il file sorgente di una particolare bozza che identifichi utilizzando il relativo ID.

Specifica l’ID della bozza.

Il modulo restituisce il contenuto del file di origine utilizzato per creare la bozza.È possibile mappare queste informazioni nei moduli successivi nello scenario.

Devi disporre di autorizzazioni sufficienti per accedere al record in [!DNL Workfront Proof] per recuperare queste informazioni.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Workfront Proof] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID bozza]</td> 
   <td> <p>Digita l’ID univoco della bozza, reperibile nella pagina [!UICONTROL Proof Details] (Dettagli bozza). Per ulteriori informazioni, consulta <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md" class="MCXref xref" data-mc-variable-override="">Gestire i dettagli della bozza in [!DNL Workfront Proof]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Leggi un record]

Questo modulo di azione legge i dati da una singola bozza in [!DNL Workfront Proof].

Puoi specificare l’ID della bozza e le informazioni che desideri ricavare dalla bozza.

Il modulo restituisce i valori dei campi scelti per la bozza, insieme ai relativi tipi. Puoi mappare queste informazioni nei moduli successivi nello scenario.

Devi disporre di autorizzazioni sufficienti per accedere al record in [!DNL Workfront Proof] per recuperare queste informazioni.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Workfront Proof] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo di record]</td> 
   <td>Seleziona se desideri leggere una bozza, i commenti della bozza o i revisori della bozza.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Output]</td> 
   <td> <p>Seleziona le informazioni da includere nel bundle di output per questo modulo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td>Inserisci o mappa l’univoco [!DNL Workfront Proof] ID del record che desideri che il modulo legga.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Richiedi riepilogo PDF]

Questo modulo di azione richiede il riepilogo dei PDF per una particolare bozza in [!DNL Workfront Proof].

Specifica l’ID della bozza.

Il modulo restituisce informazioni di riepilogo PDF. Puoi mappare queste informazioni nei moduli successivi nello scenario.

Devi disporre di autorizzazioni sufficienti per accedere al record in [!DNL Workfront Proof] per recuperare queste informazioni.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Workfront Proof] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID bozza]</td> 
   <td> <p>Immetti l’univoco [!DNL Workfront Proof] ID della bozza per la quale desideri richiedere un riepilogo PDF.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL URL callback]</td> 
   <td>Inserisci o mappa l’URL in cui desideri inviare il riepilogo dei PDF.</td> 
  </tr> 
 </tbody> 
</table>

##### Possibile errore

* **Errore**: &quot;[!UICONTROL Non si dispone dei privilegi necessari per eseguire questa richiesta. La fase deve contenere almeno un destinatario.]&quot;
* **Soluzione**: accertati di non essere l’unico assegnato alle fasi del flusso di lavoro. Un altro utente deve essere assegnato alle fasi del flusso di lavoro.

#### [!UICONTROL Aggiorna bozza]

Questo modulo di azione aggiorna una bozza esistente in [!DNL Workfront Proof].

Puoi specificare l’ID della bozza e il tipo di record, nonché i campi da includere nell’output.

Il modulo restituisce tutti i campi standard associati al record, insieme a tutti i campi e i valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario.

Devi disporre di autorizzazioni sufficienti per accedere al record in [!DNL Workfront Proof] per recuperare queste informazioni.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Workfront Proof] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID bozza]</td> 
   <td> <p>Digita l’ID univoco della bozza, reperibile nella pagina [!UICONTROL Proof Details] (Dettagli bozza). Per ulteriori informazioni, consulta <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md" class="MCXref xref" data-mc-variable-override="">Gestire i dettagli della bozza in [!DNL Workfront Proof]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Scadenza]</td> 
   <td> <p>Specifica la scadenza desiderata per la bozza creata. Utilizza il seguente formato data:</p> <p><code>YYYY-MM-DD hh:mm</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Notifiche e-mail predefinite per gli abbonati]</td> 
   <td>Seleziona una delle seguenti impostazioni predefinite di notifica e-mail da utilizzare per la bozza creata.
    <ul>
     <li> [!UICONTROL Tutti i nuovi commenti e risposte]</li>
     <li>[!UICONTROL Risponde ai miei commenti]</li>
     <li>Riepilogo giornaliero di [!UICONTROL]</li>
     <li> Riepilogo orario [!UICONTROL]</li>
     <li> [!UICONTROL Decisions only]</li>
     <li> [!UICONTROL Disabilitato]</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>Ruolo predefinito di [!UICONTROL]</td> 
   <td>Seleziona il ruolo predefinito per la bozza.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Disattiva E-Mail Sottoscrizione]</td> 
   <td>Seleziona se vuoi disabilitare l’e-mail di abbonamento per questa bozza.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL - Abilita sottoscrizioni]</td> 
   <td>Seleziona se consentire agli utenti non partecipanti di abbonarsi alla bozza.<br>Se si seleziona questa opzione, è anche possibile selezionare il [!UICONTROL Default Role] per i sottoscrittori, come descritto in questa tabella.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Abilita convalida sottoscrizioni]</td> 
   <td>Specificare se si desidera abilitare la convalida e-mail dell'abbonamento. Se questa opzione è abilitata, l’abbonato deve fare clic su un collegamento in un messaggio e-mail per accedere a una bozza.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL - Abilita URL team]</td> 
   <td>Seleziona se desideri che la bozza creata nasconda o mostri l’URL del team.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Blocca la bozza quando vengono prese tutte le decisioni necessarie]</td> 
   <td>Specifica se desideri che la bozza creata venga bloccata dopo aver preso tutte le decisioni necessarie.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Messaggio]</td> 
   <td>Immetti o mappa un messaggio da allegare alla bozza.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID bozza] </td> 
   <td>Inserisci o mappa l’ID della bozza da aggiornare.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome bozza]</td> 
   <td>Inserisci o mappa il nome della bozza da aggiornare.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Require login]</td> 
   <td> <p>Specifica se la bozza creata deve richiedere l’accesso. </p> <p>Corrisponde all'impostazione [!UICONTROL Login Required] illustrata in <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">[!UICONTROL Configura impostazioni bozza] in [!DNL Workfront Proof]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Mostra Versioni Simili]</td> 
   <td>Seleziona se desideri visualizzare un collegamento ad altre versioni di questa bozza.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Subject]</td> 
   <td>Inserisci o mappa l’oggetto della bozza</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Carica file]

Questo modulo di azione carica un file da utilizzare con [!UICONTROL Crea bozza] modulo in [!DNL Workfront Proof].

Il modulo restituisce un ID hash per il file caricato. Puoi mappare queste informazioni nei moduli successivi nello scenario.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Workfront Proof] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File di origine]</td> 
   <td> <p>Selezionare un file di origine da un modulo precedente o mappare il nome e i dati del file di origine.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Ricerche

* [[!UICONTROL Ricerca]](#search)
* [[!UICONTROL Elenca modelli flusso di lavoro]](#list-workflow-templates)

#### [!UICONTROL Ricerca]

Questo modulo di ricerca cerca i record in un oggetto in [!DNL Workfront Proof] che corrispondono alla query di ricerca specificata.

Il modulo restituisce l’ID della bozza se sta cercando una bozza. In alternativa, restituisce gli ID utente, le e-mail, i nomi, le posizioni e gli alias e-mail dei destinatari, se è in corso la ricerca dei destinatari. È possibile mappare queste informazioni nei moduli successivi nello scenario.

Devi disporre di autorizzazioni sufficienti per accedere al record in [!DNL Workfront Proof] per recuperare queste informazioni.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Workfront Proof] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Cerca</td> 
   <td> <p>Se[!UICONTROL ]selezionare il tipo di record che si desidera cercare nel modulo.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Proof]</strong> </p> <p>Immetti il Nome bozza della bozza da cercare.</p> </li> 
     <li> <p><strong>[!UICONTROL Recipient]</strong> </p> <p>Immetti l’indirizzo e-mail del destinatario da cercare.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Result Set]</td> 
   <td>Indica se il modulo cercherà <strong>[!UICONTROL Tutti I Record Corrispondenti]</strong> o solo <strong>[!UICONTROL First Matching Record]</strong>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Ordina per]</td> 
   <td>Selezionare il campo in base al quale ordinare i risultati.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Direzione ordinamento]</td> 
   <td> <p>Seleziona se desideri ordinare i risultati in modo crescente o decrescente.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Elenca modelli flusso di lavoro]

Questo modulo di ricerca elenca tutti i modelli di flusso di lavoro disponibili.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Workfront Proof] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Output]</td> 
   <td> <p>Seleziona le informazioni da includere nel bundle di output per questo modulo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Limit]</td> 
   <td> <p>Immettere o mappare il numero massimo di modelli che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>
