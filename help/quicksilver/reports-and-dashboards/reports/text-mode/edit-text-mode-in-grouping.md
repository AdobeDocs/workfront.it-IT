---
product-area: reporting
navigation-topic: text-mode-reporting
title: Modificare la modalità di testo in un raggruppamento
description: 'NOTA: rendere tutti gli articoli FVG uguali per la modifica in modalità testo)"'
author: Nolan
feature: Reports and Dashboards
exl-id: 2eeecc16-ea6d-4a56-8ea3-e213706e89bf
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1559'
ht-degree: 1%

---

# Modificare la modalità di testo in un raggruppamento

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">NOTE: make all FVG articles the same for editing in text mode)</p>
-->

È possibile modificare un raggruppamento in un elenco o in un rapporto utilizzando la modalità testo per accedere ai campi non disponibili nell’interfaccia standard e creare raggruppamenti più complessi.

>[!TIP]
>
>È consigliabile creare il maggior numero possibile di raggruppamenti in modalità standard, quindi convertirli in modalità testo per modificarlo.

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
   <td> <p>Modificare l’accesso a Filtri, Visualizzazioni, Gruppi</p> <p>Modificare l’accesso a Report, Dashboard e Calendari per modificare i raggruppamenti in un report</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto per modificare i raggruppamenti in un rapporto</p> <p>Gestire le autorizzazioni per un raggruppamento per modificarlo</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
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

## Modificare la modalità di testo in un raggruppamento

La modifica di un raggruppamento utilizzando la modalità testo è identica per i rapporti e gli elenchi. L’accesso al raggruppamento da un rapporto o da un elenco è diverso.

>[!NOTE]
>
>I raggruppamenti sono un elemento di reporting obbligatorio per la creazione di grafici nei rapporti. I raggruppamenti in modalità testo non sono supportati nei grafici. Per informazioni sull’aggiunta di grafici ai rapporti, consulta [Aggiungere un grafico a un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

Per ulteriori informazioni sulla creazione di raggruppamenti, vedi [Creare raggruppamenti in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

Per informazioni sulla creazione di un rapporto, vedi [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Esegui una delle operazioni seguenti:

   1. Per accedere al raggruppamento da un rapporto, passa al rapporto e fai clic su **Azioni dei rapporti** > **Modifica** > **Raggruppamenti** scheda .
   1. Per accedere al raggruppamento da un elenco, passa all’elenco e dalla **Raggruppamento** menu a discesa, passate il puntatore del mouse sul raggruppamento da modificare e fate clic sul pulsante **Modifica** icona ![](assets/edit-icon.png).

      Viene visualizzato il generatore di gruppi.

1. Fai clic su **Aggiungi raggruppamento** per aggiungere i raggruppamenti, fai clic su **Passa alla modalità testo** nell&#39;angolo superiore destro del generatore.

   >[!TIP]
   Puoi aggiungere fino a 3 raggruppamenti nell’interfaccia standard. Puoi aggiungere un quarto raggruppamento solo utilizzando la modalità testo e non puoi avere più di 4 livelli di raggruppamento in Workfront.

1. Inizia a digitare il nome di un campo per il quale vuoi raggruppare.

   Selezionare il nome del campo quando viene visualizzato nell’elenco.

1. Fai clic su **Passa alla modalità testo** nell&#39;angolo superiore destro del generatore.

   Il raggruppamento viene quindi visualizzato in modalità testo.

   Quando modifichi un raggruppamento in modalità testo, Workfront aggiunge la variabile

   ```
   textmode=true
   ```

   riga di codice per il raggruppamento. Questo indica che il raggruppamento viene modificato in modalità testo.

   **Esempio:** Per raggruppare un elenco di attività in base al nome del progetto e quindi al nome dell&#39;assegnatario principale, in modalità testo il raggruppamento deve essere simile al seguente.

   ```
   textmode=true<br>group.0.linkedname=project<br>group.0.namekey=view.relatedcolumn<br><strong>group.0.valuefield=project:name</strong><br>group.0.namekeyargkey.0=project<br>group.0.namekeyargkey.1=name<br><strong>group.0.valueformat=string</strong><br>group.1.linkedname=assignedTo<br>group.1.namekey=view.relatedcolumn<br><strong>group.1.valuefield=assignedTo:name</strong><br>group.1.namekeyargkey.0=assignedTo<br>group.1.namekeyargkey.1=name<br><strong>group.1.valueformat=string</strong>
   ```

   >[!IMPORTANT]
   Le righe in grassetto sono obbligatorie.

   <!--
   <div class="example" data-mc-autonum="<b>Example: </b>" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <span class="autonumber"><span><b>Example: </b></span></span>
   <p>To group a list of tasks by the Project Name and then by the name of the Primary Assignee, your grouping should look like the following, in text mode:</p>
   <p><code>textmode=true</code> </p>
   <p><code>group.0.linkedname=project</code> </p>
   <p><code>group.0.namekey=view.relatedcolumn</code> </p>
   <p><code style="font-weight: bold;">group.0.valuefield=project:name</code> </p>
   <p><code>group.0.namekeyargkey.0=project</code> </p>
   <p><code>group.0.namekeyargkey.1=name</code> </p>
   <p><code style="font-weight: bold;">group.0.valueformat=string</code> </p>
   <p><code>group.1.linkedname=assignedTo</code> </p>
   <p><code>group.1.namekey=view.relatedcolumn</code> </p>
   <p><code style="font-weight: bold;">group.1.valuefield=assignedTo:name</code> </p>
   <p><code>group.1.namekeyargkey.0=assignedTo</code> </p>
   <p><code>group.1.namekeyargkey.1=nam</code>e</p>
   <p><code style="font-weight: bold;">group.1.valueformat=string</code> </p> <note type="important">
   The lines in bold are mandatory.
   </note>
   </div>
   -->

   Ogni campo del raggruppamento ha diverse righe di codice che fanno riferimento a tale campo.

   La tabella seguente delinea le linee chiave in un raggruppamento in modalità testo.

   <!--
   <div data-mc-conditions="QuicksilverOrClassic.Draft mode">
   <p>(NOTE: Should I add the group.1. information to this table and break the snippet? If yes, delete the snippet)</p>
   <p>(NOTE: this is a snippet, same as view >> same fields >>> see the steps in creating a view and add the same steps here for making a grouping)</p>
   </div>
   -->

   >[!TIP]
   Le righe chiave in un raggruppamento in modalità testo sono simili alle righe necessarie per creare le visualizzazioni in modalità testo.

   <!--
   <note type="tip">  
   <p>The key lines in a text mode grouping are similar to the lines required to build text-mode views.</p>
   </note>
   -->

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th><strong>Linea di esempio</strong> </th> 
      <th><strong>Descrizione</strong> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td><strong>gruppo.&lt;number&gt;.</strong> </td> 
      <td> <p>Ogni riga di codice è preceduta da questo testo. Le righe di codice che fanno riferimento allo stesso campo selezionato nel raggruppamento sono numerate con lo stesso numero, come segue:</p> 
       <ul> 
        <li>Il primo raggruppamento del rapporto ha un numero di gruppo pari a 0. Tutte le righe che fanno riferimento al primo raggruppamento iniziano con <code>group.0</code>.</li> 
        <li>Il secondo raggruppamento del rapporto ha un numero di gruppo pari a 1. Tutte le righe che fanno riferimento al secondo raggruppamento iniziano con <em><code>group.1</code></em>.</li> 
        <li>Il terzo gruppo del rapporto ha un numero di gruppo pari a 2. Tutte le righe che fanno riferimento al terzo raggruppamento iniziano con <em><code>group.2</code></em>.</li> 
        <li>Solo in modalità testo è possibile aggiungere un numero di gruppo di 3 per un quarto raggruppamento. Tutte le righe che fanno riferimento al quarto raggruppamento iniziano con <em><code>group.3</code></em>.</li> 
       </ul> <p>Nota: 4 raggruppamenti non supportati nel generatore. Sono supportate solo quando si utilizza la modalità testo. Workfront non supporta più di 4 livelli di raggruppamenti.</p> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>valuefield</strong>=</p> </td> 
      <td> <p>Si tratta del nome dell’oggetto o del campo visualizzato nel database. Per ulteriori informazioni sulla modalità di visualizzazione degli oggetti e dei campi nel database, vedere <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">Esplora API</a>.</p> <p>Esistono i seguenti scenari:</p> 
       <ol> 
        <li value="1"> <p> Se il nome del campo visualizzato è una frase invece di un singolo nome, è necessario utilizzare la sintassi della maiuscole/minuscole per la variabile <code>valuefield</code>. Ad esempio, per la data di inizio pianificata di un'attività, il codice è:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span><code>group.0.valuefield=plannedStartDate</code> </p> </li> 
        <li value="2"> <p>Se desideri visualizzare un campo personalizzato, la <code>valuefield</code> value è il nome effettivo del campo, come mostrato nell’interfaccia di . Ad esempio, per un campo personalizzato denominato "Ulteriori informazioni", il codice è:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span><code>group.0.valuefield=More information</code> </p> </li> 
        <li value="3"> <p>Se si desidera raggruppare gli oggetti correlati ad altri oggetti utilizzando la <code>valuefield</code> riga di codice i nomi e gli attributi degli oggetti sono separati da due punti.</p> <p>Ad esempio, un raggruppamento per nome Portfolio per un elenco di attività ha il seguente valore per la riga campo valore:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span><code>group.0.valuefield=project:portfolio:name</code> </p> <p>Indica che dall'oggetto del rapporto (attività) è possibile accedere all'oggetto correlato successivo (progetto); da lì è possibile accedere al seguente oggetto correlato dal progetto (portfolio); quindi il nome del portafoglio (nome).</p> </li> 
       </ol> <p>Per informazioni sulla connessione reciproca degli oggetti, vedere la sezione <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects" class="MCXref xref">Interdipendenza e gerarchia degli oggetti</a> in <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Comprendere gli oggetti in Adobe Workfront</a>.</p> <p>Nota: Se si sceglie un campo in modalità testo non valido nell’interfaccia standard e si passa all’interfaccia standard, il raggruppamento viene eliminato.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>valueformat=</strong> </td> 
      <td> <p>Questa riga rappresenta il formato utilizzato per visualizzare il <code>valuefield</code>. La <code>valueformat</code> identifica se un oggetto o un campo viene visualizzato come testo, numero, percentuale o data.</p> <p>Si consiglia di utilizzare <code>HTML</code> per <code>valueformat</code>, in particolare quando si utilizza <code>valueexpression</code>, per garantire la visualizzazione più accurata delle informazioni.</p> <p>Per informazioni sui valori aggiuntivi per questa riga, consulta <a href="../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md" class="MCXref xref">Utilizzare la formattazione condizionale nella modalità Testo</a>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>valueexpression=</strong> </p> </td> 
      <td> <p>Puoi aggiungere questa riga per sostituire <code>valuefield</code>, per raggruppare l’elenco in base a un calcolo tra più campi.</p> <p>Devi racchiudere la <code>valuefield</code> degli oggetti tra parentesi graffe ogni volta che lo si utilizza in una <code>valueexpression</code>.</p> <p>Esistono i seguenti scenari:</p> 
       <ol> 
        <li value="1"> <p>Per visualizzare il nome di un raggruppamento in maiuscolo, utilizza:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span><code>group.0.valueexpression=UPPER({valuefield})</code> </p> <p>La <code>valuefield</code> dell'oggetto viene scritto così come viene visualizzato in API Explorer.</p> </li> 
        <li value="2">Per aggiungere più <code>valuefields</code> stringendoli insieme in un <code>valueexpression </code>deve essere separato per un punto.<p>Ad esempio, se desideri visualizzare il nome del portfolio in maiuscolo in un elenco di attività, utilizza il seguente codice nel <code>valueexpression</code> linea:</p><p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span><code>group.0.valueexpression=UPPER({project}.{portfolio}.{name})</code></p><p>Se si desidera utilizzare un campo personalizzato in un <code>valueexpression</code> deve precedere il nome del campo di <code>DE:</code> per indicare che si tratta di un campo personalizzato. Il nome del campo viene scritto così come viene visualizzato nell’interfaccia.</p><p>Importante: <span>Quando si utilizza un campo personalizzato inserito in una sezione di modulo personalizzata con autorizzazioni limitate per alcuni utenti, il calcolo della <code>valueexpression </code>è vuoto se gli utenti visualizzano questo calcolo in un rapporto. Per informazioni sulla regolazione delle autorizzazioni per le sezioni personalizzate del modulo, vedere</span> <span href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md"><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Creare o modificare un modulo personalizzato</a></span>.</p><p>Ad esempio, se disponi di un campo personalizzato denominato "Nome sviluppatore" e desideri raggrupparli in base a questo campo e visualizzarlo in maiuscolo, puoi utilizzare quanto segue <code>valueexpression</code> per indicare quanto segue:</p><p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span><code>group.0.valueexpression=UPPER({DE:Developer Name}</code>)</p><p>Quando si fa riferimento a un campo personalizzato di tipo Typeahead, utilizzare la seguente espressione per fare riferimento al nome dell'oggetto selezionato in un campo denominato "Nome sviluppatore":</p><p><code>valueexpression=UPPER({DE:Developer Name:name})</code></p></li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td><strong>namekey= / name=</strong> </td> 
      <td> <p>Questa riga definisce l’etichetta di raggruppamento. In questo caso utilizza il valore abbreviato basato sulla chiave.</p> <p>Se desideri modificare il nome del raggruppamento, puoi modificare questo valore nel modo seguente:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span><code>group.0.name=Your Value</code> </p> <p><code>Name</code> consente di immettere qualsiasi testo per il nome del raggruppamento, mentre <code>namekey</code> richiede l’immissione di una chiave utilizzata per tradurre il nome di un raggruppamento.</p> <p>Per modificare il nome del raggruppamento, puoi anche aggiungere la <code>displayname </code>linea, se non è presente.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>displayname =</strong> </td> 
      <td> <p>È possibile aggiungere la riga seguente per modificare il nome di una colonna, che sovrascrive il <code>namekey/name</code> valore:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span><code>group.0.displayname=Your Value</code> </p> <p>È consigliabile rimuovere tutte le righe che contengono <code>name </code>quando si rinomina un raggruppamento.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facoltativo) Aggiungi una delle seguenti righe di codice a qualsiasi raggruppamento per indicare se i risultati nel raggruppamento devono essere visualizzati in un elenco espanso o compresso. Per impostazione predefinita, i raggruppamenti vengono visualizzati espansi:


   ```
   group.0.iscollapsed=true
   ```

   per visualizzare il raggruppamento con i risultati compressi

   ```
   group.0.iscollapsed=false
   ```

   per visualizzare il raggruppamento con i risultati espansi

   <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create groupings to organize results article, Common uses of text mode, Edit groupings to organize reports, Create a Custom Report) </p>   
     -->

   >[!TIP]
   * Quando si regolano manualmente i raggruppamenti quando si visualizza un elenco, Workfront ricorda le preferenze manuali fino a quando non si disconnette. Quando si effettua di nuovo l’accesso, l’elenco viene visualizzato in base a questa impostazione.
   * I risultati di un raggruppamento vengono sempre espansi dopo l’accesso da un elemento grafico.


1. Fai clic su **Fine** per salvare le modifiche e continuare a modificare il raggruppamento o il rapporto.
1. Fai clic su **Salva raggruppamento** in un elenco o **Salva e chiudi** per salvare il rapporto.
