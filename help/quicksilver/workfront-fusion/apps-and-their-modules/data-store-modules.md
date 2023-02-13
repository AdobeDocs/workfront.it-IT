---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Moduli di archiviazione dati
description: Un [!DNL Adobe Workfront Fusion] l’archivio dati, simile a un database o a una tabella semplice, può memorizzare dati da scenari, consentendo il trasferimento di dati tra scenari o esecuzioni di scenari individuali. È possibile utilizzare un archivio dati per memorizzare i nuovi dati provenienti da diversi sistemi durante la sincronizzazione.
author: Becky
feature: Workfront Fusion
exl-id: 1dc9cb88-d1b9-4a67-91fb-be980cc1ccd1
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1103'
ht-degree: 0%

---

# [!UICONTROL Archiviazione dati] moduli

Un [!DNL Adobe Workfront Fusion] l’archivio dati, simile a un database o a una tabella semplice, può memorizzare dati da scenari, consentendo il trasferimento di dati tra scenari o esecuzioni di scenari individuali. È possibile utilizzare un archivio dati per memorizzare i nuovi dati provenienti da diversi sistemi durante la sincronizzazione.

I moduli di archiviazione dati consentono di aggiungere, sostituire, aggiornare, recuperare, eliminare, cercare o contare record nel [!DNL Adobe Workfront Fusion] archivio dati.

Per informazioni sulla creazione, la modifica e la risoluzione dei problemi relativi agli archivi dati, consulta [Archivia dati in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p>  <p>[!UICONTROL [!DNL Workfront Fusion] per automazione del lavoro</p></td> 
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

Per utilizzare [!UICONTROL Archiviazione dati] moduli, devi prima creare un archivio dati.

Per informazioni sulla creazione di archivi dati, consulta [Archivia dati in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

## [!UICONTROL Archiviazione dati] moduli e relativi campi

Quando configuri moduli Data Store, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Insieme a questi, potrebbero essere visualizzati campi archivio dati aggiuntivi, a seconda di fattori come il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se trovi il pulsante mappa sopra un campo o una funzione, puoi utilizzarlo per impostare variabili e funzioni per quel campo. Per ulteriori informazioni, consulta [Mappare informazioni da un modulo a un altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

Tutto [!UICONTROL Archiviazione dati] I moduli sono moduli di tipo Azione.

* [Aggiungi/sostituisci un record](#addreplace-a-record)
* [Aggiornare un record](#update-a-record)
* [Ottieni un record](#get-a-record)
* [Controllare l&#39;esistenza di un record](#check-the-existence-of-a-record)
* [Eliminare un record](#delete-a-record)
* [Elimina tutti i record](#delete-all-records)
* [Cerca record](#search-records)
* [Record di conteggio](#count-records)

### [!UICONTROL Aggiungi/sostituisci un record]

Questo modulo di azione aggiunge o sostituisce un record.

Specificare l&#39;archivio dati e la chiave del record.

Il modulo restituisce l’ID del record e di tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

>[!NOTE]
>
>Il modulo genera un errore quando si tenta di aggiungere il record già presente nell&#39;archivio dati con lo stesso nome e il [!UICONTROL Sovrascrivi un record esistente] è disabilitata.

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Archivio dati]</td> 
   <td> <p> Selezionare o aggiungere l'archivio dati in cui si desidera creare un record. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Key] </td> 
   <td> <p>Immettere la chiave univoca del record che si desidera aggiungere o sostituire nel modulo. La chiave può essere utilizzata in un secondo momento per recuperare il record. Se lasci vuoto questo campo, viene generata automaticamente una chiave.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sovrascrivi un record esistente] </td> 
   <td> <p>Abilita questa opzione per sovrascrivere il record. Il record che si desidera sovrascrivere deve essere specificato nel campo Chiave precedente.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record] </td> 
   <td> <p>Immetti i valori desiderati nei campi del record.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Aggiornare un record]

Questo modulo di azione aggiorna un record.

Specificare l&#39;archivio dati e la chiave del record.

Il modulo restituisce l’ID del record e di tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Archivio dati]</td> 
   <td> <p> Selezionare o aggiungere l'archivio dati in cui si desidera creare un record. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Key] </td> 
   <td> <p>Immettere la chiave univoca del record che si desidera aggiornare nel modulo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Inserisci record mancante] </td> 
   <td> <p>Abilita questa opzione per creare un nuovo record se il record con la chiave specificata non esiste già.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record]</td> 
   <td> <p> Immettere i valori desiderati nei campi del record che si desidera aggiornare.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Ottieni un record]

Questo modulo di azione recupera un record.

Specificare l&#39;archivio dati e la chiave del record.

Il modulo restituisce l’ID del record e di tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Archivio dati]</td> 
   <td> <p> Selezionare l'archivio dati da cui si desidera recuperare un record</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Key] </td> 
   <td> <p>Immettere la chiave univoca del record che si desidera recuperare dal modulo.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Controllare l&#39;esistenza di un record]

Questo modulo di azione specifica se esiste un record specifico.

Specificare l&#39;archivio dati e la chiave del record.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Archivio dati] </td> 
   <td> <p>Selezionare l'archivio dati che si desidera verificare per verificare l'esistenza del record.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Key] </td> 
   <td> <p>Immettere la chiave univoca del record che si desidera che il modulo verifichi l'esistenza.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Eliminare un record]

Questo modulo di azione elimina un record.

Specificare l&#39;archivio dati e la chiave del record.

Il modulo restituisce l’ID del record e di tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Archivio dati] </td> 
   <td> <p>Selezionare l'archivio dati che si desidera verificare per verificare l'esistenza del record.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Key] </td> 
   <td> <p>Immettere la chiave univoca del record che si desidera eliminare dal modulo.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Elimina tutti i record]

Questo modulo di azione elimina tutti i record da un particolare archivio dati.

Specificare l&#39;archivio dati.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Archivio dati] </td> 
   <td> <p>Selezionare l'archivio dati da cui si desidera eliminare tutti i record.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Cerca record]

Questo modulo di ricerca cerca i record in un oggetto dell&#39;archivio dati che corrispondono alla query di ricerca specificata.

Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Archivio dati]</td> 
   <td> <p> Selezionare l'archivio dati da cercare.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Filter]</p> </td> 
   <td> <p>Imposta il filtro per la ricerca.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Sort]</p> </td> 
   <td> <p style="font-weight: normal;">Per ogni campo di cui desideri eseguire l’ordinamento, compila i campi seguenti:</p> <p style="font-weight: bold;">[!UICONTROL Key]</p> <p>Seleziona il nome della colonna in base al quale vuoi ordinare i risultati.</p> <p style="font-weight: bold;">[!UICONTROL Order]</p> <p>Seleziona se ordinare i risultati in ordine crescente o decrescente.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td> <p> Imposta il numero massimo di risultati di ricerca [!DNL Workfront Fusion] restituisce durante un ciclo di esecuzione.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Continua l’esecuzione del percorso anche se il modulo non restituisce risultati]</td> 
   <td> <p> Se abilitato, la route di cui fa parte questo modulo continua l'elaborazione anche se questo modulo non restituisce risultati.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Record di conteggio]

Questo modulo di azione numera i record in un archivio dati.

Specificare l&#39;archivio dati.

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Archivio dati] </td> 
   <td> <p>Selezionare l'archivio dati contenente i record che si desidera conteggiare.</p> </td> 
  </tr> 
 </tbody> 
</table>
