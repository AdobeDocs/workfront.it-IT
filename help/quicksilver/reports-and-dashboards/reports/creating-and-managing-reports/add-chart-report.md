---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Aggiungere un grafico a un report
description: Puoi migliorare i rapporti aggiungendo un grafico. È possibile aggiungere grafici ai rapporti esistenti o ai rapporti che si stanno creando.
author: Nolan
feature: Reports and Dashboards
exl-id: 9b58d68c-4b7b-4344-bde3-7c65e2e1aac8
source-git-commit: 84c5772d130be78d9f9b9aef342c57183d5ec985
workflow-type: tm+mt
source-wordcount: '2768'
ht-degree: 0%

---

# Aggiungere un grafico a un report

<!--Audited: 01/2024-->

Puoi migliorare i rapporti aggiungendo un grafico. È possibile aggiungere grafici ai rapporti esistenti o ai rapporti che si stanno creando.

Prima di aggiungere un grafico a un report, è necessario creare una visualizzazione e un raggruppamento per il report.

Non è possibile aggiungere grafici alla maggior parte dei rapporti a meno che non si raggruppino prima le informazioni nel rapporto. L&#39;unico grafico che può essere aggiunto senza raggruppamento è un grafico a contatori.

Per informazioni sulle visualizzazioni, vedere [Panoramica delle visualizzazioni in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

Per ulteriori informazioni sui raggruppamenti, vedere [Panoramica sui raggruppamenti in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

Se nel report vengono visualizzati troppi elementi, non viene creato un grafico. In questo caso, devi anche aggiungere un filtro al rapporto per ridurre il numero di risultati.

Per ulteriori informazioni sui filtri, vedere [Panoramica sui filtri](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Corrente: Piano </p>
   Oppure
   <p>Nuovo: Standard</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazione del livello di accesso</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari</p> <p>Modifica accesso a Filtri, Viste, Raggruppamenti</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p>  </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront. Per ulteriori informazioni sui requisiti di accesso, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Aggiungere un grafico a un report

1. Passa a un rapporto esistente o creane uno nuovo. Per ulteriori informazioni sulla creazione di un nuovo report, vedere [Creare un report personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. (Condizionale) Se hai scelto un report esistente, fai clic su **Azioni report** > **Modifica**.

1. Verificare che la scheda **Colonne (visualizzazione)** sia stata aggiornata per visualizzare le informazioni che si desidera tracciare nel report.

   Per informazioni su come creare o modificare la visualizzazione per il report, vedere [Creare o modificare le visualizzazioni in Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

1. Fai clic sulla scheda **Raggruppamenti** e aggiungi un raggruppamento.

   >[!TIP]
   >
   >* È possibile aggiungere un grafico a un report solo quando i risultati sono raggruppati.
   >* I raggruppamenti in modalità testo non sono supportati nei grafici. Per ulteriori informazioni sui raggruppamenti in modalità testo, vedere [Modificare la modalità testo in un raggruppamento](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-grouping.md).
   >* Se aggiungi un singolo raggruppamento che rappresenta una metrica, tutti i grafici eccetto un grafico a torta visualizzano ciascuno come risultato del raggruppamento dello stesso colore.

   Per ulteriori informazioni sulla creazione di raggruppamenti, vedere [Creare raggruppamenti in Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-groupings.md).

1. Selezionare la scheda **Grafico**.
1. Fare clic su un tipo di grafico per selezionarlo.\
   ![](assets/qs-report-builder-chart-350x265.png)

1. Selezionare uno dei seguenti tipi di grafici:

   * [Istogramma](#column-chart)
   * [Grafico a barre](#bar-chart)
   * [Grafico a torta](#pie-chart)
   * [Grafico a linee](#line-chart)
   * [Grafico a barre](#gauge-chart)
   * [Grafico a bolle](#bubble-chart)

1. Fai clic su **Salva + Chiudi** per salvare il grafico e il report.

### Istogramma {#column-chart}

Per aggiungere un grafico **Colonna** al report:

1. Inizia ad aggiungere un grafico al tuo report, come descritto in [Aggiungi un grafico a un report](#add-a-chart-to-a-report).
1. Nel campo **Asse sinistro**, selezionare i valori che si desidera includere sull&#39;asse Y del grafico, nonché la modalità di riepilogo delle informazioni.
1. Nel campo **Asse inferiore (X)** selezionare il raggruppamento che si desidera includere nel grafico.
1. (Facoltativo) Seleziona **Colori personalizzati** per assegnare i colori preferiti a ciascuna colonna.\
   Per ulteriori informazioni sulla personalizzazione dei colori dei grafici, vedere [Personalizzare i colori dei grafici](#customize-chart-colors).

1. (Facoltativo) Selezionare **Mostra in 3D** per visualizzare il grafico in una visualizzazione tridimensionale.
1. (Facoltativo) **Raggruppa colonne**: selezionare questa opzione per definire la modalità di raggruppamento delle colonne.\
   Selezionare una delle opzioni seguenti:

   * Fare clic su una delle opzioni seguenti per selezionare la modalità di visualizzazione delle colonne raggruppate:

      * **Affiancati**
      * **In pila**
      * **Sovrapposizione al 100%**

   * Selezionare il raggruppamento che si desidera includere nel grafico dal menu a discesa **Raggruppa dati per**.
   * (Facoltativo) Seleziona **Colori personalizzati** per personalizzare i colori delle colonne.\
     Per ulteriori informazioni sulla personalizzazione dei colori dei grafici, vedere [Personalizzare i colori dei grafici](#customize-chart-colors).

1. (Facoltativo) Selezionare **Grafico combinato** per includere un valore aggiuntivo nel grafico, nonché la modalità di riepilogo delle informazioni.\
   Considera le seguenti opzioni:

   * **Traccia sull&#39;asse secondario**: selezionare questa opzione per tracciare i dati sul lato destro del grafico.
   * **Tipo di grafico**: selezionare se si desidera che questo valore aggiuntivo venga visualizzato come una riga o una terza colonna.\
     ![](assets/qs-column-chart-350x163.png)

1. Fai clic su **Salva + Chiudi** per salvare il grafico e il report.

### Grafico a barre {#bar-chart}

Per aggiungere un grafico a **barre** al report:

1. Inizia ad aggiungere un grafico al tuo report, come descritto in [Aggiungi un grafico a un report](#add-a-chart-to-a-report).
1. Nel campo **Asse inferiore (X)**, selezionare i valori che si desidera includere sull&#39;asse X del grafico, nonché la modalità di riepilogo delle informazioni.
1. Nel campo **Asse sinistro** selezionare il raggruppamento che si desidera includere nel grafico.
1. (Facoltativo) Seleziona **Colori personalizzati** per personalizzare i colori delle barre.\
   Per ulteriori informazioni sulla personalizzazione dei colori dei grafici, vedere [Personalizzare i colori dei grafici](#customize-chart-colors).

1. (Facoltativo) Selezionare **Mostra in 3D** per visualizzare il grafico in una visualizzazione tridimensionale.
1. (Facoltativo) Seleziona **Raggruppa barre** per definire la modalità di raggruppamento delle barre.\
   Selezionare una delle opzioni seguenti:

   * Fare clic su una delle opzioni seguenti per selezionare la modalità di visualizzazione delle barre raggruppate:

      * **Affiancati**
      * **In pila**
      * **Sovrapposizione al 100%**

   * Selezionare la modalità di raggruppamento delle informazioni nel grafico dal menu a discesa **Raggruppa dati per**.
   * (Facoltativo) Seleziona **Colori personalizzati** per personalizzare i colori delle colonne.\
     Per ulteriori informazioni sulla personalizzazione dei colori dei grafici, vedere [Personalizzare i colori dei grafici](#customize-chart-colors).

1. (Facoltativo) Selezionare **Grafico combinato** per includere un valore aggiuntivo nel grafico, nonché la modalità di riepilogo delle informazioni.\
   ![](assets/qs-bar-chart-350x167.png)

1. Fai clic su **Salva + Chiudi** per salvare il grafico e il report.

>[!IMPORTANT]
>
>Limitare i grafici a barre a un massimo di 23 barre, poiché i grafici a barre che includono più di 23 barre non visualizzano correttamente tutte le etichette delle barre.

### Grafico a torta {#pie-chart}

Per aggiungere un grafico **Torta** al report:

1. Inizia ad aggiungere un grafico al tuo report, come descritto in [Aggiungi un grafico a un report](#add-a-chart-to-a-report).
1. Nel campo **Valori** selezionare i valori che si desidera visualizzare nel report e la modalità di riepilogo.\
   Nel campo **Cunei** selezionare il raggruppamento che si desidera includere nel grafico. Il raggruppamento è rappresentato dai cunei del grafico.

1. (Facoltativo) Seleziona **Colori personalizzati** per personalizzare i colori dei cunei nel grafico.\
   Per ulteriori informazioni sulla personalizzazione dei colori dei grafici, vedere [Personalizzare i colori dei grafici](#customize-chart-colors).

1. (Facoltativo) Selezionare **Mostra in 3D** per visualizzare il grafico in una visualizzazione tridimensionale.
1. Nel campo **Mostra risultati come**, selezionare la modalità di visualizzazione dei risultati nel grafico. Considera le seguenti opzioni:

   * **Percentuale**: i risultati del grafico vengono visualizzati come percentuale.
   * **Numeri**: i risultati del grafico vengono visualizzati sotto forma di numero.\
     ![](assets/qs-pie-chart-350x171.png)

1. Fai clic su **Salva + Chiudi** per salvare il grafico e il report.

### Grafico a linee {#line-chart}

Per aggiungere un grafico **Line** al report:

1. Inizia ad aggiungere un grafico al tuo report, come descritto in [Aggiungi un grafico a un report](#add-a-chart-to-a-report).
1. Nel campo **Asse sinistro**, selezionare i valori che si desidera includere sull&#39;asse Y del grafico, nonché la modalità di riepilogo delle informazioni.
1. Nel campo **Asse inferiore (X)** selezionare il raggruppamento che si desidera includere nel grafico.
1. (Facoltativo) Selezionate un colore per personalizzare il colore della linea.
1. (Facoltativo) Selezionare **Raggruppa righe** per selezionare un raggruppamento aggiuntivo per il grafico.\
   (Facoltativo) Seleziona **Colori personalizzati** per personalizzare i colori del nuovo raggruppamento.\
   Per ulteriori informazioni sulla personalizzazione dei colori dei grafici, vedere [Personalizzare i colori dei grafici](#customize-chart-colors).

1. (Facoltativo) Selezionare **Grafico combinato** per combinare le righe di un valore aggiuntivo.\
   Considera tra le seguenti opzioni:

   * Selezionare il valore che si desidera includere nel grafico, nonché la modalità di riepilogo delle informazioni.
   * Selezionare il campo **Traccia sull&#39;asse secondario** per tracciare i dati sul lato destro del grafico.\
     ![](assets/qs-line-chart-350x172.png)

1. Fai clic su **Salva + Chiudi** per salvare il grafico e il report.

### Grafico a barre {#gauge-chart}

Un grafico **Misuratore** visualizza il numero di record che soddisfano determinati criteri in un formato di contatore. L&#39;indicatore del contatore punta al numero di record che soddisfano i criteri selezionati nella visualizzazione e nel raggruppamento del report. Non è necessario un raggruppamento di rapporti per configurare un grafico a contatori.

Per aggiungere un grafico **Misuratore** al report:

1. Inizia ad aggiungere un grafico al tuo report, come descritto in [Aggiungi un grafico a un report](#add-a-chart-to-a-report).
1. Nel campo **Valori** selezionare i valori che si desidera visualizzare nel report e la modalità di riepilogo. Se si seleziona **Conteggio record**, i valori visualizzati sono l&#39;oggetto del report.

1. Nel campo **Indicatori** selezionare il raggruppamento che si desidera includere nel grafico. Il Raggruppamento è rappresentato dalla linea dell&#39;indicatore nel grafico.\
   Se si dispone di un raggruppamento che contiene due elementi, nel grafico vengono visualizzati due indicatori.\
   Ad esempio, se si dispone di un raggruppamento dello stato del progetto e sono presenti due stati del progetto (Corrente e In sospeso), il grafico Misuratore contiene due indicatori di contatore. Indicheranno il numero di progetti che si trovano in quello stato.\
   (Facoltativo) Seleziona **Totale** nel campo **Indicatori** per visualizzare il totale degli oggetti selezionati nel campo **Valori**.

1. Nel campo **Intervallo di valori**, specificare l&#39;intervallo di valori e il colore per rappresentare tali valori da visualizzare nel grafico Misuratore.
1. (Facoltativo) Fai clic su **Aggiungi un altro intervallo di valori** per aggiungere ulteriori intervalli di valori al grafico.\
   ![](assets/qs-gauge-chart-350x181.png)

1. Fai clic su **Salva + Chiudi** per salvare il grafico e il report.

### Grafico a bolle {#bubble-chart}

È possibile visualizzare fino a tre campi di un oggetto in un grafico **A bolle**. Ciò significa che è possibile visualizzare fino a quattro punti dati in un grafico a bolle. Ogni entità con tre campi associati viene visualizzata come un cerchio che esprime due dei campi all&#39;interno della sua posizione all&#39;interno degli assi X e Y. Il terzo campo è rappresentato dalla dimensione del cerchio.

Per aggiungere un grafico a **bolle** al report:

1. Inizia ad aggiungere un grafico al tuo report, come descritto in [Aggiungi un grafico a un report](#add-a-chart-to-a-report).
1. Nel campo **Asse sinistro**, selezionare i valori che si desidera includere sull&#39;asse Y del grafico. I valori provengono dalla vista del rapporto. Specificare la modalità di riepilogo delle informazioni.
1. Nel campo **Asse inferiore (X)**, selezionare i valori che si desidera includere sull&#39;asse X del grafico. I valori provengono dalla vista del rapporto. Specificare la modalità di riepilogo delle informazioni.

   >[!NOTE]
   >
   >Assicurati di disporre di almeno una colonna riepilogata per attivare questo campo.\
   >Per ulteriori informazioni sul riepilogo delle informazioni nella colonna di un report, vedere [Creare un report personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Nel campo **Dimensioni bolle**, selezionare i valori che si desidera rappresentare in base alle dimensioni delle bolle nel grafico. I valori provengono dalla vista del rapporto. Specificare la modalità di riepilogo delle informazioni.

   >[!NOTE]
   >
   >Assicurati di disporre di almeno una colonna riepilogata per attivare questo campo.\
   >Per ulteriori informazioni sul riepilogo delle informazioni nella colonna di un report, vedere [Creare un report personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Nel campo **Bolle** selezionare il raggruppamento che si desidera includere nel grafico. Il Raggruppamento è rappresentato dalla posizione delle bolle sul grafico.
1. Nel campo **Colore bolle** selezionare il campo che si desidera rappresentare con i colori delle bolle.

   ![](assets/qs-bubble-chart-350x103.png)


   Il **colore bolla** può essere un raggruppamento definito nel report, ma è disponibile solo quando si seleziona la colonna **Nome** per l&#39;oggetto del report nel campo **Bolle**.

   Ad esempio, se hai selezionato **Nome attività** in un report attività, puoi aggiungere **Stato attività** come campo **Colore bolla**.

   ![](assets/bubbles-field-correct-can-select-bubbles-color-example.png)

   Tuttavia, se hai selezionato **Stato attività** per il campo **Bolle**, non puoi selezionare un campo **Colore bolla**. Inoltre, non puoi selezionare **Nome progetto** per il campo **Colore bolla**, nemmeno quando selezioni **Nome attività** per il campo **Bolla**.

   ![](assets/bubbles-field-wrong-cannot-select-bubbles-color-example.png)


1. Fai clic su **Salva + Chiudi** per salvare le modifiche apportate al generatore di interfacce.

## Esportare un grafico

È possibile esportare un grafico in un file PDF.

Per esportare un grafico:

1. Fai clic su **Esporta** per esportare il grafico in formato .pdf.\
   Nel computer viene scaricato un file .pdf.

1. Apri il file .pdf.\
   Il file esportato include le seguenti informazioni:

   * Immagine del grafico.
   * Titolo che rappresenta il nome del report.
   * Un nome file univoco che corrisponde al nome del report.
   * Un piè di pagina con la data e l’ora in cui il report è stato esportato e il numero di pagina.

## Personalizzare i colori del grafico {#customize-chart-colors}

È possibile consentire a Workfront di selezionare i colori degli elementi del grafico oppure personalizzarli durante l&#39;aggiunta di un grafico ai report. Se il grafico contiene un singolo raggruppamento che rappresenta una metrica, ad esempio un report di attività che mostra il numero di attività raggruppate per data di completamento effettiva, ogni risultato del raggruppamento viene visualizzato con lo stesso colore.

È possibile scegliere un solo colore per i campi visualizzati nella visualizzazione del report. È possibile scegliere diversi colori, uno per ogni opzione, per i campi visualizzati nel Raggruppamento del report.

>[!IMPORTANT]
>
>Per i campi data, è possibile selezionare un solo colore per gli elementi del grafico.

Per personalizzare i colori dei grafici:

1. Durante la creazione di un report, passare alla scheda **Grafico** nel Report Builder.
1. Selezionare un tipo di grafico da aggiungere al report.\
   Per ulteriori informazioni sull&#39;aggiunta di un grafico al report, vedere [Aggiungere un grafico a un report](#add-a-chart-to-a-report).

1. Fare clic su **Colori personalizzati** quando questo campo è disponibile.\
   Viene visualizzata la finestra di dialogo Colori personalizzati.\
   ![](assets/custom-colors-in-charts-350x286.png)

   >[!NOTE]
   >
   >È possibile associare colori personalizzati a qualsiasi campo che è possibile raggruppare in base a e ad alcuni campi che è possibile visualizzare in una visualizzazione, inclusi i campi personalizzati. Nei campi personalizzati o nelle opzioni personalizzate dei campi selezionati nella finestra di dialogo Colore personalizzato viene fatta distinzione tra maiuscole e minuscole.

1. Prendi in considerazione di selezionare una delle seguenti opzioni:

   * **Usa un solo colore**: tutti gli elementi del grafico verranno visualizzati nel colore selezionato.

      1. Inizia a digitare il nome di un’opzione del campo selezionato, quindi seleziona un colore. Questa opzione viene visualizzata nel colore selezionato del grafico.
      1. (Facoltativo) Specificate un valore esadecimale per il colore, invece di selezionarne uno dagli esempi di colore disponibili\
         Oppure\
         Fai clic sul selettore colore visualizzato dopo aver fatto clic sul codice esadecimale e seleziona un altro colore.

   * **Aggiungi colore**: continua ad aggiungere colori personalizzati per tutte le altre opzioni possibili del campo selezionato.
   * **Rimuovi tutto**: selezionare questa opzione per rimuovere tutti i colori e le opzioni del campo selezionato in precedenza.
   * **Opzioni avanzate**: selezionare una delle opzioni seguenti:

      * **Nessun valore**: selezionare questo campo e un colore personalizzato per visualizzare la colonna del grafico che raggruppa gli elementi &quot;senza valore&quot;. Si tratta di elementi che non possono essere raggruppati in base alle opzioni del campo selezionato nel raggruppamento.
      * **Tutti gli altri valori**: selezionare questo campo e un colore personalizzato per visualizzare tutti gli altri elementi del grafico le cui opzioni non sono selezionate in precedenza.

        >[!NOTE]
        >
        >I colori utilizzati più di recente vengono visualizzati nella parte superiore della finestra di dialogo Colori personalizzati. Quando passi il mouse su un colore utilizzato di recente, viene visualizzato il nome del campo associato.

1. Fare clic sulla &quot;x&quot; nell&#39;angolo superiore destro della finestra di dialogo Colori personalizzati per chiudere la finestra di dialogo Colori personalizzati. I colori selezionati vengono salvati automaticamente.
1. Fare clic su **Salva + Chiudi** per salvare il grafico ed eseguire il report.

## Rimuovere un grafico da un report

Per rimuovere un grafico da un report:

1. Apri la scheda **Grafico** del Report Builder.
1. Passa il puntatore del mouse sopra l’icona del tipo di grafico scelto e nell’angolo in alto a destra dell’icona viene visualizzato un pulsante &quot;x&quot;.
1. Fare clic sulla &quot;x&quot; per rimuovere il grafico.
1. Fai clic su **Salva e Chiudi**.

## Limitazioni durante l’utilizzo dei grafici

Tieni presente le seguenti limitazioni quando lavori con i grafici:

* La sezione **Anteprima grafico** a destra del generatore di report non contiene dati effettivi provenienti dal report. Per visualizzare il grafico con i dati, è necessario salvarlo e visualizzarlo dalla scheda **Grafico**.

* Alcuni elementi del grafico non sono modificabili:

   * Non è possibile modificare il tipo di carattere né le dimensioni dei valori di ciascun elemento.
   * Non è possibile modificare i nomi degli assi nel grafico.

* Non è possibile modificare la legenda del grafico.
* Quando si utilizzano campi calcolati per i raggruppamenti, non è possibile fare clic sugli elementi del grafico.
* Il numero massimo di coordinate visualizzabili in un grafico è quattro, in un grafico a bolle. Tutti gli altri tipi di grafico visualizzano due o un massimo di tre punti dati.
