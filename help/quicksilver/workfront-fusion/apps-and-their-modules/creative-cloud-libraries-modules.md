---
filename: creative-cloud-libraries-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Moduli delle librerie Adobe Creative Cloud
description: Con la [!DNL Adobe Workfront Fusion Adobe Creative Cloud] Moduli di librerie, puoi avviare uno scenario quando un elemento o una libreria viene creata o aggiornata. Puoi anche caricare, recuperare, archiviare o elencare elementi, oppure effettuare una chiamata al [!DNL Adobe Creative Cloud Libraries] API.
author: Becky
exl-id: 8affa34b-803d-48a5-a986-9fbe0cb8c8f5
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1193'
ht-degree: 0%

---

# Moduli delle librerie Adobe Creative Cloud

Con la [!DNL Adobe Workfront Fusion] [!DNL Adobe Creative Cloud Libraries] moduli, puoi avviare uno scenario quando un elemento o una libreria viene creata o aggiornata. Puoi anche caricare, recuperare, archiviare o elencare elementi, oppure effettuare una chiamata al [!DNL Adobe Creative Cloud Libraries] API.

Se hai bisogno di istruzioni su come creare uno scenario, vedi [Creare uno scenario](../../workfront-fusion/scenarios/create-a-scenario.md).

Per informazioni sui moduli, consulta [Moduli in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Requisiti di accesso

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] piano*</td>
      <td>
        <p>[!UICONTROL Pro] o superiore</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] licenza*</td>
      <td>
        <p>[!UICONTROL Plan], [!UICONTROL Work]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront Fusion] licenza**</td>
      <td >
        <p>[!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro]</p>
      </td>
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

Per utilizzare [!DNL Adobe Creative Cloud Libraries] moduli, è necessario disporre di un [!UICONTROL Adobe Creative Cloud] conto.

## [!UICONTROL Librerie Adobe Creative Cloud] moduli e relativi campi

Quando si configura [!UICONTROL Librerie Adobe Creative Cloud] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL Adobe Creative Cloud Libraries] potrebbero essere visualizzati, a seconda di fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se trovi il pulsante mappa sopra un campo o una funzione, puoi utilizzarlo per impostare variabili e funzioni per quel campo. Per ulteriori informazioni, consulta [Mappare informazioni da un modulo a un altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)


* [Elementi](#elements)

* [Librerie](#libraries)

* [Altro](#other)


### Elementi

* [[!UICONTROL Archiviare un elemento]](#archive-an-element)

* [[!UICONTROL Ottenere un elemento]](#get-an-element)

* [[!UICONTROL Elementi elenco]](#list-elements)

* [[!UICONTROL Caricare un elemento]](#upload-an-element)

* [!UICONTROL [Guarda nuovo elemento nella libreria]](#watch-new-element-in-library)

* [[!UICONTROL Guarda gli elementi aggiornati]](#watch-updated-elements)


#### [!UICONTROL Archiviare un elemento]

Questo modulo di azione archivia un elemento da una libreria.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Per istruzioni su come collegare le [!DNL Adobe Creative Cloud] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base.</td>
    </tr>
    <tr>
      <td role="rowheader">ID libreria [!UICONTROL]</td>
      <td >Seleziona la libreria che contiene l'elemento da archiviare.</td>
    </tr>
    <tr>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">[!UICONTROL Element ID]</td>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">Seleziona l’elemento da archiviare.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Ottenere un elemento]

Questo modulo di azione restituisce un singolo elemento da una libreria.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Per istruzioni su come collegare le [!DNL Adobe Creative Cloud] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base.</td>
    </tr>
    <tr>
      <td role="rowheader">ID libreria [!UICONTROL]</td>
      <td >Seleziona la libreria che contiene l'elemento da recuperare.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Element ID]</td>
      <td>Immetti o mappa l’ID dell’elemento da recuperare.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Selector]</td>
      <td>
        <p>Selezionare il tipo di informazioni restituito dal modulo. </p>
        <ul>
          <li>
            <p><b>[!UICONTROL Predefinito]</b>
            </p>
            <p>Dati di base</p>
          </li>
          <li>
            <p><b>[!UICONTROL Details]</b>
            </p>
            <p>Tutti i dati disponibili</p>
          </li>
          <li>
            <p><b>[!UICONTROL Rappresentanze]</b>
            </p>
            <p>Un elenco semplificato di risorse associate all’elemento libreria</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Elementi elenco]

Questo modulo di azione recupera un elenco di elementi in una libreria.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Per istruzioni su come collegare le [!DNL Adobe Creative Cloud] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base.</td>
    </tr>
    <tr>
      <td role="rowheader">ID libreria [!UICONTROL]</td>
      <td >Seleziona la libreria da cui vuoi elencare gli elementi.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Ordina per]</td>
      <td>Seleziona se desideri ordinare i risultati per nome o per l’ultima data in cui l’elemento è stato modificato.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Type]</td>
      <td >Immetti un tipo MIME per limitare i risultati agli elementi identificati con il tipo MIME specificato. Esempio: <code>string</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Selector]</td>
      <td>
        <p>Selezionare il tipo di informazioni restituito dal modulo. </p>
        <ul>
          <li>
            <p><b>[!UICONTROL Predefinito]</b>
            </p>
            <p>Dati di base</p>
          </li>
          <li>
            <p><b>[!UICONTROL Details]</b>
            </p>
            <p>Tutti i dati disponibili</p>
          </li>
          <li>
            <p><b>[!UICONTROL Rappresentanze]</b>
            </p>
            <p>Un elenco semplificato di risorse associate all’elemento libreria</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Immettere o mappare il numero massimo di record che si desidera restituire dal modulo durante ogni ciclo di esecuzione degli scenari.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Caricare un elemento]

Questo modulo di azione carica una piccola risorsa file in una libreria esistente. La dimensione massima del file è 1 GB.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Per istruzioni su come collegare le [!DNL Adobe Creative Cloud] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base.</td>
    </tr>
    <tr>
      <td role="rowheader">ID libreria [!UICONTROL]</td>
      <td >Seleziona la libreria da cui vuoi elencare gli elementi.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Invocation Mode]</td>
      <td>
        <p>Selezionare la modalità di elaborazione con cui richiamare il processo di richiesta.</p>
        <ul>
          <li>
            <p><b>[!UICONTROL sync]</b>
            </p>
            <p>La chiamata API viene elaborata in modo sincrono. La risposta viene recapitata al termine dell’elaborazione (a meno che la chiamata non termini).</p>
          </li>
          <li>
            <p><b>[!UICONTROL async]</b>
            </p>
            <p>La risposta del monitoraggio asincrono viene restituita immediatamente e l'elaborazione della richiesta avviene in modo asincrono. La chiamata è responsabile del polling dell'endpoint fino al completamento.</p>
          </li>
          <li>
            <p><b>[!UICONTROL sync,async]</b> (Predefinito)</p>
            <p>Tentativo di elaborazione sincrona della richiesta. Quando l’elaborazione si estende oltre 5000 ms, viene restituita la risposta del monitoraggio asincrono. L’URL del monitoraggio deve essere controllato fino al completamento della richiesta.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Type File]</td>
      <td >Immetti o mappa il tipo MIME del file caricato.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL File di origine]</td>
      <td>
        <p>Selezionare un file di origine da un modulo precedente o mappare il nome e i dati del file di origine.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Guarda nuovo elemento nella libreria]

Questo modulo di attivazione avvia uno scenario in cui un elemento viene aggiunto a una libreria.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Per istruzioni su come collegare le [!DNL Adobe Creative Cloud] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base.</td>
    </tr>
    <tr>
      <td role="rowheader">ID libreria [!UICONTROL]</td>
      <td >Seleziona la libreria di cui desideri tenere traccia per gli elementi aggiornati.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Immettere o mappare il numero massimo di record che si desidera restituire dal modulo durante ogni ciclo di esecuzione degli scenari.</td>
    </tr>
  </tbody>
</table>


#### [!UICONTROL Guarda gli elementi aggiornati]

Questo modulo di attivazione avvia uno scenario in cui viene aggiornato un elemento in una libreria.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Per istruzioni su come collegare le [!DNL Adobe Creative Cloud] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base.</td>
    </tr>
    <tr>
      <td role="rowheader">ID libreria [!UICONTROL]</td>
      <td >Seleziona la libreria di cui desideri tenere traccia per individuare i nuovi elementi.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Immettere o mappare il numero massimo di record che si desidera restituire dal modulo durante ogni ciclo di esecuzione degli scenari.</td>
    </tr>
  </tbody>
</table>

### Librerie

* [[!UICONTROL Guarda nuove librerie]](#watch-new-libraries)

* [[!UICONTROL Guarda le librerie aggiornate]](#watch-updated-libraries)


#### [!UICONTROL Guarda nuove librerie]

Questo modulo di attivazione avvia uno scenario quando viene creata una nuova libreria.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Per istruzioni su come collegare le [!DNL Adobe Creative Cloud] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Immettere o mappare il numero massimo di record che si desidera restituire dal modulo durante ogni ciclo di esecuzione degli scenari.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Guarda le librerie aggiornate]

Questo modulo di attivazione avvia uno scenario in cui viene aggiornata una libreria esistente.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Per istruzioni su come collegare le [!DNL Adobe Creative Cloud] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Immettere o mappare il numero massimo di record che si desidera restituire dal modulo durante ogni ciclo di esecuzione degli scenari.</td>
    </tr>
  </tbody>
</table>

### Altro

#### [!UICONTROL Effettuare una chiamata API]

Questo modulo effettua una chiamata API personalizzata al [!DNL Adobe Creative Cloud Libraries] API.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Per istruzioni su come collegare il tuo account Adobe Creative Cloud a Workfront Fusion, vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione ad Adobe Workfront Fusion - Istruzioni di base.</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]</td>
      <td>
        <p>Immettere un percorso relativo a <code>https://cc-libraries.adobe.io/api</code>.</p>
    <p>Ad esempio <code>/v1/libraries</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL API versione]</td>
      <td>
        <p>Seleziona la versione del [!DNL Adobe Analytics] API a cui desideri connetterti.</p>
      </td>
    </tr>    <tr>
      <td role="rowheader">[!UICONTROL, Metodo]</td>
      <td> <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>Aggiungi le intestazioni della richiesta sotto forma di un oggetto JSON standard.</p>
        <p>Ad esempio: <code>{"Content-type":"application/json"}</code></p>
        <p>Workfront Fusion aggiunge le intestazioni di autorizzazione.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Query String]</td>
      <td>
        <p>Aggiungi la query per la chiamata API sotto forma di un oggetto JSON standard.</p>
        <p>Ad esempio: <code>{"name":"something-urgent"}</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>Aggiungi il contenuto del corpo per la chiamata API sotto forma di un oggetto JSON standard.</p> <p>Nota:  <p>Quando si utilizzano istruzioni condizionali come <code>if</code> nel JSON, inserisci le virgolette al di fuori dell’istruzione condizionale.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
       <tr>
      <td role="rowheader">[!UICONTROL Caricare un documento transitorio]</td>
      <td>
      <p>Se si desidera caricare un documento transitorio, immettere il file di origine del documento da caricare.</p>
      <p>Selezionare un file di origine da un modulo precedente o mappare il nome e i dati del file di origine.</p>
    </td>
    </tr>

</tbody>
</table>
