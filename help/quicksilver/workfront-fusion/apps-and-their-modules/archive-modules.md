---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Moduli di archiviazione
description: In uno scenario  [!DNL Adobe Workfront Fusion] , puoi collegare un archivio, ad esempio un file compresso, a più applicazioni e servizi di terze parti. Ad esempio, puoi configurare uno scenario che
author: Becky
feature: Workfront Fusion
exl-id: e29b6d39-3666-4d6d-a178-1983ae9f3aa9
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 0%

---

# [!UICONTROL Archivia] moduli

In uno scenario [!DNL Adobe Workfront Fusion], è possibile utilizzare un archivio, ad esempio un file compresso, nel proprio scenario, per utilizzarlo nelle automazioni o nelle integrazioni.

Se hai bisogno di istruzioni per la creazione di uno scenario, consulta [Creare uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). Per informazioni sui moduli, vedere [Moduli in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## [!UICONTROL Archivia] moduli e relativi campi

Quando configuri i moduli [!UICONTROL Archivio], [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Insieme a questi, potrebbero essere visualizzati ulteriori campi di [!UICONTROL Archivio], a seconda di fattori quali il livello di accesso nell&#39;app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se viene visualizzato il pulsante Mappa sopra un campo o una funzione, è possibile utilizzarlo per impostare variabili e funzioni per tale campo. Per ulteriori informazioni, vedere [Mappare le informazioni da un modulo all&#39;altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [[!UICONTROL Estrarre un archivio]](#extract-an-archive)
* [[!UICONTROL Crea un archivio]](#create-an-archive)
* [[!UICONTROL Gonfiare]](#inflate)
* [[!UICONTROL Deflazione]](#deflate)

## [!UICONTROL Estrarre un archivio]

Questo modulo estrae un file identificato da un archivio.

Il modulo restituisce l’ID del file e dei campi associati, insieme a eventuali campi e valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Source file]</td> 
   <td> <p> Selezionate il file da estrarre. È possibile mappare questo file da un modulo precedente, ad esempio il modulo [!DNL Workfront] &gt;[!UICONTROL Download a document].</p>  </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Esempio:** Ottieni il file ZIP dalla cartella [!DNL Dropbox] definita (ad esempio, Archivi), estrailo utilizzando il modulo [!UICONTROL Archivio] e invia i file estratti all&#39;indirizzo e-mail desiderato come allegati con il modulo [!UICONTROL E-mail] o [!DNL Gmail].
>
>![](assets/example-dropbox-350x134.png)

## [!UICONTROL Crea un archivio]

Questo modulo aggregatore aggiunge i file desiderati a un archivio [!UICONTROL ZIP] o [!UICONTROL TAR].

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Modulo Source]</td> 
   <td> <p> Selezionare il modulo da cui si desidera recuperare i file.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Type] </td> 
   <td> <p>Seleziona se desideri aggiungere file a un archivio [!UICONTROL ZIP] o a un archivio [!UICONTROL TAR].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Comment]</td> 
   <td>Inserisci un commento da aggiungere all’archivio.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Raggruppa per]</td> 
   <td> <p>Definire un'espressione in base alla quale raggruppare l'output aggregato. Questa espressione può contenere uno o più elementi mappati. I dati aggregati verranno quindi separati in gruppi utilizzando il valore di questa espressione. Ogni gruppo produce come bundle separato con una chiave (l’espressione valutata) e un valore (il testo aggregato). Puoi utilizzare la chiave come filtro nei moduli successivi.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Interrompi elaborazione dopo un'aggregazione vuota]</td> 
   <td>Selezionare questa opzione per interrompere lo scenario quando non sono presenti risultati.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome archivio]</td> 
   <td> <p> Immetti un nome per l’archivio creato. Non aggiungere un'estensione.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source file]</td> 
   <td> <p>Selezionare un file di origine da un modulo precedente o mappare il nome e i dati del file di origine.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Esempio:** controlla le e-mail in arrivo utilizzando il modulo [!DNL Gmail] >[!UICONTROL Controlla e-mail]. Se viene ricevuto un messaggio e-mail, gli allegati vengono iterati in singoli bundle, quindi archiviati nel file [!DNL ZIP] e salvati nella cartella di Dropbox definita.
>
>![](assets/example-gmail-350x102.png)

## [!UICONTROL Gonfiare]

Questo modulo di trasformazione decomprime i dati binari utilizzando un algoritmo di inflazione.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data] </td> 
   <td> <p>Immettere o mappare i dati da decomprimere utilizzando la funzione di gonfiaggio.</p> </td> 
  </tr> 
 </tbody> 
</table>

## [!UICONTROL Deflazione]

Questo modulo di trasformazione comprime i dati binari utilizzando un algoritmo di deflazione.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data] </td> 
   <td> <p>Immettere o mappare i dati da comprimere utilizzando la funzione di deflazione.</p> </td> 
  </tr> 
 </tbody> 
</table>
