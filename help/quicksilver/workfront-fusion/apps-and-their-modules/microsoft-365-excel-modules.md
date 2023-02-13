---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli Excel di Microsoft Office 365
description: In un [!DNL Adobe Workfront Fusion] In questo caso, è possibile automatizzare i flussi di lavoro che utilizzano Microsoft 365 Excel e collegarli a più applicazioni e servizi di terze parti.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 9aa3739d-6800-4eb1-a17f-32fdfd8ed0f2
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2577'
ht-degree: 0%

---

# [!DNL Microsoft Office 365 Excel] moduli

In un [!DNL Adobe Workfront Fusion] puoi automatizzare i flussi di lavoro che utilizzano [!DNL Microsoft 365 Excel], nonché collegarlo a più applicazioni e servizi di terze parti.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p>  </td>  
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

Per utilizzare [!DNL Microsoft office 365 Excel], devi disporre di un account Microsoft.

## [!DNL Microsoft Office 365 Excel] moduli e relativi campi

Quando si configura [!DNL Microsoft 365 Excel] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL Microsoft 365 Excel] potrebbero essere visualizzati, a seconda di fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se trovi il pulsante mappa sopra un campo o una funzione, puoi utilizzarlo per impostare variabili e funzioni per quel campo. Per ulteriori informazioni, consulta [Mappare informazioni da un modulo a un altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Cartella di lavoro](#workbook)
* [Worksheet](#worksheet)
* [Tabella](#table)
* [Altro](#other)

### Cartella di lavoro

* [Guarda le cartelle di lavoro](#watch-workbooks)
* [Cartelle di lavoro di ricerca](#search-workbooks)
* [Scaricare una cartella di lavoro](#download-a-workbook)

#### [!UICONTROL Guarda le cartelle di lavoro]

Questo modulo di attivazione avvia uno scenario quando viene creata una cartella di lavoro.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Collega l’app o il servizio Web del modulo a [!DNL Workfront Fusion]</a> nell'articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crea uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cartella]</td> 
   <td> <p>Selezionare la cartella di cui si desidera tenere traccia per le nuove cartelle di lavoro.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Filter]</p> </td> 
   <td> <p>È possibile impostare un filtro per controllare solo le cartelle di lavoro che soddisfano i criteri selezionati.</p> <p>Per ogni filtro, immetti il campo da valutare dal filtro, l’operatore e il valore che desideri che il filtro consenta. Puoi utilizzare più di un filtro aggiungendo regole AND o OR .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Immettere o mappare il numero massimo di cartelle di lavoro che si desidera che il modulo restituisca durante ogni ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Cartelle di lavoro di ricerca]

Questo modulo di azione cerca [!DNL Excel] cartelle di lavoro.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Collega l’app o il servizio Web del modulo a [!DNL Workfront Fusion]</a> nell'articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crea uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cartella]</td> 
   <td> <p>Selezionare la cartella in cui si desidera cercare le cartelle di lavoro.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Filter]</p> </td> 
   <td> <p>È possibile impostare un filtro per cercare solo le cartelle di lavoro che soddisfano i criteri selezionati.</p> <p>Per ogni filtro, immetti il campo da valutare dal filtro, l’operatore e il valore che desideri che il filtro consenta. Puoi utilizzare più di un filtro aggiungendo regole AND o OR .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Immettere o mappare il numero massimo di fogli di lavoro che si desidera che venga restituito dal modulo durante ogni ciclo di esecuzione di uno scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Scaricare una cartella di lavoro]

Questo modulo di azione scarica il contenuto della cartella di lavoro Excel specificata.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Collega l’app o il servizio Web del modulo a [!DNL Workfront Fusion]</a> nell'articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crea uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scaricare una cartella di lavoro]</td> 
   <td> <p>Selezionare la modalità di identificazione della cartella di lavoro per il modulo da scaricare.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Immetti un ID manualmente]</strong> </p> <p>Nel campo ID cartella di lavoro immettere o mappare l'ID della cartella di lavoro specifica che si desidera scaricare nel modulo.</p> </li> 
     <li> <p><strong>[!UICONTROL Selezionando dal percorso]</strong> </p> <p>Nel campo Cartella di lavoro selezionare la cartella di lavoro che si desidera scaricare dal modulo.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Worksheet

* [[!UICONTROL Righe foglio di lavoro di controllo]](#watch-worksheet-rows)
* [[!UICONTROL Elenca fogli di lavoro]](#list-worksheets)
* [[!UICONTROL Elenca righe foglio di lavoro]](#list-worksheet-rows)
* [[!UICONTROL Aggiungi un foglio di lavoro]](#add-a-worksheet)
* [[!UICONTROL Aggiungi riga foglio di lavoro]](#add-a-worksheet-row)
* [[!UICONTROL Aggiornare una riga del foglio di lavoro]](#update-a-worksheet-row)
* [[!UICONTROL Eliminare una riga del foglio di lavoro]](#delete-a-worksheet-row)

#### [!UICONTROL Righe foglio di lavoro di controllo]

Questo modulo di attivazione avvia uno scenario in cui viene aggiunta una nuova riga al foglio.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Collega l’app o il servizio Web del modulo a [!DNL Workfront Fusion]</a> nell'articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crea uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >Cartella di lavoro [!UICONTROL] </td>
   <td> <p>Selezionare la cartella di lavoro contenente il foglio di lavoro che si desidera controllare per le nuove righe.</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL Foglio di lavoro] </td>
   <td> <p>Selezionare il foglio di Excel che si desidera controllare per le nuove righe.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limit]</td>
   <td> <p>Immettere o mappare il numero massimo di righe del foglio di lavoro che si desidera che il modulo restituisca durante ogni ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Elenca fogli di lavoro]

Questo modulo di azione recupera un elenco di fogli di lavoro nella cartella di lavoro specificata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Collega l’app o il servizio Web del modulo a [!DNL Workfront Fusion]</a> nell'articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crea uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >Cartella di lavoro [!UICONTROL] </td>
   <td> <p>Selezionare la cartella di lavoro contenente i fogli di lavoro che si desidera elencare nel modulo.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limit]</td>
   <td> <p>Immettere o mappare il numero massimo di fogli di lavoro che si desidera che venga restituito dal modulo durante ogni ciclo di esecuzione di uno scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Elenca righe foglio di lavoro]

Questo modulo di azione recupera un elenco di righe nel foglio di lavoro specificato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Collega l’app o il servizio Web del modulo a [!DNL Workfront Fusion]</a> nell'articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crea uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >Cartella di lavoro [!UICONTROL] </td>
   <td> <p>Selezionare la cartella di lavoro contenente il foglio di lavoro che include le righe che si desidera elencare.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Foglio di lavoro] </td>
   <td> <p>Selezionare il foglio di lavoro contenente le righe che si desidera elencare.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limit]</td>
   <td> <p>Immettere o mappare il numero massimo di righe del foglio di lavoro che si desidera che il modulo restituisca durante ogni ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggiungi un foglio di lavoro]

Questo modulo di azione crea un nuovo foglio di lavoro all&#39;interno della cartella di lavoro selezionata.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Collega l’app o il servizio Web del modulo a [!DNL Workfront Fusion]</a> nell'articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crea uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >Cartella di lavoro [!UICONTROL] </td>
   <td> <p>Selezionare la cartella di lavoro in cui si desidera aggiungere un foglio di lavoro.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Name] </td>
   <td> <p>Immettere o mappare un nome per il nuovo foglio di lavoro.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggiungi riga foglio di lavoro]

Questo modulo di azione aggiunge una nuova riga al foglio di lavoro selezionato.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Collega l’app o il servizio Web del modulo a [!DNL Workfront Fusion]</a> nell'articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crea uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >Cartella di lavoro [!UICONTROL] </td>
   <td> <p>Selezionare la cartella di lavoro contenente il foglio di lavoro in cui si desidera aggiungere una riga.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Foglio di lavoro] </td>
   <td> <p>Selezionare il foglio di lavoro in cui si desidera aggiungere una riga.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Tipo di valori immesso]</p> </td> 
   <td> <p>Selezionare il tipo di valore da immettere nel foglio di lavoro. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Formulas]</strong> </p> <p> Excel cerca di valutare l'espressione specificata. I nomi delle funzioni in una formula sono in inglese. Esempio: <code>[!DNL =SUM(A1:A10)]</code></p> </li> 
     <li> <p><strong>[!UICONTROL Formule locali]</strong> </p> <p>Excel cerca di valutare l'espressione specificata. I nomi delle funzioni sono nella lingua dell'applicazione Excel. Esempio: <code>=SUM(A1, 1.5)</code> vs <code>=SUMME(A1; 1,5)</code></p> </li> 
     <li> <p><strong>[!UICONTROL Value]</strong> </p> <p>Excel non valuta il valore. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Riga]</td>
    <td>Per ogni colonna, immettere il valore che si desidera assegnare alla colonna nella nuova riga.</td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggiornare una riga del foglio di lavoro]

Questo modulo di azione aggiorna una riga del foglio di lavoro esistente.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Collega l’app o il servizio Web del modulo a [!DNL Workfront Fusion]</a> nell'articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crea uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >Cartella di lavoro [!UICONTROL] </td>
   <td> <p>Selezionare la cartella di lavoro contenente il foglio di lavoro che include la riga che si desidera aggiornare.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Foglio di lavoro] </td>
   <td> <p>Selezionare il foglio di lavoro contenente la riga che si desidera aggiornare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Tipo di valori immesso]</p> </td> 
   <td> <p>Selezionare il tipo di valore da immettere nel foglio di lavoro. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Formulas]</strong> </p> <p> Excel cerca di valutare l'espressione specificata. I nomi delle funzioni in una formula sono in inglese. Esempio: <code>[!DNL =SUM(A1:A10)]</code></p> </li> 
     <li> <p><strong>[!UICONTROL Formule locali]</strong> </p> <p>Excel cerca di valutare l'espressione specificata. I nomi delle funzioni sono nella lingua dell'applicazione Excel. Esempio: <code>=SUM(A1, 1.5)</code> vs <code>=SUMME(A1; 1,5)</code></p> </li> 
     <li> <p><strong>[!UICONTROL Value]</strong> </p> <p>Excel non valuta il valore. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID riga]</td> 
   <td>Seleziona il numero della riga da aggiornare.</td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Riga]</td>
    <td>Per ogni colonna, immettere il valore che si desidera assegnare alla colonna nella nuova riga.</td>
   —&gt; 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminare una riga del foglio di lavoro]

Questo modulo di azione elimina una riga da un foglio di lavoro.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Collega l’app o il servizio Web del modulo a [!DNL Workfront Fusion]</a> nell'articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crea uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >Cartella di lavoro [!UICONTROL] </td>
   <td> <p>Selezionare la cartella di lavoro contenente il foglio di lavoro che include la riga da eliminare.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Foglio di lavoro]</td>
   <td> <p> Selezionare il foglio di lavoro contenente la riga da eliminare.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL ID riga]</td>
   <td>Immetti o mappa l’ID della riga da eliminare.</td> 
  </tr> 
 </tbody> 
</table>

### Tabella

* [[!UICONTROL Osserva righe tabella]](#watch-table-rows)
* [[!UICONTROL Tabelle elenco]](#list-tables)
* [[!UICONTROL Elenca righe tabella]](#list-table-rows)
* [[!UICONTROL Ottieni una tabella]](#get-a-table)
* [[!UICONTROL Aggiungi una tabella]](#add-a-table)
* [[!UICONTROL Aggiungere una riga di tabella]](#add-a-table-row)
* [[!UICONTROL Aggiornare una tabella]](#update-a-table)
* [[!UICONTROL Eliminare una tabella]](#delete-a-table)

#### [!UICONTROL Osserva righe tabella]

Questo trigger avvia uno scenario in cui viene aggiunta una nuova riga a una tabella.

>[!NOTE]
>
>La tabella qui fa riferimento all’elemento di tabella incorporato nella cartella di lavoro. Non l&#39;intera tabella (cartella di lavoro/foglio).

![](assets/embedded-table-350x420.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Collega l’app o il servizio Web del modulo a [!DNL Workfront Fusion]</a> nell'articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crea uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Cartella di lavoro [!UICONTROL]</p> </td> 
   <td> <p>Selezionare la cartella di lavoro contenente la tabella che si desidera controllare.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Foglio di lavoro] </td>
   <td> <p> Selezionare il foglio di lavoro che contiene la tabella che si desidera controllare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Tabella]</p> </td> 
   <td> <p>Selezionare la tabella che si desidera controllare.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limit]</td>
   <td> <p>Immetti o mappa il numero massimo di righe che desideri che il modulo restituisca durante ogni ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Tabelle elenco]

Questo modulo di ricerca recupera un elenco di tutti gli oggetti tabella.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Collega l’app o il servizio Web del modulo a [!DNL Workfront Fusion]</a> nell'articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crea uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >Cartella di lavoro [!UICONTROL] </td>
   <td> <p>Selezionare la cartella di lavoro contenente le tabelle che si desidera elencare.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Foglio di lavoro] </td>
   <td> <p>Selezionare il foglio di lavoro contenente le tabelle che si desidera elencare</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limit]</td>
   <td> <p>Immettere o mappare il numero massimo di tabelle che si desidera restituire dal modulo durante ogni ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Elenca righe tabella]

Questo modulo di ricerca recupera un elenco di tutte le righe di tabella in una cartella di lavoro.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Collega l’app o il servizio Web del modulo a [!DNL Workfront Fusion]</a> nell'articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crea uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >Cartella di lavoro [!UICONTROL] </td>
   <td> <p>Selezionare la cartella di lavoro contenente la tabella che include le righe che si desidera elencare.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Foglio di lavoro] </td>
   <td> <p>Selezionare il foglio di lavoro che contiene la tabella contenente le righe che si desidera elencare</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Tabella] </td>
   <td> <p>Selezionare la tabella contenente le righe che si desidera elencare.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limit]</td>
   <td> <p>Immettere o mappare il numero massimo di righe di tabella che si desidera che il modulo restituisca durante ogni ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottieni una tabella]

Questo modulo di azione recupera i metadati per la tabella specificata.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> 
     <p >[!UICONTROL Connection]</p>
   </td> 
   <td> 
     <p>Per istruzioni su come collegare l'account Office 365 a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Collega l’app o il servizio Web del modulo a [!DNL Workfront Fusion]</a> nell'articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crea uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p>
    --&gt; </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ottieni una tabella]</td> 
   <td> <p>Selezionare la modalità di identificazione della tabella da recuperare.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Invio manuale]</strong> </p> <p>Nel campo ID cartella di lavoro immettere o mappare l'ID della cartella di lavoro che contiene la tabella da recuperare.</p> <p>Nel campo [!UICONTROL Table Name] (Nome tabella) immettere o mappare il nome della tabella da recuperare.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleziona dall’elenco]</strong> </p> <p>Selezionare la cartella di lavoro e il foglio di lavoro che contengono la tabella che si desidera recuperare, quindi selezionare la tabella.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggiungi una tabella]

Questo modulo di azione crea un elemento tabella nel foglio di lavoro di Excel.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Collega l’app o il servizio Web del modulo a [!DNL Workfront Fusion]</a> nell'articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crea uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Cartella di lavoro [!UICONTROL] </td> 
   <td> <p>Selezionare la cartella di lavoro contenente il foglio di lavoro in cui si desidera aggiungere una tabella.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Foglio di lavoro] </td> 
   <td> <p>Selezionare il foglio di lavoro in cui si desidera aggiungere una tabella.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Con intestazioni]</td> 
   <td> <p>Abilitare questa opzione per definire la prima riga come intestazioni di tabella.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Address]</p> </td> 
   <td> <p>Impostare le dimensioni della tabella indicando le celle in alto a sinistra e in basso a destra. Esempio: <code>A1:C10</code> crea una tabella con 3 colonne e 10 righe.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggiungere una riga di tabella]

Questo modulo di azione modifica una tabella esistente.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Collega l’app o il servizio Web del modulo a [!DNL Workfront Fusion]</a> nell'articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crea uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >Cartella di lavoro [!UICONTROL] </td>
   <td> <p>Selezionare la cartella di lavoro contenente la tabella in cui si desidera aggiungere una riga.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Foglio di lavoro] </td>
   <td> <p>Selezionare il foglio di lavoro che contiene la tabella in cui si desidera aggiungere una riga.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Tabella]</td>
   <td>Selezionare la tabella in cui si desidera aggiungere una riga.</td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL Riga]</td>
    <td>Per ogni colonna, immettere il valore che si desidera assegnare alla colonna nella nuova riga.</td>
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID riga]</p> </td> 
   <td> <p>Per aggiungere una riga in una posizione specifica nella tabella, immettere o mappare un numero di riga. Il modulo inserisce la nuova riga dopo questa riga.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggiornare una tabella]

Questo modulo di azione aggiorna una tabella esistente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Collega l’app o il servizio Web del modulo a [!DNL Workfront Fusion]</a> nell'articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crea uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Aggiornare una tabella]</td> 
   <td> <p>Selezionare la modalità di identificazione della tabella da aggiornare.</p> 
    <ul> 
     <li> <p><strong>Immettere manualmente</strong> </p> <p>Nel campo ID cartella di lavoro immettere o mappare l'ID della cartella di lavoro che contiene la tabella da aggiornare.</p> <p>Nel campo [!UICONTROL Table Name] (Nome tabella) immettere o mappare il nome della tabella da aggiornare.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleziona dall’elenco]</strong> </p> <p>Selezionare la cartella di lavoro e il foglio di lavoro che contengono la tabella che si desidera aggiornare, quindi selezionare la tabella.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tabella] </td> 
   <td> <p>Selezionare la tabella da aggiornare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name]</td> 
   <td> <p>Se si desidera rinominare la tabella, immettere o mappare un nuovo nome per la tabella.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mostra intestazioni]</td> 
   <td> <p>Abilita questa opzione per visualizzare le intestazioni della tabella aggiornata.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mostra totali]</td> 
   <td>Abilitare questa opzione per visualizzare i valori totali della tabella.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Style]</td> 
   <td>Scegliere uno stile per la nuova tabella.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminare una tabella]

Questo modulo di azione elimina la tabella specificata da un [!DNL Excel] foglio di lavoro.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Collega l’app o il servizio Web del modulo a [!DNL Workfront Fusion]</a> nell'articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crea uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ottieni una tabella]</td> 
   <td> <p>Selezionare la modalità di identificazione della tabella da eliminare.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Invio manuale]</strong> </p> <p>Nel campo ID cartella di lavoro immettere o mappare l'ID della cartella di lavoro che contiene la tabella da eliminare.</p> <p>Nel campo [!UICONTROL Table Name] (Nome tabella) immettere o mappare il nome della tabella da eliminare.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleziona dall’elenco]</strong> </p> <p>Selezionare la cartella di lavoro e il foglio di lavoro che contengono la tabella da eliminare, quindi selezionare la tabella.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Altro

* [[!UICONTROL Recupera dati]](#retrieve-data)
* [[!UICONTROL Effettuare una chiamata API]](#make-an-api-call)

#### [!UICONTROL Recupera dati]

Questa azione recupera i dati dall&#39;intervallo definito del foglio di lavoro e restituisce un bundle per ogni riga.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Collega l’app o il servizio Web del modulo a [!DNL Workfront Fusion]</a> nell'articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crea uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Cartella di lavoro [!UICONTROL] </td> 
   <td> <p>Selezionare la cartella di lavoro contenente i dati che si desidera recuperare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Foglio di lavoro] </td> 
   <td> <p>Selezionare il foglio di lavoro contenente i dati che si desidera recuperare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Range] </td> 
   <td> <p>Specificare l'area del foglio da cui si desidera recuperare i dati indicando le celle in alto a sinistra e in basso a destra. Esempio: <code>A1:D10</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Effettuare una chiamata API]

Questo modulo di azione ti consente di effettuare una chiamata API personalizzata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Collega l’app o il servizio Web del modulo a [!DNL Workfront Fusion]</a> nell'articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crea uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Immettere un percorso relativo a <code>https://graph.microsoft.com</code>. Esempio:<code> /v1.0/me/drive/root/children</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL, Metodo]</td> 
   td&gt; <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
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
   <td> <p>Aggiungi il contenuto del corpo per la chiamata API sotto forma di un oggetto JSON standard.</p> <p>Nota:   <p>Quando si utilizzano istruzioni condizionali come <code>if</code> nel JSON, inserisci le virgolette al di fuori dell’istruzione condizionale.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>
