---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: apps-and-their-modules
title: E-mail Microsoft Office 365
description: In uno scenario  [!DNL Adobe Workfront Fusion] , è possibile automatizzare i flussi di lavoro che utilizzano Microsoft Office 365 Email, nonché collegarlo a più applicazioni e servizi di terze parti.
author: Becky
feature: Workfront Fusion
exl-id: 29b69e8c-a889-441e-a052-287f1db2052d
source-git-commit: 7e7294e52622a6b8164fc69bbb4be576cc113f63
workflow-type: tm+mt
source-wordcount: '2699'
ht-degree: 0%

---

# [!DNL Microsoft Office 365 Email] moduli

In uno scenario [!DNL Adobe Workfront Fusion], è possibile automatizzare i flussi di lavoro che utilizzano [!UICONTROL E-mail di Microsoft Office 365], nonché collegarlo a più applicazioni e servizi di terze parti.

Per utilizzare [!UICONTROL E-mail Office 365] con [!DNL Adobe Workfront Fusion], è necessario disporre di un account [!UICONTROL Office 365]. Puoi crearne uno all’indirizzo www.office.com.

Per istruzioni sulla connessione dell&#39;account [!UICONTROL Office 365] a [!DNL Workfront Fusion], vedere [Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base](../../workfront-fusion/connections/connect-to-fusion-general.md)

Dopo aver concesso il consenso, verrai reindirizzato alla pagina di amministrazione [!UICONTROL Workfront Fusion] in cui potrai continuare a creare lo scenario.

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

Per utilizzare i moduli [!DNL Microsoft Office 365 Email], è necessario disporre di un account [!DNL Microsoft Office 365 Email].



## Connessione del servizio [!DNL Office 365 Email] a [!DNL Workfront Fusion]

Per istruzioni sulla connessione dell&#39;account [!DNL Office 365 Email] a [!UICONTROL Workfront Fusion], vedere [Creare una connessione a [!UICONTROL Adobe Workfront Fusion] - Istruzioni di base](../../workfront-fusion/connections/connect-to-fusion-general.md)

>[!NOTE]
>
>Alcune app Microsoft utilizzano la stessa connessione, che è associata alle autorizzazioni dei singoli utenti. Pertanto, durante la creazione di una connessione, nella schermata di consenso delle autorizzazioni vengono visualizzate tutte le autorizzazioni concesse in precedenza alla connessione dell’utente, oltre alle nuove autorizzazioni necessarie per l’applicazione corrente.
>
>Ad esempio, se un utente dispone delle autorizzazioni &quot;Leggi tabella&quot; concesse tramite il connettore Excel e quindi crea una connessione nel connettore Outlook per leggere le e-mail, nella schermata di consenso delle autorizzazioni verranno visualizzate sia l’autorizzazione &quot;Leggi tabella&quot; già concessa che l’autorizzazione &quot;Scrivi e-mail&quot; appena richiesta.

## [!DNL Microsoft Office 365 Email] moduli e relativi campi

Quando configuri [!DNL Microsoft Office 365 Email] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Insieme a questi, potrebbero essere visualizzati ulteriori campi di [!DNL Microsoft Office 365 Email], a seconda di fattori quali il livello di accesso nell&#39;app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se viene visualizzato il pulsante Mappa sopra un campo o una funzione, è possibile utilizzarlo per impostare variabili e funzioni per tale campo. Per ulteriori informazioni, vedere [Mappare le informazioni da un modulo all&#39;altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Messaggio](#message)
* [Bozza di messaggio](#draft-message)
* [Allegato](#attachment)
* [Altro](#other)

### Messaggio

* [[!UICONTROL Crea e invia un messaggio (legacy)]](#create-and-send-a-message)
* [[!UICONTROL Elimina messaggio]](#delete-a-message)
* [[!UICONTROL Ricevi un messaggio]](#get-a-message)
* [[!UICONTROL Sposta un messaggio]](#move-a-message)
* [[!UICONTROL Cerca messaggi]](#search-messages)
* [[!UICONTROL Messaggi da guardare]](#watch-messages)



#### [!UICONTROL Crea e invia un messaggio (legacy)]

Crea e invia un messaggio e-mail.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Office 365] a [!DNL Workfront Fusion], vedere <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject]</td> 
   <td> <p>Inserisci o mappa l’oggetto del messaggio.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Tipo di contenuto corpo]</td> 
   <td>Seleziona se il contenuto del corpo del messaggio è HTML o Text.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contenuto corpo]</td> 
   <td> <p>Inserisci o mappa il testo del corpo del messaggio dell’e-mail.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importance]</td> 
   <td> <p>Seleziona l’importanza dell’e-mail</p> 
    <ul> 
     <li>[!UICONTROL Minimo]</li> 
     <li>[!UICONTROL Normale]</li> 
     <li>[!UICONTROL alto]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Per Destinatari]</p> </td> 
   <td> <p>Aggiungi l’indirizzo e-mail al quale desideri inviare i messaggi:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nome]</strong> </p> <p>Inserisci il nome del contatto</p> </li> 
     <li> <p><strong>[!UICONTROL Indirizzo E-Mail]</strong> </p> <p>Inserisci l’indirizzo e-mail del contatto.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL CC Recipients]</p> </td> 
   <td> <p>Aggiungi i destinatari a cui vuoi inviare una copia del messaggio:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nome]</strong> </p> <p>Inserisci il nome del contatto</p> </li> 
     <li> <p><strong>[!UICONTROL Indirizzo E-Mail]</strong> </p> <p>Inserisci l’indirizzo e-mail del contatto.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Destinatari Ccn]</p> </td> 
   <td> <p>Aggiungi i destinatari da copiare nel messaggio, senza consentire ad altri destinatari di visualizzare i propri nomi o indirizzi e-mail:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nome]</strong> </p> <p>Inserisci il nome del contatto</p> </li> 
     <li> <p><strong>[!UICONTROL Indirizzo E-Mail]</strong> </p> <p>Inserisci l’indirizzo e-mail del contatto.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Allegati]</p> </td> 
   <td> <p>Aggiungi gli allegati all’e-mail:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nome file]</strong> </p> <p>Immettere il nome del file. Esempio: <code>sample.doc</code></p> </li> 
     <li> <p><strong>[!UICONTROL Dati]</strong> </p> <p>Immetti i dati del file nel campo o mappa l’origine del file.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Intestazioni messaggi Internet]</td> 
   <td> <p>Aggiungi le intestazioni del messaggio per l’e-mail.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nome]</strong> </p> <p>Inserisci il nome dell’intestazione</p> </li> 
     <li> <p><strong>[!UICONTROL Indirizzo E-Mail]</strong> </p> <p>Immettere un valore per l'intestazione.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crea e invia un messaggio]

Crea e invia un messaggio e-mail.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Office 365] a [!DNL Workfront Fusion], vedere <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject]</td> 
   <td> <p>Inserisci o mappa l’oggetto del messaggio.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Tipo di contenuto corpo]</td> 
   <td>Seleziona se il contenuto del corpo del messaggio è HTML o Text.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contenuto corpo]</td> 
   <td> <p>Inserisci o mappa il testo del corpo del messaggio dell’e-mail.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importance]</td> 
   <td> <p>Seleziona l’importanza dell’e-mail</p> 
    <ul> 
     <li>[!UICONTROL Minimo]</li> 
     <li>[!UICONTROL Normale]</li> 
     <li>[!UICONTROL alto]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Per Destinatari]</p> </td> 
   <td> <p>Aggiungi l’indirizzo e-mail al quale desideri inviare i messaggi:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nome]</strong> </p> <p>Inserisci il nome del contatto</p> </li> 
     <li> <p><strong>[!UICONTROL Indirizzo E-Mail]</strong> </p> <p>Inserisci l’indirizzo e-mail del contatto.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL CC Recipients]</p> </td> 
   <td> <p>Aggiungi i destinatari a cui vuoi inviare una copia del messaggio:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nome]</strong> </p> <p>Inserisci il nome del contatto</p> </li> 
     <li> <p><strong>[!UICONTROL Indirizzo E-Mail]</strong> </p> <p>Inserisci l’indirizzo e-mail del contatto.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Destinatari Ccn]</p> </td> 
   <td> <p>Aggiungi i destinatari da copiare nel messaggio, senza consentire ad altri destinatari di visualizzare i propri nomi o indirizzi e-mail:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nome]</strong> </p> <p>Inserisci il nome del contatto</p> </li> 
     <li> <p><strong>[!UICONTROL Indirizzo E-Mail]</strong> </p> <p>Inserisci l’indirizzo e-mail del contatto.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Allegati]</p> </td> 
   <td> <p>Aggiungi gli allegati all’e-mail:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nome file]</strong> </p> <p>Immettere il nome del file. Esempio: <code>sample.doc</code></p> </li> 
     <li> <p><strong>[!UICONTROL Dati]</strong> </p> <p>Immetti i dati del file nel campo o mappa l’origine del file.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Intestazioni messaggi Internet]</td> 
   <td> <p>Aggiungi le intestazioni del messaggio per l’e-mail.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nome]</strong> </p> <p>Inserisci il nome dell’intestazione</p> </li> 
     <li> <p><strong>[!UICONTROL Indirizzo E-Mail]</strong> </p> <p>Immettere un valore per l'intestazione.</p> </li> 
    </ul> </td> 
  </tr> 
   <td role="rowheader">[!UICONTROL Da indirizzo e-mail]</td> 
   <td> <p> Per utilizzare un indirizzo e-mail condiviso, immetti qui l’indirizzo. L'utente le cui credenziali vengono utilizzate nella connessione utilizzata per questo modulo deve avere accesso alla cartella condivisa.<p>Lascia vuoto questo campo per usare l’indirizzo e-mail del proprietario della connessione.</p></p> </td> 
  </tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Immettere o mappare il numero massimo di record che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Elimina messaggio]

Elimina un messaggio e-mail esistente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Office 365] a [!DNL Workfront Fusion], vedere <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Da indirizzo e-mail]</td> 
   <td> <p> Per utilizzare un indirizzo e-mail condiviso, immetti qui l’indirizzo. L'utente le cui credenziali vengono utilizzate nella connessione utilizzata per questo modulo deve avere accesso alla cartella condivisa.<p>Lascia vuoto questo campo per usare l’indirizzo e-mail del proprietario della connessione.</p></p> </td> 
  </tr> 
   <td role="rowheader">[!UICONTROL ID messaggio]</td> 
   <td> <p> Seleziona o mappa l’ID del messaggio da eliminare.</p> </td> 
  </tr> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ricevi un messaggio]

Ottiene i metadati di un messaggio specifico

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Office 365] a [!DNL Workfront Fusion], vedere <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Da indirizzo e-mail]</td> 
   <td> <p> Per utilizzare un indirizzo e-mail condiviso, immetti qui l’indirizzo. L'utente le cui credenziali vengono utilizzate nella connessione utilizzata per questo modulo deve avere accesso alla cartella condivisa.<p>Lascia vuoto questo campo per usare l’indirizzo e-mail del proprietario della connessione.</p></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID messaggio]</td> 
   <td> <p> Seleziona o mappa l’ID del messaggio per cui desideri recuperare i metadati.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL - Ottieni contenuti MIME]</td> 
   <td>Abilita questa opzione per recuperare i dati sul contenuto MIME del messaggio. Il contenuto [!UICONTROL MIME] può includere immagini, audio, video o altri tipi di file.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Sposta un messaggio]

Sposta un messaggio e-mail in una cartella selezionata nella cassetta postale.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Office 365] a [!DNL Workfront Fusion], vedere <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID messaggio]</td> 
   <td> <p> Seleziona o mappa l’ID del messaggio da spostare in un’altra cartella.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL cartella di posta] </td> 
   <td> <p>Seleziona o mappa l’ID della cartella in cui desideri spostare il messaggio.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Cerca messaggi]

Cerca i messaggi in base a criteri specifici.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Office 365] a [!DNL Workfront Fusion], vedere <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL Da indirizzo e-mail]</td> 
   <td> <p> Per utilizzare un indirizzo e-mail condiviso, immetti qui l’indirizzo. L'utente le cui credenziali vengono utilizzate nella connessione utilizzata per questo modulo deve avere accesso alla cartella condivisa.<p>Lascia vuoto questo campo per usare l’indirizzo e-mail del proprietario della connessione.</p></p> </td> 
  </tr> 
<tr> 
   <td role="rowheader">[!UICONTROL cartella di posta]</td> 
   <td> <p>Selezionare la cartella contenente i messaggi che si desidera cercare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL - Ricerca]</td> 
   <td>Immettere la query di ricerca. Per informazioni su come scrivere una query di ricerca, vedere l'articolo di supporto [!DNL Microsoft] <a href="https://support.microsoft.com/en-us/office/search-mail-and-people-in-outlook-com-88108edf-028e-4306-b87e-7400bbb40aa7?ui=en-us&amp;rs=en-us&amp;ad=us">Cerca posta e persone in [!DNL Outlook.com]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordina per]</td> 
   <td> <p>Selezionare la modalità di ordinamento dei risultati:</p> 
    <ul> 
     <li>[!UICONTROL Subject (Crescente o Decrescente)]</li> 
     <li>Data e ora di creazione [!UICONTROL (crescente o decrescente)]</li> 
     <li>[!UICONTROL Data e ora ultima modifica (crescente o decrescente)]</li> 
     <li>[!UICONTROL Received Date Time (Ascending o descending)]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Immettere il numero massimo di messaggi che [!DNL Workfront Fusion] deve restituire durante un ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Messaggi da guardare]

Si attiva quando viene inviato o ricevuto un nuovo messaggio e-mail.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Office 365] a [!DNL Workfront Fusion], vedere <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Guarda i messaggi]</p> </td> 
   <td> <p>Seleziona i messaggi da guardare:</p> 
    <ul> 
     <li>[!UICONTROL Solo Non Letto]</li> 
     <li>[!UICONTROL Only read]</li> 
     <li>[!UICONTROL Tutto]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL cartella di posta]</td> 
   <td> <p>Selezionare la cartella contenente i messaggi che si desidera controllare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL - Ricerca]</td> 
   <td>Immettere la query di ricerca. Per informazioni su come scrivere una query di ricerca, vedere l'articolo di supporto [!DNL Microsoft] <a href="https://support.microsoft.com/en-us/office/search-mail-and-people-in-outlook-com-88108edf-028e-4306-b87e-7400bbb40aa7?ui=en-us&amp;rs=en-us&amp;ad=us">Cerca posta e persone in [!DNL Outlook.com]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Immettere il numero massimo di messaggi che [!DNL Workfront Fusion] deve restituire durante un ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Bozza di messaggio

* [Creare una bozza di messaggio](#create-a-draft-message)
* [Invia una bozza di messaggio](#send-a-draft-message)
* [Aggiornare un messaggio](#update-a-message)

#### [!UICONTROL Crea bozza messaggio]

Crea un nuovo messaggio e-mail.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Office 365] a [!DNL Workfront Fusion], vedere <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject]</td> 
   <td> <p>Immettere l'oggetto del messaggio.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di contenuto corpo]</td> 
   <td>Seleziona se il contenuto del corpo del messaggio è HTML o Text.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contenuto corpo]</td> 
   <td> <p>Inserisci il testo del corpo del messaggio dell’e-mail.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importance]</td> 
   <td> <p>Seleziona l’importanza dell’e-mail</p> 
    <ul> 
     <li>[!UICONTROL Minimo]</li> 
     <li>[!UICONTROL Normale]</li> 
     <li>[!UICONTROL alto]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Per Destinatari]</p> </td> 
   <td> <p>Aggiungi i destinatari a cui vuoi inviare i messaggi:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nome]</strong> </p> <p>Inserisci il nome del contatto</p> </li> 
     <li> <p><strong>[!UICONTROL Indirizzo E-Mail]</strong> </p> <p>Inserisci l’indirizzo e-mail del contatto.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL CC Recipients]</p> </td> 
   <td> <p>Aggiungi i destinatari Desideri ricevere una copia del messaggio:</p> 
    <ul> 
     <li> <p><strong>Nome</strong> </p> <p>Inserisci il nome del contatto</p> </li> 
     <li> <p><strong>Indirizzo e-mail</strong> </p> <p>Inserisci l’indirizzo e-mail del contatto.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Destinatari Ccn</p> </td> 
   <td> <p>Aggiungi i destinatari da copiare nel messaggio, senza consentire ad altri destinatari di visualizzare i propri nomi o indirizzi e-mail:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nome]</strong> </p> <p>Inserisci il nome del contatto</p> </li> 
     <li> <p><strong>[!UICONTROL Indirizzo E-Mail]</strong> </p> <p>Inserisci l’indirizzo e-mail del contatto.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Allegati]</p> </td> 
   <td> <p>Aggiungi gli allegati all’e-mail:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nome file]</strong> </p> <p>Immettere il nome del file. Esempio: <code>sample.doc</code></p> </li> 
     <li> <p><strong>[!UICONTROL Dati]</strong> </p> <p>Immetti i dati del file nel campo o mappa l’origine del file.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Da indirizzo e-mail]</td> 
   <td> <p> Per utilizzare un indirizzo e-mail condiviso, immetti qui l’indirizzo. L'utente le cui credenziali vengono utilizzate nella connessione utilizzata per questo modulo deve avere accesso alla cartella condivisa.<p>Lascia vuoto questo campo per usare l’indirizzo e-mail del proprietario della connessione.</p></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Invia una bozza di messaggio]

Invia un messaggio e-mail attualmente in bozza.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Office 365] a [!DNL Workfront Fusion], vedere <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Da indirizzo e-mail]</td> 
   <td> <p> Per utilizzare un indirizzo e-mail condiviso, immetti qui l’indirizzo. L'utente le cui credenziali vengono utilizzate nella connessione utilizzata per questo modulo deve avere accesso alla cartella condivisa.<p>Lascia vuoto questo campo per usare l’indirizzo e-mail del proprietario della connessione.</p></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID bozza messaggio]</td> 
   <td> <p> Seleziona o mappa l’ID messaggio della bozza da inviare.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggiorna un messaggio]

Aggiorna un messaggio esistente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Office 365] a [!DNL Workfront Fusion], vedere <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Da indirizzo e-mail]</td> 
   <td> <p> Per utilizzare un indirizzo e-mail condiviso, immetti qui l’indirizzo. L'utente le cui credenziali vengono utilizzate nella connessione utilizzata per questo modulo deve avere accesso alla cartella condivisa.<p>Lascia vuoto questo campo per usare l’indirizzo e-mail del proprietario della connessione.</p></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inserisci un ID messaggio]</td> 
   <td> <p>Seleziona la modalità di identificazione del messaggio da aggiornare:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Immetti Manualmente]</strong> </p> <p>Inserisci o mappa l’ID del messaggio.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleziona dall'elenco]</strong> </p> <p>Seleziona la cartella contenente il messaggio da aggiornare, quindi fai clic sul messaggio</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject]</td> 
   <td> <p>Immettere l'oggetto del messaggio.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contenuto corpo]</td> 
   <td> <p>Inserisci il testo del corpo del messaggio dell’e-mail.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importance]</td> 
   <td> <p>Seleziona l’importanza dell’e-mail</p> 
    <ul> 
     <li>[!UICONTROL Minimo]</li> 
     <li>[!UICONTROL Normale]</li> 
     <li>[!UICONTROL alto]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Per Destinatari]</p> </td> 
   <td> <p>Aggiungi l’indirizzo e-mail al quale desideri inviare i messaggi:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nome]</strong> </p> <p>Inserisci il nome del contatto</p> </li> 
     <li> <p><strong>[!UICONTROL Indirizzo E-Mail]</strong> </p> <p>Inserisci l’indirizzo e-mail del contatto.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL CC Recipients]</p> </td> 
   <td> <p>Aggiungi i destinatari Desideri ricevere una copia del messaggio:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nome]</strong> </p> <p>Inserisci il nome del contatto</p> </li> 
     <li> <p><strong>[!UICONTROL Indirizzo E-Mail]</strong> </p> <p>Inserisci l’indirizzo e-mail del contatto.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Destinatari Ccn]</p> </td> 
   <td> <p>Aggiungi i destinatari da copiare nel messaggio, senza consentire ad altri destinatari di visualizzare i propri nomi o indirizzi e-mail:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nome]</strong> </p> <p>Inserisci il nome del contatto</p> </li> 
     <li> <p><strong>[!UICONTROL Indirizzo E-Mail]</strong> </p> <p>Inserisci l’indirizzo e-mail del contatto.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Allegati]</p> </td> 
   <td> <p>Aggiungi gli allegati all’e-mail:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nome file]</strong> </p> <p>Immettere il nome del file. Esempio: <code>sample.doc</code></p> </li> 
     <li> <p><strong>[!UICONTROL Dati]</strong> </p> <p>Immetti i dati del file nel campo o mappa l’origine del file.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contrassegnalo come letto]</td> 
   <td>Abilita questa opzione per contrassegnare il messaggio aggiornato come letto.</td> 
  </tr> 
 </tbody> 
</table>

### Allegato

* [[!UICONTROL Scarica un allegato]](#download-an-attachment)
* [[!UICONTROL Elenca allegati]](#list-attachments)

#### [!UICONTROL Scarica un allegato]

Questo modulo scarica l’allegato specificato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Office 365] a [!DNL Workfront Fusion], vedere <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Da indirizzo e-mail]</td> 
   <td> <p> Per utilizzare un indirizzo e-mail condiviso, immetti qui l’indirizzo. L'utente le cui credenziali vengono utilizzate nella connessione utilizzata per questo modulo deve avere accesso alla cartella condivisa.<p>Lascia vuoto questo campo per usare l’indirizzo e-mail del proprietario della connessione.</p></p> </td> 
  </tr> 
   <td role="rowheader">[!UICONTROL ID messaggio]</td> 
   <td> <p> Seleziona o mappa l’ID del messaggio che contiene l’allegato da scaricare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID allegato]</td> 
   <td> <p>Immetti o mappa l’ID dell’allegato da scaricare.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Elenca allegati]

Questo modulo recupera un elenco di allegati appartenenti al messaggio specificato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Office 365] a [!DNL Workfront Fusion], vedere <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Da indirizzo e-mail]</td> 
   <td> <p> Per utilizzare un indirizzo e-mail condiviso, immetti qui l’indirizzo. L'utente le cui credenziali vengono utilizzate nella connessione utilizzata per questo modulo deve avere accesso alla cartella condivisa.<p>Lascia vuoto questo campo per usare l’indirizzo e-mail del proprietario della connessione.</p></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID messaggio]</td> 
   <td> <p> Seleziona o mappa l’ID del messaggio da cui desideri recuperare gli allegati.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Immettere o mappare il numero massimo di allegati che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Altro

* [[!UICONTROL Aggiungi un allegato]](#add-an-attachment)
  <!--Create and send a message-->
* [[!UICONTROL Effettuare una chiamata API]](#make-an-api-call)

#### [!UICONTROL Aggiungi un allegato]

Questo modulo aggiunge un allegato di grandi dimensioni a un messaggio.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Office 365] a [!DNL Workfront Fusion], vedere <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Da indirizzo e-mail]</td> 
   <td> <p> Per utilizzare un indirizzo e-mail condiviso, immetti qui l’indirizzo. L'utente le cui credenziali vengono utilizzate nella connessione utilizzata per questo modulo deve avere accesso alla cartella condivisa.<p>Lascia vuoto questo campo per usare l’indirizzo e-mail del proprietario della connessione.</p></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID messaggio]</td> 
   <td> <p> Seleziona o mappa l’ID del messaggio a cui desideri aggiungere un allegato.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Selezionare un file da un modulo precedente o mappare il nome e i dati del file di origine.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Effettuare una chiamata API]

Questo modulo ti consente di eseguire una chiamata API personalizzata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Office 365] a [!DNL Workfront Fusion], vedere <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Immettere un percorso relativo a <code>https://graph.microsoft.com</code>. Esempio:<code> /v1.0/me/messages</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Method]</p> </td> 
   td&gt; <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, vedere <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Aggiungi le intestazioni della richiesta sotto forma di oggetto JSON standard. Ad esempio, <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] aggiunge le intestazioni di autorizzazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Stringa Di Query]</td> 
   <td> <p> Aggiungi la query per la chiamata API sotto forma di oggetto JSON standard.</p> </td> 
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
