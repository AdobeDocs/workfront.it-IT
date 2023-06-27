---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli Adobe Campaign Classic
description: Con il [!DNL Adobe Campaign Classic] moduli, è possibile avviare un [!DNL Adobe Workfront Fusion] scenario basato sugli eventi nel tuo [!DNL Adobe Campaign Classic] creare, leggere o aggiornare contratti e altri record, cercare i record utilizzando i criteri impostati e caricare i documenti.
author: Becky
feature: Workfront Fusion
exl-id: 84e8fa35-0c3c-46bd-8886-88c6d8d9e1d5
source-git-commit: 8b4182ae2b32488a02cacc16fcb6a246fcb571fd
workflow-type: tm+mt
source-wordcount: '1194'
ht-degree: 1%

---

# [!DNL Adobe Campaign Classic] moduli

Con il [!DNL Adobe Campaign Classic] moduli, è possibile avviare un [!DNL Adobe Workfront Fusion] scenario basato sugli eventi nel tuo [!DNL Adobe Campaign Classic] creare, leggere o aggiornare i record, cercare i record utilizzando i criteri impostati ed eseguire chiamate API personalizzate.

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

## Connetti [!DNL Adobe Campaign Classic] a [!DNL Adobe Workfront Fusion]

1. In qualsiasi [!DNL Adobe Campaign Classic] modulo, fai clic su **[!UICONTROL Aggiungi]** accanto al [!UICONTROL Connessione] campo.
1. Immetti l’URL di base da utilizzare per la connessione al tuo [!DNL Adobe Campaign Classic] dell&#39;istanza.
1. Immettere il nome utente e la password.
1. Clic **[!UICONTROL Continua]** per creare la connessione e tornare al modulo.

## [!DNL Adobe Campaign Classic] moduli e relativi campi

Quando si configura [!DNL Adobe Campaign Classic] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL Adobe Campaign Classic] I campi potrebbero essere visualizzati in base a fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se viene visualizzato il pulsante Mappa sopra un campo o una funzione, è possibile utilizzarlo per impostare variabili e funzioni per tale campo. Per ulteriori informazioni, consulta [Mappare le informazioni da un modulo all’altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Azioni](#actions)
* [Ricerche](#searches)

### Triggers

#### [!UICONTROL Osserva i record]

Questo modulo di attivazione pianificato avvia uno scenario quando un record cambia.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Per istruzioni sulla creazione di una connessione a [!DNL Adobe Campaign Classic], vedi <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Creare una connessione a [!DNL Adobe Campaign Classic]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtro]</td> 
   <td>Specificare se si desidera controllare i nuovi record, i record aggiornati o entrambi.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Seleziona la risorsa da controllare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campi da includere nell'output]</td> 
   <td>Selezionare i campi da includere nell'output del modulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campi personalizzati da includere nell'output]</td> 
   <td>Per ogni campo personalizzato da includere nell’output, fai clic su <b>[!UICONTROL Add]</b> e inserisci il nome del campo personalizzato.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Numero massimo di risultati restituiti]</td> 
   <td>Immettere o mappare il numero massimo di record che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</td> 
  </tr> 
 </tbody> 
</table>


### Azioni

* [[!UICONTROL Creare un record]](#create-a-record)
* [[!UICONTROL Effettuare una chiamata API personalizzata]](#make-a-custom-api-call)
* [[!UICONTROL Eliminare un record]](#delete-record)
* [[!UICONTROL Eseguire un’azione]](#perform-an-action)
* [[!UICONTROL Leggi un record]](#-read-a-record)
* [[!UICONTROL Iscrizione o annullamento dell’iscrizione]](#subscribe-or-unsubscribe)
* [[!UICONTROL Aggiornare un record]](#update-record)

#### [!UICONTROL Creare un record]

Questo modulo di azione crea un nuovo record in [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Per istruzioni sulla creazione di una connessione a [!DNL Adobe Campaign Classic], vedi <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Creare una connessione a [!DNL Adobe Campaign Classic]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Seleziona il tipo di [!DNL Adobe Campaign Classic] record da creare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fields] </td> 
   <td>Selezionare i campi per i quali si desidera impostare i valori al momento della creazione del record, quindi immettere i valori per tali campi. I campi variano in base al tipo di record selezionato.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campi personalizzati]</td> 
   <td> Per ogni campo personalizzato che si desidera aggiungere al nuovo record, fare clic su <b>[!UICONTROL Add item]</b> e immetti o mappa il nome e il valore del campo. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Effettuare una chiamata API personalizzata]

Questo modulo effettua una chiamata API personalizzata al [!DNL Adobe Campaign Classic] API

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Per istruzioni sulla creazione di una connessione a [!DNL Adobe Campaign Classic], vedi <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Creare una connessione a [!DNL Adobe Campaign Classic]</a> in questo articolo.</td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Action]</td>
      <td><p>Seleziona l’azione da eseguire per la chiamata API.</p>
      <p>[!UICONTROL Esegui query]</p>
      <p>[!UICONTROL Write]</p>
      <p>[!UICONTROL Ottieni entità se più recente]</p>
      <p>[!UICONTROL Seleziona tutto]</p>
      <p>[!UICONTROL Evento push]</p>
    </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>Aggiungi le intestazioni della richiesta sotto forma di oggetto JSON standard.</p>
        <p>Ad esempio: <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] aggiunge automaticamente l'intestazione del token [!UICONTROL x-security].</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Corpo XML]</td>
   <td> <p>Aggiungi il contenuto del corpo della chiamata API in XML, senza l’elemento sessione. </td>     </tr>
  </tbody>
</table>

#### [!UICONTROL Elimina record]

Questo modulo di azione elimina un singolo record da [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Per istruzioni sulla creazione di una connessione a [!DNL Adobe Campaign Classic], vedi <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Creare una connessione a [!DNL Adobe Campaign Classic]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Seleziona il tipo di risorsa da eliminare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Inserisci o mappa l’ID della risorsa da eliminare.</td> 
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL Eseguire un’azione]

Questo modulo di azione esegue un&#39;azione selezionata su un oggetto in [!DNL Adobe Campaign Classic] API.

Per informazioni su azioni e campi specifici, consulta [[!DNL Adobe Campaign] - Documentazione API](https://experienceleague.adobe.com/developer/campaign-api/api/p-14.html).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Per istruzioni sulla creazione di una connessione a [!DNL Adobe Campaign Classic], vedi <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Creare una connessione a [!DNL Adobe Campaign Classic]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Action]</td> 
   <td><p>Selezionare l'azione da eseguire sull'oggetto.</p>
   <ul>
   <li><p><b>[!DNL List]</b></p><p> Per i campi disponibili, vedi <a href="#search" class="MCXref xref" >[!UICONTROL - Ricerca]</a> in questo articolo. </p></li>
     <li><p><b>[!UICONTROL Get]</b></p><p> Per i campi disponibili, vedi <a href="#search" class="MCXref xref" >[!UICONTROL - Ricerca]</a> in questo articolo. </p></li> 
   <li><p><b>[!UICONTROL Crea]</b></p><p> Per i campi disponibili, vedi <a href="#create-a-record" class="MCXref xref" >[!UICONTROL Crea record]</a> in questo articolo. </p></li>
   <li><p><b>[!UICONTROL Update]</b></p><p> Per i campi disponibili, vedi <a href="#update-record" class="MCXref xref" >[!UICONTROL Aggiorna un record]</a> in questo articolo. </p></li>
   <li><p><b>[!UICONTROL Elimina]</b></p><p> Per i campi disponibili, vedi <a href="#delete-record" class="MCXref xref" >[!UICONTROL Elimina record]</a> in questo articolo. </p></li>
   </ul>
   </td>
</tr> 
 </tbody> 
</table>

#### [!UICONTROL Leggi un record]

Questo modulo di azione legge un record da [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Per istruzioni sulla creazione di una connessione a [!DNL Adobe Campaign Classic], vedi <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Creare una connessione a [!DNL Adobe Campaign Classic]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Seleziona il tipo di [!DNL Adobe Campaign Classic] record da leggere.</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL ID] </td> 
   <td>Immetti di mappare l’ID del record da leggere.</td> 
  </tr> 
 <tr> 
   <td role="rowheader">[!UICONTROL Campi da includere nell'output] </td> 
   <td>Selezionare i campi da includere nell'output del modulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campi personalizzati da includere nell'output]</td> 
   <td>Per ogni campo personalizzato da includere nell’output, fai clic su <b>[!UICONTROL Add]</b> e inserisci il nome del campo personalizzato.</td> 
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL Iscrizione o annullamento dell’iscrizione]

Questo modulo di azione sottoscrive o annulla l&#39;abbonamento di un utente a un servizio di informazioni.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Per istruzioni sulla creazione di una connessione a [!DNL Adobe Campaign Classic], vedi <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Creare una connessione a [!DNL Adobe Campaign Classic]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sottoscrivi o annulla sottoscrizione]</td> 
   <td>Seleziona se desideri abbonarti o annullare l’abbonamento al servizio di informazioni.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome servizio]</td> 
   <td>Seleziona il servizio a cui vuoi abbonarti o dal quale vuoi annullare l’abbonamento.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Indirizzo e-mail destinatario] </td> 
   <td>Inserisci o mappa l’indirizzo e-mail dell’utente che desideri abbonarti o annullare l’abbonamento al servizio di informazioni.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggiorna record]

Questo modulo di azione aggiorna un singolo record in [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Per istruzioni sulla creazione di una connessione a [!DNL Adobe Campaign Classic], vedi <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Creare una connessione a [!DNL Adobe Campaign Classic]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Seleziona il tipo di [!DNL Adobe Campaign Classic] record da creare.</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL ID] </td> 
   <td>Immetti di mappare l’ID del record da aggiornare.</td> 
  </tr> 
<tr> 
   <td role="rowheader">[!UICONTROL Fields] </td> 
   <td>Selezionare i campi per i quali si desidera aggiornare i valori, quindi immettere i valori per tali campi. I campi variano in base al tipo di record selezionato.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campi personalizzati]</td> 
   <td> Per ogni campo personalizzato da aggiornare, fai clic su <b>[!UICONTROL Add item]</b> e immetti o mappa il nome e il valore del campo. </td> 
  </tr> 
 </tbody> 
</table>

### Ricerche

#### [!UICONTROL Ricerca]

Questo modulo di ricerca restituisce record in base ai criteri specificati.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Per istruzioni sulla creazione di una connessione a [!DNL Adobe Campaign Classic], vedi <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Creare una connessione a [!DNL Adobe Campaign Classic]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Seleziona il tipo di [!DNL Adobe Campaign Classic] record da creare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td>Immettere o mappare il numero massimo di record che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</td> 
  </tr> 
 </tbody> 
</table>
