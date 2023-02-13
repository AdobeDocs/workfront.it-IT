---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli box
description: In un [!DNL Adobe Workfront Fusion] In questo caso, è possibile automatizzare i flussi di lavoro che utilizzano Box, nonché collegarli a più applicazioni e servizi di terze parti. controlla una cartella specifica per verificare la presenza di modifiche ai file, per modificare ed eliminare i file esistenti o per caricare nuovi file in una cartella.
author: Becky
feature: Workfront Fusion
exl-id: 965ce570-40bf-474d-b318-0d2de8be6b9d
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1022'
ht-degree: 0%

---

# Moduli box

In un [!DNL Adobe Workfront Fusion] puoi automatizzare i flussi di lavoro che utilizzano [!DNL Box], nonché collegarlo a più applicazioni e servizi di terze parti. controlla una cartella specifica per verificare la presenza di modifiche ai file, per modificare ed eliminare i file esistenti o per caricare nuovi file in una cartella.

Se hai bisogno di istruzioni su come creare uno scenario, vedi [Crea uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). Per informazioni sui moduli, consulta [Moduli in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

Per utilizzare [!DNL Box] moduli, è necessario disporre di un [!DNL Box] conto.

## [!DNL Box] moduli e relativi campi

Quando si configura [!DNL Box] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL Box] potrebbero essere visualizzati, a seconda di fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se trovi il pulsante mappa sopra un campo o una funzione, puoi utilizzarlo per impostare variabili e funzioni per quel campo. Per ulteriori informazioni, consulta [Mappare informazioni da un modulo a un altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Triggers

* [[!UICONTROL Nuovo evento]](#new-event)
* [[!UICONTROL File di controllo]](#watch-files)

#### [!UICONTROL Nuovo evento]

Questo modulo di attivazione immediata avvia uno scenario in cui un file viene aggiunto, spostato, copiato, eliminato, bloccato o sbloccato.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>Selezionare il webhook che si desidera utilizzare per guardare i messaggi in uscita. Per aggiungere un webhook, fai clic su <strong>[!UICONTROL Aggiungi]</strong> e inserire il nome e la connessione del webhook.</p> <p> Per istruzioni su come collegare il tuo account [!UICONTROL Box] a [!UICONTROL Workfront Fusion], vedi <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Collega l'app o il servizio Web del modulo a [!UICONTROL Workfront Fusion]</a> nell'articolo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Creare uno scenario in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Numero massimo di eventi restituiti]</p> </td> 
   <td> <p>Immettere il numero massimo di eventi che si desidera venga restituito dal modulo durante ogni ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL File di controllo]

Questo modulo di attivazione avvia uno scenario in cui viene aggiunto un nuovo file o viene aggiornato un file esistente in una cartella controllata.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Per istruzioni su come collegare le [!DNL Box] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  <tr> 
   <td role="rowheader">Guarda</td> 
   <td> <p>Selezionare il tipo di file che si desidera controllare.</p> 
    <ul> 
     <li> <p><strong>Solo nuovi file</strong> </p> <p>Lo scenario inizia quando viene aggiunto un nuovo file.</p> </li> 
     <li> <p><strong>Nuovi file e tutte le modifiche</strong> </p> <p>Lo scenario inizia quando viene aggiunto un file o quando viene modificato il contenuto del file o un attributo di file (ad esempio il nome).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Numero massimo di file scaricati</p> </td> 
   <td> <p>Immetti il numero massimo di file che desideri che il modulo restituisca durante ogni ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Azioni

* [[!UICONTROL Carica] un file](#upload-a-file)
* [[!UICONTROL Aggiornare un file]](#update-a-file)
* [[!UICONTROL Eliminare un file]](#delete-a-file)
* [[!UICONTROL Ottieni un file]](#get-a-file)

#### [!UICONTROL Caricare un file]

Questo modulo di azione carica un file.

Il file viene specificato. Puoi anche fornire un nuovo nome file per il file.

Il modulo restituisce l’ID del file e di tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Box] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File di origine]</td> 
   <td> <p>Selezionare un file di origine da un modulo precedente o mappare il nome e i dati del file di origine.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Se questo modulo non ha esito positivo, considera quanto segue:
>
>* La dimensione del file potrebbe superare il limite massimo di dimensione del file per il tuo [!DNL Box] o potresti aver utilizzato tutti i tuoi [!DNL Box] quota di archiviazione dell&#39;account. Per ottenere più spazio di archiviazione, elimina i file esistenti da [!DNL Box] o aggiornare il [!DNL Box] conto.
>* [!DNL Box] non carica più di un file con lo stesso nome in una singola cartella. Se la cartella di destinazione contiene un file con lo stesso nome del file caricato, l’esecuzione dello scenario termina con un errore. Per evitare questa situazione, rinominare il file. Se desideri aggiornare il file, utilizza il **[!UICONTROL Aggiornare un file]** modulo .


#### [!UICONTROL Aggiornare un file]

Questo modulo di azione aggiorna un file.

Specifica l’ID del file.

Il modulo restituisce l’ID del file e di tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Box] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  <tr> 
   <td role="rowheader">[!UICONTROL File ID]</td> 
   <td>Immetti o mappa l’ID univoco del file che desideri aggiornare nel modulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File di origine]</td> 
   <td> <p>Selezionare un file di origine da un modulo precedente o mappare il nome e i dati del file di origine.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminare un file]

Questo modulo di azione elimina un file.

Specifica l’ID del file.

Il modulo restituisce l’ID del file e di tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Box] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  <tr> 
   <td role="rowheader">[!UICONTROL File ID]</td> 
   <td>Immetti o mappa l’ID univoco del file che desideri aggiornare nel modulo.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottieni un file]

Questo modulo di azione scarica un file.

Specifica l’ID del file.

Il modulo restituisce l’ID del file e di tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

>[!NOTE]
>
>Questo modulo è utile per fornire file ai moduli successivi.

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Box] account a [!DNL Workfront Fusion], vedi <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Creare una connessione a [!DNL Adobe Workfront Fusion] - Istruzioni di base</a></p> </td> 
  <tr> 
   <td role="rowheader">[!UICONTROL File ID]</td> 
   <td>Immetti o mappa l’ID univoco del file che desideri aggiornare nel modulo.</td> 
  </tr> 
 </tbody> 
</table>

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Possible problems</h2>
-->

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">This is drafted out because we don't have a download module for Box yet</p>
-->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode">Watch files trigger module doesn't download a file contained in the folder.</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">There are several situations when downloading a file fails:</p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">The current file lock setting does not allow the file to be downloaded or the downloading of the file is disabled. In this case, the file is ignored.</li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">When the scenario started, the file was being uploaded to the server and was not ready to be downloaded. The scenario run gets stopped and Workfront Fusion tries downloading the file again during the next execution of the scenario.</li>
  -->
