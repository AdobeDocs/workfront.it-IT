---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Moduli JSON
description: L’app JSON Adobe Workfront Fusion fornisce moduli per elaborare i dati in formato JSON in modo che Adobe Workfront Fusion possa lavorare ulteriormente con il contenuto dei dati o creare nuovi contenuti JSON.
author: Becky
feature: Workfront Fusion
exl-id: 60540608-9d2e-4e10-9fb2-5388dda64784
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1157'
ht-degree: 0%

---

# [!UICONTROL JSON] moduli

La [!DNL Adobe Workfront Fusion] [!UICONTROL JSON] l’app fornisce moduli per elaborare i dati in formato JSON in modo che [!DNL Adobe Workfront Fusion] può lavorare ulteriormente con il contenuto di dati o creare nuovo contenuto JSON.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p> <p>[!UICONTROL [!DNL Workfront Fusion] per automazione del lavoro </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</td> 
  </tr> 
 </tbody> 
</table>

Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, vedi [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Analizza JSON

* [Struttura dati](#data-structure)
* [Raccolta e array](#collection-vs-array)

### Struttura dati

La struttura dei dati descrive come sono organizzati i dati JSON e consente di mappare singoli elementi JSON ad altri moduli nel tuo scenario. Se non fornisci la struttura Dati, puoi eseguire manualmente il modulo e [!DNL Workfront Fusion] crea la struttura dal JSON fornito:

1. Aggiungi il [!UICONTROL Analizza JSON] in uno scenario.
1. In **[!UICONTROL Stringa JSON]** , immetti il JSON da cui desideri creare una struttura dati.
1. Non collegare altri moduli al [!UICONTROL Analizza JSON] modulo ancora. Perché [!DNL Workfront Fusion] non è ancora a conoscenza della struttura dei dati JSON, non è ancora possibile mappare i dati dal [!UICONTROL Analizza JSON] in altri moduli nel tuo scenario.
1. Esegui manualmente lo scenario. Ciò consente di [!UICONTROL Analizza JSON] modulo per identificare la struttura JSON dal JSON fornito.
1. È ora possibile collegare i seguenti moduli. Gli elementi del modulo Parse JSON sono ora disponibili per la mappatura.

Per ulteriori informazioni, consulta [Strutture dei dati in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-structures.md).

### Raccolta e array

Se il campo stringa JSON contiene una raccolta `{ ... }`, l’output è un singolo bundle contenente gli elementi della raccolta.

>[!INFO]
>
>**Esempio:**
>
>
```
>{
>       "name" : "Peter",
>
>    
   "ID" : 1
>}
>```
>
>![](assets/json-collection.png)

Se il campo stringa JSON contiene una matrice `[ ... ]`, l&#39;output è una serie di bundle. ogni bundle contiene un elemento dell&#39;array.

>[!INFO]
>
>**Esempio:**
>
>
```
>[
>   {
>       "name" : "Peter",
>       "ID" : 1
>   },
>
>  
 {
>       "name" : "Mike",
>       "ID" : 2
>   }
>]
>```
>
>![](assets/json-array.png)

## [!UICONTROL JSON] moduli e relativi campi

Quando si configura [!DNL JSON] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Insieme a questi, potrebbero essere visualizzati campi JSON aggiuntivi, a seconda di fattori come il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se trovi il pulsante mappa sopra un campo o una funzione, puoi utilizzarlo per impostare variabili e funzioni per quel campo. Per ulteriori informazioni, consulta [Mappare informazioni da un modulo a un altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Aggregazione in JSON](#aggregate-to-json)
* [Convertire JSON in XML](#convert-json-to-xml)
* [Analizza JSON](#parse-json)
* [Creare JSON](#create-json)
* [Trasforma JSON](#transform-json)

### [!UICONTROL Aggregazione in JSON]

Questo modulo aggregatore aggrega l’output di un modulo precedente in JSON.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Modulo di origine] </td> 
   <td> <p>Seleziona il modulo che genera i dati da aggregare a JSON.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data structure]</td> 
   <td> <p>Seleziona la struttura dati da utilizzare per creare JSON. La struttura dati determina quali altri campi sono disponibili in questo modulo. Per ulteriori informazioni, consulta <a href="#data-structure" class="MCXref xref">Struttura dati</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Rientro di [!UICONTROL]</td> 
   <td> <p> Seleziona se desideri applicare un rientro al JSON utilizzando schede, due spazi o quattro spazi.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Group by]</td> 
   <td>Definire un’espressione per la quale si desidera raggruppare l’output aggregato. Questa espressione può contenere uno o più elementi mappati. I dati aggregati vengono quindi separati in gruppi utilizzando il valore di questa espressione. Ogni gruppo produce come bundle separato con una chiave (l'espressione valutata) e un valore (il testo aggregato). Puoi utilizzare la chiave come filtro nei moduli successivi.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Interrompe l'elaborazione dopo un'aggregazione vuota]</td> 
   <td>Abilita questa opzione per interrompere lo scenario in assenza di risultati.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Convertire JSON in XML]

Questo modulo di azione converte una stringa JSON in XML.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL JSON string] </td> 
   <td> <p>Immetti o mappa il JSON da convertire in XML.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Analizza JSON]

Questo modulo di azione analizza una stringa JSON in una struttura di dati che ti consente di accedere ai dati all’interno della stringa JSON.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data structure]</td> 
   <td> <p>Seleziona la struttura dati da utilizzare per creare JSON. Per ulteriori informazioni, consulta <a href="#data-structure" class="MCXref xref">Struttura dati</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL JSON string] </td> 
   <td> <p>Immetti o mappa il JSON da analizzare.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Creare JSON]

Questo modulo di azione crea JSON da una struttura dati.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">Struttura dati</td> 
   <td> <p>Seleziona la struttura dati da utilizzare per creare JSON. Per ulteriori informazioni, consulta <a href="#data-structure" class="MCXref xref">Struttura dati</a> in questo articolo.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Trasforma JSON]

Questo modulo di azione trasforma un oggetto in una stringa json.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Object]</td> 
   <td> <p>Immetti o mappa l’oggetto da trasformare in JSON.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Trasformazione dei record di dati in JSON

>[!INFO]
>
>**Esempio:** L’esempio seguente mostra come trasformare i record di dati da [!DNL Google Sheets] in formato JSON:
>
>1. Posiziona il [!DNL Google Sheets] > [!UICONTROL Seleziona righe] nel tuo scenario per recuperare i dati. Imposta il modulo per recuperare le righe dal [!DNL Google] foglio di calcolo. Imposta il &#x200B;**[!UICONTROL Numero massimo di righe restituite]** a un numero ridotto, ma maggiore di uno a scopo di test (esempio, tre). Esegui il [!DNL Google Sheets] modulo facendo clic con il pulsante destro del mouse e scegliendo &quot;**[!UICONTROL Esegui solo questo modulo]**.&quot; Verifica l’output del modulo.
1. Collega [!UICONTROL Aggregatore array] modulo dopo [!DNL Google Sheets] modulo . Nella configurazione del modulo, scegli la [!DNL Google Sheets] nel modulo **[!UICONTROL Nodo di origine]** campo . Lascia gli altri campi così come sono per il momento.
1. Connetti [!UICONTROL JSON] > [!UICONTROL Creare JSON] modulo dopo [!UICONTROL Aggregatore array] modulo . La configurazione del modulo richiede una struttura dati che descrive il formato JSON. Fai clic su **[!UICONTROL Aggiungi]** per aprire la configurazione della struttura dati. Il modo più semplice per creare questa struttura dati è generarla automaticamente da un campione JSON. Fai clic su **[!UICONTROL Generatore]** e incolla il tuo campione JSON in **[!UICONTROL Dati di esempio]** campo:

   **Esempio:**
   ```
   {
   
   "books": [
   
   {
   
   "id": "ID",
   
   "title": "Title",
   
   "author": "Author"
   
   }
   
   ]
   
   }
   ```
1. Fai clic su **[!UICONTROL Salva]**. La [!UICONTROL Specifica] Il campo nella struttura dati contiene ora la struttura generata.
1. Modifica il nome della struttura dati in modo che sia più specifico e fai clic su **[!UICONTROL Salva]**. Un campo corrispondente all’attributo dell’array principale viene visualizzato come campo mappabile nella configurazione del modulo JSON.
1. Fai clic sul pulsante **[!UICONTROL Mappa]** accanto al campo e mappa il `Array[]` dall&#39;output dell&#39;aggregatore Array.
1. Fai clic su **[!UICONTROL OK]** per chiudere [!UICONTROL JSON] configurazione del modulo.
1. Apri la configurazione del [!UICONTROL Aggregatore array] modulo . Modificare la **[!UICONTROL Struttura di Target]** da [!UICONTROL Personalizzato] al [!UICONTROL JSON] campo del modulo corrispondente all’attributo della matrice radice. Mappare elementi dal [!DNL Google Sheets] ai campi appropriati.
1. Fai clic su **[!UICONTROL OK]** per chiudere [!UICONTROL Aggregatore array] configurazione del modulo.
1. Esegui lo scenario.
   La [!UICONTROL JSON] il modulo genera il formato JSON corretto.
1. Apri la configurazione del [!DNL Google Sheets] e aumentare il [!UICONTROL Numero massimo di righe restituite] deve essere maggiore del numero di righe nel foglio di calcolo per elaborare tutti i dati.


## Risoluzione dei problemi

### Impossibile mappare dati da [!UICONTROL Analizza JSON] modulo

Assicurati che il contenuto JSON sia correttamente mappato nel [!UICONTROL Analizza JSON] e che la struttura dati sia definita correttamente. Per ulteriori informazioni, consulta [Trasformazione dei record di dati in JSON](#transforming-data-records-to-json) in questo articolo.

### Il modulo non riesce quando si utilizzano istruzioni condizionali in JSON

Quando si utilizzano istruzioni condizionali come `if` nel JSON, inserisci le virgolette al di fuori dell’istruzione condizionale.

>[!INFO]
**Esempio:**
![](assets/quotes-in-json-350x120.png)
