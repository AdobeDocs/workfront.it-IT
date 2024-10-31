---
content-type: overview;reference
product-area: reporting
navigation-topic: reporting-navigation-topic
title: Introduzione ai rapporti
description: I rapporti forniscono visibilità su ciò che sta accadendo con gli utenti e il lavoro. Utilizzando i rapporti, puoi visualizzare informazioni sugli oggetti in Adobe Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: 478512af-a47c-4488-878a-581e238e0064
source-git-commit: f30bed961b339e20c0693a8b5e485f872375b688
workflow-type: tm+mt
source-wordcount: '3296'
ht-degree: 0%

---

# Introduzione ai rapporti

<!-- Audited: 12/2023 -->

I rapporti forniscono visibilità su ciò che sta accadendo con gli utenti e il lavoro. Utilizzando i rapporti, puoi visualizzare informazioni sugli oggetti in Adobe Workfront.

Per informazioni su come comprendere gli oggetti e come segnalarli nell&#39;applicazione Workfront, vedi [Panoramica sugli oggetti di Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Elementi del rapporto

I rapporti sono una combinazione dei seguenti tre elementi in Workfront:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Visualizza</td> 
   <td> <li>Definisce le colonne del report e le informazioni che è possibile includere in ogni colonna.</li> <li>Per informazioni sulle visualizzazioni, vedere <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Panoramica delle visualizzazioni in Adobe Workfront</a>.</li> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Raggruppamento</td> 
   <td> <li>Classifica le informazioni in base a un'informazione comune ed elenca i risultati del rapporto sotto i titoli.</li> <li>Per informazioni sui raggruppamenti, vedere <a href="../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md" class="MCXref xref">Panoramica sui raggruppamenti in Adobe Workfront</a>.</li> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Filtro</td> 
   <td> <li>Controlla la quantità di informazioni visualizzate in un report.</li> <li>Per informazioni sui filtri, vedere <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">Panoramica sui filtri</a>.</li> <li>Per informazioni sui modificatori di filtro, vedere <a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">Modificatori di filtro e di condizione</a>.</li> <li>Puoi filtrare utilizzando i caratteri jolly, per rendere i filtri più generali e dare loro maggiore flessibilità di utilizzo.</li> <li>Per informazioni sull'utilizzo dei caratteri jolly nei filtri, vedere <a href="../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md" class="MCXref xref">Variabili filtro con caratteri jolly</a>.</li> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Quando selezioni un nuovo filtro, una nuova visualizzazione o un nuovo raggruppamento da un elenco, tale selezione viene mantenuta anche se esci da Workfront o chiudi il browser.

Per informazioni sugli elementi del report, vedere [Elementi del report: filtri, visualizzazioni e raggruppamenti](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

Per migliorare i rapporti, puoi aggiungere i seguenti elementi:

* Un grafico: una rappresentazione visiva dei risultati nel rapporto.\
  Per informazioni sui report grafico, vedere [Aggiungere un grafico a un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* Un raggruppamento di matrici: riepiloga le informazioni del rapporto in un formato di tabella aggregata.\
  Per informazioni sui report matrice, vedere [Creare un report matrice](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

* Un prompt: un filtro aperto che puoi personalizzare e applicare in modo diverso ogni volta che esegui il rapporto.\
  Per informazioni sui prompt, vedere [Aggiungere un prompt a un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

Durante la creazione di un rapporto, puoi modificare singolarmente uno di questi elementi nel Report Builder.

Un altro modo per migliorare la pertinenza delle informazioni incluse nei rapporti consiste nell’applicare la formattazione condizionale alle viste. Per informazioni sull&#39;utilizzo della formattazione condizionale, vedere [Utilizzare la formattazione condizionale nelle visualizzazioni](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

## Rapporti di sistema

Workfront fornisce diversi rapporti di sistema caricati nel sistema per impostazione predefinita.\
Dopo aver inserito le informazioni nel sistema, puoi utilizzare questi rapporti per visualizzarle visivamente.

Per ulteriori informazioni su come accedere ai report di sistema e quali report di sistema sono disponibili, vedere [Utilizzare i report incorporati di Adobe Workfront](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md).

## Creare rapporti

Oltre ai rapporti sul sistema forniti da Workfront, puoi creare rapporti personalizzati per soddisfare le esigenze della tua organizzazione.

Per creare un rapporto è possibile effettuare una delle seguenti operazioni:

* Crea un rapporto da zero.
* Copia un rapporto esistente.

  Per copiare un report creato da un altro utente è necessario disporre almeno dell&#39;autorizzazione Visualizzazione. Per ulteriori informazioni sulla copia di un report, vedere [Creare una copia di un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

Per informazioni sulla creazione di report, vedere [Creare un report personalizzato](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

### Prerequisiti per la creazione di rapporti {#prerequisites-for-creating-reports}

* Per creare rapporti personalizzati è necessario disporre di una licenza Pianificazione (licenze correnti) o di una licenza Standard (nuove licenze).

  Per informazioni sui tipi di licenza di Workfront, vedere [Panoramica licenze](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md) per le licenze correnti e [Panoramica nuove licenze](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md) per le nuove licenze.

* L’amministratore di Workfront deve consentire l’accesso alla funzione di modifica dei rapporti nel proprio livello di accesso.

  Per informazioni su come concedere l&#39;accesso a Modifica report, vedere [Concedere l&#39;accesso a report, dashboard e calendari](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

* L’amministratore di Workfront deve consentire l’accesso a Modifica filtri, visualizzazioni e raggruppamenti nel livello di accesso.

  Per informazioni sulla concessione dell&#39;accesso a Modifica filtri, viste e raggruppamenti, vedere [Concedere l&#39;accesso a filtri, viste e raggruppamenti](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

* È necessario definire un oggetto per il quale si desidera creare un rapporto. I report sono specifici per gli oggetti in Workfront e per iniziare a creare il report è necessario selezionare un tipo di oggetto. È possibile creare rapporti solo sugli oggetti disponibili nell’interfaccia di Workfront.

### Proprietà del rapporto {#report-ownership}

Quando crei un rapporto in Workfront, ne diventi il proprietario predefinito e viene visualizzato nella sezione I miei rapporti. Non è possibile cambiare il proprietario di un report.

Quando si copia un report, si diventa automaticamente il proprietario del report copiato.
Per informazioni sulla copia dei report, vedere [Creare una copia di un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

Puoi vedere chi possiede un report esaminando il campo **Inserito da**.

![Campo Inserito da](assets/unshimmed-entered-by.png)

### Creare rapporti nell’interfaccia di generazione {#create-reports-in-the-builder-interface}

Per creare un nuovo rapporto, è consigliabile utilizzare prima l’interfaccia di creazione del rapporto. L’interfaccia offre un set di strumenti semplificati che ti guida attraverso la creazione di elementi per creare il rapporto desiderato. Puoi selezionare dagli elenchi e aggiungere oggetti e campi a tutti gli elementi di reporting.\
Per ulteriori informazioni sulla creazione di report nell&#39;interfaccia di creazione report, vedere [Creare un report personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Per un elenco degli oggetti per i quali è possibile creare un report, vedere la sezione [Report sugli oggetti](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#report-on-objects) nell&#39;articolo [Panoramica sugli oggetti di Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

Per ulteriori informazioni sui campi che è possibile visualizzare nei report, vedere [Glossario della terminologia di Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

### Creare rapporti in modalità testo {#create-reports-in-text-mode}

Talvolta potresti non essere in grado di trovare alcuni campi nell’interfaccia del generatore, ma potrebbero essere disponibili nell’API.\
Per informazioni sui campi disponibili nell&#39;API, vedere l&#39;articolo [API Explorer](../../../wf-api/general/api-explorer.md).

Per informazioni sull&#39;utilizzo di API Explorer, vedere l&#39;articolo [Utilizzo di API Explorer](../../../wf-api/general/using-api-explorer.md).

>[!NOTE]
>
>Non è possibile creare rapporti nell’interfaccia di Workfront su oggetti non disponibili nel generatore di rapporti. Tuttavia, puoi creare rapporti sui campi associati agli oggetti nel Report Builder se tali campi sono disponibili tramite l’API. A tale scopo, è necessario utilizzare l&#39;interfaccia Modalità testo.

La modalità testo consente di creare visualizzazioni, filtri, raggruppamenti e prompt più complessi, consentendo di utilizzare campi non disponibili nell&#39;interfaccia della modalità standard.

#### Terminologia della modalità testo {#text-mode-terminology}

È necessario utilizzare una sintassi specifica per utilizzare l&#39;interfaccia della modalità testo di Workfront.

Per ulteriori dettagli sulla sintassi di Workfront per la modalità testo, vedere [Panoramica sulla sintassi della modalità testo](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md).

#### Colonne calcolate, formattazione condizionale e altri utilizzi della modalità testo {#calculated-columns-conditional-formatting-and-other-uses-of-text-mode}

Al di fuori dei rapporti sui campi non disponibili nell’interfaccia del generatore, puoi utilizzare la modalità Testo per visualizzare calcoli o confronti tra determinati campi.

Per un elenco degli usi più comuni della modalità testo in un report, vedere [Panoramica degli usi comuni della modalità testo](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).

Per informazioni sull&#39;inclusione dei dati personalizzati calcolati nei report, vedere [Dati personalizzati calcolati nei report](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-data-reports.md).

Per informazioni sul confronto dei campi nella formattazione condizionale, vedere [Confrontare i campi nella formattazione condizionale](../../../reports-and-dashboards/reports/text-mode/compare-fields-conditional-formatting.md).

È inoltre possibile fare riferimento ai campi della raccolta utilizzando la modalità Testo nei rapporti.\
Per informazioni sull&#39;utilizzo della modalità testo per visualizzare le informazioni sulla raccolta in un report, vedere [Riferimento alle raccolte in un report](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

#### Esempi di modalità testo {#text-mode-samples}

È disponibile una libreria di esempi delle visualizzazioni, dei filtri e dei raggruppamenti più utilizzati che è possibile creare con la modalità testo.

Per sfogliare questa libreria e utilizzare alcuni esempi offerti, vedere l&#39;articolo [Visualizzazione personalizzata, filtro e raggruppamento di esempi: indice articolo](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md).

## Schede di un rapporto

Un rapporto può contenere diverse schede quando lo si esegue nell’interfaccia.

Per informazioni sull&#39;esecuzione di un report, vedere l&#39;articolo [Eseguire un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-report.md).

In ogni scheda, le informazioni incluse nel rapporto vengono visualizzate in formati leggermente diversi. Scegli il formato che meglio si adatta alle esigenze della tua organizzazione.

Puoi impostare qualsiasi scheda come predefinita del rapporto. La scheda predefinita è la prima scheda visualizzata quando si fa clic sul nome di un report per aprirlo ed è la scheda visualizzata quando si posiziona il report su un dashboard.

### Scheda Dettagli {#details-tab}

Nella scheda Dettagli di un report vengono visualizzati l&#39;oggetto dei report e gli attributi scelti per tale oggetto in una maschera elenco. Ogni rapporto ha una scheda Dettagli.

>[!IMPORTANT]
>
>Le informazioni nella scheda Dettagli possono essere visualizzate in modo diverso rispetto alla scheda Grafico in base al fuso orario.\
>Ad esempio, un utente in California ha completato un’attività alle 21:30 PST del 12 febbraio. Quando un utente di New York visualizza un rapporto che include il completamento di questa attività, la data di completamento effettiva viene visualizzata come 13 febbraio sia nella scheda Dettagli che nei dettagli del grafico, in quanto è stato completato alle 00:30 EST del 13 febbraio. Tuttavia, nel grafico viene incluso nel raggruppamento del 12 febbraio fino a quando non si espande l’elemento del grafico.

### Scheda Riepilogo {#summary-tab}

I rapporti che includono un raggruppamento dispongono di una scheda Riepilogo.

Le stesse informazioni visualizzate in formato elenco nella scheda Dettagli vengono riepilogate e aggregate in base ai raggruppamenti nel rapporto della scheda Riepilogo.

Per informazioni sui raggruppamenti, vedere [Panoramica sui raggruppamenti in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

### Scheda Matrice {#matrix-tab}

I report che includono un raggruppamento di matrici dispongono di una scheda Matrice.

Le stesse informazioni visualizzate in formato elenco nella scheda Dettagli vengono visualizzate in formato tabella, raggruppate in base ai raggruppamenti nel report della scheda Matrice.

Quando si aggiunge un raggruppamento di matrici a un report, la scheda Riepilogo viene sostituita dalla scheda Matrice.

Per informazioni sulla creazione di un raggruppamento di matrici, vedere l&#39;articolo [Creare un report di matrici](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

### Scheda Grafico {#chart-tab}

I report che includono un grafico dispongono di una scheda Grafico.

Prendi in considerazione l’inclusione di un grafico nei rapporti per dashboard di grande impatto per i dirigenti. I grafici sono un modo conciso per visualizzare le informazioni in un rapporto. È possibile espandere un elemento del grafico facendo clic su di esso per visualizzarne gli elementi.

>[!IMPORTANT]
>
>Quando si fa clic su un elemento del grafico, le informazioni espanse potrebbero essere visualizzate in modo diverso rispetto al grafico in base al fuso orario.\
>Ad esempio, un utente in California ha completato un’attività alle 21:30 PST del 12 febbraio. Quando un utente di New York visualizza un rapporto che include il completamento di questa attività, la data di completamento effettiva viene visualizzata come 13 febbraio sia nella scheda Dettagli che nei dettagli del grafico, in quanto è stato completato alle 00:30 EST del 13 febbraio. Tuttavia, nel grafico viene incluso nel raggruppamento del 12 febbraio fino a quando non si espande l’elemento del grafico.

Per informazioni sulla creazione di un report con un grafico, vedere l&#39;articolo [Aggiungere un grafico a un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

### Scheda Prompts {#prompts-tab}

I rapporti che includono una richiesta dispongono di una scheda Prompts.

Una richiesta consente di aggiungere un filtro a un report ogni volta che si esegue il report. Quando si aggiunge un prompt al report, la scheda Prompts diventa automaticamente la scheda predefinita del report. Questa scheda non può essere modificata in un&#39;altra.

Per informazioni sulla creazione di un prompt per un report, vedere l&#39;articolo [Aggiungere un prompt a un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

## Condividere i rapporti

Dopo aver creato un rapporto, puoi condividerlo con altri utenti.

### Concedere autorizzazioni di condivisione a un report {#give-sharing-permissions-to-a-report}

È possibile assegnare autorizzazioni di condivisione a un altro utente per visualizzare o gestire un report creato. Puoi assegnare a un altro utente un livello di autorizzazioni uguale o inferiore al tuo. È inoltre possibile rendere pubblico un report utilizzando le autorizzazioni di condivisione. Per informazioni sulla condivisione di un report, vedere [Condividere un report in Adobe Workfront](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

### Pianificare la consegna di un rapporto {#schedule-a-report-delivery}

Puoi pianificare un rapporto per la consegna. Gli utenti con cui stai condividendo il report ricevono un’e-mail con un allegato dei risultati del report. L&#39;allegato può essere nei seguenti formati:

* HTML
* PDF
* Excel
* .TSV

Per informazioni sulla pianificazione della consegna di un report, vedi [Panoramica della consegna del report](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

### Esportare i risultati di un rapporto {#export-the-results-of-a-report}

Puoi esportare i risultati di un rapporto nei seguenti formati di file:

* PDF
* Excel (formati .xls e .xlsx)
* Delimitato in tabella

Per informazioni sull&#39;esportazione dei risultati di un report, vedere [Esporta dati](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

Dopo aver esportato il report in uno di questi formati, è possibile condividerlo con altri utenti inviandolo tramite e-mail come allegato o stampandolo.

### Aggiungere un rapporto a una dashboard {#add-a-report-to-a-dashboard}

Puoi aggiungere un rapporto a una dashboard e condividerla con altri utenti. Per informazioni sull&#39;aggiunta di report a un dashboard, vedere [Aggiungere un report a un dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/add-report-dashboard.md).

## Creare calendari

Se si desidera visualizzare i dati in un formato calendario, è possibile creare calendari anziché report.

Per informazioni sulla creazione e l&#39;utilizzo dei calendari, vedere [Panoramica sui report calendario](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

## Utilizzo report

Dopo aver creato i rapporti e averli condivisi con altri utenti, puoi tenere traccia della frequenza con cui utilizzano tali rapporti.
Per informazioni sull&#39;utilizzo del report, tra cui la frequenza con cui vengono visualizzati, l&#39;utente e le dashboard in cui vengono visualizzati, vedere l&#39;articolo [Panoramica sull&#39;utilizzo del report](../../../reports-and-dashboards/reports/report-usage/report-usage-overview.md).

## Termini comuni utilizzati in riferimento ai rapporti

I seguenti termini vengono utilizzati in riferimento ai rapporti di Workfront:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Termine o frase</strong> </th> 
   <th><strong>Definizione</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Opzioni avanzate</td> 
   <td> <p>Fa riferimento al collegamento nella scheda Colonne (Visualizzazione) del generatore di rapporti che consente di effettuare le seguenti operazioni:</p> 
    <ul> 
     <li>Imposta la formattazione condizionale delle colonne per il testo e le immagini in base ai criteri selezionati.</li> 
     <li>Rietichettare la colonna.</li> 
     <li>Formatta i valori nella colonna.</li> 
    </ul> <p>È possibile, ad esempio, che si desideri visualizzare tutte le attività padre in grassetto o che si desideri visualizzare la Data di completamento pianificata in rosso se l'attività è in ritardo.</p> </td> 
  </tr> 
  <tr> 
   <td>Attributo</td> 
   <td> Campo di un oggetto definito nel database. Viene utilizzato in un'espressione in modalità testo. <br>Ad esempio, il campo Stato viene visualizzato come <em>stato</em> quando viene utilizzato in un'espressione in modalità testo. </td> 
  </tr> 
  <tr> 
   <td>Bean o JavaBean</td> 
   <td>Un Bean rappresenta un elemento di programmazione riutilizzabile. Il termine Bean identifica le relazioni tra oggetti diversi nell'applicazione Workfront. È importante avere familiarità con queste relazioni quando si tenta di visualizzare attributi aggiuntivi su un oggetto che non sono disponibili negli strumenti di reporting di base.</td> 
  </tr> 
  <tr> 
   <td>Interfaccia o Report Builder di generazione</td> 
   <td>L'interfaccia Builder è la serie di menu a discesa contenenti i campi visualizzati nelle schede Colonne (Visualizza), Filtro e Raggruppamento. Fornisce un mapping intuitivo delle relazioni Bean per identificare le colonne di una visualizzazione, i criteri di un filtro e gli attributi comuni di un raggruppamento.</td> 
  </tr> 
  <tr> 
   <td>Camel Case</td> 
   <td> <p>Camel Case si riferisce a un modo specifico per scrivere elementi di programmazione per stringere attributi con più parole insieme. Quando si scrive un attributo in Camel Case, la prima lettera della prima parola è minuscola, non c'è spazio tra le parole e la prima lettera di qualsiasi parola successiva è maiuscola.</p> <p>Ad esempio, il Gruppo predefinito viene scritto come <em>gruppoHome</em>, il Pool di Risorse come <em>gruppoRisorse</em> e la Data di Inizio Reale come <em>dataInizioReale</em>.</p> </td> 
  </tr> 
  <tr> 
   <td>Diagramma</td> 
   <td> <p>Una scheda all’interno del generatore di report, una scheda report, dopo aver salvato il report, nonché un elemento facoltativo di un report che consente di aggiungere un grafico a qualsiasi report. È necessario definire un Raggruppamento nel report prima di poter creare un grafico.</p> <p>Di seguito sono riportati i tipi di grafici che è possibile aggiungere a qualsiasi rapporto:<br></p> 
    <ul> 
     <li>Colonna</li> 
     <li>Barra</li> 
     <li>Torta</li> 
     <li>Linee</li> 
     <li>Indicatori</li> 
     <li>Bolla</li> 
    </ul> <p>Per ulteriori informazioni sull'aggiunta di grafici ai report, vedere l'articolo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md" class="MCXref xref">Aggiungere un grafico a un report</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Dettagli</td> 
   <td>Questa è una delle schede di un rapporto, dopo aver salvato il rapporto. Visualizza i risultati del report, visualizzati nella visualizzazione e nel raggruppamento desiderati.</td> 
  </tr> 
  <tr> 
   <td>Espressione</td> 
   <td>Un'espressione è una formula scritta in modalità testo per trasmettere le informazioni da cercare o visualizzare quando si utilizza l'interfaccia in modalità testo. In genere si tratta di una riga in un'istruzione Text Mode più grande.</td> 
  </tr> 
  <tr> 
   <td>Campi</td> 
   <td> <p>Si riferisce agli attributi degli oggetti. Ad esempio, "Stato" è un campo per Progetti, Attività o Problemi. "Gestione Portfoli" è un campo per l'oggetto Portfolio.</p> <p>È inoltre possibile creare e aggiungere campi personalizzati ai moduli personalizzati.<br>Per informazioni sulla creazione di moduli personalizzati, vedere l'articolo <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Progettare un modulo con il progettista del modulo</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Nome Campo </td> 
   <td>Valore di un attributo visualizzato in una visualizzazione o utilizzato nella condizione di un filtro o come elemento comune di un raggruppamento. Le opzioni per Nome campo dipendono dalla selezione di Source campo.</td> 
  </tr> 
  <tr> 
   <td>Sorgente Campo </td> 
   <td>Valore di un oggetto visualizzato in una vista o utilizzato nella condizione di un filtro o come elemento comune di un raggruppamento. Le opzioni nel Field Source dipendono dal tipo di oggetto dell’elemento dell’interfaccia utente che viene creato. Il Field Source consente di fare riferimento ad attributi da oggetti diversi dal tipo di oggetto dell'elemento UI.</td> 
  </tr> 
  <tr> 
   <td>Filtro</td> 
   <td>Elemento principale del rapporto che determina quali risultati visualizzare nel rapporto.</td> 
  </tr> 
  <tr> 
   <td>Modulo </td> 
   <td>Utilizzato in modo intercambiabile con "Modulo personalizzato". I campi e le sezioni vengono aggiunti ai moduli, che vengono quindi allegati a un oggetto per estendere il numero di campi che è possibile associare a un oggetto.</td> 
  </tr> 
  <tr> 
   <td>Raggruppamento </td> 
   <td>Elemento report principale che identifica la modalità di organizzazione di un elenco di risultati. Il raggruppamento crea barre orizzontali in tutto il rapporto per raggruppare i risultati in base agli attributi comuni definiti durante la creazione. I raggruppamenti vengono utilizzati nei report matrice per aggregare i dati, nonché nei grafici per determinare gli assi dei grafici.</td> 
  </tr> 
  <tr> 
   <td>Oggetto o tipo di oggetto</td> 
   <td> Un oggetto è un elemento applicativo di Workfront, ad esempio Progetto, Attività, Gruppo, Società, Filtro. Il Tipo di oggetto viene utilizzato quando si crea un nuovo report, vista, filtro o raggruppamento per identificare quale oggetto è attivo nel report. I report possono avere un solo tipo di oggetto, che è l'oggetto principale del report.<br>È possibile fare riferimento a oggetti padre nello stesso report.<br>Per ulteriori informazioni sulla gerarchia degli oggetti, vedere la sezione "Informazioni sull'interdipendenza e sulla gerarchia degli oggetti" nell'articolo <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Panoramica sugli oggetti di Adobe Workfront</a>.</td> 
  </tr> 
  <tr> 
   <td>Prompt</td> 
   <td> <p>Elemento report facoltativo che può essere aggiunto a un report quando è necessario utilizzare un filtro diverso ogni volta che si esegue il report.</p> <p>Per informazioni sui prompt, vedere <a href="/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md" class="MCXref xref">Aggiungere un prompt a un report</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Qualificatore o modificatori condizione</td> 
   <td> <p>Questo campo viene visualizzato nelle seguenti aree di un rapporto:</p> 
    <ul> 
     <li>Nella scheda Filtro</li> 
     <li>La schermata Opzioni avanzate per la colonna nella scheda Colonne (Visualizzazione). Definendo un qualificatore, è possibile confrontare il Nome campo con un altro campo o valore.</li> 
     <li> In un prompt personalizzato<br><p>Per informazioni sui prompt, vedere <a href="/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md" class="MCXref xref">Aggiungere un prompt a un report</a>.</p>.</li> 
    </ul> <p>Ad esempio, quando si crea un filtro per le attività con una Data di completamento pianificata di oggi, si seleziona <strong>Uguale</strong> nel campo Qualificatore e la data odierna nel campo Data:</p> <p><em>Attività&gt; Data di completamento pianificata&gt;Uguale&gt;(data odierna)</em> </p> <p>In questo scenario il qualificatore è <strong>Equal</strong>.<br>Per ulteriori informazioni sui qualificatori, vedere l'articolo <a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">Filtri e modificatori di condizioni</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Rapporto </td> 
   <td>La combinazione di una vista, un filtro e (a volte) un raggruppamento. Lo scopo di un report è quello di visualizzare i dati in modo coerente nell’interfaccia, distribuire le informazioni ed eliminare la necessità di eseguire regolarmente la stessa ricerca o query.</td> 
  </tr> 
  <tr> 
   <td>Dichiarazione</td> 
   <td>Consiste di diverse espressioni che vengono messe insieme per definire quali informazioni visualizzare in un rapporto quando si utilizza la modalità Testo. È possibile creare un'istruzione per una visualizzazione, un filtro, un raggruppamento o per un prompt personalizzato in un report.</td> 
  </tr> 
  <tr> 
   <td>Riepilogo</td> 
   <td>Questa è una delle schede di un rapporto, dopo aver salvato il rapporto. Questa scheda viene creata solo quando si definisce un raggruppamento per il report. Vengono riepilogate le informazioni in base al raggruppamento definito durante la creazione del report e viene fornita una rapida panoramica degli oggetti aggregati del report. Non visualizza tutti gli oggetti del report, ma solo quelli aggregati.</td> 
  </tr> 
  <tr> 
   <td>Interfaccia modalità testo</td> 
   <td>Consente di creare o modificare il codice di viste, filtri, raggruppamenti e prompt personalizzati originariamente creati tramite l'interfaccia Builder. Si consiglia di creare gli elementi del rapporto inizialmente tramite l’interfaccia Builder, quindi di convertirli nella modalità testo dopo averli salvati, per semplificare la codifica di viste, filtri, raggruppamenti o prompt avanzati.</td> 
  </tr> 
  <tr> 
   <td>Interfaccia utente</td> 
   <td>Si riferisce ai componenti o ai blocchi predefiniti di ciò che viene visualizzato sullo schermo di un utente in un dato momento.</td> 
  </tr> 
  <tr> 
   <td>Visualizza (o Colonne)</td> 
   <td>Uno degli elementi principali di un rapporto. Identifica le intestazioni di colonna che verranno visualizzate nell’elenco di un rapporto.</td> 
  </tr> 
 </tbody> 
</table>
