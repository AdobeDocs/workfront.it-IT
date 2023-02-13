---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli Microsoft OneDrive for Business
description: In un [!DNL Adobe Workfront Fusion] puoi automatizzare i flussi di lavoro che utilizzano [!DNL Microsoft OneDrive for Business], nonché collegarlo a più applicazioni e servizi di terze parti.
author: Becky
feature: Workfront Fusion
exl-id: b7175cb9-aade-49b7-a28b-25fc9805a078
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1039'
ht-degree: 0%

---

# [!DNL Microsoft OneDrive for Business] moduli

In un [!DNL Adobe Workfront Fusion] puoi automatizzare i flussi di lavoro che utilizzano [!DNL Microsoft OneDrive for Business], nonché collegarlo a più applicazioni e servizi di terze parti.

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

Per utilizzare [!DNL Microsoft OneDrive for Business] con [!DNL Adobe Workfront Fusion], sarà necessario un [!DNL Microsoft] conto.

Per istruzioni su come collegare le [!DNL OneDrive for Business] account a [!DNL Workfront Fusion], vedi [Creare una connessione ad Adobe [!DNL Workfront Fusion] - Istruzioni di base](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!DNL Microsoft OneDrive for Business] moduli e relativi campi

Quando si configura [!DNL Microsoft OneDrive for Business] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL Microsoft OneDrive for Business] potrebbero essere visualizzati, a seconda di fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se trovi il pulsante mappa sopra un campo o una funzione, puoi utilizzarlo per impostare variabili e funzioni per quel campo. Per ulteriori informazioni, consulta [Mappare informazioni da un modulo a un altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Azioni](#actions)

### Triggers

* [[!UICONTROL File di controllo]](#watch-files)
* [[!UICONTROL Cartelle di controllo]](#watch-folders)

#### [!UICONTROL File di controllo]

Questo modulo di attivazione si attiva quando un nuovo file viene aggiunto o aggiornato in una cartella controllata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Collega l’app o il servizio Web del modulo a [!DNL Workfront Fusion]</a> nell'articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crea uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID unità]</p> </td> 
   <td> <p>Selezionare l'unità che si desidera controllare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cartella]</td> 
   <td> <p> Selezionare la cartella da controllare. In uno scenario, è possibile monitorare una sola cartella.</p> <p>Suggerimento: Per tenere traccia di più cartelle, crea uno scenario indipendente per ciascuna di esse.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Voglio guardare]</p> </td> 
   <td> <p>Selezionare se si desidera visualizzare solo i nuovi file e tutte le modifiche o i nuovi file.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Numero massimo di righe restituite]</td> 
   <td> <p> Imposta il numero massimo di risultati che [!DNL Workfront Fusion] funziona con durante un ciclo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Cartelle di controllo]

Questo modulo trigger si attiva quando viene aggiunta una nuova cartella alla cartella controllata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Collega l’app o il servizio Web del modulo a [!DNL Workfront Fusion]</a> nell'articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crea uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID unità]</p> </td> 
   <td> <p>Selezionare l'unità che si desidera controllare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cartella]</td> 
   <td> <p> Selezionare la cartella da controllare. In uno scenario, è possibile monitorare una sola cartella.</p> <p>Suggerimento: Per tenere traccia di più cartelle, crea uno scenario indipendente per ciascuna di esse.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Voglio guardare]</p> </td> 
   <td> <p>Seleziona se visualizzare solo le nuove cartelle e tutte le modifiche o le nuove cartelle.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Numero massimo di righe restituite]</td> 
   <td> <p> Imposta il numero massimo di risultati che [!DNL Workfront Fusion] funziona con durante un ciclo.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Azioni

* [[!UICONTROL Caricare un file]](#upload-a-file)
* [[!UICONTROL Eliminare un file]](#delete-a-file)
* [[!UICONTROL Ottieni un file]](#get-a-file)
* [[!UICONTROL Creare una cartella]](#create-a-folder)
* [[!UICONTROL Eliminare una cartella]](#delete-a-folder)
* [[!UICONTROL Ottenere un collegamento di condivisione]](#get-a-sharing-link)

#### [!UICONTROL Caricare un file]

Questo modulo di azione carica un file binario o di testo in una cartella specifica

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Collega l’app o il servizio Web del modulo a [!DNL Workfront Fusion]</a> nell'articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crea uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID unità]</td> 
   <td> <p>Selezionare l'unità in cui si desidera caricare un file.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cartella] </td> 
   <td> <p>Selezionare la cartella all'interno dell'unità.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL File di origine]</p> </td> 
   <td> <p>Selezionare un file di origine da un modulo precedente o mappare il nome e i dati del file di origine.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Se esiste il file con lo stesso nome]</td> 
   <td> <p> Seleziona ciò che desideri fare se esiste già un file con lo stesso nome del file che stai tentando di caricare.</p> 
    <ul> 
     <li>[!UICONTROL Sostituisci il file esistente]</li> 
     <li>[!UICONTROL Rinomina il nuovo file]</li> 
     <li>[!UICONTROL Fine con un errore]</li> 
    </ul> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminare un file]

Questo modulo di azione sposta il file specificato nel cestino.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Collega l’app o il servizio Web del modulo a [!DNL Workfront Fusion]</a> nell'articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crea uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID unità]</td> 
   <td> <p>Selezionare l'unità da cui si desidera eliminare un file.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File ID]</td> 
   <td> <p>Immetti l’ID del file da eliminare. </p> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottieni un file]

Questo modulo di azione recupera il file con l’ID specificato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Collega l’app o il servizio Web del modulo a [!DNL Workfront Fusion]</a> nell'articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crea uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID unità]</td> 
   <td> <p>Selezionare l'unità da cui si desidera recuperare un file.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File ID]</td> 
   <td> <p>Immetti l’ID del file da recuperare. </p> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Creare una cartella]

Crea una cartella all’interno della cartella principale specificata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>[!UICONTROL Connection]</strong> </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Collega l’app o il servizio Web del modulo a [!DNL Workfront Fusion]</a> nell'articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crea uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL ID unità]</strong> </td> 
   <td> <p>Selezionare l'unità in cui si desidera creare una nuova cartella.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL Cartella]</strong> </td> 
   <td> <p>Selezionare la cartella in cui si desidera creare una nuova cartella.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL Nome cartella]</strong> </td> 
   <td>Immettere o mappare un nome per la nuova cartella.</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminare una cartella]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Collega l’app o il servizio Web del modulo a [!DNL Workfront Fusion]</a> nell'articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crea uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID unità]</td> 
   <td> <p>Selezionare l'unità da cui si desidera eliminare un file.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>ID cartella [!UICONTROL]</td> 
   <td> <p>Immetti o mappa l’ID della cartella da eliminare. </p> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottenere un collegamento di condivisione]

Questo modulo recupera un collegamento che è possibile condividere per consentire l’accesso al file specificato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Office 365] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Collega l’app o il servizio Web del modulo a [!DNL Workfront Fusion]</a> nell'articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crea uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID unità]</td> 
   <td> <p>Selezionare l'unità in cui si desidera caricare un file.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Enter]</td> 
   <td> <p>Selezionare se si desidera scegliere un file utilizzando l'ID file o il percorso del file. Immettere l'ID o il percorso del file nel campo visualizzato.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Tipo di autorizzazione]</p> </td> 
   <td> <p>Seleziona se le persone che ricevono il collegamento devono disporre delle autorizzazioni di lettura/scrittura o di sola lettura.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Ambito [!UICONTROL]</td> 
   <td> <p> Seleziona se desideri che il file sia accessibile a chiunque disponga del collegamento o accessibile solo ai membri della tua organizzazione.</p> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>
