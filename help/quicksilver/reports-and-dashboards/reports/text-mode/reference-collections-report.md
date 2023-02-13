---
product-area: reporting
navigation-topic: text-mode-reporting
title: Riferimento alle raccolte in un rapporto
description: Riferimento alle raccolte in un rapporto
author: Nolan
feature: Reports and Dashboards
exl-id: 18ba3f4b-ae03-4694-a2fe-fdbeeb576ea9
source-git-commit: 8b6324302a70319f387d1e09d1eb92fbdabf7e32
workflow-type: tm+mt
source-wordcount: '2609'
ht-degree: 0%

---

# Riferimento alle raccolte in un rapporto

La creazione di un report in Adobe Workfront consente di visualizzare un set di oggetti, i relativi campi o gli oggetti collegati in un elenco, una griglia o un formato grafico.

Per ulteriori informazioni sulla creazione di un rapporto in Workfront, vedi [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

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
   <td> <p>Modificare l’accesso a Filtri, Visualizzazioni, Gruppi</p> <p>Accesso a rapporti, dashboard, calendari</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p> <p>Gestire le autorizzazioni per una visualizzazione, un filtro o un raggruppamento </p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Comprendere le raccolte

Un insieme è un elenco di oggetti collegati a un altro oggetto.

In Workfront sono presenti le due seguenti relazioni tra gli oggetti:

* **Una relazione uno-a-uno**: Un oggetto può essere collegato a un solo altro oggetto alla volta.\
   Ad esempio, un progetto può essere collegato a un solo portfolio alla volta.

* **Una relazione uno-a-molti**: Un oggetto può essere collegato a diversi altri oggetti alla volta.\
   Ad esempio, un progetto può avere più attività. In questo caso, l’elenco delle attività costituisce una raccolta per il progetto.

>[!IMPORTANT]
>
>È possibile creare un rapporto che mostri la relazione uno-a-uno tra gli oggetti utilizzando il generatore di report standard. Tuttavia, è possibile creare solo un rapporto che mostri la relazione uno-a-molti tra gli oggetti utilizzando l’interfaccia in modalità testo nel generatore di report.

Per ulteriori informazioni sulla creazione di un report nel generatore di report standard, vedi [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Per ulteriori informazioni sulla creazione di un rapporto tramite l’interfaccia in modalità testo, consulta:

* [Panoramica della modalità testo](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [Panoramica degli usi comuni della modalità testo](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).
* [Panoramica della sintassi della modalità testo](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)

## Trova gli oggetti raccolta e i relativi campi in API Explorer {#find-collection-objects-and-their-fields-in-the-api-explorer}

Non tutte le raccolte possono essere segnalate su .

Per comprendere quali oggetti possono essere associati a una raccolta di altri, è necessario utilizzare API Explorer.\
Per ulteriori informazioni sulla tabella di Esplora API, consulta la sezione [Esplora API](../../../wf-api/general/api-explorer.md).

Per scoprire su quali raccolte è possibile segnalare:

1. Vai a [Esplora API](../../../wf-api/general/api-explorer.md).
1. Trova l&#39;oggetto del report.
1. Seleziona la **collezioni** scheda .

   >[!NOTE]
   >
   >Solo gli oggetti elencati in questa scheda possono essere rappresentati come raccolta in un rapporto per l’oggetto selezionato.

1. Espandi l’oggetto della raccolta facendo clic su di esso.
1. Fai clic sul collegamento visualizzato per passare all’oggetto della raccolta.\
   Viene aperta la **field** scheda per l&#39;oggetto della raccolta.

   >[!NOTE]
   >
   >Nel rapporto di raccolta è possibile fare riferimento solo ai campi elencati in questa scheda oppure ai campi associati agli oggetti elencati in questa scheda.

## Raccolte di riferimento nei rapporti

È possibile fare riferimento a oggetti di una raccolta nei seguenti elementi di reporting:

* Viste
* Filtri
* Richieste

Non è possibile fare riferimento a oggetti di una raccolta nei seguenti elementi di reporting:

* Raggruppamenti
* Diagramma

Ad esempio, è possibile fare riferimento all&#39;attività o alle raccolte di problemi da un rapporto di progetto per mostrare le informazioni sull&#39;attività o sul problema a livello di progetto.

* [Fare riferimento a una raccolta nella visualizzazione di un rapporto](#reference-a-collection-in-the-view-of-a-report)
* [Fare riferimento a una raccolta nel Filtro di un rapporto](#reference-a-collection-in-the-filter-of-a-report)
* [Riferimento a una raccolta nel prompt personalizzato di un rapporto](#reference-a-collection-in-the-custom-prompt-of-a-report)

### Fare riferimento a una raccolta nella visualizzazione di un rapporto {#reference-a-collection-in-the-view-of-a-report}

È possibile fare riferimento a una raccolta di oggetti nella visualizzazione di un rapporto per mostrare gli attributi degli oggetti associati all&#39;oggetto del rapporto.

Ad esempio, è possibile visualizzare le informazioni sull&#39;attività o sul problema in un rapporto di progetto, creando una colonna di raccolta per le attività o un problema nella visualizzazione del rapporto.

È possibile visualizzare informazioni sulle attività o sui problemi, come nomi, date, assegnatari principali, percentuale di completamento, ecc. nella visualizzazione raccolta.

Nella visualizzazione vengono visualizzate le informazioni sulle attività o sui problemi in un formato elenco, con ogni riga dell&#39;elenco che rappresenta informazioni su un&#39;attività o su un problema. L’elenco delle attività o dei problemi e i relativi campi vengono visualizzati sulla stessa riga del progetto a cui appartengono le attività o i problemi.\
![issue_and_Tasks_collections_in_reports.png](assets/issue-and-tasks-collections-in-reports-350x171.png)

* [Aggiungere una colonna di raccolta in una visualizzazione rapporto](#add-a-collection-column-in-a-report-view)
* [Comprendere le righe di una visualizzazione raccolta in modalità testo](#understand-the-lines-of-a-collection-view-in-text-mode)
* [Limitazioni di una visualizzazione raccolta](#limitations-of-a-collection-view)

### Aggiungere una colonna di raccolta in una visualizzazione rapporto {#add-a-collection-column-in-a-report-view}

Per aggiungere una colonna di raccolta in una visualizzazione rapporto:

1. Fai clic sul pulsante **Principale** menu ![](assets/main-menu-icon.png), quindi fai clic su **Rapporti**.
1. Fai clic su **Nuovo rapporto**.
1. Selezionare l&#39;oggetto del rapporto.
1. Allontanarsi dal rapporto e utilizzare [Esplora API](../../../wf-api/general/api-explorer.md), determina le raccolte disponibili per l’oggetto selezionato per il rapporto.

   Per ulteriori informazioni sulla selezione dell&#39;oggetto della raccolta, consulta la sezione . [Trova gli oggetti raccolta e i relativi campi in API Explorer](#find-collection-objects-and-their-fields-in-the-api-explorer) in questo articolo.\
   Indicare il nome dell&#39;oggetto per la raccolta.

1. Utilizzo della [Esplora API](../../../wf-api/general/api-explorer.md), passare all’elenco dei campi per l’oggetto che si desidera visualizzare nella raccolta.

   Per ulteriori informazioni su come trovare i campi dell&#39;oggetto della raccolta, consulta la sezione . [Trova gli oggetti raccolta e i relativi campi in API Explorer](#find-collection-objects-and-their-fields-in-the-api-explorer) in questo articolo.

   Indicare il nome del campo che si desidera visualizzare nella raccolta.

1. Torna al rapporto e nella **Colonne (visualizzazione)** scheda , fai clic su **Aggiungi colonna**.
1. Fai clic su **Passa alla modalità testo**.
1. Passa il puntatore del mouse sulla finestra di dialogo e fai clic su **Fare clic per modificare il testo**.
1. Seleziona tutto il testo nel **Modalità testo** e rimuoverlo, quindi incollare il codice seguente se si sta facendo riferimento a un campo dell&#39;oggetto raccolta:

   ```
   valueformat=HTML
   textmode=true
   type=iterate
   listdelimiter=<p>
   displayname=Column Name
   listmethod=nested(collection object name).lists
   valuefield=collection object field
   ```

1. Sostituisci **Nome colonna** con il nome della colonna nel `displayname` linea.
1. Sostituisci **nome oggetto raccolta** con il nome dell&#39;oggetto raccolta nel `listmethod` come appare nella [Esplora API](../../../wf-api/general/api-explorer.md).

1. Sostituisci **campo oggetto raccolta** con il nome del campo dell&#39;oggetto raccolta nel `valuefield` come appare nella [Esplora API](../../../wf-api/general/api-explorer.md).

   È possibile sostituire **valuefield** con **valueexpression**, se desideri creare un’espressione personalizzata nella visualizzazione.

   Per ulteriori informazioni sulle espressioni personalizzate calcolate, consulta [Espressioni dati calcolate](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

   Ad esempio, se desideri visualizzare un elenco delle attività in un rapporto di progetto. Questa raccolta utilizza un `valuefield` riga per fare riferimento ai nomi delle attività.

   Esegui una delle operazioni seguenti:

   * Utilizza il codice seguente per generare la colonna:

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

      Tieni presente che in una raccolta devi utilizzare **questioni** per **listmethod** linea, anziché **opTasks** che è il nome del database per Problemi. Per informazioni su quando utilizzare **problema** e quando utilizzare **opTask** quando fai riferimento ai problemi, vedi [Usa &quot;opTask&quot; e &quot;issue&quot; quando si fa riferimento a problemi](../../../manage-work/issues/issue-information/use-optask-instead-of-issue.md).

   * Se desideri visualizzare un elenco delle attività in un rapporto di progetto insieme al relativo assegnatario principale, utilizza un **valueexpression** riga per fare riferimento ai nomi delle attività adiacenti ai nomi dei rispettivi assegnatari principali anziché **valuefield**.

      Utilizza il codice seguente per generare la colonna:

      ```
      valueformat=HTML
      textmode=true
      type=iterate
      listdelimiter=<p>
      displayname=Tasks Names - Primary Assignee
      listmethod=nested(tasks).lists
      valueexpression=CONCAT({name},' - ',{assignedTo}.{name})
      ```

1. Nel rapporto sul progetto viene visualizzata la colonna seguente, in cui sono elencate tutte le attività di ciascun progetto insieme alle relative assegnatarie principali:

   ![](assets/project-report-with-task-and-assignee-collection-view-nwe-350x222.png)

1. Fai clic su **Salva**.
1. (Facoltativo) Continua a modificare il rapporto.

   Oppure

   Fai clic su **Salva e chiudi** per salvare il rapporto.

#### Comprendere le righe di una visualizzazione raccolta in modalità testo

Le righe in una visualizzazione in modalità testo per una raccolta sono descritte nella tabella seguente:

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
   <td><code>valueformat=HTML</code> </td> 
   <td> <p>Puoi utilizzare vari valori per questa riga, ma ti consigliamo di <code style="font-weight: normal;">valueformat</code> per un elenco di raccolte <strong>HTML.</strong></p>
   </td> 
  </tr> 
  <tr> 
   <td><code>textmode=true</code> </td> 
   <td> <p>Questa riga indica che la colonna è stata configurata utilizzando la modalità testo. Se si rimuove questa riga, Workfront la aggiunge nuovamente per impostazione predefinita.</p> </td> 
  </tr> 
  <tr> 
   <td><code>type=iterate</code> </td> 
   <td> <p>La <code>type</code> di un elenco è sempre <code>iterate</code>, quando si crea una visualizzazione.</p> </td> 
  </tr> 
  <tr> 
   <td><code>listdelimiter=&lt;p&gt;</code> </td> 
   <td> <p>Questo è il delimitatore utilizzato per separare i valori nell’elenco.<br>Si consiglia di utilizzare <code>&lt;p&gt;</code> che aggiunge un’interruzione di riga tra i valori.</p> <p>Puoi anche utilizzare i seguenti elementi:</p> <p><code>&amp;zwj;</code> (joiner a larghezza zero). I valori della raccolta non hanno alcuna separazione.<br><strong>,</strong> =separatore virgola. I valori della raccolta sono separati da una virgola seguita da uno spazio vuoto.<br><strong>/</strong> = separatore della barra. I valori della raccolta sono separati da una barra.<br><strong>-</strong> = separatore del trattino. I valori della raccolta sono separati da un trattino.<br>Lasciando vuota questa riga, si aggiunge una virgola seguita da uno spazio tra i valori della raccolta, per impostazione predefinita.</p> </td> 
  </tr> 
  <tr> 
   <td><code>displayname=</code><em>Nome colonna</em> </td> 
   <td> <p>Sostituisci <strong>Nome colonna</strong> con il nome effettivo della nuova colonna.</p> </td> 
  </tr> 
  <tr> 
   <td><code>listmethod=nested(collection object name).list</code> </td> 
   <td> <p> Questa riga definisce la raccolta a cui fai riferimento.</p> <p>Sostituisci <strong>nome oggetto raccolta</strong> con il nome dell'oggetto a cui si fa riferimento nella raccolta, come visualizzato nella <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">Esplora API</a>. Questo valore è in genere la forma plurale del nome dell'oggetto raccolta.</p> </td> 
  </tr> 
  <tr> 
   <td><code>valuefield=collection object field</code> </td> 
   <td> <p>Questa riga definisce il campo a cui si fa riferimento dall'oggetto raccolta.</p> <p>Sostituisci <strong>campo oggetto raccolta</strong> con il nome del campo dell'oggetto a cui si fa riferimento nella raccolta, come visualizzato nella <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">Esplora API</a>.</p> <p>Puoi sostituire questa riga con:</p> <p><strong>valueexpression</strong>=campo/campi oggetto raccolta calcolato</p> <p>Utilizzo <strong>valueexpression</strong>, puoi visualizzare un’espressione personalizzata calcolata nella colonna .</p> <p>Per ulteriori informazioni sul formato <strong>valueexpression</strong> linee, vedi <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">Panoramica della sintassi della modalità testo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Limitazioni di una visualizzazione raccolta {#limitations-of-a-collection-view}

Quando crei una visualizzazione raccolta, considera le seguenti limitazioni:

* Non è possibile controllare l&#39;ordine di visualizzazione dei dati di raccolta.
* Non è possibile applicare la formattazione condizionale a una visualizzazione raccolta.
* Non è possibile fare in modo che un oggetto di una raccolta diventi un collegamento cliccabile.
* Non è possibile creare una visualizzazione raccolta di un&#39;altra raccolta.\
   Ad esempio, non è possibile visualizzare tutti gli assegnatari per ogni attività in un rapporto di progetto. È possibile visualizzare solo l&#39;assegnatario principale per ogni attività in una visualizzazione del progetto.

### Fare riferimento a una raccolta nel Filtro di un rapporto {#reference-a-collection-in-the-filter-of-a-report}

È possibile fare riferimento a una raccolta di oggetti nel filtro di un rapporto per filtrare gli attributi degli oggetti associati all&#39;oggetto del rapporto.

Ad esempio, è possibile filtrare le informazioni relative alle attività o ai problemi contenuti in un rapporto di progetto utilizzando un riferimento agli attributi delle attività o ai problemi relativi al progetto nell’istruzione filtro.

Per aggiungere un riferimento a una raccolta in un filtro di rapporto:

1. Fai clic sul pulsante **Principale** menu ![](assets/main-menu-icon.png), quindi fai clic su **Rapporti**.
1. Fai clic su **Nuovo rapporto**.
1. Selezionare l&#39;oggetto del rapporto.
1. Allontanarsi dal rapporto e utilizzare [Esplora API](../../../wf-api/general/api-explorer.md), determina le raccolte disponibili per l’oggetto selezionato per il rapporto.

   Per ulteriori informazioni sulla selezione dell&#39;oggetto della raccolta, consulta la sezione . [Trova gli oggetti raccolta e i relativi campi in API Explorer](#find-collection-objects-and-their-fields-in-the-api-explorer) in questo articolo.

   Indicare il nome dell&#39;oggetto per la raccolta.

1. Utilizzo della [Esplora API](../../../wf-api/general/api-explorer.md), passare all’elenco dei campi per l’oggetto che si desidera visualizzare nella raccolta.

   Per ulteriori informazioni su come trovare i campi dell&#39;oggetto della raccolta, consulta la sezione . [Trova gli oggetti raccolta e i relativi campi in API Explorer](#find-collection-objects-and-their-fields-in-the-api-explorer) in questo articolo.

   Prendi nota del campo che desideri visualizzare nella raccolta.

1. Torna al rapporto e nella **Filtri** scheda , fai clic su **Passa alla modalità testo**.

1. In **Impostare regole di filtro per il rapporto** area, incolla il seguente codice:

   ```
   collection object name:collection object field=collection object value
   collection object name:collection object field_Mod=value of the modifier
   ```

1. Sostituisci **nome oggetto raccolta** con il nome dell&#39;oggetto raccolta così come viene visualizzato nel [Esplora API](../../../wf-api/general/api-explorer.md). Questo valore è in genere la forma plurale del nome dell&#39;oggetto raccolta.

1. Sostituisci **campo oggetto raccolta** con il nome del campo dell&#39;oggetto raccolta in, come visualizzato nel [Esplora API](../../../wf-api/general/api-explorer.md).

1. Sostituisci **valore dell&#39;oggetto collection** con il valore dell&#39;oggetto raccolta così come viene visualizzato in Workfront.
1. Sostituisci **valore del modificatore** con un modificatore valido.

   Per un elenco dei modificatori, consulta [Modificatori di filtri e condizioni](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).\
   Ad esempio, per creare un rapporto sul progetto in cui sono visualizzati solo i progetti con attività il cui nome contiene il nome &quot;Marketing&quot;, utilizza il codice seguente:

   ```
   tasks:name=Marketing
   tasks:name_Mod=cicontains
   ```

   Questo rapporto visualizza solo i progetti il cui nome contiene almeno un’attività denominata &quot;marketing&quot;.

   ![](assets/marketing-only-tasks-in-project-report-nwe-350x309.png)

1. Per filtrare il nome di un problema, utilizza il codice seguente:

   ```
   issues:name=Marketing
   issues:name_Mod=cicontains
   ```

   >[!TIP]
   >
   >Tieni presente che devi utilizzare `issues` per il nome dell&#39;oggetto raccolta, anziché `optask` in che modo i problemi vengono visualizzati in API Explorer.

1. Fai clic su **Fine**.
1. (Facoltativo) Continua a modificare il rapporto.

   Oppure

   Fai clic su **Salva e chiudi** per salvare il rapporto.

### Riferimento a una raccolta nel prompt personalizzato di un rapporto {#reference-a-collection-in-the-custom-prompt-of-a-report}

È possibile fare riferimento a una raccolta di oggetti nel prompt personalizzato di un rapporto, per filtrare i risultati del rapporto per gli attributi degli oggetti associati all&#39;oggetto del rapporto.

Ad esempio, è possibile richiedere informazioni sulle attività in un rapporto di progetto utilizzando un riferimento agli attributi delle attività nel prompt personalizzato del rapporto.

>[!NOTE]
>
>Non è possibile fare riferimento alle raccolte in un prompt standard.

Un prompt personalizzato è un filtro personalizzato in cui le istruzioni sono collegate da simboli e commerciale. È consigliabile creare l’istruzione in un filtro, prima di tutto, unire le righe delle istruzioni con le e commerciale.

Per ulteriori informazioni sulla creazione di un’istruzione filtro con un riferimento alla raccolta, consulta la sezione . [Fare riferimento a una raccolta nel Filtro di un rapporto](#reference-a-collection-in-the-filter-of-a-report) in questo articolo.

Per aggiungere un riferimento a una raccolta nel prompt personalizzato di un rapporto:

1. Fai clic sul pulsante **Principale** menu ![](assets/main-menu-icon.png), quindi fai clic su **Rapporti**.
1. Fai clic su **Nuovo rapporto**.
1. Selezionare l&#39;oggetto del rapporto.
1. Creare un filtro con un riferimento alla raccolta come descritto nella sezione [Fare riferimento a una raccolta nel Filtro di un rapporto](#reference-a-collection-in-the-filter-of-a-report) in questo articolo.
1. Fai clic su **Impostazioni dei rapporti**.
1. Fai clic su **Richieste di rapporto**.
1. Fai clic su **Aggiungi prompt**.
1. Fai clic su **Prompt personalizzato**.
1. Specifica il nome del prompt nel **Campo***name** campo .

1. Specifica una **Etichetta elemento a discesa**.
1. Specifica quanto segue nella **Condizione** campo:

   ```
   collection object name:collection object field_Mod=value of the modifier
   ```

1. (Facoltativo) Specifica se questa opzione è visualizzata per impostazione predefinita nel prompt.
1. Sostituisci **nome oggetto raccolta** con il nome dell&#39;oggetto raccolta così come viene visualizzato nel [Esplora API](../../../wf-api/general/api-explorer.md). Questo valore è in genere la forma plurale del nome dell&#39;oggetto raccolta.
1. Sostituisci **campo oggetto raccolta** con il nome del campo dell&#39;oggetto raccolta, come visualizzato nel [Esplora API](../../../wf-api/general/api-explorer.md).
1. Sostituisci **valore dell&#39;oggetto collection** con il valore dell&#39;oggetto raccolta così come viene visualizzato in Workfront.

   Ad esempio, se filtri progetti in cui il nome dell’attività contiene &quot;Marketing&quot;, sostituisci **valore dell&#39;oggetto collection** con **marketing**.

1. Sostituisci **valore del modificatore** con un modificatore valido.

   Per un elenco dei modificatori, consulta  [Modificatori di filtri e condizioni](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   **Esempio:** Ad esempio, per creare un rapporto di progetto con un prompt personalizzato in cui visualizzare solo i progetti a cui è stata assegnata almeno un’attività a un utente specifico, utilizza il codice seguente:

   ```
   tasks:assignedToID=57cf1b7a000077c9f02f66cb09c8f86c&tasks:assignedToID_Mod=in
   ```

   Viene generato un rapporto in cui a tutti i progetti elencati è assegnata almeno un’attività all’utente il cui GUID è 57cf1b7a00077c9f02f66cb09c8f86c.

   >[!NOTE]
   >
   >Non è possibile fare riferimento al nome dell&#39;assegnatario principale (&quot;Assegnato a&quot; campo) di un&#39;attività, in base al [Esplora API](../../../wf-api/general/api-explorer.md). Puoi fare riferimento solo all’ID dell’assegnatario principale.

   Ad esempio, per filtrare i progetti in cui uno dei problemi del progetto viene assegnato a un utente specifico, utilizza il codice seguente per il prompt personalizzato:

   ```
   issues:assignedToID=57cf1b7a000077c9f02f66cb09c8f86c&issues:assignedToID_Mod=in
   ```

   Viene generato un rapporto in cui a tutti i progetti elencati è assegnato almeno un problema all’utente il cui GUID è 57cf1b7a00077c9f02f66cb09c8f86c.

   >[!NOTE]
   Tieni presente che devi utilizzare **questioni** per il nome dell&#39;oggetto raccolta. In questo momento, Esplora API non offre un nome di oggetto raccolta per i problemi.

1. Fai clic su **Fine**.
1. (Facoltativo) Continua a modificare il rapporto.

   Oppure

   Fai clic su **Salva e chiudi** per salvare il rapporto.
