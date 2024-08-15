---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Visualizzare la cronologia di esecuzione di uno scenario in Adobe Workfront Fusion
description: È possibile visualizzare informazioni su tutte le esecuzioni di uno scenario oppure cercare dati specifici in tutte le esecuzioni dello scenario.
author: Becky
feature: Workfront Fusion
exl-id: cc2c3f87-34dc-4a06-9f5f-1a7fb10a3b82
source-git-commit: 1b729960a23e43252bda16d9bfb7ca9656a115a1
workflow-type: tm+mt
source-wordcount: '958'
ht-degree: 0%

---

# Visualizzare la cronologia di esecuzione di uno scenario in [!DNL Adobe Workfront Fusion]

È possibile visualizzare informazioni su tutte le esecuzioni di uno scenario oppure cercare dati specifici in tutte le esecuzioni dello scenario.

La cronologia di esecuzione di uno scenario visualizza tutte le esecuzioni dello scenario negli ultimi 30 giorni.

## Requisiti di accesso

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto">  
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] piano*</td> 
   <td> <p>[!DNL Pro] o superiore</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza [!UICONTROL Adobe Workfront Fusion]**</td> 
  <td>
   <p>Requisiti di licenza correnti: nessun requisito di licenza [!DNL Workfront Fusion].</p>
   <p>Oppure</p>
   <p>Requisito licenza legacy: [!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione lavoro], [!UICONTROL [!DNL Workfront Fusion] per automazione lavoro]</p>
   </td>  
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>
   <p>Fabbisogno prodotto corrente: se si dispone del piano [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront], l'organizzazione deve acquistare [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo. [!DNL Workfront Fusion] è incluso nel piano [!UICONTROL Ultimate] [!DNL Workfront].</p>
   <p>Oppure</p>
   <p>Requisiti del prodotto legacy: la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Per conoscere il piano, il tipo di licenza o l&#39;accesso disponibili, contattare l&#39;amministratore [!DNL Workfront].

Per informazioni sulle [!DNL Adobe Workfront Fusion] licenze, vedere [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Visualizzare tutte le esecuzioni di uno scenario

### Visualizza la cronologia di esecuzione dello scenario nella pagina [!UICONTROL Dettagli scenario]

1. Fai clic sulla scheda **[!UICONTROL Scenario]** nel pannello a sinistra, quindi fai clic sullo scenario.

   Oppure

   Se si sta lavorando sullo scenario nell&#39;editor scenari, fare clic sulla freccia sinistra ![](assets/exit-editing-arrow.png) nell&#39;angolo superiore sinistro della finestra.

1. Visualizzare le informazioni nell&#39;elenco a destra.

   Puoi anche fare clic su per visualizzare una pagina intera di queste informazioni. La visualizzazione a pagina intera consente di filtrare la cronologia per visualizzare esecuzioni specifiche.

   Per ogni esecuzione dello scenario sono elencati i seguenti dettagli:

   * Data in cui è stata **[!UICONTROL avviata]**
   * **[!UICONTROL Stato]** (operazione riuscita o non riuscita)
   * Esegui **[!UICONTROL Durata]**
   * Numero di **[!UICONTROL operazioni]**
   * Dimensione di **[!UICONTROL Trasferimento dati]**
   * Collega a **[!UICONTROL Dettagli]**

>[!NOTE]
>
>Nella cronologia degli scenari viene visualizzato un contrassegno **Elaborazione** accanto agli scenari eseguiti di recente, mentre i dettagli di esecuzione vengono scritti nell&#39;archivio. L’elaborazione si verifica immediatamente dopo l’esecuzione dello scenario. e non dovrebbe durare più di qualche minuto. I dettagli dell’esecuzione dello scenario potrebbero non essere visibili durante l’elaborazione dell’esecuzione.

### Visualizza la cronologia di esecuzione dello scenario nella scheda [!UICONTROL Cronologia]

La scheda [!UICONTROL Cronologia] mostra più dettagli di quelli disponibili nella pagina [!UICONTROL Dettagli scenario]. Puoi anche filtrare e ordinare le esecuzioni nella scheda [!UICONTROL Cronologia].

1. Fai clic sulla scheda **[!UICONTROL Scenario]** nel pannello a sinistra, quindi fai clic sullo scenario.

   Oppure

   Se si sta lavorando sullo scenario nell&#39;editor scenari, fare clic sulla freccia sinistra ![](assets/exit-editing-arrow.png) nell&#39;angolo superiore sinistro della finestra.

1. Fai clic sulla scheda **[!UICONTROL Cronologia]** nell&#39;angolo superiore sinistro della pagina
1. (Facoltativo) Per informazioni dettagliate sull&#39;esecuzione di uno scenario selezionato, inclusi i bundle elaborati, fai clic sul collegamento **[!UICONTROL Dettagli]**.

   Per ulteriori informazioni sull&#39;elaborazione dei bundle, vedere [Flusso di esecuzione dello scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).

   >[!NOTE]
   >
   >* Il collegamento [!UICONTROL details] è visibile solo se sono disponibili dettagli sull&#39;esecuzione.
   >
   >* La cronologia degli scenari visualizza un contrassegno **Cronologia elaborazione** accanto agli scenari eseguiti di recente, mentre i dettagli di esecuzione vengono scritti nell&#39;archivio. L’elaborazione si verifica immediatamente dopo l’esecuzione dello scenario. e non dovrebbe durare più di qualche minuto. I dettagli dell’esecuzione dello scenario potrebbero non essere visibili durante l’elaborazione dell’esecuzione.

## Filtrare la cronologia di esecuzione dello scenario

Puoi filtrare la cronologia di esecuzione per visualizzare solo le esecuzioni con i valori specificati.

1. Aprire la cronologia a pagina intera per uno scenario come descritto in [Visualizzare la cronologia di esecuzione dello scenario nella scheda [!UICONTROL Cronologia]](#view-scenario-execution-history-on-the-history-tab) in questo articolo.
1. Fai clic sull&#39;icona [!UICONTROL filter] ![](assets/fusion-scenario-filter-icon.png) nell&#39;intestazione della colonna in base alla quale desideri filtrare.
1. Nella finestra di dialogo [!UICONTROL filter], immetti i valori in base ai quali desideri filtrare.
1. Fai clic su **[!UICONTROL Salva]**.

L’icona del filtro è arancione nelle colonne con un filtro attualmente attivo.

## Ordinare la cronologia di esecuzione dello scenario

Puoi ordinare la cronologia di esecuzione dello scenario.

1. Aprire la cronologia a pagina intera per uno scenario come descritto in [Visualizzare la cronologia di esecuzione dello scenario nella scheda [!UICONTROL Cronologia]](#view-scenario-execution-history-on-the-history-tab) in questo articolo.
1. Fai clic sull&#39;icona [!UICONTROL Ordina] nell&#39;intestazione della colonna in base alla quale desideri filtrare.
1. Facoltativo: per invertire l&#39;ordine, fare di nuovo clic sull&#39;icona [!UICONTROL Ordina].

## Cercare tutte le esecuzioni di uno scenario

1. Fai clic sull&#39;icona **[!UICONTROL Scenario]** ![](assets/scenarios-icon.png) nel pannello a sinistra, quindi fai clic sullo scenario.

   Oppure

   Se si sta lavorando sullo scenario nell&#39;editor scenari, fare clic sulla freccia sinistra ![](assets/exit-editing-arrow.png) nell&#39;angolo superiore sinistro della finestra.

1. Fai clic sulla scheda **[!UICONTROL Cronologia]** nell&#39;angolo superiore sinistro dello schermo.
1. Fai clic su **[!UICONTROL Ricerca full-text]** in alto nell&#39;elenco delle esecuzioni.

   Oppure

   Digitare **Ctrl+Maiusc+F** (Windows) o **Cmd+Maiusc+F** (Mac)
Viene visualizzata la finestra [!UICONTROL Cerca nella cronologia].

1. (Facoltativo) Per cercare esecuzioni contenenti testo specifico, immettere il testo nella barra di ricerca della finestra **[!UICONTROL Cerca nella cronologia]**.

   Per cercare il testo esatto, racchiuderlo tra virgolette doppie (&quot;esempio&quot;).

   >[!INFO]
   >
   >**Esempio:** Se desideri trovare l&#39;esecuzione che ha creato un progetto specifico, immetti l&#39;ID del progetto nella barra di [!UICONTROL Ricerca full-text].
   >
   >&quot;625ef2ef0006036bd1794b6e52d737c5&quot;

1. (Facoltativo) Per limitare la ricerca in base all&#39;intervallo di date, selezionare le date di inizio e fine della ricerca desiderata nell&#39;area [!UICONTROL Per intervallo di date].

   >[!NOTE]
   >
   >* Le esecuzioni sono disponibili solo per i 30 giorni precedenti.
   >
   >* [!DNL Workfront Fusion] memorizza i payload del webhook per 30 giorni. L&#39;accesso a un payload del webhook dopo più di 30 giorni dalla creazione genera l&#39;errore &quot;[!UICONTROL Impossibile leggere il file dall&#39;archivio.]&quot;


1. (Facoltativo) Per limitare la ricerca in base allo stato, seleziona lo stato desiderato nel menu a discesa **[!UICONTROL Per stato]**.


   Gli stati disponibili sono:

   * [!UICONTROL Tutti]

   * [!UICONTROL Errore]

   * [!UICONTROL Avviso]

   * [!UICONTROL Operazione completata]

1. (Facoltativo) Modifica l&#39;ordine di visualizzazione dei risultati nel menu a discesa **[!UICONTROL Ordina per date]**.

1. (Facoltativo) Per copiare un ID di esecuzione dello scenario, fai clic sull&#39;icona **[!UICONTROL Copia ID esecuzione]** <img src="assets/copy-fusion-execution-id-icon.png"> nella riga dell&#39;esecuzione desiderata

1. (Facoltativo) Fai clic su un risultato della [!UICONTROL ricerca full-text] per esaminare il bundle di output del modulo scenario contenente le informazioni.
