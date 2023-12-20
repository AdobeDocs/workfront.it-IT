---
product-area: reporting
navigation-topic: text-mode-reporting
title: Modificare una vista utilizzando la modalità testo
description: "NOTA: aggiungi una sezione in questo articolo: /Content/Reports and Dashboards/Reports/Reporting Elements/create-customize-views.html *** Inoltre, crea una bozza di quest’area nell’articolo di panoramica sulla modalità testo"
author: Nolan
feature: Reports and Dashboards
exl-id: b99a2d14-a226-4075-9b1b-ac9426fd41b8
source-git-commit: dad054fe52bd7c5ca97144567c80e6d340541a50
workflow-type: tm+mt
source-wordcount: '1639'
ht-degree: 0%

---

# Modificare una vista utilizzando la modalità testo

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">NOTE: add a section in this article: /Content/Reports and Dashboards/Reports/Reporting Elements/create-customize-views.html *** Also, draft this area in the Text Mode overview article) </p>
-->

È possibile modificare una visualizzazione in un elenco o in un report utilizzando la modalità testo per accedere a campi non disponibili nell&#39;interfaccia standard e creare visualizzazioni più complesse.

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
   <td> <p>Modifica accesso a Filtri, Viste, Raggruppamenti</p> <p>Modificare l’accesso a Rapporti, Dashboard e Calendari per modificare gli elementi di reporting in un rapporto</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un report per modificare le visualizzazioni in un report</p> <p>Gestire le autorizzazioni per una visualizzazione per modificarla</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

## Prerequisiti

Prima di iniziare a utilizzare la modalità testo in un report o in un elenco, accertati di avere sempre familiarità con la sintassi della modalità testo di Workfront.

Per ulteriori informazioni, consulta:

* [Panoramica sulla modalità testo](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [Panoramica sulla sintassi della modalità testo](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)
* [Esempi di visualizzazione, filtro e raggruppamento personalizzati: indice articolo](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## Modificare la modalità testo in una visualizzazione

La modifica di una visualizzazione utilizzando la modalità testo è identica per i report e gli elenchi. L&#39;accesso alla visualizzazione da un report o da un elenco è diverso.

>[!TIP]
>
>È consigliabile creare la maggior quantità possibile di visualizzazione in modalità standard, quindi convertirla in modalità testo per modificarla.

Per informazioni sulla creazione di viste, vedere [Panoramica delle visualizzazioni in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

Per informazioni sulla creazione di un rapporto, consulta [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Esegui una delle operazioni seguenti:

   1. Per accedere alla visualizzazione da un report, passa al report, quindi fai clic su **Azioni report** > **Modifica** > **Colonne (visualizzazione)** scheda.
   1. Per accedere alla vista da un elenco, vai all’elenco e dalla **Visualizza** menu a discesa, posizionare il puntatore del mouse sulla vista da modificare e fare clic sulla **Modifica** icona ![](assets/edit-icon.png).

      Viene aperto il generatore di viste (View Builder).

1. Selezionare una colonna nella visualizzazione.

   Oppure

   Seleziona la **Colonne (visualizzazione)** del generatore di report, quindi seleziona una colonna.

   >[!TIP]
   >
   >Per modificare una vista utilizzando la modalità testo, è necessario modificare una colonna alla volta.

1. Clic **Passa alla modalità testo** nell’angolo superiore destro del generatore.

   >[!NOTE]
   >
   >Quando si modifica una colonna in modalità testo, Workfront aggiunge `textmode=true` riga di codice della colonna. Indica che la colonna è stata modificata in modalità testo.

   ![](assets/switch-to-text-mode-in-view-nwe-highlighted-350x447.png)

   La tabella seguente illustra le linee chiave in una vista in modalità testo:

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: make this a snippet and add it to the grouping article too)</p>
   -->

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Riga di esempio</th> 
      <th>Descrizione</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p><strong>valuefield</strong>=</p> </td> 
      <td> <p>Nome dell'oggetto o del campo visualizzato nel database. Per ulteriori informazioni sull'aspetto degli oggetti e dei campi nel database, vedere <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>.</p> <p>Esistono i seguenti scenari:</p> 
       <ol> 
        <li value="1"> <p> Se il nome del campo visualizzato è una frase invece di un singolo sostantivo, è necessario utilizzare la sintassi Camel Case per <code>valuefield</code>. Ad esempio, per la Data inizio pianificata di un'attività il codice è: </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span><code>valuefield=plannedStartDate</code> </p> </li> 
        <li value="2"> <p>Se si desidera visualizzare un campo personalizzato, <code>valuefield</code> value è il nome effettivo del campo, come visualizzato nell’interfaccia. Ad esempio, per un campo personalizzato denominato "Ulteriori informazioni", il codice è:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span><code>valuefield=More information</code> </p> </li> 
        <li value="3"> <p>Se si desidera visualizzare oggetti correlati ad altri oggetti in una vista utilizzando <code>valuefield</code> riga di codice i nomi e gli attributi degli oggetti sono separati da due punti. </p> <p>Una colonna in una visualizzazione delle attività in cui viene visualizzato il nome del proprietario del Portfolio, ad esempio, ha il seguente valore per la riga del campo valore:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span><code>valuefield=project:portfolio:owner:name</code> </p> <p>Indica che dall'oggetto del report (attività) è possibile accedere all'oggetto correlato successivo (progetto), da cui è possibile accedere al seguente oggetto correlato dal progetto (portfolio), quindi dal proprietario del portfolio e infine dal nome (nome). </p> </li> 
       </ol> <p>Per informazioni sulla connessione tra gli oggetti, vedere la sezione <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects" class="MCXref xref">Interdipendenza e gerarchia degli oggetti</a> in <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Comprendere gli oggetti in Adobe Workfront</a>.</p> <p>Nota: se si sceglie un campo in modalità testo non valido nell'interfaccia standard, non è possibile tornare all'interfaccia standard all'interno della colonna.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>valueformat=</strong> </td> 
      <td> <p>Questa riga rappresenta il formato utilizzato per visualizzare <code>valuefield</code>. Il <code>valueformat</code> identifica se un oggetto o un campo viene visualizzato come testo, numero, percentuale o data.</p> <p>È consigliabile utilizzare <code>HTML</code> per <code>valueformat</code>, soprattutto quando si utilizza <code>valueexpression</code>, per garantire la visualizzazione più accurata delle informazioni. </p> <p>Per informazioni sui valori aggiuntivi per questa riga, consulta <a href="../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md" class="MCXref xref">Utilizzare la formattazione condizionale in modalità testo</a>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>valueexpression=</strong> </p> </td> 
      <td> <p>Puoi aggiungere questa riga per sostituire <code>valuefield</code>, se si desidera visualizzare un campo calcolato nella colonna.</p> <p>È necessario racchiudere <code>valuefield</code> degli oggetti tra parentesi graffe ogni volta che lo si utilizza in un <code>valueexpression</code>.</p> <p>Esistono i seguenti scenari: </p> 
       <ol> 
        <li value="1"> <p>Se desideri visualizzare un campo in una colonna in maiuscolo, puoi utilizzare:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span><code>valueexpression=UPPER({valuefield})</code> </p> <p>Il <code>valuefield</code> dell’oggetto viene digitato nel modo in cui viene visualizzato in API Explorer. </p> </li> 
        <li value="2">Se desideri aggiungere più <code>valuefields</code> unendoli, è necessario separarli con un punto.</li> 
        <li value="3"> <p>Ad esempio, se si desidera visualizzare il nome dell'assegnatario principale di un'attività utilizzando <code>valueexpression</code>, puoi utilizzare:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span><code>valueexpreesion={assignedTo}.{name}</code> </p> </li> 
        <li value="4"> <p>Se desideri utilizzare un campo personalizzato in un <code>valueexpression</code> riga che deve precedere il nome del campo <code>DE:</code> per indicare che è un campo personalizzato. Il nome del campo viene digitato nel modo in cui viene visualizzato nell’interfaccia. </p> <p>Importante: quando si utilizza un campo personalizzato inserito in una sezione di un modulo personalizzato con autorizzazioni limitate per alcuni utenti, il calcolo dell'espressione di valore è vuoto quando tali utenti visualizzano questo calcolo in un report. Per informazioni sulla modifica delle autorizzazioni per le sezioni dei moduli personalizzati, consulta <span href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md"><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Creare o modificare un modulo personalizzato</a></span>.</p> <p>Ad esempio, se disponi di un campo personalizzato denominato "Nome sviluppatore" e desideri visualizzarlo in maiuscolo in una colonna, puoi utilizzare quanto segue <code>valueexpression</code> per indicare quanto segue:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span><code>valueexpression=UPPER({DE:Developer Name}</code>) </p> <p>Quando si fa riferimento a un campo personalizzato di tipo Typeahead, utilizzare l'espressione seguente per fare riferimento al nome dell'oggetto selezionato in un campo con etichetta "Nome sviluppatore":</p> <p><code>valueexpression=UPPER({DE:Developer Name:name})</code> </p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>descriptionkey= / description=</strong> </p> </td> 
      <td> <p>Questa riga definisce il testo di una descrizione quando si passa il mouse sul nome della colonna. In questo caso, utilizza una chiave per tradurre il valore del nome nel testo della descrizione. Se si desidera modificare la descrizione, modificare questa riga in: </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span><code>description=Your Value</code>.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>namekey= / name=</strong> </td> 
      <td> <p>Questa riga definisce l’etichetta della colonna. In questo caso utilizza il valore abbreviato basato sulla chiave.</p> <p>Se desideri modificare il nome della colonna, puoi modificare questo valore in: </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span><code>name=Your Value</code> </p> <p><code>Name</code> consente di immettere qualsiasi testo per il nome della colonna, mentre<code>namekey</code> richiede di immettere una chiave utilizzata per tradurre il nome di una colonna.</p> <p>Per modificare il nome della colonna puoi anche aggiungere <code>displayname </code>riga, se non presente.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>displayname =</strong> </td> 
      <td> <p>È possibile aggiungere la riga seguente per modificare il nome di una colonna, che sospende <code>namekey/name</code> valore:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span><code>displayname=Your Value</code> </p> </td> 
     </tr> 
     <tr> 
      <td><strong>querysort</strong> </td> 
      <td>Questa riga definisce l’ordinamento dei risultati quando si fa clic sull’intestazione della colonna. Se non è presente, la colonna non può essere ordinata dopo l’esecuzione del rapporto.</td> 
     </tr> 
     <tr> 
      <td><strong>width= larghezza</strong> </td> 
      <td> <p>Questa riga rappresenta il numero di pixel utilizzati per la colonna. Se la riga viene omessa o impostata su 0 (zero), la colonna non viene visualizzata nella vista.</p> <p>Quando modifichi questo campo manualmente in modalità testo, devi aggiungere anche <code>usewidths=true</code> alla colonna.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>usewidths=true</strong> </td> 
      <td> <p>Devi utilizzare questa riga oltre al <code>width=</code> durante la personalizzazione della larghezza di una colonna. </p> </td> 
     </tr> 
     <tr> 
      <td><strong>makeFieldEditable= makeFieldModificabile</strong> </td> 
      <td> <p>Questa riga definisce se il valore visualizzato in una colonna può essere o meno modificato in linea. Se questa riga è uguale a <strong>true</strong>, il valore nella colonna è modificabile in linea. Se questa riga è uguale a <code>false</code>, il valore nella colonna non è modificabile in linea.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>link.valuefield=</strong> </td> 
      <td> <p>Inserire questa riga solo se si desidera che il valore visualizzato in una colonna venga collegato all'oggetto associato. Il collegamento apre la pagina dei dettagli dell’oggetto. Questo valore deve corrispondere al valore <code>valuefield=</code> linea. Quando inserisci questo, devi aggiungere anche il <code>link.valueformat=</code> linea. </p> <p> Ad esempio, puoi inserire <code>link.valuefield=priority</code> in una visualizzazione del problema e la Priorità del problema viene visualizzata come collegamento. Fai clic su questo collegamento per aprire la pagina Problema.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>link.valueformat=</strong> </td> 
      <td> <p>Inserire questa riga solo dopo aver inserito <code>link.valuefield</code> riga per aggiungere un collegamento al valore in una colonna. Il collegamento apre la pagina dei dettagli dell’oggetto. Questo valore deve corrispondere al valore <code>valueformat=</code> e indica il formato utilizzato per visualizzare <code>valuefield</code>. </p> <p>Importante: quando visualizzi la modalità testo in una colonna incorporata che include anche un collegamento, noterai una serie di righe che fanno riferimento al collegamento. Alcune di queste righe potrebbero non essere più supportate o non essere necessarie quando crei una colonna personalizzata in modalità testo e aggiungi le istruzioni di collegamento. Le righe obbligatorie quando si aggiunge un valore collegato sono<code> link.valuefield</code> e <code>link.valueformat</code>. </p> </td> 
     </tr> 
     <tr> 
      <td><strong>aggregator.function=</strong> </td> 
      <td> <p>Si riferisce al modo in cui vengono riepilogati i valori di ciascuna colonna. Sono presenti più righe che iniziano con <code>aggregator.</code> e si riferiscono tutti all’aggregatore che riepiloga i risultati della colonna. </p> <p>Come regola generale, il <code>aggregator.</code> righe corrispondenti a quelle dell'oggetto column. </p> 
       <div class="example" data-mc-autonum="<b>Example: </b>">
        <span class="autonumber"><span><b>Esempio: </b></span></span> 
        <p>La colonna Ore pianificate in un rapporto attività riepilogato per Somma può avere un aspetto simile al seguente: </p> 
        <div>
         <pre>textmode=true</pre>
         <pre>valuefield=workRequired</pre>
         <pre>valueformat=composto</pre>
         <pre>aggregator.function=SUM</pre>
         <pre>aggregator.valuefield=workRequired</pre>
         <pre>aggregator.displayformat=minutesAsHoursString</pre>
         <pre>aggregator.valueformat=compound</pre>
         <pre>namekey=workRequired</pre>
         <pre>shortview=false</pre> 
        </div> 
       </div> 
       <div>
        Il <code>aggregator. </code>le righe possono contenere <code>valuefield </code>o un <code>valueexpression</code>
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clic **Applica** se si desidera salvare le modifiche e continuare a modificare la visualizzazione.
1. Clic **Salva e chiudi** per salvare il report.

   Oppure

   Clic **Salva visualizzazione** per salvare la visualizzazione in un elenco.
