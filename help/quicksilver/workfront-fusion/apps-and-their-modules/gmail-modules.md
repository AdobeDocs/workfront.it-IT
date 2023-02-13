---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli Gmail
description: In un [!DNL Adobe Workfront Fusion] In questo caso, puoi automatizzare i flussi di lavoro che utilizzano Gmail e collegarli a più applicazioni e servizi di terze parti.
author: Becky
feature: Workfront Fusion
exl-id: 1987156c-e003-4f99-8913-cb47f77efbfc
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1785'
ht-degree: 0%

---

# [!DNL Gmail] moduli

In un [!DNL Adobe Workfront Fusion] puoi automatizzare i flussi di lavoro che utilizzano [!DNL Gmail], nonché collegarlo a più applicazioni e servizi di terze parti.

Se hai bisogno di istruzioni su come creare uno scenario, vedi [Crea uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). Per informazioni sui moduli, consulta [Moduli in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

Per utilizzare [!DNL Gmail] moduli, è necessario disporre di un [!DNL Gmail] conto.

## Connetti [!DNL Gmail] a [!DNL Workfront Fusion] {#connect-gmail-to-workfront-fusion}

* [Connetti [!DNL Gmail] a [!DNL Workfront Fusion] utilizzo di [!DNL G Suite]](#connect-gmail-to-workfront-fusion-usingg-suite)
* [Connetti [!DNL Gmail] a [!DNL Workfront Fusion] utilizzo [!DNL gmail.com] o [!DNL googlemail].com](#connect-gmail-to-workfront-fusion-using-gmailcom-or-googlemailcom)

### Connetti [!DNL Gmail] a [!DNL Workfront Fusion] utilizzo[!DNL  G Suite] {#connect-gmail-to-workfront-fusion-using-g-suite}

Per istruzioni su come collegare le [!DNL G Suite] account a [!UICONTROL Workfront Fusion], vedi [Collega l’app o il servizio Web del modulo a [!DNL Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md#connect) nell&#39;articolo [Crea uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

### Connetti [!DNL Gmail] a [!DNL Workfront Fusion] utilizzo [!DNL gmail.com] o [!DNL googlemail].com {#connect-gmail-to-workfront-fusion-using-gmail-com-or-googlemail-com}

Se sei [!DNL @gmail.com] o [!DNL @googlemail.com] utente è necessario creare un client OAuth in [la [!DNL Google Cloud Platform]](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) per ottenere un [!UICONTROL ID client] e [!UICONTROL Segreto client].

Per istruzioni dettagliate su come creare il client OAuth e ottenere un [!UICONTROL ID client] e [!UICONTROL Segreto client], vedi [Connettere Adobe Workfront Fusion a Google Services utilizzando un client OAuth personalizzato](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

## [!DNL Gmail] moduli e relativi campi

Quando si configura [!DNL Gmail] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL Gmail] potrebbero essere visualizzati, a seconda di fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se trovi il pulsante mappa sopra un campo o una funzione, puoi utilizzarlo per impostare variabili e funzioni per quel campo. Per ulteriori informazioni, consulta [Mappare informazioni da un modulo a un altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Azioni](#actions)
* [Iteratori](#iterators)

### Triggers

#### [!UICONTROL Guarda le e-mail]

Questo modulo trigger esegue uno scenario in cui viene ricevuta una nuova e-mail da elaborare.

Il modulo restituisce tutti i campi standard associati al record o ai record, insieme a tutti i campi e i valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Gmail] account a [!DNL Workfront Fusion], vedi <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Gmail] a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cartella] </td> 
   <td> <p>Seleziona la cartella e-mail che desideri controllare.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo di filtro] </td> 
   <td> <p>Seleziona il tipo di filtro da utilizzare per guardare le e-mail</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Filtro semplice]</strong> </p> <p>Compila i campi [!UICONTROL Criteria], [!UICONTROL Sender Email Address], [!UICONTROL Subject] e [!UICONTROL Search Phrase]</p> </li> 
     <li> <p> <strong>[!UICONTROL Filtro Gmail]</strong> </p> <p>Nel campo Query [!UICONTROL] , inserisci la query da utilizzare per filtrare le e-mail.</p> <p>Per ulteriori informazioni su [!DNL Gmail] filtri, vedi <a href="https://support.google.com/mail/answer/7190">Operatori di ricerca</a> in [!DNL Gmail] documentazione.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Criteri di [!UICONTROL]</td> 
   <td>Seleziona se desideri guardare le e-mail di [!UICONTROL all e-mail], [!UICONTROL leggi solo le e-mail] o le e-mail di [!UICONTROL solo non lette].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Indirizzo e-mail mittente]</td> 
   <td> <p> Inserisci un indirizzo e-mail per visualizzare solo le e-mail inviate da tale indirizzo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Subject]</td> 
   <td>Immetti una stringa di testo per visualizzare solo le e-mail che contengono tale stringa di testo nell’oggetto.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Frase di ricerca]</td> 
   <td>Immetti una stringa di testo per visualizzare solo le e-mail che hanno quella stringa di testo in un punto qualsiasi dell’e-mail.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Segna i messaggi e-mail come letti al momento del recupero]</td> 
   <td> <p> Abilita questa opzione per contrassegnare le e-mail recuperate come lette.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Numero massimo di risultati]</td> 
   <td> <p> Imposta il numero massimo di risultati che [!DNL Workfront Fusion] funziona con durante un ciclo.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Azioni

* [[!UICONTROL Invia un messaggio e-mail]](#send-an-email)
* [[!UICONTROL Creare una bozza]](#create-a-draft)
* [[!UICONTROL Contrassegnare un messaggio e-mail come letto]](#mark-an-email-as-read)
* [[!UICONTROL Contrassegnare un messaggio e-mail come non letto]](#mark-an-email-as-unread)
* [[!UICONTROL Spostare un messaggio e-mail]](#move-an-email)
* [[!UICONTROL Copiare un messaggio e-mail]](#copy-an-email)
* [[!UICONTROL Eliminare un messaggio e-mail]](#delete-an-email)
* [[!UICONTROL Modificare le etichette e-mail]](#modify-email-labels)

#### [!UICONTROL Invia un messaggio e-mail]

Questo modulo di azione invia un nuovo messaggio e-mail.

Specifica il destinatario dell’e-mail.

Il modulo restituisce l’ID dell’e-mail e di tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Gmail] account a [!DNL Workfront Fusion], vedi <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Gmail] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL DA]</td> 
   <td> <p>Immetti o mappa un indirizzo e-mail del mittente.</p> <p>Nota: Se immetti un indirizzo e-mail non corretto, potrebbe verificarsi un errore durante l’invio di un messaggio perché il tuo account potrebbe non disporre dell’autorizzazione per l’invio di e-mail da un indirizzo diverso dal tuo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL A] </td> 
   <td> <p>Fai clic su <strong>[!UICONTROL Aggiungi]</strong>, quindi immetti o mappa l’indirizzo e-mail di ciascun destinatario.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Subject] </td> 
   <td> <p>Immetti o mappa l’oggetto dell’e-mail.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Content] </td> 
   <td> <p>Immetti o mappa il contenuto dell’e-mail (corpo del messaggio). I tag HTML sono consentiti.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Allegati] </td> 
   <td> <p>Fai clic su <strong>[!UICONTROL Aggiungi]</strong> per aggiungere un allegato. Puoi mappare un file dai moduli precedenti.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Copia destinatari]</td> 
   <td> <p> Fai clic su <strong>[!UICONTROL Aggiungi]</strong>, quindi immetti o mappa l’indirizzo e-mail per ciascun destinatario della copia.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Destinatari di copia cieca]</td> 
   <td> <p> Fai clic su <strong>[!UICONTROL Aggiungi]</strong>, quindi immetti o mappa l’indirizzo e-mail di ogni destinatario della copia cieca.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Creare una bozza]

Questo modulo di azione crea una nuova bozza e-mail e la aggiunge a una cartella specificata.

Specificate la cartella in cui desiderate creare una bozza.

Il modulo restituisce l’ID della bozza dell’e-mail e di tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Gmail] account a [!DNL Workfront Fusion], vedi <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Gmail] a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cartella] </td> 
   <td> <p>Seleziona la [!DNL Gmail] cartella in cui si desidera creare una bozza.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL A] </td> 
   <td> <p>Fai clic su <strong>[!UICONTROL Aggiungi]</strong>, quindi immetti o mappa l’indirizzo e-mail di ciascun destinatario.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Subject] </td> 
   <td> <p>Immetti o mappa l’oggetto dell’e-mail.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Content] </td> 
   <td> <p>Immetti o mappa il contenuto dell’e-mail (corpo del messaggio). I tag HTML sono consentiti.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Allegati] </td> 
   <td> <p>Fai clic su <strong>[!UICONTROL Aggiungi]</strong> per aggiungere un allegato. Puoi mappare un file dai moduli precedenti.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Copia destinatari]</td> 
   <td> <p> Fai clic su <strong>[!UICONTROL Aggiungi]</strong>, quindi immetti o mappa l’indirizzo e-mail per ciascun destinatario della copia.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Destinatari di copia cieca]</td> 
   <td> <p> Fai clic su <strong>[!UICONTROL Aggiungi]</strong>, quindi immetti o mappa l’indirizzo e-mail di ogni destinatario della copia cieca.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Contrassegnare un messaggio e-mail come letto]

Questo modulo di azione contrassegna un messaggio e-mail come letto.

Specifica l’ID dell’e-mail e la relativa cartella.

Il modulo restituisce l’ID dell’e-mail e di tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario .

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Gmail] account a [!DNL Workfront Fusion], vedi <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Gmail] a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cartella] </td> 
   <td> <p>Seleziona la [!DNL Gmail] cartella che contiene il messaggio e-mail.</p> </td> 
  </tr> 
  <tr> 
   <td>ID e-mail (UID)</td> 
   <td> <p> Immetti o mappa l’ID e-mail.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Contrassegnare un messaggio e-mail come non letto]

Questo modulo di azione contrassegna un’e-mail o una bozza di e-mail come non letta.

Specifica l’ID dell’e-mail e la relativa cartella.

Il modulo restituisce l’ID dell’e-mail e di tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario .

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Gmail] account a [!DNL Workfront Fusion], vedi <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Gmail] a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cartella] </td> 
   <td> <p>Seleziona la [!DNL Gmail] cartella che contiene il messaggio e-mail.</p> </td> 
  </tr> 
  <tr> 
   <td>ID e-mail (UID) </td> 
   <td> <p>Immetti o mappa l’ID e-mail dell’e-mail che desideri contrassegnare come non letto.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Spostare un messaggio e-mail]

Questo modulo di azione sposta un messaggio e-mail o una bozza e-mail in una cartella specificata.

Puoi specificare la cartella, la cartella di destinazione e l’ID dell’e-mail.

Il modulo restituisce l’ID dell’e-mail e di tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario .

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Gmail] account a [!DNL Workfront Fusion], vedi <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Gmail] a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cartella] </td> 
   <td> <p>Seleziona la [!DNL Gmail] cartella di origine contenente l'e-mail che si desidera spostare.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cartella di destinazione]</td> 
   <td> <p> Seleziona la [!DNL Gmail] cartella di destinazione in cui spostare il messaggio e-mail.</p> </td> 
  </tr> 
  <tr> 
   <td>ID e-mail (UID)</td> 
   <td> <p> Immetti o mappa l’ID e-mail dell’e-mail da spostare.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Copiare un messaggio e-mail]

Questo modulo di azione copia una bozza e-mail o e-mail in una cartella specificata.

Puoi specificare la cartella, la cartella di destinazione e l’ID dell’e-mail.

Il modulo restituisce l’ID dell’e-mail e di tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario .

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Gmail] account a [!DNL Workfront Fusion], vedi <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Gmail] a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cartella] </td> 
   <td> <p>Seleziona la [!DNL Gmail] cartella di origine che contiene l’e-mail da copiare.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cartella di destinazione]</td> 
   <td> <p>Seleziona la [!DNL Gmail] cartella di destinazione in cui copiare il messaggio e-mail.</p> </td> 
  </tr> 
  <tr> 
   <td>ID e-mail (UID)</td> 
   <td> <p>Immetti o mappa l’ID e-mail dell’e-mail da copiare.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminare un messaggio e-mail]

Questo modulo di azione rimuove un’e-mail o una bozza di e-mail da una cartella specificata.

Il modulo restituisce l’ID dell’e-mail e di tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Gmail] account a [!DNL Workfront Fusion], vedi <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Gmail] a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL [!DNL Gmail] ID messaggio]</p> </td> 
   <td> <p>Immetti o mappa l’ID e-mail dell’e-mail da eliminare.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Permanentemente] </td> 
   <td> <p>Abilita questa opzione per consentire al modulo di eliminare definitivamente l’e-mail, anziché spostarla nella cartella del cestino.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Modificare le etichette e-mail]

Questo modulo di azione modifica l’etichetta in un messaggio e-mail specificato.

Il modulo restituisce l’ID dell’e-mail e di tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Gmail] account a [!DNL Workfront Fusion], vedi <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Gmail] a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL [!DNL Gmail] ID messaggio]</td> 
   <td> <p> Immetti o mappa l’ID e-mail dell’e-mail da eliminare.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Etichette da aggiungere</p> </td> 
   <td> <p>Seleziona o mappa l’etichetta da aggiungere al messaggio e-mail selezionato.</p> </td> 
  </tr> 
  <tr> 
   <td>Etichette da rimuovere</td> 
   <td> <p> Seleziona o mappa l’etichetta da rimuovere dal messaggio e-mail selezionato.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>[!UICONTROL Etichetta da aggiungere] e [!UICONTROL Etichetta da rimuovere] i campi caricano solo le etichette create dall’utente.

### Iteratori

#### [!UICONTROL Itera allegati]

È possibile eseguire iterazioni degli allegati e-mail. Ogni allegato è un bundle separato nell&#39;output del modulo. Per ulteriori informazioni, consulta [Modulo iteratore in Adobe Workfront Fusion](../../workfront-fusion/modules/iterator-module.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Modulo di origine] </td> 
   <td> <p>Selezionare il modulo da cui si desidera eseguire l'iterazione degli allegati. </p> </td> 
  </tr> 
 </tbody> 
</table>
