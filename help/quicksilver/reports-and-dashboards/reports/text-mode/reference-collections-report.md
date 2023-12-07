---
product-area: reporting
navigation-topic: text-mode-reporting
title: Fare riferimento alle raccolte in un rapporto
description: Fare riferimento alle raccolte in un rapporto
author: Nolan
feature: Reports and Dashboards
exl-id: 18ba3f4b-ae03-4694-a2fe-fdbeeb576ea9
source-git-commit: 32966d4732221d73aa3397771e157b630f7d5760
workflow-type: tm+mt
source-wordcount: '2587'
ht-degree: 0%

---

# Fare riferimento alle raccolte in un rapporto

La creazione di un report in Adobe Workfront consente di visualizzare un set di oggetti, i rispettivi campi o gli oggetti collegati in un elenco, una griglia o un formato grafico.

Per ulteriori informazioni sulla creazione di un rapporto in Workfront, consulta [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

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
   <td> <p>Modifica accesso a Filtri, Viste, Raggruppamenti</p> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p> <p>Gestire le autorizzazioni per una visualizzazione, un filtro o un raggruppamento </p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

## Comprendere le raccolte

Un insieme è un elenco di oggetti collegati a un altro oggetto.

In Workfront sono disponibili le due relazioni seguenti tra gli oggetti:

* **Una relazione uno-a-uno**: è possibile collegare un oggetto a un solo altro oggetto alla volta.\
  Ad esempio, un progetto può essere collegato a un solo portfolio alla volta.

* **Una relazione uno-a-molti**: un oggetto può essere collegato a diversi altri oggetti alla volta.\
  Ad esempio, un progetto può avere più attività. In questo caso, l&#39;elenco delle attività costituisce una raccolta per il progetto.

>[!IMPORTANT]
>
>È possibile creare un report che mostra la relazione uno-a-uno tra gli oggetti utilizzando il generatore di report standard. Tuttavia, puoi creare un rapporto che mostra la relazione uno-a-molti tra gli oggetti utilizzando l’interfaccia in modalità testo nel generatore di rapporti.

Per ulteriori informazioni sulla creazione di un rapporto nel generatore di rapporti standard, consulta [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Per ulteriori informazioni sulla creazione di un rapporto tramite l’interfaccia in modalità testo, consulta:

* [Panoramica sulla modalità testo](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [Panoramica sugli usi comuni della modalità testo](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).
* [Panoramica sulla sintassi della modalità testo](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)

## Trovare gli oggetti raccolta e i relativi campi in API Explorer {#find-collection-objects-and-their-fields-in-the-api-explorer}

Non tutte le raccolte possono essere segnalate su.

Per capire quali oggetti possono essere associati a un insieme di altri, è necessario utilizzare API Explorer.\
Per ulteriori informazioni sulla tabella API Explorer, vedi [API Explorer](../../../wf-api/general/api-explorer.md).

Per scoprire su quali raccolte è possibile generare un rapporto:

1. Vai a [API Explorer](../../../wf-api/general/api-explorer.md).
1. Trova l’oggetto del rapporto.
1. Seleziona la **raccolte** scheda.

   >[!NOTE]
   >
   >Solo gli oggetti elencati in questa scheda possono essere rappresentati come un insieme in un report per l&#39;oggetto selezionato.

1. Espandere l&#39;oggetto della raccolta facendo clic su di esso.
1. Fare clic sul collegamento visualizzato per passare all&#39;oggetto della raccolta.\
   Verrà aperto il **campi** per l&#39;oggetto dell&#39;insieme.

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

* [Fare riferimento a una raccolta nella visualizzazione di un rapporto](#reference-a-collection-in-the-view-of-a-report)
* [Fare riferimento a una raccolta nel filtro di un report](#reference-a-collection-in-the-filter-of-a-report)
* [Fare riferimento a una raccolta nel prompt personalizzato di un report](#reference-a-collection-in-the-custom-prompt-of-a-report)

### Fare riferimento a una raccolta nella visualizzazione di un rapporto {#reference-a-collection-in-the-view-of-a-report}

È possibile fare riferimento a un insieme di oggetti nella visualizzazione di un report per visualizzare gli attributi degli oggetti associati all&#39;oggetto del report.

Ad esempio, è possibile visualizzare le informazioni sulle attività o sui problemi in un report di progetto creando una colonna di raccolta per le attività o i problemi nella visualizzazione del report.

È possibile visualizzare informazioni sulle attività o sui problemi, ad esempio nomi, date, assegnatari principali, percentuale di completamento e così via nella visualizzazione della raccolta.

Nella visualizzazione le informazioni sulle attività o sui problemi vengono visualizzate in formato elenco, con ogni riga dell&#39;elenco che rappresenta le informazioni su un&#39;attività o un problema. L&#39;elenco delle attività o dei problemi e i relativi campi vengono visualizzati sulla stessa riga del progetto a cui appartengono le attività o i problemi.\
![issue_and_tasks_collections_in_reports.png](assets/issue-and-tasks-collections-in-reports-350x171.png)

* [Aggiungere una colonna di raccolta in una visualizzazione report](#add-a-collection-column-in-a-report-view)
* [Comprendere le righe di una visualizzazione raccolta in modalità testo](#understand-the-lines-of-a-collection-view-in-text-mode)
* [Limitazioni di una visualizzazione raccolta](#limitations-of-a-collection-view)

### Aggiungere una colonna di raccolta in una visualizzazione report {#add-a-collection-column-in-a-report-view}

Per aggiungere una colonna di raccolta in una visualizzazione report:

1. Fai clic su **Principale** menu ![](assets/main-menu-icon.png), quindi fai clic su **Rapporti**.
1. Clic **Nuovo rapporto**.
1. Seleziona l’oggetto del rapporto.
1. Allontanarsi dal report e utilizzare [API Explorer](../../../wf-api/general/api-explorer.md), determina le raccolte disponibili per l&#39;oggetto selezionato per il report.

   Per ulteriori informazioni sulla selezione dell&#39;oggetto dell&#39;insieme, vedere la sezione [Trovare gli oggetti raccolta e i relativi campi in API Explorer](#find-collection-objects-and-their-fields-in-the-api-explorer) in questo articolo.\
   Prendere nota del nome dell&#39;oggetto per l&#39;insieme.

1. Utilizzo di [API Explorer](../../../wf-api/general/api-explorer.md), passare all&#39;elenco dei campi per l&#39;oggetto che si desidera visualizzare nell&#39;insieme.

   Per ulteriori informazioni sulla ricerca dei campi dell&#39;oggetto dell&#39;insieme, vedere la sezione [Trovare gli oggetti raccolta e i relativi campi in API Explorer](#find-collection-objects-and-their-fields-in-the-api-explorer) in questo articolo.

   Prendere nota del nome del campo da visualizzare nella raccolta.

1. Torna al report e nella sezione **Colonne (visualizzazione)** , fare clic su **Aggiungi colonna**.
1. Clic **Passa alla modalità testo**.
1. Passare il puntatore del mouse sulla finestra di dialogo e fare clic su **Fare clic per modificare il testo**.
1. Seleziona tutto il testo nel **Modalità testo** e rimuoverla, quindi incollare il codice seguente se si fa riferimento a un campo dell&#39;oggetto insieme:

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
1. Sostituisci **nome oggetto raccolta** con il nome dell&#39;oggetto raccolta in `listmethod` linea, come appare nella [API Explorer](../../../wf-api/general/api-explorer.md).

1. Sostituisci **campo oggetto raccolta** con il nome del campo dell&#39;oggetto insieme nel `valuefield` linea, come appare nella [API Explorer](../../../wf-api/general/api-explorer.md).

   È possibile sostituire **valuefield** con **valueexpression**, se desideri creare un’espressione personalizzata nella visualizzazione.

   Per ulteriori informazioni sulle espressioni personalizzate calcolate, vedi [Panoramica delle espressioni di dati calcolati](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

   Ad esempio, se si desidera visualizzare un elenco delle attività in un report di progetto. Questa raccolta utilizza un `valuefield` riga per fare riferimento ai nomi delle attività.

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

     In una raccolta devi utilizzare **problemi** per **listmethod** riga, invece di **Operazioni** che è il nome del database per Issues. Per informazioni su quando utilizzare **problema** e quando utilizzare **opTask** quando si fa riferimento ai problemi, consulta [Utilizza &quot;opTask&quot; e &quot;issue&quot; quando si fa riferimento a problemi](../../../manage-work/issues/issue-information/use-optask-instead-of-issue.md).

   * Se si desidera visualizzare un elenco delle attività in un report di progetto insieme al relativo assegnatario principale, è possibile utilizzare un **valueexpression** riga per fare riferimento ai nomi delle attività adiacenti ai nomi dei relativi assegnatari principali anziché **valuefield**.

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

   ![](assets/project-report-with-task-and-assignee-collection-view-nwe-350x222.png)

1. Fai clic su **Salva**.
1. (Facoltativo) Continua a modificare il rapporto.

   Oppure

   Clic **Salva e chiudi** per salvare il rapporto.

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
   <td> <p>È possibile utilizzare vari valori per questa riga, ma si consiglia di <code style="font-weight: normal;">valueformat</code> per un elenco di raccolta deve essere <strong>HTML.</strong></p>
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
   <td> <p>Delimitatore utilizzato per separare i valori nell'elenco.<br>È consigliabile utilizzare <code>&lt;p&gt;</code> che aggiunge un’interruzione di riga tra i valori.</p> <p>Puoi inoltre utilizzare quanto segue:</p> <p><code>&amp;zwj;</code> (unificatore a larghezza zero). I valori della raccolta non sono separati.<br><strong>,</strong> =separatore virgola. I valori della raccolta sono separati da una virgola seguita da uno spazio.<br><strong>/</strong> = separatore barra. I valori della raccolta sono separati da una barra.<br><strong>-</strong> = separatore di trattino. I valori della raccolta sono separati da un trattino.<br>Se questa riga viene lasciata vuota, per impostazione predefinita viene aggiunta una virgola seguita da uno spazio tra i valori della raccolta.</p> </td> 
  </tr> 
  <tr> 
   <td><code>displayname=</code><em>Nome colonna</em> </td> 
   <td> <p>Sostituisci <strong>Nome colonna</strong> con il nome effettivo della nuova colonna.</p> </td> 
  </tr> 
  <tr> 
   <td><code>listmethod=nested(collection object name).list</code> </td> 
   <td> <p> Questa riga definisce la raccolta a cui si fa riferimento.</p> <p>Sostituisci <strong>nome oggetto raccolta</strong> con il nome dell'oggetto a cui si fa riferimento nell'insieme, come visualizzato nel <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>. Questo valore è in genere la forma plurale del nome dell'oggetto raccolta.</p> </td> 
  </tr> 
  <tr> 
   <td><code>valuefield=collection object field</code> </td> 
   <td> <p>Questa riga definisce il campo a cui si fa riferimento dall'oggetto insieme.</p> <p>Sostituisci <strong>campo oggetto raccolta</strong> con il nome del campo dell'oggetto a cui si fa riferimento nell'insieme, come visualizzato nel <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>.</p> <p>Puoi sostituire questa riga con:</p> <p><strong>valueexpression</strong>=campi oggetto raccolta calcolati</p> <p>Utilizzo di <strong>valueexpression</strong>, è possibile visualizzare un’espressione personalizzata calcolata nella colonna.</p> <p>Per ulteriori informazioni su come formattare <strong>valueexpression</strong> righe, vedi <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">Panoramica sulla sintassi della modalità testo</a>.</p> </td> 
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

1. Fai clic su **Principale** menu ![](assets/main-menu-icon.png), quindi fai clic su **Rapporti**.
1. Clic **Nuovo rapporto**.
1. Seleziona l’oggetto del rapporto.
1. Allontanarsi dal report e utilizzare [API Explorer](../../../wf-api/general/api-explorer.md), determina le raccolte disponibili per l&#39;oggetto selezionato per il report.

   Per ulteriori informazioni sulla selezione dell&#39;oggetto dell&#39;insieme, vedere la sezione [Trovare gli oggetti raccolta e i relativi campi in API Explorer](#find-collection-objects-and-their-fields-in-the-api-explorer) in questo articolo.

   Prendere nota del nome dell&#39;oggetto per l&#39;insieme.

1. Utilizzo di [API Explorer](../../../wf-api/general/api-explorer.md), passare all&#39;elenco dei campi per l&#39;oggetto che si desidera visualizzare nell&#39;insieme.

   Per ulteriori informazioni sulla ricerca dei campi dell&#39;oggetto dell&#39;insieme, vedere la sezione [Trovare gli oggetti raccolta e i relativi campi in API Explorer](#find-collection-objects-and-their-fields-in-the-api-explorer) in questo articolo.

   Prendere nota del campo che si desidera visualizzare nella raccolta.

1. Torna al report e nella sezione **Filtri** , fare clic su **Passa alla modalità testo**.

1. In **Impostare le regole di filtro per il report** area, incolla il seguente codice:

   ```
   collection object name:collection object field=collection object value
   collection object name:collection object field_Mod=value of the modifier
   ```

1. Sostituisci **nome oggetto raccolta** con il nome dell&#39;oggetto insieme visualizzato nella [API Explorer](../../../wf-api/general/api-explorer.md). Questo valore è in genere la forma plurale del nome dell&#39;oggetto raccolta.

1. Sostituisci **campo oggetto raccolta** con il nome del campo dell&#39;oggetto insieme in, come visualizzato nel [API Explorer](../../../wf-api/general/api-explorer.md).

1. Sostituisci **valore dell&#39;oggetto raccolta** con il valore dell&#39;oggetto insieme visualizzato in Workfront.
1. Sostituisci **valore del modificatore** con un modificatore valido.

   Per un elenco dei modificatori, vedi [Modificatori di filtri e condizioni](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).\
   Ad esempio, per creare un report di progetti che visualizzi solo i progetti il cui nome contiene &quot;Marketing&quot;, utilizza il seguente codice:

   ```
   tasks:name=Marketing
   tasks:name_Mod=cicontains
   ```

   Questo report visualizza solo i progetti che hanno almeno un&#39;attività il cui nome contiene la parola &quot;marketing&quot;.

   ![](assets/marketing-only-tasks-in-project-report-nwe-350x309.png)

1. Per filtrare in base al nome di un problema, utilizza il seguente codice:

   ```
   issues:name=Marketing
   issues:name_Mod=cicontains
   ```

   >[!TIP]
   >
   >Nota che devi utilizzare `issues` per il nome dell&#39;oggetto raccolta, anziché `optask` Questo è il modo in cui vengono visualizzati i problemi in API Explorer.

1. Clic **Fine**.
1. (Facoltativo) Continua a modificare il rapporto.

   Oppure

   Clic **Salva e chiudi** per salvare il rapporto.

### Fare riferimento a una raccolta nel prompt personalizzato di un report {#reference-a-collection-in-the-custom-prompt-of-a-report}

È possibile fare riferimento a un insieme di oggetti nel prompt personalizzato di un report per filtrare i risultati del report per gli attributi degli oggetti associati all&#39;oggetto del report.

È ad esempio possibile richiedere informazioni sulle attività in un report del progetto utilizzando un riferimento agli attributi delle attività nel prompt personalizzato del report.

>[!NOTE]
>
>Non è possibile fare riferimento a raccolte in un prompt standard.

Un prompt personalizzato è un filtro personalizzato in cui le istruzioni sono unite da simboli di e commerciale. È consigliabile creare l&#39;istruzione in un filtro, quindi unire le righe delle istruzioni con il simbolo e commerciale.

Per ulteriori informazioni sulla creazione di un&#39;istruzione di filtro con un riferimento a una raccolta, vedere la sezione [Fare riferimento a una raccolta nel filtro di un report](#reference-a-collection-in-the-filter-of-a-report) in questo articolo.

Per aggiungere un riferimento a una raccolta nel prompt personalizzato di un report:

1. Fai clic su **Principale** menu ![](assets/main-menu-icon.png), quindi fai clic su **Rapporti**.
1. Clic **Nuovo rapporto**.
1. Seleziona l’oggetto del rapporto.
1. Creare un filtro con un riferimento a una raccolta come descritto nella sezione [Fare riferimento a una raccolta nel filtro di un report](#reference-a-collection-in-the-filter-of-a-report) in questo articolo.
1. Clic **Impostazioni dei rapporti**.
1. Clic **Prompt dei report**.
1. Clic **Aggiungi richiesta**.
1. Clic **Prompt personalizzato**.
1. Specifica il nome del prompt in **Nome****campo** campo.

1. Specifica un **Etichetta elemento a discesa**.
1. Specifica quanto segue in **Condizione** campo:

   ```
   collection object name:collection object field_Mod=value of the modifier
   ```

1. (Facoltativo) Specifica se questa scelta viene visualizzata per impostazione predefinita nel prompt.
1. Sostituisci **nome oggetto raccolta** con il nome dell&#39;oggetto insieme visualizzato nella [API Explorer](../../../wf-api/general/api-explorer.md). Questo valore è in genere la forma plurale del nome dell&#39;oggetto raccolta.
1. Sostituisci **campo oggetto raccolta** con il nome del campo dell&#39;oggetto insieme, come visualizzato nel [API Explorer](../../../wf-api/general/api-explorer.md).
1. Sostituisci **valore dell&#39;oggetto raccolta** con il valore dell&#39;oggetto insieme visualizzato in Workfront.

   Ad esempio, se si filtrano progetti in cui il nome dell&#39;attività contiene &quot;Marketing&quot;, sostituire **valore dell&#39;oggetto raccolta** con **marketing**.

1. Sostituisci **valore del modificatore** con un modificatore valido.

   Per un elenco dei modificatori, vedi  [Modificatori di filtri e condizioni](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   **Esempio:** Ad esempio, per creare un rapporto di progetto con un prompt personalizzato in cui visualizzare solo i progetti a cui è stata assegnata almeno un’attività, utilizza il codice seguente:

   ```
   tasks:assignedToID=57cf1b7a000077c9f02f66cb09c8f86c&tasks:assignedToID_Mod=in
   ```

   Viene generato un report in cui a tutti i progetti elencati è assegnata almeno un&#39;attività all&#39;utente il cui GUID è 57cf1b7a000077c9f02f66cb09c8f86c.

   >[!NOTE]
   >
   >Non è possibile fare riferimento al nome dell&#39;assegnatario principale (campo &quot;Assegnato a&quot;) di un&#39;attività in base al [API Explorer](../../../wf-api/general/api-explorer.md). Puoi fare riferimento solo all’ID dell’assegnatario principale.

   Ad esempio, per filtrare i progetti in cui uno dei problemi del progetto è assegnato a un utente specifico, utilizza il seguente codice per il prompt personalizzato:

   ```
   issues:assignedToID=57cf1b7a000077c9f02f66cb09c8f86c&issues:assignedToID_Mod=in
   ```

   Questo genera un rapporto in cui tutti i progetti elencati presentano almeno un problema assegnato all’utente il cui GUID è 57cf1b7a000077c9f02f66cb09c8f86c.

   >[!NOTE]
   >
   Nota che devi utilizzare **problemi** per il nome dell&#39;oggetto insieme. API Explorer non offre al momento un nome di oggetto raccolta per i problemi.

1. Clic **Fine**.
1. (Facoltativo) Continua a modificare il rapporto.

   Oppure

   Clic **Salva e chiudi** per salvare il rapporto.
