---
filename: workday-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli Workday
description: In uno scenario Adobe Workfront Fusion, è possibile automatizzare i flussi di lavoro che utilizzano [!DNL Workday], nonché collegarlo a più applicazioni e servizi di terze parti.
author: Becky
exl-id: 535573e0-b6ad-43a2-b7cb-ed32d1dc8d16
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '965'
ht-degree: 2%

---

# [!DNL Workday] moduli

In un [!DNL Adobe Workfront Fusion] puoi automatizzare i flussi di lavoro che utilizzano [!DNL Workday], nonché collegarlo a più applicazioni e servizi di terze parti.

Se hai bisogno di istruzioni su come creare uno scenario, vedi [Crea uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Per informazioni sui moduli, consulta [Moduli in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

Per utilizzare [!DNL Workday] moduli, è necessario:

* Avere [!DNL Workday] conto.

* Creare un’applicazione OAuth in [!DNL Workday]. Per istruzioni, consulta la sezione [!DNL Workday] documentazione.

## Connetti [!DNL Workday] a [!DNL Workfront Fusion]

1. In qualsiasi [!DNL Workfront Fusion] modulo, fai clic su [!UICONTROL Aggiungi] accanto al [!UICONTROL Connessione] field

2. Compila i campi seguenti:

   <table style="table-layout:auto"> 
        <col/>
        <col/>
        <tbody>
            <tr>
                <td role="rowheader">
                    <p role="rowheader">[!UICONTROL Nome connessione]</p>
                </td>
                <td>Immettere un nome per la connessione</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Workday host]</td>
                <td>Inserisci l'indirizzo del tuo [!DNL Workday] host senza <code>https://</code>. Ad esempio: <code>mycompany.workday.com</code>.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Services URL]</td>
                <td>Inserisci l'indirizzo del tuo [!DNL Workday] servizi web senza <code>https://</code>. Ad esempio: <code>mycompany-services.workday.com</code>.</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Nome tenant]</td>
                <td>Immetti il tenant per questo [!DNL Workday] conto. Il tenant è l’identificatore dell’organizzazione e può essere visualizzato nell’URL utilizzato per accedere a Workday. Esempio: all'indirizzo <code>https://www.myworkday.com/mycompany</code>, il tenant è <code>mycompany</code>.</td>
            </tr>
            <tr>
                <td role="rowheader">ID client [!UICONTROL]</td>
                <td>Immetti l’ID client per il [!DNL Workday] applicazione utilizzata da questa connessione. Puoi ottenere questo risultato quando crei l'applicazione in [!DNL Workday].</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Segreto client]</td>
                <td>Inserisci il segreto client per il [!DNL Workday] applicazione utilizzata da questa connessione. Puoi ottenere questo risultato quando crei l'applicazione in [!DNL Workday].</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Timeout sessione (min)]</td>
                <td >Immetti il numero di minuti dopo la scadenza del token di autorizzazione.</td>
            </tr>
        </tbody>
    </table>


3. Fai clic su [!UICONTROL Continua] per salvare la connessione e tornare al modulo

## [!DNL Workday] moduli e relativi campi

Quando si configura [!DNL Workday] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL Workday] potrebbero essere visualizzati, a seconda di fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se trovi il pulsante mappa sopra un campo o una funzione, puoi utilizzarlo per impostare variabili e funzioni per quel campo. Per ulteriori informazioni, consulta [Mappare informazioni da un modulo a un altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Azione](#action)

* [Ricerca](#search)


### Azione

* [[!UICONTROL Creare un record]](#create-a-record)

* [[!UICONTROL Eliminare un record]](#delete-a-record)

* [[!UICONTROL Effettuare una chiamata API personalizzata]](#make-a-custom-api-call)

* [[!UICONTROL Aggiornare un record]](#update-a-record)


#### [!UICONTROL Creare un record]

Questo modulo di azione crea un record singolo in [!DNL Workday].

<table style="table-layout:auto"> 
    <col/>
    <col/>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL Connection]</td>
            <td>Per istruzioni su come collegare le [!DNL Workday] account a Workfront Fusion, vedi <a href="#Connect" class="MCXref xre[!DNL ]f" >Connetti [!DNL Workday] a [!DNL Workfront Fusion]</a>.</td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL Tipo di record]</td>
            <td>Selezionare il tipo di record che si desidera creare.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td>Immettere o mappare l'ID del record che si desidera creare.</td>
        </tr>
        <tr>
            <td role="rowheader">ID [!UICONTROL SOTTOsorgente]</td>
            <td >Immetti o mappa l’ID della risorsa secondaria che desideri creare.</td>
        </tr>
    </tbody>
</table>

#### [!UICONTROL Eliminare un record]

Questo modulo di azione elimina un record singolo in [!DNL Workday].

<table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL Connection]</td>
            <td>Per istruzioni su come collegare le [!DNL Workday] account a [!DNL Workfront Fusion], vedi <a href="#Connect" class="MCXref xre[!DNL ]f" >Connetti [!DNL Workday] a [!DNL Workfront Fusion]</a>.</td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL Tipo di record]</td>
            <td>Selezionare il tipo di record da eliminare.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL Tipo di record specifico]</td>
            <td>Selezionare il tipo di record specifico che si desidera eliminare. Questi si basano sul tipo di record scelto.</td>
        </tr>
        <tr>
            <td  role="rowheader">ID [!UICONTROL SOTTOsorgente]</td>
            <td>Immetti o mappa l’ID della risorsa secondaria che desideri eliminare.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td >Immettere o mappare l'ID del record che si desidera eliminare.</td>
        </tr>
    </tbody>
</table>


### [!UICONTROL Effettuare una chiamata API personalizzata]

Questo modulo di azione ti consente di effettuare una chiamata autenticata personalizzata al [!DNL Workday] API. In questo modo, puoi creare un’automazione del flusso di dati che non può essere eseguita dall’altro [!DNL Workday] moduli.

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

Il modulo restituisce il codice di stato a, insieme alle intestazioni e al corpo della chiamata API.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Connection]</p> </td> 
            <td>Per istruzioni su come collegare le [!DNL Workday] account a [!DNL Workfront Fusion], vedi <a href="#Connect" class="MCXref xre[!DNL ]f" >Connetti [!DNL Workday] a [!DNL Workfront Fusion]</a>.</td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Immettere un percorso relativo a <code style="color: #ff1493;">https://&lt;tenantHostname>/api/&lt;serviceName>/&lt;version>/&lt;tenant></code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL, Metodo]</td> 
   <td> <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Aggiungi le intestazioni della richiesta sotto forma di un oggetto JSON standard.</p> <p>Ad esempio: <code>{"Content-type":"application/json"}</code></p> <p>[!UICONTROL Workfront Fusion] aggiunge le intestazioni di autorizzazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>Aggiungi la query per la chiamata API sotto forma di un oggetto JSON standard.</p> <p>Ad esempio: <code>{"name":"something-urgent"}</code></p> </td> 
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

#### [!UICONTROL Aggiornare un record]

Questo modulo di azione aggiorna un singolo record in [!DNL Workday].

<table style="table-layout:auto"> 
    <col/>
    <col/>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL Connection]</td>
            <td>Per istruzioni su come collegare le [!DNL Workday] account a Workfront Fusion, vedi <a href="#Connect" class="MCXref xref" >[!UICONTROL Connect [!DNL Workday] a Workfront Fusion]</a></td>
        </tr>
        <tr>
            <td  role="rowheader">Tipo di record</td>
            <td>Selezionare il tipo di record t[!UICONTROL ]che si desidera aggiornare.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td>Immettere o mappare l'ID del record che si desidera aggiornare.</td>
        </tr>
        <tr>
            <td role="rowheader">ID [!UICONTROL SOTTOsorgente]</td>
            <td >Immetti o mappa l’ID della risorsa secondaria che desideri aggiornare.</td>
        </tr>
    </tbody>
</table>

### Ricerca

* [[!UICONTROL Leggi un record]](#read-a-record)

* [[!UICONTROL Elencare record]](#list-records)


#### [!UICONTROL Leggi un record]

Questo modulo di azione legge un record singolo.

<table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL Connection]</td>
            <td>Per istruzioni su come collegare le [!DNL Workday] account a Workfront Fusion, vedi <a href="#Connect" class="MCXref xref" >[!UICONTROL Connect [!DNL Workday] a Workfront Fusion]</a></td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL Tipo di record]</td>
            <td>Selezionare il tipo di record da eliminare.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL Tipo di record specifico]</td>
            <td>Selezionare il tipo di record specifico che si desidera leggere. Questi si basano sul tipo di record scelto.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td >Immettere o mappare l'ID del record che si desidera eliminare.</td>
        </tr>
    </tbody>
</table>

#### [!UICONTROL Elencare record]

Questo modulo di ricerca recupera un elenco di record del tipo specificato.

<table style="table-layout:auto"> 
      <col/>
      <col/>
      <tbody>
          <tr>
              <td role="rowheader">[!UICONTROL Connection]</td>
              <td>Per istruzioni su come collegare le [!DNL Workday] account a [!DNL Workfront Fusion], vedi <a href="#Connect" class="MCXref xref" >Connetti [!DNL Workday] a [!DNL Workfront Fusion]</a></td>
          </tr>
          <tr>
              <td  role="rowheader">[!UICONTROL Tipo di record]</td>
              <td>Selezionare il tipo di record da recuperare.</td>
          </tr>
          <tr>
              <td role="rowheader">[!UICONTROL Limit]</td>
              <td >
                  <p>Immettere o mappare il numero massimo di record che si desidera recuperare dal modulo durante ogni ciclo di esecuzione degli scenari.</p>
              </td>
          </tr>
      </tbody>
  </table>
