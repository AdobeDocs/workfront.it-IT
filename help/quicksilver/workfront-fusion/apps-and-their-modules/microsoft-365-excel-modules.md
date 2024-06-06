---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli Excel di Microsoft Office 365
description: In un [!DNL Adobe Workfront Fusion] scenario, puoi automatizzare i flussi di lavoro che utilizzano Microsoft 365 Excel e collegarlo a più applicazioni e servizi di terze parti.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 9aa3739d-6800-4eb1-a17f-32fdfd8ed0f2
source-git-commit: 7d5f7c21fe38d43fb5601c81b8a31cc80587848f
workflow-type: tm+mt
source-wordcount: '2744'
ht-degree: 0%

---

# [!DNL Microsoft Office 365 Excel] moduli

In un [!DNL Adobe Workfront Fusion] scenario, puoi automatizzare i flussi di lavoro che utilizzano [!DNL Microsoft 365 Excel], oltre a collegarlo a più applicazioni e servizi di terze parti.

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

Da utilizzare [!DNL Microsoft office 365 Excel], è necessario disporre di un account Microsoft.



## Collegamento di [!DNL Office 365 Excel] servizio a [!DNL Workfront Fusion]

Per istruzioni sulla connessione [!DNL Office 365 Excel] account a [!UICONTROL Workfront Fusion], vedi [Creare una connessione a [!UICONTROL Adobe Workfront Fusion] - Istruzioni di base](../../workfront-fusion/connections/connect-to-fusion-general.md)

>[!NOTE]
>
>Alcune app Microsoft utilizzano la stessa connessione, che è associata alle autorizzazioni dei singoli utenti. Pertanto, durante la creazione di una connessione, nella schermata di consenso delle autorizzazioni vengono visualizzate tutte le autorizzazioni concesse in precedenza alla connessione dell’utente, oltre alle nuove autorizzazioni necessarie per l’applicazione corrente.
>
>Ad esempio, se un utente dispone delle autorizzazioni &quot;Leggi tabella&quot; concesse tramite il connettore Excel e quindi crea una connessione nel connettore Outlook per leggere le e-mail, nella schermata di consenso delle autorizzazioni verranno visualizzate sia l’autorizzazione &quot;Leggi tabella&quot; già concessa che l’autorizzazione &quot;Scrivi e-mail&quot; appena richiesta.

## [!DNL Microsoft Office 365 Excel] moduli e relativi campi

Quando si configura [!DNL Microsoft 365 Excel] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL Microsoft 365 Excel] I campi potrebbero essere visualizzati in base a fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se viene visualizzato il pulsante Mappa sopra un campo o una funzione, è possibile utilizzarlo per impostare variabili e funzioni per tale campo. Per ulteriori informazioni, consulta [Mappare le informazioni da un modulo all’altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Cartella di lavoro](#workbook)
* [Foglio di lavoro](#worksheet)
* [Tabella](#table)
* [Altro](#other)

### Cartella di lavoro

* [Cartelle di lavoro di controllo](#watch-workbooks)
* [Cerca cartelle di lavoro](#search-workbooks)
* [Scaricare una cartella di lavoro](#download-a-workbook)

#### [!UICONTROL Cartelle di lavoro di controllo]

Questo modulo di attivazione avvia uno scenario quando viene creata una cartella di lavoro.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connetti l’app o il servizio web del modulo a [!DNL Workfront Fusion]</a> nell’articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Creare uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td> <p>Selezionare la cartella da controllare per le nuove cartelle di lavoro.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Filtro]</p> </td> 
   <td> <p>È possibile impostare un filtro per controllare solo le cartelle di lavoro che soddisfano i criteri selezionati.</p> <p>Per ogni filtro, immetti il campo che desideri che il filtro valuti, l’operatore e il valore che desideri che il filtro consenta. Puoi utilizzare più di un filtro aggiungendo regole AND o OR.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Immettere o mappare il numero massimo di cartelle di lavoro che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Cerca cartelle di lavoro]

Questo modulo di azione cerca [!DNL Excel] cartelle di lavoro.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connetti l’app o il servizio web del modulo a [!DNL Workfront Fusion]</a> nell’articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Creare uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td> <p>Selezionare la cartella in cui si desidera cercare le cartelle di lavoro.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Filtro]</p> </td> 
   <td> <p>È possibile impostare un filtro per cercare solo le cartelle di lavoro che soddisfano i criteri selezionati.</p> <p>Per ogni filtro, immetti il campo che desideri che il filtro valuti, l’operatore e il valore che desideri che il filtro consenta. Puoi utilizzare più di un filtro aggiungendo regole AND o OR.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Immettere o mappare il numero massimo di fogli di lavoro che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Scaricare una cartella di lavoro]

Questo modulo di azione scarica il contenuto della cartella di lavoro di Excel specificata.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connetti l’app o il servizio web del modulo a [!DNL Workfront Fusion]</a> nell’articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Creare uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scarica una cartella di lavoro]</td> 
   <td> <p>Selezionare la modalità di identificazione della cartella di lavoro per il modulo da scaricare.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Immettendo manualmente un ID]</strong> </p> <p>Nel campo [!UICONTROL ID cartella di lavoro] immettere o mappare l'ID della cartella di lavoro specifica che si desidera scaricare dal modulo.</p> </li> 
     <li> <p><strong>[!UICONTROL Selezionando dal percorso]</strong> </p> <p>Nel campo [!UICONTROL Cartella di lavoro] selezionare la cartella di lavoro che si desidera scaricare nel modulo.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Foglio di lavoro

* [[!UICONTROL Visualizza righe foglio di lavoro]](#watch-worksheet-rows)
* [[!UICONTROL Elenco fogli di lavoro]](#list-worksheets)
* [[!UICONTROL Elenca righe foglio di lavoro]](#list-worksheet-rows)
* [[!UICONTROL Aggiungi un foglio di lavoro]](#add-a-worksheet)
* [[!UICONTROL Aggiungere una riga del foglio di lavoro]](#add-a-worksheet-row)
* [[!UICONTROL Aggiornare una riga del foglio di lavoro]](#update-a-worksheet-row)
* [[!UICONTROL Eliminare una riga del foglio di lavoro]](#delete-a-worksheet-row)

#### [!UICONTROL Visualizza righe foglio di lavoro]

Questo modulo di attivazione avvia uno scenario quando viene aggiunta una nuova riga al foglio.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connetti l’app o il servizio web del modulo a [!DNL Workfront Fusion]</a> nell’articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Creare uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL cartella di lavoro] </td>
   <td> <p>Selezionare la cartella di lavoro contenente il foglio di lavoro che si desidera controllare per le nuove righe.</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL Worksheet] </td>
   <td> <p>Selezionare il foglio di Excel da controllare per le nuove righe.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limit]</td>
   <td> <p>Immettere o mappare il numero massimo di righe del foglio di lavoro che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Elenco fogli di lavoro]

Questo modulo di azione recupera un elenco di fogli di lavoro nella cartella di lavoro specificata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connetti l’app o il servizio web del modulo a [!DNL Workfront Fusion]</a> nell’articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Creare uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL cartella di lavoro] </td>
   <td> <p>Selezionare la cartella di lavoro contenente i fogli di lavoro che si desidera elencare nel modulo.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limit]</td>
   <td> <p>Immettere o mappare il numero massimo di fogli di lavoro che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</p> </td> 
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
   <td> <p>Per istruzioni sulla connessione [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connetti l’app o il servizio web del modulo a [!DNL Workfront Fusion]</a> nell’articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Creare uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL cartella di lavoro] </td>
   <td> <p>Selezionare la cartella di lavoro contenente il foglio di lavoro che include le righe da elencare.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Worksheet] </td>
   <td> <p>Selezionare il foglio di lavoro contenente le righe da elencare.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limit]</td>
   <td> <p>Immettere o mappare il numero massimo di righe del foglio di lavoro che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggiungi un foglio di lavoro]

Questo modulo di azione crea un nuovo foglio di lavoro all’interno della cartella di lavoro selezionata.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connetti l’app o il servizio web del modulo a [!DNL Workfront Fusion]</a> nell’articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Creare uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL cartella di lavoro] </td>
   <td> <p>Selezionare la cartella di lavoro in cui si desidera aggiungere un foglio di lavoro.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Name] </td>
   <td> <p>Immettere o associare un nome per il nuovo foglio di lavoro.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggiungere una riga del foglio di lavoro]

Questo modulo di azione aggiunge una nuova riga al foglio di lavoro selezionato.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connetti l’app o il servizio web del modulo a [!DNL Workfront Fusion]</a> nell’articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Creare uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL cartella di lavoro] </td>
   <td> <p>Selezionare la cartella di lavoro contenente il foglio di lavoro in cui si desidera aggiungere una riga.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Worksheet] </td>
   <td> <p>Selezionare il foglio di lavoro in cui aggiungere una riga.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Tipo di valori immessi]</p> </td> 
   <td> <p>Selezionare il tipo di valore da immettere nel foglio di lavoro. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Formule]</strong> </p> <p> Excel tenta di valutare l'espressione specificata. I nomi delle funzioni in una formula sono in inglese. Esempio: <code>[!DNL =SUM(A1:A10)]</code></p> </li> 
     <li> <p><strong>[!UICONTROL Formulas local]</strong> </p> <p>Excel tenta di valutare l'espressione specificata. I nomi delle funzioni sono nella lingua dell'applicazione Excel. Esempio: <code>=SUM(A1, 1.5)</code> vs <code>=SUMME(A1; 1,5)</code></p> </li> 
     <li> <p><strong>Valore [!UICONTROL]</strong> </p> <p>Excel non valuta il valore. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Riga]</td>
    <td>Per ogni colonna, immettere il valore desiderato per la colonna nella nuova riga.</td>
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
   <td> <p>Per istruzioni sulla connessione [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connetti l’app o il servizio web del modulo a [!DNL Workfront Fusion]</a> nell’articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Creare uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL cartella di lavoro] </td>
   <td> <p>Selezionare la cartella di lavoro contenente il foglio di lavoro che include la riga che si desidera aggiornare.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Worksheet] </td>
   <td> <p>Selezionare il foglio di lavoro contenente la riga da aggiornare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Tipo di valori immessi]</p> </td> 
   <td> <p>Selezionare il tipo di valore da immettere nel foglio di lavoro. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Formule]</strong> </p> <p> Excel tenta di valutare l'espressione specificata. I nomi delle funzioni in una formula sono in inglese. Esempio: <code>[!DNL =SUM(A1:A10)]</code></p> </li> 
     <li> <p><strong>[!UICONTROL Formulas local]</strong> </p> <p>Excel tenta di valutare l'espressione specificata. I nomi delle funzioni sono nella lingua dell'applicazione Excel. Esempio: <code>=SUM(A1, 1.5)</code> vs <code>=SUMME(A1; 1,5)</code></p> </li> 
     <li> <p><strong>Valore [!UICONTROL]</strong> </p> <p>Excel non valuta il valore. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Row ID]</td> 
   <td>Seleziona il numero della riga da aggiornare.</td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Riga]</td>
    <td>Per ogni colonna, immettere il valore desiderato per la colonna nella nuova riga.</td>
   --&gt; 
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
   <td> <p>Per istruzioni sulla connessione [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connetti l’app o il servizio web del modulo a [!DNL Workfront Fusion]</a> nell’articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Creare uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL cartella di lavoro] </td>
   <td> <p>Selezionare la cartella di lavoro contenente il foglio di lavoro che include la riga che si desidera eliminare.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Worksheet]</td>
   <td> <p> Selezionare il foglio di lavoro contenente la riga che si desidera eliminare.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Row ID]</td>
   <td>Inserisci o mappa l’ID della riga da eliminare.</td> 
  </tr> 
 </tbody> 
</table>

### Tabella

* [[!UICONTROL Osserva righe tabella]](#watch-table-rows)
* [[!UICONTROL Tabelle elenco]](#list-tables)
* [[!UICONTROL Righe tabella elenco]](#list-table-rows)
* [[!UICONTROL Ottieni un tavolo]](#get-a-table)
* [[!UICONTROL Aggiungi una tabella]](#add-a-table)
* [[!UICONTROL Aggiungi una riga di tabella]](#add-a-table-row)
* [[!UICONTROL Aggiornare una tabella]](#update-a-table)
* [[!UICONTROL Eliminare una tabella]](#delete-a-table)

#### [!UICONTROL Osserva righe tabella]

Questo trigger avvia uno scenario quando viene aggiunta una nuova riga a una tabella.

>[!NOTE]
>
>La tabella qui fa riferimento all&#39;elemento tabella incorporato nella cartella di lavoro. Non l&#39;intera tabella (cartella/foglio).

![](assets/embedded-table-350x420.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connetti l’app o il servizio web del modulo a [!DNL Workfront Fusion]</a> nell’articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Creare uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL cartella di lavoro]</p> </td> 
   <td> <p>Selezionare la cartella di lavoro contenente la tabella che si desidera controllare.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Worksheet] </td>
   <td> <p> Selezionare il foglio di lavoro contenente la tabella che si desidera controllare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Tabella [!UICONTROL]</p> </td> 
   <td> <p>Selezionare la tabella che si desidera controllare.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limit]</td>
   <td> <p>Immettere o mappare il numero massimo di righe che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</p> </td> 
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
   <td> <p>Per istruzioni sulla connessione [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connetti l’app o il servizio web del modulo a [!DNL Workfront Fusion]</a> nell’articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Creare uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL cartella di lavoro] </td>
   <td> <p>Selezionare la cartella di lavoro contenente le tabelle da elencare.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Worksheet] </td>
   <td> <p>Selezionare il foglio di lavoro contenente le tabelle da elencare</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limit]</td>
   <td> <p>Immettere o mappare il numero massimo di tabelle che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Righe tabella elenco]

Questo modulo di ricerca recupera un elenco di tutte le righe di tabella in una cartella di lavoro.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connetti l’app o il servizio web del modulo a [!DNL Workfront Fusion]</a> nell’articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Creare uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL cartella di lavoro] </td>
   <td> <p>Selezionare la cartella di lavoro contenente la tabella che include le righe da elencare.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Worksheet] </td>
   <td> <p>Selezionare il foglio di lavoro contenente la tabella che include le righe da elencare</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >Tabella [!UICONTROL] </td>
   <td> <p>Selezionare la tabella contenente le righe da elencare.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limit]</td>
   <td> <p>Immettere o mappare il numero massimo di righe di tabella che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottieni un tavolo]

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
     <p>Per istruzioni sulla connessione dell'account Office 365 a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connetti l’app o il servizio web del modulo a [!DNL Workfront Fusion]</a> nell’articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Creare uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p>
    --&gt; </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Recupera una tabella]</td> 
   <td> <p>Selezionare la modalità di identificazione della tabella che si desidera recuperare.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Invio manuale]</strong> </p> <p>Nel campo [!UICONTROL ID cartella di lavoro] immettere o mappare l'ID della cartella di lavoro che contiene la tabella che si desidera recuperare.</p> <p>Nel campo [!UICONTROL Nome tabella] immettere o mappare il nome della tabella che si desidera recuperare.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleziona dall'elenco]</strong> </p> <p>Selezionare la cartella di lavoro e il foglio di lavoro contenenti la tabella che si desidera recuperare, quindi selezionare la tabella.</p> </li> 
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
   <td> <p>Per istruzioni sulla connessione [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connetti l’app o il servizio web del modulo a [!DNL Workfront Fusion]</a> nell’articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Creare uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL cartella di lavoro] </td> 
   <td> <p>Selezionare la cartella di lavoro contenente il foglio di lavoro in cui si desidera aggiungere una tabella.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Worksheet] </td> 
   <td> <p>Selezionare il foglio di lavoro in cui aggiungere una tabella.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ha Intestazioni]</td> 
   <td> <p>Abilita questa opzione per definire la prima riga come intestazioni di tabella.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Address]</p> </td> 
   <td> <p>Impostare le dimensioni della tabella indicando le celle in alto a sinistra e in basso a destra. Esempio: <code>A1:C10</code> crea una tabella con 3 colonne e 10 righe.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggiungi una riga di tabella]

Questo modulo modifica una tabella esistente.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connetti l’app o il servizio web del modulo a [!DNL Workfront Fusion]</a> nell’articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Creare uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL cartella di lavoro] </td>
   <td> <p>Selezionare la cartella di lavoro contenente la tabella in cui si desidera aggiungere una riga.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Worksheet] </td>
   <td> <p>Selezionare il foglio di lavoro contenente la tabella in cui si desidera aggiungere una riga.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >Tabella [!UICONTROL]</td>
   <td>Selezionare la tabella in cui si desidera aggiungere una riga.</td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL Riga]</td>
    <td>Per ogni colonna, immettere il valore desiderato per la colonna nella nuova riga.</td>
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Row ID]</p> </td> 
   <td> <p>Per aggiungere una riga in una posizione specifica della tabella, immettere o mappare un numero di riga. Il modulo inserisce la nuova riga dopo questa riga.</p> </td> 
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
   <td> <p>Per istruzioni sulla connessione [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connetti l’app o il servizio web del modulo a [!DNL Workfront Fusion]</a> nell’articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Creare uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Aggiorna una tabella]</td> 
   <td> <p>Selezionare la modalità di identificazione della tabella da aggiornare.</p> 
    <ul> 
     <li> <p><strong>Inserisci manualmente</strong> </p> <p>Nel campo [!UICONTROL ID cartella di lavoro] immettere o mappare l'ID della cartella di lavoro contenente la tabella che si desidera aggiornare.</p> <p>Nel campo [!UICONTROL Nome tabella] immettere o mappare il nome della tabella che si desidera aggiornare.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleziona dall'elenco]</strong> </p> <p>Selezionare la cartella di lavoro e il foglio di lavoro contenenti la tabella che si desidera aggiornare, quindi selezionare la tabella.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Tabella [!UICONTROL] </td> 
   <td> <p>Selezionare la tabella da aggiornare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name]</td> 
   <td> <p>Se si desidera rinominare la tabella, immettere o mappare un nuovo nome per la tabella.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mostra intestazioni]</td> 
   <td> <p>Abilita questa opzione per mostrare le intestazioni della tabella aggiornata.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mostra totali]</td> 
   <td>Abilita questa opzione per visualizzare i valori totali della tabella.</td> 
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
   <td> <p>Per istruzioni sulla connessione [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connetti l’app o il servizio web del modulo a [!DNL Workfront Fusion]</a> nell’articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Creare uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Recupera una tabella]</td> 
   <td> <p>Selezionare la modalità di identificazione della tabella da eliminare.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Invio manuale]</strong> </p> <p>Nel campo [!UICONTROL ID cartella di lavoro] immettere o mappare l'ID della cartella di lavoro che contiene la tabella da eliminare.</p> <p>Nel campo [!UICONTROL Nome tabella] immettere o mappare il nome della tabella che si desidera eliminare.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleziona dall'elenco]</strong> </p> <p>Selezionare la cartella di lavoro e il foglio di lavoro contenenti la tabella che si desidera eliminare, quindi selezionare la tabella.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Altro

* [[!UICONTROL Recuperare i dati]](#retrieve-data)
* [[!UICONTROL Effettuare una chiamata API]](#make-an-api-call)

#### [!UICONTROL Recuperare i dati]

Questa azione recupera i dati dall&#39;intervallo del foglio di lavoro definito e restituisce un bundle per ogni riga.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connetti l’app o il servizio web del modulo a [!DNL Workfront Fusion]</a> nell’articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Creare uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL cartella di lavoro] </td> 
   <td> <p>Selezionare la cartella di lavoro contenente i dati da recuperare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Worksheet] </td> 
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
   <td> <p>Per istruzioni sulla connessione [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connetti l’app o il servizio web del modulo a [!DNL Workfront Fusion]</a> nell’articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Creare uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Inserisci un percorso relativo a <code>https://graph.microsoft.com</code>. Esempio:<code> /v1.0/me/drive/root/children</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   td&gt; <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
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
   <td> <p>Aggiungi il contenuto body per la chiamata API sotto forma di oggetto JSON standard.</p> <p>Nota:   <p>Quando si utilizzano istruzioni condizionali quali <code>if</code> nel JSON, inserisci le virgolette al di fuori dell’istruzione condizionale.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>
