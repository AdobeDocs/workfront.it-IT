---
filename: workday-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli Workday
description: In uno scenario Adobe Workfront Fusion, puoi automatizzare i flussi di lavoro che utilizzano [!DNL Workday], oltre a collegarlo a più applicazioni e servizi di terze parti.
author: Becky
exl-id: 535573e0-b6ad-43a2-b7cb-ed32d1dc8d16
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1013'
ht-degree: 2%

---

# [!DNL Workday] moduli

In un [!DNL Adobe Workfront Fusion] scenario, puoi automatizzare i flussi di lavoro che utilizzano [!DNL Workday], oltre a collegarlo a più applicazioni e servizi di terze parti.

Per istruzioni sulla creazione di uno scenario, consulta [Creare uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Per informazioni sui moduli, consulta [Moduli in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

Per utilizzare [!DNL Workday] moduli, è necessario:

* Avere un [!DNL Workday] account.

* Creare un’applicazione OAuth in [!DNL Workday]. Per istruzioni, vedere [!DNL Workday] documentazione.

## Connetti [!DNL Workday] a [!DNL Workfront Fusion]

1. In qualsiasi [!DNL Workfront Fusion] modulo, fai clic su [!UICONTROL Aggiungi] accanto al [!UICONTROL Connessione] campo

2. Compila i campi seguenti:

   <table style="table-layout:auto"> 
        <col/>
        <col/>
        <tbody>
            <tr>
                <td role="rowheader">
                    <p role="rowheader">[!UICONTROL Nome connessione]</p>
                </td>
                <td>Immetti un nome per la connessione</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Workday host]</td>
                <td>Inserisci l’indirizzo del tuo [!DNL Workday] host senza <code>https://</code>. Ad esempio: <code>mycompany.workday.com</code>.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL URL servizi]</td>
                <td>Inserisci l’indirizzo del tuo [!DNL Workday] servizi web senza <code>https://</code>. Ad esempio: <code>mycompany-services.workday.com</code>.</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Nome tenant]</td>
                <td>Immetti il tenant per questo [!DNL Workday] account. Il tenant è l'identificatore dell'organizzazione ed è visibile nell'URL utilizzato per accedere a Workday. Esempio: nell’indirizzo <code>https://www.myworkday.com/mycompany</code>, il tenant è <code>mycompany</code>.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL ID client]</td>
                <td>Immetti l'ID client per [!DNL Workday] applicazione utilizzata da questa connessione. Otteni questo risultato quando crei l’applicazione in [!DNL Workday].</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Segreto client]</td>
                <td>Immetti il segreto client per [!DNL Workday] applicazione utilizzata da questa connessione. Otteni questo risultato quando crei l’applicazione in [!DNL Workday].</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Session timeout (min)]</td>
                <td >Immetti il numero di minuti dopo i quali scade il token di autorizzazione.</td>
            </tr>
        </tbody>
    </table>


3. Clic [!UICONTROL Continua] per salvare la connessione e tornare al modulo

## [!DNL Workday] moduli e relativi campi

Quando si configura [!DNL Workday] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL Workday] I campi potrebbero essere visualizzati in base a fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se viene visualizzato il pulsante Mappa sopra un campo o una funzione, è possibile utilizzarlo per impostare variabili e funzioni per tale campo. Per ulteriori informazioni, consulta [Mappare le informazioni da un modulo all’altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Azione](#action)

* [Ricerca](#search)


### Azione

* [[!UICONTROL Creare un record]](#create-a-record)

* [[!UICONTROL Eliminare un record]](#delete-a-record)

* [[!UICONTROL Effettuare una chiamata API personalizzata]](#make-a-custom-api-call)

* [[!UICONTROL Aggiornare un record]](#update-a-record)


#### [!UICONTROL Creare un record]

Questo modulo di azione crea un singolo record in [!DNL Workday].

<table style="table-layout:auto"> 
    <col/>
    <col/>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL Connection]</td>
            <td>Per istruzioni sulla connessione [!DNL Workday] account a Workfront Fusion, vedi <a href="#Connect" class="MCXref xre[!DNL ]f" >Connetti [!DNL Workday] a [!DNL Workfront Fusion]</a>.</td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL Tipo di record]</td>
            <td>Selezionare il tipo di record da creare.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td>Inserisci o mappa l’ID del record che desideri creare.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID sottorisorsa]</td>
            <td >Immetti o mappa l’ID della risorsa secondaria da creare.</td>
        </tr>
    </tbody>
</table>

#### [!UICONTROL Eliminare un record]

Questo modulo di azione elimina un singolo record in [!DNL Workday].

<table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL Connection]</td>
            <td>Per istruzioni sulla connessione [!DNL Workday] account a [!DNL Workfront Fusion], vedi <a href="#Connect" class="MCXref xre[!DNL ]f" >Connetti [!DNL Workday] a [!DNL Workfront Fusion]</a>.</td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL Tipo di record]</td>
            <td>Selezionare il tipo di record che si desidera eliminare.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL Tipo di record specifico]</td>
            <td>Selezionare il tipo di record specifico che si desidera eliminare. Questi sono basati sul tipo di record scelto.</td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL ID sottorisorsa]</td>
            <td>Immetti o mappa l’ID della risorsa secondaria da eliminare.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td >Immettere o mappare l'ID del record che si desidera eliminare.</td>
        </tr>
    </tbody>
</table>


### [!UICONTROL Effettuare una chiamata API personalizzata]

Questo modulo di azione consente di effettuare una chiamata autenticata personalizzata al [!DNL Workday] API. In questo modo, puoi creare un’automazione del flusso di dati che non può essere eseguita dall’altro [!DNL Workday] moduli.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

Il modulo restituisce il codice di stato a, insieme alle intestazioni e al corpo della chiamata API.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Connection]</p> </td> 
            <td>Per istruzioni sulla connessione [!DNL Workday] account a [!DNL Workfront Fusion], vedi <a href="#Connect" class="MCXref xre[!DNL ]f" >Connetti [!DNL Workday] a [!DNL Workfront Fusion]</a>.</td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Inserisci un percorso relativo a <code style="color: #ff1493;">https://&lt;tenantHostname>/api/&lt;serviceName>/&lt;version>/&lt;tenant></code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Aggiungi le intestazioni della richiesta sotto forma di oggetto JSON standard.</p> <p>Ad esempio: <code>{"Content-type":"application/json"}</code></p> <p>[!UICONTROL Workfront Fusion] aggiunge automaticamente le intestazioni di autorizzazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Stringa Di Query]</td> 
   <td> <p>Aggiungi la query per la chiamata API sotto forma di oggetto JSON standard.</p> <p>Ad esempio: <code>{"name":"something-urgent"}</code></p> </td> 
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

#### [!UICONTROL Aggiornare un record]

Questo modulo di azione aggiorna un singolo record in [!DNL Workday].

<table style="table-layout:auto"> 
    <col/>
    <col/>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL Connection]</td>
            <td>Per istruzioni sulla connessione [!DNL Workday] account a Workfront Fusion, vedi <a href="#Connect" class="MCXref xref" >[!UICONTROL Connect [!DNL Workday] a Workfront Fusion]</a></td>
        </tr>
        <tr>
            <td  role="rowheader">Tipo di record</td>
            <td>Selezionare il tipo di record t[!UICONTROL ]da aggiornare.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td>Immetti o mappa l’ID del record da aggiornare.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID sottorisorsa]</td>
            <td >Immetti o mappa l’ID della risorsa secondaria da aggiornare.</td>
        </tr>
    </tbody>
</table>

### Ricerca

* [[!UICONTROL Leggi un record]](#read-a-record)

* [[!UICONTROL Elencare record]](#list-records)


#### [!UICONTROL Leggi un record]

Questo modulo di azione legge un singolo record.

<table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL Connection]</td>
            <td>Per istruzioni sulla connessione [!DNL Workday] account a Workfront Fusion, vedi <a href="#Connect" class="MCXref xref" >[!UICONTROL Connect [!DNL Workday] a Workfront Fusion]</a></td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL Tipo di record]</td>
            <td>Selezionare il tipo di record che si desidera eliminare.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL Tipo di record specifico]</td>
            <td>Selezionare il tipo di record specifico che si desidera leggere. Questi sono basati sul tipo di record scelto.</td>
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
              <td>Per istruzioni sulla connessione [!DNL Workday] account a [!DNL Workfront Fusion], vedi <a href="#Connect" class="MCXref xref" >Connetti [!DNL Workday] a [!DNL Workfront Fusion]</a></td>
          </tr>
          <tr>
              <td  role="rowheader">[!UICONTROL Tipo di record]</td>
              <td>Selezionare il tipo di record da recuperare.</td>
          </tr>
          <tr>
              <td role="rowheader">[!UICONTROL Limit]</td>
              <td >
                  <p>Immettere o mappare il numero massimo di record che il modulo deve recuperare durante ogni ciclo di esecuzione dello scenario.</p>
              </td>
          </tr>
      </tbody>
  </table>
