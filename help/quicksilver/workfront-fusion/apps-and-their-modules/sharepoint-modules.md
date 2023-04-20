---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli SharePoint
description: In un [!DNL Adobe Workfront Fusion] In questo caso, puoi automatizzare i flussi di lavoro che utilizzano SharePoint e collegarli a più applicazioni e servizi di terze parti.
author: Becky
feature: Workfront Fusion
exl-id: 16d49031-06d2-4c86-bac4-f58cd9b2f1f5
source-git-commit: 8283022f24913988248005da0c8e583b29f19652
workflow-type: tm+mt
source-wordcount: '2371'
ht-degree: 0%

---

# [!DNL SharePoint] moduli

In un [!DNL Adobe Workfront Fusion] puoi automatizzare i flussi di lavoro che utilizzano [!DNL SharePoint], nonché collegarlo a più applicazioni e servizi di terze parti.

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

Per utilizzare [!DNL SharePoint] moduli, è necessario disporre di un [!DNL SharePoint] conto.

## Connetti [!DNL SharePoint] a [!DNL Workfront Fusion] {#connect-sharepoint-to-workfront-fusion}

* [Connetti [!DNL SharePoint] a [!DNL Workfront Fusion] utilizzando [!DNL Microsoft] account](#connect-sharepoint-to-workfront-fusion-using-a-microsoft-account)
* [Connetti [!DNL SharePoint] a [!DNL Workfront Fusion] utilizzo delle impostazioni avanzate](#connect-sharepoint-to-workfront-fusion-using-advanced-settings)

### Connetti [!DNL SharePoint] a [!DNL Workfront Fusion] utilizzando [!DNL Microsoft] account

È possibile utilizzare [!DNL Microsoft] per creare una connessione a [!DNL SharePoint]. Per istruzioni su come collegare le [!DNL Sharepoint] account a [!DNL Workfront Fusion], vedi [Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base](../../workfront-fusion/connections/connect-to-fusion-general.md)

### Connetti [!DNL SharePoint] a [!DNL Workfront Fusion] utilizzo delle impostazioni avanzate

Connessione [!DNL SharePoint] a [!DNL Workfront Fusion] senza [!DNL Microsoft] account, devi disporre di un ID client, di un segreto client e di un ID tenant.

1. Fai clic su **[!UICONTROL Aggiungi]** vicino alla parte superiore del **[!DNL SharePoint]** per aprire **[!UICONTROL Creare una connessione]** scatola.

1. (Facoltativo) Modificare il valore predefinito **[!UICONTROL Nome connessione]**.
1. Fai clic su **[!UICONTROL Mostra impostazioni avanzate]**.
1. Inserisci il [!DNL SharePoint] **[!UICONTROL ID client]** e **[!UICONTROL Segreto client]**.

1. Fai clic su **[!UICONTROL Continua]**.
1. Nella finestra di accesso visualizzata, immetti le tue credenziali per accedere all’app se non lo hai già fatto.
1. (Condizionale) Se un **[!UICONTROL Consenti]** viene visualizzato il pulsante , fai clic sul pulsante per collegare l’app a [!DNL Workfront Fusion].

## [!DNL SharePoint] moduli e relativi campi

Quando si configura [!DNL SharePoint] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL SharePoint] potrebbero essere visualizzati, a seconda di fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se trovi il pulsante mappa sopra un campo o una funzione, puoi utilizzarlo per impostare variabili e funzioni per quel campo. Per ulteriori informazioni, consulta [Mappare informazioni da un modulo a un altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Elemento drive](#drive-item)
* [Voce](#item)
* [Lista](#list)
* [Pagina (Beta)](#page-beta)
* [Sito](#site)
* [Altro](#other)

### Elemento drive

* [Creare un file](#create-a-file)
* [Creare una cartella](#create-a-folder)
* [Ottieni un file](#get-a-file)
* [Elementi cartella di controllo](#watch-folder-items)

#### Creare un file

Questo modulo di azione crea un nuovo file in SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL SharePoint] account a [!DNL Workfront Fusion], vedi <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connetti [!DNL SharePoint] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Immetti ID sito, unità e cartelle]</td> 
   <td> <p>Selezionare la modalità di identificazione della posizione del file che si desidera creare.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Invio manuale]</strong> </p> <p>Inserisci o mappa il <strong>[!UICONTROL Site ID]</strong>, <strong>[!UICONTROL List ID]</strong>e <strong>ID cartella [!UICONTROL]</strong> nei campi visualizzati.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleziona dall’elenco che segui]</strong> </p> <p>Selezionare il percorso in cui si desidera creare il file. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File di origine]</td> 
   <td>Selezionare un file di origine da un modulo precedente o mappare il nome e i dati del file di origine.</td> 
  </tr>  </tbody> 
</table>

#### Creare una cartella

Questo modulo di azione crea una nuova cartella in SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL SharePoint] account a [!DNL Workfront Fusion], vedi <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connetti [!DNL SharePoint] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Immetti ID sito, unità e cartelle]</td> 
   <td> <p>Selezionare la posizione in cui si desidera identificare la cartella da creare.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Invio manuale]</strong> </p> <p>Inserisci o mappa il <strong>[!UICONTROL Site ID]</strong>, <strong>[!UICONTROL List ID]</strong>e <strong>ID cartella [!UICONTROL]</strong> nei campi visualizzati.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleziona dall’elenco che segui]</strong> </p> <p>Selezionare il percorso in cui si desidera creare la cartella. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome cartella]</td> 
   <td>Immettere o mappare un nome per la nuova cartella.</td> 
  </tr>
  </tbody> 
</table>

#### Ottieni un file

Questo modulo di azione recupera il file SharePoint specificato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL SharePoint] account a [!DNL Workfront Fusion], vedi <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connetti [!DNL SharePoint] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Immetti ID sito, unità e cartelle]</td> 
   <td> <p>Selezionare la modalità di identificazione della posizione del file che si desidera ottenere.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Invio manuale]</strong> </p> <p>Inserisci o mappa il <strong>[!UICONTROL Site ID]</strong>, <strong>[!UICONTROL List ID]</strong>e <strong>[!UICONTROL File ID]</strong> nei campi visualizzati.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleziona dall’elenco che segui]</strong> </p> <p>Selezionare la posizione del file. </p> </li> 
    </ul> </td> 
  </tr> 
</tbody> 
</table>

#### Elementi cartella di controllo

Questo modulo di attivazione avvia uno scenario quando un elemento viene aggiornato in una cartella selezionata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL SharePoint] account a [!DNL Workfront Fusion], vedi <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connetti [!DNL SharePoint] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Immetti ID sito, unità e cartelle]</td> 
   <td> <p>Selezionare la modalità di identificazione della posizione del file che si desidera ottenere.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Invio manuale]</strong> </p> <p>Inserisci o mappa il <strong>[!UICONTROL Site ID]</strong>, <strong>[!UICONTROL List ID]</strong>e <strong>ID cartella [!UICONTROL]</strong> nei campi visualizzati.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleziona dall’elenco che segui]</strong> </p> <p>Selezionare il percorso della cartella che si desidera controllare. </p> </li> 
    </ul> </td> 
  </tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Immettere il numero massimo di elementi [!DNL Workfront Fusion] dovrebbe essere restituito durante un ciclo di esecuzione di uno scenario.</td> 
  <tr>
  </tr>
</tbody> 
</table>

### Voce

* [[!UICONTROL Elementi da guardare]](#watch-items)
* [[!UICONTROL Elementi elenco]](#list-items)
* [[!UICONTROL Ottieni un elemento]](#get-an-item)
* [[!UICONTROL Creare un elemento]](#create-an-item)
* [[!UICONTROL Aggiornare un elemento]](#update-an-item)
* [[!UICONTROL Eliminare un elemento]](#delete-an-item)

#### [!UICONTROL Elementi da guardare]

Questo modulo di attivazione avvia uno scenario quando un elemento viene creato o modificato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL SharePoint] account a [!DNL Workfront Fusion], vedi <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connetti [!DNL SharePoint] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch List]</td> 
   <td>Seleziona se visualizzare gli elenchi per ora di creazione (nuovi elementi) o per ora di modifica (elementi aggiornati).</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Immetti l’ID del sito e dell’elenco]</td> 
   <td> <p>Selezionare la modalità di identificazione del sito e dell'elenco che si desidera controllare.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Invio manuale]</strong> </p> <p>Inserisci o mappa il <strong>[!UICONTROL Site ID]</strong> e <strong>[!UICONTROL List ID]</strong> nei campi visualizzati.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleziona dall’elenco che segui]</strong> </p> <p>Selezionare il sito da controllare, quindi selezionare l’elenco. Questi elenchi a discesa recuperano solo i siti seguiti.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Immettere o mappare il numero massimo di elementi che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Elementi elenco]

Questo modulo di azione recupera un elenco di tutti gli elementi in un elenco specificato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL SharePoint] account a [!DNL Workfront Fusion], vedi <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connetti [!DNL SharePoint] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ELENCO ELEMENTI]</td> 
   <td> <p>Selezionare la modalità di identificazione dell'elenco da cui si desidera recuperare gli elementi.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Invio manuale]</strong> </p> <p>Inserisci o mappa il <strong>[!UICONTROL Site ID]</strong> e <strong>[!UICONTROL List ID]</strong> nei campi visualizzati.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleziona dall’elenco]</strong> </p> <p>Selezionare il sito contenente l'elenco da cui si desidera recuperare gli elementi, quindi selezionare l'elenco. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Immettere o mappare il numero massimo di elementi che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottieni un elemento]

Questo modulo di azione restituisce i dati di un elemento specificato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL SharePoint] account a [!DNL Workfront Fusion], vedi <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connetti [!DNL SharePoint] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ottieni un elemento]</td> 
   <td> <p>Selezionare la modalità di identificazione del sito e dell'elenco che contengono l'elemento che si desidera ottenere.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Invio manuale]</strong> </p> <p>Inserisci o mappa il <strong>[!UICONTROL Site ID]</strong>, <strong>[!UICONTROL List ID]</strong>e <strong>[!UICONTROL ID elemento]</strong> nei campi visualizzati.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleziona dall’elenco]</strong> </p> <p>Selezionare il sito contenente l'elenco da cui si desidera recuperare un elemento, quindi selezionare l'elenco, quindi selezionare l'elemento. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Creare un elemento]

Questo modulo di azione crea un nuovo elemento in un elenco SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL SharePoint] account a [!DNL Workfront Fusion], vedi <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connetti [!DNL SharePoint] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Creare un elemento]</td> 
   <td> <p>Selezionare la modalità di identificazione del sito e dell'elenco in cui si desidera creare un elemento.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Invio manuale]</strong> </p> <p>Inserisci o mappa il <strong>[!UICONTROL Site ID]</strong> e <strong>[!UICONTROL List ID]</strong> nei campi visualizzati.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleziona dall’elenco]</strong> </p> <p>Selezionare il sito contenente l'elenco in cui si desidera creare un elemento, quindi selezionare l'elenco. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fields]</td> 
   <td>Per ogni campo che si desidera impostare per il nuovo elemento, immettere la chiave del campo (identifica il campo) e il valore che si desidera assegnare al nuovo elemento per tale campo.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggiornare un elemento]

Questo modulo di azione aggiorna un elemento esistente in un elenco SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL SharePoint] account a [!DNL Workfront Fusion], vedi <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connetti [!DNL SharePoint] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Aggiornare un elemento]</td> 
   <td> <p>Selezionare la modalità di identificazione del sito e dell'elenco contenente l'elemento che si desidera aggiornare.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Invio manuale]</strong> </p> <p>Inserisci o mappa il <strong>[!UICONTROL Site ID]</strong>, <strong>[!UICONTROL List ID]</strong>e <strong>[!UICONTROL ID elemento]</strong> nei campi visualizzati.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleziona dall’elenco]</strong> </p> <p>Selezionare il sito contenente l'elemento che si desidera aggiornare, quindi selezionare l'elenco, quindi selezionare l'elemento. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fields]</td> 
   <td>Per ogni campo che si desidera aggiornare per il nuovo elemento, immettere la chiave del campo (identifica il campo) e il nuovo valore che si desidera assegnare all'elemento per tale campo.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminare un elemento]

Questo modulo di azione elimina un elemento esistente in un elenco SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL SharePoint] account a [!DNL Workfront Fusion], vedi <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connetti [!DNL SharePoint] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Aggiornare un elemento]</td> 
   <td> <p>Selezionare la modalità di identificazione del sito e dell'elenco contenente l'elemento che si desidera eliminare.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Invio manuale]</strong> </p> <p>Inserisci o mappa il <strong>[!UICONTROL Site ID]</strong>, <strong>[!UICONTROL List ID]</strong>e <strong>[!UICONTROL ID elemento]</strong> nei campi visualizzati.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleziona dall’elenco]</strong> </p> <p>Selezionare il sito che contiene l'elemento da eliminare, quindi selezionare l'elenco, quindi selezionare l'elemento. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Lista

* [[!UICONTROL Elenchi di controllo]](#watch-lists)
* [[!UICONTROL Elenchi]](#list-lists)
* [[!UICONTROL Ottieni elenco]](#get-a-list)
* [[!UICONTROL Creare un elenco]](#create-a-list)

#### [!UICONTROL Elenchi di controllo]

Questo modulo di attivazione avvia uno scenario quando viene creato o modificato un elenco.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL SharePoint] account a [!DNL Workfront Fusion], vedi <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connetti [!DNL SharePoint] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch List]</td> 
   <td>Seleziona se visualizzare gli elenchi per ora di creazione (nuovi elementi) o per ora di modifica (elementi aggiornati).</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Immetti l’ID del sito e dell’elenco]</td> 
   <td> <p>Selezionare la modalità di identificazione del sito e dell'elenco che si desidera controllare.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Invio manuale]</strong> </p> <p>Inserisci o mappa il <strong>[!UICONTROL Site ID]</strong> in cui si trova l’elenco da visualizzare.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleziona dall’elenco che segui]</strong> </p> <p>Seleziona il sito da controllare. Il menu a discesa recupera solo il sito che segui.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Immettere o mappare il numero massimo di elenchi che si desidera che il modulo restituisca durante ogni ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Elenchi]

Questo modulo di azione recupera un elenco di tutti gli elementi in un elenco specificato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL SharePoint] account a [!DNL Workfront Fusion], vedi <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connetti [!DNL SharePoint] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elenco Elenchi]</td> 
   <td> <p>Selezionare la modalità di identificazione del sito da cui si desidera recuperare gli elenchi.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Invio manuale]</strong> </p> <p>Inserisci o mappa il <strong>[!UICONTROL Site ID]</strong>.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleziona dall’elenco]</strong> </p> <p>Selezionare il sito contenente gli elenchi da recuperare. Il menu a discesa recupera solo i siti seguiti.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Immettere o mappare il numero massimo di elenchi che si desidera che il modulo restituisca durante ogni ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottieni elenco]

Questo modulo di azione restituisce i dati di un elenco specificato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL SharePoint] account a [!DNL Workfront Fusion], vedi <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connetti [!DNL SharePoint] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ottieni un elenco]</td> 
   <td> <p>Selezionare la modalità di identificazione del sito e dell'elenco che contengono l'elemento che si desidera ottenere.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Invio manuale]</strong> </p> <p>Inserisci o mappa il <strong>[!UICONTROL Site ID]</strong> e <strong>ID elenco</strong> nei campi visualizzati.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleziona dall’elenco]</strong> </p> <p>Selezionare il sito contenente l'elenco che si desidera recuperare, quindi selezionare l'elenco. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Creare un elenco]

Questo modulo di azione crea un nuovo elenco in SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL SharePoint] account a [!DNL Workfront Fusion], vedi <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connetti [!DNL SharePoint] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Immettere un ID sito]</td> 
   <td> <p>Selezionare la modalità di identificazione del sito e dell’elenco in cui si desidera creare un elenco.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Invio manuale]</strong> </p> <p>Inserisci o mappa il <strong>[!UICONTROL Site ID]</strong> in cui si desidera creare un elenco.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleziona dall’elenco]</strong> </p> <p>Selezionare il sito in cui si desidera creare un elenco. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Display Name]</td> 
   <td>Immettere o mappare un nome per il nuovo elenco.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Descrizione]</td> 
   <td>Immettere o mappare una descrizione per il nuovo elenco.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Aggiungi colonne]</td> 
   <td>Per ogni colonna che si desidera impostare per il nuovo elenco, immettere un valore <strong>[!UICONTROL Name]</strong> per il campo e seleziona la <strong>[!UICONTROL Type]</strong> del valore che si desidera assegnare alla nuova colonna.</td> 
  </tr> 
 </tbody> 
</table>

### Pagina (Beta)

>[!NOTE]
>
>API in `beta` versione in [!DNL Microsoft Graph] sono soggette a cambiamento. L&#39;utilizzo di queste API nelle applicazioni di produzione non è supportato.

#### [!UICONTROL Ottieni una pagina]

Questo modulo di azione restituisce i dati di una pagina specificata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL SharePoint] account a [!DNL Workfront Fusion], vedi <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connetti [!DNL SharePoint] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ottieni una pagina]</td> 
   <td> <p>Seleziona la modalità di identificazione della pagina da recuperare.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Invio manuale]</strong> </p> <p>Inserisci o mappa il <strong>[!UICONTROL Site ID]</strong>e <strong>[!UICONTROL Page ID]</strong>.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleziona dall’elenco]</strong> </p> <p>Seleziona il sito che contiene la pagina da recuperare, quindi seleziona la pagina.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Sito

* [[!UICONTROL Ricerca siti]](#search-sites)
* [[!UICONTROL Ottieni sito]](#get-a-site)

#### [!UICONTROL Ricerca siti]

Questo modulo di azione cerca i siti in base a un parametro specificato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL SharePoint] account a [!DNL Workfront Fusion], vedi <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connetti [!DNL SharePoint] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Parola chiave del nome visualizzato]</td> 
   <td> <p>Immetti o mappa il termine di ricerca per il quale desideri eseguire la ricerca nei siti.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Immettere o mappare il numero massimo di siti che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottieni sito]

Questo modulo di azione restituisce i dati di un sito specificato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL SharePoint] account a [!DNL Workfront Fusion], vedi <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connetti [!DNL SharePoint] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ottenere un sito]</td> 
   <td> <p>Seleziona la modalità di identificazione della pagina da recuperare.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Invio manuale]</strong> </p> <p>Inserisci o mappa il <strong>[!UICONTROL Site ID]</strong>.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleziona dall’elenco]</strong> </p> <p>Selezionare il sito da recuperare.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Altro

#### [!UICONTROL Effettuare una chiamata API]

Questo modulo ti consente di eseguire una chiamata API personalizzata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL SharePoint] account a [!DNL Workfront Fusion], vedi <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connetti [!DNL SharePoint] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Immettere un percorso relativo a <code>https://graph.microsoft.com</code>. Esempio:<code> /beta/sites</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL, Metodo]</p> </td> 
   td&gt; <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Aggiungi le intestazioni della richiesta sotto forma di un oggetto JSON standard. Ad esempio, <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] aggiunge le intestazioni di autorizzazione per te.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p> Aggiungi la query per la chiamata API sotto forma di un oggetto JSON standard.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type]</td> 
   <td>Seleziona il tipo di dati da inviare nella chiamata API.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Aggiungi il contenuto del corpo per la chiamata API sotto forma di un oggetto JSON standard.</p> <p>Nota:  <p>Quando si utilizzano istruzioni condizionali come <code>if</code> nel JSON, inserisci le virgolette al di fuori dell’istruzione condizionale.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

