---
product-area: reporting
navigation-topic: text-mode-reporting
title: Modificare una visualizzazione utilizzando la modalità testo
description: 'NOTA: aggiungi una sezione in questo articolo: /Content/Reports and Dashboards/Reports/Reporting Elements/create-customize-views.html *** Inoltre, crea questa area nell’articolo Panoramica della modalità testo)"'
author: Nolan
feature: Reports and Dashboards
exl-id: b99a2d14-a226-4075-9b1b-ac9426fd41b8
source-git-commit: 89a6d856f9f87a67b6a2ccfb4282f9f6200b977c
workflow-type: tm+mt
source-wordcount: '1636'
ht-degree: 1%

---

# Modificare una visualizzazione utilizzando la modalità testo

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">NOTE: add a section in this article: /Content/Reports and Dashboards/Reports/Reporting Elements/create-customize-views.html *** Also, draft this area in the Text Mode overview article) </p>
-->

È possibile modificare una visualizzazione in un elenco o in un rapporto utilizzando la modalità testo per accedere ai campi non disponibili nell’interfaccia standard e creare viste più complesse.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modificare l’accesso a Filtri, Visualizzazioni, Gruppi</p> <p>Modificare l’accesso a Report, Dashboard e Calendari per modificare gli elementi di reporting in un report</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto per modificare le visualizzazioni in un rapporto</p> <p>Gestire le autorizzazioni per una visualizzazione per modificarla</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Prerequisiti

Prima di iniziare a utilizzare la modalità testo in un rapporto o in un elenco, assicurati di avere sempre familiarità con la sintassi della modalità testo di Workfront.

Per ulteriori informazioni, consulta:

* [Panoramica della modalità testo](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [Panoramica della sintassi della modalità testo](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)
* [Esempi di visualizzazione, filtro e raggruppamento personalizzati](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## Modalità Modifica testo in una visualizzazione

La modifica di una visualizzazione in modalità testo è identica per i rapporti e gli elenchi. L’accesso alla visualizzazione da un rapporto o da un elenco è diverso.

>[!TIP]
>
>È consigliabile creare la maggior parte della visualizzazione possibile in modalità standard, quindi convertirla in modalità testo per modificarla.

Per informazioni sulla creazione di visualizzazioni, vedi [Panoramica delle visualizzazioni in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

Per informazioni sulla creazione di un rapporto, vedi [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Esegui una delle operazioni seguenti:

   1. Per accedere alla visualizzazione da un rapporto, accedi al rapporto e fai clic su **Azioni dei rapporti** > **Modifica** > **Colonne (visualizzazione)** scheda .
   1. Per accedere alla visualizzazione da un elenco, vai all’elenco e dalla **Visualizza** menu a discesa, passate il puntatore del mouse sulla visualizzazione da modificare e fate clic sul pulsante **Modifica** icona ![](assets/edit-icon.png).

      Viene aperto il generatore di viste.

1. Seleziona una colonna nella visualizzazione.

   Oppure

   Seleziona la **Colonne (visualizzazione)** scheda del generatore di report, quindi seleziona una colonna.

   >[!TIP]
   >
   >Per modificare una visualizzazione utilizzando la modalità testo, è necessario modificare una colonna alla volta.

1. Fai clic su **Passa alla modalità testo** nell&#39;angolo superiore destro del generatore.

   >[!NOTE]
   >
   >Quando modifichi una colonna in modalità testo, in Workfront viene aggiunta la `textmode=true` riga di codice alla colonna. Indica che la colonna viene modificata in modalità testo.

   ![](assets/switch-to-text-mode-in-view-nwe-highlighted-350x447.png)

   La tabella seguente illustra le linee chiave in una visualizzazione in modalità testo:

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: make this a snippet and add it to the grouping article too)</p>
   -->

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Linea di esempio</th> 
      <th>Descrizione</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p><strong>valuefield</strong>=</p> </td> 
      <td> <p>Si tratta del nome dell’oggetto o del campo visualizzato nel database. Per ulteriori informazioni sulla modalità di visualizzazione degli oggetti e dei campi nel database, vedere <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">Esplora API</a>.</p> <p>Esistono i seguenti scenari:</p> 
       <ol> 
        <li value="1"> <p> Se il nome del campo visualizzato è una frase invece di un singolo nome, è necessario utilizzare la sintassi della maiuscole/minuscole per la variabile <code>valuefield</code>. Ad esempio, per la data di inizio pianificata di un'attività, il codice è: </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span><code>valuefield=plannedStartDate</code> </p> </li> 
        <li value="2"> <p>Se desideri visualizzare un campo personalizzato, la <code>valuefield</code> value è il nome effettivo del campo, come mostrato nell’interfaccia di . Ad esempio, per un campo personalizzato denominato "Ulteriori informazioni", il codice è:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span><code>valuefield=More information</code> </p> </li> 
        <li value="3"> <p>Se si desidera visualizzare oggetti correlati ad altri oggetti in una visualizzazione utilizzando <code>valuefield</code> riga di codice i nomi e gli attributi degli oggetti sono separati da due punti. </p> <p>Ad esempio, una colonna in una visualizzazione attività in cui viene visualizzato il nome del proprietario del Portfolio ha il seguente valore per la riga del campo di valore:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span><code>valuefield=project:portfolio:owner:name</code> </p> <p>Indica che dall'oggetto del report (attività) è possibile accedere all'oggetto correlato successivo (progetto), da lì è possibile accedere al seguente oggetto correlato dal progetto (portfolio), quindi al proprietario del portfolio (proprietario) e quindi al relativo nome (nome). </p> </li> 
       </ol> <p>Per informazioni sulla connessione reciproca degli oggetti, vedere la sezione <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects" class="MCXref xref">Interdipendenza e gerarchia degli oggetti</a> in <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Comprendere gli oggetti in Adobe Workfront</a>.</p> <p>Nota: Se si sceglie un campo in modalità testo non valido nell’interfaccia standard, non sarà possibile tornare all’interfaccia standard all’interno della colonna.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>valueformat=</strong> </td> 
      <td> <p>Questa riga rappresenta il formato utilizzato per visualizzare il <code>valuefield</code>. La <code>valueformat</code> identifica se un oggetto o un campo viene visualizzato come testo, numero, percentuale o data.</p> <p>Si consiglia di utilizzare <code>HTML</code> per <code>valueformat</code>, in particolare quando si utilizza <code>valueexpression</code>, per garantire la visualizzazione più accurata delle informazioni. </p> <p>Per informazioni sui valori aggiuntivi per questa riga, consulta <a href="../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md" class="MCXref xref">Utilizzare la formattazione condizionale nella modalità Testo</a>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>valueexpression=</strong> </p> </td> 
      <td> <p>Puoi aggiungere questa riga per sostituire <code>valuefield</code>, se desideri visualizzare un campo calcolato nella colonna .</p> <p>Devi racchiudere la <code>valuefield</code> degli oggetti tra parentesi graffe ogni volta che lo si utilizza in una <code>valueexpression</code>.</p> <p>Esistono i seguenti scenari: </p> 
       <ol> 
        <li value="1"> <p>Per visualizzare un campo in una colonna in maiuscolo, utilizzare:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span><code>valueexpression=UPPER({valuefield})</code> </p> <p>La <code>valuefield</code> dell'oggetto viene scritto così come viene visualizzato in API Explorer. </p> </li> 
        <li value="2">Per aggiungere più <code>valuefields</code> stringendoli insieme, dovete separarli per un punto.</li> 
        <li value="3"> <p>Ad esempio, se si desidera visualizzare il nome dell'assegnatario primario di un'attività utilizzando <code>valueexpression</code>, puoi utilizzare:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span><code>valueexpreesion={assignedTo}.{name}</code> </p> </li> 
        <li value="4"> <p>Se si desidera utilizzare un campo personalizzato in un <code>valueexpression</code> deve precedere il nome del campo di <code>DE:</code> per indicare che si tratta di un campo personalizzato. Il nome del campo viene scritto così come viene visualizzato nell’interfaccia. </p> <p>Importante: Quando si utilizza un campo personalizzato inserito in una sezione di modulo personalizzata con autorizzazioni limitate per alcuni utenti, il calcolo dell’espressione di valore è vuoto se gli utenti visualizzano questo calcolo in un rapporto. Per informazioni sulla regolazione delle autorizzazioni per le sezioni personalizzate del modulo, vedere <span href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md"><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Creare o modificare un modulo personalizzato</a></span>.</p> <p>Ad esempio, se disponi di un campo personalizzato denominato "Nome sviluppatore" e desideri visualizzare questo campo in maiuscolo in una colonna, puoi utilizzare quanto segue <code>valueexpression</code> per indicare quanto segue:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span><code>valueexpression=UPPER({DE:Developer Name}</code>) </p> <p>Quando si fa riferimento a un campo personalizzato di tipo Typeahead, utilizzare la seguente espressione per fare riferimento al nome dell'oggetto selezionato in un campo denominato "Nome sviluppatore":</p> <p><code>valueexpression=UPPER({DE:Developer Name:name})</code> </p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>descriptionkey= / description=</strong> </p> </td> 
      <td> <p>Questa riga definisce il testo di una descrizione comandi quando si posiziona il puntatore del mouse sul nome della colonna. In questo caso utilizza una chiave per tradurre il valore del nome nel testo della descrizione. Se desideri modificare la descrizione, modifica questa riga in modo da leggere: </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span><code>description=Your Value</code>.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>namekey= / name=</strong> </td> 
      <td> <p>Questa riga definisce l’etichetta della colonna. In questo caso utilizza il valore abbreviato basato sulla chiave.</p> <p>Se desideri modificare il nome della colonna, puoi modificare questo valore in: </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span><code>name=Your Value</code> </p> <p><code>Name</code> consente di immettere qualsiasi testo per il nome della colonna, mentre<code>namekey</code> richiede l’immissione di una chiave utilizzata per tradurre il nome di una colonna.</p> <p>Per modificare il nome della colonna, puoi anche aggiungere la <code>displayname </code>linea, se non è presente.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>displayname =</strong> </td> 
      <td> <p>È possibile aggiungere la riga seguente per modificare il nome di una colonna, che sospende il <code>namekey/name</code> valore:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span><code>displayname=Your Value</code> </p> </td> 
     </tr> 
     <tr> 
      <td><strong>querysort=</strong> </td> 
      <td>Questa riga definisce l’ordine dei risultati quando si fa clic sull’intestazione della colonna. Se non è presente, non è possibile ordinare la colonna dopo l’esecuzione del rapporto.</td> 
     </tr> 
     <tr> 
      <td><strong>width=</strong> </td> 
      <td> <p>Questa riga rappresenta il numero di pixel utilizzati per la colonna. Se la riga viene omessa o impostata su 0 (zero), la colonna non viene visualizzata nella vista.</p> <p>Quando si modifica manualmente questo campo in modalità testo, è necessario aggiungere anche il <code>usewidths=true</code> nella colonna.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>usewidths=true</strong> </td> 
      <td> <p>È necessario utilizzare questa riga oltre al <code>width=</code> quando si personalizza la larghezza di una colonna. </p> </td> 
     </tr> 
     <tr> 
      <td><strong>makeFieldEditable=</strong> </td> 
      <td> <p>Questa riga definisce se il valore visualizzato in una colonna è modificabile in linea o meno. Se questa riga è uguale a <strong>true</strong>, il valore nella colonna è modificabile in linea. Se questa riga è uguale a <code>false</code>, il valore nella colonna non è modificabile in linea.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>link.valuefield=</strong> </td> 
      <td> <p>Inserire questa riga solo quando si desidera che il valore visualizzato in una colonna si colleghi all'oggetto associato. Il collegamento apre la pagina dei dettagli dell’oggetto. Questo valore deve corrispondere al <code>valuefield=</code> linea. Quando inserisci questo valore, devi anche aggiungere il <code>link.valueformat=</code> linea. </p> <p> Ad esempio, puoi inserire <code>link.valuefield=priority</code> in una visualizzazione del problema e la priorità del problema viene visualizzata come collegamento. Facendo clic su questo collegamento si apre la pagina Problema .</p> </td> 
     </tr> 
     <tr> 
      <td><strong>link.valueformat=</strong> </td> 
      <td> <p>Inserisci questa riga solo quando hai inserito il <code>link.valuefield</code> per aggiungere un collegamento al valore in una colonna. Il collegamento apre la pagina dei dettagli dell’oggetto. Questo valore deve corrispondere al <code>valueformat=</code> e indica il formato utilizzato per visualizzare il <code>valuefield</code>. </p> <p>Importante: Quando visualizzi la modalità testo in una colonna incorporata che include anche un collegamento, noterai un numero di righe che fanno riferimento al collegamento. Alcune di queste righe potrebbero non essere più supportate o non essere necessarie quando crei una colonna personalizzata in modalità testo e aggiungi le istruzioni di collegamento ad essa. Le righe obbligatorie quando si aggiunge un valore collegato sono<code> link.valuefield</code> e <code>link.valueformat</code>. </p> </td> 
     </tr> 
     <tr> 
      <td><strong>aggregator.function=</strong> </td> 
      <td> <p>Si riferisce al modo in cui vengono riepilogati i valori di ciascuna colonna. Ci sono più linee che iniziano con <code>aggregator.</code> e si riferiscono tutti all'aggregatore che riassume i risultati della colonna. </p> <p>In linea generale, la <code>aggregator.</code> le righe corrispondono a quelle dell’oggetto column . </p> 
       <div class="example" data-mc-autonum="<b>Example: </b>">
        <span class="autonumber"><span><b>Esempio: </b></span></span> 
        <p>La colonna Ora pianificata in un rapporto attività riepilogato da Somma potrebbe avere l'aspetto seguente: </p> 
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
        La <code>aggregator. </code>le righe possono contenere <code>valuefield </code>o <code>valueexpression</code>
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Applica** per salvare le modifiche e continuare a modificarle.
1. Fai clic su **Salva e chiudi** per salvare il rapporto.

   Oppure

   Fai clic su **Salva visualizzazione** per salvare la visualizzazione in un elenco.
