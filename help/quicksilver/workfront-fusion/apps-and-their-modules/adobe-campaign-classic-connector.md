---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli Adobe Campaign v7/v8
description: La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione. Questo articolo è stato dichiarato obsoleto, ma contiene un collegamento al nuovo articolo che descrive questa funzionalità.
author: Becky
feature: Workfront Fusion
exl-id: 84e8fa35-0c3c-46bd-8886-88c6d8d9e1d5
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1490'
ht-degree: 1%

---

# [!DNL Adobe Campaign] moduli

>[!IMPORTANT]
>
>La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione.
>
>Le informazioni contenute in questo articolo sono ora disponibili nell’articolo:
>
>* [Moduli Adobe Campaign](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/adobe-connectors/adobe-campaign-classic-connector.html)
>
>Aggiorna eventuali segnalibri.
>
>Questo articolo non è più in fase di aggiornamento e verrà rimosso nel prossimo futuro.

Con i moduli [!DNL Adobe Campaign], puoi avviare uno scenario [!DNL Adobe Workfront Fusion] basato sugli eventi nell&#39;account [!DNL Adobe Campaign v7/v8], creare, leggere o aggiornare record, cercare record utilizzando i criteri impostati ed eseguire chiamate API personalizzate.

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

Aggiungere gli indirizzi IP di Fusion a [!DNL Adobe Campaign].

* Per istruzioni sull&#39;aggiunta di indirizzi IP al inserisco nell&#39;elenco Consentiti di targeting di Campaign, consulta [Aggiunta di indirizzi IP al Adobe Campaign di targeting di](https://experienceleague.adobe.com/en/docs/control-panel/using/sftp-management/ip-range-allow-listing#adding-ip-addresses-allow-list) nella documentazione di inserire nell&#39;elenco Consentiti.
* Per un elenco di indirizzi IP da aggiungere al inserisco nell&#39;elenco Consentiti di, vedere [Indirizzi IP per accedere ad Adobe Workfront Fusion](/help/quicksilver/workfront-fusion/get-started/ip-addresses-for-fusion.md).

## Informazioni API di Adobe Campaign

Il connettore Adobe Campaign utilizza quanto segue:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Tag API</td> 
   <td>v1.7.22</td> 
  </tr>
 </tbody> 
 </table>

## Connetti [!DNL Adobe Campaign] a [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>Si consiglia vivamente di creare una connessione server-to-server. Adobe Campaign ha aggiornato la propria API per accettare solo connessioni server-to-server. Se ti connetti a Campaign versione 8 o successiva, **devi** creare una connessione server-to-server.
>
>Per ulteriori informazioni sui nuovi requisiti di connessione di Campaign, consulta [Migrazione degli operatori tecnici di Campaign a Adobe Developer Console](https://experienceleague.adobe.com/docs/campaign/technotes-ac/tn-new/ims-migration.html) nella documentazione di Campaign.

1. In qualsiasi modulo [!DNL Adobe Campaign], fai clic su **[!UICONTROL Aggiungi]** accanto al campo [!UICONTROL Connessione].
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
          <td>Immettere l'URL di base utilizzato per connettersi all'istanza [!DNL Adobe Campaign].</td>
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
          <td>Se si sta creando una connessione server-to-server, immettere l'ID client [!DNL Adobe] [!UICONTROL]. È disponibile nella sezione [!UICONTROL Credentials details] di [!DNL Adobe Developer Console].</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Segreto client]</td>
          <td>Se si sta creando una connessione server-to-server, immettere [!DNL Adobe] [!UICONTROL Client Secret]. È disponibile nella sezione [!UICONTROL Credentials details] di [!DNL Adobe Developer Console].
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
1. Fai clic su **[!UICONTROL Continua]** per creare la connessione e tornare al modulo.

## [!DNL Adobe Campaign] moduli e relativi campi

Quando configuri [!DNL Adobe Campaign] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Insieme a questi, potrebbero essere visualizzati ulteriori campi di [!DNL Adobe Campaign], a seconda di fattori quali il livello di accesso nell&#39;app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se viene visualizzato il pulsante Mappa sopra un campo o una funzione, è possibile utilizzarlo per impostare variabili e funzioni per tale campo. Per ulteriori informazioni, vedere [Mappare le informazioni da un modulo all&#39;altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Azioni](#actions)
* [Ricerche](#searches)

### Triggers

#### [!UICONTROL Osserva record]

Questo modulo di attivazione pianificato avvia uno scenario quando un record cambia.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Per istruzioni sulla creazione di una connessione a [!DNL Adobe Campaign], vedere <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Creare una connessione a [!DNL Adobe Campaign]</a> in questo articolo.</td> 
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
   <td>Per ogni campo personalizzato da includere nell'output, fare clic su <b>[!UICONTROL Add]</b> e immettere il nome del campo personalizzato.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Numero massimo di risultati restituiti]</td> 
   <td>Immettere o mappare il numero massimo di record che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</td> 
  </tr> 
 </tbody> 
</table>


### Azioni

* [[!UICONTROL Crea un record]](#create-a-record)
* [[!UICONTROL Effettuare una chiamata API personalizzata]](#make-a-custom-api-call)
* [[!UICONTROL Eliminare un record]](#delete-record)
* [[!UICONTROL Esegui un&#39;azione]](#perform-an-action)
* [[!UICONTROL Leggi un record]](#-read-a-record)
* [[!UICONTROL Sottoscrizione o annullamento dell&#39;iscrizione]](#subscribe-or-unsubscribe)
* [[!UICONTROL Aggiorna un record]](#update-record)

#### [!UICONTROL Crea un record]

Questo modulo azioni crea un nuovo record in [!DNL Adobe Campaign].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Per istruzioni sulla creazione di una connessione a [!DNL Adobe Campaign], vedere <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Creare una connessione a [!DNL Adobe Campaign]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Selezionare il tipo di record [!DNL Adobe Campaign] da creare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fields] </td> 
   <td>Selezionare i campi per i quali si desidera impostare i valori al momento della creazione del record, quindi immettere i valori per tali campi. I campi variano in base al tipo di record selezionato.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campi personalizzati]</td> 
   <td> Per ogni campo personalizzato che si desidera aggiungere al nuovo record, fare clic su <b>[!UICONTROL Add item]</b> e immettere o associare il nome e il valore del campo. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Effettuare una chiamata API personalizzata]

Questo modulo effettua una chiamata API personalizzata all&#39;API [!DNL Adobe Campaign]

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Per istruzioni sulla creazione di una connessione a [!DNL Adobe Campaign], vedere <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Creare una connessione a [!DNL Adobe Campaign]</a> in questo articolo.</td> 
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
   <td>Per istruzioni sulla creazione di una connessione a [!DNL Adobe Campaign], vedere <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Creare una connessione a [!DNL Adobe Campaign]</a> in questo articolo.</td> 
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


#### [!UICONTROL Esegui un&#39;azione]

Questo modulo di azione esegue un&#39;azione selezionata su un oggetto nell&#39;API [!DNL Adobe Campaign].

Per informazioni su azioni e campi specifici, vedere [[!DNL Adobe Campaign] - Documentazione API](https://experienceleague.adobe.com/developer/campaign-api/api/p-14.html).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Per istruzioni sulla creazione di una connessione a [!DNL Adobe Campaign], vedere <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Creare una connessione a [!DNL Adobe Campaign]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Action]</td> 
   <td><p>Selezionare l'azione da eseguire sull'oggetto.</p>
   <ul>
   <li><p><b>[!DNL List]</b></p><p> Per i campi disponibili, vedere <a href="#search" class="MCXref xref" >[!UICONTROL Search]</a> in questo articolo. </p></li>
     <li><p><b>[!UICONTROL Get]</b></p><p> Per i campi disponibili, vedere <a href="#search" class="MCXref xref" >[!UICONTROL Search]</a> in questo articolo. </p></li> 
   <li><p><b>[!UICONTROL Crea]</b></p><p> Per i campi disponibili, vedere <a href="#create-a-record" class="MCXref xref" >[!UICONTROL Create a record]</a> in questo articolo. </p></li>
   <li><p><b>[!UICONTROL Update]</b></p><p> Per i campi disponibili, vedere <a href="#update-record" class="MCXref xref" >[!UICONTROL Update a record]</a> in questo articolo. </p></li>
   <li><p><b>[!UICONTROL Elimina]</b></p><p> Per i campi disponibili, vedere <a href="#delete-record" class="MCXref xref" >[!UICONTROL Eliminare un record]</a> in questo articolo. </p></li>
   </ul>
   </td>
</tr> 
 </tbody> 
</table>

#### [!UICONTROL Leggi un record]

Questo modulo di azione legge un record di [!DNL Adobe Campaign].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Per istruzioni sulla creazione di una connessione a [!DNL Adobe Campaign], vedere <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Creare una connessione a [!DNL Adobe Campaign]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Selezionare il tipo di record [!DNL Adobe Campaign] da leggere.</td> 
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
   <td>Per ogni campo personalizzato da includere nell'output, fare clic su <b>[!UICONTROL Add]</b> e immettere il nome del campo personalizzato.</td> 
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL Sottoscrizione o annullamento dell&#39;iscrizione]

Questo modulo di azione sottoscrive o annulla l&#39;abbonamento di un utente a un servizio di informazioni.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Per istruzioni sulla creazione di una connessione a [!DNL Adobe Campaign], vedere <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Creare una connessione a [!DNL Adobe Campaign]</a> in questo articolo.</td> 
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
   <td>Per istruzioni sulla creazione di una connessione a [!DNL Adobe Campaign], vedere <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Creare una connessione a [!DNL Adobe Campaign]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Selezionare il tipo di record [!DNL Adobe Campaign] da creare.</td> 
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
   <td> Per ogni campo personalizzato che si desidera aggiornare, fare clic su <b>[!UICONTROL Add item]</b> e immettere o mappare il nome e il valore del campo. </td> 
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
   <td>Per istruzioni sulla creazione di una connessione a [!DNL Adobe Campaign], vedere <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Creare una connessione a [!DNL Adobe Campaign]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Selezionare il tipo di record [!DNL Adobe Campaign] da creare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td>Immettere o mappare il numero massimo di record che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</td> 
  </tr> 
 </tbody> 
</table>
