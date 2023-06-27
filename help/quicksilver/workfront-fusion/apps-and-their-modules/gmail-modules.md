---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli Gmail
description: In un [!DNL Adobe Workfront Fusion] scenario, puoi automatizzare i flussi di lavoro che utilizzano Gmail e collegarlo a più applicazioni e servizi di terze parti.
author: Becky
feature: Workfront Fusion
exl-id: 1987156c-e003-4f99-8913-cb47f77efbfc
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1833'
ht-degree: 0%

---

# [!DNL Gmail] moduli

In un [!DNL Adobe Workfront Fusion] scenario, puoi automatizzare i flussi di lavoro che utilizzano [!DNL Gmail], oltre a collegarlo a più applicazioni e servizi di terze parti.

Per istruzioni sulla creazione di uno scenario, consulta [Creare uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). Per informazioni sui moduli, consulta [Moduli in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, consulta [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Prerequisiti

Da utilizzare [!DNL Gmail] moduli, è necessario disporre di un [!DNL Gmail] account.

## Connetti [!DNL Gmail] a [!DNL Workfront Fusion] {#connect-gmail-to-workfront-fusion}

* [Connetti [!DNL Gmail] a [!DNL Workfront Fusion] utilizzo di [!DNL G Suite]](#connect-gmail-to-workfront-fusion-usingg-suite)
* [Connetti [!DNL Gmail] a [!DNL Workfront Fusion] utilizzo [!DNL gmail.com] o [!DNL googlemail].com](#connect-gmail-to-workfront-fusion-using-gmailcom-or-googlemailcom)

### Connetti [!DNL Gmail] a [!DNL Workfront Fusion] utilizzo[!DNL  G Suite] {#connect-gmail-to-workfront-fusion-using-g-suite}

Per istruzioni sulla connessione [!DNL G Suite] account a [!UICONTROL Workfront Fusion], vedi [Connetti l’app o il servizio web del modulo a [!DNL Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md#connect) nell’articolo [Creare uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

### Connetti [!DNL Gmail] a [!DNL Workfront Fusion] utilizzo [!DNL gmail.com] o [!DNL googlemail].com {#connect-gmail-to-workfront-fusion-using-gmail-com-or-googlemail-com}

Se sei [!DNL @gmail.com] o [!DNL @googlemail.com] utente su cui è necessario creare un client OAuth [il [!DNL Google Cloud Platform]](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) al fine di ottenere un [!UICONTROL ID client] e [!UICONTROL Segreto client].

Per istruzioni dettagliate su come creare il client OAuth e ottenere un [!UICONTROL ID client] e [!UICONTROL Segreto client], vedi [Connettere Adobe Workfront Fusion a Google Services utilizzando un client OAuth personalizzato](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

## [!DNL Gmail] moduli e relativi campi

Quando si configura [!DNL Gmail] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL Gmail] I campi potrebbero essere visualizzati in base a fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se viene visualizzato il pulsante Mappa sopra un campo o una funzione, è possibile utilizzarlo per impostare variabili e funzioni per tale campo. Per ulteriori informazioni, consulta [Mappare le informazioni da un modulo all’altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Azioni](#actions)
* [Iteratori](#iterators)

### Triggers

#### [!UICONTROL Guarda le e-mail]

Questo modulo trigger esegue uno scenario quando viene ricevuto un nuovo messaggio e-mail da elaborare.

Il modulo restituisce tutti i campi standard associati al record o ai record, insieme a tutti i campi e i valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Gmail] account a [!DNL Workfront Fusion], vedi <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Gmail] a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Seleziona la cartella e-mail da guardare.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo di filtro] </td> 
   <td> <p>Seleziona il tipo di filtro da utilizzare per guardare le e-mail</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Simple filter]</strong> </p> <p>Compila i campi [!UICONTROL Criteri], [!UICONTROL Indirizzo e-mail mittente], [!UICONTROL Oggetto] e [!UICONTROL Frase di ricerca]</p> </li> 
     <li> <p> <strong>[!UICONTROL Gmail filter]</strong> </p> <p>Nel campo [!UICONTROL Query] immettere la query che si desidera utilizzare per filtrare le e-mail.</p> <p>Per ulteriori informazioni su [!DNL Gmail] filtri, vedi <a href="https://support.google.com/mail/answer/7190">Cerca operatori</a> nel [!DNL Gmail] documentazione.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Criteria]</td> 
   <td>Seleziona se desideri guardare le e-mail di [!UICONTROL all email], [!UICONTROL only read email] o [!UICONTROL only unread].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Indirizzo e-mail mittente]</td> 
   <td> <p> Immetti un indirizzo e-mail per controllare solo le e-mail inviate da tale indirizzo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Subject]</td> 
   <td>Inserisci una stringa di testo per guardare solo le e-mail che hanno quella stringa di testo nell’oggetto.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Frase di ricerca]</td> 
   <td>Inserisci una stringa di testo per guardare solo le e-mail che contengono tale stringa di testo in un punto qualsiasi dell’e-mail.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Contrassegna messaggi e-mail come letti al recupero]</td> 
   <td> <p> Abilita questa opzione per contrassegnare le e-mail recuperate come lette.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Numero massimo di risultati]</td> 
   <td> <p> Imposta il numero massimo di risultati che [!DNL Workfront Fusion] funzionerà con durante un ciclo.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Azioni

* [[!UICONTROL Inviare un’e-mail]](#send-an-email)
* [[!UICONTROL Creare una bozza]](#create-a-draft)
* [[!UICONTROL Contrassegna un messaggio e-mail come letto]](#mark-an-email-as-read)
* [[!UICONTROL Contrassegna un&#39;e-mail come non letta]](#mark-an-email-as-unread)
* [[!UICONTROL Spostare un’e-mail]](#move-an-email)
* [[!UICONTROL Copiare un messaggio e-mail]](#copy-an-email)
* [[!UICONTROL Eliminare un’e-mail]](#delete-an-email)
* [[!UICONTROL Modificare le etichette e-mail]](#modify-email-labels)

#### [!UICONTROL Inviare un’e-mail]

Questo modulo di azione invia una nuova e-mail.

Specifica il destinatario dell’e-mail.

Il modulo restituisce l’ID dell’e-mail e degli eventuali campi associati, insieme a eventuali campi e valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Gmail] account a [!DNL Workfront Fusion], vedi <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Gmail] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Da]</td> 
   <td> <p>Inserisci o mappa un indirizzo e-mail del mittente.</p> <p>Nota: se immetti un indirizzo e-mail errato, potrebbe verificarsi un errore durante l’invio di un messaggio, perché il tuo account potrebbe non disporre dell’autorizzazione per inviare e-mail da un indirizzo diverso dal tuo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL A] </td> 
   <td> <p>Clic <strong>[!UICONTROL Add]</strong>, quindi immetti o mappa l’indirizzo e-mail per ciascun destinatario.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Subject] </td> 
   <td> <p>Inserisci o mappa l’oggetto dell’e-mail.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Content] </td> 
   <td> <p>Inserisci o mappa il contenuto dell’e-mail (corpo del messaggio). I tag HTML sono consentiti.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Allegati] </td> 
   <td> <p>Clic <strong>[!UICONTROL Add]</strong> per aggiungere un allegato. È possibile mappare un file dai moduli precedenti.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Copia destinatari]</td> 
   <td> <p> Clic <strong>[!UICONTROL Add]</strong>, quindi immetti o mappa l’indirizzo e-mail per ciascun destinatario della copia.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Destinatari copia nascosta]</td> 
   <td> <p> Clic <strong>[!UICONTROL Add]</strong>, quindi immetti o mappa l’indirizzo e-mail per ciascun destinatario della copia nascosta.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Creare una bozza]

Questo modulo di azione crea una nuova bozza e-mail e la aggiunge a una cartella specificata.

Specificate la cartella in cui desiderate creare una bozza.

Il modulo restituisce l’ID della bozza e-mail e tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Gmail] account a [!DNL Workfront Fusion], vedi <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Gmail] a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Seleziona la [!DNL Gmail] cartella in cui si desidera creare una bozza.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL A] </td> 
   <td> <p>Clic <strong>[!UICONTROL Add]</strong>, quindi immetti o mappa l’indirizzo e-mail per ciascun destinatario.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Subject] </td> 
   <td> <p>Inserisci o mappa l’oggetto dell’e-mail.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Content] </td> 
   <td> <p>Inserisci o mappa il contenuto dell’e-mail (corpo del messaggio). I tag HTML sono consentiti.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Allegati] </td> 
   <td> <p>Clic <strong>[!UICONTROL Add]</strong> per aggiungere un allegato. È possibile mappare un file dai moduli precedenti.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Copia destinatari]</td> 
   <td> <p> Clic <strong>[!UICONTROL Add]</strong>, quindi immetti o mappa l’indirizzo e-mail per ciascun destinatario della copia.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Destinatari copia nascosta]</td> 
   <td> <p> Clic <strong>[!UICONTROL Add]</strong>, quindi immetti o mappa l’indirizzo e-mail per ciascun destinatario della copia nascosta.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Contrassegna un messaggio e-mail come letto]

Questo modulo di azione contrassegna un messaggio e-mail come letto.

Specifica l’ID dell’e-mail e della relativa cartella.

Il modulo restituisce l’ID dell’e-mail e degli eventuali campi associati, insieme a eventuali campi e valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Gmail] account a [!DNL Workfront Fusion], vedi <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Gmail] a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Seleziona la [!DNL Gmail] cartella contenente l’e-mail.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Email ID (UID)]</td> 
   <td> <p> Inserisci o mappa l’ID e-mail.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Contrassegna un&#39;e-mail come non letta]

Questo modulo di azione contrassegna un’e-mail o una bozza e-mail come non letta.

Specifica l’ID dell’e-mail e della relativa cartella.

Il modulo restituisce l’ID dell’e-mail e degli eventuali campi associati, insieme a eventuali campi e valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Gmail] account a [!DNL Workfront Fusion], vedi <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Gmail] a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Seleziona la [!DNL Gmail] cartella contenente l’e-mail.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Email ID (UID)] </td> 
   <td> <p>Inserisci o mappa l’ID e-mail dell’e-mail che desideri contrassegnare come non letta.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Spostare un’e-mail]

Questo modulo di azione sposta un’e-mail o una bozza e-mail in una cartella specificata.

Puoi specificare la cartella, la cartella di destinazione e l’ID dell’e-mail.

Il modulo restituisce l’ID dell’e-mail e degli eventuali campi associati, insieme a eventuali campi e valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Gmail] account a [!DNL Workfront Fusion], vedi <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Gmail] a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Seleziona la [!DNL Gmail] cartella di origine contenente l’e-mail che desideri spostare.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cartella di destinazione]</td> 
   <td> <p> Seleziona la [!DNL Gmail] cartella di destinazione in cui desideri spostare l’e-mail.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Email ID (UID)]</td> 
   <td> <p> Inserisci o mappa l’ID e-mail dell’e-mail che desideri spostare.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Copiare un messaggio e-mail]

Questo modulo di azione copia una bozza e-mail o e-mail in una cartella specificata.

Puoi specificare la cartella, la cartella di destinazione e l’ID dell’e-mail.

Il modulo restituisce l’ID dell’e-mail e degli eventuali campi associati, insieme a eventuali campi e valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Gmail] account a [!DNL Workfront Fusion], vedi <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Gmail] a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Seleziona la [!DNL Gmail] cartella di origine contenente l’e-mail che desideri copiare.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cartella di destinazione]</td> 
   <td> <p>Seleziona la [!DNL Gmail] cartella di destinazione in cui desideri copiare l’e-mail.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Email ID (UID)]</td> 
   <td> <p>Inserisci o mappa l’ID e-mail dell’e-mail da copiare.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminare un’e-mail]

Questo modulo di azione rimuove un’e-mail o una bozza e-mail da una cartella specificata.

Il modulo restituisce l’ID dell’e-mail e degli eventuali campi associati, insieme a eventuali campi e valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Gmail] account a [!DNL Workfront Fusion], vedi <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Gmail] a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL [!DNL Gmail] ID messaggio]</p> </td> 
   <td> <p>Inserisci o mappa l’ID e-mail dell’e-mail da eliminare.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL in modo permanente] </td> 
   <td> <p>Abilita questa opzione per consentire al modulo di eliminare definitivamente l’e-mail, invece di spostarla nella cartella del cestino.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Modificare le etichette e-mail]

Questo modulo di azione modifica l’etichetta di un messaggio e-mail specificato.

Il modulo restituisce l’ID dell’e-mail e degli eventuali campi associati, insieme a eventuali campi e valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Gmail] account a [!DNL Workfront Fusion], vedi <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Gmail] a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL [!DNL Gmail] ID messaggio]</td> 
   <td> <p> Inserisci o mappa l’ID e-mail dell’e-mail da eliminare.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Etichette da aggiungere]</p> </td> 
   <td> <p>Seleziona o mappa l’etichetta da aggiungere al messaggio e-mail selezionato.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL etichette da rimuovere]</td> 
   <td> <p> Seleziona o mappa l’etichetta da rimuovere dal messaggio e-mail selezionato.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>[!UICONTROL Etichetta da aggiungere] e [!UICONTROL Etichetta da rimuovere] I campi caricano solo le etichette create dall&#39;utente.

### Iteratori

#### [!UICONTROL Itera allegati]

È possibile iterare gli allegati e-mail. Ogni allegato è un bundle separato nell&#39;output del modulo. Per ulteriori informazioni, consulta [Modulo Iterator in Adobe Workfront Fusion](../../workfront-fusion/modules/iterator-module.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Modulo di origine] </td> 
   <td> <p>Selezionare il modulo da cui si desidera iterare gli allegati. </p> </td> 
  </tr> 
 </tbody> 
</table>
