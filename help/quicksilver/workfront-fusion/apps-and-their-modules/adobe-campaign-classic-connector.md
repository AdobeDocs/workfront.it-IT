---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli Adobe Campaign v7/v8
description: Con il [!DNL Adobe Campaign] moduli, è possibile avviare un [!DNL Adobe Workfront Fusion] scenario basato sugli eventi nel tuo [!DNL Adobe Campaign] creare, leggere o aggiornare contratti e altri record, cercare i record utilizzando i criteri impostati e caricare i documenti.
author: Becky
feature: Workfront Fusion
exl-id: 84e8fa35-0c3c-46bd-8886-88c6d8d9e1d5
source-git-commit: 7decc5cbf4bb2c3d4d1802dec1f369ca061f6b48
workflow-type: tm+mt
source-wordcount: '1434'
ht-degree: 0%

---

# [!DNL Adobe Campaign] moduli

Con il [!DNL Adobe Campaign] moduli, è possibile avviare un [!DNL Adobe Workfront Fusion] scenario basato sugli eventi nel tuo [!DNL Adobe Campaign v7/v8] creare, leggere o aggiornare i record, cercare i record utilizzando i criteri impostati ed eseguire chiamate API personalizzate.

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

È necessario aggiungere gli indirizzi IP di Fusion a [!DNL Adobe Campaign].

* Per istruzioni sull’aggiunta di indirizzi IP al tuo elenco Consentiti di campagna di, consulta [Aggiunta di indirizzi IP al inserisco nell&#39;elenco Consentiti di](https://experienceleague.adobe.com/en/docs/control-panel/using/sftp-management/ip-range-allow-listing#adding-ip-addresses-allow-list) nella documentazione di Adobe Campaign.
* Per un elenco di indirizzi IP da aggiungere al inserisco nell&#39;elenco Consentiti di, consulta [Indirizzi IP per l&#39;accesso ad Adobe Workfront Fusion](/help/quicksilver/workfront-fusion/get-started/ip-addresses-for-fusion.md).

## Connetti [!DNL Adobe Campaign] a [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>Si consiglia vivamente di creare una connessione server-to-server. Adobe Campaign ha aggiornato la propria API per accettare solo connessioni server-to-server. Se ti connetti a Campaign versione 8 o successiva, **deve** creare una connessione server-to-server.
>
>Per ulteriori informazioni sui nuovi requisiti di connessione di Campaign, consulta [Migrazione degli operatori tecnici di Campaign alla console Adobe Developer](https://experienceleague.adobe.com/docs/campaign/technotes-ac/tn-new/ims-migration.html) nella documentazione di Campaign.

1. In qualsiasi [!DNL Adobe Campaign] modulo, fai clic su **[!UICONTROL Aggiungi]** accanto al [!UICONTROL Connessione] campo.
1. Compila i campi seguenti:
   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
          <td role="rowheader">[!UICONTROL Tipo di connessione]</td>
          <td>
            <p>Selezionare se si sta creando una connessione di base o una connessione da server a server.</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Nome connessione]</td>
          <td>
            <p>Immettere un nome per la connessione.</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL URL di base]</td>
          <td>Immetti l’URL di base da utilizzare per la connessione al tuo [!DNL Adobe Campaign] dell'istanza.</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Username]</td>
          <td>Se stai creando una connessione di base, immetti il tuo nome utente Adobe Campaign.</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Password]</td>
          <td>Se stai creando una connessione di base, immetti la password di Adobe Campaign.</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL ID client]</td>
          <td>Se si sta creando una connessione server-to-server, immettere [!DNL Adobe] [!UICONTROL ID client]. È disponibile nella sezione [!UICONTROL Credentials details] del file [!DNL Adobe Developer Console].</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Segreto client]</td>
          <td>Se si sta creando una connessione server-to-server, immettere [!DNL Adobe] [!UICONTROL Segreto Client]. È disponibile nella sezione [!UICONTROL Credentials details] del file [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Environment]</td>
          <td>Seleziona se sei connesso a un ambiente di produzione o non di produzione.
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Type]</td>
          <td>Specificare se ci si connette a un account di servizio o a un account personale.
        </tr>
   </tbody>
    </table>
1. Clic **[!UICONTROL Continua]** per creare la connessione e tornare al modulo.

## [!DNL Adobe Campaign] moduli e relativi campi

Quando si configura [!DNL Adobe Campaign] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL Adobe Campaign] I campi potrebbero essere visualizzati in base a fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

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
   <td>Per istruzioni sulla creazione di una connessione a [!DNL Adobe Campaign], vedi <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Creare una connessione a [!DNL Adobe Campaign]</a> in questo articolo.</td> 
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

Questo modulo di azione crea un nuovo record in [!DNL Adobe Campaign].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Per istruzioni sulla creazione di una connessione a [!DNL Adobe Campaign], vedi <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Creare una connessione a [!DNL Adobe Campaign]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Seleziona il tipo di [!DNL Adobe Campaign] record da creare.</td> 
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

Questo modulo effettua una chiamata API personalizzata al [!DNL Adobe Campaign] API

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Per istruzioni sulla creazione di una connessione a [!DNL Adobe Campaign], vedi <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Creare una connessione a [!DNL Adobe Campaign]</a> in questo articolo.</td> 
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

Questo modulo di azione elimina un singolo record da [!DNL Adobe Campaign].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Per istruzioni sulla creazione di una connessione a [!DNL Adobe Campaign], vedi <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Creare una connessione a [!DNL Adobe Campaign]</a> in questo articolo.</td> 
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

Questo modulo di azione esegue un&#39;azione selezionata su un oggetto in [!DNL Adobe Campaign] API.

Per informazioni su azioni e campi specifici, consulta [[!DNL Adobe Campaign] - Documentazione API](https://experienceleague.adobe.com/developer/campaign-api/api/p-14.html).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Per istruzioni sulla creazione di una connessione a [!DNL Adobe Campaign], vedi <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Creare una connessione a [!DNL Adobe Campaign]</a> in questo articolo.</td> 
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

Questo modulo di azione legge un record da [!DNL Adobe Campaign].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Per istruzioni sulla creazione di una connessione a [!DNL Adobe Campaign], vedi <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Creare una connessione a [!DNL Adobe Campaign]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Seleziona il tipo di [!DNL Adobe Campaign] record da leggere.</td> 
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
   <td>Per istruzioni sulla creazione di una connessione a [!DNL Adobe Campaign], vedi <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Creare una connessione a [!DNL Adobe Campaign]</a> in questo articolo.</td> 
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

Questo modulo di azione aggiorna un singolo record in [!DNL Adobe Campaign].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Per istruzioni sulla creazione di una connessione a [!DNL Adobe Campaign], vedi <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Creare una connessione a [!DNL Adobe Campaign]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Seleziona il tipo di [!DNL Adobe Campaign] record da creare.</td> 
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
   <td>Per istruzioni sulla creazione di una connessione a [!DNL Adobe Campaign], vedi <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Creare una connessione a [!DNL Adobe Campaign]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Seleziona il tipo di [!DNL Adobe Campaign] record da creare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td>Immettere o mappare il numero massimo di record che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</td> 
  </tr> 
 </tbody> 
</table>
