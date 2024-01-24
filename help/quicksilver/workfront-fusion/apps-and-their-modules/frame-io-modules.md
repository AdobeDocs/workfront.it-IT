---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli Frame.io
description: Il [!DNL Adobe Workfront Fusion Frame].io modules enable you to monitor, create, update, retrieve, or delete assets and comments in your [!DNL Frame.io] account.
author: Becky
feature: Workfront Fusion
exl-id: 373a86f6-fbba-4914-b08d-a3a035ac0ae4
source-git-commit: c51169c18bef8ac8126a04c08deb88d830517b0b
workflow-type: tm+mt
source-wordcount: '2338'
ht-degree: 0%

---

# [!DNL Frame.io] moduli

Il [!DNL Adobe Workfront Fusion] [!DNL Frame.io] consentono di monitorare, creare, aggiornare, recuperare o eliminare risorse e commenti [!DNL Frame.io] account.

Per un video introduttivo sul connettore Frame.io, vedi:

* [Frame.io](https://video.tv.adobe.com/v/3427032/){target=_blank}

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

Da utilizzare [!DNL Frame.io] moduli, è necessario disporre di un [!DNL Frame.io] account

## Connetti [!DNL Frame.io] a [!UICONTROL Adobe Workfront Fusion]

È possibile connettersi a [!DNL Frame.io] utilizzando un token API o utilizzando OAuth 2.0.

[Connetti a [!DNL Frame.io] utilizzo di un token API](#connect-to-frameio-using-an-api-token)

[Connetti a [!DNL Frame.io] utilizzo di OAuth 2.0 PKCE](#connect-to-frameio-using-oauth-20-pkce)

### Connetti a [!DNL Frame.io] utilizzo di un token API

Per collegare [!DNL Frame.io] account a [!DNL Workfront Fusion] utilizzando un token API, devi creare il token API nel tuo [!DNL Frame.io] e inseriscilo nel [!DNL Workfront Fusion] [!DNL Frame.io] [!UICONTROL Creare una connessione] .

1. Accedi al tuo [!DNL Frame.io] account.
1. Vai a **[!UICONTROL Token]** pagina in [!DNL Frame.io] Sviluppatore.
1. Clic **[!UICONTROL Nuovo]**.
1. Inserisci il nome del token, seleziona gli ambiti da utilizzare e fai clic su **[!UICONTROL Crea]**.
1. Copia il token fornito.
1. Vai a [!DNL Workfront Fusion] e apri [!DNL Frame.io] del modulo **[!UICONTROL Creare una connessione]** .
1. In **[!UICONTROL Tipo di connessione]** campo, seleziona **[!DNL Frame.io]**.
1. Immetti il token copiato al punto 5 in **[!UICONTROL Il tuo [!DNL Frame.io] Chiave API]** e fai clic su **[!UICONTROL Continua]** per stabilire la connessione.

La connessione è stata stabilita. Puoi procedere con la configurazione del modulo.

### Connetti a [!DNL Frame.io] utilizzo di OAuth 2.0 PKCE

Puoi creare una connessione a [!DNL Frame.io] utilizzo di OAuth 2.0 PKCE con un ID client opzionale. Se desideri includere un ID client nella connessione, devi creare un’app OAuth 2.0 nel tuo [!DNL Frame.io] account.

* [Connetti a [!DNL Frame.io] utilizzo di OAuth 2.0 PKCE (senza ID client)](#connect-to-frameio-using-using-oauth-20-pkce-without-client-id)
* [Connetti a [!DNL Frame.io] utilizzo di OAuth 2.0 PKCE (con ID client)](#connect-to-frameio-using-using-oauth-20-pkce-with-client-id)

#### Connetti a [!DNL Frame.io] utilizzo di OAuth 2.0 PKCE (senza ID client)

1. Vai a [!DNL Workfront Fusion] e apri [!DNL Frame.io] del modulo **[!UICONTROL Creare una connessione]** .
1. In **[!UICONTROL Tipo di connessione]** campo, seleziona **[!UICONTROL [!DNL Frame.io]PKCE OAuth 2.0]**.
1. Immetti un nome per la nuova connessione in **[!UICONTROL Nome connessione]** campo.
1. Clic **[!UICONTROL Continua]** per stabilire la connessione.

La connessione è stata stabilita. Puoi procedere con la configurazione del modulo.

#### Connetti a [!DNL Frame.io] utilizzo di OAuth 2.0 PKCE (con ID client)

1. Creare un’app OAuth 2.0 in [!DNL Frame.io]. Per istruzioni, vedere [!DNL Frame.io] documentazione su [!UICONTROL Flusso di autorizzazione del codice OAuth 2.0].

   >[!IMPORTANT]
   >
   >Durante la creazione dell’app OAuth 2.0 in [!DNL Frame.io]:
   >
   >* Immetti quanto segue come URI di reindirizzamento:
   >   
   >  Americhe/APAC `https://app.workfrontfusion.com/oauth/cb/frame-io5`
   >
   >  EMEA `https://app-eu.workfrontfusion.com/oauth/cb/frame-io5`
   >
   >* Abilitare l&#39;opzione PCKE.


1. Copia il fornito `client_id`.
1. Vai a [!DNL Workfront Fusion] e apri [!DNL Frame.io] del modulo **[!UICONTROL Creare una connessione]** .
1. In **[!UICONTROL Tipo di connessione]** campo, seleziona **[!UICONTROL [!DNL Frame.io]PKCE OAuth 2.0]**.
1. Immetti un nome per la nuova connessione in **[!UICONTROL Nome connessione]** campo.
1. Clic **[!UICONTROL Mostra impostazioni avanzate]**.
1. Inserisci il `client_id` hai copiato nel passaggio 2 in **[!UICONTROL ID client]** campo.
1. Clic **[!UICONTROL Continua]** per stabilire la connessione.

La connessione è stata stabilita. Puoi procedere con la configurazione del modulo.

## [!DNL Frame.io] moduli e relativi campi

Quando si configura [!DNL Frame.io] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL Frame.io] I campi potrebbero essere visualizzati in base a fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se viene visualizzato il pulsante Mappa sopra un campo o una funzione, è possibile utilizzarlo per impostare variabili e funzioni per tale campo. Per ulteriori informazioni, consulta [Mappare le informazioni da un modulo all’altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Risorse](#assets)
* [Commenti](#comments)
* [Progetti](#projects)
* [Altro](#other)

### Risorse

* [[!UICONTROL Creare una risorsa]](#create-an-asset)
* [[!UICONTROL Eliminare una risorsa]](#delete-an-asset)
* [[!UICONTROL Ottieni una risorsa]](#get-an-asset)
* [[!UICONTROL Elencare risorse]](#list-assets)
* [[!UICONTROL Aggiornare una risorsa]](#update-an-asset)
* [[!UICONTROL Osserva risorsa eliminata]](#watch-asset-deleted)
* [[!UICONTROL Etichetta risorsa di controllo aggiornata]](#watch-asset-label-updated)
* [[!UICONTROL Guarda nuova risorsa]](#watch-new-asset)

#### [!UICONTROL Creare una risorsa]

Questo modulo crea una nuova risorsa.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Per istruzioni sulla creazione di una connessione a [!DNL Frame.io], vedi <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connetti [!DNL Frame.io] a [!DNL Adobe Workfront Fusion]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID team] </td> 
   <td> <p>Seleziona o mappa il team a cui appartiene il progetto per il quale desideri creare una risorsa.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID progetto] </td> 
   <td> <p>Seleziona il progetto o mappa l’ID del progetto per il quale desideri creare una risorsa.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID cartella] </td> 
   <td> <p>Seleziona la cartella o mappa l’ID della cartella in cui desideri creare una risorsa.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type] </td> 
   <td> <p>Seleziona se creare una cartella o un file.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Immettere il nome del nuovo file o cartella.</p> </td> 
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
   <td> <p>Inserire una breve descrizione della risorsa.</p> </td> 
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
   <td>Per istruzioni sulla creazione di una connessione a [!DNL Frame.io], vedi <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connetti [!DNL Frame.io] a [!DNL Adobe Workfront Fusion]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID team] </td> 
   <td> <p>Seleziona o mappa il team a cui appartiene il progetto che contiene la risorsa da eliminare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID progetto]</td> 
   <td> <p> Seleziona il progetto o che contiene la risorsa da eliminare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID cartella] </td> 
   <td> <p>Seleziona la cartella contenente la risorsa da eliminare</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID risorsa] </td> 
   <td> <p>Seleziona o mappa la risorsa da eliminare.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottieni una risorsa]

Questo modulo di azione recupera i dettagli della risorsa.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Per istruzioni sulla creazione di una connessione a [!DNL Frame.io], vedi <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connetti [!DNL Frame.io] a [!DNL Adobe Workfront Fusion]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID team] </td> 
   <td> <p>Seleziona o mappa il team a cui appartiene il progetto che contiene la risorsa di cui desideri recuperare i dettagli.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID progetto]</td> 
   <td> <p> Seleziona il progetto contenente la risorsa di cui desideri recuperare i dettagli.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID cartella] </td> 
   <td> <p>Seleziona la cartella contenente la risorsa di cui desideri recuperare i dettagli.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID risorsa] </td> 
   <td> <p>Seleziona la risorsa o mappa l’ID della risorsa di cui desideri recuperare i dettagli.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Elencare risorse]

Questo modulo di ricerca recupera tutte le risorse nella cartella del progetto specificato.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Per istruzioni sulla creazione di una connessione a [!DNL Frame.io], vedi <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connetti [!DNL Frame.io] a [!DNL Adobe Workfront Fusion]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID team] </td> 
   <td> <p>Seleziona o mappa il team a cui appartiene il progetto contenente la cartella da cui desideri recuperare le risorse.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID progetto]</td> 
   <td> <p> Seleziona il progetto che contiene la cartella da cui desideri recuperare le risorse.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID cartella] </td> 
   <td> <p>Seleziona la cartella da cui elencare le risorse.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Impostare il numero massimo di risorse [!DNL Workfront Fusion] restituirà durante un ciclo di esecuzione.</p> </td> 
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
   <td>Per istruzioni sulla creazione di una connessione a [!DNL Frame.io], vedi <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connetti [!DNL Frame.io] a [!DNL Adobe Workfront Fusion]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID team] </td> 
   <td> <p>Seleziona o mappa il team a cui appartiene il progetto per il quale desideri aggiornare una risorsa.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID progetto] </td> 
   <td> <p>Seleziona il progetto o mappa l’ID del progetto per il quale desideri aggiornare una risorsa.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID cartella] </td> 
   <td> <p>Seleziona la cartella o mappa l’ID della cartella in cui desideri aggiornare una risorsa.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Immettere il nome del file aggiornato.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Descrizione] </td> 
   <td> <p>Inserisci una breve descrizione della risorsa aggiornata.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Osserva risorsa eliminata]

Questo modulo di attivazione avvia uno scenario quando una risorsa viene eliminata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome webhook]</td> 
   <td> <p> Immetti il nome del webhook, ad esempio Risorsa eliminata.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Per istruzioni sulla creazione di una connessione a [!DNL Frame.io], vedi <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connetti [!DNL Frame.io] a [!DNL Adobe Workfront Fusion]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID team] </td> 
   <td> <p>Selezionare il team per cui è stato creato il webhook.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Etichetta risorsa di controllo aggiornata]

Questo modulo di attivazione avvia uno scenario quando lo stato di una risorsa viene impostato, modificato o rimosso.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome webhook]</td> 
   <td> <p> Inserisci il nome del webhook. Ad esempio, stato risorsa aggiornato.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Per istruzioni sulla creazione di una connessione a [!DNL Frame.io], vedi <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connetti [!DNL Frame.io] a [!DNL Adobe Workfront Fusion]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID team] </td> 
   <td> <p>Selezionare il team per cui è stato creato il webhook.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Guarda nuova risorsa]

Questo modulo di attivazione avvia uno scenario quando viene creata una nuova risorsa.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome webhook]</td> 
   <td> <p> Immetti il nome del webhook, ad esempio Risorsa creata.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Per istruzioni sulla creazione di una connessione a [!DNL Frame.io], vedi <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connetti [!DNL Frame.io] a [!DNL Adobe Workfront Fusion]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID team] </td> 
   <td> <p>Selezionare il team per cui è stato creato il webhook.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Commenti

* [[!UICONTROL Crea un commento]](#create-a-comment)
* [[!UICONTROL Eliminare un commento]](#delete-a-comment)
* [[!UICONTROL Leggi un commento]](#get-a-comment)
* [[!UICONTROL Elenca commenti]](#list-comments)
* [[!UICONTROL Aggiornare un commento]](#update-a-comment)
* [[!UICONTROL Osserva commento aggiornato]](#watch-comment-updated)
* [[!UICONTROL Guarda nuovo commento]](#watch-new-comment)

#### [!UICONTROL Crea un commento]

Questo modulo di azione aggiunge un nuovo commento o una nuova risposta alla risorsa.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Per istruzioni sulla creazione di una connessione a [!DNL Frame.io], vedi <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connetti [!DNL Frame.io] a [!DNL Adobe Workfront Fusion]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type] </td> 
   <td> <p>Specificare se si desidera creare un commento o rispondere a un commento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID team] </td> 
   <td> <p>Seleziona o mappa il team a cui appartiene il progetto contenente la risorsa a cui desideri aggiungere un commento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID progetto] </td> 
   <td> <p>Seleziona il progetto o mappa l’ID del progetto che contiene la risorsa a cui desideri aggiungere un commento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID cartella] </td> 
   <td> <p>Seleziona la cartella o mappa l’ID della cartella che contiene la risorsa a cui desideri aggiungere un commento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID risorsa] </td> 
   <td> <p>Seleziona o mappa la risorsa a cui desideri aggiungere un commento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID commento] </td> 
   <td> <p>Seleziona o mappa il commento a cui desideri aggiungere una risposta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Text]</td> 
   <td> <p> Immettere il contenuto del testo del commento o della risposta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Timestamp] </td> 
   <td> <p>Immetti il numero del fotogramma nel video a cui deve essere collegato il commento.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminare un commento]

Questo modulo elimina un commento esistente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Per istruzioni sulla creazione di una connessione a [!DNL Frame.io], vedi <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connetti [!DNL Frame.io] a [!DNL Adobe Workfront Fusion]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID team]</td> 
   <td> <p> Seleziona o esegui il mapping del team a cui appartiene il progetto contenente la risorsa da cui desideri eliminare un commento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID progetto]</td> 
   <td> <p> Seleziona il progetto o mappa l’ID del progetto che contiene la risorsa da cui desideri eliminare un commento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID cartella]</td> 
   <td> <p> Seleziona la cartella contenente la risorsa da cui desideri eliminare un commento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID risorsa] </td> 
   <td> <p>Seleziona la risorsa contenente il commento da eliminare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID commento] </td> 
   <td> <p>Selezionare il commento che si desidera eliminare.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Leggi un commento]

Questo modulo di azione recupera i dettagli del commento specificato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Per istruzioni sulla creazione di una connessione a [!DNL Frame.io], vedi <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connetti [!DNL Frame.io] a [!DNL Adobe Workfront Fusion]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID team] </td> 
   <td> <p>Seleziona o mappa il team a cui appartiene il progetto contenente la cartella da cui desideri recuperare le risorse.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID progetto] </td> 
   <td> <p>Seleziona il progetto che contiene la cartella da cui desideri recuperare le risorse.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID cartella] </td> 
   <td> <p>Seleziona la cartella da cui elencare le risorse.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID risorsa] </td> 
   <td> <p>Seleziona la risorsa contenente il commento da recuperare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID commento] </td> 
   <td> <p>Seleziona il commento di cui desideri recuperare i dettagli.</p> </td> 
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
   <td>Per istruzioni sulla creazione di una connessione a [!DNL Frame.io], vedi <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connetti [!DNL Frame.io] a [!DNL Adobe Workfront Fusion]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID team] </td> 
   <td> <p>Selezionare o mappare il team proprietario del progetto contenente la cartella da cui si desidera recuperare i commenti.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID progetto] </td> 
   <td> <p>Selezionare il progetto contenente la cartella da cui si desidera recuperare i commenti.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID cartella] </td> 
   <td> <p>Seleziona la cartella contenente la risorsa da cui desideri elencare i commenti.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID risorsa] </td> 
   <td> <p>Seleziona la risorsa per la quale desideri elencare i commenti.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Imposta il numero massimo di commenti [!DNL Workfront Fusion] restituirà durante un ciclo di esecuzione.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggiornare un commento]

Questo modulo modifica un commento esistente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Per istruzioni sulla creazione di una connessione a [!DNL Frame.io], vedi <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connetti [!DNL Frame.io] a [!DNL Adobe Workfront Fusion]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID team] </td> 
   <td> <p>Seleziona o mappa il team a cui appartiene il progetto contenente la risorsa su cui desideri aggiornare un commento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID progetto] </td> 
   <td> <p>Seleziona il progetto \ che contiene la risorsa su cui desideri aggiornare un commento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID cartella] </td> 
   <td> <p>Seleziona la cartella contenente la risorsa su cui desideri aggiornare un commento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID risorsa] </td> 
   <td> <p>Seleziona la risorsa per la quale desideri aggiornare un commento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID commento] </td> 
   <td> <p>Seleziona il commento da aggiornare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Text]</td> 
   <td> <p> Immetti il contenuto del testo del commento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Timestamp] </td> 
   <td> <p>Immetti il numero del fotogramma nel video a cui è collegato il commento.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Osserva commento aggiornato]

Questo modulo di attivazione avvia uno scenario quando viene modificato un commento.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome webhook] </td> 
   <td> <p>Immetti il nome del webhook, ad esempio Commento modificato.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Per istruzioni sulla creazione di una connessione a [!DNL Frame.io], vedi <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connetti [!DNL Frame.io] a [!DNL Adobe Workfront Fusion]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID team] </td> 
   <td> <p>Selezionare il team per cui è stato creato il webhook.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Guarda nuovo commento]

Questo modulo di attivazione avvia uno scenario quando viene creato un nuovo commento o una nuova risposta.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome webhook] </td> 
   <td> <p>Immetti il nome del webhook, ad esempio Nuovo commento.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Per istruzioni sulla creazione di una connessione a [!DNL Frame.io], vedi <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connetti [!DNL Frame.io] a [!DNL Adobe Workfront Fusion]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID team] </td> 
   <td> <p>Selezionare il team per cui è stato creato il webhook.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Progetti

#### [!UICONTROL Elencare progetti]

Questo modulo di ricerca recupera tutti i progetti per il team specificato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Per istruzioni sulla creazione di una connessione a [!DNL Frame.io], vedi <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connetti [!DNL Frame.io] a [!DNL Adobe Workfront Fusion]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID team] </td> 
   <td> <p>Seleziona o mappa il team per il quale desideri recuperare i progetti.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Imposta il numero massimo di progetti [!DNL Workfront Fusion] restituirà durante un ciclo di esecuzione.</p> </td> 
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
   <td>Per istruzioni sulla creazione di una connessione a [!DNL Frame.io], vedi <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connetti [!DNL Frame.io] a [!DNL Adobe Workfront Fusion]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Inserisci un percorso relativo a <code>https://api.frame.io</code>. Esempio: <code> /v2/teams</code></p> <p>Nota: per un elenco degli endpoint disponibili, fare riferimento al [!DNL Frame.io] Riferimento API.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Method]</p> </td> 
   <td> <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Aggiungi le intestazioni della richiesta sotto forma di oggetto JSON standard.</p> <p>Ad esempio: <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] aggiunge automaticamente le intestazioni di autorizzazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Stringa Di Query] </td> 
   <td> <p>Immettere la stringa di query richiesta. Per ogni parametro che si desidera includere nella stringa di query, fare clic su <b>[!UICONTROL Add item]</b> e inserisci il nome del campo e il valore desiderato.</p> </td> 
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

**Esempio:** La seguente chiamata API restituisce tutti i team e i relativi dettagli nel [!DNL Frame.io] account:

URL: `/v2/teams`

Metodo: `GET`

![](assets/api-call-example.png)

Il risultato si trova nell’Output del modulo in Bundle > Body.

Nel nostro esempio, sono stati restituiti i dettagli di 1 team:

![](assets/api-call-output.png)
