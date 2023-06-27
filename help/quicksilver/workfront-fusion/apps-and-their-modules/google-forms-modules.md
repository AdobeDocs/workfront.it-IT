---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli Forms di Google
description: Il [!DNL Adobe Workfront Fusion Google Forms] I moduli consentono di monitorare, selezionare, aggiungere, aggiornare o eliminare le risposte sul Forms Google.
author: Becky
feature: Workfront Fusion
exl-id: 45c86879-bc4e-4134-b63c-02410b9de43b
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1430'
ht-degree: 0%

---

# [!DNL Google Forms] moduli

Il [!DNL Adobe Workfront Fusion] [!DNL Google Forms] moduli di consentono di monitorare, selezionare, aggiungere, aggiornare o eliminare le risposte [!DNL Google Forms].

Per utilizzare [!DNL Google Docs] con [!DNL Adobe Workfront Fusion], è necessario disporre di un [!DNL Google] account. Se non hai un [!DNL Google] tuttavia, è possibile crearne uno in corrispondenza del [!DNL Google] Pagina della guida dell’account.

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

Da utilizzare [!DNL Google Forms] moduli, è necessario disporre di un [!DNL Google] account.

## Creazione di un foglio di calcolo dal modulo

Per utilizzare le risposte del modulo, è necessario creare il foglio di calcolo delle risposte.

1. Aprire il modulo.
1. Vai a **[!UICONTROL Risposte]** scheda.
1. Fai clic su **[!UICONTROL Crea foglio di calcolo]** icona ![](assets/spreadsheet-icon.png).

1. Seleziona se desideri creare un nuovo foglio di calcolo o un foglio di calcolo esistente
1. Fai clic su **[!UICONTROL Crea]**.

## [!DNL Google Forms] moduli e relativi campi

Quando si configura [!DNL Google Forms] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL Google Forms] I campi potrebbero essere visualizzati in base a fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se viene visualizzato il pulsante Mappa sopra un campo o una funzione, è possibile utilizzarlo per impostare variabili e funzioni per tale campo. Per ulteriori informazioni, consulta [Mappare le informazioni da un modulo all’altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Azioni](#actions)
* [Ricerche](#searches)

### Triggers

#### [!UICONTROL Osservare le risposte]

Controlla il modulo per individuare nuove risposte.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Google] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connetti l’app o il servizio web del modulo a [!DNL Workfront Fusion]</a> nell’articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Creare uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Foglio di calcolo di [!UICONTROL]</td> 
   <td> <p>Selezionare il foglio di calcolo contenente le risposte del modulo che si desidera controllare per individuare le nuove risposte.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Foglio]</td> 
   <td> <p> Selezionare il foglio contenente le risposte del modulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Riga con intestazioni]</td> 
   <td>Specifica la riga di intestazione della tabella. La riga predefinita è <code>A1:Z1</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Opzione di rendering del valore [!UICONTROL]</td> 
   <td> <p>Specifica come eseguire il rendering dei valori nell’output.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Valore formattato]</strong> </p> <p>I valori vengono calcolati e formattati nella risposta in base alla formattazione della cella. La formattazione si basa sulle impostazioni locali del foglio di calcolo, non sulle impostazioni locali dell'utente richiedente. Ad esempio, se <code>A1</code> è <code>1. 23</code> e <code>A2 </code>è <code>=A1</code> e formattato come valuta, quindi <code>A2</code> restituisce <code>$1. 23</code> .</p> </li> 
     <li> <p><strong>[!UICONTROL Valore non formattato]</strong> </p> <p>I valori vengono calcolati, ma non formattati nella risposta. Ad esempio, se <code>A1</code> è <code>1. 23</code> e <code>A2 </code>è <code>=A1</code> e formattato come valuta, quindi <code>A2</code> restituisce il numero <code>1. 23</code> .</p> </li> 
     <li> <p><strong>[!UICONTROL Formula]</strong> </p> <p>I valori non vengono calcolati. La risposta include le formule. Ad esempio, se <code>A1</code> è <code>1. 23</code> e <code>A2 </code>è <code>=A1</code> e formattato come valuta, quindi <code>A2</code> restituisce <code>=A1</code>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data e ora opzione di rendering]</td> 
   <td>Seleziona la modalità di rappresentazione di date, ore e durata nell’output. Questo campo viene ignorato se [!UICONTROL Value Render Option] è impostato su [!UICONTROL Formatted Value].</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p> Imposta il numero massimo di risposte [!DNL Workfront Fusion] funziona con durante un ciclo.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Azioni

* [[!UICONTROL Aggiungi una risposta]](#add-a-response)
* [[!UICONTROL Aggiornare una risposta]](#update-a-response)
* [[!UICONTROL Eliminare una risposta]](#delete-a-response)

#### [!UICONTROL Aggiungi una risposta]

Questo modulo aggiunge una nuova risposta alla parte inferiore del foglio di calcolo del modulo.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Google] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connetti l’app o il servizio web del modulo a [!DNL Workfront Fusion]</a> nell’articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Creare uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Foglio di calcolo di [!UICONTROL]</td> 
   <td> <p>Selezionare il foglio di calcolo contenente il foglio in cui si desidera aggiungere una risposta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Foglio]</td> 
   <td> <p> Selezionare il foglio contenente le risposte del modulo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Values]</p> </td> 
   <td> <p>Immetti i valori desiderati nelle colonne del foglio.</p> <p>Per la colonna [!UICONTROL Timestamp] nel formato corretto, utilizzare il valore seguente:</p><pre>formatDate(now;GG/MM/AAAA HH:mm;UTC)</pre> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Opzione di input del valore [!UICONTROL]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p> I valori immessi dall’utente non vengono analizzati e vengono memorizzati così come sono. </p> </li> 
     <li> <p><strong>[!UICONTROL User entered]</strong></p> <p>I valori vengono analizzati come se l’utente li avesse digitati nell’interfaccia utente. I numeri rimangono numeri, ma le stringhe possono essere convertite in numeri, date o altri formati seguendo le stesse regole applicate quando si immette testo in una cella tramite [!DNL Google Sheets] UI.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Inserisci dati, opzione]</td> 
   <td> <p>Specifica come vengono modificati i dati esistenti quando vengono immessi nuovi dati. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Overwrite]</strong> </p> <p>I nuovi dati sovrascrivono quelli esistenti nelle aree in cui vengono scritti. L'aggiunta di dati alla fine del foglio consente di inserire nuove righe o colonne in modo da poter scrivere i dati.</p> </li> 
     <li> <p><strong>[!UICONTROL Inserisci righe]</strong></p> <p>Le righe vengono inserite per i nuovi dati.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggiornare una risposta]

Questo modulo aggiorna la risposta selezionata.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Google] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connetti l’app o il servizio web del modulo a [!DNL Workfront Fusion]</a> nell’articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Creare uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Foglio di calcolo di [!UICONTROL]</td> 
   <td> <p>Selezionare il foglio di calcolo contenente il foglio in cui si desidera aggiornare una risposta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Foglio]</td> 
   <td> <p> Selezionare il foglio contenente le risposte del modulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Numero riga]</p> </td> 
   <td> <p>Immettere o mappare il numero della riga da aggiornare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Values]</p> </td> 
   <td> <p>Immettere i nuovi valori nelle colonne desiderate.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Opzione di input del valore [!UICONTROL]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p> I valori immessi dall’utente non vengono analizzati e vengono memorizzati così come sono. </p> </li> 
     <li> <p><strong>[!UICONTROL User entered]</strong></p> <p>I valori vengono analizzati come se l’utente li avesse digitati nell’interfaccia utente. I numeri rimangono numeri, ma le stringhe possono essere convertite in numeri, date o altri formati seguendo le stesse regole applicate quando si immette testo in una cella tramite [!DNL Google Sheets] UI.</p> </li> 
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
   <td> <p>Per istruzioni sulla connessione [!DNL Google] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connetti l’app o il servizio web del modulo a [!DNL Workfront Fusion]</a> nell’articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Creare uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Foglio di calcolo di [!UICONTROL]</td> 
   <td> <p>Selezionare il foglio di calcolo contenente il foglio in cui si desidera eliminare una risposta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Foglio]</td> 
   <td> <p> Selezionare il foglio contenente le risposte del modulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Numero riga]</p> </td> 
   <td> <p>Immettere o mappare il numero della riga da eliminare.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Ricerche

* [[!UICONTROL Cerca risposte]](#search-responses)
* [[!UICONTROL Cerca risposte (Avanzate)])](#search-responses-advanced)

#### [!UICONTROL Cerca risposte]

Questo modulo restituisce le risposte che corrispondono ai criteri specificati.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
    <td>Connessione</td>
   <td> <p>Per istruzioni sulla connessione [!DNL Google] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connetti l’app o il servizio web del modulo a [!DNL Workfront Fusion]</a> nell’articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Creare uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>Foglio di calcolo di [!UICONTROL]</td>
   <td> <p>Selezionare il modulo in cui eseguire la ricerca.</p> </td> 
  </tr> 
  <tr data-mc-conditions="">
    <td>[!UICONTROL Foglio] </td>
   <td> <p>Selezionare il foglio contenente le risposte del modulo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>[!UICONTROL Intervallo colonne]</td>
   <td> <p> Selezionare l'intervallo di colonne che si desidera cercare.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Filtro]</td> 
   <td> <p>Definisci il filtro in base al quale desideri cercare le risposte.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>Ordinamento [!UICONTROL] </td>
   <td> <p>Seleziona se ordinare le risposte restituite in ordine crescente o decrescente.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>[!UICONTROL Ordina per]</td>
   <td> <p> Selezionare la colonna in base alla quale ordinare le risposte restituite.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Opzione di rendering del valore [!UICONTROL]</td> 
   <td> <p>Specifica come eseguire il rendering dei valori nell’output.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Valore formattato]</strong></p> <p>I valori vengono calcolati e formattati nella risposta in base alla formattazione della cella. La formattazione si basa sulle impostazioni locali del foglio di calcolo, non sulle impostazioni locali dell'utente richiedente. Ad esempio, se <code>A1</code> è <code>1. 23</code> e <code>A2 </code>è <code>=A1</code> e formattato come valuta, quindi <code>A2</code> restituisce <code>$1. 23</code> .</p> </li> 
     <li> <p><strong>[!UICONTROL Valore non formattato]</strong> </p> <p>I valori vengono calcolati, ma non formattati nella risposta. Ad esempio, se <code>A1</code> è <code>1. 23</code> e <code>A2 </code>è <code>=A1</code> e formattato come valuta, quindi <code>A2</code> restituisce il numero <code>1. 23</code> .</p> </li> 
     <li> <p><strong>[!UICONTROL Formula]</strong> </p> <p>I valori non vengono calcolati. La risposta include le formule. Ad esempio, se <code>A1</code> è <code>1. 23</code> e <code>A2 </code>è <code>=A1</code> e formattato come valuta, quindi <code>A2</code> restituisce <code>=A1</code>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions="">
    <td>[!UICONTROL Data e ora opzione di rendering]</td>
    <td>Seleziona la modalità di rappresentazione di date, ore e durata nell’output. Questo campo viene ignorato se l'opzione [!UICONTROL Value Render] è impostata su Formatted Value. </td>
  </tr> 
  <tr>
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">[!UICONTROL Numero massimo di risposte restituite]</td>
   <td> <p> Imposta il numero massimo di risposte [!DNL Workfront Fusion] restituisce durante un ciclo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Risposte di ricerca (avanzate)]

Questo modulo esegue una ricerca utilizzando [[!DNL Google Charts Query Language]](https://developers.google.com/chart/interactive/docs/querylanguage). Questo modulo non restituisce un numero di riga.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Connection]</td>
   <td> <p>Per istruzioni sulla connessione [!DNL Google] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connetti l’app o il servizio web del modulo a [!DNL Workfront Fusion]</a> nell’articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Creare uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr>
    <td>Foglio di calcolo di [!UICONTROL]</td>
   <td> <p>Selezionare il foglio di calcolo contenente il foglio che si desidera cercare.</p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Foglio]</td>
   <td> <p> Selezionare il foglio contenente le risposte del modulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtro]</td> 
   <td> <p>Definire la query di ricerca utilizzando <a href="https://developers.google.com/chart/interactive/docs/querylanguage">[!DNL Google Charts Query Language]</a>.</p> <p>Esempio: <code>select * where C = "John"</code> recupera tutti i valori per la riga in cui la colonna C è "John".</p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Numero massimo di righe restituite]</td>
   <td> <p> Imposta il numero massimo di risposte [!DNL Workfront Fusion] restituisce durante un ciclo.</p> </td> 
  </tr> 
 </tbody> 
</table>
