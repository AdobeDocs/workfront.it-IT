---
product-area: reporting
navigation-topic: text-mode-reporting
title: Fare riferimento alle raccolte in un rapporto
description: Fare riferimento alle raccolte in un rapporto
author: Nolan
feature: Reports and Dashboards
exl-id: 18ba3f4b-ae03-4694-a2fe-fdbeeb576ea9
source-git-commit: af4a82ad11b57c7a7457d5d7ee74ee18494a1dc0
workflow-type: tm+mt
source-wordcount: '2539'
ht-degree: 0%

---

# Fare riferimento alle raccolte in un rapporto

<!-- Audited: 1/2025 -->

La creazione di un report in Adobe Workfront consente di visualizzare un set di oggetti, i rispettivi campi o gli oggetti collegati in un elenco, una griglia o un formato grafico.

Per ulteriori informazioni sulla creazione di un report in Workfront, vedere [Creare un report personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

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
   <td> <p>Modifica accesso a Filtri, Viste, Raggruppamenti</p> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p> <p>Gestire le autorizzazioni per una visualizzazione, un filtro o un raggruppamento </p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Comprendere le raccolte

Un insieme è un elenco di oggetti collegati a un altro oggetto.

In Workfront sono disponibili le due relazioni seguenti tra gli oggetti:

* **Relazione uno-a-uno**: un oggetto può essere collegato a un solo altro oggetto alla volta.\
  Ad esempio, un progetto può essere collegato a un solo portfolio alla volta.

* **Relazione uno-a-molti**: un oggetto può essere collegato a diversi altri oggetti contemporaneamente.\
  Ad esempio, un progetto può avere più attività. In questo caso, l&#39;elenco delle attività costituisce una raccolta per il progetto.

>[!IMPORTANT]
>
>È possibile creare un report che mostra la relazione uno-a-uno tra gli oggetti utilizzando il generatore di report standard. Tuttavia, puoi creare un rapporto che mostra la relazione uno-a-molti tra gli oggetti utilizzando l’interfaccia in modalità testo nel generatore di rapporti.

Per ulteriori informazioni sulla creazione di un report nel generatore di report standard, vedere [Creare un report personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Per ulteriori informazioni sulla creazione di un rapporto tramite l’interfaccia in modalità testo, consulta:

* [Panoramica sulla modalità testo](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [Panoramica sugli usi comuni per la modalità testo](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).
* [Panoramica sulla sintassi della modalità testo](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)

## Trovare gli oggetti raccolta e i relativi campi in API Explorer {#find-collection-objects-and-their-fields-in-the-api-explorer}

Non tutte le raccolte possono essere segnalate su.

Per capire quali oggetti possono essere associati a un insieme di altri, è necessario utilizzare API Explorer.\
Per ulteriori informazioni sulla tabella API Explorer, vedere [API Explorer](../../../wf-api/general/api-explorer.md).

Per scoprire su quali raccolte è possibile generare un rapporto:

1. Vai a [API Explorer](../../../wf-api/general/api-explorer.md).
1. Trova l’oggetto del rapporto.
1. Seleziona la scheda **raccolte**.

   >[!NOTE]
   >
   >Solo gli oggetti elencati in questa scheda possono essere rappresentati come un insieme in un report per l&#39;oggetto selezionato.

1. Espandere l&#39;oggetto della raccolta facendo clic su di esso.
1. Fare clic sul collegamento visualizzato per passare all&#39;oggetto della raccolta.\
   Verrà aperta la scheda **fields** per l&#39;oggetto della raccolta.

   >[!NOTE]
   >
   >Nel report di raccolta o nei campi associati agli oggetti elencati in questa scheda è possibile fare riferimento solo ai campi elencati in questa scheda.

## Fare riferimento alle raccolte nei rapporti

È possibile fare riferimento a oggetti di una raccolta nei seguenti elementi di reporting:

* Viste
* Filtri
* Prompt

Non è possibile fare riferimento a oggetti di un insieme nei seguenti elementi di reporting:

* Raggruppamenti
* Diagramma

Ad esempio, puoi fare riferimento alle raccolte di attività o problemi da un rapporto di progetto, per mostrare le informazioni su attività o problemi a livello di progetto.

* [Fare riferimento a una raccolta nella visualizzazione di un report](#reference-a-collection-in-the-view-of-a-report)
* [Fare riferimento a una raccolta nel filtro di un report](#reference-a-collection-in-the-filter-of-a-report)
* [Fare riferimento a una raccolta nel prompt personalizzato di un report](#reference-a-collection-in-the-custom-prompt-of-a-report)

### Fare riferimento a una raccolta nella visualizzazione di un rapporto {#reference-a-collection-in-the-view-of-a-report}

È possibile fare riferimento a un insieme di oggetti nella visualizzazione di un report per visualizzare gli attributi degli oggetti associati all&#39;oggetto del report.

Ad esempio, è possibile visualizzare le informazioni sulle attività o sui problemi in un report di progetto creando una colonna di raccolta per le attività o i problemi nella visualizzazione del report.

È possibile visualizzare informazioni sulle attività o sui problemi, ad esempio nomi, date, assegnatari principali, percentuale di completamento e così via nella visualizzazione della raccolta.

Nella visualizzazione le informazioni sulle attività o sui problemi vengono visualizzate in formato elenco, con ogni riga dell&#39;elenco che rappresenta le informazioni su un&#39;attività o un problema. L&#39;elenco delle attività o dei problemi e i relativi campi vengono visualizzati sulla stessa riga del progetto a cui appartengono le attività o i problemi.

![issue_and_tasks_collections_in_reports.png](assets/issue-and-tasks-collections-in-reports-350x171.png){width=400}

* [Aggiungere una colonna della raccolta in una visualizzazione report](#add-a-collection-column-in-a-report-view)
* [Comprendere le righe di una visualizzazione raccolta in modalità testo](#understand-the-lines-of-a-collection-view-in-text-mode)
* [Limitazioni di una visualizzazione raccolta](#limitations-of-a-collection-view)

### Aggiungere una colonna di raccolta in una visualizzazione report {#add-a-collection-column-in-a-report-view}

Per aggiungere una colonna di raccolta in una visualizzazione report:

1. Fai clic sul menu **Principale** ![](assets/main-menu-icon.png), quindi fai clic su **Rapporti**.
1. Fare clic su **Nuovo report**.
1. Seleziona l’oggetto del rapporto.
1. Esci dal report e, utilizzando [API Explorer](../../../wf-api/general/api-explorer.md), determina quali raccolte sono disponibili per l&#39;oggetto selezionato per il report.

   Per ulteriori informazioni sulla selezione dell&#39;oggetto della raccolta, vedere la sezione [Trova gli oggetti della raccolta e i relativi campi in API Explorer](#find-collection-objects-and-their-fields-in-the-api-explorer) in questo articolo.

   Prendere nota del nome dell&#39;oggetto per l&#39;insieme.

1. Utilizzando [API Explorer](../../../wf-api/general/api-explorer.md), vai all&#39;elenco dei campi per l&#39;oggetto che desideri visualizzare nell&#39;insieme.

   Per ulteriori informazioni sulla ricerca dei campi dell&#39;oggetto della raccolta, vedere la sezione [Trova gli oggetti della raccolta e i relativi campi in API Explorer](#find-collection-objects-and-their-fields-in-the-api-explorer) in questo articolo.

   Prendere nota del nome del campo da visualizzare nella raccolta.

1. Torna al report e nella scheda **Colonne (Visualizzazione)** fai clic su **Aggiungi colonna**.
1. Fare clic su **Passa alla modalità testo**.
1. Fare clic su **Modifica modalità testo**.
1. Selezionare tutto il testo nella finestra di dialogo **Modalità testo** e rimuoverlo, quindi incollare il codice seguente se si fa riferimento a un campo dell&#39;oggetto raccolta:

   ```
   valueformat=HTML
   textmode=true
   type=iterate
   listdelimiter=<p>
   displayname=Column Name
   listmethod=nested(collection object name).lists
   valuefield=collection object field
   ```

1. Sostituisci **Nome colonna** con il nome della colonna nella riga `displayname`.
1. Sostituisci **nome oggetto raccolta** con il nome dell&#39;oggetto raccolta nella riga `listmethod`, come visualizzato in [API Explorer](../../../wf-api/general/api-explorer.md).

1. Sostituisci il campo **oggetto raccolta** con il nome del campo dell&#39;oggetto raccolta nella riga `valuefield`, come visualizzato in [API Explorer](../../../wf-api/general/api-explorer.md).

   È possibile sostituire **valuefield** con **valueexpression**, se si desidera creare un&#39;espressione personalizzata nella visualizzazione.

   Per ulteriori informazioni sulle espressioni personalizzate calcolate, vedere [Panoramica delle espressioni di dati calcolati](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

   Ad esempio, se si desidera visualizzare un elenco delle attività in un report di progetto. Questa raccolta utilizza una riga `valuefield` per fare riferimento ai nomi delle attività.

   Esegui una delle operazioni seguenti:

   * Utilizza il seguente codice per generare la colonna:

     ```
     valueformat=HTML
     textmode=true
     type=iterate
     listdelimiter=<p>
     displayname=Project Tasks Names
     listmethod=nested(tasks).lists
     valuefield=name
     ```

   * Utilizza il codice seguente per visualizzare un elenco dei problemi nel rapporto:

     ```
     displayname=Project Issues Names
     listdelimiter=<p>
     listmethod=nested(issues).lists
     textmode=true
     type=iterate
     valuefield=name
     valueformat=HTML
     ```

     In una raccolta è necessario utilizzare **issues** per la riga **listmethod**, invece di **opTasks** che è il nome del database per Issues. Per informazioni su quando utilizzare **problema** e quando utilizzare **opTask** quando si fa riferimento a problemi, vedi [Utilizzare &quot;opTask&quot; e &quot;problema&quot; quando si fa riferimento a problemi](../../../manage-work/issues/issue-information/use-optask-instead-of-issue.md).

   * Se si desidera visualizzare un elenco delle attività in un report di progetto insieme all&#39;assegnatario principale, utilizzare una riga **valueexpression** per fare riferimento ai nomi delle attività adiacenti ai nomi degli assegnatari principali anziché **valuefield**.

     Utilizza il seguente codice per generare la colonna:

     ```
     valueformat=HTML
     textmode=true
     type=iterate
     listdelimiter=<p>
     displayname=Tasks Names - Primary Assignee
     listmethod=nested(tasks).lists
     valueexpression=CONCAT({name},' - ',{assignedTo}.{name})
     ```

1. Nel rapporto del progetto viene visualizzata la colonna seguente, in cui sono elencate tutte le attività di ciascun progetto insieme ai relativi assegnatari principali:

   ![](assets/project-report-with-task-and-assignee-collection-view-nwe-350x222.png){width=400}

1. Fai clic su **Salva**.
1. (Facoltativo) Continua a modificare il rapporto.

   Oppure

   Fare clic su **Salva + Chiudi** per salvare il report.

#### Comprendere le righe di una visualizzazione raccolta in modalità testo

Nella tabella seguente vengono descritte le righe di una raccolta in modalità testo:

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
   <td><code>valueformat=HTML</code> </td> 
   <td> <p>È possibile utilizzare vari valori per questa riga, ma si consiglia che <code style="font-weight: normal;">valueformat</code> per un elenco di raccolte sia <strong>HTML.</strong></p>
   </td> 
  </tr> 
  <tr> 
   <td><code>textmode=true</code> </td> 
   <td> <p>Questa riga indica che la colonna è stata configurata utilizzando la modalità testo. Se rimuovi questa riga, Workfront la aggiunge nuovamente per impostazione predefinita.</p> </td> 
  </tr> 
  <tr> 
   <td><code>type=iterate</code> </td> 
   <td> <p>Il <code>type</code> di un elenco è sempre <code>iterate</code>, durante la creazione di una visualizzazione.</p> </td> 
  </tr> 
  <tr> 
   <td><code>listdelimiter=&lt;p&gt;</code> </td> 
   <td> <p>Delimitatore utilizzato per separare i valori nell'elenco.<br>È consigliabile utilizzare <code>&lt;p&gt;</code>, che aggiunge un'interruzione di riga tra i valori.</p> <p>Puoi inoltre utilizzare quanto segue:</p> <p><code>&amp;zwj;</code> (unificatore a larghezza zero). I valori della raccolta non sono separati.<br><strong>,</strong> =separatore virgola. I valori della raccolta sono separati da una virgola seguita da uno spazio.<br><strong>/</strong> = separatore barra. I valori della raccolta sono separati da una barra.<br><strong>-</strong> = separatore di trattini. I valori della raccolta sono separati da un trattino.<br>Se si lascia vuota questa riga, per impostazione predefinita viene aggiunta una virgola seguita da uno spazio tra i valori della raccolta.</p> </td> 
  </tr> 
  <tr> 
   <td><code>displayname=</code><em>Nome colonna</em> </td> 
   <td> <p>Sostituisci <strong>Nome colonna</strong> con il nome effettivo della nuova colonna.</p> </td> 
  </tr> 
  <tr> 
   <td><code>listmethod=nested(collection object name).list</code> </td> 
   <td> <p> Questa riga definisce la raccolta a cui si fa riferimento.</p> <p>Sostituire <strong>nome oggetto raccolta</strong> con il nome dell'oggetto a cui si fa riferimento nella raccolta, come visualizzato in <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>. Questo valore è in genere la forma plurale del nome dell'oggetto raccolta.</p> </td> 
  </tr> 
  <tr> 
   <td><code>valuefield=collection object field</code> </td> 
   <td> <p>Questa riga definisce il campo a cui si fa riferimento dall'oggetto insieme.</p> <p>Sostituisci il campo <strong>oggetto raccolta</strong> con il nome del campo dell'oggetto a cui si fa riferimento nella raccolta, come visualizzato in <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>.</p> <p>Puoi sostituire questa riga con:</p> <p><strong>valueexpression</strong>=campi/campi oggetto raccolta calcolati</p> <p>Utilizzando <strong>valueexpression</strong>, puoi  visualizza un’espressione personalizzata calcolata nella colonna.</p> <p>Per ulteriori informazioni su come formattare <strong>righe di espressione di valore</strong>, vedere <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">Panoramica sulla sintassi della modalità testo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Limitazioni di una visualizzazione raccolta {#limitations-of-a-collection-view}

Quando crei una vista di raccolta, considera le seguenti limitazioni:

* Non è possibile controllare l&#39;ordine di visualizzazione dei dati della raccolta.
* Non è possibile applicare la formattazione condizionale a una visualizzazione raccolta.
* Non è possibile impostare un oggetto di un insieme come collegamento selezionabile.
* Non è possibile creare una visualizzazione raccolta di un&#39;altra raccolta.\
  Ad esempio, non è possibile visualizzare tutti gli assegnatari di ogni attività in un report di progetto. È possibile visualizzare solo l&#39;assegnatario principale per ogni attività in una visualizzazione di progetto.

### Fare riferimento a una raccolta nel filtro di un report {#reference-a-collection-in-the-filter-of-a-report}

È possibile fare riferimento a un insieme di oggetti nel filtro di un report per filtrare gli attributi degli oggetti associati all&#39;oggetto del report.

Ad esempio, è possibile filtrare le informazioni su attività o problemi in un report di progetto utilizzando un riferimento agli attributi delle attività o dei problemi sul progetto nell&#39;istruzione di filtro.

Per aggiungere un riferimento a una raccolta in un filtro di report:

1. Fai clic sul menu **Principale** ![](assets/main-menu-icon.png), quindi fai clic su **Rapporti**.
1. Fare clic su **Nuovo report**.
1. Seleziona l’oggetto del rapporto.
1. Esci dal report e, utilizzando [API Explorer](../../../wf-api/general/api-explorer.md), determina quali raccolte sono disponibili per l&#39;oggetto selezionato per il report.

   Per ulteriori informazioni sulla selezione dell&#39;oggetto della raccolta, vedere la sezione [Trova gli oggetti della raccolta e i relativi campi in API Explorer](#find-collection-objects-and-their-fields-in-the-api-explorer) in questo articolo.

   Prendere nota del nome dell&#39;oggetto per l&#39;insieme.

1. Utilizzando [API Explorer](../../../wf-api/general/api-explorer.md), vai all&#39;elenco dei campi per l&#39;oggetto che desideri visualizzare nell&#39;insieme.

   Per ulteriori informazioni sulla ricerca dei campi dell&#39;oggetto della raccolta, vedere la sezione [Trova gli oggetti della raccolta e i relativi campi in API Explorer](#find-collection-objects-and-their-fields-in-the-api-explorer) in questo articolo.

   Prendere nota del campo che si desidera visualizzare nella raccolta.

1. Tornare al report e nella scheda **Filtri** fare clic su **Passa alla modalità testo** e quindi su **Modifica modalità testo**.

1. Nell&#39;area **Imposta regole filtro per il report**, incolla il seguente codice:

   ```
   collection object name:collection object field=collection object value
   collection object name:collection object field_Mod=value of the modifier
   ```

1. Sostituisci **nome oggetto raccolta** con il nome dell&#39;oggetto raccolta come visualizzato in [API Explorer](../../../wf-api/general/api-explorer.md). Questo valore è in genere la forma plurale del nome dell&#39;oggetto raccolta.

1. Sostituisci il campo **oggetto raccolta** con il nome del campo dell&#39;oggetto raccolta in, come visualizzato in [API Explorer](../../../wf-api/general/api-explorer.md).

1. Sostituire **il valore dell&#39;oggetto raccolta** con il valore dell&#39;oggetto raccolta visualizzato in Workfront.
1. Sostituisci **il valore del modificatore** con un modificatore valido.

   Per un elenco dei modificatori, vedere [Filtro e modificatori di condizione](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).\
   Ad esempio, per creare un report di progetti che visualizzi solo i progetti il cui nome contiene &quot;Marketing&quot;, utilizza il seguente codice:

   ```
   tasks:name=Marketing
   tasks:name_Mod=cicontains
   ```

   Questo report visualizza solo i progetti che hanno almeno un&#39;attività il cui nome contiene la parola &quot;marketing&quot;.

   ![](assets/marketing-only-tasks-in-project-report-nwe-350x309.png){width=400}

1. Per filtrare in base al nome di un problema, utilizza il seguente codice:

   ```
   issues:name=Marketing
   issues:name_Mod=cicontains
   ```

   >[!TIP]
   >
   >Si noti che è necessario utilizzare `issues` per il nome dell&#39;oggetto della raccolta, anziché `optask`, che è il modo in cui vengono visualizzati i problemi in API Explorer.

1. Fai clic su **Fine**.
1. (Facoltativo) Continua a modificare il rapporto.

   Oppure

   Fare clic su **Salva + Chiudi** per salvare il report.

### Fare riferimento a una raccolta nel prompt personalizzato di un report {#reference-a-collection-in-the-custom-prompt-of-a-report}

È possibile fare riferimento a un insieme di oggetti nel prompt personalizzato di un report per filtrare i risultati del report per gli attributi degli oggetti associati all&#39;oggetto del report.

È ad esempio possibile richiedere informazioni sulle attività in un report del progetto utilizzando un riferimento agli attributi delle attività nel prompt personalizzato del report.

>[!NOTE]
>
>Non è possibile fare riferimento a raccolte in un prompt standard.

Un prompt personalizzato è un filtro personalizzato in cui le istruzioni sono unite da simboli di e commerciale. È consigliabile creare l&#39;istruzione in un filtro, quindi unire le righe delle istruzioni con il simbolo e commerciale.

Per ulteriori informazioni sulla creazione di un&#39;istruzione di filtro con un riferimento a una raccolta, vedere la sezione [Fare riferimento a una raccolta nel filtro di un report](#reference-a-collection-in-the-filter-of-a-report) in questo articolo.

Per aggiungere un riferimento a una raccolta nel prompt personalizzato di un report:

1. Fai clic sul menu **Principale** ![](assets/main-menu-icon.png), quindi fai clic su **Rapporti**.
1. Fare clic su **Nuovo report**.
1. Seleziona l’oggetto del rapporto.
1. Creare un filtro con un riferimento a una raccolta come descritto nella sezione [Fare riferimento a una raccolta nel filtro di un report](#reference-a-collection-in-the-filter-of-a-report) in questo articolo.
1. Fare clic su **Impostazioni report**.
1. Fai clic su **Prompt dei rapporti**.
1. Fare clic su **Aggiungi prompt**.
1. Fare clic su **Prompt personalizzato**.
1. Specifica il nome della richiesta nel campo **Field****name**.

1. Specificare un&#39;etichetta **per elemento a discesa**.
1. Specifica quanto segue nel campo **Condizione**:

   ```
   collection object name:collection object field_Mod=value of the modifier
   ```

1. (Facoltativo) Specifica se questa scelta viene visualizzata per impostazione predefinita nel prompt.
1. Sostituisci **nome oggetto raccolta** con il nome dell&#39;oggetto raccolta come visualizzato in [API Explorer](../../../wf-api/general/api-explorer.md). Questo valore è in genere la forma plurale del nome dell&#39;oggetto raccolta.
1. Sostituisci il campo **oggetto raccolta** con il nome del campo dell&#39;oggetto raccolta, come visualizzato in [API Explorer](../../../wf-api/general/api-explorer.md).
1. Sostituire **il valore dell&#39;oggetto raccolta** con il valore dell&#39;oggetto raccolta visualizzato in Workfront.

   Ad esempio, se si filtrano progetti in cui il nome dell&#39;attività contiene &quot;Marketing&quot;, sostituire **il valore dell&#39;oggetto raccolta** con **marketing**.

1. Sostituisci **il valore del modificatore** con un modificatore valido.

   Per un elenco dei modificatori, vedere [Filtro e modificatori di condizione](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   **Esempio:** Ad esempio, per creare un report di progetti con un prompt personalizzato in cui si desidera visualizzare solo i progetti a cui è stata assegnata almeno un&#39;attività, utilizzare il codice seguente:

   ```
   tasks:assignedToID=57cf1b7a000077c9f02f66cb09c8f86c&tasks:assignedToID_Mod=in
   ```

   Viene generato un report in cui a tutti i progetti elencati è assegnata almeno un&#39;attività all&#39;utente il cui GUID è 57cf1b7a000077c9f02f66cb09c8f86c.

   >[!NOTE]
   >
   >Impossibile fare riferimento al nome dell&#39;assegnatario primario (campo &quot;Assigned To&quot;) di un&#39;attività, in base a [API Explorer](../../../wf-api/general/api-explorer.md). Puoi fare riferimento solo all’ID dell’assegnatario principale.

   Ad esempio, per filtrare i progetti in cui uno dei problemi del progetto è assegnato a un utente specifico, utilizza il seguente codice per il prompt personalizzato:

   ```
   issues:assignedToID=57cf1b7a000077c9f02f66cb09c8f86c&issues:assignedToID_Mod=in
   ```

   Questo genera un rapporto in cui tutti i progetti elencati presentano almeno un problema assegnato all’utente il cui GUID è 57cf1b7a000077c9f02f66cb09c8f86c.

   >[!NOTE]
   >
   >È necessario utilizzare **issues** per il nome dell&#39;oggetto raccolta. API Explorer non offre al momento un nome di oggetto raccolta per i problemi.

1. Fai clic su **Fine**.
1. (Facoltativo) Continua a modificare il rapporto.

   Oppure

   Fare clic su **Salva + Chiudi** per salvare il report.
