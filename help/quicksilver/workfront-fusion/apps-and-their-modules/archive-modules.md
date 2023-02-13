---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Moduli di archiviazione
description: In una [!DNL Adobe Workfront Fusion] In questo caso, è possibile collegare un archivio, ad esempio un file zip, a più applicazioni e servizi di terze parti. Ad esempio, puoi configurare uno scenario che
author: Becky
feature: Workfront Fusion
exl-id: e29b6d39-3666-4d6d-a178-1983ae9f3aa9
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 0%

---

# [!UICONTROL Archivia] moduli

In una [!DNL Adobe Workfront Fusion] in uno scenario, puoi utilizzare un archivio, ad esempio un file zip, per utilizzarlo nelle tue automatizzazioni o integrazioni.

Se hai bisogno di istruzioni su come creare uno scenario, vedi [Crea uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). Per informazioni sui moduli, consulta [Moduli in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## [!UICONTROL Archivia] moduli e relativi campi

Quando si configura [!UICONTROL Archivia] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!UICONTROL Archivia] potrebbero essere visualizzati, a seconda di fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se trovi il pulsante mappa sopra un campo o una funzione, puoi utilizzarlo per impostare variabili e funzioni per quel campo. Per ulteriori informazioni, consulta [Mappare informazioni da un modulo a un altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [[!UICONTROL Estrarre un archivio]](#extract-an-archive)
* [[!UICONTROL Creare un archivio]](#create-an-archive)
* [[!UICONTROL gonfiare]](#inflate)
* [[!UICONTROL Deflazione]](#deflate)

## [!UICONTROL Estrarre un archivio]

Questo modulo di azione estrae un file identificato da un archivio.

Il modulo restituisce l’ID del file e di tutti i campi associati, insieme a eventuali campi e valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL File di origine]</td> 
   <td> <p> Selezionare il file da estrarre. Questo file può essere mappato da un modulo precedente (ad esempio [!DNL Workfront] &gt;[!UICONTROL Scarica un modulo di documento]).</p>  </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Esempio:** Ottenere il file ZIP dal definito [!DNL Dropbox] cartella (ad esempio, Archives), estrarla utilizzando il [!UICONTROL Archivia] e invia i file estratti all&#39;indirizzo e-mail desiderato come allegati con [!UICONTROL E-mail] o [!DNL Gmail] modulo .
>
>![](assets/example-dropbox-350x134.png)

## [!UICONTROL Creare un archivio]

Questo modulo aggregatore aggiunge i file desiderati a un [!UICONTROL ZIP] o [!UICONTROL TAR] archivio.

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Modulo di origine]</td> 
   <td> <p> Selezionare il modulo da cui si desidera recuperare i file.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Type] </td> 
   <td> <p>Seleziona se desideri aggiungere file a un archivio ZIP o a un archivio TAR.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Commento]</td> 
   <td>Inserisci un commento da aggiungere all’archivio.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Group by]</td> 
   <td> <p>Definire un’espressione per la quale si desidera raggruppare l’output aggregato. Questa espressione può contenere uno o più elementi mappati. I dati aggregati saranno quindi separati in gruppi utilizzando il valore di questa espressione. Ogni gruppo produce come bundle separato con una chiave (l'espressione valutata) e un valore (il testo aggregato). Puoi utilizzare la chiave come filtro nei moduli successivi.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Interrompe l'elaborazione dopo un'aggregazione vuota]</td> 
   <td>Selezionare questa opzione per interrompere lo scenario in assenza di risultati.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome archivio]</td> 
   <td> <p> Immettere un nome per l'archivio creato. Non aggiungere un'estensione.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File di origine]</td> 
   <td> <p>Selezionare un file di origine da un modulo precedente o mappare il nome e i dati del file di origine.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Esempio:** Osserva le e-mail in arrivo utilizzando [!DNL Gmail] >[!UICONTROL Guarda le e-mail] modulo . Se viene ricevuta un’e-mail, i relativi allegati vengono iterati in singoli bundle e quindi archiviati nel [!DNL ZIP] e salvati nella cartella di Dropbox definita.
>
>![](assets/example-gmail-350x102.png)

## [!UICONTROL gonfiare]

Questo modulo di trasformazione decomprime i dati binari utilizzando un algoritmo di inflazione.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data] </td> 
   <td> <p>Immetti o mappa i dati da decomprimere utilizzando la funzione gonfiare.</p> </td> 
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
   <td> <p>Immettere o mappare i dati che si desidera comprimere utilizzando la funzione deflate.</p> </td> 
  </tr> 
 </tbody> 
</table>
