---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli di prova Workfront
description: In un [!DNL Adobe Workfront Fusion] puoi automatizzare i flussi di lavoro che utilizzano [!DNL Workfront Proof], nonché collegarlo a più applicazioni e servizi di terze parti.
author: Becky
feature: Workfront Fusion, Workfront Proof, Digital Content and Documents
exl-id: f5c6fb08-880d-4432-aef1-57db13b3ecdb
source-git-commit: a79c6b2fb2b651987f973bc0d74e0eeea312c5bc
workflow-type: tm+mt
source-wordcount: '2886'
ht-degree: 0%

---

# [!DNL Workfront Proof] moduli

In un [!DNL Adobe Workfront Fusion] puoi automatizzare i flussi di lavoro che utilizzano [!DNL Workfront Proof], nonché collegarlo a più applicazioni e servizi di terze parti.

Questa opzione è utile se è necessario eseguire attività attualmente non supportate nella correzione di [!DNL Workfront] o [!DNL Workfront Proof], ad esempio l’aggiornamento delle bozze in base a determinati eventi e la ricerca dei destinatari di una bozza.

La [!DNL Workfront Proof] connettore non viene conteggiato rispetto al numero di app attive disponibili per la tua organizzazione. Tutti gli scenari, anche se utilizzano solo [!DNL Workfront Proof] app, conteggia rispetto al conteggio totale degli scenari dell&#39;organizzazione.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p>  <p>[!UICONTROL [!DNL Workfront Fusion] per automazione del lavoro</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</td> 
  </tr> 
 </tbody> 
</table>

Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, vedi [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!DNL Workfront Proof] moduli e relativi campi

Quando si configura [!DNL Workfront Proof] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL Workfront Proof] potrebbero essere visualizzati, a seconda di fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se trovi il pulsante mappa sopra un campo o una funzione, puoi utilizzarlo per impostare variabili e funzioni per quel campo. Per ulteriori informazioni, consulta [Mappare informazioni da un modulo a un altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Azioni](#actions)
* [Ricerche](#searches)

### Triggers

* [Mostra bozze](#watch-proofs)
* [Riepilogo PDF](#watch-for-pdf-summary)
* [[!UICONTROL Attività di verifica]](#watch-proof-activity)

#### [!UICONTROL Mostra bozze]

Questo modulo trigger pianificato esegue uno scenario in cui un utente crea o prende una decisione su una bozza.

Il modulo restituisce un elenco di tutti i record trovati durante il periodo specificato, insieme ai relativi tipi. Inoltre restituisce i valori dei campi specificati. Se il modulo ha trovato decisioni sulla bozza, include sia i valori precedenti che quelli correnti, in campi separati. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Questo accade in un intervallo regolarmente programmato specificato.

Devi disporre di autorizzazioni sufficienti per accedere alle prove o alle bozze in [!DNL Workfront Proof] per recuperare queste informazioni.

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Workfront Proof] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Tipo di record</td> 
   <td>Seleziona il tipo di [!DNL Workfront Proof] registrare che si desidera che il modulo visualizzi.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Uscite</td> 
   <td> <p>Selezionare le informazioni che si desidera includere nel pacchetto di output per questo modulo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Limite</td> 
   <td> <p>Immettere o mappare il numero massimo di record che si desidera restituire dal modulo durante ogni ciclo di esecuzione degli scenari.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Riepilogo PDF]

Questo modulo di attivazione immediata esegue uno scenario in cui un utente crea un riepilogo di PDF per una bozza.

In questo modulo è richiesto un webhook.

Il modulo restituisce tutti i campi standard associati alla bozza, insieme a tutti i campi e i valori personalizzati a cui accede la connessione. Inoltre, crea una nuova sottoscrizione evento per i riepiloghi di PDF e restituisce il contenuto dall’attributo &quot;pdf_url&quot; inviato nel payload. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Workfront Proof] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Webhook]</td> 
   <td>Puoi selezionare un webhook esistente o crearne uno nuovo. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">Trigger istantanei (webhook) in [!DNL Adobe Workfront Fusion]</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td>Immettere o mappare il numero massimo di record che si desidera restituire dal modulo durante ogni ciclo di esecuzione degli scenari.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Attività di verifica]

Questo modulo trigger esegue uno scenario quando un’attività specifica si verifica su una bozza.

Il modulo restituisce tutti i campi standard associati alla bozza, insieme a tutti i campi e i valori personalizzati a cui accede la connessione. Inoltre, crea una nuova sottoscrizione evento per i riepiloghi e invia il contenuto dal `pdf_url` attributo inviato nel payload. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Workfront Proof] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo di attività]</td> 
   <td>Seleziona se vuoi visualizzare una nuova decisione (comprese le modifiche allo stato della bozza) o solo se lo stato della bozza globale cambia.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td>Immettere o mappare il numero massimo di record che si desidera restituire dal modulo durante ogni ciclo di esecuzione degli scenari.</td> 
  </tr> 
 </tbody> 
</table>

### Azioni

* [[!UICONTROL Crea bozza]](#create-proof)
* [[!UICONTROL Chiamata API personalizzata]](#custom-api-call)
* [[!UICONTROL Scarica bozza]](#download-proof)
* [[!UICONTROL Leggi un record]](#read-a-record)
* [[!UICONTROL Riepilogo richiesta PDF]](#request-pdf-summary)
* [[!UICONTROL Aggiorna bozza]](#update-proof)
* [[!UICONTROL Carica file]](#upload-file)

#### [!UICONTROL Crea bozza]

Questo modulo di azione crea una nuova bozza o una nuova versione di una bozza in [!DNL Workfront Proof].

Se crei una nuova versione, specifica i parametri della nuova bozza e della bozza sorgente.

Il modulo restituisce l’ID della nuova versione di prova o bozza.Puoi mappare queste informazioni nei moduli successivi nello scenario.

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Workfront Proof] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo di bozza]</td> 
   <td> <p>Specifica se la bozza creata deve disporre di un flusso di lavoro di base o di un flusso di lavoro automatizzato.</p> <p>Quindi compila i campi da visualizzare per il tipo di bozza scelto. Ad esempio, se hai scelto [!UICONTROL Automated Workflow], compila <strong>[!UICONTROL Workflow Stages]</strong> per configurare gli stadi.</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Consenti download del file originale]</td> 
   <td>Selezionare se si desidera consentire il download del file originale da cui è stata creata la bozza.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Classic Proof Viewer]</td> 
   <td>Seleziona se utilizzi il visualizzatore delle prove classiche.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Combina tutti i file in un’unica bozza]</td> 
   <td>Abilita questa opzione per combinare tutti i file in un’unica bozza a più pagine.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Creare una nuova versione di prova]</td> 
   <td>Seleziona questa opzione se desideri che il modulo crei una nuova versione di una bozza esistente. Quindi, nella <strong>[!UICONTROL ID bozza esistente]</strong> campo che visualizza, mappa o immetti l’ID univoco della bozza.</td> 
  </tr> 
  <tr> 
   <td>Etichetta [!UICONTROL Custom Link]</td> 
   <td>Immetti o mappa un’etichetta per il collegamento di bozza personalizzato.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL URL di collegamento personalizzato]</td> 
   <td>Immetti o mappa l’URL del collegamento personalizzato.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Notifiche e-mail predefinite per gli abbonati]</td> 
   <td>Digita uno dei seguenti numeri per indicare quale delle seguenti impostazioni di notifica e-mail predefinite desideri utilizzare per la bozza creata.
    <ul>
     <li><strong>1</strong> - Tutte le nuove osservazioni e risposte</li>
     <li><strong>2</strong> - Risposte ai miei commenti</li>
     <li><strong>3</strong> - Riepilogo giornaliero</li>
     <li><strong>4</strong> - Riepilogo orario</li>
     <li><strong>5</strong> - Solo decisioni</li>
     <li><strong>9</strong> - Disattivato</li>
    </ul></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Disattiva riepilogo Excel]</td> 
   <td>Seleziona se disabilitare la possibilità di scaricare commenti di bozza in un file Excel.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Disattiva riepilogo PDF]</td> 
   <td>Seleziona se disabilitare la possibilità di scaricare commenti di bozza in un file PDF.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Disattiva e-mail di abbonamento]</td> 
   <td>Seleziona se vuoi disattivare l’e-mail di abbonamento per questa bozza.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Abilita Lettore Da Incorporare]</td> 
   <td>Seleziona se desideri abilitare il lettore incorporato per questa bozza.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Abilita abbonamenti]</td> 
   <td>Seleziona se le persone non partecipanti possono effettuare l’iscrizione alla bozza.<br>Se selezioni questa opzione, puoi anche selezionare il Ruolo predefinito per gli abbonati, come descritto in questa tabella.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Abilita convalida sottoscrizioni]</td> 
   <td>Seleziona se desideri abilitare la convalida dell’e-mail di abbonamento. Se questa opzione è abilitata, l’utente con sottoscrizione deve fare clic su un collegamento presente in un messaggio e-mail per accedere a una bozza.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Abilita URL team]</td> 
   <td>Seleziona se vuoi che la bozza creata nasconda o mostri l’URL del team.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL File Hash] <span style="font-weight: normal;">o</span> [!UICONTROL File Hash]</td> 
   <td>Aggiungi l'ID del file o dei file da cui desideri creare una bozza o delle bozze.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL File Names]</td> 
   <td>Aggiungere il nome o i nomi del file per la bozza creata Questo campo è obbligatorio.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Blocca la bozza quando vengono prese tutte le decisioni necessarie]</td> 
   <td>Specifica se la bozza creata deve essere bloccata dopo che sono state prese tutte le decisioni necessarie.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Notifica ai destinatari questa bozza]</td> 
   <td>Seleziona un’opzione per indicare se desideri ricevere una notifica al momento della creazione della bozza.&gt;</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome bozza]</td> 
   <td>Digitare un nome per la bozza creata Questo campo è obbligatorio. Utilizzare un simbolo di barra verticale (|) per separare i nomi per più bozze.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID proprietario bozza]</td> 
   <td>Immetti o mappa l'ID del proprietario della bozza. Se questo campo viene lasciato vuoto, il proprietario della bozza viene impostato sull'utente corrente.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID riferimento]</td> 
   <td>Immetti l'ID di riferimento per la bozza.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Richiedi firma elettronica]</td> 
   <td>Selezionare se si desidera richiedere a chiunque prenda una decisione su una bozza di inviare una firma elettronica.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Richiedi accesso]</td> 
   <td> <p>Specifica se la bozza creata deve richiedere un accesso. </p> <p>È la stessa impostazione di [!UICONTROL Login Required] spiegata in <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">[!UICONTROL Configura impostazioni bozza] in [!DNL Workfront Proof]</a></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>ID risoluzione [!UICONTROL]</td> 
   <td>Immetti l’ID della risoluzione da utilizzare per la bozza. Per un elenco degli ID di risoluzione, vedi [!DNL Workfront Proof] <a href="http://api.proofhq.com/home/objects/soapworkflowproofobject">Documentazione API</a>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL SWF]</td> 
   <td>Immettere il tipo di bozza di SWF.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Show] [item]</td> 
   <td>Per ogni elemento, seleziona se desideri visualizzarlo nella bozza.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Workspace ID]</td> 
   <td>Immetti l’ID dell’area di lavoro in cui desideri creare la bozza. </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Recipients]</td> 
   <td>Aggiungi gli indirizzi e-mail dei destinatari desiderati per la bozza creata .</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Scadenza]</td> 
   <td> <p>Specifica la scadenza per la bozza creata. Utilizza il formato data seguente:</p> <p><code>YYYY-MM-DD hh:mm</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Chiamata API personalizzata]

Questo modulo di azione ti consente di effettuare una chiamata autenticata personalizzata al [!DNL Workfront Proof] API. In questo modo, puoi creare un’automazione del flusso di dati che non può essere eseguita dall’altro [!DNL Workfront Proof] moduli.

Il modulo restituisce il codice di stato, le intestazioni e il corpo. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Workfront Proof] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL, Metodo]</td> 
   <td>Imposta l’azione per la chiamata API. Per le azioni disponibili, consulta la sezione <a href="http://api.proofhq.com/">Documentazione API di prova</a>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Body (XML)]</td> 
   <td> <p>Aggiungi il contenuto del corpo per la chiamata API sotto forma di un oggetto JSON standard.</p> <p>Nota:  <p>Quando si utilizzano istruzioni condizionali come <code>if</code> nel JSON, inserisci le virgolette al di fuori dell’istruzione condizionale.</p> 
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

Questo modulo di azione scarica il file sorgente di una prova particolare identificata utilizzando il relativo ID.

Specifica l’ID della bozza.

Il modulo restituisce il contenuto del file di origine utilizzato per creare la bozza.È possibile mappare queste informazioni nei moduli successivi nello scenario.

È necessario disporre di autorizzazioni sufficienti per accedere al record in [!DNL Workfront Proof] per recuperare queste informazioni.

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Workfront Proof] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID bozza]</td> 
   <td> <p>Digita l’ID univoco della bozza, disponibile nella pagina [!UICONTROL Proof Details] . Per ulteriori informazioni, consulta <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md" class="MCXref xref" data-mc-variable-override="">Gestisci dettagli bozza in [!DNL Workfront Proof]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Leggi un record]

Questo modulo di azione legge i dati da una singola bozza in [!DNL Workfront Proof].

Specifica l’ID della bozza e le informazioni desiderate dalla bozza.

Il modulo restituisce i valori dei campi scelti per la bozza, insieme ai relativi tipi. Puoi mappare queste informazioni nei moduli successivi nello scenario .

È necessario disporre di autorizzazioni sufficienti per accedere al record in [!DNL Workfront Proof] per recuperare queste informazioni.

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Workfront Proof] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo di record]</td> 
   <td>Seleziona se desideri leggere una bozza, commenti di bozza o revisori di prove.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Uscite]</td> 
   <td> <p>Selezionare le informazioni che si desidera includere nel pacchetto di output per questo modulo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td>Immetti o mappa l'univoco [!DNL Workfront Proof] ID del record che si desidera leggere nel modulo.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Riepilogo richiesta PDF]

Questo modulo di azione richiede il riepilogo di PDF per una prova particolare in [!DNL Workfront Proof].

Specifica l’ID della bozza.

Il modulo restituisce informazioni di riepilogo di PDF. Puoi mappare queste informazioni nei moduli successivi nello scenario .

È necessario disporre di autorizzazioni sufficienti per accedere al record in [!DNL Workfront Proof] per recuperare queste informazioni.

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Workfront Proof] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID bozza]</td> 
   <td> <p>Inserisci l'univoco [!DNL Workfront Proof] ID della bozza di cui si desidera richiedere un riepilogo di PDF.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Callback URL]</td> 
   <td>Immetti o mappa l’URL in cui desideri inviare il riepilogo di PDF.</td> 
  </tr> 
 </tbody> 
</table>

##### Possibile errore

* **Errore**: &quot;[!UICONTROL Non si dispone del privilegio di eseguire questa richiesta. La fase deve contenere almeno un destinatario.]&quot;
* **Soluzione**: Assicurati di non essere l’unico assegnato alle fasi del flusso di lavoro. Deve essere assegnato un altro utente alle fasi del flusso di lavoro.

#### [!UICONTROL Aggiorna bozza]

Questo modulo di azione aggiorna una bozza esistente in [!DNL Workfront Proof].

Puoi specificare l’ID e il tipo di record della bozza e i campi da includere nell’output.

Il modulo restituisce tutti i campi standard associati al record, insieme a eventuali campi e valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

È necessario disporre di autorizzazioni sufficienti per accedere al record in [!DNL Workfront Proof] per recuperare queste informazioni.

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Workfront Proof] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID bozza]</td> 
   <td> <p>Digita l’ID univoco della bozza, disponibile nella pagina [!UICONTROL Proof Details] . Per ulteriori informazioni, consulta <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md" class="MCXref xref" data-mc-variable-override="">Gestisci dettagli bozza in [!DNL Workfront Proof]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Scadenza]</td> 
   <td> <p>Specifica la scadenza per la bozza creata. Utilizza il formato data seguente:</p> <p><code>YYYY-MM-DD hh:mm</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Notifiche e-mail predefinite per gli abbonati]</td> 
   <td>Seleziona una delle seguenti impostazioni di notifica e-mail predefinite da utilizzare per la bozza creata.
    <ul>
     <li> [!UICONTROL Tutti i nuovi commenti e risposte]</li>
     <li>[!UICONTROL Risposte ai miei commenti]</li>
     <li>Riepilogo giornaliero di [!UICONTROL]</li>
     <li> Riepilogo orario</li>
     <li> Solo decisioni</li>
     <li> [!UICONTROL disabilitata]</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ruolo predefinito]</td> 
   <td>Selezionare il ruolo predefinito per la bozza.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Disattiva e-mail di abbonamento]</td> 
   <td>Seleziona se vuoi disattivare l’e-mail di abbonamento per questa bozza.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Abilita abbonamenti]</td> 
   <td>Seleziona se le persone non partecipanti possono effettuare l’iscrizione alla bozza.<br>Se selezioni questa opzione, puoi anche selezionare il [!UICONTROL Default Role] per gli abbonati, come descritto in questa tabella.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Abilita convalida sottoscrizioni]</td> 
   <td>Seleziona se desideri abilitare la convalida dell’e-mail di abbonamento. Se questa opzione è abilitata, l’utente con sottoscrizione deve fare clic su un collegamento presente in un messaggio e-mail per accedere a una bozza.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Abilita URL team]</td> 
   <td>Seleziona se vuoi che la bozza creata nasconda o mostri l’URL del team.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Blocca la bozza quando vengono prese tutte le decisioni necessarie]</td> 
   <td>Specifica se la bozza creata deve essere bloccata dopo che sono state prese tutte le decisioni necessarie.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Message]</td> 
   <td>Immetti o mappa un messaggio che desideri accompagnare la bozza.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID bozza] </td> 
   <td>Immetti o mappa l’ID della bozza da aggiornare.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome bozza]</td> 
   <td>Immetti o mappa il nome della bozza da aggiornare.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Richiedi accesso]</td> 
   <td> <p>Specifica se la bozza creata deve richiedere un accesso. </p> <p>È la stessa impostazione di [!UICONTROL Login Required] spiegata in <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">[!UICONTROL Configura impostazioni bozza] in [!DNL Workfront Proof]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Mostra versioni come]</td> 
   <td>Seleziona se visualizzare un collegamento ad altre versioni di questa bozza.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Subject]</td> 
   <td>Immettere o mappare l'oggetto della bozza</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Carica file]

Questo modulo di azione carica un file da utilizzare con il [!UICONTROL Crea bozza] modulo in [!DNL Workfront Proof].

Il modulo restituisce un ID hash per il file caricato. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Workfront Proof] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File di origine]</td> 
   <td> <p>Selezionare un file di origine da un modulo precedente o mappare il nome e i dati del file di origine.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Ricerche

* [[!UICONTROL Ricerca]](#search)
* [[!UICONTROL Elenca modelli di flussi di lavoro]](#list-workflow-templates)

#### [!UICONTROL Ricerca]

Questo modulo di ricerca cerca i record in un oggetto in [!DNL Workfront Proof] che corrispondono alla query di ricerca specificata.

Il modulo restituisce l’ID della bozza se sta cercando una bozza. Oppure restituisce gli ID utente, le e-mail, i nomi, le posizioni e gli alias e-mail dei destinatari, se sta cercando i destinatari. Puoi mappare queste informazioni nei moduli successivi nello scenario .

È necessario disporre di autorizzazioni sufficienti per accedere al record in [!DNL Workfront Proof] per recuperare queste informazioni.

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Workfront Proof] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Cerca</td> 
   <td> <p>Se[!UICONTROL ]selezionare il tipo di record che si desidera cercare nel modulo.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Proof]</strong> </p> <p>Immettere il nome della bozza da cercare.</p> </li> 
     <li> <p><strong>[!UICONTROL Recipient]</strong> </p> <p>Immetti l’indirizzo e-mail del destinatario che desideri cercare.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Set di risultati]</td> 
   <td>Indica se il modulo cercherà <strong>[!UICONTROL Tutti i record corrispondenti]</strong> o solo <strong>[!UICONTROL Record di prima corrispondenza]</strong>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Ordina per]</td> 
   <td>Selezionare il campo in base al quale si desidera ordinare i risultati.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Direzione di ordinamento]</td> 
   <td> <p>Seleziona se ordinare i risultati in ordine crescente o decrescente.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Elenca modelli di flussi di lavoro]

Questo modulo di ricerca elenca tutti i modelli di flusso di lavoro disponibili.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Workfront Proof] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Uscite]</td> 
   <td> <p>Selezionare le informazioni che si desidera includere nel pacchetto di output per questo modulo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Limit]</td> 
   <td> <p>Immetti o mappa il numero massimo di modelli che desideri che il modulo restituisca durante ogni ciclo di esecuzione di uno scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>
