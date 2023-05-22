---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Aggiungere un grafico a un report
description: Puoi migliorare i rapporti aggiungendo un grafico. È possibile aggiungere grafici ai rapporti esistenti o ai rapporti che si stanno creando.
author: Nolan
feature: Reports and Dashboards
exl-id: 9b58d68c-4b7b-4344-bde3-7c65e2e1aac8
source-git-commit: be47bc4da5e3921a7c36e19831acde91aad55db1
workflow-type: tm+mt
source-wordcount: '2756'
ht-degree: 0%

---

# Aggiungere un grafico a un report

Puoi migliorare i rapporti aggiungendo un grafico. È possibile aggiungere grafici ai rapporti esistenti o ai rapporti che si stanno creando.

Prima di aggiungere un grafico a un report, è necessario creare una visualizzazione e un raggruppamento per il report. La maggior parte dei grafici può essere aggiunta solo se le informazioni sono raggruppate nel rapporto. L&#39;unico grafico che può essere aggiunto senza raggruppamento è un grafico a contatori.\
Per informazioni sulla creazione di una visualizzazione, vedere [Panoramica delle visualizzazioni in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).\
Per ulteriori informazioni sui raggruppamenti, consulta [Panoramica sui raggruppamenti in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

Se nel report vengono visualizzati troppi elementi, non viene creato un grafico. In questo caso, devi anche aggiungere un filtro al rapporto per ridurre il numero di risultati.\
Per ulteriori informazioni sui filtri, consulta [Panoramica sui filtri in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari</p> <p>Modifica accesso a Filtri, Viste, Raggruppamenti</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

## Aggiungere un grafico a un report

1. Passa a un rapporto esistente o creane uno nuovo. Per ulteriori informazioni sulla creazione di un nuovo rapporto, consulta [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. (Condizionale) Se hai visitato un rapporto esistente, fai clic su **Azioni report** > **Modifica**.

1. Assicurati che **Colonne (visualizzazione)** La scheda è stata aggiornata per soddisfare le esigenze del rapporto.\
   Per informazioni su come creare o modificare la visualizzazione del report, vedere [Panoramica delle visualizzazioni in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. Fai clic su **Raggruppamenti** e aggiungere un raggruppamento.

   >[!TIP]
   >
   >* È possibile aggiungere un grafico a un report solo quando i risultati sono raggruppati.
   >* I raggruppamenti in modalità testo non sono supportati nei grafici. Per ulteriori informazioni sui raggruppamenti in modalità testo, vedere [Modifica modalità testo in un raggruppamento](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-grouping.md).
   >* Se aggiungi un singolo raggruppamento che rappresenta una metrica, tutti i grafici eccetto un grafico a torta visualizzano ciascuno come risultato del raggruppamento dello stesso colore.


   Per ulteriori informazioni sui raggruppamenti, consulta [Panoramica sui raggruppamenti in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Seleziona la **Grafico** scheda.
1. Fare clic su un tipo di grafico per selezionarlo.\
   ![](assets/qs-report-builder-chart-350x265.png)

1. Puoi aggiungere i seguenti tipi di grafici a un rapporto di Adobe Workfront:

   * [Istogramma](#column-chart)
   * [Grafico a barre](#bar-chart)
   * [Grafico a torta](#pie-chart)
   * [Grafico a linee](#line-chart)
   * [Grafico a barre](#gauge-chart)
   * [Grafico a bolle](#bubble-chart)

1. Clic **Salva e chiudi** per salvare il grafico e il report.

### Istogramma {#column-chart}

Per aggiungere una **Colonna** grafico per il report:

1. Inizia ad aggiungere un grafico al report, come descritto in [Aggiungere un grafico a un report](#add-a-chart-to-a-report).
1. In **Asse (Y) sinistro** , selezionare i valori che si desidera includere sull&#39;asse Y del grafico, nonché la modalità di riepilogo delle informazioni.
1. In **Asse inferiore (X)** selezionare il Raggruppamento che si desidera includere nel grafico.
1. (Facoltativo) Seleziona **Colori personalizzati** per assegnare i colori preferiti a ciascuna colonna.\
   Per ulteriori informazioni sulla personalizzazione dei colori dei grafici, vedere [Personalizzare i colori del grafico](#customize-chart-colors).

1. (Facoltativo) Seleziona **Mostra in 3D** per visualizzare il grafico in una visualizzazione tridimensionale.
1. (Facoltativo) **Raggruppa colonne**: seleziona questa opzione per definire il modo in cui desideri raggruppare le colonne.\
   Selezionare una delle opzioni seguenti:

   * Fare clic su una delle opzioni seguenti per selezionare la modalità di visualizzazione delle colonne raggruppate:\
      **- Affiancato**

      **- Impilate**
      **- Impilate al 100%**

   * Selezionare il Raggruppamento che si desidera includere nel grafico.
   * (Facoltativo) Seleziona **Colori personalizzati** per personalizzare i colori delle colonne.\
      Per ulteriori informazioni sulla personalizzazione dei colori dei grafici, vedere [Personalizzare i colori del grafico](#customize-chart-colors).

1. (Facoltativo) Seleziona **Grafico combinato** per includere un valore aggiuntivo nel grafico, nonché come si desidera riepilogare le informazioni.\
   Considera le seguenti opzioni:

   * **Traccia sull&#39;asse secondario**: seleziona questa opzione per tracciare i dati sul lato destro del grafico.
   * **Tipo di grafico**: seleziona se desideri che questo valore aggiuntivo venga visualizzato come riga o come terza colonna.\
      ![](assets/qs-column-chart-350x163.png)

1. Clic **Salva e chiudi** per salvare il grafico e il report.

### Grafico a barre {#bar-chart}

Per aggiungere una **Barre** grafico per il report:

1. Inizia ad aggiungere un grafico al report, come descritto in [Aggiungere un grafico a un report](#add-a-chart-to-a-report).
1. In **Asse inferiore (X)** , selezionare i valori che si desidera includere sull&#39;asse X del grafico, nonché la modalità di riepilogo delle informazioni.
1. In **Asse (Y) sinistro** selezionare il Raggruppamento che si desidera includere nel grafico.
1. (Facoltativo) Seleziona **Colori personalizzati** per personalizzare i colori delle barre.\
   Per ulteriori informazioni sulla personalizzazione dei colori dei grafici, vedere [Personalizzare i colori del grafico](#customize-chart-colors).

1. (Facoltativo) Seleziona **Mostra in 3D** per visualizzare il grafico in una visualizzazione tridimensionale.
1. (Facoltativo) Raggruppa barre**: selezionare questa opzione per definire la modalità di raggruppamento delle barre.\
   Selezionare una delle opzioni seguenti:

   * Fare clic su una delle opzioni seguenti per selezionare la modalità di visualizzazione delle barre raggruppate:\
      **- Affiancato**

      **- Impilate**
      **- Impilate al 100%**

   * Selezionare il Raggruppamento che si desidera includere nel grafico.
   * (Facoltativo) Seleziona **Colori personalizzati** per personalizzare i colori delle colonne.\
      Per ulteriori informazioni sulla personalizzazione dei colori dei grafici, vedere [Personalizzare i colori del grafico](#customize-chart-colors).

1. (Facoltativo) Seleziona **Grafico combinato** per includere un valore aggiuntivo nel grafico, nonché come si desidera riepilogare le informazioni.\
   ![](assets/qs-bar-chart-350x167.png)

1. Clic **Salva e chiudi** per salvare il grafico e il report.

### Grafico a torta {#pie-chart}

Per aggiungere una **Torta** grafico per il report:

1. Inizia ad aggiungere un grafico al report, come descritto in [Aggiungere un grafico a un report](#add-a-chart-to-a-report).
1. In **Valori** selezionare i valori che si desidera visualizzare nel rapporto e la modalità di riepilogo.\
   In **Cunei** selezionare il Raggruppamento che si desidera includere nel grafico. Il raggruppamento è rappresentato dai cunei del grafico.

1. (Facoltativo) Seleziona **Colori personalizzati** per personalizzare i colori dei cunei nel grafico.\
   Per ulteriori informazioni sulla personalizzazione dei colori dei grafici, vedere [Personalizzare i colori del grafico](#customize-chart-colors).

1. (Facoltativo) Seleziona **Mostra in 3D** per visualizzare il grafico in una visualizzazione tridimensionale.
1. In **Mostra risultati come** , selezionare la modalità di visualizzazione dei risultati nel grafico. Considera le seguenti opzioni:

   * **Percento**: i risultati del grafico vengono visualizzati come percentuale.
   * **Numeri**: i risultati del grafico vengono visualizzati sotto forma di numero.\
      ![](assets/qs-pie-chart-350x171.png)

1. Clic **Salva e chiudi** per salvare il grafico e il report.

### Grafico a linee {#line-chart}

Per aggiungere una **Linea** grafico per il report:

1. Inizia ad aggiungere un grafico al report, come descritto in [Aggiungere un grafico a un report](#add-a-chart-to-a-report).
1. In **Asse (Y) sinistro** , selezionare i valori che si desidera includere sull&#39;asse Y del grafico, nonché la modalità di riepilogo delle informazioni.
1. In **Asse inferiore (X)** selezionare il Raggruppamento che si desidera includere nel grafico.
1. (Facoltativo) Selezionate un colore per personalizzare il colore della linea.
1. (Facoltativo) Seleziona **Raggruppa linee**, per selezionare un raggruppamento aggiuntivo per il grafico.\
   (Facoltativo) Seleziona **Colori personalizzati** per personalizzare i colori per il nuovo raggruppamento.\
   Per ulteriori informazioni sulla personalizzazione dei colori dei grafici, vedere [Personalizzare i colori del grafico](#customize-chart-colors).

1. (Facoltativo) Seleziona **Grafico combinato** per combinare le linee con un valore aggiuntivo.\
   Considera tra le seguenti opzioni:

   * Selezionare il valore che si desidera includere nel grafico, nonché la modalità di riepilogo delle informazioni.
   * Seleziona la **Traccia sull&#39;asse secondario** per tracciare i dati sul lato destro del grafico.\
      ![](assets/qs-line-chart-350x172.png)

1. Clic **Salva e chiudi** per salvare il grafico e il report.

### Grafico a barre {#gauge-chart}

A **Misuratore** grafico visualizza il numero di record che soddisfano un determinato criterio in un formato di indicatore. L&#39;indicatore del contatore punta al numero di record che soddisfano i criteri selezionati nella visualizzazione e nel raggruppamento del report. Non è necessario un raggruppamento di rapporti per configurare un grafico a contatori.

Per aggiungere una **Misuratore** grafico per il report:

1. Inizia ad aggiungere un grafico al report, come descritto in [Aggiungere un grafico a un report](#add-a-chart-to-a-report).
1. In **Valori** selezionare i valori che si desidera visualizzare nel rapporto e la modalità di riepilogo. Se si seleziona **Conteggio record**, i valori visualizzati sono l’oggetto del rapporto.

1. In **Indicatori** selezionare il Raggruppamento che si desidera includere nel grafico. Il Raggruppamento è rappresentato dalla linea dell&#39;indicatore nel grafico.\
   Se si dispone di un raggruppamento che contiene due elementi, nel grafico vengono visualizzati due indicatori.\
   Ad esempio, se si dispone di un raggruppamento dello stato del progetto e sono presenti due stati del progetto (Corrente e In sospeso), il grafico Misuratore contiene due indicatori di contatore. Indicheranno il numero di progetti che si trovano in quello stato.\
   (Facoltativo) Seleziona **Totale** nel **Indicatori** per visualizzare il totale degli oggetti selezionati nel campo **Valori** campo.

1. In **Intervallo di valori** , specificare l&#39;intervallo di valori e il colore per rappresentare tali valori da visualizzare nel grafico Misuratore.
1. (Facoltativo) Fai clic su **Aggiungi un altro intervallo di valori** per aggiungere ulteriori intervalli di valori al grafico.\
   ![](assets/qs-gauge-chart-350x181.png)

1. Clic **Salva e chiudi** per salvare il grafico e il report.

### Grafico a bolle {#bubble-chart}

È possibile visualizzare fino a tre campi di un oggetto in una **Bolla** grafico. Ciò significa che è possibile visualizzare fino a quattro punti dati in un grafico a bolle. Ogni entità con tre campi associati viene visualizzata come un cerchio che esprime due dei campi all&#39;interno della sua posizione all&#39;interno degli assi X e Y. Il terzo campo è rappresentato dalla dimensione del cerchio.

Per aggiungere una **Bolla** grafico per il report:

1. Inizia ad aggiungere un grafico al report, come descritto in [Aggiungere un grafico a un report](#add-a-chart-to-a-report).
1. In **Asse (Y) sinistro** selezionare i valori che si desidera includere sull&#39;asse Y del grafico. I valori provengono dalla vista del rapporto. Specificare la modalità di riepilogo delle informazioni.
1. In **Campo Asse inferiore (X)**, selezionare i valori che si desidera includere sull&#39;asse X del grafico. I valori provengono dalla vista del rapporto. Specificare la modalità di riepilogo delle informazioni.

   >[!NOTE]
   >
   >Assicurati di disporre di almeno una colonna riepilogata per attivare questo campo.\
   >Per ulteriori informazioni sul riepilogo delle informazioni in una colonna di un report, vedere [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. In **Dimensione bolla** , selezionare i valori che si desidera rappresentare in base alle dimensioni delle bolle del grafico. I valori provengono dalla vista del rapporto. Specificare la modalità di riepilogo delle informazioni.

   >[!NOTE]
   >
   >Assicurati di disporre di almeno una colonna riepilogata per attivare questo campo.\
   >Per ulteriori informazioni sul riepilogo delle informazioni in una colonna di un report, vedere [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. In **Bolle** selezionare il Raggruppamento che si desidera includere nel grafico. Il Raggruppamento è rappresentato dalla posizione delle bolle sul grafico.
1. In **Colore bolla** , selezionare il campo che si desidera rappresentare con i colori delle bolle.

   ![](assets/qs-bubble-chart-350x103.png)


   Il **Colore bolla** può essere un Raggruppamento definito nel rapporto, ma è disponibile solo quando selezioni il **Nome** per l&#39;oggetto del report nella **Bolle** campo.

   Ad esempio, se hai selezionato **Nome attività** in un report attività è possibile aggiungere **Stato attività** come **Colore bolla** campo.

   ![](assets/bubbles-field-correct-can-select-bubbles-color-example.png)

   Tuttavia, se hai selezionato **Stato attività** per **Bolle** , non è possibile selezionare un **Colore bolla** campo. Inoltre, non è possibile selezionare **Nome progetto** per **Colore bolla** anche quando selezioni **Nome attività** per **Bolla** campo.

   ![](assets/bubbles-field-wrong-cannot-select-bubbles-color-example.png)


1. Clic **Salva e chiudi** per salvare le modifiche apportate al generatore di interfacce.

## Esportare un grafico

È possibile esportare un grafico in un file PDF.

Per esportare un grafico:

1. Clic **Esporta** per esportare il grafico in formato .pdf.\
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

1. Durante la creazione di un rapporto, vai al **Grafico** nel report builder.
1. Selezionare un tipo di grafico da aggiungere al report.\
   Per ulteriori informazioni sull&#39;aggiunta di un grafico al report, vedere [Aggiungere un grafico a un report](#add-a-chart-to-a-report).

1. Clic **Colori personalizzati** quando questo campo è disponibile.\
   Viene visualizzata la finestra di dialogo Colori personalizzati.\
   ![](assets/custom-colors-in-charts-350x286.png)

   >[!NOTE]
   >
   >È possibile associare colori personalizzati a qualsiasi campo che è possibile raggruppare in base a e ad alcuni campi che è possibile visualizzare in una visualizzazione, inclusi i campi personalizzati. Nei campi personalizzati o nelle opzioni personalizzate dei campi selezionati nella finestra di dialogo Colore personalizzato viene fatta distinzione tra maiuscole e minuscole.

1. Prendi in considerazione di selezionare una delle seguenti opzioni:

   * **Usa un colore**: tutti gli elementi del grafico vengono visualizzati con il colore selezionato.

      1. Inizia a digitare il nome di un’opzione del campo selezionato, quindi seleziona un colore. Questa opzione viene visualizzata nel colore selezionato del grafico.
      1. (Facoltativo) Specificate un valore esadecimale per il colore, invece di selezionarne uno dagli esempi di colore disponibili\
         Oppure\
         Fai clic sul selettore colore visualizzato dopo aver fatto clic sul codice esadecimale e seleziona un altro colore.
   * **Aggiungi colore**: continua ad aggiungere colori personalizzati per tutte le altre opzioni possibili del campo selezionato.
   * **Rimuovi tutto**: seleziona questa opzione per rimuovere tutti i colori e le opzioni del campo selezionato in precedenza.
   * **Opzioni avanzate**: seleziona una delle seguenti opzioni:

      * **Nessun valore**: seleziona questo campo e un colore personalizzato per visualizzare la colonna del grafico che raggruppa gli elementi &quot;senza valore&quot;. Si tratta di elementi che non possono essere raggruppati in base alle opzioni del campo selezionato nel raggruppamento.
      * **Tutti gli altri valori**: seleziona questo campo e un colore personalizzato per visualizzare tutti gli altri elementi del grafico le cui opzioni non sono selezionate sopra.

         >[!NOTE]
         >
         >I colori utilizzati più di recente vengono visualizzati nella parte superiore della finestra di dialogo Colori personalizzati. Quando passi il mouse su un colore utilizzato di recente, viene visualizzato il nome del campo associato.


1. Fare clic sulla &quot;x&quot; nell&#39;angolo superiore destro della finestra di dialogo Colori personalizzati per chiudere la finestra di dialogo Colori personalizzati. I colori selezionati vengono salvati automaticamente.
1. Clic **Salva e chiudi** per salvare il grafico ed eseguire il report.

## Rimuovere un grafico da un report

Per rimuovere un grafico da un report:

1. Apri **Grafico** del report builder.
1. Passa il puntatore del mouse sopra l’icona del tipo di grafico scelto e nell’angolo in alto a destra dell’icona viene visualizzato un pulsante &quot;x&quot;.
1. Fare clic sulla &quot;x&quot; per rimuovere il grafico.
1. Clic **Salva e chiudi**.

## Limitazioni durante l’utilizzo dei grafici

Tieni presente le seguenti limitazioni quando lavori con i grafici:

* Il **Anteprima grafico** a destra di report builder non contiene i dati effettivi provenienti dal report. È necessario salvare il grafico e visualizzarlo dal **Grafico** per visualizzare il grafico con i dati.

* Alcuni elementi del grafico non sono modificabili:

   * Non è possibile modificare il tipo di carattere né le dimensioni dei valori di ciascun elemento.
   * Non è possibile modificare i nomi degli assi nel grafico.

* Non è possibile modificare la legenda del grafico.
* Quando si utilizzano campi calcolati per i raggruppamenti, non è possibile fare clic sugli elementi del grafico.
* Il numero massimo di coordinate visualizzabili in un grafico è quattro, in un grafico a bolle. Tutti gli altri tipi di grafico visualizzano due o un massimo di tre punti dati.
