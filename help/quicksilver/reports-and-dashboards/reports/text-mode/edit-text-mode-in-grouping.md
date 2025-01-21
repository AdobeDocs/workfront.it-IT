---
product-area: reporting
navigation-topic: text-mode-reporting
title: Modificare un raggruppamento utilizzando la modalità testo
description: È possibile modificare un raggruppamento in un elenco o in un report utilizzando la modalità testo per accedere a campi non disponibili nell’interfaccia standard e creare raggruppamenti più complessi.
author: Nolan
feature: Reports and Dashboards
exl-id: 2eeecc16-ea6d-4a56-8ea3-e213706e89bf
source-git-commit: e620074ab0509e3052678e8c7e46e9629f3b34f2
workflow-type: tm+mt
source-wordcount: '1537'
ht-degree: 0%

---

# Modificare un raggruppamento utilizzando la modalità testo

<!-- Audited: 1/2025 -->

È possibile modificare un raggruppamento in un elenco o in un report utilizzando la modalità testo per accedere a campi non disponibili nell’interfaccia standard e creare raggruppamenti più complessi.

>[!TIP]
>
>È consigliabile creare il più possibile il raggruppamento in modalità standard, quindi convertirlo in modalità testo per modificarlo.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Devi avere i seguenti:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> 
      <p>Nuovo:</p>
         <ul>
         <li><p>Standard</p></li>
         </ul>
      <p>Corrente:</p>
         <ul>
         <li><p>Piano</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica accesso a Filtri, Viste, Raggruppamenti</p> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari per modificare i raggruppamenti in un rapporto</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un report per modificare i raggruppamenti in un report</p> <p>Gestire le autorizzazioni per un raggruppamento per modificarlo</p></td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

Prima di iniziare a utilizzare la modalità testo in un report o in un elenco, accertati di avere sempre familiarità con la sintassi della modalità testo di Workfront.

Per ulteriori informazioni, consulta:

* [Panoramica sulla modalità testo](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [Panoramica sulla sintassi della modalità testo](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)
* [Esempi di visualizzazione, filtro e raggruppamento personalizzati: indice articolo](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## Modificare un raggruppamento utilizzando la modalità testo

La modifica di un raggruppamento utilizzando la modalità testo è identica per i report e gli elenchi. L’accesso al raggruppamento da un rapporto o da un elenco è diverso.

>[!NOTE]
>
>I raggruppamenti sono un elemento obbligatorio di reporting per la creazione di grafici nei rapporti. I raggruppamenti in modalità testo non sono supportati nei grafici. Per informazioni sull&#39;aggiunta di grafici ai report, vedere [Aggiungere un grafico a un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

Per ulteriori informazioni sulla creazione di raggruppamenti, vedere [Creare raggruppamenti in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

Per informazioni sulla creazione di un report, vedere [Creare un report personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Esegui una delle operazioni seguenti:

   1. Per accedere al raggruppamento da un report, passa al report, quindi fai clic sulla scheda **Azioni report** > **Modifica** > **Raggruppamenti**.
   1. Per accedere al raggruppamento da un elenco, passa all&#39;elenco e dal menu a discesa **Raggruppamento**, passa il puntatore del mouse sul raggruppamento da modificare e fai clic sull&#39;icona **Modifica** ![](assets/edit-icon.png).

      Viene aperto il generatore di raggruppamenti.

1. Fai clic su **Aggiungi raggruppamento** per aggiungere i raggruppamenti, fai clic su **Passa alla modalità testo** nell&#39;angolo superiore destro del generatore, quindi fai clic su **Modifica modalità testo**.

   >[!TIP]
   >
   >Puoi aggiungere fino a 3 raggruppamenti nell’interfaccia standard. È possibile aggiungere un quarto raggruppamento solo utilizzando la modalità testo e non è possibile avere più di 4 livelli di raggruppamento in Workfront.

1. Inizia a digitare il nome di un campo in base al quale desideri eseguire il raggruppamento.

   Selezionare il nome del campo quando viene visualizzato nell&#39;elenco.

1. Fare clic su **Passa alla modalità testo** nell&#39;angolo superiore destro del generatore.

   Il raggruppamento viene quindi visualizzato in modalità testo.

   Quando si modifica un raggruppamento in modalità testo, Workfront aggiunge

   ```
   textmode=true
   ```

   riga di codice per il raggruppamento. Indica che il raggruppamento viene modificato in modalità testo.

   **Esempio:** Per raggruppare un elenco di attività in base al nome del progetto e quindi in base al nome dell&#39;assegnatario principale, il raggruppamento deve essere simile al seguente, in modalità testo.

   ```
   textmode=true<br>group.0.linkedname=project<br>group.0.namekey=view.relatedcolumn<br><strong>group.0.valuefield=project:name</strong><br>group.0.namekeyargkey.0=project<br>group.0.namekeyargkey.1=name<br><strong>group.0.valueformat=string</strong><br>group.1.linkedname=assignedTo<br>group.1.namekey=view.relatedcolumn<br><strong>group.1.valuefield=assignedTo:name</strong><br>group.1.namekeyargkey.0=assignedTo<br>group.1.namekeyargkey.1=name<br><strong>group.1.valueformat=string</strong>
   ```

   >[!IMPORTANT]
   >
   >Le righe in grassetto sono obbligatorie.

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
   >
   >Le righe chiave in un raggruppamento in modalità testo sono simili alle righe necessarie per creare visualizzazioni in modalità testo.

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
      <th><strong>Riga di esempio</strong> </th> 
      <th><strong>Descrizione</strong> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td><strong> gruppo.&lt;numero&gt;.</strong> </td> 
      <td> <p>Ogni riga di codice è preceduta da questo testo. Le righe di codice che si riferiscono allo stesso campo selezionato nel raggruppamento sono numerate con lo stesso numero, come segue:</p> 
       <ul> 
        <li>Il primo raggruppamento del rapporto ha un numero di gruppo pari a 0. Tutte le righe che fanno riferimento al primo raggruppamento iniziano con <code>group.0</code>.</li> 
        <li>Il secondo raggruppamento del rapporto ha un numero di gruppo pari a 1. Tutte le righe che fanno riferimento al secondo raggruppamento iniziano con <em><code>group.1</code></em>.</li> 
        <li>Il terzo gruppo del rapporto ha un numero di gruppo pari a 2. Tutte le righe che fanno riferimento al terzo raggruppamento iniziano con <em><code>group.2</code></em>.</li> 
        <li>Solo in modalità testo è possibile aggiungere un numero di gruppo 3 per un quarto raggruppamento. Tutte le righe che fanno riferimento al quarto raggruppamento iniziano con <em><code>group.3</code></em>.</li> 
       </ul> <p>Nota: il generatore non supporta 4 raggruppamenti. Sono supportate solo quando si utilizza la modalità testo. Workfront non supporta più di 4 livelli di raggruppamenti.</p> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>valorefield</strong>=</p> </td> 
      <td> <p>Nome dell'oggetto o del campo visualizzato nel database. Per ulteriori informazioni sull'aspetto degli oggetti e dei campi nel database, vedere <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>.</p> <p>Esistono i seguenti scenari:</p> 
       <ol> 
        <li value="1"> <p> Se il nome del campo visualizzato è una frase invece di un singolo sostantivo, è necessario utilizzare la sintassi Camel Case per <code>valuefield</code>. Ad esempio, per la Data inizio pianificata di un'attività il codice è:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span><code>group.0.valuefield=plannedStartDate</code> </p> </li> 
        <li value="2"> <p>Se si desidera visualizzare un campo personalizzato, il valore <code>valuefield</code> è il nome effettivo del campo, come visualizzato nell'interfaccia. Ad esempio, per un campo personalizzato denominato "Ulteriori informazioni", il codice è:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span><code>group.0.valuefield=More information</code> </p> </li> 
        <li value="3"> <p>Se si desidera eseguire il raggruppamento in base a oggetti correlati ad altri oggetti utilizzando la riga di codice <code>valuefield</code>, i nomi e gli attributi degli oggetti sono separati da due punti.</p> <p>Un raggruppamento per nome Portfolio per un elenco di attività, ad esempio, ha il seguente valore per la riga del campo valore:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span><code>group.0.valuefield=project:portfolio:name</code> </p> <p>Indica che dall'oggetto del report (attività) è possibile accedere all'oggetto correlato successivo (progetto), quindi al seguente oggetto correlato dal progetto (portfolio) e infine al nome del portfolio (nome).</p> </li> 
       </ol> <p>Per informazioni sulla connessione tra gli oggetti, vedere la sezione <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects" class="MCXref xref">Interdipendenza e gerarchia degli oggetti</a> in <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Informazioni sugli oggetti in Adobe Workfront</a>.</p> <p>Nota: se si sceglie un campo in modalità testo non valido nell'interfaccia standard e si passa all'interfaccia standard, il raggruppamento viene eliminato.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>formato valore=</strong> </td> 
      <td> <p>Questa riga rappresenta il formato utilizzato per visualizzare <code>valuefield</code>. <code>valueformat</code> identifica se un oggetto o un campo viene visualizzato come testo, numero, percentuale o data.</p> <p>È consigliabile utilizzare <code>HTML</code> per <code>valueformat</code>, soprattutto quando si utilizza <code>valueexpression</code>, per garantire una visualizzazione ottimale delle informazioni.</p> <p>Per informazioni sui valori aggiuntivi per questa riga, vedere <a href="../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md" class="MCXref xref">Utilizzare la formattazione condizionale in modalità testo</a>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>espressione valore=</strong> </p> </td> 
      <td> <p>È possibile aggiungere questa riga per sostituire <code>valuefield</code>, se si desidera raggruppare l'elenco in base a un calcolo tra più campi.</p> <p>È necessario racchiudere <code>valuefield</code> degli oggetti tra parentesi graffe ogni volta che lo si utilizza in un <code>valueexpression</code>.</p> <p>Esistono i seguenti scenari:</p> 
       <ol> 
        <li value="1"> <p>Per visualizzare il nome di un raggruppamento in maiuscolo, utilizza:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span><code>group.0.valueexpression=UPPER({valuefield})</code> </p> <p>Il <code>valuefield</code> dell'oggetto viene digitato nel modo in cui viene visualizzato in API Explorer.</p> </li> 
        <li value="2">Se si desidera aggiungere più <code>valuefields</code> raggruppandoli in una riga <code>valueexpression </code>, è necessario separarli per un punto.<p>Ad esempio, se si desidera visualizzare il nome del portfolio in maiuscolo in un elenco di attività, è necessario utilizzare il codice seguente nella riga <code>valueexpression</code>:</p><p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span><code>group.0.valueexpression=UPPER({project}.{portfolio}.{name})</code></p><p>Se si desidera utilizzare un campo personalizzato in una riga <code>valueexpression</code>, è necessario anteporre <code>DE:</code> al nome del campo per indicare che si tratta di un campo personalizzato. Il nome del campo viene digitato nel modo in cui viene visualizzato nell’interfaccia.</p><p>Importante: <span>Quando si utilizza un campo personalizzato inserito in una sezione di un modulo personalizzato con autorizzazioni limitate per alcuni utenti, il calcolo di <code>valueexpression </code> è vuoto quando tali utenti visualizzano questo calcolo in un report. Per informazioni sulla modifica delle autorizzazioni per le sezioni dei moduli personalizzati, vedere</span> <span href="help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md"><a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Creare un modulo personalizzato</a></span>.</p><p>Ad esempio, se hai un campo personalizzato con l'etichetta "Nome sviluppatore" e desideri raggrupparlo per questo campo e visualizzarlo in maiuscolo, puoi utilizzare il seguente <code>valueexpression</code> per indicare questo:</p><p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span><code>group.0.valueexpression=UPPER({DE:Developer Name}</code>)</p><p>Quando si fa riferimento a un campo personalizzato di tipo Typeahead, utilizzare l'espressione seguente per fare riferimento al nome dell'oggetto selezionato in un campo con etichetta "Nome sviluppatore":</p><p><code>valueexpression=UPPER({DE:Developer Name:name})</code></p></li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td><strong>chiave del nome= / nome=</strong> </td> 
      <td> <p>Questa riga definisce l’etichetta di raggruppamento. In questo caso utilizza il valore abbreviato basato sulla chiave.</p> <p>Se si desidera modificare il nome del raggruppamento, è possibile modificare questo valore nel modo seguente:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span><code>group.0.name=Your Value</code> </p> <p><code>Name</code> consente di immettere qualsiasi testo per il nome del raggruppamento, mentre <code>namekey</code> richiede di immettere una chiave utilizzata per tradurre il nome di un raggruppamento.</p> <p>Per modificare il nome del raggruppamento, puoi anche aggiungere la riga <code>displayname </code>, se non è presente.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>nomevisualizzato =</strong> </td> 
      <td> <p>È possibile aggiungere la riga seguente per modificare il nome di una colonna, che sovrascrive il valore <code>namekey/name</code>:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span><code>group.0.displayname=Your Value</code> </p> <p>È consigliabile rimuovere tutte le righe che contengono <code>name </code> quando si rinomina un raggruppamento.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facoltativo) Aggiungi una delle seguenti righe di codice a un raggruppamento per indicare se i risultati del raggruppamento devono essere visualizzati in un elenco espanso o compresso. Per impostazione predefinita, i raggruppamenti vengono visualizzati espansi:


   ```
   group.0.iscollapsed=true
   ```

   se si desidera visualizzare il raggruppamento con i risultati compressi

   ```
   group.0.iscollapsed=false
   ```

   per visualizzare il raggruppamento con i risultati espansi

   <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create groupings to organize results article, Common uses of text mode, Edit groupings to organize reports, Create a Custom Report) </p>   
     -->

   >[!TIP]
   >   
   >* Quando si modificano manualmente i raggruppamenti durante la visualizzazione di un elenco, Workfront ricorda la preferenza manuale fino alla disconnessione. Quando effettui di nuovo l’accesso, l’elenco viene visualizzato in base a questa impostazione.
   >* I risultati di un raggruppamento vengono sempre visualizzati in modalità espansa dopo essere stati accessibili da un elemento del grafico.

1. Fai clic su **Fine** per salvare le modifiche e continuare a modificare il raggruppamento o il report.
1. Fai clic su **Salva raggruppamento** in un elenco o su **Salva + Chiudi** per salvare il report.
