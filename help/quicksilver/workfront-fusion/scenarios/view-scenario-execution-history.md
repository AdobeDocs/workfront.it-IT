---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Visualizzare la cronologia di esecuzione di uno scenario in Adobe Workfront Fusion
description: È possibile visualizzare informazioni su tutte le esecuzioni di uno scenario oppure cercare dati specifici in tutte le esecuzioni dello scenario.
author: Becky
feature: Workfront Fusion
exl-id: cc2c3f87-34dc-4a06-9f5f-1a7fb10a3b82
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '856'
ht-degree: 1%

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
   <p>Fabbisogno di licenza corrente: No [!DNL Workfront Fusion] requisito di licenza.</p>
   <p>Oppure</p>
   <p>Requisito licenza legacy: [!UICONTROL [!DNL Workfront Fusion] per l'automazione e l'integrazione del lavoro], [!UICONTROL [!DNL Workfront Fusion] per automazione lavoro]</p>
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

## Visualizzare tutte le esecuzioni di uno scenario

### Visualizzare la cronologia di esecuzione dello scenario in [!UICONTROL Dettagli scenario] pagina

1. Fai clic su **[!UICONTROL Scenario]** nel pannello a sinistra, quindi fai clic sullo scenario.

   Oppure

   Se stai lavorando sullo scenario nell’editor scenario, fai clic sulla freccia sinistra ![](assets/exit-editing-arrow.png) nell&#39;angolo superiore sinistro della finestra.

1. Visualizzare le informazioni nell&#39;elenco a destra.

   ![](assets/open-history-tab-350x202.png)

   Clr

   Puoi anche fare clic su per visualizzare una pagina intera di queste informazioni. La visualizzazione a pagina intera consente di filtrare la cronologia per visualizzare esecuzioni specifiche.

   Per ogni esecuzione dello scenario sono elencati i seguenti dettagli:

   * Data in cui è stata eseguita **[!UICONTROL Avviato]**
   * **[!UICONTROL Stato]** (operazione riuscita o non riuscita)
   * Esegui **[!UICONTROL Durata]**
   * Numero di **[!UICONTROL Operazioni]**
   * Dimensione di **[!UICONTROL Trasferimento dati]**
   * Collega a **[!UICONTROL Dettagli]**

### Visualizzare la cronologia di esecuzione dello scenario in [!UICONTROL Cronologia] scheda

Il [!UICONTROL Cronologia] La scheda mostra più dettagli di quanto non sia disponibile nella [!UICONTROL Dettagli scenario] pagina. Puoi anche filtrare e ordinare le esecuzioni sulla [!UICONTROL Cronologia] scheda.

1. Fai clic su **[!UICONTROL Scenario]** nel pannello a sinistra, quindi fai clic sullo scenario.

   Oppure

   Se stai lavorando sullo scenario nell’editor scenario, fai clic sulla freccia sinistra ![](assets/exit-editing-arrow.png) nell&#39;angolo superiore sinistro della finestra.

1. Fai clic su **[!UICONTROL Cronologia]** Scheda vicino all’angolo superiore sinistro della pagina
1. (Facoltativo) Per informazioni dettagliate su un’esecuzione dello scenario selezionato, compresi i bundle elaborati, fai clic su **[!UICONTROL Dettagli]** collegamento.

   Per ulteriori informazioni sull’elaborazione dei bundle, consulta [Flusso di esecuzione dello scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).

   >[!NOTE]
   >
   >Il [!UICONTROL dettagli] il collegamento è visibile solo se sono disponibili i dettagli dell’esecuzione.

## Filtrare la cronologia di esecuzione dello scenario

Puoi filtrare la cronologia di esecuzione per visualizzare solo le esecuzioni con i valori specificati.

1. Aprire la cronologia dell&#39;intera pagina per uno scenario come descritto in [Visualizzare la cronologia di esecuzione dello scenario in [!UICONTROL Cronologia] scheda](#view-scenario-execution-history-on-the-history-tab) in questo articolo.
1. Fai clic su [!UICONTROL filter] icona ![](assets/fusion-scenario-filter-icon.png) nell’intestazione della colonna in base alla quale desideri filtrare.
1. In [!UICONTROL filter] , immetti i valori in base ai quali desideri filtrare.
1. Fai clic su **[!UICONTROL Salva]**.

L’icona del filtro è arancione nelle colonne con un filtro attualmente attivo.

## Ordinare la cronologia di esecuzione dello scenario

Puoi ordinare la cronologia di esecuzione dello scenario.

1. Aprire la cronologia dell&#39;intera pagina per uno scenario come descritto in [Visualizzare la cronologia di esecuzione dello scenario in [!UICONTROL Cronologia] scheda](#view-scenario-execution-history-on-the-history-tab) in questo articolo.
1. Fai clic su [!UICONTROL Ordina] nell’intestazione della colonna in base alla quale desideri filtrare.
1. Facoltativo: per invertire l&#39;ordine, fare clic sul pulsante [!UICONTROL Ordina] di nuovo.

## Cercare tutte le esecuzioni di uno scenario

1. Fai clic su **[!UICONTROL Scenario]** icona ![](assets/scenarios-icon.png) nel pannello a sinistra, fai clic sullo scenario.

   Oppure

   Se stai lavorando sullo scenario nell’editor scenario, fai clic sulla freccia sinistra ![](assets/exit-editing-arrow.png) nell&#39;angolo superiore sinistro della finestra.

1. Fai clic su **[!UICONTROL Cronologia]** nell&#39;angolo superiore sinistro dello schermo.
1. Clic **[!UICONTROL Ricerca full-text]** in cima all’elenco delle esecuzioni.

   Oppure

   Tipo **Ctrl+Maiusc+F** (Windows) o **Cmd+Maiusc+F** (Mac) Il [!UICONTROL Cerca nella cronologia] viene visualizzata la finestra.

1. (Facoltativo) Per cercare esecuzioni che contengono testo specifico, inserisci il testo nella barra di ricerca del **[!UICONTROL Cerca nella cronologia]** finestra.

   Per cercare il testo esatto, racchiuderlo tra virgolette doppie (&quot;esempio&quot;).

   >[!INFO]
   >
   >**Esempio:** Se desideri trovare l’esecuzione che ha creato un progetto specifico, inserisci l’ID progetto in [!UICONTROL Ricerca full-text] barra.
   >
   >&quot;625ef2ef0006036bd1794b6e52d737c5&quot;

1. (Facoltativo) Per limitare la ricerca in base all’intervallo di date, seleziona le date di inizio e fine della ricerca desiderata in [!UICONTROL Per intervallo di date] area.

   >[!NOTE]
   >
   >* Le esecuzioni sono disponibili solo per i 30 giorni precedenti.
   >
   >* [!DNL Workfront Fusion] memorizza i payload del webhook per 30 giorni. Se si accede a un payload del webhook più di 30 giorni dopo la sua creazione, viene generato l’errore &quot;[!UICONTROL Impossibile leggere il file dall&#39;archivio.]&quot;


1. (Facoltativo) Per limitare la ricerca in base allo stato, seleziona lo stato desiderato nella sezione **[!UICONTROL Per stato]** a discesa.


   Gli stati disponibili sono:

   * [!UICONTROL Tutti]

   * [!UICONTROL Errore]

   * [!UICONTROL Avvertenza]

   * [!UICONTROL Operazione completata]

1. (Facoltativo) Modifica l’ordine di visualizzazione dei risultati in **[!UICONTROL Ordina per date]** a discesa.

1. (Facoltativo) Per copiare un ID di esecuzione di uno scenario, fai clic sul pulsante **[!UICONTROL Copia ID esecuzione]** icona <img src="assets/copy-fusion-execution-id-icon.png"> nella riga dell’esecuzione desiderata

1. (Facoltativo) Fai clic su un risultato del [!UICONTROL Ricerca full-text] per esaminare il bundle di output del modulo scenario contenente le informazioni.
