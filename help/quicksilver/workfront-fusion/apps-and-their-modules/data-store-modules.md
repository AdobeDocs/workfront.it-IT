---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Moduli archivio dati
description: Un archivio dati  [!DNL Adobe Workfront Fusion] , simile a un database o a una semplice tabella, può memorizzare i dati di scenari, consentendo il trasferimento di dati tra scenari singoli o l'esecuzione di scenari singoli. È possibile utilizzare un archivio dati per memorizzare nuovi dati provenienti da vari sistemi durante la sincronizzazione.
author: Becky
feature: Workfront Fusion
exl-id: 1dc9cb88-d1b9-4a67-91fb-be980cc1ccd1
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '1164'
ht-degree: 0%

---

# [!UICONTROL Moduli archivio dati]

Un archivio dati [!DNL Adobe Workfront Fusion], simile a un database o a una semplice tabella, può memorizzare i dati di scenari, consentendo il trasferimento dei dati tra scenari singoli o l&#39;esecuzione di scenari singoli. È possibile utilizzare un archivio dati per memorizzare nuovi dati provenienti da vari sistemi durante la sincronizzazione.

I moduli dell&#39;archivio dati consentono di aggiungere, sostituire, aggiornare, recuperare, eliminare, cercare o contare i record nell&#39;archivio dati [!DNL Adobe Workfront Fusion].

Per informazioni sulla creazione, la modifica e la risoluzione dei problemi relativi agli archivi dati, vedere [Archivi dati in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

Per un video introduttivo sugli archivi dati in Workfront Fusion, vedi:

* [Archivi dati](https://video.tv.adobe.com/v/3427029/){target=_blank}

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
   <p>Requisiti di licenza correnti: nessun requisito di licenza [!DNL Workfront Fusion].</p>
   <p>Oppure</p>
   <p>Requisito licenza legacy: [!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione lavoro], [!UICONTROL [!DNL Workfront Fusion] per automazione lavoro]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>
   <p>Fabbisogno prodotto corrente: se disponi del piano [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront], la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo. [!DNL Workfront Fusion] è incluso nel piano [!UICONTROL Ultimate] [!DNL Workfront].</p>
   <p>Oppure</p>
   <p>Requisiti del prodotto legacy: la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Per conoscere il piano, il tipo di licenza o l&#39;accesso disponibili, contattare l&#39;amministratore [!DNL Workfront].

Per informazioni sulle [!DNL Adobe Workfront Fusion] licenze, vedere [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Prerequisiti

Per utilizzare i moduli [!UICONTROL Archivio dati], è necessario innanzitutto creare un archivio dati.

Per informazioni sulla creazione di archivi dati, vedere [Archivi dati in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

## Moduli [!UICONTROL Archivio dati] e relativi campi

Quando si configurano i moduli Archivio dati, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Insieme a questi, potrebbero essere visualizzati campi aggiuntivi del Data Store, a seconda di fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se viene visualizzato il pulsante Mappa sopra un campo o una funzione, è possibile utilizzarlo per impostare variabili e funzioni per tale campo. Per ulteriori informazioni, vedere [Mappare le informazioni da un modulo all&#39;altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

Tutti i moduli [!UICONTROL Archivio dati] sono moduli di tipo Azione.

* [Aggiungere/sostituire un record](#addreplace-a-record)
* [Aggiornare un record](#update-a-record)
* [Ottieni un record](#get-a-record)
* [Verificare l&#39;esistenza di un record](#check-the-existence-of-a-record)
* [Eliminare un record](#delete-a-record)
* [Elimina tutti i record](#delete-all-records)
* [Cerca record](#search-records)
* [Conteggio record](#count-records)

### [!UICONTROL Aggiungi/Sostituisci un record]

Questo modulo di azione aggiunge o sostituisce un record.

Specificare l&#39;archivio dati e la chiave del record.

Il modulo restituisce l’ID del record ed eventuali campi associati, insieme a eventuali campi e valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario.

>[!NOTE]
>
>Il modulo genera un errore quando si tenta di aggiungere il record già presente nell&#39;archivio dati con lo stesso nome e l&#39;opzione [!UICONTROL Sovrascrivi un record esistente] è disabilitata.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Archivio dati [!UICONTROL]</td> 
   <td> <p> Selezionare o aggiungere l'archivio dati in cui si desidera creare un record. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Key] </td> 
   <td> <p>Immettere la chiave univoca del record che si desidera venga aggiunto o sostituito dal modulo. La chiave può essere utilizzata in un secondo momento per recuperare il record. Se lasci vuoto questo campo, viene generata automaticamente una chiave.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sovrascrive un record esistente] </td> 
   <td> <p>Abilita questa opzione per sovrascrivere il record. Il record che desideri sovrascrivere deve essere specificato nel campo Chiave qui sopra.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record] </td> 
   <td> <p>Immettere i valori desiderati nei campi del record.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Aggiorna un record]

Questo modulo di azione aggiorna un record.

Specificare l&#39;archivio dati e la chiave del record.

Il modulo restituisce l’ID del record ed eventuali campi associati, insieme a eventuali campi e valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Archivio dati [!UICONTROL]</td> 
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

Il modulo restituisce l’ID del record ed eventuali campi associati, insieme a eventuali campi e valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Archivio dati [!UICONTROL]</td> 
   <td> <p> Selezionare l'archivio dati da cui si desidera recuperare un record</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Key] </td> 
   <td> <p>Immettere la chiave univoca del record che si desidera recuperare dal modulo.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Verifica l&#39;esistenza di un record]

Questo modulo di azione specifica se esiste un record specifico.

Specificare l&#39;archivio dati e la chiave del record.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Archivio dati [!UICONTROL] </td> 
   <td> <p>Selezionare l'archivio dati che si desidera verificare per verificare l'esistenza del record.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Key] </td> 
   <td> <p>Immettere la chiave univoca del record che si desidera che il modulo verifichi.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Eliminare un record]

Questo modulo di azione elimina un record.

Specificare l&#39;archivio dati e la chiave del record.

Il modulo restituisce l’ID del record ed eventuali campi associati, insieme a eventuali campi e valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Archivio dati [!UICONTROL] </td> 
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

Specifica l’archivio dati.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Archivio dati [!UICONTROL] </td> 
   <td> <p>Selezionare l'archivio dati da cui si desidera eliminare tutti i record.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Cerca record]

Questo modulo di ricerca cerca i record in un oggetto nell’archivio dati che corrispondono alla query di ricerca specificata.

Puoi mappare queste informazioni nei moduli successivi nello scenario.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Archivio dati [!UICONTROL]</td> 
   <td> <p> Seleziona l’archivio dati in cui desideri eseguire la ricerca.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Filtro]</p> </td> 
   <td> <p>Imposta il filtro per la ricerca.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Sort]</p> </td> 
   <td> <p style="font-weight: normal;">Per ogni campo in base al quale si desidera eseguire l'ordinamento, compilare i campi seguenti:</p> <p style="font-weight: bold;">[!UICONTROL Key]</p> <p>Selezionare il nome della colonna in base al quale si desidera ordinare i risultati.</p> <p style="font-weight: bold;">[!UICONTROL Order]</p> <p>Seleziona se desideri ordinare i risultati in ordine crescente o decrescente.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td> <p> Impostare il numero massimo di risultati di ricerca [!DNL Workfront Fusion] restituiti durante un ciclo di esecuzione.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Continua l'esecuzione della route anche se il modulo non restituisce alcun risultato]</td> 
   <td> <p> Se attivato, il ciclo di lavorazione di cui fa parte il modulo continua l'elaborazione anche se il modulo non restituisce alcun risultato.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Conteggio record]

Questo modulo di azione numera i record in un archivio dati.

Specifica l’archivio dati.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Archivio dati [!UICONTROL] </td> 
   <td> <p>Selezionare l'archivio dati contenente i record che si desidera conteggiare.</p> </td> 
  </tr> 
 </tbody> 
</table>
