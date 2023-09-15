---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: Creare un grafico per un rapporto in base a un campo personalizzato a selezione multipla
description: È possibile tracciare un report in base a un campo personalizzato a selezione multipla solo dopo aver creato un campo calcolato aggiuntivo che acquisisce le scelte selezionate nel campo personalizzato a selezione multipla.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: cda77319-dce6-409d-8f59-53838820cafb
source-git-commit: b0447fd2ea9419fabcc21a1131910485c18b75d0
workflow-type: tm+mt
source-wordcount: '1007'
ht-degree: 0%

---

# Creare un grafico per un rapporto in base a un campo personalizzato a selezione multipla

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->

Invece di creare un grafico utilizzando un campo personalizzato a selezione multipla, è consigliabile creare campi separati per ogni opzione di un campo personalizzato a selezione multipla.

Di seguito sono riportati alcuni esempi di campi personalizzati a selezione multipla:

* Checkboxe
* Menu a discesa a selezione multipla

Per informazioni sull’utilizzo della modalità testo, consulta l’articolo [Panoramica sulla modalità testo](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Tuttavia, se non è possibile disporre di campi separati per ogni opzione di un campo a selezione multipla, è possibile tracciare un rapporto in base a un campo personalizzato a selezione multipla utilizzando i campi personalizzati calcolati per raggruppare prima le scelte del campo a selezione multipla. Successivamente, è possibile tracciare il rapporto in base ai campi calcolati.

>[!NOTE]
>
>Gli elementi con una delle scelte selezionate vengono conteggiati una sola volta.
>
>Ad esempio, se si dispone di un campo personalizzato Casella di controllo con le opzioni Scelta 1 e Scelta 2 e si allega il modulo alle attività, le attività con entrambe le opzioni Scelta 1 e Scelta 2 vengono visualizzate in un elemento grafico separato rispetto alle attività con solo la scelta 1 o la scelta 2 selezionate.
>
>Le attività per le quali è selezionata la Scelta 1 non vengono visualizzate nello stesso elemento del grafico delle attività per le quali sono selezionate le Scelta 1 e Scelta 2.

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

## Prerequisiti

Prima di iniziare, è necessario creare un campo personalizzato calcolato che mostri i valori selezionati dal campo personalizzato a selezione multipla. Per informazioni, vedere [Creare un campo personalizzato calcolato che faccia riferimento a un campo personalizzato a selezione multipla](#build-a-calculated-custom-field-that-references-a-multi-select-custom-field) in questo articolo.

## Creare un grafico per i campi personalizzati a selezione multipla

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this moved to its own article, linked in the Note above!)</p>
-->

Non è possibile creare un grafico in un report facendo riferimento a un campo personalizzato a selezione multipla. È invece possibile creare un campo calcolato che registra i valori del campo personalizzato a selezione multipla per un determinato oggetto e raggruppa in base al campo calcolato. 

* [Creare un campo personalizzato calcolato che faccia riferimento a un campo personalizzato a selezione multipla](#build-a-calculated-custom-field-that-references-a-multi-select-custom-field)
* [Creare un grafico che faccia riferimento a un campo personalizzato calcolato](#build-a-chart-that-references-a-calculated-custom-field)

### Creare un campo personalizzato calcolato che faccia riferimento a un campo personalizzato a selezione multipla {#build-a-calculated-custom-field-that-references-a-multi-select-custom-field}

Per creare un campo calcolato che faccia riferimento a un campo personalizzato a selezione multipla, è necessario disporre dei seguenti prerequisiti:

* Campo personalizzato a selezione multipla in un modulo personalizzato.\
  Per informazioni sulla creazione di moduli personalizzati e sull’aggiunta di campi personalizzati, consulta l’articolo [Creare o modificare un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

* Modulo personalizzato con campo personalizzato a selezione multipla associato agli oggetti.
* Valori per il campo personalizzato a selezione multipla per ciascun oggetto.

Per generare il campo personalizzato calcolato che fa riferimento al campo personalizzato a selezione multipla:

1. Crea un modulo personalizzato o modificane uno esistente.

   Per informazioni sulla creazione di moduli personalizzati, consulta [Creare o modificare un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. Selezionare l&#39;oggetto o gli oggetti che si intende utilizzare con il modulo personalizzato.
1. Clic **Aggiungi un campo**, quindi **Calcolato** per aggiungere al modulo il campo personalizzato a selezione multipla.

1. In **Etichetta** , assegnare un nome al nuovo campo calcolato per indicare che fa riferimento al campo personalizzato a selezione multipla.

   Ad esempio: &quot;Campo a selezione multipla calcolato&quot;.

1. In **Calcolo** immettere il codice seguente:

   `{DE:Multi-select Custom Field}`

   In questo modo le scelte selezionate nel campo personalizzato a selezione multipla vengono aggiunte al campo personalizzato calcolato. Ad esempio, se il modulo è allegato ad attività e la scelta 1 è selezionata dal campo personalizzato a selezione multipla, il campo personalizzato calcolato visualizza il valore &quot;Scelta 1&quot;. Se le opzioni Scelta 1 e Scelta 2 sono selezionate per un&#39;attività diversa, nel campo personalizzato calcolato verrà visualizzato il valore &quot;Scelta 1, Scelta 2&quot;.

1. Sostituisci &quot;Campo personalizzato a selezione multipla&quot; con il nome effettivo del campo personalizzato a selezione multipla, come visualizzato in Workfront.

   ![](assets/calculated-multi-select-custom-field-nwe-350x223.png)

1. (Facoltativo) Se il campo personalizzato a selezione multipla è già incluso in questo modulo e se questo modulo è già allegato agli oggetti, abilita **Aggiorna calcoli precedenti (in background)** opzione.

   In questo modo il nuovo campo calcolato viene compilato automaticamente con il valore del campo personalizzato a selezione multipla che viene aggiunto ai moduli già allegati agli oggetti.

1. Clic **Fine**.
1. Clic **Salva e chiudi**.

   Il campo personalizzato calcolato viene aggiunto al modulo personalizzato e, se il modulo è attualmente associato a oggetti, il campo viene compilato con le informazioni del campo personalizzato a selezione multipla.

### Creare un grafico che faccia riferimento a un campo personalizzato calcolato {#build-a-chart-that-references-a-calculated-custom-field}

1. (Facoltativo) Per fare in modo che tutti i campi calcolati in base ai quali si desidera creare il grafico vengano compilati con valori, dalla scheda Dettagli del report selezionare tutti gli oggetti che contengono il modulo personalizzato con il campo personalizzato a selezione multipla e il campo personalizzato calcolato, quindi fare clic su **Modifica**.
1. (Facoltativo e condizionale) Seleziona il **Ricalcolare Espressioni Personalizzate** , quindi fai clic su **Salva modifiche**.\
   ![](assets/recalculate-custom-expressions-350x259.png)

   >[!NOTE]
   >
   >Questa opzione è stata eliminata dalla modifica in blocco di progetti.  È comunque possibile ricalcolare le espressioni per i progetti in blocco facendo clic sul pulsante **Altro** icona ![](assets/more-icon-45x33.png) nella parte superiore dell’elenco di un progetto, quindi **Ricalcola espressioni**.


1. Vai al report in cui desideri aggiungere il grafico per il campo calcolato che fa riferimento al campo personalizzato a selezione multipla.
1. Clic **Azioni report**, quindi **Modifica**.

1. Seleziona la <strong>Raggruppamenti</strong> , quindi fai clic su <strong>Aggiungi raggruppamento</strong>.
1. Aggiungi il <strong>Campo a selezione multipla calcolato</strong> creato come raggruppamento.
1. Seleziona la <strong>Grafico</strong> e aggiungere un grafico al report.

   Ad esempio, scegli un **Colonna** grafico.
   <br>Per informazioni sull&#39;aggiunta di un grafico a un report, vedere la sezione <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md#add-a-chart" class="MCXref xref">Aggiungere un grafico a un report</a> nell’articolo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Creare un rapporto personalizzato</a>.
1. In **Asse inferiore (X)** , selezionare il campo <strong>Campo a selezione multipla calcolato</strong> da visualizzare nel grafico.
1. Clic <strong>Salva e chiudi</strong>.

   Il rapporto visualizza i risultati raggruppati per il campo a selezione multipla calcolato in un grafico.

   ![](assets/chart-multi-select-field-column-chart-example.png)