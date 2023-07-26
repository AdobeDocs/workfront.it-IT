---
filename: adobe-journey-optimizer-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Moduli Adobe Journey Optimizer
description: In un [!DNL Adobe Workfront Fusion] scenario, puoi automatizzare i flussi di lavoro che utilizzano [!DNL Adobe Journey Optimizer], oltre a collegarlo a più applicazioni e servizi di terze parti.
author: Becky
feature: Workfront Fusion
exl-id: 2c1aea46-edbf-42a3-a6e9-f8aea042a48d
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '1602'
ht-degree: 0%

---

# [!DNL Adobe Journey Optimizer] Moduli

<!--
Becky: pull from main, add to TOCs, then push to merge.
-->

In un [!DNL Adobe Workfront Fusion] scenario, puoi automatizzare i flussi di lavoro che utilizzano [!DNL Adobe Journey Optimizer], oltre a collegarlo a più applicazioni e servizi di terze parti. [!DNL Adobe Journey Optimizer] consente di creare, leggere, aggiornare o eliminare record oppure di eseguire una chiamata API personalizzata al [!DNL Adobe Journey Optimizer] API.


Per istruzioni sulla creazione di uno scenario, consulta [Creare uno scenario](../../workfront-fusion/scenarios/create-a-scenario.md).

Per informazioni sui moduli, consulta [Moduli in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Requisiti di accesso

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] piano*</td>
      <td>
        <p>[!UICONTROL Pro] o versione successiva</p>
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

Prima di utilizzare il [!DNL Adobe Journey Optimizer] connettore, è necessario assicurarsi che siano soddisfatti i seguenti prerequisiti:

* È necessario disporre di un [!DNL Adobe Journey Optimizer] account.

## Creare una connessione a [!DNL Adobe Journey Optimizer]

Per creare una connessione per [!DNL Adobe Journey Optimizer] moduli:

1. In qualsiasi [!DNL Adobe Journey Optimizer] modulo, fai clic su **[!UICONTROL Aggiungi]** accanto alla casella Connessione.

1. Compila i campi seguenti:

   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
          <td role="rowheader">[!UICONTROL Nome connessione]</td>
          <td>
            <p>Immettere un nome per la connessione.</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL ID client]</td>
          <td>Immetti il [!DNL Adobe] [!UICONTROL ID client]. È disponibile nella sezione [!UICONTROL Credentials details] del file [!DNL Adobe Developer Console].</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Segreto client]</td>
          <td>Immetti il [!DNL Adobe] [!UICONTROL Segreto Client]. È disponibile nella sezione [!UICONTROL Credentials details] del file [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL ID account tecnico]</td>
          <td>Immetti il [!DNL Adobe] [!UICONTROL ID account tecnico]. È disponibile nella sezione [!UICONTROL Credentials details] del file [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL ID organizzazione]</td>
          <td>Immetti il [!DNL Adobe] [!UICONTROL ID organizzazione]. È disponibile nella sezione [!UICONTROL Credentials details] del file [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Meta ambiti]</td>
          <td>
            Immetti i meta-ambiti necessari per la connessione.
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Chiave privata]</td>
          <td>
            <p>Immetti la chiave privata generata al momento della creazione delle credenziali in [!DNL Adobe Developer Console]. </p>
            <p>Per estrarre la chiave privata o il certificato:</p>
            <ol>
              <li value="1">
                <p>Clic <b>[!UICONTROL Extract]</b>.</p>
              </li>
              <li value="2">
                <p>Selezionare il tipo di file da estrarre.</p>
              </li>
              <li value="3">
                <p>Seleziona il file che contiene la chiave privata o il certificato.</p>
              </li>
              <li value="4">
                <p>Immettere la password per il file.</p>
              </li>
              <li value="5">
                <p>Clic <b>[!UICONTROL Salva]</b> per estrarre il file e tornare alla configurazione della connessione.</p>
              </li>
            </ol>
          </td>
        </tr>
      </tbody>
    </table>
1. Clic **[!UICONTROL Continua]** per salvare la connessione e tornare al modulo.

## [!DNL Adobe Journey Optimizer] moduli e relativi campi

Quando si configura [!DNL Adobe Journey Optimizer] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL Adobe Journey Optimizer] I campi potrebbero essere visualizzati in base a fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se viene visualizzato il pulsante Mappa sopra un campo o una funzione, è possibile utilizzarlo per impostare variabili e funzioni per tale campo. Per ulteriori informazioni, consulta [Mappare le informazioni da un modulo all’altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Azioni](#actions)
* [Ricerche](#searches)

### Azioni

* [[!UICONTROL Creare un record]](#create-a-record)
* [[!UICONTROL Effettuare una chiamata API personalizzata]](#make-a-custom-api-call)
* [[!UICONTROL Eliminare un record]](#delete-a-record)
* [[!UICONTROL Aggiornare un record]](#update-a-record)

#### [!UICONTROL Creare un record]

Questo modulo di azione crea un posizionamento, una regola di decisione, un tag, un’offerta personalizzata, una raccolta o un’offerta di fallback.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
     <td>Per istruzioni sulla creazione di una connessione a [!DNL Adobe Journey Optimizer], vedi <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Creare una connessione a [!DNL Adobe Journey Optimizer]</a> in questo articolo.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Tipo di record]
      </td>
      <td>
        Selezionare il tipo di record da creare
        <ul>
        <li><b>[!UICONTROL Posizionamento]</b>: continua con <a href="#placement-fields" >Campi [!UICONTROL Placement]</a>.</li>
        <li><b>[!UICONTROL Regola di decisione]</b>: continua con <a href="#decision-rule-fields" >Campi [!UICONTROL Regola di decisione]</a>.</li>
        <li><b>[!UICONTROL Decision]</b>: continua con <a href="#decision-fields" >Campi [!UICONTROL Decision]</a>.</li>
        <li><b>[!UICONTROL Tag]</b>: continua con <a href="#tag-fields" >Campi [!UICONTROL Tag]</a>.</li>
        <li><b>[!UICONTROL Collection]</b>: continua con <a href="#collection-fields" >Campi di [!UICONTROL Collection]</a>.</li>
        <li><b>[!UICONTROL Offerta di fallback]</b>: continua con <a href="#fallback-offer-fields" >Campi di [!UICONTROL Offerta di fallback]</a>.</li>
        <li><b>[!UICONTROL Offerta personalizzata]</b>: continua con <a href="#personalized-offer-fields" >Campi dell'offerta personalizzata [!UICONTROL]</a>.</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Posizione] campi

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>Immettete o mappate un nome per il posizionamento.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Descrizione]
      </td>
      <td>Immettete o mappate una descrizione per il posizionamento.
      </td>
    </tr>
  </tbody>
</table>


##### [!UICONTROL Regola di decisione] campi

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>Immettere o mappare un nome per la regola di descrizione.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Descrizione]
      </td>
      <td>Immetti o mappa una descrizione per la regola di decisione.
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        Condizione [!UICONTROL]
      </td>
      <td>Inserisci o mappa la condizione per la regola di decisione.
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Decisione] campi

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>Immettere o mappare un nome per la regola di descrizione.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Stato]</td>
      <td>Seleziona lo stato della decisione.
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Data di inizio]</td>
      <td><p>Immetti o mappa la data di inizio della decisione.</p><p>Per un elenco dei formati di data supportati consulta <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Tipo di coercizione in [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Data di fine]</td>
      <td><p>Inserisci o mappa la data di fine della decisione.</p><p>Per un elenco dei formati di data supportati consulta <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Tipo di coercizione in [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Posizionamenti]</td>
      <td>Seleziona i posizionamenti da aggiungere a questa decisione
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Collection]</td>
      <td>Seleziona la raccolta di offerte contenente le offerte che verranno prese in considerazione da questa decisione.
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Offerta di fallback]</td>
      <td>Seleziona l’offerta di fallback che verrà presentata ai clienti che non soddisfano le regole di questa decisione.
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Tag] campi

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>Immetti o mappa un nome per il tag.</td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Raccolta] campi

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>Immetti o mappa un nome per la raccolta.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Filter Type]
      </td>
      <td>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Elements]
      </td>
      <td>Seleziona i tag da includere nella raccolta.
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Offerta di fallback] campi

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>Inserisci o mappa un nome per l’offerta di fallback.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Stato]
      </td>
      <td> Seleziona lo stato dell’offerta di fallback.
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Posizionamento]
      </td>
      <td>Inserisci o mappa il posizionamento per l’offerta di fallback.
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Offerta personalizzata] campi

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>Immettere o mappare un nome per la regola di descrizione.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Stato]</td>
      <td>Seleziona lo stato della decisione.
      </td>
    </tr>
    <tr>
      <td role="rowheader">Posizionamento</td>
      <td>Seleziona il posizionamento per l’offerta personalizzata.
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Data di inizio]</td>
      <td><p>Immetti o mappa la data di inizio dell’offerta personalizzata.</p><p>Per un elenco dei formati di data supportati consulta <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Tipo di coercizione in [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Data di fine]</td>
      <td><p>Inserisci o mappa la data di fine dell’offerta personalizzata.</p><p>Per un elenco dei formati di data supportati consulta <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Tipo di coercizione in [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Regole di decisione]</td>
      <td>Seleziona le regole di decisione da aggiungere a questa offerta personalizzata.
      </td>
    </tr>
   <tr>
      <td role="rowheader">Priorità [!UICONTROL]</td>
      <td>Seleziona la priorità di questa offerta. La priorità influisce sulla presentazione di questa offerta piuttosto che di un’altra.
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Capping constraint]</td>
      <td>Immetti o mappa il numero di volte in cui verrà presentata questa offerta.
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Eliminare un record]

Questo modulo di azione elimina un singolo record in [!DNL Adobe Journey Optimizer].

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
     <td>Per istruzioni sulla creazione di una connessione a [!DNL Adobe Journey Optimizer], vedi <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Creare una connessione a [!DNL Adobe Journey Optimizer]</a> in questo articolo.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Tipo di record]
      </td>
      <td>
        Selezionare il tipo di record da eliminare
        <ul>
        <li>[!UICONTROL Posizionamento]</li>
        <li>[!UICONTROL Regola di decisione]</li>
        <li>[!UICONTROL Decision]</li>
        <li>[!UICONTROL Tag]</li>
        <li>[!UICONTROL Collection]</li>
        <li>[!UICONTROL Offerta di fallback]</li>
        <li>[!UICONTROL Offerta personalizzata]</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Placement]/[!UICONTROL Decision Rule]/[!UICONTROL Decision]/[!UICONTROL Tag]/[!UICONTROL Collection]/[!UICONTROL Fallback offer]/[!UICONTROL Personalized offer]
      </td>
      <td>
        Selezionare il record che si desidera eliminare.
      </td>
    </tr>

</tbody>
</table>

#### [!UICONTROL Effettuare una chiamata API personalizzata]

Questo modulo effettua una chiamata API personalizzata al [!DNL Adobe Journey Optimizer] API

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Connection]</td>
     <td>Per istruzioni sulla creazione di una connessione a [!DNL Adobe Journey Optimizer], vedi <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Creare una connessione a [!DNL Adobe Journey Optimizer]</a> in questo articolo.</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Path]</p>
      </td>
      <td>
        <p>Inserisci un percorso relativo a {baseURL} avvio con<code>/</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Method]</p>
      </td>
      <td>
   <td> <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>Aggiungi le intestazioni della richiesta sotto forma di oggetto JSON standard.</p>
        <p>Ad esempio: <code>{"Content-type":"application/json"}</code></p>
        <p>Workfront Fusion aggiunge automaticamente le intestazioni di autorizzazione e le intestazioni di x-api-key.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Stringa Di Query]  </td>
      <td>
        <p>Immettere la stringa di query richiesta.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>Aggiungi il contenuto body per la chiamata API sotto forma di oggetto JSON standard.</p> <p>Nota:  <p>Quando si utilizzano istruzioni condizionali quali <code>if</code> nel JSON, inserisci le virgolette al di fuori dell’istruzione condizionale.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>Immettere il numero massimo di risultati che il modulo deve restituire in un ciclo di esecuzione.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Eliminare un record]

Questo modulo di azione elimina un singolo record in [!DNL Adobe Journey Optimizer].

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Connection]</td>
     <td>Per istruzioni sulla creazione di una connessione a [!DNL Adobe Journey Optimizer], vedi <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Creare una connessione a [!DNL Adobe Journey Optimizer]</a> in questo articolo.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Tipo di record]
      </td>
      <td>
        Selezionare il tipo di record da eliminare
        <ul>
        <li>[!UICONTROL Posizionamento]</li>
        <li>[!UICONTROL Regola di decisione]</li>
        <li>[!UICONTROL Decision]</li>
        <li>[!UICONTROL Tag]</li>
        <li>[!UICONTROL Collection]</li>
        <li>[!UICONTROL Offerta di fallback]</li>
        <li>[!UICONTROL Offerta personalizzata]</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Placement]/[!UICONTROL Decision Rule]/[!UICONTROL Decision]/[!UICONTROL Tag]/[!UICONTROL Collection]/[!UICONTROL Fallback offer]/[!UICONTROL Personalized offer]
      </td>
      <td>
        Selezionare il record che si desidera eliminare.
      </td>
    </tr>

</tbody>
</table>

#### [!UICONTROL Aggiornare un record]

Questo modulo di azione crea un posizionamento, una decisione, una regola di decisione, un tag, un’offerta personalizzata, una raccolta o un’offerta di fallback.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Connection]</td>
     <td>Per istruzioni sulla creazione di una connessione a [!DNL Adobe Journey Optimizer], vedi <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Creare una connessione a [!DNL Adobe Journey Optimizer]</a> in questo articolo.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Tipo di record]
      </td>
      <td>
        Selezionare il tipo di record da aggiornare
        <ul>
        <li>[!UICONTROL Posizionamento]</li>
        <li>[!UICONTROL Regola di decisione]</li>
        <li>[!UICONTROL Decision]</li>
        <li>[!UICONTROL Tag]</li>
        <li>[!UICONTROL Collection]</li>
        <li>[!UICONTROL Offerta di fallback]</li>
        <li>[!UICONTROL Offerta personalizzata]</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Placement]/[!UICONTROL Decision Rule]/[!UICONTROL Decision]/[!UICONTROL Tag]/[!UICONTROL Collection]/[!UICONTROL Fallback offer]/[!UICONTROL Personalized offer]
      </td>
      <td>
        Selezionare il record da aggiornare.
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Fields]
      </td>
      <td>Per ogni campo da aggiornare:
      <ol>
      <li>Clic <b>[!UICONTROL Add]</b>.</li>
      <li>Specificare se si desidera aggiungere, sostituire o rimuovere valori.</li>
      <li>Immettere il campo da aggiornare.</li>
      <li>Immettere il nuovo valore per il campo.</li>
      </td>
    </tr>

</tbody>
</table>


### Ricerche

#### [!UICONTROL Elencare record]

Questo modulo di ricerca elenca i record del tipo selezionato e restituisce i risultati in base ai criteri specificati.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Connection]</td>
     <td>Per istruzioni sulla creazione di una connessione a [!DNL Adobe Journey Optimizer], vedi <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Creare una connessione a [!DNL Adobe Journey Optimizer]</a> in questo articolo.</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Tipo di record]</p>
      </td>
      <td>
        <p>Selezionare il tipo di record da elencare.</p>
        <ul>
        <li>[!UICONTROL Posizionamento]</li>
        <li>[!UICONTROL Regola di decisione]</li>
        <li>[!UICONTROL Decision]</li>
        <li>[!UICONTROL Tag]</li>
        <li>[!UICONTROL Collection]</li>
        <li>[!UICONTROL Offerta di fallback]</li>
        <li>[!UICONTROL Offerta personalizzata]</li>
       </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Query operator]</p>
      </td>
      <td>
        <p>Seleziona un operatore da applicare ai parametri nella query</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Fields]</td>
      <td><p>Se si desidera limitare la ricerca a campi specifici, immettere i campi. Per ogni campo a cui si desidera limitare la ricerca, fare clic su [!UICONTROL Aggiungi elemento] e immettere il nome del campo.</p><p>Le espressioni di percorso sono sotto forma di percorsi separati da punti come <code>_instance.xdm:name</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Ordina per] </td>
      <td>Immettere o mappare la proprietà in base alla quale si desidera ordinare i risultati.
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Direzione ordine]</td>
   <td>Seleziona se desideri ordinare i risultati in ordine crescente o decrescente.
    </td>
     </tr>
  </tbody>
</table>
