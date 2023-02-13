---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: apps-and-their-modules
title: E-mail Microsoft Office 365
description: In un [!DNL Adobe Workfront Fusion] In questo caso, è possibile automatizzare i flussi di lavoro che utilizzano e-mail Microsoft Office 365 e collegarli a più applicazioni e servizi di terze parti.
author: Becky
feature: Workfront Fusion
exl-id: 29b69e8c-a889-441e-a052-287f1db2052d
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1838'
ht-degree: 0%

---

# [!DNL Microsoft Office 365 Email]

In un [!DNL Adobe Workfront Fusion] puoi automatizzare i flussi di lavoro che utilizzano [!UICONTROL E-mail Microsoft Office 365], nonché collegarlo a più applicazioni e servizi di terze parti.

Per utilizzare [!UICONTROL E-mail Office 365] con [!DNL Adobe Workfront Fusion], è necessario disporre di un [!UICONTROL Account Office 365]. Puoi crearne uno all’indirizzo www.office.com.

Per istruzioni su come collegare le [!UICONTROL Office 365] account a [!DNL Workfront Fusion], vedi [Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base](../../workfront-fusion/connections/connect-to-fusion-general.md)

Dopo aver concesso il consenso, vieni reindirizzato nuovamente al [!UICONTROL Workfront Fusion] pagina di amministrazione in cui puoi continuare a creare lo scenario.

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

Per utilizzare [!DNL Microsoft Office 365 Email] moduli, è necessario disporre di un [!DNL Microsoft Office 365 Email] conto.

## [!DNL Microsoft Office 365 Email] moduli e relativi campi

Quando si configura [!DNL Microsoft Office 365 Email] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL Microsoft Office 365 Email] potrebbero essere visualizzati, a seconda di fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se trovi il pulsante mappa sopra un campo o una funzione, puoi utilizzarlo per impostare variabili e funzioni per quel campo. Per ulteriori informazioni, consulta [Mappare informazioni da un modulo a un altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Messaggio](#message)
* [Messaggio bozza](#draft-message)
* [Allegato](#attachment)
* [Altro](#other)

### Messaggio

* [[!UICONTROL Messaggi di controllo]](#watch-messages)
* [[!UICONTROL Messaggi di ricerca]](#search-messages)
* [[!UICONTROL Ottieni un messaggio]](#get-a-message)
* [[!UICONTROL Creare e inviare un messaggio]](#create-and-send-a-message)
* [[!UICONTROL Spostare un messaggio]](#move-a-message)
* [[!UICONTROL Eliminare un messaggio]](#delete-a-message)

#### [!UICONTROL Messaggi di controllo]

Attiva quando viene inviato o ricevuto un nuovo messaggio e-mail.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Guarda i messaggi]</p> </td> 
   <td> <p>Seleziona i messaggi da visualizzare:</p> 
    <ul> 
     <li>[!UICONTROL Solo non letto]</li> 
     <li>[!UICONTROL Solo lettura]</li> 
     <li>[!UICONTROL ALL]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cartella Posta Elettronica]</td> 
   <td> <p>Selezionare la cartella contenente i messaggi che si desidera controllare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Search]</td> 
   <td>Inserisci la query di ricerca. Per informazioni su come scrivere una query di ricerca, consulta la [!DNL Microsoft] articolo di supporto <a href="https://support.microsoft.com/en-us/office/search-mail-and-people-in-outlook-com-88108edf-028e-4306-b87e-7400bbb40aa7?ui=en-us&amp;rs=en-us&amp;ad=us">Cerca e-mail e persone in [!DNL Outlook.com]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Immettere il numero massimo di messaggi [!DNL Workfront Fusion] dovrebbe essere restituito durante un ciclo di esecuzione di uno scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Messaggi di ricerca]

Cerca i messaggi in base a criteri specifici.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cartella Posta Elettronica]</td> 
   <td> <p>Selezionare la cartella contenente i messaggi da cercare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Search]</td> 
   <td>Inserisci la query di ricerca. Per informazioni su come scrivere una query di ricerca, consulta la [!DNL Microsoft] articolo di supporto <a href="https://support.microsoft.com/en-us/office/search-mail-and-people-in-outlook-com-88108edf-028e-4306-b87e-7400bbb40aa7?ui=en-us&amp;rs=en-us&amp;ad=us">Cerca e-mail e persone in [!DNL Outlook.com]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordina per]</td> 
   <td> <p>Seleziona la modalità di ordinamento dei risultati:</p> 
    <ul> 
     <li>[!UICONTROL Oggetto (crescente o decrescente)]</li> 
     <li>[!UICONTROL Data e ora di creazione (crescente o decrescente)]</li> 
     <li>[!UICONTROL Data ultima modifica (crescente o decrescente)]</li> 
     <li>[!UICONTROL Data e ora di ricezione (crescente o decrescente)]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Immettere il numero massimo di messaggi [!DNL Workfront Fusion] dovrebbe essere restituito durante un ciclo di esecuzione di uno scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottieni un messaggio]

Ottiene i metadati di un messaggio specifico

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Message ID]</td> 
   <td> <p> Seleziona o mappa l’ID del messaggio per il quale desideri recuperare i metadati.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ottieni contenuto MIME]</td> 
   <td>Abilita questa opzione per recuperare i dati sul contenuto MIME del messaggio. Il contenuto MIME può includere immagini, audio, video o altri tipi di file.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Creare e inviare un messaggio]

Crea e invia un messaggio e-mail.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject]</td> 
   <td> <p>Inserisci o mappa l’oggetto del messaggio.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Body Content Type]</td> 
   <td>Seleziona se il contenuto del messaggio è HTML o Testo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contenuto del corpo]</td> 
   <td> <p>Immetti o mappa il testo del corpo del messaggio dell’e-mail.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importance]</td> 
   <td> <p>Seleziona l’importanza dell’e-mail</p> 
    <ul> 
     <li>[!UICONTROL Bassa]</li> 
     <li>[!UICONTROL Normale]</li> 
     <li>[!UICONTROL High]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Ai Destinatari]</p> </td> 
   <td> <p>Aggiungi l’indirizzo e-mail a cui desideri inviare i messaggi:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Immettere il nome del contatto</p> </li> 
     <li> <p><strong>[!UICONTROL Email Address]</strong> </p> <p>Immettere l'indirizzo e-mail del contatto.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL CC Recipients]</p> </td> 
   <td> <p>Aggiungi i destinatari che desideri ricevere una copia del messaggio:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Immettere il nome del contatto</p> </li> 
     <li> <p><strong>[!UICONTROL Email Address]</strong> </p> <p>Immettere l'indirizzo e-mail del contatto.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Destinatari Ccn [!UICONTROL]</p> </td> 
   <td> <p>Aggiungi i destinatari da copiare sul messaggio senza consentire ad altri destinatari di visualizzare i loro nomi o indirizzi e-mail:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Immettere il nome del contatto</p> </li> 
     <li> <p><strong>[!UICONTROL Email Address]</strong> </p> <p>Immettere l'indirizzo e-mail del contatto.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Allegati]</p> </td> 
   <td> <p>Aggiungi gli allegati all’e-mail:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL File name]</strong> </p> <p>Immettere il nome del file. Esempio: <code>sample.doc</code></p> </li> 
     <li> <p><strong>[!UICONTROL Data]</strong> </p> <p>Immettere i dati del file nel campo o mappare l'origine del file.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Internet Message Headers]</td> 
   <td> <p>Aggiungi le intestazioni del messaggio per l’e-mail.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Immettere il nome dell'intestazione</p> </li> 
     <li> <p><strong>[!UICONTROL Email Address]</strong> </p> <p>Immetti un valore per l’intestazione.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Spostare un messaggio]

Sposta un messaggio e-mail in una cartella selezionata nella cassetta postale.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Message ID]</td> 
   <td> <p> Seleziona o mappa l’ID del messaggio da spostare in un’altra cartella.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cartella Posta Elettronica] </td> 
   <td> <p>Seleziona o mappa l’ID della cartella in cui desideri spostare il messaggio.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminare un messaggio]

Elimina un messaggio e-mail esistente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Message ID]</td> 
   <td> <p> Seleziona o mappa l’ID del messaggio da eliminare.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Messaggio bozza

* [Creare una bozza di messaggio](#create-a-draft-message)
* [Inviare un messaggio di bozza](#send-a-draft-message)
* [Aggiornare un messaggio](#update-a-message)

#### [!UICONTROL Creare una bozza di messaggio]

Crea un nuovo messaggio e-mail.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject]</td> 
   <td> <p>Inserisci l’oggetto del messaggio.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body Content Type]</td> 
   <td>Seleziona se il contenuto del messaggio è HTML o Testo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contenuto del corpo]</td> 
   <td> <p>Inserisci il testo del corpo del messaggio dell’e-mail.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importance]</td> 
   <td> <p>Seleziona l’importanza dell’e-mail</p> 
    <ul> 
     <li>[!UICONTROL Bassa]</li> 
     <li>[!UICONTROL Normale]</li> 
     <li>[!UICONTROL High]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Ai Destinatari]</p> </td> 
   <td> <p>Aggiungi i destinatari a cui desideri inviare i messaggi:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Immettere il nome del contatto</p> </li> 
     <li> <p><strong>[!UICONTROL Email Address]</strong> </p> <p>Immettere l'indirizzo e-mail del contatto.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL CC Recipients]</p> </td> 
   <td> <p>Aggiungi i destinatari L’utente che desidera ricevere una copia del messaggio:</p> 
    <ul> 
     <li> <p><strong>Nome</strong> </p> <p>Immettere il nome del contatto</p> </li> 
     <li> <p><strong>Indirizzo Email</strong> </p> <p>Immettere l'indirizzo e-mail del contatto.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Destinatari Ccn</p> </td> 
   <td> <p>Aggiungi i destinatari da copiare sul messaggio senza consentire ad altri destinatari di visualizzare i loro nomi o indirizzi e-mail:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Immettere il nome del contatto</p> </li> 
     <li> <p><strong>[!UICONTROL Email Address]</strong> </p> <p>Immettere l'indirizzo e-mail del contatto.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Allegati]</p> </td> 
   <td> <p>Aggiungi gli allegati all’e-mail:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL File name]</strong> </p> <p>Immettere il nome del file. Esempio: <code>sample.doc</code></p> </li> 
     <li> <p><strong>[!UICONTROL Data]</strong> </p> <p>Immettere i dati del file nel campo o mappare l'origine del file.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Inviare un messaggio di bozza]

Invia un messaggio e-mail attualmente in bozza.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID messaggio bozza [!UICONTROL]</td> 
   <td> <p> Seleziona o mappa l’ID messaggio della bozza da inviare.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggiornare un messaggio]

Aggiorna un messaggio esistente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Immetti un ID messaggio]</td> 
   <td> <p>Seleziona la modalità di identificazione del messaggio da aggiornare:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Invio manuale]</strong> </p> <p>Immetti o mappa l'ID messaggio.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleziona dall’elenco]</strong> </p> <p>Seleziona la cartella contenente il messaggio da aggiornare, quindi seleziona il messaggio</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject]</td> 
   <td> <p>Inserisci l’oggetto del messaggio.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contenuto del corpo]</td> 
   <td> <p>Inserisci il testo del corpo del messaggio dell’e-mail.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importance]</td> 
   <td> <p>Seleziona l’importanza dell’e-mail</p> 
    <ul> 
     <li>[!UICONTROL Bassa]</li> 
     <li>[!UICONTROL Normale]</li> 
     <li>[!UICONTROL High]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Ai Destinatari]</p> </td> 
   <td> <p>Aggiungi l’indirizzo e-mail a cui desideri inviare i messaggi:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Immettere il nome del contatto</p> </li> 
     <li> <p><strong>[!UICONTROL Email Address]</strong> </p> <p>Immettere l'indirizzo e-mail del contatto.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL CC Recipients]</p> </td> 
   <td> <p>Aggiungi i destinatari L’utente che desidera ricevere una copia del messaggio:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Immettere il nome del contatto</p> </li> 
     <li> <p><strong>[!UICONTROL Email Address]</strong> </p> <p>Immettere l'indirizzo e-mail del contatto.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Destinatari Ccn [!UICONTROL]</p> </td> 
   <td> <p>Aggiungi i destinatari da copiare sul messaggio senza consentire ad altri destinatari di visualizzare i loro nomi o indirizzi e-mail:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Immettere il nome del contatto</p> </li> 
     <li> <p><strong>[!UICONTROL Email Address]</strong> </p> <p>Immettere l'indirizzo e-mail del contatto.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Allegati]</p> </td> 
   <td> <p>Aggiungi gli allegati all’e-mail:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL File name]</strong> </p> <p>Immettere il nome del file. Esempio: <code>sample.doc</code></p> </li> 
     <li> <p><strong>[!UICONTROL Data]</strong> </p> <p>Immettere i dati del file nel campo o mappare l'origine del file.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contrassegnalo come letto]</td> 
   <td>Abilita questa opzione per contrassegnare il messaggio aggiornato come letto.</td> 
  </tr> 
 </tbody> 
</table>

### Allegato

* [[!UICONTROL Elenco allegati]](#list-attachments)
* [[!UICONTROL Scaricare un allegato]](#download-an-attachment)

#### [!UICONTROL Elenco allegati]

Questo modulo recupera un elenco di allegati appartenenti al messaggio specificato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Message ID]</td> 
   <td> <p> Seleziona o mappa l’ID del messaggio da cui desideri recuperare gli allegati.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Immettere o mappare il numero massimo di allegati che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Scaricare un allegato]

Questo modulo scarica l&#39;allegato specificato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Message ID]</td> 
   <td> <p> Seleziona o mappa l’ID del messaggio contenente l’allegato da scaricare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Attachment ID]</td> 
   <td> <p>Immettere o mappare l'ID dell'allegato che si desidera scaricare.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Altro

* [[!UICONTROL Effettuare una chiamata API]](#make-an-api-call)
* [[!UICONTROL Aggiungi un allegato]](#add-an-attachment)

#### [!UICONTROL Effettuare una chiamata API]

Questo modulo ti consente di eseguire una chiamata API personalizzata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Immettere un percorso relativo a <code>https://graph.microsoft.com</code>. Esempio:<code> /v1.0/me/messages</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL, Metodo]</p> </td> 
   td&gt; <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Aggiungi le intestazioni della richiesta sotto forma di un oggetto JSON standard. Ad esempio, <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] aggiunge le intestazioni di autorizzazione per te.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p> Aggiungi la query per la chiamata API sotto forma di un oggetto JSON standard.</p> </td> 
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

#### [!UICONTROL Aggiungi un allegato]

Questo modulo aggiunge un allegato di grandi dimensioni a un messaggio.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Message ID]</td> 
   <td> <p> Seleziona o mappa l'ID del messaggio a cui desideri aggiungere un allegato.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File di origine]</td> 
   <td> <p>Selezionare un file da un modulo precedente o mappare il nome e i dati del file di origine.</p> </td> 
  </tr> 
 </tbody> 
</table>
