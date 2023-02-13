---
content-type: overview;reference
navigation-topic: workfront-navigation
title: Comprendere gli oggetti in [!DNL Adobe Workfront]
description: Comprendere gli oggetti in [!DNL Adobe Workfront]
feature: Get Started with Workfront
exl-id: f324f198-5472-4cf2-a46e-7fc24605ca90
source-git-commit: 9c78d8e08e62c86a4e1340644ed76c61ce7f2674
workflow-type: tm+mt
source-wordcount: '2308'
ht-degree: 6%

---

# Comprendere gli oggetti in [!DNL Adobe Workfront]

<!--
<***Linked to several articles, do not remove/ change. 
-->

Le informazioni visualizzate in [!DNL Adobe Workfront] è rappresentato da oggetti memorizzati nel [!DNL Workfront] database. Gli oggetti sono ciò che guida le informazioni in [!DNL Workfront].

Informazioni sulla definizione degli oggetti in [!DNL Workfront] è importante in modo da poter utilizzare l’oggetto corretto per le esigenze dell’organizzazione.

Ad esempio, quando si pianifica una grande quantità di lavoro, è necessario utilizzare il [!UICONTROL Progetto] oggetto per definire tale lavoro. Per suddividere questo lavoro in incrementi pianificati più piccoli, puoi utilizzare il [!UICONTROL Attività] oggetto. Per una minore quantità di lavoro non pianificata e che può verificarsi in modo imprevisto, è possibile utilizzare l&#39;oggetto Issue. Se desideri tenere traccia dell’avanzamento e dell’aderenza al budget e alla timeline di un gruppo di progetti, puoi organizzarli in [!UICONTROL Portfoli] e [!UICONTROL Programmi]. Per definire altri elementi che consentono di risolvere il lavoro, utilizzare altri oggetti memorizzati in [!UICONTROL Progetti], [!UICONTROL Attività], [!UICONTROL Problemi]oppure [!UICONTROL Portfoli], come [!UICONTROL Documenti], [!UICONTROL Note], [!UICONTROL Ore], [!UICONTROL Utenti]oppure [!UICONTROL Ruoli processo].

[!UICONTROL Rapporti] e [!UICONTROL Dashboard] sono un altro esempio di oggetti che può essere utile per organizzare la quantità di dati a disposizione [!DNL Workfront] per renderlo facilmente accessibile a tutti gli utenti.

Per un elenco completo degli oggetti in [!DNL Workfront], vedi [Esplora API](../../../wf-api/general/api-explorer.md).

## Interdipendenza e gerarchia degli oggetti

Gli oggetti sono collegati tra loro in [!UICONTROL Workfront]. Ad esempio, un&#39;attività o un problema non può mai esistere indipendentemente al di fuori di un progetto. [!UICONTROL Attività] e [!UICONTROL questioni] sono esempi di oggetti memorizzati nel [!UICONTROL progetto] oggetto. [!UICONTROL Attività] e [!UICONTROL questioni] sono considerati oggetti secondari per progetti.

Di seguito sono riportati alcuni degli oggetti più comunemente utilizzati in [!DNL Workfront] e i rispettivi oggetti padre e figlio:

| **Oggetto** | **Oggetti principali** | **Oggetti secondari** |
|---|---|---|
| [!UICONTROL Portfolio] |  | [!UICONTROL Programmi], [!UICONTROL Progetti], [!UICONTROL Documenti], [!DNL Notes], [!UICONTROL Utenti] |
| [!UICONTROL Programmi] | [!UICONTROL Portfolio] | [!UICONTROL Progetti], [!UICONTROL Documenti], [!UICONTROL Note], [!UICONTROL Utenti] |
| [!UICONTROL Progetti] | [!UICONTROL Portfoli], [!UICONTROL Programmi] | [!UICONTROL Attività], [!UICONTROL Problemi], [!UICONTROL Documenti], [!UICONTROL Note], [!UICONTROL Ore], [!UICONTROL Utenti] |
| [!UICONTROL Attività] | [!UICONTROL Progetti] | [!UICONTROL Problemi], [!UICONTROL Attività figlio], [!UICONTROL Documenti], [!UICONTROL Note], [!UICONTROL Ore], [!UICONTROL Utenti] |
| [!UICONTROL Problemi] | [!UICONTROL Attività], [!UICONTROL Progetti] | [!UICONTROL Documenti], [!UICONTROL Note], [!UICONTROL Ore], [!UICONTROL Utenti] |
| [!UICONTROL Dashboard] |  | [!UICONTROL Rapporti], Pagine esterne |
| [!UICONTROL Report] | [!UICONTROL Dashboard] |  |
| [!UICONTROL Gruppi] |  | [!UICONTROL Utenti] |
| [!UICONTROL Team] |  | [!UICONTROL Utenti] |
| [!UICONTROL Utenti] | [!UICONTROL Gruppi], [!UICONTROL Team], [!UICONTROL Aziende] | [!UICONTROL Ruoli] |
| [!UICONTROL Aziende] |  | [!UICONTROL Utenti] |
| [!UICONTROL Documenti] | [!UICONTROL Attività], [!UICONTROL Problemi], [!UICONTROL Progetti], [!UICONTROL Portfoli], [!UICONTROL Programmi], [!UICONTROL Utenti] |  |
| [!UICONTROL Piani]* |  | [!UICONTROL Iniziative] |
| [!DNL Goals]* |  | [!UICONTROL Risultati], [!UICONTROL Attività] |

Per un elenco completo degli oggetti in [!DNL Workfront], vedi [Esplora API](../../../wf-api/general/api-explorer.md).

*I piani sono gli oggetti del [!DNL Workfront Scenario Planner]. Per informazioni sulla [!DNL Scenario Planner], vedi [La [!UICONTROL Pianificazione scenario] panoramica](../../../scenario-planner/scenario-planner-overview.md).

*[!UICONTROL Obiettivi] sono gli oggetti [!DNL Workfront Goals]. Per informazioni su [!DNL Workfront Goals], vedi [[!DNL Adobe Workfront Goals] panoramica](../../../workfront-goals/goal-management/wf-goals-overview.md).


## Personalizzare i nomi degli oggetti

Come [!DNL Workfront] amministratore, è possibile personalizzare i nomi degli oggetti in [!DNL Workfront] utilizzando un  [!UICONTROL Modello di layout].

Per ulteriori informazioni su come personalizzare i nomi degli oggetti utilizzando un  [!UICONTROL Modello di layout], vedi [Creare e gestire modelli di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

Dopo aver personalizzato un modello di layout e averlo assegnato agli utenti, questi ultimi visualizzano i nomi personalizzati per gli oggetti. Gli utenti assegnati al modello di layout non visualizzano più i nomi predefiniti per gli oggetti in un punto qualsiasi dell&#39;applicazione Web.

>[!NOTE]
>
>Affinché i nuovi nomi degli oggetti siano visibili agli utenti, questi devono disconnettersi ed effettuare nuovamente l&#39;accesso a [!DNL Workfront] dopo aver salvato il  [!UICONTROL Modello di layout].

>[!IMPORTANT]
>
>La [!DNL Workfront] La documentazione fa sempre riferimento ai nomi predefiniti degli oggetti. Come [!DNL Workfront] assicurarsi di informare gli utenti delle modifiche apportate ai nomi degli oggetti in modo che possano comprendere come utilizzare il [!DNL Workfront] la documentazione, nonché le aree delle applicazioni che non riflettono le modifiche nei nomi degli oggetti.

* [Nomi di oggetti personalizzabili utilizzando un  [!UICONTROL Modello di layout]](#object-names-that-can-be-customized-using-a-layout-template)
* [Zone [!DNL Workfront] che riflettono i nomi degli oggetti personalizzati](#areas-of-workfront-that-reflect-the-customized-object-names)
* [Zone [!DNL Workfront] che non riflettono i nomi degli oggetti personalizzati](#areas-of-workfront-that-do-not-reflect-the-customized-object-names)

### Nomi di oggetti personalizzabili utilizzando un [!UICONTROL Modello di layout]

Come [!DNL Workfront] amministratore, è possibile personalizzare i nomi dei seguenti oggetti in modo che corrispondano alla terminologia della propria organizzazione:

* [!UICONTROL Portfolio]
* [!UICONTROL Programma]
* [!UICONTROL Progetto]
* [!UICONTROL Attività]
* [!UICONTROL Problema]
* [!UICONTROL Obiettivo]*
* [!UICONTROL Risultato]*
* [!UICONTROL Attività]*

   *[!UICONTROL Obiettivi], [!UICONTROL risultati]e [!UICONTROL attività] sono disponibili solo se l’azienda ha acquistato [!DNL Workfront Goals]. Per informazioni su [!DNL Workfront Goals], vedi [[!DNL Adobe Workfront Goals] panoramica](../../../workfront-goals/goal-management/wf-goals-overview.md).

* [!UICONTROL Iniziativa]**
* [!UICONTROL Scenario]**
* [!UICONTROL Piano]**

   **[!UICONTROL Iniziative], [!UICONTROL scenari]e [!UICONTROL piani] sono disponibili solo se l’azienda ha acquistato [!DNL Workfront Scenario Planner]. Per informazioni sulla [!DNL Scenario Planner], vedi [Introduzione al [!DNL Scenario Planner]](../../../scenario-planner/get-started-with-scenario-planning.md).


Ad esempio, se la maggiore quantità di lavoro nell&#39;organizzazione è nota come &quot;Coinvolgimento&quot;, è possibile sostituire il nome &#39;[!UICONTROL Progetto]con &quot;Engagement&quot;. Le [!DNL Workfront] l&#39;interfaccia mostra &quot;Coinvolgimento&quot; invece di &quot;Coinvolgimento&quot;[!UICONTROL Progetto]&#39; ovunque il nome &#39;[!UICONTROL Progetto]&quot; appariva.

Per ulteriori informazioni su come personalizzare i nomi degli oggetti utilizzando  [!UICONTROL Modelli di layout], vedi [Creare e gestire modelli di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

Non è possibile personalizzare i nomi di qualsiasi altro oggetto in Workfront. Per un elenco completo degli oggetti in [!DNL Workfront], vedi [Esplora API](../../../wf-api/general/api-explorer.md).

Quando si personalizza il nome di un oggetto, nella maggior parte delle aree del [!DNL Workfront] applicazione in cui viene visualizzato il nome dell&#39;oggetto.

### Zone [!DNL Workfront] che riflettono i nomi degli oggetti personalizzati

Le aree seguenti mostrano il nome aggiornato degli oggetti:

* Spostamento superiore
* Tutte le sezioni nel pannello di navigazione a sinistra
* Tutti i menu
* Notifiche in-app
* Generatore di report ed elementi di reporting (visualizzazioni, filtri e raggruppamenti)
* [!UICONTROL Salva] pulsanti
* File esportati
* E-mail
* App mobili

### Zone [!DNL Workfront] che non riflettono i nomi degli oggetti personalizzati

Le aree seguenti non mostrano il nome aggiornato degli oggetti:

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Referenced Object Type selection for a Typeahead field in a Custom Form </p> <p>(NOTE: drafting this because I don't think this is true)</p> </li>
  -->

* [!DNL Outlook] Componente aggiuntivo

## Implicazioni della personalizzazione dei nomi degli oggetti

Quando si personalizzano i nomi degli oggetti in [!DNL Workfront]:

* È possibile che si verifichino errori stilistici o grammaticali nei display del sistema. Ad esempio, se rinomini &#39;[!UICONTROL Problema]Da &quot;Richiedi&quot; e vedi in qualsiasi punto del sistema la frase &quot;Una richiesta&quot;, questo funziona come previsto e non dovrebbe essere considerato un bug.
* I nomi personalizzati degli oggetti non sono traducibili. Solo il [!DNL Workfront] i nomi predefiniti possono essere tradotti nelle lingue supportate. Per ulteriori informazioni sulle lingue supportate in [!DNL Workfront], vedi [Lingue supportate in [!DNL Adobe Workfront]](../../../workfront-basics/supported-languages-in-workfront.md). I campi del nome oggetto personalizzato supportano i caratteri stranieri, consentendo di inserire la terminologia in qualsiasi lingua.
* Quando si personalizzano i nomi degli oggetti utilizzando un  [!UICONTROL Modello di layout], ti consigliamo di assegnare il tuo  [!UICONTROL Modelli di layout] intorno alle unità aziendali (team o gruppi).\
   Per evitare confusione, ti consigliamo di utilizzare nomi chiaramente compresi dagli utenti di queste business unit.
* Le notifiche e-mail e i rapporti consegnati contengono sempre i nomi degli oggetti definiti dalla  [!UICONTROL Modello di layout] dell’utente che genera l’e-mail. Gli utenti devono essere preparati a visualizzare i nomi degli oggetti nelle e-mail che non sono correlati al gruppo o al team, se ricevono notifiche e-mail da utenti di altri team e gruppi.\
   Come [!DNL Workfront] consigliare agli utenti di osservare le icone associate a ciascun oggetto. Le icone rimangono coerenti tra i vari nomi oggetto e coerenti con l’oggetto predefinito, come viene visualizzato nel database. Per un elenco di tutti [!DNL Workfront] icone associate agli oggetti, vedi [Icone degli oggetti](#object-icons).

   >[!TIP]
   >
   >Per le attività più comuni nell’organizzazione, è consigliabile creare una documentazione personalizzata che rifletta la terminologia utilizzata.

## Icone degli oggetti

La [!DNL Workfront] La documentazione fa sempre riferimento ai nomi predefiniti degli oggetti. Se i nomi degli oggetti sono stati personalizzati, è possibile fare affidamento sull&#39;icona associata per capire quale oggetto personalizzato corrisponde a quale [!DNL Workfront] oggetto predefinito.

Per ulteriori informazioni sugli oggetti che possono avere nomi personalizzati in [!DNL Workfront], vedi [Nomi di oggetti personalizzabili utilizzando un  [!UICONTROL Modello di layout]](#object-names-that-can-be-customized-using-a-layout-template).

Di seguito è riportato un elenco di oggetti e le relative icone in Workfront.

| **Oggetto** | **Icona** | **Nome oggetto personalizzabile** |
|---|---|---|
| [!UICONTROL Azienda] | ![](assets/company-icon-nwe.png)  , ![](assets/nwe-company-icon-54x54.png) |  |
| [!UICONTROL Dashboard] | ![](assets/dashboard-icon-nwe.png)  , ![](assets/nwe-dashboards-icon.png) |  |
| [!UICONTROL Obiettivo] | ![](assets/nwe-goal-icon.png) | ↓ |
| [!UICONTROL Gruppo] | ![](assets/groups-icon-nwe.png)  , ![](assets/nwe-group-icon.png) |  |
| [!UICONTROL Problema] | ![](assets/issue-icon-nwe.png)  , ![](assets/nwe-issues-icon.png) | ✔ |
| [!UICONTROL Ruolo] | ![job_role_icon.png](assets/job-role-icon-52x50.png), ![job_role_icon__1_.png](assets/job-role-icon--1--53x44.png), ![](assets/job-role-nwe-no-color.png), ![](assets/job-role-icon-nwe-color.png) |  |
| [!UICONTROL Piano] | ![](assets/plan-icon.png), ![](assets/nwe-plan-icon-60x57.png) |  |
| [!UICONTROL Portfolio] | ![](assets/portfolio-icon-nwe.png)  , ![](assets/nwe-portfolios-icon.png) | ✔ |
| [!UICONTROL Programma] | ![](assets/program-icon-nwe.png)  , ![](assets/nwe-programs-icon.png) | ✔ |
| [!UICONTROL Progetto] | ![](assets/project-icon-nwe.png)  , ![](assets/nwe-projects-icon.png) | ✔ |
| [!UICONTROL Rapporto] | ![](assets/report-icon-nwe.png) , ![](assets/nwe-reports-icon.png) |  |
| [!UICONTROL Attività] | ![](assets/task-icon-new.png)  , ![](assets/nwe-tasks-icon.png) | ✔ |
| [!UICONTROL Team] | ![](assets/team-icon-nwe.png), ![](assets/team-icon-nwe-color.png) , ![](assets/nwe-teams-icon.png) |  |
| [!UICONTROL Modello] | ![](assets/template-icon-nwe.png)  , ![](assets/nwe-templates-icon.png) |  |

## Numeri di riferimento degli oggetti

Ogni oggetto creato in [!DNL Workfront] viene assegnato un numero di riferimento univoco. I numeri di riferimento sono utili per distinguere tra due oggetti altrimenti simili (ad esempio, attività con lo stesso nome). È possibile cercare gli oggetti utilizzando i relativi numeri di riferimento e includere i numeri di riferimento nei rapporti.

Per informazioni sulla ricerca di oggetti per numero di riferimento, vedere [Utilizzare il numero di riferimento degli oggetti](../../../workfront-basics/navigate-workfront/search/reference-number-of-objects.md).

## Ricerche specifiche per oggetti

È possibile eseguire ricerche in tutti gli oggetti ricercabili in [!DNL Workfront]oppure è possibile selezionare un oggetto specifico da cercare nelle ricerche di base e avanzate.

Non tutti gli oggetti sono ricercabili in [!DNL Workfront]. È possibile eseguire ricerche di base e avanzate per i seguenti oggetti in [!DNL Workfront]:

| **Oggetto** | **Ricerca Base** | **Ricerca avanzata** |
|---|---|---|
| [!UICONTROL Progetti] | ✓ | ✓ |
| [!UICONTROL Attività] | ✓ | ✓ |
| [!UICONTROL Problemi] | ✓ | ✓ |
| [!UICONTROL Report] | ✓ | ✓ |
| [!UICONTROL Utenti] | ✓ | ✓ |
| [!UICONTROL Modelli] | ✓ | ✓ |
| [!UICONTROL Documenti] | ✓ | ✓ |
| [!UICONTROL Portfolio] | ✓ | ✓ |
| [!UICONTROL Programmi] | ✓ | ✓ |
| [!UICONTROL Dashboard] | ✓ | ✓ |
| [!UICONTROL Aziende] | ✓ | ✓ |
| [!UICONTROL Note] | ✓ |  |

Per ulteriori informazioni sull’esecuzione di ricerche di base e avanzate in [!DNL Workfront], vedi [Ricerca [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/search/search-workfront.md).

## Rapporto sugli oggetti

È estremamente importante comprendere la gerarchia e l’interdipendenza degli oggetti prima di iniziare a creare rapporti in [!DNL Workfront]. I rapporti sono specifici dell’oggetto. È necessario selezionare l&#39;oggetto corretto per il rapporto prima di visualizzare i dati desiderati.

A seconda dell’oggetto selezionato per il rapporto, è possibile accedere solo agli oggetti direttamente collegati all’oggetto del rapporto.

>[!IMPORTANT]
>
>È possibile creare rapporti solo sull&#39;oggetto selezionato e sugli oggetti principali nello stesso rapporto. Non è possibile avere informazioni sugli oggetti secondari in un rapporto sugli oggetti principali. Ad esempio, è possibile visualizzare le informazioni sul progetto in un rapporto di attività, ma non in un rapporto di progetto.

Puoi creare rapporti su tutti gli oggetti del database utilizzando la nostra API aperta. Per un elenco completo di tutti gli oggetti del database, vedere [Esplora API](../../../wf-api/general/api-explorer.md).

>[!NOTE]
>
>Se i nomi degli oggetti sono stati personalizzati utilizzando un modello di layout, sono stati personalizzati anche i nomi dell&#39;oggetto nel generatore di report. Assicurati di sapere quali oggetti sono stati personalizzati e cerca il nome personalizzato nel generatore di report. Per ulteriori informazioni sugli oggetti che possono avere nomi personalizzati in [!DNL Workfront], vedi *[Nomi di oggetti personalizzabili utilizzando un  [!UICONTROL Modello di layout]](#object-names-that-can-be-customized-using-a-layout-template).*
>Quando si utilizza la modalità testo nei rapporti, i nomi degli oggetti nelle espressioni in modalità testo sono quelli standard in [!DNL Workfront]e non i nomi degli oggetti personalizzati. Per ulteriori informazioni sull’utilizzo della modalità testo nei rapporti, consulta [Panoramica della modalità testo](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Per ulteriori informazioni sulla creazione di un rapporto, vedi [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).\
Per ulteriori informazioni sulla nostra API, vedi [Esplora API](../../../wf-api/general/api-explorer.md).

È possibile creare rapporti sui seguenti oggetti quando si utilizza il generatore di report in [!DNL Workfront] applicazione web:

* [!UICONTROL Progetto]
* [!UICONTROL Attività]
* [!UICONTROL Ora]
* [!UICONTROL Problema]
* [!UICONTROL Utente]
* [!UICONTROL Livello di accesso]
* [!UICONTROL Approval]
* [!UICONTROL Processo di approvazione]
* [!UICONTROL Assegnazione]
* [!UICONTROL Elemento di lavoro backlog]\
   Visualizza attività o problemi nel backlog agile. Per ulteriori informazioni sul backlog agile, vedi [Gestire il backlog agile](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

* [!UICONTROL Linea di base]
* [!UICONTROL Attività linea di base]
* [!UICONTROL record fatturazione]
* [!UICONTROL Ore preventivate]

   Questa è la [!UICONTROL Ore previste], come mostrato in negli strumenti di gestione delle risorse obsoleti.

   Il &quot;Bud&quot;. Hours&quot; nel campo [!UICONTROL Ora budget] il rapporto si riferisce alle ore in budget per i ruoli di lavoro nel [!UICONTROL Planner risorse]. Per ulteriori informazioni, consulta [Comprendere [!UICONTROL Costo manodopera a budget] e [!UICONTROL Ore previste] per progetti](../../../manage-work/projects/project-finances/budgeted-labor-cost.md).

* [!UICONTROL Evento calendario]
* [!UICONTROL Categoria] o [!UICONTROL Modulo personalizzato])
* [!UICONTROL Azienda]
* [!UICONTROL Dashboard]
* [!UICONTROL Documento]
* [!UICONTROL Approvazione documento]
* [!UICONTROL Versione documento]\
   Consente di visualizzare varie informazioni sulla versione del documento, sul documento a cui è associata la versione, sull&#39;autore della versione e sull&#39;utente che ha creato la bozza nella versione del documento, se presente (Proof Creator).
* [!UICONTROL Modello e-mail]
* [!UICONTROL Spesa]
* [!UICONTROL Tipo di Spesa]
* [!UICONTROL Pagina Esterna]
* [!UICONTROL Preferito]
* [!UICONTROL Filtro]
* [!UICONTROL Obiettivo]

   Puoi creare un rapporto per obiettivi strategici oppure visualizzare informazioni relative all’obiettivo in un rapporto di progetto quando i progetti sono associati a obiettivi come attività obiettivo. Puoi creare obiettivi strategici e collegarli ai progetti solo se la tua organizzazione ha acquistato un [!DNL Workfront Goals] licenza. Per informazioni su [!DNL Workfront Goals], vedi [[!DNL Workfront Goals] panoramica](https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FWorkfront_Goals%2FGoal_management%2Fwf-goals-overview.htm&amp;_LANG=en). Per informazioni sul collegamento di progetti a obiettivi strategici, consulta [Aggiungere progetti agli obiettivi in Obiettivi di Adobe Workfront](https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FWorkfront_Goals%2FResults_and_activities%2Fconnect-projects-to-goals-overview.htm&amp;_LANG=en).

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: hardcoded links in this paragraph)
  </MadCap:conditionalText>
  -->

   >[!TIP]
   >
   >Non puoi creare rapporti sugli obiettivi di progetto associati a un [!UICONTROL Business case]. Per informazioni sugli obiettivi del progetto e sugli obiettivi strategici, consulta [Glossario di [!DNL Adobe Workfront] terminologia](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

* [!UICONTROL Gruppo]
* [!UICONTROL Raggruppamento]
* [!UICONTROL Tipo di ora]
* [!UICONTROL Iniziativa]

   Puoi creare un rapporto per le iniziative che sono oggetti secondari di un piano solo se la tua azienda ha acquistato un [!DNL Workfront Scenario Planner] licenza. Per informazioni sulle iniziative, vedi [Panoramica delle iniziative in [!DNL Workfront Scenario Planner]](https://one.workfront.com/s/csh?context=2066&amp;pubname=the-new-workfront-experience).

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: this link is hardcoded)
  </MadCap:conditionalText>
  -->

* Mansione iniziativa

   È possibile creare un rapporto per i ruoli di lavoro associati alle iniziative in un piano solo se l’azienda ha acquistato un [!DNL Workfront Scenario Planner] licenza. Per informazioni sulla creazione di iniziative e sull&#39;associazione di queste con i ruoli di lavoro, consulta [Creare e modificare iniziative in [!DNL Workfront Scenario Planner]](https://one.workfront.com/s/csh?context=2061&amp;pubname=the-new-workfront-experience).

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: this link is hardcoded)
  </MadCap:conditionalText>
  -->

* [!UICONTROL Iterazione]
* [!UICONTROL Ruolo]
* [!UICONTROL Voce del diario]

   Puoi creare rapporti sugli aggiornamenti di sistema tracciati nella sezione [!UICONTROL Aggiornamenti] area di oggetti quali attività, progetti, problemi, ecc. Per ulteriori informazioni, consulta [Relazione [!UICONTROL Aggiornamenti] area](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

* [!UICONTROL Modello di layout]
* [!UICONTROL Milestone]
* [!UICONTROL Percorso milestone]
* [!UICONTROL Nota]

   >[!NOTE]
   >
   >È possibile creare rapporti sui commenti aggiunti dai singoli utenti.

* [!UICONTROL Parametro] o [!UICONTROL Campo personalizzato])
* [!UICONTROL Gruppo di parametri] o [!UICONTROL Interruzione di sezione])
* [!UICONTROL Profilo del portale] (vengono visualizzate informazioni obsolete)
* [!UICONTROL Portfolio]
* [!UICONTROL Programma]
* [!UICONTROL Progetto] ([!UICONTROL Dati finanziari])

   >[!NOTE]
   >
   >Le informazioni finanziarie vengono inserite in [!UICONTROL Progetto] ([!UICONTROL Dati finanziari]) genera rapporti solo quando i dati ad essa associati hanno meno di 5 anni. Ad esempio, se un ruolo di lavoro è stato assegnato a un compito nel gennaio 2015 e oggi è settembre 2021, un campo finanziario come il [!UICONTROL Data di allocazione] per il ruolo di lavoro non viene popolato nel [!UICONTROL Progetto (dati finanziari)] rapporto.

* [!UICONTROL Approvazione bozza]\
   Consente di visualizzare varie informazioni sull’approvazione della bozza, tra cui: la prova presentata per l&#39;approvazione, le informazioni [!UICONTROL Approvatore], informazioni sul Richiedente (se il Richiedente è una licenza [!DNL Workfront] utente), informazioni sulla versione, l’ID della bozza e la data di creazione della bozza.\
   [!UICONTROL Approvazione della bozza] I rapporti includono solo le bozze disponibili nelle aree di lavoro degli utenti in cui non sono state ancora prese decisioni.\
   Le approvazioni di prova sono assegnate in [!DNL Workfront] come descritto [Aggiungere utenti a una bozza](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md#add) in [Condividi una bozza in [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

* [!UICONTROL Coda]
* [!UICONTROL Argomento Coda]
* [!UICONTROL Rate] (viene visualizzato il ruolo del processo) [!UICONTROL Tasso di fatturazione] informazioni)
* [!UICONTROL Notifica promemoria]
* [!UICONTROL Rapporto]
* [!UICONTROL Gruppo di risorse]
* [!UICONTROL Rischio]
* [!UICONTROL Tipo Rischio]
* [!UICONTROL Pianificazione]
* [!UICONTROL Scorecard]
* [!UICONTROL Team]
* [!UICONTROL Modello]
* [!UICONTROL Attività modello]
* [!UICONTROL Indisponibilità]

   Puoi creare rapporti sull’orario di inattività di un utente, come indicato dall’utente nel suo profilo.

* [!UICONTROL Scheda orario]
* [!UICONTROL Profilo scheda orario]
* [!UICONTROL Gruppo di argomenti]
* [!UICONTROL Delega utente]

   Puoi creare rapporti sugli utenti delegati per eseguire attività e problemi altrui mentre sono fuori sede. Questo rapporto mostra l’utente che non è in ufficio e l’utente che svolge i propri compiti mentre è fuori.

* [!UICONTROL Visualizza]
* [!UICONTROL Elemento di lavoro] (si tratta di compiti e questioni)
