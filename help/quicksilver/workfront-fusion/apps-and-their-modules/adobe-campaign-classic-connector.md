---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli Adobe Campaign Classic
description: Con la [!DNL Adobe Campaign Classic] moduli, è possibile avviare un [!DNL Adobe Workfront Fusion] in base agli eventi nel [!DNL Adobe Campaign Classic] creare, leggere o aggiornare accordi e altri record, cercare record utilizzando i criteri impostati e caricare documenti.
author: Becky
feature: Workfront Fusion
exl-id: 84e8fa35-0c3c-46bd-8886-88c6d8d9e1d5
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1146'
ht-degree: 1%

---

# [!DNL Adobe Campaign Classic] moduli

Con la [!DNL Adobe Campaign Classic] moduli, è possibile avviare un [!DNL Adobe Workfront Fusion] in base agli eventi nel [!DNL Adobe Campaign Classic] creare, leggere o aggiornare i record, cercare i record utilizzando i criteri impostati ed eseguire chiamate API personalizzate.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</td> 
  </tr> 
 </tbody> 
</table>

Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, vedi [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Connetti [!DNL Adobe Campaign Classic] a [!DNL Adobe Workfront Fusion]

1. In qualsiasi [!DNL Adobe Campaign Classic] modulo, fai clic su **[!UICONTROL Aggiungi]** accanto al [!UICONTROL Connessione] campo .
1. Immetti l’URL di base utilizzato per la connessione al tuo [!DNL Adobe Campaign Classic] istanza.
1. Immetti il tuo nome utente e la tua password.
1. Fai clic su **[!UICONTROL Continua]** per creare la connessione e tornare al modulo .

## [!DNL Adobe Campaign Classic] moduli e relativi campi

Quando si configura [!DNL Adobe Campaign Classic] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL Adobe Campaign Classic] potrebbero essere visualizzati, a seconda di fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se trovi il pulsante mappa sopra un campo o una funzione, puoi utilizzarlo per impostare variabili e funzioni per quel campo. Per ulteriori informazioni, consulta [Mappare informazioni da un modulo a un altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Azioni](#actions)
* [Ricerche](#searches)

### Triggers

#### [!UICONTROL Registri di controllo]

Questo modulo trigger pianificato avvia uno scenario in cui un record cambia.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Per istruzioni su come creare una connessione a [!DNL Adobe Campaign Classic], vedi <a href="#connect-adobe-campaign-connector-to-adobe-workfront-fusion" class="MCXref xref" >Creare una connessione a [!DNL Adobe Campaign Classic]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td>Selezionare se si desidera controllare i nuovi record, i record aggiornati o entrambi.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Seleziona la risorsa da cercare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campi da includere nell’output]</td> 
   <td>Seleziona i campi da includere nell’output del modulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campi personalizzati da includere nell’output]</td> 
   <td>Per ogni campo personalizzato che si desidera includere nell'output, fare clic su <b>[!UICONTROL Aggiungi]</b> e immettere il nome del campo personalizzato.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Numero massimo di risultati restituiti]</td> 
   <td>Immettere o mappare il numero massimo di record che si desidera restituire dal modulo durante ogni ciclo di esecuzione degli scenari.</td> 
  </tr> 
 </tbody> 
</table>


### Azioni

* [[!UICONTROL Creare un record]](#create-a-record)
* [[!UICONTROL Effettuare una chiamata API personalizzata]](#make-a-custom-api-call)
* [[!UICONTROL Eliminare un record]](#delete-record)
* [[!UICONTROL Esegui un&#39;azione]](#perform-an-action)
* [[!UICONTROL Leggi un record]](#-read-a-record)
* [[!UICONTROL Abbonati o annulla sottoscrizione]](#subscribe-or-unsubscribe)
* [[!UICONTROL Aggiornare un record]](#update-record)

#### [!UICONTROL Creare un record]

Questo modulo di azione crea un nuovo record in [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Per istruzioni su come creare una connessione a [!DNL Adobe Campaign Classic], vedi <a href="#connect-adobe-campaign-connector-to-adobe-workfront-fusion" class="MCXref xref" >Creare una connessione a [!DNL Adobe Campaign Classic]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Seleziona il tipo di [!DNL Adobe Campaign Classic] record da creare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fields] </td> 
   <td>Selezionare i campi per i quali si desidera impostare i valori al momento della creazione del record, quindi inserire i valori per tali campi. I campi variano in base al tipo di record selezionato.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campi personalizzati]</td> 
   <td> Per ogni campo personalizzato che si desidera aggiungere al nuovo record, fare clic su <b>[!UICONTROL Aggiungi elemento]</b> e immettere o mappare il nome e il valore del campo. </td> 
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
   <td>Per istruzioni su come creare una connessione a [!DNL Adobe Campaign Classic], vedi <a href="#connect-adobe-campaign-connector-to-adobe-workfront-fusion" class="MCXref xref" >Creare una connessione a [!DNL Adobe Campaign Classic]</a> in questo articolo.</td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Action]</td>
      <td><p>Seleziona l’azione da eseguire nella chiamata API.</p>
      <p>[!UICONTROL Esegui query]</p>
      <p>[!UICONTROL Write]</p>
      <p>[!UICONTROL Ottieni entità se più recente]</p>
      <p>[!UICONTROL Seleziona tutto]</p>
      <p>[!UICONTROL Push event]</p>
    </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>Aggiungi le intestazioni della richiesta sotto forma di un oggetto JSON standard.</p>
        <p>Ad esempio: <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] aggiunge automaticamente l'intestazione del token x-security.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL XML Body]</td>
   <td> <p>Aggiungi il contenuto del corpo per la chiamata API in XML, senza l’elemento di sessione. </td>     </tr>
  </tbody>
</table>

#### [!UICONTROL Elimina record]

Questo modulo di azione elimina un record singolo da [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Per istruzioni su come creare una connessione a [!DNL Adobe Campaign Classic], vedi <a href="#connect-adobe-campaign-connector-to-adobe-workfront-fusion" class="MCXref xref" >Creare una connessione a [!DNL Adobe Campaign Classic]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Seleziona il tipo di risorsa da eliminare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Immetti o mappa l’ID della risorsa da eliminare.</td> 
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL Esegui un&#39;azione]

Questo modulo di azione esegue un&#39;azione selezionata su un oggetto nel [!DNL Adobe Campaign Classic] API.

Per informazioni su azioni e campi specifici, consulta [[!DNL Adobe Campaign] - Documentazione API](https://experienceleague.adobe.com/developer/campaign-api/api/p-14.html).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Per istruzioni su come creare una connessione a [!DNL Adobe Campaign Classic], vedi <a href="#connect-adobe-campaign-connector-to-adobe-workfront-fusion" class="MCXref xref" >Creare una connessione a [!DNL Adobe Campaign Classic]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Action]</td> 
   <td><p>Selezionare l’azione da eseguire sull’oggetto.</p>
   <ul>
   <li><p><b>[!DNL List]</b></p><p> Per i campi disponibili, vedi <a href="#search" class="MCXref xref" >[!UICONTROL Search]</a> in questo articolo. </p></li>
     <li><p><b>[!UICONTROL Get]</b></p><p> Per i campi disponibili, vedi <a href="#search" class="MCXref xref" >[!UICONTROL Search]</a> in questo articolo. </p></li> 
   <li><p><b>[!UICONTROL Create]</b></p><p> Per i campi disponibili, vedi <a href="#create-a-record" class="MCXref xref" >[!UICONTROL Creare un record]</a> in questo articolo. </p></li>
   <li><p><b>[!UICONTROL Update]</b></p><p> Per i campi disponibili, vedi <a href="#update-record" class="MCXref xref" >[!UICONTROL Aggiornare un record]</a> in questo articolo. </p></li>
   <li><p><b>[!UICONTROL Elimina]</b></p><p> Per i campi disponibili, vedi <a href="#delete-record" class="MCXref xref" >[!UICONTROL Eliminare un record]</a> in questo articolo. </p></li>
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
   <td>Per istruzioni su come creare una connessione a [!DNL Adobe Campaign Classic], vedi <a href="#connect-adobe-campaign-connector-to-adobe-workfront-fusion" class="MCXref xref" >Creare una connessione a [!DNL Adobe Campaign Classic]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Seleziona il tipo di [!DNL Adobe Campaign Classic] record che si desidera leggere.</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL ID] </td> 
   <td>Immettere l'ID del record da leggere.</td> 
  </tr> 
 <tr> 
   <td role="rowheader">[!UICONTROL Campi da includere nell’output] </td> 
   <td>Seleziona i campi da includere nell’output del modulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campi personalizzati da includere nell’output]</td> 
   <td>Per ogni campo personalizzato che si desidera includere nell'output, fare clic su <b>[!UICONTROL Aggiungi]</b> e immettere il nome del campo personalizzato.</td> 
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL Abbonati o annulla sottoscrizione]

Questo modulo di azione sottoscrive o annulla l’abbonamento di un utente a un servizio di informazione.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Per istruzioni su come creare una connessione a [!DNL Adobe Campaign Classic], vedi <a href="#connect-adobe-campaign-connector-to-adobe-workfront-fusion" class="MCXref xref" >Creare una connessione a [!DNL Adobe Campaign Classic]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Iscriviti o annulla sottoscrizione]</td> 
   <td>Seleziona se desideri abbonarti o annullare l’abbonamento al servizio informazioni.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome servizio]</td> 
   <td>Seleziona il servizio a cui vuoi abbonarti o di cui vuoi annullare l’abbonamento.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Indirizzo e-mail destinatario] </td> 
   <td>Immetti o mappa l’indirizzo e-mail dell’utente che desideri sottoscrivere o annullare l’iscrizione al servizio informazioni.</td> 
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
   <td>Per istruzioni su come creare una connessione a [!DNL Adobe Campaign Classic], vedi <a href="#connect-adobe-campaign-connector-to-adobe-workfront-fusion" class="MCXref xref" >Creare una connessione a [!DNL Adobe Campaign Classic]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Seleziona il tipo di [!DNL Adobe Campaign Classic] record da creare.</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL ID] </td> 
   <td>Immettere l'ID del record da aggiornare.</td> 
  </tr> 
<tr> 
   <td role="rowheader">[!UICONTROL Fields] </td> 
   <td>Seleziona i campi per i quali desideri aggiornare i valori, quindi compila i valori per tali campi. I campi variano in base al tipo di record selezionato.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campi personalizzati]</td> 
   <td> Per ogni campo personalizzato che si desidera aggiornare, fare clic su <b>[!UICONTROL Aggiungi elemento]</b> e immettere o mappare il nome e il valore del campo. </td> 
  </tr> 
 </tbody> 
</table>

### Ricerche

#### [!UICONTROL Ricerca]

Questo modulo di ricerca restituisce i record in base ai criteri specificati.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Per istruzioni su come creare una connessione a [!DNL Adobe Campaign Classic], vedi <a href="#connect-adobe-campaign-connector-to-adobe-workfront-fusion" class="MCXref xref" >Creare una connessione a [!DNL Adobe Campaign Classic]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Seleziona il tipo di [!DNL Adobe Campaign Classic] record da creare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td>Immettere o mappare il numero massimo di record che si desidera restituire dal modulo durante ogni ciclo di esecuzione degli scenari.</td> 
  </tr> 
 </tbody> 
</table>
