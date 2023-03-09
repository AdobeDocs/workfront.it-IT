---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: Creare un grafico per un rapporto in base a un campo personalizzato a selezione multipla
description: Non è possibile tracciare un report con un campo personalizzato a selezione multipla. È necessario creare un campo calcolato aggiuntivo che faccia riferimento al campo personalizzato a selezione multipla per tracciare il rapporto anche in base al valore del campo personalizzato a selezione multipla.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: cda77319-dce6-409d-8f59-53838820cafb
source-git-commit: 23257f11b0795aa1f1e422923f6d596017c58126
workflow-type: tm+mt
source-wordcount: '796'
ht-degree: 0%

---

# Creare un grafico per un rapporto in base a un campo personalizzato a selezione multipla

<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima.</span>

Non è possibile tracciare un report con un campo personalizzato a selezione multipla. È necessario creare un campo calcolato aggiuntivo che faccia riferimento al campo personalizzato a selezione multipla per tracciare il rapporto anche in base al valore del campo personalizzato a selezione multipla.

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

Per poter creare un campo calcolato che faccia riferimento a un campo personalizzato a selezione multipla, è necessario disporre dei seguenti prerequisiti:

* Crea il campo personalizzato a selezione multipla in un modulo personalizzato.\
   Per informazioni sulla creazione di moduli personalizzati e sull’aggiunta di campi personalizzati, consulta l’articolo [Creare o modificare un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

* Allegare il modulo personalizzato agli oggetti.
* Compila il campo personalizzato a selezione multipla con un valore su ciascun oggetto.

Per generare il campo personalizzato calcolato che fa riferimento al campo personalizzato a selezione multipla:

1. Crea un modulo personalizzato o modificane uno esistente.\
   Per informazioni sulla creazione di moduli personalizzati, consulta l’articolo [Creare o modificare un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. Selezionare l&#39;oggetto o gli oggetti che si intende utilizzare con il modulo personalizzato.
1. Clic **Aggiungi un campo**, quindi **Calcolato** per aggiungere al modulo il campo personalizzato a selezione multipla.

1. In **Etichetta** , assegnare un nome al nuovo campo calcolato per indicare che fa riferimento al campo personalizzato a selezione multipla.\
   Ad esempio: &quot;Campo a selezione multipla calcolato&quot;.

1. In **Calcolo** immettere il codice seguente:

   ```
   {DE:Multi-select Custom Field}
   ```

1. Sostituisci &quot;Campo personalizzato a selezione multipla&quot; con il nome effettivo del campo personalizzato a selezione multipla, come visualizzato in Workfront.

   ![](assets/calculated-multi-select-custom-field-nwe-350x223.png)

1. (Facoltativo) Se il campo personalizzato a selezione multipla è già incluso in questo modulo e se questo modulo è già allegato agli oggetti, abilita **Aggiorna calcoli precedenti** opzione.\
   In questo modo il nuovo campo viene compilato automaticamente con il valore del campo personalizzato a selezione multipla che viene aggiunto ai moduli già allegati agli oggetti.

1. Clic **Fine**.
1. Clic **Salva +Chiudi**.

### Creare un grafico che faccia riferimento a un campo personalizzato calcolato {#build-a-chart-that-references-a-calculated-custom-field}

1. (Facoltativo) Per fare in modo che tutti i campi calcolati in base ai quali si desidera creare il grafico vengano compilati con valori, selezionare tutti gli oggetti del report che contengono il modulo personalizzato con il campo personalizzato a selezione multipla e il campo personalizzato calcolato, quindi fare clic su **Modifica**.
1. (Facoltativo e condizionale) Abilita il **Ricalcolare Espressioni Personalizzate** , quindi fai clic su **Salva modifiche**.\
   ![](assets/recalculate-custom-expressions-350x259.png)

   >[!NOTE]
   >
   ><span class="preview">Questa opzione è stata eliminata dalla modifica in blocco di progetti nell’ambiente di anteprima.  È comunque possibile ricalcolare le espressioni per i progetti in blocco facendo clic su **Altro** ![](assets/more-icon-45x33.png) nella parte superiore dell’elenco di un progetto, quindi **Ricalcola espressioni**. </span>


1. Vai al report in cui desideri aggiungere il grafico per il campo calcolato che fa riferimento al campo personalizzato a selezione multipla.
1. Clic **Azioni report**, quindi **Modifica**.

1. Seleziona la <strong>Raggruppamenti</strong> , quindi fai clic su <strong>Aggiungi raggruppamento</strong>.
1. Aggiungi il<strong>Campo a selezione multipla calcolato</strong> creato come raggruppamento.
1. Seleziona la <strong>Grafico</strong> e aggiungere un grafico al report.<br>Per informazioni sull&#39;aggiunta di un grafico a un report, vedere la sezione <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md#add-a-chart" class="MCXref xref">Aggiungere un grafico a un report</a> nell’articolo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Creare un rapporto personalizzato</a>.
1. Seleziona la <strong>Campo a selezione multipla calcolato</strong> come uno dei campi da visualizzare nel grafico.
1. Clic <strong>Salva e chiudi</strong>.<br>Il rapporto visualizza i risultati raggruppati per il campo a selezione multipla calcolato in un grafico.
