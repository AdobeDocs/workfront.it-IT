---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli Split.io
description: In un [!DNL Adobe Workfront Fusion] puoi automatizzare i flussi di lavoro che utilizzano [!DNL Split.io], nonché collegarlo a più applicazioni e servizi di terze parti.
author: Becky
feature: Workfront Fusion
exl-id: 4576a2e4-b495-430e-a9de-4e1ec7379ab8
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1773'
ht-degree: 0%

---

# [!DNL Split.io] moduli

In un [!DNL Adobe Workfront Fusion] puoi automatizzare i flussi di lavoro che utilizzano [!DNL Split.io], nonché collegarlo a più applicazioni e servizi di terze parti.

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

Per utilizzare [!DNL Split.io] moduli, è necessario disporre di un [!DNL Split.io] conto.

## Connetti [!DNL Split.io] a [!DNL Workfront Fusion] {#connect-split-io-to-workfront-fusion}

Puoi creare una connessione al tuo [!DNL Split.io] account direttamente dall&#39;interno di un [!DNL Split.io] modulo .

1. In qualsiasi [!DNL Split.io] modulo, fai clic su **[!UICONTROL Aggiungi]** accanto al [!UICONTROL Connessione] campo .
1. Immettere un nome per la connessione.
1. Inserisci il tuo [!DNL Split.io] Chiave API.

   Per ulteriori informazioni su [!DNL Split.io] Chiavi API, vedi [Chiavi API](https://help.split.io/hc/en-us/articles/360019916211-API-keys) in [!DNL Split.io] documentazione.

1. Fai clic su **[!UICONTROL Continua]** per creare la connessione e tornare al modulo .

## [!DNL Split.io] moduli e relativi campi

Quando si configura [!DNL split.io] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL split.io] potrebbero essere visualizzati, a seconda di fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se trovi il pulsante mappa sopra un campo o una funzione, puoi utilizzarlo per impostare variabili e funzioni per quel campo. Per ulteriori informazioni, consulta [Mappare informazioni da un modulo a un altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Azioni](#actions)
* [Ricerche](#searches)

### Azioni

* [[!UICONTROL Chiamata API personalizzata]](#custom-api-call)
* [[!UICONTROL Dividi]](#get-split)
* [[!UICONTROL Ottieni definizione divisa in ambiente]](#get-split-definition-in-environment)
* [[!UICONTROL Crea divisione]](#create-split)
* [[!UICONTROL Elimina suddivisione]](#delete-split)
* [[!UICONTROL Creare una definizione divisa in ambiente]](#create-split-definition-in-environment)
* [[!UICONTROL Rimuovi definizione divisa dall&#39;ambiente]](#remove-split-definition-from-environment)
* [[!UICONTROL Definizione di suddivisione dell&#39;aggiornamento parziale in ambiente]](#partial-update-split-definition-in-environment)
* [[!UICONTROL Associa tag]](#associate-tags)

#### [!UICONTROL Chiamata API personalizzata]

Questo modulo di azione ti consente di effettuare una chiamata autenticata personalizzata al [!DNL split.io] API. In questo modo, puoi creare un’automazione del flusso di dati che non può essere eseguita dall’altro [!DNL split.io] moduli.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Split.io] account a [!DNL Workfront Fusion], vedi <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Split.io] a [!UICONTROL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Immettere un percorso relativo a <code>https://api.split.io/internal/api/v2/</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL, Metodo]</td> 
   <td> <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Aggiungi le intestazioni della richiesta sotto forma di un oggetto JSON standard.</p> <p>Ad esempio: <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion aggiunge le intestazioni di autorizzazione.</p> </td> 
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
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Immettere o mappare il numero massimo di record con cui si desidera che il modulo funzioni durante ogni ciclo di esecuzione degli scenari.</td> 
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
   <td> <p>Per istruzioni su come collegare le [!DNL Split.io] account a [!DNL Workfront Fusion], vedi <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Split.io] a [!UICONTROL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Selezionare o mappare l'area di lavoro che contiene la suddivisione da recuperare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>Immettere o mappare il nome della divisione che si desidera recuperare.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottieni definizione divisa in ambiente]

Questo modulo di azione recupera una definizione di suddivisione specifica dall&#39;ambiente designato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Split.io] account a [!DNL Workfront Fusion], vedi <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Split.io] a [!UICONTROL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Seleziona o mappa l'area di lavoro che contiene la definizione di suddivisione da recuperare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome ambiente o ID]</td> 
   <td>Seleziona o mappa l’ambiente che contiene la definizione di suddivisione da recuperare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>Immettere o mappare il nome della suddivisione per la quale si desidera recuperare la definizione della suddivisione.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crea divisione]

Questo modulo di azione crea una nuova suddivisione nell&#39;organizzazione, in base a un tipo di traffico.

>[!NOTE]
>
>L’API non configura la suddivisione in alcun ambiente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Split.io] account a [!DNL Workfront Fusion], vedi <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Split.io] a [!UICONTROL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Seleziona o mappa l’area di lavoro in cui desideri creare la suddivisione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID o nome del tipo di traffico]</td> 
   <td>Seleziona o mappa il tipo di traffico che desideri utilizzare per creare la suddivisione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>Inserisci o mappa un nome per la suddivisione da creare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Description]</td> 
   <td>Immetti o mappa una descrizione [!UICONTROL split] per la suddivisione da creare.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Elimina suddivisione]

Questo modulo di azione elimina una suddivisione dall&#39;organizzazione. In questo modo la definizione di suddivisione viene automaticamente deconfigurata da tutti gli ambienti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Split.io] account a [!DNL Workfront Fusion], vedi <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Split.io] a [!UICONTROL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Seleziona o mappa l’area di lavoro in cui desideri eliminare la suddivisione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>Immettere o mappare il nome della divisione da eliminare.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Creare una definizione divisa in ambiente]

Questo modulo di azione configura una definizione di suddivisione per un ambiente specifico.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Split.io] account a [!DNL Workfront Fusion], vedi <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Split.io] a [!UICONTROL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Selezionare o mappare l'area di lavoro in cui si desidera creare una definizione di suddivisione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome ambiente o ID]</td> 
   <td>Seleziona o mappa l’ambiente in cui desideri creare una definizione di suddivisione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>Immettere o mappare il nome della suddivisione per la quale si desidera creare una definizione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Commenti]</td> 
   <td>Inserisci o mappa i commenti da aggiungere alla definizione di suddivisione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Rules]</td> 
   <td> <p>Per ogni regola di targeting che desideri aggiungere alla definizione, fai clic su <b>[!UICONTROL Aggiungi elemento]</b>, quindi immetti o mappa la regola.</p> <p>Per ulteriori informazioni sulle regole di targeting, vedi <a href="https://docs.split.io/reference#create-split-definition-in-environment">Creare una definizione divisa in un ambiente</a> in [!DNL Split.io] documentazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Regola predefinita]</td> 
   <td> <p>Immetti o mappa la regola che desideri che la suddivisione utilizzi per il traffico che non soddisfa le specifiche per le altre regole.</p> <p>Per ulteriori informazioni sulle regole di targeting, vedi <a href="https://docs.split.io/reference#create-split-definition-in-environment">Creare una definizione divisa in un ambiente</a> in [!DNL Split.io] documentazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Trattamento predefinito]</td> 
   <td> <p>Inserire o mappare il trattamento che si desidera utilizzare per la suddivisione se la suddivisione viene interrotta o se il cliente non è incluso nell'allocazione del traffico.</p> <p>Per ulteriori informazioni sui trattamenti, vedi <a href="https://docs.split.io/reference#create-split-definition-in-environment">Creare una definizione divisa in un ambiente</a> in [!DNL Split.io] documentazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Trattamenti]</td> 
   <td> <p>Per ogni trattamento che si desidera aggiungere alla definizione, fare clic su <b>[!UICONTROL Aggiungi elemento]</b>, quindi inserire o mappare il trattamento.</p> <p>Per ulteriori informazioni sui trattamenti, vedi <a href="https://docs.split.io/reference#create-split-definition-in-environment">Creare una definizione divisa in un ambiente</a> in [!DNL Split.io] documentazione.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Rimuovi definizione divisa dall&#39;ambiente]

Questo modulo di azione consente di annullare la configurazione di una definizione di suddivisione per un ambiente specifico.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Split.io] account a [!DNL Workfront Fusion], vedi <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Split.io] a [!UICONTROL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Selezionare o mappare l'area di lavoro in cui si desidera rimuovere una definizione di suddivisione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome ambiente o ID]</td> 
   <td>Seleziona o mappa l’ambiente in cui desideri rimuovere una definizione di suddivisione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>Immettere o mappare il nome della divisione per la quale si desidera rimuovere una definizione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Commenti]</td> 
   <td>Inserisci o mappa i commenti da aggiungere alla definizione di suddivisione.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Definizione di suddivisione dell&#39;aggiornamento parziale in ambiente]

Questo modulo di azione aggiorna una definizione di suddivisione per un ambiente specifico.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Split.io] account a [!DNL Workfront Fusion], vedi <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Split.io] a [!UICONTROL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Selezionare o mappare l'area di lavoro in cui si desidera aggiornare una definizione di suddivisione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome ambiente o ID]</td> 
   <td>Seleziona o mappa l’ambiente in cui desideri aggiornare una definizione di suddivisione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>Immettere o mappare il nome della suddivisione per la quale si desidera aggiornare una definizione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Aggiornare il contenuto]</td> 
   <td> <p>Per ogni attributo della suddivisione da aggiornare, fai clic su <b>[!UICONTROL Aggiungi elemento]</b> e immetti o mappa le modifiche desiderate.</p> <p>Per ulteriori informazioni, consulta <a href="https://docs.split.io/reference#partial-update-split-definition-in-environment">Definizione di suddivisione dell'aggiornamento parziale in ambiente</a> in [!DNL Split.io] documentazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Commenti]</td> 
   <td>Inserisci o mappa i commenti da aggiungere alla definizione di suddivisione.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Associa tag]

Questo modulo di azione aggiunge tag all&#39;oggetto specificato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Split.io] account a [!DNL Workfront Fusion], vedi <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Split.io] a [!UICONTROL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Seleziona o mappa l’area di lavoro in cui desideri aggiungere un tag.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Object Name]</td> 
   <td>Immettere o mappare il nome dell'oggetto a cui si desidera aggiungere i tag,</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di oggetto]</td> 
   <td> <p>Immettere o mappare il tipo di oggetto a cui si desidera aggiungere i tag.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tags]</td> 
   <td> <p>Per ogni tag da aggiungere, fai clic su <b>[!UICONTROL Aggiungi elemento]</b> e immetti o mappa il tag .</p> </td> 
  </tr> 
 </tbody> 
</table>

### Ricerche

* [[!UICONTROL Ottieni aree di lavoro]](#get-workspaces)
* [[!UICONTROL Ottieni ambienti]](#get-environments)
* [[!UICONTROL Get Splits]](#get-splits)
* [[!UICONTROL Elencare definizioni di suddivisione in un ambiente]](#list-split-definitions-in-an-environment)
* [[!UICONTROL Ottieni tipi di traffico]](#get-traffic-types)

#### [!UICONTROL Ottieni aree di lavoro]

Questo modulo di ricerca recupera le aree di lavoro di un&#39;organizzazione.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Split.io] account a [!DNL Workfront Fusion], vedi <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Split.io] a [!UICONTROL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Immettere o mappare il numero massimo di aree di lavoro che si desidera recuperare dal modulo durante ogni ciclo di esecuzione dello scenario.</td> 
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
   <td> <p>Per istruzioni su come collegare le [!DNL Split.io] account a [!DNL Workfront Fusion], vedi <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Split.io] a [!UICONTROL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Seleziona o mappa l’area di lavoro che contiene gli ambienti da elencare.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get Splits]

Questo modulo di ricerca recupera un elenco di suddivisioni.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Split.io] account a [!DNL Workfront Fusion], vedi <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Split.io] a [!UICONTROL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Selezionare o mappare l'area di lavoro contenente le suddivisioni che si desidera elencare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Immettere o mappare il numero massimo di suddivisioni che si desidera recuperare nel modulo durante ogni ciclo di esecuzione dello scenario.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Elencare definizioni di suddivisione in un ambiente]

Questo modulo di ricerca recupera un elenco di definizioni suddivise in un determinato ambiente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Split.io] account a [!DNL Workfront Fusion], vedi <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Split.io] a [!UICONTROL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Selezionare o mappare l'area di lavoro contenente le definizioni di suddivisione da elencare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome ambiente o ID]</td> 
   <td>Seleziona o mappa l’ambiente che contiene le definizioni di suddivisione da elencare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Immettere o mappare il numero massimo di definizioni suddivise che si desidera recuperare nel modulo durante ogni ciclo di esecuzione dello scenario.</td> 
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
   <td> <p>Per istruzioni su come collegare le [!DNL Split.io] account a [!DNL Workfront Fusion], vedi <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Split.io] a [!UICONTROL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Seleziona o mappa l’area di lavoro che contiene i tipi di traffico da elencare.</td> 
  </tr> 
 </tbody> 
</table>
