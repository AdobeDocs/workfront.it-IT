---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli Split.io
description: In un [!DNL Adobe Workfront Fusion] scenario, puoi automatizzare i flussi di lavoro che utilizzano [!DNL Split.io], oltre a collegarlo a più applicazioni e servizi di terze parti.
author: Becky
feature: Workfront Fusion
exl-id: 4576a2e4-b495-430e-a9de-4e1ec7379ab8
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1821'
ht-degree: 0%

---

# [!DNL Split.io] moduli

In un [!DNL Adobe Workfront Fusion] scenario, puoi automatizzare i flussi di lavoro che utilizzano [!DNL Split.io], oltre a collegarlo a più applicazioni e servizi di terze parti.

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

Da utilizzare [!DNL Split.io] moduli, è necessario disporre di un [!DNL Split.io] account.

## Connetti [!DNL Split.io] a [!DNL Workfront Fusion] {#connect-split-io-to-workfront-fusion}

Puoi creare una connessione al tuo [!DNL Split.io] account direttamente dall&#39;interno di un [!DNL Split.io] modulo.

1. In qualsiasi [!DNL Split.io] modulo, fai clic su **[!UICONTROL Aggiungi]** accanto al [!UICONTROL Connessione] campo.
1. Immettere un nome per la connessione.
1. Immetti il [!DNL Split.io] Chiave API.

   Per ulteriori informazioni su [!DNL Split.io] Chiavi API, vedi [Chiavi API](https://help.split.io/hc/en-us/articles/360019916211-API-keys) nel [!DNL Split.io] documentazione.

1. Clic **[!UICONTROL Continua]** per creare la connessione e tornare al modulo.

## [!DNL Split.io] moduli e relativi campi

Quando si configura [!DNL split.io] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL split.io] I campi potrebbero essere visualizzati in base a fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se viene visualizzato il pulsante Mappa sopra un campo o una funzione, è possibile utilizzarlo per impostare variabili e funzioni per tale campo. Per ulteriori informazioni, consulta [Mappare le informazioni da un modulo all’altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Azioni](#actions)
* [Ricerche](#searches)

### Azioni

* [[!UICONTROL Chiamata API personalizzata]](#custom-api-call)
* [[!UICONTROL Dividi]](#get-split)
* [[!UICONTROL Ottieni definizione di suddivisione nell’ambiente]](#get-split-definition-in-environment)
* [[!UICONTROL Crea suddivisione]](#create-split)
* [[!UICONTROL Elimina suddivisione]](#delete-split)
* [[!UICONTROL Creare una definizione di suddivisione nell’ambiente]](#create-split-definition-in-environment)
* [[!UICONTROL Rimuovi definizione di suddivisione dall’ambiente]](#remove-split-definition-from-environment)
* [[!UICONTROL Definizione suddivisione aggiornamento parziale nell’ambiente]](#partial-update-split-definition-in-environment)
* [[!UICONTROL Associa tag]](#associate-tags)

#### [!UICONTROL Chiamata API personalizzata]

Questo modulo di azione consente di effettuare una chiamata autenticata personalizzata al [!DNL split.io] API. In questo modo, puoi creare un’automazione del flusso di dati che non può essere eseguita dall’altro [!DNL split.io] moduli.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Split.io] account a [!DNL Workfront Fusion], vedi <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Split.io] a [!UICONTROL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Inserisci un percorso relativo a <code>https://api.split.io/internal/api/v2/</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Aggiungi le intestazioni della richiesta sotto forma di oggetto JSON standard.</p> <p>Ad esempio: <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion aggiunge automaticamente le intestazioni di autorizzazione.</p> </td> 
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
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Immettere o mappare il numero massimo di record con cui si desidera lavorare il modulo durante ogni ciclo di esecuzione dello scenario.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Dividi]

Questo modulo di azione recupera la suddivisione.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Split.io] account a [!DNL Workfront Fusion], vedi <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Split.io] a [!UICONTROL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID area di lavoro]</td> 
   <td>Selezionate o mappate l'area di lavoro contenente la divisione da recuperare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>Immettere o mappare il nome della divisione che si desidera recuperare.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottieni definizione di suddivisione nell’ambiente]

Questo modulo di azione recupera una definizione di suddivisione specifica dall’ambiente designato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Split.io] account a [!DNL Workfront Fusion], vedi <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Split.io] a [!UICONTROL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID area di lavoro]</td> 
   <td>Selezionate o mappate l'area di lavoro contenente la definizione di suddivisione da recuperare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome o ID ambiente]</td> 
   <td>Seleziona o mappa l’ambiente che contiene la definizione di suddivisione da recuperare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>Immettere o mappare il nome della divisione per la quale si desidera recuperare la definizione di divisione.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crea suddivisione]

Questo modulo di azione crea una nuova suddivisione nell’organizzazione, in base a un tipo di traffico.

>[!NOTE]
>
>L’API non configura la suddivisione in alcun ambiente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Split.io] account a [!DNL Workfront Fusion], vedi <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Split.io] a [!UICONTROL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID area di lavoro]</td> 
   <td>Selezionate o mappate l'area di lavoro in cui desiderate creare la suddivisione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome o ID tipo di traffico]</td> 
   <td>Seleziona o mappa il tipo di traffico da utilizzare per creare la suddivisione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>Immettere o mappare un nome per la divisione da creare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Descrizione suddivisione]</td> 
   <td>Immettere o mappare una descrizione [!UICONTROL split] per la suddivisione che si desidera creare.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Elimina suddivisione]

Questo modulo di azione elimina una suddivisione dall’organizzazione. Questa operazione annulla automaticamente la configurazione della definizione divisa da tutti gli ambienti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Split.io] account a [!DNL Workfront Fusion], vedi <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Split.io] a [!UICONTROL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID area di lavoro]</td> 
   <td>Selezionate o mappate l'area di lavoro in cui desiderate eliminare la divisione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>Immettere o mappare il nome della divisione che si desidera eliminare.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Creare una definizione di suddivisione nell’ambiente]

Questo modulo di azione configura una definizione divisa per un ambiente specifico.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Split.io] account a [!DNL Workfront Fusion], vedi <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Split.io] a [!UICONTROL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID area di lavoro]</td> 
   <td>Seleziona o mappa l’area di lavoro in cui desideri creare una definizione di suddivisione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome o ID ambiente]</td> 
   <td>Seleziona o mappa l’ambiente in cui desideri creare una definizione di suddivisione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>Immettere o mappare il nome della divisione per la quale si desidera creare una definizione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Commenti]</td> 
   <td>Immettere o mappare i commenti che si desidera aggiungere alla definizione di suddivisione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Rules]</td> 
   <td> <p>Per ogni regola di targeting che desideri aggiungere alla definizione, fai clic su <b>[!UICONTROL Add item]</b>, quindi inserisci o mappa la regola.</p> <p>Per ulteriori informazioni sulle regole di targeting, consulta <a href="https://docs.split.io/reference#create-split-definition-in-environment">Creare una definizione di suddivisione in un ambiente</a> nel [!DNL Split.io] documentazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Regola predefinita]</td> 
   <td> <p>Immetti o mappa la regola da utilizzare per il traffico che non soddisfa le specifiche delle altre regole.</p> <p>Per ulteriori informazioni sulle regole di targeting, consulta <a href="https://docs.split.io/reference#create-split-definition-in-environment">Creare una definizione di suddivisione in un ambiente</a> nel [!DNL Split.io] documentazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Default treatment]</td> 
   <td> <p>Immettere o mappare il trattamento che si desidera utilizzare per la suddivisione se questa viene terminata o se il cliente non è incluso nell'allocazione del traffico.</p> <p>Per ulteriori informazioni sui trattamenti, consulta <a href="https://docs.split.io/reference#create-split-definition-in-environment">Creare una definizione di suddivisione in un ambiente</a> nel [!DNL Split.io] documentazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Treatments]</td> 
   <td> <p>Per ogni trattamento che desideri aggiungere alla definizione, fai clic su <b>[!UICONTROL Add item]</b>, quindi inserisci o mappa il trattamento.</p> <p>Per ulteriori informazioni sui trattamenti, consulta <a href="https://docs.split.io/reference#create-split-definition-in-environment">Creare una definizione di suddivisione in un ambiente</a> nel [!DNL Split.io] documentazione.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Rimuovi definizione di suddivisione dall’ambiente]

Questo modulo di azione annulla la configurazione di una definizione divisa per un ambiente specifico.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Split.io] account a [!DNL Workfront Fusion], vedi <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Split.io] a [!UICONTROL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID area di lavoro]</td> 
   <td>Selezionare o mappare l'area di lavoro in cui si desidera rimuovere una definizione di suddivisione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome o ID ambiente]</td> 
   <td>Seleziona o mappa l’ambiente in cui desideri rimuovere una definizione di suddivisione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>Immettere o mappare il nome della divisione per la quale si desidera rimuovere una definizione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Commenti]</td> 
   <td>Immettere o mappare i commenti che si desidera aggiungere alla definizione di suddivisione.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Definizione suddivisione aggiornamento parziale nell’ambiente]

Questo modulo di azione aggiorna una definizione divisa per un ambiente specifico.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Split.io] account a [!DNL Workfront Fusion], vedi <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Split.io] a [!UICONTROL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID area di lavoro]</td> 
   <td>Seleziona o mappa l’area di lavoro in cui desideri aggiornare una definizione di suddivisione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome o ID ambiente]</td> 
   <td>Seleziona o mappa l’ambiente in cui desideri aggiornare una definizione di suddivisione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>Immettere o mappare il nome della suddivisione per la quale si desidera aggiornare la definizione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Aggiorna contenuto]</td> 
   <td> <p>Per ogni attributo della suddivisione che desideri aggiornare, fai clic su <b>[!UICONTROL Add item]</b> e inserisci o mappa le modifiche desiderate.</p> <p>Per ulteriori informazioni, consulta <a href="https://docs.split.io/reference#partial-update-split-definition-in-environment">Definizione suddivisione aggiornamento parziale nell’ambiente</a> nel [!DNL Split.io] documentazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Commenti]</td> 
   <td>Immettere o mappare i commenti che si desidera aggiungere alla definizione di suddivisione.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Associa tag]

Questo modulo di azione aggiunge tag all’oggetto specificato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Split.io] account a [!DNL Workfront Fusion], vedi <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Split.io] a [!UICONTROL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID area di lavoro]</td> 
   <td>Seleziona o mappa l’area di lavoro in cui desideri aggiungere un tag.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome Oggetto]</td> 
   <td>Immettere o mappare il nome dell'oggetto a cui si desidera aggiungere i tag,</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Tipo di oggetto [!UICONTROL]</td> 
   <td> <p>Immettere o mappare il tipo di oggetto a cui si desidera aggiungere i tag.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tags]</td> 
   <td> <p>Per ogni tag che desideri aggiungere, fai clic su <b>[!UICONTROL Add item]</b> e inserisci o mappa il tag.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Ricerche

* [[!UICONTROL Ottieni aree di lavoro]](#get-workspaces)
* [[!UICONTROL Ottieni ambienti]](#get-environments)
* [[!UICONTROL Ottieni divisioni]](#get-splits)
* [[!UICONTROL Elencare le definizioni di suddivisione in un ambiente]](#list-split-definitions-in-an-environment)
* [[!UICONTROL Ottieni tipi di traffico]](#get-traffic-types)

#### [!UICONTROL Ottieni aree di lavoro]

Questo modulo di ricerca recupera le aree di lavoro di un’organizzazione.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Split.io] account a [!DNL Workfront Fusion], vedi <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Split.io] a [!UICONTROL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Immettere o mappare il numero massimo di aree di lavoro che il modulo deve recuperare durante ogni ciclo di esecuzione dello scenario.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottieni ambienti]

Questo modulo di ricerca recupera un elenco di ambienti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Split.io] account a [!DNL Workfront Fusion], vedi <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Split.io] a [!UICONTROL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID area di lavoro]</td> 
   <td>Seleziona o mappa l’area di lavoro contenente gli ambienti che desideri elencare.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottieni divisioni]

Questo modulo di ricerca recupera un elenco di divisioni.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Split.io] account a [!DNL Workfront Fusion], vedi <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Split.io] a [!UICONTROL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID area di lavoro]</td> 
   <td>Selezionate o mappate l'area di lavoro contenente le divisioni da elencare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Immettere o mappare il numero massimo di divisioni che il modulo deve recuperare durante ogni ciclo di esecuzione dello scenario.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Elencare le definizioni di suddivisione in un ambiente]

Questo modulo di ricerca recupera un elenco di definizioni di suddivisioni in un determinato ambiente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Split.io] account a [!DNL Workfront Fusion], vedi <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Split.io] a [!UICONTROL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID area di lavoro]</td> 
   <td>Selezionate o mappate l'area di lavoro contenente le definizioni di suddivisione da elencare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome o ID ambiente]</td> 
   <td>Seleziona o mappa l’ambiente che contiene le definizioni di suddivisione da elencare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Immetti o mappa il numero massimo di definizioni di suddivisione che il modulo deve recuperare durante ciascun ciclo di esecuzione dello scenario.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottieni tipi di traffico]

Questo modulo di ricerca recupera un elenco di tipi di traffico.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Split.io] account a [!DNL Workfront Fusion], vedi <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Split.io] a [!UICONTROL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID area di lavoro]</td> 
   <td>Seleziona o mappa l’area di lavoro contenente i tipi di traffico che desideri elencare.</td> 
  </tr> 
 </tbody> 
</table>
