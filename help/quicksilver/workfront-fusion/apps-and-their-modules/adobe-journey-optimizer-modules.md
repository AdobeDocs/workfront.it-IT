---
filename: adobe-journey-optimizer-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Moduli Adobe Journey Optimizer
description: In un [!DNL Adobe Workfront Fusion] puoi automatizzare i flussi di lavoro che utilizzano [!DNL Adobe Journey Optimizer], nonché collegarlo a più applicazioni e servizi di terze parti.
author: Becky
exl-id: 2c1aea46-edbf-42a3-a6e9-f8aea042a48d
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1554'
ht-degree: 0%

---

# [!DNL Adobe Journey Optimizer] Moduli

<!--
Becky: pull from main, add to TOCs, then push to merge.
-->

In un [!DNL Adobe Workfront Fusion] puoi automatizzare i flussi di lavoro che utilizzano [!DNL Adobe Journey Optimizer], nonché collegarlo a più applicazioni e servizi di terze parti. [!DNL Adobe Journey Optimizer] I moduli ti consentono di creare, leggere, aggiornare o eliminare record o di eseguire una chiamata API personalizzata per [!DNL Adobe Journey Optimizer] API.


Se hai bisogno di istruzioni su come creare uno scenario, vedi [Creare uno scenario](../../workfront-fusion/scenarios/create-a-scenario.md).

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

Prima di poter utilizzare il [!DNL Adobe Journey Optimizer] connettore, è necessario assicurarsi che siano soddisfatti i seguenti prerequisiti:

* Devi avere un attivo [!DNL Adobe Journey Optimizer] conto.

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
          <td role="rowheader">ID client [!UICONTROL]</td>
          <td>Inserisci il tuo [!DNL Adobe] [!UICONTROL Client ID]. Questo è possibile trovare nella sezione [!UICONTROL Credentials details] del [!DNL Adobe Developer Console].</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Segreto client]</td>
          <td>Inserisci il tuo [!DNL Adobe] [!UICONTROL Segreto client]. Questo è possibile trovare nella sezione [!UICONTROL Credentials details] del [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL ID account tecnico]</td>
          <td>Inserisci il tuo [!DNL Adobe] [!UICONTROL Technical account ID]. Questo è possibile trovare nella sezione [!UICONTROL Credentials details] del [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Organization ID]</td>
          <td>Inserisci il tuo [!DNL Adobe] [!UICONTROL Organization ID]. Questo è possibile trovare nella sezione [!UICONTROL Credentials details] del [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Meta ambito]</td>
          <td>
            Immettere i metadati necessari per la connessione.
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Chiave privata]</td>
          <td>
            <p>Immetti la chiave privata generata al momento della creazione delle credenziali nel [!DNL Adobe Developer Console]. </p>
            <p>Per estrarre la chiave privata o il certificato:</p>
            <ol>
              <li value="1">
                <p>Fai clic su <b>[!UICONTROL Extract]</b>.</p>
              </li>
              <li value="2">
                <p>Selezionare il tipo di file da estrarre.</p>
              </li>
              <li value="3">
                <p>Selezionare il file contenente la chiave privata o il certificato.</p>
              </li>
              <li value="4">
                <p>Immetti la password del file.</p>
              </li>
              <li value="5">
                <p>Fai clic su <b>[!UICONTROL Save]</b> per estrarre il file e tornare alla configurazione della connessione.</p>
              </li>
            </ol>
          </td>
        </tr>
      </tbody>
    </table>
1. Fai clic su **[!UICONTROL Continua]** per salvare la connessione e tornare al modulo .

## [!DNL Adobe Journey Optimizer] moduli e relativi campi

Quando si configura [!DNL Adobe Journey Optimizer] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL Adobe Journey Optimizer] potrebbero essere visualizzati, a seconda di fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se trovi il pulsante mappa sopra un campo o una funzione, puoi utilizzarlo per impostare variabili e funzioni per quel campo. Per ulteriori informazioni, consulta [Mappare informazioni da un modulo a un altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Azioni](#actions)
* [Ricerche](#searches)

### Azioni

* [[!UICONTROL Creare un record]](#create-a-record)
* [[!UICONTROL Effettuare una chiamata API personalizzata]](#make-a-custom-api-call)
* [[!UICONTROL Eliminare un record]](#delete-a-record)
* [[!UICONTROL Aggiornare un record]](#update-a-record)

#### [!UICONTROL Creare un record]

Questo modulo di azione crea un posizionamento, una regola decisionale, un tag, un’offerta personalizzata, una raccolta o un’offerta di fallback.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
     <td>Per istruzioni su come creare una connessione a [!DNL Adobe Journey Optimizer], vedi <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Creare una connessione a [!DNL Adobe Journey Optimizer]</a> in questo articolo.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Tipo di record]
      </td>
      <td>
        Selezionare il tipo di record da creare
        <ul>
        <li><b>[!UICONTROL Placement]</b>: Continua a <a href="#placement-fields" >Campi [!UICONTROL Placement]</a>.</li>
        <li><b>[!UICONTROL Regola decisionale]</b>: Continua a <a href="#decision-rule-fields" >Campi della regola decisionale</a>.</li>
        <li><b>[!UICONTROL Decision]</b>: Continua a <a href="#decision-fields" >Campi [!UICONTROL Decision]</a>.</li>
        <li><b>Tag [!UICONTROL]</b>: Continua a <a href="#tag-fields" >Campi di tag</a>.</li>
        <li><b>Raccolta [!UICONTROL]</b>: Continua a <a href="#collection-fields" >Campi della raccolta</a>.</li>
        <li><b>[!UICONTROL Offerta di fallback]</b>: Continua a <a href="#fallback-offer-fields" >Campi dell’ [!UICONTROL Fallback offer]</a>.</li>
        <li><b>[!UICONTROL Offerta personalizzata]</b>: Continua a <a href="#personalized-offer-fields" >Campi di [!UICONTROL Personalizza offerta]</a>.</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Posizionamento] field

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>Immetti o mappa un nome per il posizionamento.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Descrizione]
      </td>
      <td>Immetti o mappa una descrizione del posizionamento.
      </td>
    </tr>
  </tbody>
</table>


##### [!UICONTROL Regola decisionale] field

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>Immetti o mappa un nome per la regola di descrizione.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Descrizione]
      </td>
      <td>Immetti o mappa una descrizione per la regola decisionale.
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Condition]
      </td>
      <td>Immettere o mappare la condizione della regola decisionale.
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Decisione] field

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>Immetti o mappa un nome per la regola di descrizione.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Status]</td>
      <td>Seleziona lo stato della decisione.
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Data di inizio]</td>
      <td><p>Immettere o mappare la data di inizio della decisione.</p><p>Per un elenco dei formati di data supportati, consulta <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Tipo di coercizione in [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Data di fine]</td>
      <td><p>Immettere o mappare la data di fine della decisione.</p><p>Per un elenco dei formati di data supportati, consulta <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Tipo di coercizione in [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Placements]</td>
      <td>Seleziona i posizionamenti da aggiungere a questa decisione
      </td>
    </tr>
   <tr>
      <td role="rowheader">Raccolta [!UICONTROL]</td>
      <td>Seleziona la raccolta di offerte che contiene le offerte che verranno prese in considerazione in questa decisione.
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Offerta di fallback]</td>
      <td>Seleziona l’offerta di fallback che verrà presentata ai clienti che non soddisfano le regole per questa decisione.
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Tag] field

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>Immetti o mappa un nome per il tag .</td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Raccolta] field

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>Immettere o mappare un nome per la raccolta.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Tipo filtro]
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

##### [!UICONTROL Offerta di fallback] field

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>Immetti o mappa un nome per l’offerta di fallback.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Status]
      </td>
      <td> Seleziona lo stato dell’offerta di fallback.
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Placement]
      </td>
      <td>Immetti o mappa il posizionamento per l’offerta di fallback.
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Offerta personalizzata] field

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>Immetti o mappa un nome per la regola di descrizione.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Status]</td>
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
      <td><p>Immetti o mappa la data di inizio dell’offerta personalizzata.</p><p>Per un elenco dei formati di data supportati, consulta <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Tipo di coercizione in [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Data di fine]</td>
      <td><p>Immetti o mappa la data di fine dell’offerta personalizzata.</p><p>Per un elenco dei formati di data supportati, consulta <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Tipo di coercizione in [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Regole decisionali]</td>
      <td>Seleziona le regole di decisione da aggiungere a questa offerta personalizzata.
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Priority]</td>
      <td>Seleziona la priorità dell’offerta. La priorità influisce sul fatto che questa offerta verrà presentata anziché su un’altra.
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Limite di limitazione di limitazione di limitazione]</td>
      <td>Immetti o mappa il numero di volte in cui verrà presentata l’offerta.
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Eliminare un record]

Questo modulo di azione elimina un record singolo in [!DNL Adobe Journey Optimizer].

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
     <td>Per istruzioni su come creare una connessione a [!DNL Adobe Journey Optimizer], vedi <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Creare una connessione a [!DNL Adobe Journey Optimizer]</a> in questo articolo.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Tipo di record]
      </td>
      <td>
        Selezionare il tipo di record da eliminare
        <ul>
        <li>[!UICONTROL Placement]</li>
        <li>[!UICONTROL Regola decisionale]</li>
        <li>[!UICONTROL Decision]</li>
        <li>Tag [!UICONTROL]</li>
        <li>Raccolta [!UICONTROL]</li>
        <li>[!UICONTROL Offerta di fallback]</li>
        <li>[!UICONTROL Offerta personalizzata]</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Placement]/[!UICONTROL Decision rule]/[!UICONTROL Decision]/[!UICONTROL Tag]/[!UICONTROL Collection]/[!UICONTROL Fallback offer]/[!UICONTROL Offerta personalizzata]
      </td>
      <td>
        Selezionare il record da eliminare.
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
     <td>Per istruzioni su come creare una connessione a [!DNL Adobe Journey Optimizer], vedi <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Creare una connessione a [!DNL Adobe Journey Optimizer]</a> in questo articolo.</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Path]</p>
      </td>
      <td>
        <p>Immetti un percorso relativo a {baseURL} che inizia con<code>/</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL, Metodo]</p>
      </td>
      <td>
   <td> <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>Aggiungi le intestazioni della richiesta sotto forma di un oggetto JSON standard.</p>
        <p>Ad esempio: <code>{"Content-type":"application/json"}</code></p>
        <p>Workfront Fusion aggiunge automaticamente intestazioni di autorizzazione e intestazioni x-api-key.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Query String]  </td>
      <td>
        <p>Immetti la stringa di query della richiesta.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>Aggiungi il contenuto del corpo per la chiamata API sotto forma di un oggetto JSON standard.</p> <p>Nota:  <p>Quando si utilizzano istruzioni condizionali come <code>if</code> nel JSON, inserisci le virgolette al di fuori dell’istruzione condizionale.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>Immettere il numero massimo di risultati che si desidera che il modulo restituisca in un ciclo di esecuzione.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Eliminare un record]

Questo modulo di azione elimina un record singolo in [!DNL Adobe Journey Optimizer].

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Connection]</td>
     <td>Per istruzioni su come creare una connessione a [!DNL Adobe Journey Optimizer], vedi <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Creare una connessione a [!DNL Adobe Journey Optimizer]</a> in questo articolo.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Tipo di record]
      </td>
      <td>
        Selezionare il tipo di record da eliminare
        <ul>
        <li>[!UICONTROL Placement]</li>
        <li>[!UICONTROL Regola decisionale]</li>
        <li>[!UICONTROL Decision]</li>
        <li>Tag [!UICONTROL]</li>
        <li>Raccolta [!UICONTROL]</li>
        <li>[!UICONTROL Offerta di fallback]</li>
        <li>[!UICONTROL Offerta personalizzata]</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Placement]/[!UICONTROL Decision rule]/[!UICONTROL Decision]/[!UICONTROL Tag]/[!UICONTROL Collection]/[!UICONTROL Fallback offer]/[!UICONTROL Offerta personalizzata]
      </td>
      <td>
        Selezionare il record da eliminare.
      </td>
    </tr>

</tbody>
</table>

#### [!UICONTROL Aggiornare un record]

Questo modulo di azione crea un posizionamento, una decisione, una regola decisionale, un tag, un’offerta personalizzata, una raccolta o un’offerta di fallback.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Connection]</td>
     <td>Per istruzioni su come creare una connessione a [!DNL Adobe Journey Optimizer], vedi <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Creare una connessione a [!DNL Adobe Journey Optimizer]</a> in questo articolo.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Tipo di record]
      </td>
      <td>
        Selezionare il tipo di record da aggiornare
        <ul>
        <li>[!UICONTROL Placement]</li>
        <li>[!UICONTROL Regola decisionale]</li>
        <li>[!UICONTROL Decision]</li>
        <li>Tag [!UICONTROL]</li>
        <li>Raccolta [!UICONTROL]</li>
        <li>[!UICONTROL Offerta di fallback]</li>
        <li>[!UICONTROL Offerta personalizzata]</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Placement]/[!UICONTROL Decision rule]/[!UICONTROL Decision]/[!UICONTROL Tag]/[!UICONTROL Collection]/[!UICONTROL Fallback offer]/[!UICONTROL Offerta personalizzata]
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
      <li>Fai clic su <b>[!UICONTROL Aggiungi]</b>.</li>
      <li>Seleziona se desideri aggiungere, sostituire o rimuovere valori.</li>
      <li>Immetti il campo da aggiornare.</li>
      <li>Immettere il nuovo valore per il campo.</li>
      </td>
    </tr>

</tbody>
</table>


### Ricerche

#### [!UICONTROL Elencare record]

Questo modulo di ricerca elenca i record del tipo selezionato, che restituiscono i risultati in base ai criteri specificati.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Connection]</td>
     <td>Per istruzioni su come creare una connessione a [!DNL Adobe Journey Optimizer], vedi <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Creare una connessione a [!DNL Adobe Journey Optimizer]</a> in questo articolo.</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Tipo di record]</p>
      </td>
      <td>
        <p>Selezionare il tipo di record da elencare.</p>
        <ul>
        <li>[!UICONTROL Placement]</li>
        <li>[!UICONTROL Regola decisionale]</li>
        <li>[!UICONTROL Decision]</li>
        <li>Tag [!UICONTROL]</li>
        <li>Raccolta [!UICONTROL]</li>
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
        <p>Selezionare un operatore da applicare ai parametri nella query</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Fields]</td>
      <td><p>Se si desidera limitare la ricerca a campi specifici, immettere i campi. Per ogni campo a cui si desidera limitare la ricerca, fare clic su [!UICONTROL Aggiungi elemento] e immettere il nome del campo.</p><p>Le espressioni percorso si presentano sotto forma di percorsi separati da punti, come <code>_instance.xdm:name</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Ordina per] </td>
      <td>Immettere o mappare la proprietà in base alla quale si desidera ordinare i risultati.
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Direzione ordine]</td>
   <td>Seleziona se vuoi ordinare i risultati in direzione ascendente o decrescente.
    </td>
     </tr>
  </tbody>
</table>
