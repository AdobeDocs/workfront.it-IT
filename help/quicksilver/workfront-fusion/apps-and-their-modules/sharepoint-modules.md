---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli SharePoint
description: In un [!DNL Adobe Workfront Fusion] scenario, puoi automatizzare i flussi di lavoro che utilizzano SharePoint e collegarlo a più applicazioni e servizi di terze parti.
author: Becky
feature: Workfront Fusion
exl-id: 16d49031-06d2-4c86-bac4-f58cd9b2f1f5
source-git-commit: 8b4182ae2b32488a02cacc16fcb6a246fcb571fd
workflow-type: tm+mt
source-wordcount: '2850'
ht-degree: 0%

---

# [!DNL SharePoint] moduli

In un [!DNL Adobe Workfront Fusion] scenario, puoi automatizzare i flussi di lavoro che utilizzano [!DNL SharePoint], oltre a collegarlo a più applicazioni e servizi di terze parti.

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

Da utilizzare [!DNL SharePoint] moduli, è necessario disporre di un [!DNL SharePoint] account.

## Connetti [!DNL SharePoint] a [!DNL Workfront Fusion] {#connect-sharepoint-to-workfront-fusion}

* [Connetti [!DNL SharePoint] a [!DNL Workfront Fusion] utilizzando un [!DNL Microsoft] account](#connect-sharepoint-to-workfront-fusion-using-a-microsoft-account)
* [Connetti [!DNL SharePoint] a [!DNL Workfront Fusion] utilizzo delle impostazioni avanzate](#connect-sharepoint-to-workfront-fusion-using-advanced-settings)

### Connetti [!DNL SharePoint] a [!DNL Workfront Fusion] utilizzando un [!DNL Microsoft] account

Puoi utilizzare il tuo [!DNL Microsoft] account a cui creare una connessione [!DNL SharePoint]. Per istruzioni sulla connessione [!DNL Sharepoint] account a [!DNL Workfront Fusion], vedi [Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base](../../workfront-fusion/connections/connect-to-fusion-general.md)

### Connetti [!DNL SharePoint] a [!DNL Workfront Fusion] utilizzo delle impostazioni avanzate

Per connettersi [!DNL SharePoint] a [!DNL Workfront Fusion] senza [!DNL Microsoft] , è necessario un ID client, un segreto client e un ID tenant.

1. Clic **[!UICONTROL Aggiungi]** vicino alla parte superiore del **[!DNL SharePoint]** per aprire la **[!UICONTROL Creare una connessione]** casella.

1. (Facoltativo) Modifica il valore predefinito **[!UICONTROL Nome connessione]**.
1. Clic **[!UICONTROL Mostra impostazioni avanzate]**.
1. Inserisci il [!DNL SharePoint] **[!UICONTROL ID client]** e **[!UICONTROL Segreto client]**.

1. Clic **[!UICONTROL Continua]**.
1. Nella finestra di accesso visualizzata, inserisci le credenziali per accedere all’app, se non lo hai già fatto.
1. (Condizionale) Se un **[!UICONTROL Consenti]** viene visualizzato, fai clic sul pulsante per collegare l’app a [!DNL Workfront Fusion].

## [!DNL SharePoint] moduli e relativi campi

Quando si configura [!DNL SharePoint] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL SharePoint] I campi potrebbero essere visualizzati in base a fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se viene visualizzato il pulsante Mappa sopra un campo o una funzione, è possibile utilizzarlo per impostare variabili e funzioni per tale campo. Per ulteriori informazioni, consulta [Mappare le informazioni da un modulo all’altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Elemento unità](#drive-item)
* [Voce](#item)
* [Lista](#list)
* [Pagina (Beta)](#page-beta)
* [Sito](#site)
* [Altro](#other)

### Elemento unità

* [Creare un file](#create-a-file)
* [Creare una cartella](#create-a-folder)
* [Ottieni un file](#get-a-file)
* [Osserva elementi cartella](#watch-folder-items)

#### Ottieni modifiche

Questo modulo restituisce le modifiche apportate in SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL SharePoint] account a [!DNL Workfront Fusion], vedi <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connetti [!DNL SharePoint] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Immetti ID di sito, unità e cartella]</td> 
   <td> <p>Seleziona la modalità di identificazione della posizione della cartella in cui desideri recuperare le modifiche.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Invio manuale]</strong> </p> <p>Inserisci o mappa il <strong>[!UICONTROL ID sito]</strong>, <strong>[!UICONTROL ID elenco]</strong>, e <strong>[!UICONTROL ID cartella]</strong> nei campi visualizzati.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleziona dall'elenco che segui]</strong> </p> <p>Seleziona il percorso in cui desideri recuperare le modifiche. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Token]</td> 
   <td> </td> 
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
   <td> <p>Per istruzioni sulla connessione [!DNL SharePoint] account a [!DNL Workfront Fusion], vedi <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connetti [!DNL SharePoint] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Immetti ID di sito, unità e cartella]</td> 
   <td> <p>Seleziona la modalità di identificazione della posizione della cartella da creare.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Invio manuale]</strong> </p> <p>Inserisci o mappa il <strong>[!UICONTROL ID sito]</strong>, <strong>[!UICONTROL ID elenco]</strong>, e <strong>[!UICONTROL ID cartella]</strong> nei campi visualizzati.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleziona dall'elenco che segui]</strong> </p> <p>Seleziona il percorso in cui desideri creare la cartella. </p> </li> 
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
   <td> <p>Per istruzioni sulla connessione [!DNL SharePoint] account a [!DNL Workfront Fusion], vedi <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connetti [!DNL SharePoint] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Immetti ID di sito, unità e cartella]</td> 
   <td> <p>Selezionare la modalità di identificazione della posizione del file che si desidera ottenere.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Invio manuale]</strong> </p> <p>Inserisci o mappa il <strong>[!UICONTROL ID sito]</strong>, <strong>[!UICONTROL ID elenco]</strong>, e <strong>[!UICONTROL ID file]</strong> nei campi visualizzati.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleziona dall'elenco che segui]</strong> </p> <p>Selezionare il percorso del file. </p> </li> 
    </ul> </td> 
  </tr> 
</tbody> 
</table>

#### Osserva elementi cartella

Questo modulo di attivazione avvia uno scenario quando un elemento viene aggiornato in una cartella selezionata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL SharePoint] account a [!DNL Workfront Fusion], vedi <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connetti [!DNL SharePoint] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Immetti ID di sito, unità e cartella]</td> 
   <td> <p>Selezionare la modalità di identificazione della posizione del file che si desidera ottenere.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Invio manuale]</strong> </p> <p>Inserisci o mappa il <strong>[!UICONTROL ID sito]</strong>, <strong>[!UICONTROL ID elenco]</strong>, e <strong>[!UICONTROL ID cartella]</strong> nei campi visualizzati.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleziona dall'elenco che segui]</strong> </p> <p>Seleziona il percorso della cartella da controllare. </p> </li> 
    </ul> </td> 
  </tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Immetti il numero massimo di elementi [!DNL Workfront Fusion] deve essere restituito durante un ciclo di esecuzione dello scenario.</td> 
  <tr>
  </tr>
</tbody> 
</table>

### Voce

* [[!UICONTROL Copia elemento]](#copy-an-item)
* [[!UICONTROL Creare un elemento]](#create-an-item)
* [[!UICONTROL Eliminare un elemento]](#delete-an-item)
* [[!UICONTROL Ottieni un elemento]](#get-an-item)
* [[!UICONTROL Elementi elenco]](#list-items)
* [[!UICONTROL Sposta elemento]](#move-an-item)
* [[!UICONTROL Aggiornare un elemento]](#update-an-item)
* [[!UICONTROL Osserva elementi] (Pianificato)](#watch-items-scheduled)


#### [!UICONTROL Copia elemento]

Questo modulo di azione copia un elemento esistente in un elenco SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL SharePoint] account a [!DNL Workfront Fusion], vedi <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connetti [!DNL SharePoint] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Immetti ID sito, unità e cartella</td> 
   <td> <p>Selezionare la modalità di identificazione del sito e dell'elenco contenente l'elemento che si desidera copiare.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Invio manuale]</strong> </p> <p>Inserisci o mappa il <strong>[!UICONTROL ID sito]</strong>, <strong>[!UICONTROL ID elenco]</strong>, e <strong>[!UICONTROL ID elemento]</strong> nei campi visualizzati.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleziona dall'elenco che segui]</strong> </p> <p>Nel campo Tipo elemento selezionare se si sta spostando un campo o una cartella.  Selezionare il sito contenente l'elemento che si desidera copiare, quindi selezionare l'elenco, quindi selezionare l'elemento. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID destinazione]</td> 
   <td> Immettere o mappare l'ID della cartella in cui si desidera copiare l'elemento. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nuovo nome]</td> 
   <td>Immettere o mappare un nome per la nuova copia dell'elemento. </td> 
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
   <td> <p>Per istruzioni sulla connessione [!DNL SharePoint] account a [!DNL Workfront Fusion], vedi <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connetti [!DNL SharePoint] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Crea un elemento]</td> 
   <td> <p>Selezionare la modalità di identificazione del sito e dell'elenco in cui si desidera creare un elemento.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Invio manuale]</strong> </p> <p>Inserisci o mappa il <strong>[!UICONTROL ID sito]</strong> e <strong>[!UICONTROL ID elenco]</strong> nei campi visualizzati.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleziona dall'elenco]</strong> </p> <p>Selezionare il sito contenente l'elenco in cui si desidera creare un elemento, quindi selezionare l'elenco. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fields]</td> 
   <td>Per ogni campo che si desidera impostare per il nuovo elemento, immettere la chiave del campo (identifica il campo) e il valore che si desidera assegnare al nuovo elemento per tale campo.</td> 
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
   <td> <p>Per istruzioni sulla connessione [!DNL SharePoint] account a [!DNL Workfront Fusion], vedi <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connetti [!DNL SharePoint] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Aggiorna un elemento]</td> 
   <td> <p>Selezionare la modalità di identificazione del sito e dell'elenco che contiene l'elemento che si desidera eliminare.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Invio manuale]</strong> </p> <p>Inserisci o mappa il <strong>[!UICONTROL ID sito]</strong>, <strong>[!UICONTROL ID elenco]</strong>, e <strong>[!UICONTROL ID elemento]</strong> nei campi visualizzati.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleziona dall'elenco]</strong> </p> <p>Selezionare il sito contenente l'elemento che si desidera eliminare, quindi selezionare l'elenco e l'elemento. </p> </li> 
    </ul> </td> 
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
   <td> <p>Per istruzioni sulla connessione [!DNL SharePoint] account a [!DNL Workfront Fusion], vedi <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connetti [!DNL SharePoint] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ottiene un elemento]</td> 
   <td> <p>Selezionare la modalità di identificazione del sito e dell'elenco che contiene l'elemento che si desidera ottenere.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Invio manuale]</strong> </p> <p>Inserisci o mappa il <strong>[!UICONTROL ID sito]</strong>, <strong>[!UICONTROL ID elenco]</strong>, e <strong>[!UICONTROL ID elemento]</strong> nei campi visualizzati.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleziona dall'elenco]</strong> </p> <p>Selezionare il sito contenente l'elenco dal quale si desidera recuperare un elemento, quindi selezionare l'elenco e selezionare l'elemento. </p> </li> 
    </ul> </td> 
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
   <td> <p>Per istruzioni sulla connessione [!DNL SharePoint] account a [!DNL Workfront Fusion], vedi <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connetti [!DNL SharePoint] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL voci di elenco]</td> 
   <td> <p>Selezionare la modalità di identificazione dell'elenco da cui si desidera recuperare gli elementi.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Invio manuale]</strong> </p> <p>Inserisci o mappa il <strong>[!UICONTROL ID sito]</strong> e <strong>[!UICONTROL ID elenco]</strong> nei campi visualizzati.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleziona dall'elenco]</strong> </p> <p>Selezionare il sito contenente l'elenco da cui si desidera recuperare gli elementi, quindi selezionare l'elenco. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Immettere o mappare il numero massimo di elementi che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Spostare un elemento]

Questo modulo di azione copia un elemento esistente in un elenco SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL SharePoint] account a [!DNL Workfront Fusion], vedi <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connetti [!DNL SharePoint] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Immetti ID sito, unità e cartella</td> 
   <td> <p>Selezionare la modalità di identificazione del sito e dell'elenco che contiene l'elemento che si desidera spostare.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Invio manuale]</strong> </p> <p>Inserisci o mappa il <strong>[!UICONTROL ID sito]</strong>, <strong>[!UICONTROL ID elenco]</strong>, e <strong>[!UICONTROL ID elemento]</strong> nei campi visualizzati.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleziona dall'elenco che segui]</strong> </p> <p>Nel campo Tipo elemento selezionare se si sta spostando un campo o una cartella. Selezionare il sito contenente l'elemento che si desidera copiare, quindi selezionare l'elenco, quindi selezionare l'elemento. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID destinazione]</td> 
   <td> Immettere o mappare l'ID della cartella in cui si desidera spostare l'elemento. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nuovo nome]</td> 
   <td>Immettere o mappare un nome per l'elemento spostato. </td> 
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
   <td> <p>Per istruzioni sulla connessione [!DNL SharePoint] account a [!DNL Workfront Fusion], vedi <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connetti [!DNL SharePoint] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Aggiorna un elemento]</td> 
   <td> <p>Selezionare la modalità di identificazione del sito e dell'elenco contenente l'elemento che si desidera aggiornare.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Invio manuale]</strong> </p> <p>Inserisci o mappa il <strong>[!UICONTROL ID sito]</strong>, <strong>[!UICONTROL ID elenco]</strong>, e <strong>[!UICONTROL ID elemento]</strong> nei campi visualizzati.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleziona dall'elenco]</strong> </p> <p>Selezionare il sito contenente l'elemento che si desidera aggiornare, quindi selezionare l'elenco e l'elemento. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fields]</td> 
   <td>Per ogni campo che si desidera aggiornare per il nuovo elemento, immettere la chiave del campo (identifica il campo) e il nuovo valore che si desidera assegnare all'elemento per tale campo.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Osserva elementi] (Pianificato)

Questo modulo di attivazione avvia uno scenario quando un elemento viene creato o modificato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL SharePoint] account a [!DNL Workfront Fusion], vedi <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connetti [!DNL SharePoint] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elenchi di controllo]</td> 
   <td>Seleziona se desideri controllare gli elenchi in base all’ora di creazione (nuovi elementi) o di modifica (elementi aggiornati).</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Immetti ID sito ed elenco]</td> 
   <td> <p>Selezionare la modalità di identificazione del sito e dell'elenco che si desidera controllare.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Invio manuale]</strong> </p> <p>Inserisci o mappa il <strong>[!UICONTROL ID sito]</strong> e <strong>[!UICONTROL ID elenco]</strong> nei campi visualizzati.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleziona dall'elenco che segui]</strong> </p> <p>Seleziona il sito da monitorare, quindi fai clic sull’elenco. Questi menu a discesa recuperano solo i siti seguiti.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Immettere o mappare il numero massimo di elementi che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Lista

* [[!UICONTROL Creare un elenco]](#create-a-list)
* [[!UICONTROL Ottieni un elenco]](#get-a-list)
* [[!UICONTROL Elenchi]](#list-lists)
* [[!UICONTROL Elenchi di verifica]](#watch-lists)

#### [!UICONTROL Creare un elenco]

Questo modulo di azione crea un nuovo elenco in SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL SharePoint] account a [!DNL Workfront Fusion], vedi <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connetti [!DNL SharePoint] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Immetti un ID sito]</td> 
   <td> <p>Selezionare la modalità di identificazione del sito e dell'elenco in cui si desidera creare un elenco.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Invio manuale]</strong> </p> <p>Inserisci o mappa il <strong>[!UICONTROL ID sito]</strong> dove si desidera creare un elenco.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleziona dall'elenco]</strong> </p> <p>Selezionare il sito in cui si desidera creare un elenco. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome visualizzato]</td> 
   <td>Immettere o mappare un nome per il nuovo elenco.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Descrizione]</td> 
   <td>Immettere o mappare una descrizione per il nuovo elenco.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Aggiungi colonne]</td> 
   <td>Per ogni colonna che si desidera impostare per il nuovo elenco, immettere un valore <strong>[!UICONTROL Name]</strong> per il campo e selezionare <strong>[!UICONTROL Type]</strong> del valore desiderato per la nuova colonna.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottieni un elenco]

Questo modulo di azione restituisce i dati di un elenco specificato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL SharePoint] account a [!DNL Workfront Fusion], vedi <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connetti [!DNL SharePoint] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ottiene un elenco]</td> 
   <td> <p>Selezionare la modalità di identificazione del sito e dell'elenco che contiene l'elemento che si desidera ottenere.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Invio manuale]</strong> </p> <p>Inserisci o mappa il <strong>[!UICONTROL ID sito]</strong> e <strong>ID elenco</strong> nei campi visualizzati.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleziona dall'elenco]</strong> </p> <p>Selezionare il sito contenente l'elenco che si desidera recuperare, quindi selezionare l'elenco. </p> </li> 
    </ul> </td> 
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
   <td> <p>Per istruzioni sulla connessione [!DNL SharePoint] account a [!DNL Workfront Fusion], vedi <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connetti [!DNL SharePoint] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elenchi]</td> 
   <td> <p>Selezionare la modalità di identificazione del sito da cui si desidera recuperare gli elenchi.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Invio manuale]</strong> </p> <p>Inserisci o mappa il <strong>[!UICONTROL ID sito]</strong>.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleziona dall'elenco]</strong> </p> <p>Selezionare il sito contenente gli elenchi che si desidera recuperare. Il menu a discesa recupera solo i siti che segui.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Immettere o mappare il numero massimo di elenchi che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Elenchi di verifica]

Questo modulo di attivazione avvia uno scenario quando viene creato o modificato un elenco.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL SharePoint] account a [!DNL Workfront Fusion], vedi <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connetti [!DNL SharePoint] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elenchi di controllo]</td> 
   <td>Seleziona se desideri controllare gli elenchi in base all’ora di creazione (nuovi elementi) o di modifica (elementi aggiornati).</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Immetti ID sito ed elenco]</td> 
   <td> <p>Selezionare la modalità di identificazione del sito e dell'elenco che si desidera controllare.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Invio manuale]</strong> </p> <p>Inserisci o mappa il <strong>[!UICONTROL ID sito]</strong> dove si trova l’elenco che desideri controllare.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleziona dall'elenco che segui]</strong> </p> <p>Seleziona il sito da monitorare. L’elenco a discesa recupera solo il sito che segui.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Immettere o mappare il numero massimo di elenchi che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Pagina (Beta)

>[!NOTE]
>
>API in `beta` versione in [!DNL Microsoft Graph] sono soggette a modifiche. L’utilizzo di queste API nelle applicazioni di produzione non è supportato.

#### [!UICONTROL Ottieni una pagina]

Questo modulo di azione restituisce i dati di una pagina specificata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL SharePoint] account a [!DNL Workfront Fusion], vedi <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connetti [!DNL SharePoint] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ottieni pagina]</td> 
   <td> <p>Seleziona la modalità di identificazione della pagina da recuperare.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Invio manuale]</strong> </p> <p>Inserisci o mappa il <strong>[!UICONTROL ID sito]</strong>e <strong>[!UICONTROL ID pagina]</strong>.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleziona dall'elenco]</strong> </p> <p>Seleziona il sito contenente la pagina da recuperare, quindi fai clic sulla pagina.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Sito

* [[!UICONTROL Ottieni un sito]](#get-a-site)
* [[!UICONTROL Cerca siti]](#search-sites)

#### [!UICONTROL Ottieni un sito]

Questo modulo di azione restituisce i dati di un sito specificato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL SharePoint] account a [!DNL Workfront Fusion], vedi <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connetti [!DNL SharePoint] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ottieni sito]</td> 
   <td> <p>Seleziona la modalità di identificazione della pagina da recuperare.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Invio manuale]</strong> </p> <p>Inserisci o mappa il <strong>[!UICONTROL ID sito]</strong>.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleziona dall'elenco]</strong> </p> <p>Seleziona il sito da recuperare.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Cerca siti]

Questo modulo di azione cerca i siti in base a un parametro specificato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL SharePoint] account a [!DNL Workfront Fusion], vedi <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connetti [!DNL SharePoint] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Parola chiave [!UICONTROL del nome visualizzato]</td> 
   <td> <p>Immettere o mappare il termine di ricerca che si desidera cercare nei siti.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Immettere o mappare il numero massimo di siti che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Altro

#### Ottieni modifiche

Questo modulo recupera le aggiunte, gli aggiornamenti e le eliminazioni effettuati nella cartella SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL SharePoint] account a [!DNL Workfront Fusion], vedi <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connetti [!DNL SharePoint] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Immetti ID di sito, unità e cartella]</td> 
   <td> <p>Selezionare la modalità di identificazione del sito e dell'elenco contenente l'elemento che si desidera aggiornare.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Invio manuale]</strong> </p> <p>Inserisci o mappa il <strong>[!UICONTROL ID sito]</strong>, <strong>[!UICONTROL ID unità]</strong>, e <strong>[!UICONTROL ID cartella]</strong> nei campi visualizzati.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleziona dall'elenco]</strong> </p> <p>Selezionare il sito contenente l'elemento che si desidera aggiornare, quindi selezionare l'unità e la cartella. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Token]</td> 
   <td> Il token identifica da quale punto il modulo deve iniziare a recuperare le modifiche.  </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Effettuare una chiamata API]

Questo modulo ti consente di eseguire una chiamata API personalizzata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL SharePoint] account a [!DNL Workfront Fusion], vedi <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connetti [!DNL SharePoint] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Inserisci un percorso relativo a <code>https://graph.microsoft.com</code>. Esempio:<code> /beta/sites</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Method]</p> </td> 
   <td> <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
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
   <td role="rowheader">[!UICONTROL Type]</td> 
   <td>Seleziona il tipo di dati da inviare nella chiamata API.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Aggiungi il contenuto body per la chiamata API sotto forma di oggetto JSON standard.</p> <p>Nota:  <p>Quando si utilizzano istruzioni condizionali quali <code>if</code> nel JSON, inserisci le virgolette al di fuori dell’istruzione condizionale.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### Guarda gli eventi

Questo modulo di attivazione immediata avvia uno scenario quando un elemento viene aggiunto, aggiornato o eliminato in SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
  <!--
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL SharePoint] account to [!DNL Workfront Fusion], see <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  -->
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>Seleziona un webhook esistente oppure fai clic su Aggiungi per crearne uno nuovo.</p> 
   </td> 
  </tr> 
 </tbody> 
</table>

