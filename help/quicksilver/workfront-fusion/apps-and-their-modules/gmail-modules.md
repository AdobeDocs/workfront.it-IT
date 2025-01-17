---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli Gmail
description: La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione. Questo articolo è stato dichiarato obsoleto, ma contiene un collegamento al nuovo articolo che descrive questa funzionalità.
author: Becky
feature: Workfront Fusion
exl-id: 1987156c-e003-4f99-8913-cb47f77efbfc
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1873'
ht-degree: 0%

---

# [!DNL Gmail] moduli

>[!IMPORTANT]
>
>La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione.
>
>Le informazioni contenute in questo articolo sono ora disponibili nell’articolo:
>
>* [Moduli Gmail](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/gmail-modules.html)
>
>Aggiorna eventuali segnalibri.
>
>Questo articolo non è più in fase di aggiornamento e verrà rimosso nel prossimo futuro.

In uno scenario [!DNL Adobe Workfront Fusion], è possibile automatizzare i flussi di lavoro che utilizzano [!DNL Gmail] e collegarlo a più applicazioni e servizi di terze parti.

Se hai bisogno di istruzioni per la creazione di uno scenario, consulta [Creare uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). Per informazioni sui moduli, vedere [Moduli in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

Per utilizzare i moduli [!DNL Gmail], è necessario disporre di un account [!DNL Gmail].

## Connetti [!DNL Gmail] a [!DNL Workfront Fusion] {#connect-gmail-to-workfront-fusion}

* [Connetti [!DNL Gmail] a [!DNL Workfront Fusion] tramite [!DNL Google Workspace]](#connect-gmail-to-workfront-fusion-usingg-suite)
* [Connetti [!DNL Gmail] a [!DNL Workfront Fusion] utilizzando [!DNL gmail.com] or [!DNL googlemail].com](#connect-gmail-to-workfront-fusion-using-gmailcom-or-googlemailcom)

### Connetti [!DNL Gmail] a [!DNL Workfront Fusion] tramite [!DNL  Google Workspace] {#connect-gmail-to-workfront-fusion-using-g-suite}

Per istruzioni sulla connessione dell&#39;account [!DNL Google Workspace] a [!UICONTROL Workfront Fusion], vedere [Connettere l&#39;app o il servizio Web del modulo a [!DNL Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md#connect) nell&#39;articolo [Creare uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

### Connetti [!DNL Gmail] a [!DNL Workfront Fusion] tramite [!DNL gmail.com] o [!DNL googlemail].com {#connect-gmail-to-workfront-fusion-using-gmail-com-or-googlemail-com}

Se sei [!DNL @gmail.com] o [!DNL @googlemail.com] utente, devi creare un client OAuth su [the [!DNL Google Cloud Platform]](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) per ottenere un [!UICONTROL ID client] e un [!UICONTROL Segreto client].

Per istruzioni dettagliate su come creare il client OAuth e ottenere un [!UICONTROL ID client] e un [!UICONTROL segreto client], vedere [Connettere Adobe Workfront Fusion a Google Services utilizzando un client OAuth personalizzato](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

## [!DNL Gmail] moduli e relativi campi

Quando configuri [!DNL Gmail] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Insieme a questi, potrebbero essere visualizzati ulteriori campi di [!DNL Gmail], a seconda di fattori quali il livello di accesso nell&#39;app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se viene visualizzato il pulsante Mappa sopra un campo o una funzione, è possibile utilizzarlo per impostare variabili e funzioni per tale campo. Per ulteriori informazioni, vedere [Mappare le informazioni da un modulo all&#39;altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Azioni](#actions)
* [Iteratori](#iterators)

### Triggers

#### [!UICONTROL Controlla le e-mail]

Questo modulo trigger esegue uno scenario quando viene ricevuto un nuovo messaggio e-mail da elaborare.

Il modulo restituisce tutti i campi standard associati al record o ai record, insieme a tutti i campi e i valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Gmail] a [!DNL Workfront Fusion], vedere <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connettere [!DNL Gmail] a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Seleziona la cartella e-mail da guardare.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo di filtro] </td> 
   <td> <p>Seleziona il tipo di filtro da utilizzare per guardare le e-mail</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Filtro semplice]</strong> </p> <p>Compila i campi [!UICONTROL Criteri], [!UICONTROL Indirizzo e-mail mittente], [!UICONTROL Oggetto] e [!UICONTROL Frase di ricerca]</p> </li> 
     <li> <p> <strong>[!UICONTROL Gmail filter]</strong> </p> <p>Nel campo [!UICONTROL Query] immettere la query che si desidera utilizzare per filtrare le e-mail.</p> <p>Per ulteriori informazioni sui filtri [!DNL Gmail], vedere <a href="https://support.google.com/mail/answer/7190">Operatori di ricerca</a> nella documentazione di [!DNL Gmail].</p> </li> 
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
   <td> <p> Impostare il numero massimo di risultati con cui [!DNL Workfront Fusion] lavorerà durante un ciclo.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Azioni

* [[!UICONTROL Invia un&#39;e-mail]](#send-an-email)
* [[!UICONTROL Crea una bozza]](#create-a-draft)
* [[!UICONTROL Contrassegna un&#39;e-mail come già letta]](#mark-an-email-as-read)
* [[!UICONTROL Contrassegna un&#39;e-mail come non letta]](#mark-an-email-as-unread)
* [[!UICONTROL Spostare un&#39;e-mail]](#move-an-email)
* [[!UICONTROL Copia un&#39;e-mail]](#copy-an-email)
* [[!UICONTROL Eliminare un&#39;e-mail]](#delete-an-email)
* [[!UICONTROL Modifica etichette e-mail]](#modify-email-labels)

#### [!UICONTROL Invia un&#39;e-mail]

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
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Gmail] a [!DNL Workfront Fusion], vedere <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connessione di [!DNL Gmail] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Da]</td> 
   <td> <p>Inserisci o mappa un indirizzo e-mail del mittente.</p> <p>Nota: se immetti un indirizzo e-mail errato, potrebbe verificarsi un errore durante l’invio di un messaggio, perché il tuo account potrebbe non disporre dell’autorizzazione per inviare e-mail da un indirizzo diverso dal tuo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL A] </td> 
   <td> <p>Fai clic su <strong>[!UICONTROL Add]</strong>, quindi immetti o mappa l'indirizzo e-mail per ciascun destinatario.</p> </td> 
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
   <td> <p>Fare clic su <strong>[!UICONTROL Add]</strong> per aggiungere un allegato. È possibile mappare un file dai moduli precedenti.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Copia destinatari]</td> 
   <td> <p> Fai clic su <strong>[!UICONTROL Add]</strong>, quindi immetti o mappa l'indirizzo e-mail per ogni destinatario della copia.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Destinatari copia nascosta]</td> 
   <td> <p> Fai clic su <strong>[!UICONTROL Add]</strong>, quindi immetti o mappa l'indirizzo e-mail per ogni destinatario della copia nascosta.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crea una bozza]

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
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Gmail] a [!DNL Workfront Fusion], vedere <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connettere [!DNL Gmail] a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Selezionare la cartella [!DNL Gmail] in cui si desidera creare una bozza.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL A] </td> 
   <td> <p>Fai clic su <strong>[!UICONTROL Add]</strong>, quindi immetti o mappa l'indirizzo e-mail per ciascun destinatario.</p> </td> 
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
   <td> <p>Fare clic su <strong>[!UICONTROL Add]</strong> per aggiungere un allegato. È possibile mappare un file dai moduli precedenti.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Copia destinatari]</td> 
   <td> <p> Fai clic su <strong>[!UICONTROL Add]</strong>, quindi immetti o mappa l'indirizzo e-mail per ogni destinatario della copia.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Destinatari copia nascosta]</td> 
   <td> <p> Fai clic su <strong>[!UICONTROL Add]</strong>, quindi immetti o mappa l'indirizzo e-mail per ogni destinatario della copia nascosta.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Contrassegna un&#39;e-mail come già letta]

Questo modulo di azione contrassegna un messaggio e-mail come letto.

Specifica l’ID dell’e-mail e della relativa cartella.

Il modulo restituisce l’ID dell’e-mail e degli eventuali campi associati, insieme a eventuali campi e valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Gmail] a [!DNL Workfront Fusion], vedere <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connettere [!DNL Gmail] a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Selezionare la cartella [!DNL Gmail] che contiene l'e-mail.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID e-mail (UID)]</td> 
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
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Gmail] a [!DNL Workfront Fusion], vedere <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connettere [!DNL Gmail] a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Selezionare la cartella [!DNL Gmail] che contiene l'e-mail.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID e-mail (UID)] </td> 
   <td> <p>Inserisci o mappa l’ID e-mail dell’e-mail che desideri contrassegnare come non letta.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Spostare un&#39;e-mail]

Questo modulo di azione sposta un’e-mail o una bozza e-mail in una cartella specificata.

Puoi specificare la cartella, la cartella di destinazione e l’ID dell’e-mail.

Il modulo restituisce l’ID dell’e-mail e degli eventuali campi associati, insieme a eventuali campi e valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Gmail] a [!DNL Workfront Fusion], vedere <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connettere [!DNL Gmail] a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Selezionare la cartella di origine [!DNL Gmail] contenente l'e-mail che si desidera spostare.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cartella di destinazione]</td> 
   <td> <p> Selezionare la cartella di destinazione [!DNL Gmail] in cui si desidera spostare l'e-mail.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID e-mail (UID)]</td> 
   <td> <p> Inserisci o mappa l’ID e-mail dell’e-mail che desideri spostare.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Copia un&#39;e-mail]

Questo modulo di azione copia una bozza e-mail o e-mail in una cartella specificata.

Puoi specificare la cartella, la cartella di destinazione e l’ID dell’e-mail.

Il modulo restituisce l’ID dell’e-mail e degli eventuali campi associati, insieme a eventuali campi e valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Gmail] a [!DNL Workfront Fusion], vedere <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connettere [!DNL Gmail] a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Selezionare la cartella di origine [!DNL Gmail] contenente l'e-mail che si desidera copiare.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cartella di destinazione]</td> 
   <td> <p>Selezionare la cartella di destinazione [!DNL Gmail] in cui copiare l'e-mail.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID e-mail (UID)]</td> 
   <td> <p>Inserisci o mappa l’ID e-mail dell’e-mail da copiare.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminare un&#39;e-mail]

Questo modulo di azione rimuove un’e-mail o una bozza e-mail da una cartella specificata.

Il modulo restituisce l’ID dell’e-mail e degli eventuali campi associati, insieme a eventuali campi e valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Gmail] a [!DNL Workfront Fusion], vedere <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connettere [!DNL Gmail] a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td> 
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

#### [!UICONTROL Modifica etichette e-mail]

Questo modulo di azione modifica l’etichetta di un messaggio e-mail specificato.

Il modulo restituisce l’ID dell’e-mail e degli eventuali campi associati, insieme a eventuali campi e valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Gmail] a [!DNL Workfront Fusion], vedere <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connettere [!DNL Gmail] a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td> 
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
>[!UICONTROL Etichetta da aggiungere] e [!UICONTROL Etichetta da rimuovere] campi caricano solo le etichette create dall&#39;utente.

### Iteratori

#### [!UICONTROL Itera allegati]

È possibile iterare gli allegati e-mail. Ogni allegato è un bundle separato nell&#39;output del modulo. Per ulteriori informazioni, vedere [Modulo Iterator in Adobe Workfront Fusion](../../workfront-fusion/modules/iterator-module.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Modulo Source] </td> 
   <td> <p>Selezionare il modulo da cui si desidera iterare gli allegati. </p> </td> 
  </tr> 
 </tbody> 
</table>
