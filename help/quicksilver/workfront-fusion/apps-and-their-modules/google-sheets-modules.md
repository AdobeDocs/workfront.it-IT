---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli Google Sheets
description: Per utilizzare [!DNL Google Sheets] con [!DNL Adobe Workfront Fusion],you need the [!UICONTROL Workfront Fusion Google Sheets] estensione (facoltativa, ma necessaria per i trigger istantanei).
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 11d62222-df34-472d-93d7-f0d53eb95c9b
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '3942'
ht-degree: 0%

---

# [!DNL Google Sheets] moduli

In un [!DNL Adobe Workfront Fusion] scenario, puoi automatizzare i flussi di lavoro che utilizzano [!DNL Google Sheets], oltre a collegarlo a più applicazioni e servizi di terze parti.

Per istruzioni sulla connessione [!DNL Google Sheets] account a [!DNL Workfront Fusion], vedi [Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base](../../workfront-fusion/connections/connect-to-fusion-general.md)

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

Da utilizzare [!UICONTROL Fogli Google] moduli, è necessario disporre di un [!UICONTROL Google] account.

## Triggers

### [!UICONTROL Righe di controllo]

Recupera i valori da ogni riga appena aggiunta nel foglio di calcolo.

Il modulo recupera solo le nuove righe che non sono state compilate in precedenza. Il trigger non elaborerà una riga sovrascritta.

>[!IMPORTANT]
>
>Se il foglio di lavoro contiene una riga vuota, non verrà elaborata alcuna riga dopo la riga vuota.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Google Sheets] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connetti l’app o il servizio web del modulo a [!DNL Workfront Fusion]</a> nell’articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Creare uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Foglio di calcolo di [!UICONTROL] </td> 
   <td> <p>Selezionare il foglio di calcolo contenente il foglio che si desidera controllare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Foglio] </td> 
   <td> <p>Selezionare il foglio da controllare per una nuova riga.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL La tabella contiene intestazioni]</td> 
   <td> <p> Selezionare se il foglio di calcolo contiene la riga di intestazione.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Sì]</strong> </p> <p>Il modulo non recupera la riga di intestazione come dati di output. </p> <p>I nomi delle variabili nell’output vengono richiamati dalle intestazioni.</p> </li> 
     <li> <p><strong>[!UICONTROL No]</strong> </p> <p>Il modulo recupera anche la prima riga della tabella</p> <p>I nomi delle variabili nell'output sono denominati A, B, C, D e così via.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Riga con intestazioni] </td> 
   <td> <p>Immettere l'intervallo della riga di intestazione. Ad esempio, <code>A1:F1</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Prima riga tabella]</td> 
   <td> <p>Immettere l'intervallo della prima riga della tabella. Ad esempio, <code>A1:F1</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Opzione di rendering del valore [!UICONTROL]</p> </td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Valore formattato]</p> <p>I valori verranno calcolati e formattati nella risposta in base alla formattazione della cella. La formattazione si basa sulle impostazioni locali del foglio di calcolo, non sulle impostazioni locali dell'utente richiedente. Ad esempio, se <code>A1</code> è <code>1.23</code> e <code>A2</code> è <code>=A1</code> e formattato come valuta, quindi <code>A2</code> restituirebbe <code>"$1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL Valore non formattato]</p> <p>I valori verranno calcolati, ma non formattati nella risposta. Ad esempio, se <code>A1</code> è <code>1.23</code> e <code>A2</code> è <code>=A1</code> e formattato come valuta, quindi <code>A2</code> restituirebbe il numero <code>"1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL Formula]</p> <p>I valori non verranno calcolati. La risposta includerà le formule. Ad esempio, se <code>A1</code> è <code>1.23</code> e <code>A2</code> è <code>=A1</code> e formattato come valuta, quindi <code>A2</code> restituirebbe <code>"=A1"</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Data e ora opzione di rendering]</p> </td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Numero di serie]</p> <p>Indica che i campi di data, ora, dataora e durata devono essere generati come duplicati in formato "numero seriale", come reso popolare da Lotus 1-2-3. La porzione del numero intero del valore (a sinistra del decimale) conta i giorni dal 30 dicembre 1899. La parte frazionaria (a destra del decimale) conta l’ora come frazione del giorno. Ad esempio, il 1 gennaio 1900 a mezzogiorno sarebbe 2,5, 2 perché sono 2 giorni dopo il 30 dicembre 1899, e 0,5 perché mezzogiorno è mezza giornata. Il primo febbraio 1900 alle 15:00 sarebbe il 33.625. Questo considera correttamente l'anno 1900 come non un anno bisestile.</p> <p style="font-weight: bold;">[!UICONTROL Stringa formattata]</p> <p>Indica che i campi di data, ora, dataora e durata devono essere generati come stringhe nel formato numero specificato (che dipende dalle impostazioni internazionali del foglio di calcolo).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Imposta il numero massimo di risultati che [!DNL Workfront Fusion] funzionerà con durante un ciclo di esecuzione.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Azioni

* [[!UICONTROL Aggiungi una riga]](#add-a-row)
* [[!UICONTROL Aggiornare una riga]](#update-a-row)
* [[!UICONTROL Cancella riga]](#clear-a-row)
* [[!UICONTROL Eliminare una riga]](#delete-a-row)
* [[!UICONTROL Ottieni una cella]](#get-a-cell)
* [[!UICONTROL Aggiornare una cella]](#update-a-cell)
* [[!UICONTROL Cancella cella]](#clear-a-cell)
* [[!UICONTROL Aggiungi un foglio]](#add-a-sheet)
* [[!UICONTROL Creare un foglio di calcolo]](#create-a-spreadsheet)
* [[!UICONTROL Eliminare un foglio]](#delete-a-sheet)
* [[!UICONTROL Effettuare una chiamata API]](#make-an-api-call)

### [!UICONTROL Aggiungi una riga]

Questo modulo aggiunge una riga a un foglio.

Quando si configura [!DNL Google Sheets] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL Google Sheets] I campi potrebbero essere visualizzati in base a fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se viene visualizzato il pulsante Mappa sopra un campo o una funzione, è possibile utilizzarlo per impostare variabili e funzioni per tale campo. Per ulteriori informazioni, consulta [Mappare le informazioni da un modulo all’altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Google Sheets] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connetti l’app o il servizio web del modulo a [!DNL Workfront Fusion]</a> nell’articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Creare uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Mode]</td> 
   <td> <p>Specificare se si desidera selezionare il foglio di calcolo e il foglio manualmente o mediante mapping.</p> <p>Nota: la mappatura manuale è utile, ad esempio, quando si crea un nuovo foglio di calcolo in un [!DNL Workfront Fusion] e desideri aggiungere i dati nel nuovo foglio di calcolo direttamente nello scenario.</p> </td> 
  </tr> 
  <tr> 
   <td>Foglio di calcolo di [!UICONTROL] </td> 
   <td> <p>Seleziona la [!DNL Google] foglio di calcolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Foglio] </td> 
   <td> <p>Selezionare il foglio a cui si desidera aggiungere una riga.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Intervallo colonne]</td> 
   <td>Selezionare l'intervallo di colonne che si desidera utilizzare.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL La tabella contiene intestazioni]</td> 
   <td> <p> Selezionare se il foglio di calcolo contiene la riga di intestazione.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Sì]</strong> </p> <p>Il modulo non recupera la riga di intestazione come dati di output. </p> <p>I nomi delle variabili nell’output vengono richiamati dalle intestazioni.</p> </li> 
     <li> <p><strong>[!UICONTROL No]</strong> </p> <p>Il modulo recupera anche la prima riga della tabella</p> <p>I nomi delle variabili nell'output sono denominati A, B, C, D e così via.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Values] </td> 
   <td> <p>Immetti o mappa le celle desiderate della riga da aggiungere.</p> </td> 
  </tr> 
  <tr> 
   <td>Opzione di input del valore [!UICONTROL]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL User entered]</strong></p> <p>I valori vengono analizzati come se l’utente li avesse digitati nell’interfaccia utente. I numeri rimangono numeri, ma le stringhe possono essere convertite in numeri, date o altri formati seguendo le stesse regole applicate quando si immette testo in una cella tramite [!DNL Google Sheets] UI.</p> </li> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p> I valori immessi dall’utente non vengono analizzati e vengono memorizzati così come sono. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Inserisci dati, opzione]</td> 
   <td> <p>Specifica come vengono modificati i dati esistenti quando vengono immessi nuovi dati. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Inserisci righe]</strong></p> <p>Le righe vengono inserite per i nuovi dati.</p> </li> 
     <li> <p><strong>[!UICONTROL Overwrite]</strong> </p> <p>I nuovi dati sovrascrivono quelli esistenti nelle aree in cui vengono scritti. L'aggiunta di dati alla fine del foglio consente di inserire nuove righe o colonne in modo da poter scrivere i dati.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Aggiornare una riga]

Questo modulo consente di modificare il contenuto della cella in una riga selezionata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Google Sheets] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connetti l’app o il servizio web del modulo a [!DNL Workfront Fusion]</a> nell’articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Creare uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Mode]</td> 
   <td> <p>Specificare se si desidera selezionare il foglio di calcolo e il foglio manualmente o mediante mapping.</p> <p>Nota: la mappatura manuale è utile, ad esempio, quando si crea un nuovo foglio di calcolo nello scenario [!UICONTROL Workfront Fusion] e si desidera aggiungere dati al nuovo foglio di calcolo direttamente nello scenario.</p> </td> 
  </tr> 
  <tr> 
   <td>Foglio di calcolo di [!UICONTROL] </td> 
   <td> <p>Seleziona la [!DNL Google] foglio di calcolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Foglio] </td> 
   <td> <p>Selezionare il foglio in cui si desidera aggiornare una riga.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Numero riga]</td> 
   <td> <p> Immettere il numero della riga da aggiornare.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL La tabella contiene intestazioni]</td> 
   <td> <p> Selezionare se il foglio di calcolo contiene la riga di intestazione.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Sì]</strong> </p> <p>Il modulo non recupera la riga di intestazione come dati di output. </p> <p>I nomi delle variabili nell’output vengono richiamati dalle intestazioni.</p> </li> 
     <li> <p><strong>[!UICONTROL No]</strong> </p> <p>Il modulo recupera anche la prima riga della tabella</p> <p>I nomi delle variabili nell'output sono denominati A, B, C, D e così via.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Values] </td> 
   <td> <p>Immettere o mappare i valori alle celle desiderate della riga che si desidera modificare (aggiornare).</p> </td> 
  </tr> 
  <tr> 
   <td>Opzione di input del valore [!UICONTROL]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL User entered]</strong></p> <p>I valori vengono analizzati come se l’utente li avesse digitati nell’interfaccia utente. I numeri rimangono numeri, ma le stringhe possono essere convertite in numeri, date o altri formati seguendo le stesse regole applicate quando si immette testo in una cella tramite [!DNL Google Sheets] UI.</p> </li> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p> I valori immessi dall’utente non vengono analizzati e vengono memorizzati così come sono. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Cancella riga]

Elimina i valori da una riga specificata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Google Sheets] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connetti l’app o il servizio web del modulo a [!DNL Workfront Fusion]</a> nell’articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Creare uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Foglio di calcolo di [!UICONTROL] </td> 
   <td> <p>Seleziona la [!DNL Google] foglio di calcolo contenente il foglio da cui si desidera cancellare una riga.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Foglio] </td> 
   <td> <p> Selezionare il foglio da cui si desidera cancellare i dati.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Numero riga]</td> 
   <td> <p>Immettere il numero della riga da cui si desidera cancellare i dati. Ad esempio, <code> 23</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Eliminare una riga]

Elimina una riga specificata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Google Sheets] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connetti l’app o il servizio web del modulo a [!DNL Workfront Fusion]</a> nell’articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Creare uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Foglio di calcolo di [!UICONTROL] </td> 
   <td> <p>Selezionare il foglio di calcolo di Google contenente il foglio da cui si desidera eliminare una riga.</p> </td> 
  </tr> 
  <tr> 
   <td>Foglio </td> 
   <td> <p>Selezionare il foglio da cui si desidera eliminare una riga.</p> </td> 
  </tr> 
  <tr> 
   <td>Numero riga</td> 
   <td> <p>Immettere il numero della riga che si desidera eliminare. Esempio: <code>23</code></p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Ottieni una cella]

Recupera un valore da una cella selezionata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Google Sheets] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connetti l’app o il servizio web del modulo a [!DNL Workfront Fusion]</a> nell’articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Creare uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Foglio di calcolo di [!UICONTROL] </td> 
   <td> <p>Seleziona la [!DNL Google] foglio di calcolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Foglio] </td> 
   <td> <p>Selezionare il foglio contenente la cella da cui si desidera recuperare i dati.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cella] </td> 
   <td> <p>Immettere l'ID della cella da cui si desidera recuperare i dati. Esempio: <code>A6</code></p> </td> 
  </tr> 
  <tr> 
   <td>Opzione di rendering del valore [!UICONTROL]</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Valore formattato]</p> <p>I valori verranno calcolati e formattati nella risposta in base alla formattazione della cella. La formattazione si basa sulle impostazioni locali del foglio di calcolo, non sulle impostazioni locali dell'utente richiedente. Ad esempio, se <code>A1</code> è <code>1.23</code> e <code>A2</code> è <code>=A1</code> e formattato come valuta, quindi <code>A2</code> restituirebbe <code>"$1.23"</code>.</p> <p style="font-weight: bold;">[!DNL Unformatted value]</p> <p>I valori verranno calcolati, ma non formattati nella risposta. Ad esempio, se <code>A1</code> è <code>1.23</code> e <code>A2</code> è <code>=A1</code> e formattato come valuta, quindi <code>A2</code> restituirebbe il numero <code>"1.23"</code>.</p> <p style="font-weight: bold;">[!DNL Formula]</p> <p>I valori non verranno calcolati. La risposta includerà le formule. Ad esempio, se <code>A1</code> è <code>1.23</code> e <code>A2</code> è <code>=A1</code> e formattato come valuta, quindi <code>A2</code> restituirebbe <code>"=A1"</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Date and time render option]</td> 
   <td> <p style="font-weight: bold;">[!DNL Serial number]</p> <p>Indica che i campi di data, ora, dataora e durata devono essere generati come duplicati in formato "numero seriale", come reso popolare da Lotus 1-2-3. La porzione del numero intero del valore (a sinistra del decimale) conta i giorni dal 30 dicembre 1899. La parte frazionaria (a destra del decimale) conta l’ora come frazione del giorno. Ad esempio, il 1 gennaio 1900 a mezzogiorno sarebbe 2,5, 2 perché sono 2 giorni dopo il 30 dicembre 1899, e 0,5 perché mezzogiorno è mezza giornata. Il primo febbraio 1900 alle 15:00 sarebbe il 33.625. Questo considera correttamente l'anno 1900 come non un anno bisestile.</p> <p style="font-weight: bold;">[!DNL Formatted string]</p> <p>Indica che i campi di data, ora, dataora e durata devono essere generati come stringhe nel formato numero specificato (che dipende dalle impostazioni internazionali del foglio di calcolo).</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Aggiornare una cella]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Google Sheets] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connetti l’app o il servizio web del modulo a [!DNL Workfront Fusion]</a> nell’articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Creare uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Foglio di calcolo di [!UICONTROL] </td> 
   <td> <p>Seleziona la [!DNL Google] foglio di calcolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cella] </td> 
   <td> <p>Immettere l'ID della cella da aggiornare. Esempio: <code>A5</code></p> </td> 
  </tr> 
  <tr> 
   <td>Valore [!UICONTROL]</td> 
   <td> <p>Immettere il nuovo valore per la cella.</p> </td> 
  </tr> 
  <tr> 
   <td>Opzione di input del valore [!UICONTROL]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL User entered]</strong></p> <p>I valori vengono analizzati come se l’utente li avesse digitati nell’interfaccia utente. I numeri rimangono numeri, ma le stringhe possono essere convertite in numeri, date o altri formati seguendo le stesse regole applicate quando si immette testo in una cella tramite [!DNL Google Sheets] UI.</p> </li> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p> I valori immessi dall’utente non vengono analizzati e vengono memorizzati così come sono. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Cancella cella]

Elimina un valore da una cella specificata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Google Sheets] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connetti l’app o il servizio web del modulo a [!DNL Workfront Fusion]</a> nell’articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Creare uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Foglio di calcolo di [!UICONTROL] </td> 
   <td> <p>Selezionare il foglio di calcolo di Google contenente il foglio da cui si desidera cancellare una cella.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Foglio] </td> 
   <td> <p>Selezionare il foglio da cui si desidera cancellare una cella.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cella] </td> 
   <td> <p>Immettere l'ID della cella che si desidera cancellare. Esempio: <code>A5</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Aggiungi un foglio]

Crea un nuovo foglio in un foglio di calcolo selezionato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Google Sheets] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connetti l’app o il servizio web del modulo a [!DNL Workfront Fusion]</a> nell’articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Creare uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Foglio di calcolo di [!UICONTROL] </td> 
   <td> <p>Selezionare il foglio di calcolo Google in cui si desidera aggiungere un foglio.</p> </td> 
  </tr> 
  <tr> 
   <td>Proprietà [!UICONTROL]</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">[!UICONTROL Title]</p> <p>Immettere il nome del nuovo foglio.</p> </li> 
     <li> <p style="font-weight: bold;">[!UICONTROL Index]</p> <p>Immettere la posizione del foglio. Il valore di default è 0 (posiziona il foglio al primo posto)</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Creare un foglio di calcolo]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Google Sheets] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connetti l’app o il servizio web del modulo a [!DNL Workfront Fusion]</a> nell’articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Creare uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Title] </td> 
   <td> <p>Immettere il nome di un nuovo foglio di calcolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Locale]</td> 
   <td> <p>Immettere le impostazioni locali del foglio di calcolo in uno dei seguenti formati:</p> 
    <ul> 
     <li>un codice lingua ISO 639-1 come <code>en</code></li> 
     <li>un codice lingua ISO 639-2 come <code>haw</code>, se non esiste il codice 639-1</li> 
     <li>una combinazione del codice della lingua ISO e del codice del paese, come <code>en_US</code></li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Intervallo di ricalcolo]</td> 
   <td> <p>Quantità di tempo di attesa prima del ricalcolo delle funzioni volatili:</p> <p style="font-weight: bold;">[!UICONTROL in caso di modifica]</p> <p>Le funzioni volatili vengono aggiornate a ogni modifica.</p> <p style="font-weight: bold;">[!UICONTROL su modifica e ogni minuto]</p> <p>Le funzioni volatili vengono aggiornate a ogni cambiamento e ogni minuto.</p> <p style="font-weight: bold;">[!UICONTROL su modifica e su base oraria]</p> <p>Le funzioni volatili vengono aggiornate a ogni modifica e ogni ora.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fuso orario]</td> 
   <td> <p> Seleziona il fuso orario del foglio di calcolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Formato numero]</td> 
   <td> <p>Selezionare il formato predefinito di tutte le celle del foglio di calcolo.</p> <p><strong>[!UICONTROL Text]</strong>: formattazione del testo. Esempio: <code>1000. 12</code></p> <p><strong>[!UICONTROL Number]</strong>: formattazione dei numeri. Esempio: <code>1,000.12</code></p> <p><strong>[!UICONTROL Percent]</strong>: formattazione percentuale. Esempio: <code>10. 12%</code></p> <p><strong>[!UICONTROL Valuta]</strong>: formattazione della valuta. Esempio: <code>$1,000.12</code></p> <p><strong>[!UICONTROL Date]</strong>: formattazione della data. Esempio: <code>9/26/2008</code></p> <p><strong>[!UICONTROL Time]</strong>: formattazione del tempo. Esempio: <code>3:59:00 PM</code></p> <p><strong>[!UICONTROL Data e ora]</strong>: formattazione di data e ora. Esempio: <code>9/26/08 15:59:00</code> </p> <p><strong>[!UICONTROL Scientifico]</strong>Formattazione scientifica dei numeri. Esempio: <code>1. 01E+03</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fogli] </td> 
   <td> <p>Clic <strong>[!UICONTROL Add]</strong> per aggiungere un foglio al foglio di calcolo. Per ogni foglio, immettere o mappare un titolo per il foglio e l'indice del foglio. Un indice pari a 0 rappresenta il primo foglio.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Eliminare un foglio]

Elimina un foglio specifico.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Google Sheets] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connetti l’app o il servizio web del modulo a [!DNL Workfront Fusion]</a> nell’articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Creare uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Foglio di calcolo di [!UICONTROL] </td> 
   <td> <p>Seleziona la [!DNL Google] foglio di calcolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Foglio] </td> 
   <td> <p>Selezionare il foglio che si desidera eliminare.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Effettuare una chiamata API]

Questo modulo di azione ti consente di eseguire una chiamata API personalizzata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione dell'account [Fusion App] a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td>Inserisci un percorso relativo a <code>https://sheets.googleapis.com/v4/</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Method]</p> </td> 
   <td> <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Aggiungi le intestazioni della richiesta sotto forma di oggetto JSON standard. Ad esempio, <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] aggiunge le intestazioni di autorizzazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Stringa Di Query]</td> 
   <td> <p> Aggiungi la query per la chiamata API sotto forma di oggetto JSON standard.</p> </td> 
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

## Ricerche

* [[!UICONTROL Cerca righe]](#search-rows)
* [[!UICONTROL Cerca righe (Avanzate)]](#search-rows-advanced)
* [[!UICONTROL Ottieni valori intervallo]](#get-range-values)
* [[!UICONTROL Elenca fogli]](#list-sheets)

### [!UICONTROL Cerca righe]

Cerca le righe utilizzando le opzioni di filtro.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione dell'account [Fusion App] a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td>Foglio di calcolo di [!UICONTROL] </td> 
   <td> <p>Seleziona la [!DNL Google] foglio di calcolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Foglio] </td> 
   <td> <p>Seleziona il foglio in cui desideri cercare le righe.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL La tabella contiene intestazioni]</td> 
   <td> <p> Selezionare se il foglio di calcolo contiene la riga di intestazione. Se è selezionata l'opzione [!UICONTROL Yes], il modulo non recupera la riga di intestazione in quanto i dati di output e i nomi delle variabili nell'output vengono quindi richiamati dalle intestazioni. Se è selezionata l'opzione [!UICONTROL No], il modulo recupera anche la prima riga della tabella e i nomi delle variabili nell'output vengono quindi chiamati solo A, B, C, D e così via.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Intervallo colonne]</td> 
   <td>Seleziona l’intervallo di colonne su cui lavorare. Esempio: <code>A-F</code></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Filtro]</td> 
   <td> <p>Impostare il filtro per la riga in base alla quale eseguire la ricerca.</p> <p>Per ulteriori informazioni sui filtri, consulta <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">Aggiungere un filtro a uno scenario in [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Ordinamento [!UICONTROL]</td> 
   <td>Seleziona se desideri ordinare in modo crescente o decrescente.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordina per]</td> 
   <td>Scegliere la colonna in base alla quale si desidera eseguire l'ordinamento.</td> 
  </tr> 
  <tr> 
   <td>Opzione di rendering del valore [!UICONTROL]</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Valore formattato]</p> <p>I valori verranno calcolati e formattati nella risposta in base alla formattazione della cella. La formattazione si basa sulle impostazioni locali del foglio di calcolo, non sulle impostazioni locali dell'utente richiedente. Ad esempio, se <code>A1</code> è <code>1.23</code> e <code>A2</code> è <code>=A1</code> e formattato come valuta, quindi <code>A2</code> restituirebbe <code>"$1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL Valore non formattato]</p> <p>I valori verranno calcolati, ma non formattati nella risposta. Ad esempio, se <code>A1</code> è <code>1.23</code> e <code>A2</code> è <code>=A1</code> e formattato come valuta, quindi <code>A2</code> restituirebbe il numero <code>"1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL Formula]</p> <p>I valori non verranno calcolati. La risposta includerà le formule. Ad esempio, se <code>A1</code> è <code>1.23</code> e <code>A2</code> è <code>=A1</code> e formattato come valuta, quindi <code>A2</code> restituirebbe <code>"=A1"</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data e ora opzione di rendering]</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Numero di serie]</p> <p>Indica che i campi di data, ora, dataora e durata devono essere generati come duplicati in formato "numero seriale", come reso popolare da Lotus 1-2-3. La porzione del numero intero del valore (a sinistra del decimale) conta i giorni dal 30 dicembre 1899. La parte frazionaria (a destra del decimale) conta l’ora come frazione del giorno. Ad esempio, il 1 gennaio 1900 a mezzogiorno sarebbe 2,5, 2 perché sono 2 giorni dopo il 30 dicembre 1899, e 0,5 perché mezzogiorno è mezza giornata. Il primo febbraio 1900 alle 15:00 sarebbe il 33.625. Questo considera correttamente l'anno 1900 come non un anno bisestile.</p> <p style="font-weight: bold;">[!UICONTROL Stringa formattata]</p> <p>Indica che i campi di data, ora, dataora e durata devono essere generati come stringhe nel formato numero specificato (che dipende dalle impostazioni internazionali del foglio di calcolo).</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Numero massimo di righe restituite]</td> 
   <td>Imposta il numero massimo di righe che [!DNL Workfront Fusion] restituirà durante un ciclo di esecuzione.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Cerca righe (Avanzate)]

Restituisce risultati che corrispondono ai criteri specificati.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Google Sheets] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connetti l’app o il servizio web del modulo a [!DNL Workfront Fusion]</a> nell’articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Creare uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Foglio di calcolo di [!UICONTROL] </td> 
   <td> <p>Selezionare il foglio di calcolo di Google contenente il foglio che si desidera cercare.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Foglio] </td> 
   <td> <p>Selezionare il foglio contenente le righe che si desidera cercare.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Query]</td> 
   <td> <p>Utilizza il [!DNL Google Charts Query Language]. Esempio: <code>select * where B = "John"</code></p> <p>Per ulteriori informazioni su [!DNL Google Charts Query Language], vedi <a href="https://developers.google.com/chart/interactive/docs/querylanguage">Riferimento linguaggio di query</a> nel [!DNL Google] documentazione.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Ottieni valori intervallo]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Google Sheets] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connetti l’app o il servizio web del modulo a [!DNL Workfront Fusion]</a> nell’articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Creare uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Foglio di calcolo di [!UICONTROL] </td> 
   <td> <p>Seleziona la [!DNL Google] foglio di calcolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Foglio] </td> 
   <td> <p>Selezionare il foglio da cui si desidera ottenere il contenuto dell'intervallo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Range] </td> 
   <td> <p>Immettere l'intervallo che si desidera ottenere. Esempio: <code>A1:D25</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL La tabella contiene intestazioni]</td> 
   <td> <p>Selezionare questa casella se il foglio contiene una riga di intestazione</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Riga con intestazioni]</td> 
   <td>Immetti l’intervallo delle intestazioni della tabella. Esempio <code>A1:F1</code>. Se si lascia vuoto il campo, [!DNL Workfront Fusion] supponiamo che l’intestazione si trovi nella prima riga dell’intervallo specificato.</td> 
  </tr> 
  <tr> 
   <td>Opzione di rendering del valore [!UICONTROL]</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Valore formattato]</p> <p>I valori verranno calcolati e formattati nella risposta in base alla formattazione della cella. La formattazione si basa sulle impostazioni locali del foglio di calcolo, non sulle impostazioni locali dell'utente richiedente. Ad esempio, se <code>A1</code> è <code>1.23</code> e <code>A2</code> è <code>=A1</code> e formattato come valuta, quindi <code>A2</code> restituirebbe <code>"$1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL Valore non formattato]</p> <p>I valori verranno calcolati, ma non formattati nella risposta. Ad esempio, se <code>A1</code> è <code>1.23</code> e <code>A2</code> è <code>=A1</code> e formattato come valuta, quindi <code>A2</code> restituirebbe il numero <code>"1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL Formula]</p> <p>I valori non verranno calcolati. La risposta includerà le formule. Ad esempio, se <code>A1</code> è <code>1.23</code> e <code>A2</code> è <code>=A1</code> e formattato come valuta, quindi <code>A2</code> restituirebbe <code>"=A1"</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data e ora opzione di rendering]</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Numero di serie]</p> <p>Indica che i campi di data, ora, dataora e durata devono essere generati come duplicati in formato "numero seriale", come reso popolare da Lotus 1-2-3. La porzione del numero intero del valore (a sinistra del decimale) conta i giorni dal 30 dicembre 1899. La parte frazionaria (a destra del decimale) conta l’ora come frazione del giorno. Ad esempio, il 1 gennaio 1900 a mezzogiorno sarebbe 2,5, 2 perché sono 2 giorni dopo il 30 dicembre 1899, e 0,5 perché mezzogiorno è mezza giornata. Il primo febbraio 1900 alle 15:00 sarebbe il 33.625. Questo considera correttamente l'anno 1900 come non un anno bisestile.</p> <p style="font-weight: bold;">[!UICONTROL Stringa formattata]</p> <p>Indica che i campi di data, ora, dataora e durata devono essere generati come stringhe nel formato numero specificato (che dipende dalle impostazioni internazionali del foglio di calcolo).</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Elenca fogli]

Questo modulo restituisce un elenco di tutti i fogli di un foglio di calcolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Google Sheets] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connetti l’app o il servizio web del modulo a [!DNL Workfront Fusion]</a> nell’articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Creare uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Foglio di calcolo di [!UICONTROL] </td> 
   <td> <p>Seleziona la [!DNL Google] foglio di calcolo contenente i fogli che si desidera elencare.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Limiti di utilizzo

Se l’errore `429: RESOURCE_EXHAUSTED` si verifica, hai superato il limite di velocità API.

Il [!DNL Google Sheets] L’API ha un limite di 500 richieste per 100 secondi per progetto e di 100 richieste per 100 secondi per utente. I limiti per le letture e le scritture vengono tracciati separatamente. Non esiste alcun limite di utilizzo giornaliero.

Ulteriori dettagli sono disponibili all&#39;indirizzo [developers.google.com/sheets/api/limits](https://developers.google.com/sheets/api/limits).

## Suggerimenti

* [Come ottenere celle vuote da un [!DNL Google] Foglio](#how-to-get-empty-cells-from-a-google-sheet)
* [Aggiungere un pulsante in un foglio per eseguire uno scenario](#add-a-button-in-a-sheet-to-run-a-scenario)

### Come ottenere celle vuote da un [!DNL Google Sheet]

Utilizza il [!UICONTROL Cerca righe (Avanzate)] e utilizza questa formula per ottenere le colonne vuote.
<pre>seleziona * [!UICONTROL dove E è null​]</pre>Qui "E" è la colonna e "è nullo" è la condizione. È possibile creare una query più avanzata utilizzando [Google Query Lang.](https://developers.google.com/chart/interactive/docs/querylanguage)

### Aggiungere un pulsante in un foglio per eseguire uno scenario

1. In entrata [!DNL Workfront Fusion], inserire il **[!UICONTROL Webhook]** > **[!UICONTROL Webhook personalizzati]** modulo/trigger nello scenario e configurarlo (vedi [Webhook](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md)).

1. Copia l’URL del webhook.
1. Esegui lo scenario.
1. In Google Sheets, scegliere **[!UICONTROL Inserisci]** > **[!UICONTROL Disegno]**... dalla barra dei menu principale.

1. In [!UICONTROL Disegno] , fare clic sul pulsante **[!UICONTROL Casella di testo]** icona ![](assets/text-box.png) nella parte superiore della finestra.
1. Progettare un pulsante e fare clic su **[!UICONTROL Salva e chiudi]** nell’angolo in alto a destra:
1. Il pulsante verrà inserito nel foglio di lavoro. Fai clic sui tre punti verticali nell’angolo in alto a destra del pulsante:
1. Scegli **[!UICONTROL Assegna script..].** dal menu.
1. Immetti il nome dello script (funzione), ad esempio `runScenario` e fai clic su **[!UICONTROL OK]**:
1. Scegli **[!UICONTROL Strumenti]** > **[!UICONTROL Editor di script]** dalla barra dei menu principale.

1. Inserire il codice seguente:

   * Il nome della funzione deve corrispondere al nome specificato nel passaggio 9.
   * Sostituisci l’URL con l’URL del webhook copiato nel passaggio 2.

     <pre>function runScenario() {</pre><pre>UrlFetchApp.fetch("<webhook you copied>");</pre><pre>}</pre>

1. Premi **[!UICONTROL Ctrl+S]** per salvare il file script, immettete un nome di progetto e fate clic su **[!UICONTROL OK]**.

1. Torna a [!DNL Google Sheets] e fai clic sul nuovo pulsante.
1. Concedi l&#39;autorizzazione richiesta allo script:
1. In entrata [!DNL Workfront Fusion], verifica che lo scenario sia stato eseguito correttamente.

## Memorizzazione delle date in un foglio di calcolo

Se memorizzi un valore Data in un foglio di calcolo senza formattazione, questo verrà visualizzato nel foglio di calcolo come testo in formato ISO 8601. Tuttavia, [!DNL Google Sheets] formule o funzioni che utilizzano date che non comprendono questo testo (Esempio: formula `=A1+10`) visualizza il seguente errore:

![](assets/mceclip6-350x87.png)

Per consentire [!DNL Google Sheets] per comprendere la data, formattala con [[!UICONTROL formatDate] (data; formato; [fuso orario])](../../workfront-fusion/functions/date-and-time-functions.md#formatda) funzione. Il formato corretto passato alla funzione come secondo argomento dipende dalle impostazioni internazionali del foglio di calcolo.

Per determinare il formato corretto:

1. Scegli **[!UICONTROL File]** > **[!UICONTROL Foglio di calcolo]** dal menu principale per verificare/impostare le impostazioni internazionali.

1. Dopo aver verificato/impostato le impostazioni internazionali corrette, determinare il formato di data e ora corrispondente scegliendo **[!UICONTROL Formato]** > **[!UICONTROL Numero]** dal menu principale. Il formato viene visualizzato accanto alla voce di menu Data e ora:

1. Per comporre il formato corretto da passare al [!UICONTROL formatDate()] funzione, fare riferimento all&#39;elenco di [Token per la formattazione di data e ora in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md).

**Esempio:** L&#39;uso di `MM/DD/YYYY HH:mm:ss` formato per le impostazioni internazionali degli Stati Uniti:

![](assets/locale-time-350x83.png)

## Sfruttamento [!DNL Google Sheets] funzioni

Se salti una funzione incorporata, ma è caratterizzata da [!DNL Google Sheets], è possibile sfruttarlo. Per ulteriori informazioni, consulta [Utilizzare [!DNL Google Sheets] funzioni](../../workfront-fusion/functions/map-using-functions.md#exploiti) in [Mappare gli elementi utilizzando le funzioni in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/map-using-functions.md) .

## Mantieni [!DNL Google Sheets] da numeri a date

È possibile che una stringa di numeri utilizzata come testo venga interpretata come una data in un [!DNL Google] foglio di lavoro. Ad esempio, si digita 1-2019 con l&#39;intento di impostarlo come testo, ma Google lo interpreta come una data. È possibile preformattare il numero come testo normale per impedirlo.

1. In entrata [!DNL Google Sheets], evidenzia la colonna o la cella contenente il numero o i numeri.
1. Clic **[!UICONTROL Formato]** > **[!UICONTROL Numero]** > **[!UICONTROL Testo normale]**.

Un’altra soluzione alternativa in [!DNL Workfront Fusion] : per digitare un apostrofo (&#39;) prima di un numero, ad esempio &#39;1-2019 o &#39;1/47. L’apostrofo non viene visualizzato nella cella dopo l’invio dei dati da [!DNL Workfront Fusion].
