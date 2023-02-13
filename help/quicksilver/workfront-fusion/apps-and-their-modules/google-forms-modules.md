---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli Google Forms
description: La [!DNL Adobe Workfront Fusion Google Forms] I moduli ti consentono di monitorare, selezionare, aggiungere, aggiornare o eliminare le risposte sul tuo Forms Google.
author: Becky
feature: Workfront Fusion
exl-id: 45c86879-bc4e-4134-b63c-02410b9de43b
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1382'
ht-degree: 0%

---

# [!DNL Google Forms] moduli

La [!DNL Adobe Workfront Fusion] [!DNL Google Forms] i moduli ti consentono di monitorare, selezionare, aggiungere, aggiornare o eliminare le risposte [!DNL Google Forms].

Per utilizzare [!DNL Google Docs] con [!DNL Adobe Workfront Fusion], è necessario disporre di un [!DNL Google] conto. Se non hai un [!DNL Google] tuttavia, è possibile crearne una nella [!DNL Google] Pagina della guida dell’account.

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

Per utilizzare [!DNL Google Forms] moduli, è necessario disporre di un [!DNL Google] conto.

## Creazione di un foglio di calcolo dal modulo

Per utilizzare le risposte del modulo, è necessario creare il foglio di calcolo delle risposte.

1. Apri il modulo.
1. Vai a **[!UICONTROL Risposte]** scheda .
1. Fai clic sul pulsante **[!UICONTROL Crea foglio di calcolo]** icona ![](assets/spreadsheet-icon.png).

1. Seleziona se desideri creare un nuovo foglio di calcolo o un foglio di calcolo esistente
1. Fai clic su **[!UICONTROL Crea]**.

## [!DNL Google Forms] moduli e relativi campi

Quando si configura [!DNL Google Forms] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL Google Forms] potrebbero essere visualizzati, a seconda di fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se trovi il pulsante mappa sopra un campo o una funzione, puoi utilizzarlo per impostare variabili e funzioni per quel campo. Per ulteriori informazioni, consulta [Mappare informazioni da un modulo a un altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Azioni](#actions)
* [Ricerche](#searches)

### Triggers

#### [!UICONTROL Risposte di controllo]

Visualizza il modulo per le nuove risposte.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Collega l’app o il servizio Web del modulo a [!DNL Workfront Fusion]</a> nell'articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crea uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Foglio di calcolo]</td> 
   <td> <p>Selezionare il foglio di calcolo contenente le risposte del modulo che si desidera controllare per le nuove risposte.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sheet]</td> 
   <td> <p> Selezionare il foglio contenente le risposte del modulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Riga con intestazioni]</td> 
   <td>Specifica la riga di intestazione della tabella. La riga predefinita è <code>A1:Z1</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Valore Render Option]</td> 
   <td> <p>Specifica come eseguire il rendering dei valori nell'output.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Valore formattato]</strong> </p> <p>I valori vengono calcolati e formattati nella risposta in base alla formattazione della cella. La formattazione si basa sulle impostazioni internazionali del foglio di calcolo, non sulle impostazioni internazionali dell'utente richiedente. Ad esempio, se <code>A1</code> è <code>1. 23</code> e <code>A2 </code>è <code>=A1</code> e formattato come valuta, quindi <code>A2</code> return <code>$1. 23</code> .</p> </li> 
     <li> <p><strong>[!UICONTROL Valore non formattato]</strong> </p> <p>I valori vengono calcolati, ma non formattati nella risposta. Ad esempio, se <code>A1</code> è <code>1. 23</code> e <code>A2 </code>è <code>=A1</code> e formattato come valuta, quindi <code>A2</code> restituisce il numero <code>1. 23</code> .</p> </li> 
     <li> <p><strong>Formula [!UICONTROL]</strong> </p> <p>I valori non vengono calcolati. La risposta include le formule. Ad esempio, se <code>A1</code> è <code>1. 23</code> e <code>A2 </code>è <code>=A1</code> e formattato come valuta, quindi <code>A2</code> return <code>=A1</code>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Opzione di rendering per data e ora]</td> 
   <td>Seleziona la modalità di rappresentazione di date, ore e durata nell’output. Questo campo viene ignorato se [!UICONTROL Value Render Option] è impostato su [!UICONTROL Formatted Value].</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p> Imposta il numero massimo di risposte che [!DNL Workfront Fusion] funziona con durante un ciclo.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Azioni

* [[!UICONTROL Aggiungi una risposta]](#add-a-response)
* [[!UICONTROL Aggiornare una risposta]](#update-a-response)
* [[!UICONTROL Eliminare una risposta]](#delete-a-response)

#### [!UICONTROL Aggiungi una risposta]

Questo modulo aggiunge una nuova risposta alla parte inferiore del foglio di calcolo del modulo.

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Collega l’app o il servizio Web del modulo a [!DNL Workfront Fusion]</a> nell'articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crea uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Foglio di calcolo]</td> 
   <td> <p>Selezionare il foglio di calcolo contenente il foglio in cui si desidera aggiungere una risposta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sheet]</td> 
   <td> <p> Selezionare il foglio contenente le risposte del modulo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Values]</p> </td> 
   <td> <p>Immettere i valori desiderati nelle colonne del foglio.</p> <p>Per la colonna [!UICONTROL Timestamp] nel formato corretto, utilizza il seguente valore:</p><pre>formatDate(now;DD/MM/YYYY HH:mm;UTC)</pre> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Opzione di immissione del valore]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p> I valori immessi dall’utente non vengono analizzati e vengono memorizzati così come sono. </p> </li> 
     <li> <p><strong>[!UICONTROL Utente inserito]</strong></p> <p>I valori vengono analizzati come se l’utente li avesse digitati nell’interfaccia utente. I numeri rimangono numeri, ma le stringhe possono essere convertite in numeri, date o altri formati seguendo le stesse regole applicate quando si immette del testo in una cella tramite la [!DNL Google Sheets] Interfaccia utente.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Inserisci opzione dati]</td> 
   <td> <p>Specificare la modalità di modifica dei dati esistenti quando vengono immessi nuovi dati. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Sovrascrivi]</strong> </p> <p>I nuovi dati sovrascrivono quelli esistenti nelle aree in cui sono scritti. L'aggiunta di dati alla fine del foglio inserisce nuove righe o colonne in modo che i dati possano essere scritti.</p> </li> 
     <li> <p><strong>[!UICONTROL Inserisci righe]</strong></p> <p>Vengono inserite righe per i nuovi dati.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggiornare una risposta]

Questo modulo aggiorna la risposta selezionata.

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Collega l’app o il servizio Web del modulo a [!DNL Workfront Fusion]</a> nell'articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crea uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Foglio di calcolo]</td> 
   <td> <p>Selezionare il foglio di calcolo contenente il foglio in cui si desidera aggiornare una risposta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sheet]</td> 
   <td> <p> Selezionare il foglio contenente le risposte del modulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Numero di riga]</p> </td> 
   <td> <p>Immettere o mappare il numero della riga che si desidera aggiornare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Values]</p> </td> 
   <td> <p>Immetti i nuovi valori per le colonne desiderate.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Opzione di immissione del valore]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p> I valori immessi dall’utente non vengono analizzati e vengono memorizzati così come sono. </p> </li> 
     <li> <p><strong>[!UICONTROL Utente inserito]</strong></p> <p>I valori vengono analizzati come se l’utente li avesse digitati nell’interfaccia utente. I numeri rimangono numeri, ma le stringhe possono essere convertite in numeri, date o altri formati seguendo le stesse regole applicate quando si immette del testo in una cella tramite la [!DNL Google Sheets] Interfaccia utente.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminare una risposta]

Questo modulo elimina una risposta selezionata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Google] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Collega l’app o il servizio Web del modulo a [!DNL Workfront Fusion]</a> nell'articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crea uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Foglio di calcolo]</td> 
   <td> <p>Selezionare il foglio di calcolo contenente il foglio in cui si desidera eliminare una risposta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sheet]</td> 
   <td> <p> Selezionare il foglio contenente le risposte del modulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Numero di riga]</p> </td> 
   <td> <p>Immettere o mappare il numero della riga da eliminare.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Ricerche

* [[!UICONTROL Risposte alla ricerca]](#search-responses)
* [[!UICONTROL Risposte alla ricerca (avanzate])](#search-responses-advanced)

#### [!UICONTROL Risposte alla ricerca]

Questo modulo restituisce le risposte corrispondenti ai criteri specificati.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
    <td>Connessione</td>
   <td> <p>Per istruzioni su come collegare le [!DNL Google] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Collega l’app o il servizio Web del modulo a [!DNL Workfront Fusion]</a> nell'articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crea uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>[!UICONTROL Foglio di calcolo]</td>
   <td> <p>Selezionare il modulo da cercare.</p> </td> 
  </tr> 
  <tr data-mc-conditions="">
    <td>[!UICONTROL Sheet] </td>
   <td> <p>Selezionare il foglio contenente le risposte del modulo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>[!UICONTROL Intervallo colonne]</td>
   <td> <p> Selezionare l’intervallo di colonne da cercare.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td> <p>Definisci il filtro per il quale vuoi cercare le risposte alle risposte.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>Ordinamento [!UICONTROL] </td>
   <td> <p>Seleziona se ordinare le risposte restituite in ordine crescente o decrescente.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>[!UICONTROL Ordina per]</td>
   <td> <p> Selezionare la colonna per la quale si desidera ordinare le risposte restituite.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Valore Render Option]</td> 
   <td> <p>Specifica come eseguire il rendering dei valori nell'output.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Valore formattato]</strong></p> <p>I valori vengono calcolati e formattati nella risposta in base alla formattazione della cella. La formattazione si basa sulle impostazioni internazionali del foglio di calcolo, non sulle impostazioni internazionali dell'utente richiedente. Ad esempio, se <code>A1</code> è <code>1. 23</code> e <code>A2 </code>è <code>=A1</code> e formattato come valuta, quindi <code>A2</code> return <code>$1. 23</code> .</p> </li> 
     <li> <p><strong>[!UICONTROL Valore non formattato]</strong> </p> <p>I valori vengono calcolati, ma non formattati nella risposta. Ad esempio, se <code>A1</code> è <code>1. 23</code> e <code>A2 </code>è <code>=A1</code> e formattato come valuta, quindi <code>A2</code> restituisce il numero <code>1. 23</code> .</p> </li> 
     <li> <p><strong>Formula [!UICONTROL]</strong> </p> <p>I valori non vengono calcolati. La risposta include le formule. Ad esempio, se <code>A1</code> è <code>1. 23</code> e <code>A2 </code>è <code>=A1</code> e formattato come valuta, quindi <code>A2</code> return <code>=A1</code>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions="">
    <td>[!UICONTROL Opzione di rendering per data e ora]</td>
    <td>Seleziona la modalità di rappresentazione di date, ore e durata nell’output. Questo campo viene ignorato se l’opzione [!UICONTROL Value Render] è impostata su Valore formattato. </td>
  </tr> 
  <tr>
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">[!UICONTROL Numero massimo di risposte restituite]</td>
   <td> <p> Imposta il numero massimo di risposte che [!DNL Workfront Fusion] restituisce durante un ciclo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Risposte alla ricerca (avanzate)]

Questo modulo esegue una ricerca utilizzando [[!DNL Google Charts Query Language]](https://developers.google.com/chart/interactive/docs/querylanguage). Questo modulo non restituisce un numero di riga.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Connection]</td>
   <td> <p>Per istruzioni su come collegare le [!DNL Google] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Collega l’app o il servizio Web del modulo a [!DNL Workfront Fusion]</a> nell'articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crea uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Foglio di calcolo]</td>
   <td> <p>Selezionare il foglio di calcolo contenente il foglio da cercare.</p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Sheet]</td>
   <td> <p> Selezionare il foglio contenente le risposte del modulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td> <p>Definire la query di ricerca utilizzando <a href="https://developers.google.com/chart/interactive/docs/querylanguage">[!DNL Google Charts Query Language]</a>.</p> <p>Esempio: <code>select * where C = "John"</code> recupera tutti i valori per la riga in cui la colonna C è "John".</p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Numero massimo di righe restituite]</td>
   <td> <p> Imposta il numero massimo di risposte che [!DNL Workfront Fusion] restituisce durante un ciclo.</p> </td> 
  </tr> 
 </tbody> 
</table>
