---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli Frame.io
description: La [!DNL Adobe Workfront Fusion Frame].io modules enable you to monitor, create, update, retrieve, or delete assets and comments in your [!DNL Frame.io] conto.
author: Becky
feature: Workfront Fusion
exl-id: 373a86f6-fbba-4914-b08d-a3a035ac0ae4
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2263'
ht-degree: 0%

---

# [!DNL Frame.io] moduli

La [!DNL Adobe Workfront Fusion] [!DNL Frame.io] i moduli consentono di monitorare, creare, aggiornare, recuperare o eliminare risorse e commenti nei [!DNL Frame.io] conto.

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

Per utilizzare [!DNL Frame.io] moduli, è necessario disporre di un [!DNL Frame.io] account

## Connetti [!DNL Frame.io] a [!UICONTROL Adobe Workfront Fusion]

È possibile connettersi a [!DNL Frame.io] utilizzando un token API o OAuth 2.0.

[Connetti a [!DNL Frame.io] utilizzo di un token API](#connect-to-frameio-using-an-api-token)

[Connetti a [!DNL Frame.io] utilizzo della PKCE OAuth 2.0](#connect-to-frameio-using-oauth-20-pkce)

### Connetti a [!DNL Frame.io] utilizzo di un token API

Per collegare il [!DNL Frame.io] account a [!DNL Workfront Fusion] utilizzando un token API, devi creare il token API nel [!DNL Frame.io] e inserirlo nel [!DNL Workfront Fusion] [!DNL Frame.io] [!UICONTROL Creare una connessione] finestra di dialogo.

1. Accedi al tuo [!DNL Frame.io] conto.
1. Vai a **[!UICONTROL Token]** nella pagina [!DNL Frame.io] Sviluppatore.
1. Fai clic su **[!UICONTROL Nuovo]**.
1. Immettere il nome del token, selezionare gli ambiti da utilizzare e fare clic su **[!UICONTROL Crea]**.
1. Copia il token fornito.
1. Vai a [!DNL Workfront Fusion] e aprire [!DNL Frame.io] del modulo **[!UICONTROL Creare una connessione]** finestra di dialogo.
1. In **[!UICONTROL Tipo di connessione]** campo , seleziona **[!DNL Frame.io]**.
1. Immetti il token copiato nel passaggio 5 nel **[!UICONTROL Le [!DNL Frame.io] Chiave API]** campo e fai clic su **[!UICONTROL Continua]** stabilire il collegamento.

Il collegamento è stato stabilito. È possibile procedere alla configurazione del modulo.

### Connetti a [!DNL Frame.io] utilizzo della PKCE OAuth 2.0

È possibile creare una connessione a [!DNL Frame.io] utilizzo della PKCE OAuth 2.0 con un ID client opzionale. Se desideri includere un ID client nella connessione, devi creare un’app OAuth 2.0 nel [!DNL Frame.io] conto.

* [Connetti a [!DNL Frame.io] utilizzo della PKCE OAuth 2.0 (senza ID client)](#connect-to-frameio-using-using-oauth-20-pkce-without-client-id)
* [Connetti a [!DNL Frame.io] utilizzo della PKCE OAuth 2.0 (con ID client)](#connect-to-frameio-using-using-oauth-20-pkce-with-client-id)

#### Connetti a [!DNL Frame.io] utilizzo della PKCE OAuth 2.0 (senza ID client)

1. Vai a [!DNL Workfront Fusion] e aprire [!DNL Frame.io] del modulo **[!UICONTROL Creare una connessione]** finestra di dialogo.
1. In **[!UICONTROL Tipo di connessione]** campo , seleziona **[!UICONTROL [!DNL Frame.io]PKCE OAuth 2.0]**.
1. Immettere un nome per la nuova connessione nel **[!UICONTROL Nome connessione]** campo .
1. Fai clic su **[!UICONTROL Continua]** stabilire il collegamento.

Il collegamento è stato stabilito. È possibile procedere alla configurazione del modulo.

#### Connetti a [!DNL Frame.io] utilizzo della PKCE OAuth 2.0 (con ID client)

1. Creare un’app OAuth 2.0 in [!DNL Frame.io]. Per istruzioni, consulta la sezione [!DNL Frame.io] documentazione [!UICONTROL Flusso di autorizzazione del codice OAuth 2.0].

   >[!IMPORTANT]
   >
   >Quando crei l’app OAuth 2.0 in [!DNL Frame.io]:
   >
   >* Inserisci quanto segue come URI di reindirizzamento:
   >   
   >  Americhe / APAC `https://app.workfrontfusion.com/oauth/cb/frame-io5`
   >
   >  EMEA `https://app-eu.workfrontfusion.com/oauth/cb/frame-io5`
   >
   >* Attiva l&#39;opzione PCKE.



1. Copia i dati forniti `client_id`.
1. Vai a [!DNL Workfront Fusion] e aprire [!DNL Frame.io] del modulo **[!UICONTROL Creare una connessione]** finestra di dialogo.
1. In **[!UICONTROL Tipo di connessione]** campo , seleziona **[!UICONTROL [!DNL Frame.io]PKCE OAuth 2.0]**.
1. Immettere un nome per la nuova connessione nel **[!UICONTROL Nome connessione]** campo .
1. Fai clic su **[!UICONTROL Mostra impostazioni avanzate]**.
1. Inserisci il `client_id` hai copiato nel passaggio 2 in **[!UICONTROL ID client]** campo .
1. Fai clic su **[!UICONTROL Continua]** stabilire il collegamento.

Il collegamento è stato stabilito. È possibile procedere alla configurazione del modulo.

## [!DNL Frame.io] moduli e relativi campi

Quando si configura [!DNL Frame.io] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL Frame.io] potrebbero essere visualizzati, a seconda di fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se trovi il pulsante mappa sopra un campo o una funzione, puoi utilizzarlo per impostare variabili e funzioni per quel campo. Per ulteriori informazioni, consulta [Mappare informazioni da un modulo a un altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Risorse](#assets)
* [Commenti](#comments)
* [Progetti](#projects)
* [Altro](#other)

### Risorse

* [[!UICONTROL Creare una risorsa]](#create-an-asset)
* [[!UICONTROL Eliminare una risorsa]](#delete-an-asset)
* [[!UICONTROL Ottenere una risorsa]](#get-an-asset)
* [[!UICONTROL Elenca risorse]](#list-assets)
* [[!UICONTROL Aggiornare una risorsa]](#update-an-asset)
* [[!UICONTROL Risorsa di controllo eliminata]](#watch-asset-deleted)
* [[!UICONTROL Etichetta della risorsa aggiornata]](#watch-asset-label-updated)
* [[!UICONTROL Guarda nuova risorsa]](#watch-new-asset)

#### [!UICONTROL Creare una risorsa]

Questo modulo di azione crea una nuova risorsa.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Per istruzioni su come creare una connessione a [!DNL Frame.io], vedi <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connetti [!DNL Frame.io] a [!DNL Adobe Workfront Fusion]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Seleziona o mappa il team a cui appartiene il progetto per il quale vuoi creare una risorsa.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project ID] </td> 
   <td> <p>Seleziona il progetto o mappa l’ID del progetto per il quale vuoi creare una risorsa.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID cartella [!UICONTROL] </td> 
   <td> <p>Seleziona la cartella o mappa l’ID della cartella in cui desideri creare la risorsa.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type] </td> 
   <td> <p>Seleziona se creare una cartella o un file.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Immettere il nome del nuovo file o della nuova cartella.</p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">File Type </td> 
    <td> <p>Select the type of file you want to upload.</p> </td> 
   </tr>
  --> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">File Size </td> 
    <td> <p>The file size in bytes.</p> </td> 
   </tr>
  --> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL di origine] </td> 
   <td> <p>Immetti l’URL del file da caricare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Descrizione] </td> 
   <td> <p>Immetti una breve descrizione della risorsa.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminare una risorsa]

Questo modulo di azione elimina una risorsa specificata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Per istruzioni su come creare una connessione a [!DNL Frame.io], vedi <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connetti [!DNL Frame.io] a [!DNL Adobe Workfront Fusion]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Seleziona o mappa il team proprietario del progetto che contiene la risorsa da eliminare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project ID]</td> 
   <td> <p> Seleziona il progetto o che contiene la risorsa da eliminare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID cartella [!UICONTROL] </td> 
   <td> <p>Seleziona la cartella che contiene la risorsa da eliminare</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID] </td> 
   <td> <p>Seleziona o mappa la risorsa da eliminare.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottenere una risorsa]

Questo modulo di azione recupera i dettagli della risorsa.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Per istruzioni su come creare una connessione a [!DNL Frame.io], vedi <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connetti [!DNL Frame.io] a [!DNL Adobe Workfront Fusion]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Seleziona o mappa il team proprietario del progetto che contiene la risorsa di cui desideri recuperare i dettagli.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project ID]</td> 
   <td> <p> Seleziona il progetto che contiene la risorsa di cui desideri recuperare i dettagli.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID cartella [!UICONTROL] </td> 
   <td> <p>Seleziona la cartella contenente la risorsa di cui desideri recuperare i dettagli.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID] </td> 
   <td> <p>Seleziona la risorsa o mappa l’ID della risorsa di cui desideri recuperare i dettagli.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Elenca risorse]

Questo modulo di ricerca recupera tutte le risorse nella cartella del progetto specificato.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Per istruzioni su come creare una connessione a [!DNL Frame.io], vedi <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connetti [!DNL Frame.io] a [!DNL Adobe Workfront Fusion]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Seleziona o mappa il team proprietario del progetto contenente la cartella da cui desideri recuperare le risorse.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project ID]</td> 
   <td> <p> Seleziona il progetto che contiene la cartella da cui desideri recuperare le risorse.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID cartella [!UICONTROL] </td> 
   <td> <p>Seleziona la cartella da cui vuoi elencare le risorse.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Impostare il numero massimo di risorse [!DNL Workfront Fusion] tornerà durante un ciclo di esecuzione.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### `[!UICONTROL Update an Asset]`

Questo modulo di azione ti consente di aggiornare il nome, la descrizione o i campi personalizzati di una risorsa esistente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Per istruzioni su come creare una connessione a [!DNL Frame.io], vedi <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connetti [!DNL Frame.io] a [!DNL Adobe Workfront Fusion]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Seleziona o mappa il team proprietario del progetto per il quale vuoi aggiornare una risorsa.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project ID] </td> 
   <td> <p>Seleziona il progetto o mappa l’ID del progetto per il quale vuoi aggiornare una risorsa.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID cartella [!UICONTROL] </td> 
   <td> <p>Seleziona la cartella o mappa l’ID della cartella in cui desideri aggiornare una risorsa.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Immetti il nome del file aggiornato.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Descrizione] </td> 
   <td> <p>Immetti una breve descrizione della risorsa aggiornata.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Risorsa di controllo eliminata]

Questo modulo di attivazione avvia uno scenario in cui una risorsa viene eliminata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook name]</td> 
   <td> <p> Immettere il nome del webhook, ad esempio Risorsa eliminata.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Per istruzioni su come creare una connessione a [!DNL Frame.io], vedi <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connetti [!DNL Frame.io] a [!DNL Adobe Workfront Fusion]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Selezionare il team per il quale viene creato il webhook.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Etichetta della risorsa aggiornata]

Questo modulo di attivazione avvia uno scenario in cui lo stato di una risorsa viene impostato, modificato o rimosso.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook name]</td> 
   <td> <p> Inserisci il nome del webhook, ad esempio lo stato del cespite aggiornato.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Per istruzioni su come creare una connessione a [!DNL Frame.io], vedi <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connetti [!DNL Frame.io] a [!DNL Adobe Workfront Fusion]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Selezionare il team per il quale viene creato il webhook.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Guarda nuova risorsa]

Questo modulo di attivazione avvia uno scenario in cui viene creata una nuova risorsa.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook name]</td> 
   <td> <p> Inserisci il nome del webhook, ad esempio Risorsa creata.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Per istruzioni su come creare una connessione a [!DNL Frame.io], vedi <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connetti [!DNL Frame.io] a [!DNL Adobe Workfront Fusion]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Selezionare il team per il quale viene creato il webhook.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Commenti

* [[!UICONTROL Creare un commento]](#create-a-comment)
* [[!UICONTROL Eliminare un commento]](#delete-a-comment)
* [[!UICONTROL Ottieni un commento]](#get-a-comment)
* [[!UICONTROL Elenca commenti]](#list-comments)
* [[!UICONTROL Aggiornare un commento]](#update-a-comment)
* [[!UICONTROL Commento di controllo aggiornato]](#watch-comment-updated)
* [[!UICONTROL Guarda nuovo commento]](#watch-new-comment)

#### [!UICONTROL Creare un commento]

Questo modulo di azione aggiunge un nuovo commento o risposta alla risorsa.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Per istruzioni su come creare una connessione a [!DNL Frame.io], vedi <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connetti [!DNL Frame.io] a [!DNL Adobe Workfront Fusion]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type] </td> 
   <td> <p>Seleziona se desideri creare un commento o una risposta a un commento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Seleziona o mappa il team a cui appartiene il progetto contenente la risorsa a cui desideri aggiungere un commento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project ID] </td> 
   <td> <p>Seleziona il progetto o mappa l’ID del progetto che contiene la risorsa a cui desideri aggiungere un commento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID cartella [!UICONTROL] </td> 
   <td> <p>Seleziona la cartella o mappa l’ID della cartella contenente la risorsa a cui desideri aggiungere un commento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID] </td> 
   <td> <p>Seleziona o mappa la risorsa a cui desideri aggiungere un commento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID commento </td> 
   <td> <p>Selezionare o mappare il commento a cui si desidera aggiungere una risposta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Testo]</td> 
   <td> <p> Inserisci il contenuto del commento o della risposta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Timestamp] </td> 
   <td> <p>Immetti il numero di fotogramma nel video a cui deve essere collegato il commento.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminare un commento]

Questo modulo di azione elimina un commento esistente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Per istruzioni su come creare una connessione a [!DNL Frame.io], vedi <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connetti [!DNL Frame.io] a [!DNL Adobe Workfront Fusion]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID]</td> 
   <td> <p> Seleziona o mappa il team proprietario del progetto contenente la risorsa da cui vuoi eliminare un commento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project ID]</td> 
   <td> <p> Seleziona il progetto o mappa l’ID del progetto che contiene la risorsa da cui vuoi eliminare un commento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID cartella [!UICONTROL]</td> 
   <td> <p> Seleziona la cartella contenente la risorsa da cui vuoi eliminare un commento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID] </td> 
   <td> <p>Seleziona la risorsa che contiene il commento da eliminare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID commento </td> 
   <td> <p>Selezionare il commento da eliminare.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottieni un commento]

Questo modulo di azione recupera i dettagli del commento specificato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Per istruzioni su come creare una connessione a [!DNL Frame.io], vedi <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connetti [!DNL Frame.io] a [!DNL Adobe Workfront Fusion]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Seleziona o mappa il team proprietario del progetto contenente la cartella da cui desideri recuperare le risorse.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project ID] </td> 
   <td> <p>Seleziona il progetto che contiene la cartella da cui desideri recuperare le risorse.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID cartella [!UICONTROL] </td> 
   <td> <p>Seleziona la cartella da cui vuoi elencare le risorse.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID] </td> 
   <td> <p>Seleziona la risorsa che contiene il commento da recuperare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID commento </td> 
   <td> <p>Selezionare il commento di cui si desidera recuperare i dettagli.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Elenca commenti]

Questo modulo di ricerca recupera tutti i commenti della risorsa specificata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Per istruzioni su come creare una connessione a [!DNL Frame.io], vedi <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connetti [!DNL Frame.io] a [!DNL Adobe Workfront Fusion]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Seleziona o mappa il team proprietario del progetto contenente la cartella da cui desideri recuperare i commenti.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project ID] </td> 
   <td> <p>Selezionare il progetto contenente la cartella da cui si desidera recuperare i commenti.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID cartella [!UICONTROL] </td> 
   <td> <p>Seleziona la cartella contenente la risorsa da cui vuoi elencare i commenti.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID] </td> 
   <td> <p>Seleziona la risorsa per la quale vuoi elencare i commenti.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Imposta il numero massimo di commenti [!DNL Workfront Fusion] tornerà durante un ciclo di esecuzione.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggiornare un commento]

Questo modulo di azione modifica un commento esistente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Per istruzioni su come creare una connessione a [!DNL Frame.io], vedi <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connetti [!DNL Frame.io] a [!DNL Adobe Workfront Fusion]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Seleziona o mappa il team proprietario del progetto che contiene la risorsa sulla quale desideri aggiornare un commento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project ID] </td> 
   <td> <p>Seleziona il progetto \ contenente la risorsa sulla quale desideri aggiornare un commento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID cartella [!UICONTROL] </td> 
   <td> <p>Seleziona la cartella contenente la risorsa sulla quale desideri aggiornare un commento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID] </td> 
   <td> <p>Seleziona la risorsa sulla quale desideri aggiornare un commento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID commento </td> 
   <td> <p>Selezionare il commento da aggiornare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Testo]</td> 
   <td> <p> Inserisci il contenuto testuale del commento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Timestamp] </td> 
   <td> <p>Immetti il numero di fotogramma nel video a cui è collegato il commento.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Commento di controllo aggiornato]

Questo modulo di attivazione avvia uno scenario in cui viene modificato un commento.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook name] </td> 
   <td> <p>Inserisci il nome del webhook, ad esempio Commento modificato.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Per istruzioni su come creare una connessione a [!DNL Frame.io], vedi <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connetti [!DNL Frame.io] a [!DNL Adobe Workfront Fusion]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Selezionare il team per il quale viene creato il webhook.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Guarda nuovo commento]

Questo modulo di attivazione avvia uno scenario in cui viene creato un nuovo commento o risposta.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook name] </td> 
   <td> <p>Inserisci il nome del webhook, ad esempio Nuovo commento.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Per istruzioni su come creare una connessione a [!DNL Frame.io], vedi <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connetti [!DNL Frame.io] a [!DNL Adobe Workfront Fusion]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Selezionare il team per il quale viene creato il webhook.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Progetti

#### [!UICONTROL Elenca progetti]

Questo modulo di ricerca recupera tutti i progetti per il team specificato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Per istruzioni su come creare una connessione a [!DNL Frame.io], vedi <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connetti [!DNL Frame.io] a [!DNL Adobe Workfront Fusion]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Seleziona o mappa il team per il quale desideri recuperare i progetti.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Imposta il numero massimo di progetti [!DNL Workfront Fusion] tornerà durante un ciclo di esecuzione.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Altro

#### [!UICONTROL Effettuare una chiamata API]

Questo modulo ti consente di eseguire una chiamata API personalizzata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Per istruzioni su come creare una connessione a [!DNL Frame.io], vedi <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connetti [!DNL Frame.io] a [!DNL Adobe Workfront Fusion]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Immettere un percorso relativo a <code>https://api.frame.io</code>. Esempio: <code> /v2/teams</code></p> <p>Nota: Per l’elenco degli endpoint disponibili, consulta [!DNL Frame.io] Riferimento API.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL, Metodo]</p> </td> 
   <td> <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Aggiungi le intestazioni della richiesta sotto forma di un oggetto JSON standard.</p> <p>Ad esempio: <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] aggiunge automaticamente le intestazioni di autorizzazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String] </td> 
   <td> <p>Immetti la stringa di query della richiesta. Per ogni parametro che si desidera includere nella stringa di query, fare clic su <b>[!UICONTROL Aggiungi elemento]</b> e immettere il nome del campo e il valore desiderato.</p> </td> 
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

**Esempio:** La seguente chiamata API restituisce tutti i team e i relativi dettagli nel [!DNL Frame.io] account:

URL: `/v2/teams`

Metodo: `GET`

![](assets/api-call-example.png)

Il risultato si trova in Output del modulo in Bundle > Corpo.

Nel nostro esempio, sono stati restituiti i dettagli di 1 team:

![](assets/api-call-output.png)
