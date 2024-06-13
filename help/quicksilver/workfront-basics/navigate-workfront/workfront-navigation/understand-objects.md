---
content-type: overview;reference
navigation-topic: workfront-navigation
title: "[!DNL Adobe Workfront] panoramica degli oggetti"
description: "Le informazioni visualizzate in [!DNL Adobe Workfront] è rappresentato da oggetti archiviati in [!DNL Workfront] database. Gli oggetti sono ciò che guida le informazioni in [!DNL Workfront]. Per ulteriori informazioni su questi oggetti, consulta questo articolo."
feature: Get Started with Workfront
author: Alina
exl-id: f324f198-5472-4cf2-a46e-7fc24605ca90
source-git-commit: 25939493f6ffed31ae1bdaf26d417ce4e5e5c004
workflow-type: tm+mt
source-wordcount: '2419'
ht-degree: 1%

---

# [!DNL Adobe Workfront] panoramica degli oggetti

<!--Audited: 12/2023-->

<!--
<***Linked to several articles, do not remove/ change. 
-->

Informazioni visualizzate in [!DNL Adobe Workfront] è rappresentato da oggetti archiviati in [!DNL Workfront] database. Gli oggetti sono ciò che guida le informazioni in [!DNL Workfront].

Definizione degli oggetti in [!DNL Workfront] è importante per poter utilizzare l’oggetto corretto in base alle esigenze dell’organizzazione.

Ad esempio, quando pianifichi una grande quantità di lavoro, devi utilizzare [!UICONTROL Progetto] per definire tale lavoro. Per suddividere questo lavoro in incrementi pianificati più piccoli, puoi utilizzare [!UICONTROL Attività] oggetto. Per una quantità inferiore di lavoro non pianificato e che può verificarsi in modo imprevisto, è possibile utilizzare l&#39;oggetto Issue. Se desideri tenere traccia dell’avanzamento e del rispetto del budget e della tempistica di un gruppo di progetti, puoi organizzarli in [!UICONTROL Portfoli] e [!UICONTROL Programmi]. Per definire altri elementi che consentono di risolvere il lavoro, si desidera utilizzare altri oggetti memorizzati in [!UICONTROL Progetti], [!UICONTROL Attività], [!UICONTROL Problemi], o [!UICONTROL Portfoli], come [!UICONTROL Documenti], [!UICONTROL Aggiornamenti], [!UICONTROL Ore], [!UICONTROL Utenti], o [!UICONTROL Mansioni].

[!UICONTROL Rapporti] e [!UICONTROL Dashboard] sono un altro esempio di oggetti che possono aiutarti a organizzare la quantità di dati che hai in [!DNL Workfront] visivamente, per renderla facilmente accessibile a tutti gli utenti.

Per un elenco completo degli oggetti in [!DNL Workfront], vedere [API Explorer](../../../wf-api/general/api-explorer.md).

## Interdipendenza e gerarchia degli oggetti

Gli oggetti sono collegati tra loro in [!UICONTROL Workfront]. Ad esempio, un’attività o un problema non può mai esistere indipendentemente al di fuori di un progetto. [!UICONTROL Attività] e [!UICONTROL problemi] sono esempi di oggetti archiviati in [!UICONTROL progetto] oggetto. [!UICONTROL Attività] e [!UICONTROL problemi] sono considerati oggetti figlio di progetti.

Di seguito sono riportati alcuni degli oggetti più comunemente utilizzati in [!DNL Workfront] e i rispettivi oggetti padre e figlio:

| **Oggetto** | **Oggetti padre** | **Oggetti secondari** |
|---|---|---|
| [!UICONTROL Portfolio] |  | [!UICONTROL Programmi], [!UICONTROL Progetti], [!UICONTROL Documenti], [!DNL Notes], [!UICONTROL Utenti] |
| [!UICONTROL Programmi] | [!UICONTROL Portfolio] | [!UICONTROL Progetti], [!UICONTROL Documenti], [!UICONTROL Note], [!UICONTROL Utenti] |
| [!UICONTROL Progetti] | [!UICONTROL Portfoli], [!UICONTROL Programmi] | [!UICONTROL Attività], [!UICONTROL Problemi], [!UICONTROL Documenti], [!UICONTROL Note], [!UICONTROL Ore], [!UICONTROL Utenti] |
| [!UICONTROL Attività] | [!UICONTROL Progetti] | [!UICONTROL Problemi], [!UICONTROL Attività figlio], [!UICONTROL Documenti], [!UICONTROL Note], [!UICONTROL Ore], [!UICONTROL Utenti] |
| [!UICONTROL Problemi] | [!UICONTROL Attività], [!UICONTROL Progetti] | [!UICONTROL Documenti], [!UICONTROL Note], [!UICONTROL Ore], [!UICONTROL Utenti] |
| [!UICONTROL Dashboard] |  | [!UICONTROL Rapporti], Pagine esterne |
| [!UICONTROL Rapporti] | [!UICONTROL Dashboard] |  |
| [!UICONTROL Gruppi] |  | [!UICONTROL Utenti] |
| [!UICONTROL Team] |  | [!UICONTROL Utenti] |
| [!UICONTROL Utenti] | [!UICONTROL Gruppi], [!UICONTROL Team], [!UICONTROL Aziende] | [!UICONTROL Mansioni] |
| [!UICONTROL Aziende] |  | [!UICONTROL Utenti] |
| [!UICONTROL Documenti] | [!UICONTROL Attività], [!UICONTROL Problemi], [!UICONTROL Progetti], [!UICONTROL Portfoli], [!UICONTROL Programmi], [!UICONTROL Utenti] |  |
| [!UICONTROL Piani]* |  | [!UICONTROL Iniziative] |
| [!DNL Goals]* |  | [!UICONTROL Risultati], [!UICONTROL Attività] |

Per un elenco completo degli oggetti in [!DNL Workfront], vedere [API Explorer](../../../wf-api/general/api-explorer.md).

*I piani sono gli oggetti [!DNL Adobe Workfront Scenario Planner]. Per informazioni su [!DNL Scenario Planner], vedi [Il [!UICONTROL Pianificazione scenario] panoramica](../../../scenario-planner/scenario-planner-overview.md).

*[!UICONTROL Obiettivi] sono gli oggetti di [!DNL Adobe Workfront Goals]. Per informazioni su [!DNL Workfront Goals], vedi [[!DNL Adobe Workfront Goals] panoramica](../../../workfront-goals/goal-management/wf-goals-overview.md).


## Personalizzare i nomi degli oggetti

As a [!DNL Workfront] amministratore, è possibile personalizzare i nomi degli oggetti in [!DNL Workfront] utilizzando un [!UICONTROL Modello di layout].

Per ulteriori informazioni su come personalizzare i nomi degli oggetti mediante  [!UICONTROL Modello di layout], vedi [Creare e gestire modelli di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

Dopo aver personalizzato un modello di layout e averlo assegnato agli utenti, questi ultimi visualizzano i nomi personalizzati degli oggetti. Gli utenti che sono stati assegnati al modello di layout non visualizzano più i nomi predefiniti per gli oggetti in nessun punto dell&#39;applicazione Web.

Ad esempio, se la maggior parte del lavoro nell’organizzazione è nota come &quot;Coinvolgimento&quot;, puoi sostituire il nome &quot;[!UICONTROL Progetto]&#39; con &#39;Engagement&#39;. Il tuo [!DNL Workfront] L&#39;interfaccia mostra &#39;Engagement&#39; invece di &#39;[!UICONTROL Progetto]&#39; ovunque dove il nome &#39;[!UICONTROL Progetto]apparirebbe.

>[!NOTE]
>
>Affinché i nuovi nomi degli oggetti siano visibili agli utenti, è necessario disconnettersi e accedere nuovamente a [!DNL Workfront] dopo aver salvato  [!UICONTROL Modello di layout].

>[!IMPORTANT]
>
>Il [!DNL Workfront] La documentazione fa sempre riferimento ai nomi predefiniti degli oggetti. As a [!DNL Workfront] amministratore, assicurarsi di notificare agli utenti le modifiche apportate ai nomi degli oggetti, in modo che possano capire come utilizzare [!DNL Workfront] nonché le aree delle applicazioni che non riflettono le modifiche nei nomi degli oggetti.

* [Nomi di oggetti che possono essere personalizzati utilizzando un  [!UICONTROL Modello di layout]](#object-names-that-can-be-customized-using-a-layout-template)
* [Aree di [!DNL Workfront] che riflettono i nomi degli oggetti personalizzati](#areas-of-workfront-that-reflect-the-customized-object-names)
* [Aree di [!DNL Workfront] che non riflettono i nomi degli oggetti personalizzati](#areas-of-workfront-that-do-not-reflect-the-customized-object-names)

### Nomi di oggetti che possono essere personalizzati utilizzando un [!UICONTROL Modello di layout]

As a [!DNL Workfront] amministratore, puoi personalizzare i nomi dei seguenti oggetti in base alla terminologia della tua organizzazione:

* [!UICONTROL Portfolio]
* [!UICONTROL Programma]
* [!UICONTROL Progetto]
* [!UICONTROL Attività]
* [!UICONTROL Problema]
* [!UICONTROL Obiettivo]*
* [!UICONTROL Risultato]*
* [!UICONTROL Attività]*

  *[!UICONTROL Obiettivi], [!UICONTROL risultati], e [!UICONTROL attività] sono disponibili solo se la tua azienda ha acquistato [!DNL Workfront Goals]. Per informazioni su [!DNL Workfront Goals], vedi [[!DNL Adobe Workfront Goals] panoramica](../../../workfront-goals/goal-management/wf-goals-overview.md).

* [!UICONTROL Iniziativa]**
* [!UICONTROL Scenario]**
* [!UICONTROL Piano]**

  **[!UICONTROL Iniziative], [!UICONTROL scenari], e [!UICONTROL piani] sono disponibili solo se la tua azienda ha acquistato [!DNL Workfront Scenario Planner]. Per informazioni su [!DNL Scenario Planner], vedi [Introduzione a [!DNL Scenario Planner]](../../../scenario-planner/get-started-with-scenario-planning.md).



Per ulteriori informazioni su come personalizzare i nomi degli oggetti mediante  [!UICONTROL Modelli di layout], vedi [Creare e gestire modelli di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

Non è possibile personalizzare i nomi di altri oggetti in Workfront. Per un elenco completo degli oggetti in [!DNL Workfront], vedere [API Explorer](../../../wf-api/general/api-explorer.md).

Quando si personalizza il nome di un oggetto, il nuovo nome dell&#39;oggetto viene visualizzato nella maggior parte delle aree del [!DNL Workfront] dell&#39;applicazione in cui verrebbe visualizzato il nome dell&#39;oggetto.

### Aree di [!DNL Workfront] che riflettono i nomi degli oggetti personalizzati

Nelle aree seguenti viene visualizzato il nome aggiornato degli oggetti:

* Spostamento superiore
* Tutte le sezioni nel pannello di navigazione a sinistra
* Tutti i menu
* Notifiche in-app
* Generatore di rapporti ed elementi di reporting (visualizzazioni, filtri e raggruppamenti)
* [!UICONTROL Salva] pulsanti
* File esportati
* E-mail
* App mobili

### Aree di [!DNL Workfront] che non riflettono i nomi degli oggetti personalizzati

Nelle seguenti aree non viene visualizzato il nome aggiornato degli oggetti:

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Referenced Object Type selection for a Typeahead field in a Custom Form </p> <p>(NOTE: drafting this because I don't think this is true)</p> </li>
  -->

* [!DNL Outlook] Componente aggiuntivo

### Implicazioni della personalizzazione dei nomi degli oggetti

Quando si personalizzano i nomi degli oggetti in, è necessario tenere presente quanto segue [!DNL Workfront]:

* È possibile che si verifichino errori stilistici o grammaticali nelle visualizzazioni di sistema. Ad esempio, se si rinomina &#39;[!UICONTROL Problema]&quot; a &quot;Request&quot; (Richiesta) e viene visualizzata in qualsiasi punto del sistema la frase &quot;An request&quot; (Una richiesta), questo funziona come previsto e non deve essere considerato un bug.
* I nomi personalizzati per gli oggetti non sono traducibili. Solo il [!DNL Workfront] i nomi predefiniti possono essere tradotti nelle lingue supportate. Per ulteriori informazioni sulle lingue supportate in [!DNL Workfront], vedi [Lingue supportate in [!DNL Adobe Workfront]](../../../workfront-basics/supported-languages-in-workfront.md). I campi del nome oggetto personalizzato supportano caratteri esterni, in modo da poter immettere la terminologia in qualsiasi lingua.
* Quando si personalizzano i nomi degli oggetti utilizzando una  [!UICONTROL Modello di layout], si consiglia di assegnare  [!UICONTROL Modelli di layout] in base alle unità aziendali (team o gruppi).\
   Per evitare confusione, si consiglia di utilizzare nomi chiaramente compresi dagli utenti di queste unità aziendali.
* Le notifiche e-mail e i report consegnati contengono sempre i nomi degli oggetti definiti dal  [!UICONTROL Modello di layout] dell’utente che genera l’e-mail. Gli utenti devono essere preparati a visualizzare nelle e-mail i nomi degli oggetti che non sono correlati al proprio gruppo o team, se ricevono notifiche e-mail da utenti di altri team e gruppi.\
   As a [!DNL Workfront] consiglia agli utenti di notare le icone associate a ciascun oggetto. Le icone rimangono coerenti tra i vari nomi di oggetto e coerenti con l&#39;oggetto predefinito, come viene visualizzato nel database. Per un elenco di tutti [!DNL Workfront] icone associate agli oggetti, vedi [Icone oggetto](#object-icons).

  >[!TIP]
  >
  >Per le attività comuni nell’organizzazione, puoi creare una documentazione personalizzata che rifletta la terminologia utilizzata.

## Icone oggetto

Il [!DNL Workfront] La documentazione fa sempre riferimento ai nomi predefiniti degli oggetti. Se i nomi degli oggetti sono stati personalizzati, è possibile fare riferimento all&#39;icona associata per capire a quale oggetto personalizzato corrisponde [!DNL Workfront] oggetto predefinito.

Per ulteriori informazioni sugli oggetti che possono avere nomi personalizzati in [!DNL Workfront], vedi [Nomi di oggetti che possono essere personalizzati utilizzando un  [!UICONTROL Modello di layout]](#object-names-that-can-be-customized-using-a-layout-template).

Di seguito è riportato un elenco di oggetti e delle relative icone in Workfront.

| **Oggetto** | **Icona** | **Nome oggetto personalizzabile** |
|---|---|---|
| [!UICONTROL Azienda] | ![](assets/company-icon-nwe.png)  , ![](assets/nwe-company-icon-54x54.png) |  |
| [!UICONTROL Dashboard] | ![](assets/dashboard-icon-nwe.png)  , ![](assets/nwe-dashboards-icon.png) |  |
| [!UICONTROL Obiettivo] | ![](assets/nwe-goal-icon.png) | ✔ |
| [!UICONTROL Gruppo] | ![](assets/groups-icon-nwe.png)  , ![](assets/nwe-group-icon.png) |  |
| [!UICONTROL Problema] | ![](assets/issue-icon-nwe.png)  , ![](assets/nwe-issues-icon.png) | ✔ |
| [!UICONTROL Ruolo] | ![job_role_icon.png](assets/job-role-icon-52x50.png), ![job_role_icon__1_.png](assets/job-role-icon--1--53x44.png), ![](assets/job-role-nwe-no-color.png), ![](assets/job-role-icon-nwe-color.png) |  |
| [!UICONTROL Piano] | ![](assets/plan-icon.png), ![](assets/nwe-plan-icon-60x57.png) |  |
| [!UICONTROL Portfolio] | ![](assets/portfolio-icon-nwe.png)  , ![](assets/nwe-portfolios-icon.png) | ✔ |
| [!UICONTROL Programma] | ![](assets/program-icon-nwe.png)  , ![](assets/nwe-programs-icon.png) | ✔ |
| [!UICONTROL Progetto] | ![](assets/project-icon-nwe.png)  , ![](assets/nwe-projects-icon.png) | ✔ |
| [!UICONTROL Report] | ![](assets/report-icon-nwe.png) , ![](assets/nwe-reports-icon.png) |  |
| [!UICONTROL Attività] | ![](assets/task-icon-new.png)  , ![](assets/nwe-tasks-icon.png) | ✔ |
| [!UICONTROL Team] | ![](assets/team-icon-nwe.png), ![](assets/team-icon-nwe-color.png) , ![](assets/nwe-teams-icon.png) |  |
| [!UICONTROL Modello] | ![](assets/template-icon-nwe.png)  , ![](assets/nwe-templates-icon.png) |  |
| [!UICONTROL Utente] | ![](assets/users-icon-gray.png) , ![](assets/user-icon-blue.png) , ![](assets/user-icon-initials.png) , ![](assets/user-avatar.png) , ![](assets/user-main-menu-area.png) |  |

## Numero di riferimento di oggetti

Ogni oggetto creato in [!DNL Workfront] viene assegnato un numero di riferimento univoco. I numeri di riferimento sono utili per distinguere due oggetti altrimenti simili, ad esempio attività con lo stesso nome. È possibile cercare gli oggetti utilizzando i relativi numeri di riferimento e includere tali numeri nei report.

Per informazioni su come cercare gli oggetti in base al numero di riferimento, vedere [Utilizza il numero di riferimento degli oggetti](../../../workfront-basics/navigate-workfront/search/reference-number-of-objects.md).

## Ricerche specifiche dell&#39;oggetto

Puoi eseguire ricerche in tutti gli oggetti in cui è possibile eseguire ricerche [!DNL Workfront], oppure è possibile selezionare un oggetto specifico da cercare nelle ricerche di base e avanzate.

Non tutti gli oggetti sono ricercabili in [!DNL Workfront]. Puoi eseguire ricerche di base e avanzate per i seguenti oggetti in [!DNL Workfront]:

| **Oggetto** | **Ricerca di base** | **Ricerca avanzata** |
|---|---|---|
| [!UICONTROL Progetti] | ✓ | ✓ |
| [!UICONTROL Attività] | ✓ | ✓ |
| [!UICONTROL Problemi] | ✓ | ✓ |
| [!UICONTROL Rapporti] | ✓ | ✓ |
| [!UICONTROL Utenti] | ✓ | ✓ |
| [!UICONTROL Modelli] | ✓ | ✓ |
| [!UICONTROL Documenti] | ✓ | ✓ |
| [!UICONTROL Portfolio] | ✓ | ✓ |
| [!UICONTROL Programmi] | ✓ | ✓ |
| [!UICONTROL Dashboard] | ✓ | ✓ |
| [!UICONTROL Aziende] | ✓ | ✓ |
| [!UICONTROL Note] (o [!UICONTROL Aggiornamenti]) | ✓ |  |

Per ulteriori informazioni sull&#39;esecuzione di ricerche di base e avanzate in [!DNL Workfront], vedi [Ricerca [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/search/search-workfront.md).


## Accesso limitato agli oggetti

Quando un utente non ha accesso a un oggetto, visualizza &quot;Nessun accesso&quot; in qualsiasi punto del nome dell’oggetto in Workfront.

L&#39;accesso agli oggetti può essere limitato nel livello di accesso o nelle autorizzazioni di un oggetto specifico.

Questo vale per tutti gli oggetti e gli oggetti secondari elencati nel [Interdipendenza e gerarchia degli oggetti](#interdependency-and-hierarchy-of-objects) in questo articolo. Questo non si applica agli oggetti Team e User.

## Report sugli oggetti

Comprendere la gerarchia e l’interdipendenza degli oggetti è estremamente importante prima di iniziare a creare rapporti in [!DNL Workfront]. I report sono specifici per gli oggetti. È necessario selezionare l&#39;oggetto corretto per il report prima di poter visualizzare i dati desiderati.

>[!IMPORTANT]
>
>È possibile creare rapporti solo sull&#39;oggetto selezionato e sugli oggetti padre nello stesso rapporto. Non è possibile avere informazioni sugli oggetti figlio in un report di oggetti padre. È possibile, ad esempio, visualizzare le informazioni sul progetto in un report attività, ma non le informazioni sull&#39;attività in un report progetto.

Puoi creare rapporti su tutti gli oggetti nel database utilizzando la nostra API aperta. Per un elenco completo di tutti gli oggetti del database, vedere [API Explorer](../../../wf-api/general/api-explorer.md).

>[!NOTE]
>
> * Se i nomi degli oggetti sono stati personalizzati utilizzando un modello di layout, anche i nomi degli oggetti nel generatore di report sono stati personalizzati. Assicurati di sapere quali oggetti sono stati personalizzati e cerca il nome personalizzato nel Report Builder. Per ulteriori informazioni sugli oggetti che possono avere nomi personalizzati in [!DNL Workfront], vedi [Nomi di oggetti che possono essere personalizzati utilizzando un  [!UICONTROL Modello di layout]](#object-names-that-can-be-customized-using-a-layout-template) in questo articolo.
> * Quando si utilizza la modalità testo nei report, i nomi degli oggetti nelle espressioni della modalità testo sono i nomi standard in [!DNL Workfront]e non i nomi degli oggetti personalizzati. Per ulteriori informazioni sull’utilizzo della modalità testo nei rapporti, consulta [Panoramica sulla modalità testo](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Per ulteriori informazioni sulla creazione di un rapporto, consulta [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).\
Per ulteriori informazioni sulle API, consulta [API Explorer](../../../wf-api/general/api-explorer.md).

### Oggetti disponibili per i report

È possibile creare rapporti sui seguenti oggetti quando si utilizza il generatore di rapporti in [!DNL Workfront] applicazione web. I punti elenco con rientro forniscono ulteriori informazioni sull&#39;oggetto e non rappresentano oggetti aggiuntivi.

* [!UICONTROL Progetto]
* [!UICONTROL Attività]
* [!UICONTROL Hour]
* [!UICONTROL Problema]
* [!UICONTROL Utente]
* [!UICONTROL Accesso] Livello
* [!UICONTROL Approvazione]
* [!UICONTROL Processo di approvazione]
* [!UICONTROL Assegnazione]
* [!UICONTROL Linea di base]
* [!UICONTROL Attività linea di base]
* [!UICONTROL Fatturazione]
* [!UICONTROL Ore preventivate]
   * Questo è il [!UICONTROL Ore preventivate], come appaiono in nei precedenti strumenti obsoleti di gestione delle risorse.
   * Il &quot;Bocciolo. Ore&quot; nel campo [!UICONTROL Ore preventivate] il rapporto si riferisce alle ore preventivate per le mansioni nel [!UICONTROL Pianificazione risorse]. Per ulteriori informazioni, consulta [Comprendere [!UICONTROL Costo manodopera preventivato] e [!UICONTROL Ore preventivate] per i progetti](../../../manage-work/projects/project-finances/budgeted-labor-cost.md).

* [!UICONTROL Evento calendario]
* [!UICONTROL Azienda]
* [!UICONTROL Modulo personalizzato]
* [!UICONTROL Dashboard]
* [!UICONTROL Documento]
* [!UICONTROL Approvazione documento]
* [!UICONTROL Versione documento]
   * È possibile visualizzare informazioni sulla versione del documento, sul documento a cui è associata la versione, su chi ha creato la versione e sull&#39;utente che ha creato la bozza sulla versione del documento, se presente (Creatore bozza).
* [!UICONTROL Modello e-mail]
* [!UICONTROL Spesa]
* [!UICONTROL Tipo di Spesa]
* [!UICONTROL Pagina esterna]
* [!UICONTROL Preferito]
* [!UICONTROL Filtro]
* [!UICONTROL Obiettivo]
   * Puoi creare un rapporto per gli obiettivi strategici oppure visualizzare informazioni relative all’obiettivo in un rapporto di progetto quando i progetti sono associati a obiettivi come attività obiettivo. Puoi creare obiettivi strategici e collegarli ai progetti solo se la tua organizzazione ha acquistato un [!DNL Workfront Goals] licenza. Per informazioni su [!DNL Workfront Goals], vedi [[!DNL Workfront Goals] panoramica](../../../workfront-goals/goal-management/wf-goals-overview.md). Per informazioni sulla connessione dei progetti agli obiettivi strategici, consulta [Aggiungere progetti agli obiettivi in Obiettivi di Adobe Workfront](../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).
*Non è possibile creare rapporti sugli obiettivi del progetto associati a un [!UICONTROL Business Case]. Per informazioni sugli obiettivi del progetto rispetto agli obiettivi strategici, consulta [Glossario di [!DNL Adobe Workfront] terminologia](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

* [!UICONTROL Gruppo]
* [!UICONTROL Raggruppamento]
* [!UICONTROL Tipo di Ora]
* [!UICONTROL Iniziativa]
   * È possibile creare un report per le iniziative che sono gli oggetti figlio di un piano solo se l&#39;azienda ha acquistato un [!DNL Workfront Scenario Planner] licenza. Per informazioni sulle iniziative, consulta [Panoramica delle iniziative in [!DNL Workfront Scenario Planner]](../../../scenario-planner/initiatives-overview.md).

* Mansione iniziativa
   * È possibile generare un report per le mansioni associate alle iniziative in un piano solo se la società ha acquistato un [!DNL Workfront Scenario Planner] licenza. Per informazioni sulla creazione di iniziative e sulla loro associazione a ruoli, consulta [Creare e modificare le iniziative in [!DNL Workfront Scenario Planner]](../../../scenario-planner/create-and-edit-initiatives.md).

* [!UICONTROL Iterazione]
* [!UICONTROL Ruolo]
* [!UICONTROL Voce diario]
   * È possibile creare rapporti sugli aggiornamenti di sistema tracciati in [!UICONTROL Aggiornamenti] area di oggetti come attività, progetti, problemi, ecc. Per ulteriori informazioni, consulta [Rapporto sulla [!UICONTROL Aggiornamenti] area](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

* [!UICONTROL Modello di layout]
* [!UICONTROL Milestone]
* [!UICONTROL Percorso milestone]
* [!UICONTROL Nota] o [!UICONTROL Aggiornamenti]
   * Puoi creare rapporti sui commenti aggiunti dai singoli utenti.

* [!UICONTROL Parametro] (o [!UICONTROL Campo personalizzato])
* [!UICONTROL Raggruppa parametri] (o [!UICONTROL Interruzione di sezione])
* [!UICONTROL Portfolio]
* [!UICONTROL Programma]
* [!UICONTROL Progetto (dati finanziari)]
   * Le informazioni finanziarie vengono compilate in [!UICONTROL Progetto (dati finanziari)] segnala solo quando i dati ad esso associati hanno meno di 5 anni. Ad esempio, se una mansione è stata assegnata a un’attività a gennaio 2015 e oggi è settembre 2021, un campo finanziario come [!UICONTROL Data di allocazione] per il ruolo non viene popolato in [!UICONTROL Progetto (dati finanziari)] rapporto.

  >[!CAUTION]
  >
  >L&#39;esecuzione di un report Progetto (Dati finanziari) comporta il ricalcolo dei dati finanziari, che può sovrascrivere i dati finanziari precedenti e richiedere molto tempo. Per ulteriori informazioni sulle conseguenze del ricalcolo dei dati finanziari, consulta [Ricalcolare i dati finanziari del progetto](/help/quicksilver/manage-work/projects/project-finances/recalculate-project-finances.md).

* [!UICONTROL Approvazione bozza]
   * Consente di visualizzare varie informazioni sull’approvazione della bozza, tra cui: la bozza inviata per l’approvazione, informazioni sulla [!UICONTROL Approvatore], informazioni sul richiedente (se il richiedente è un [!DNL Workfront] utente), informazioni sulla versione, ID bozza e data di creazione della bozza.\
      [!UICONTROL Approvazione bozza] I rapporti includono solo le bozze disponibili nelle aree Il mio lavoro degli utenti in cui non sono ancora state prese decisioni.\
   * Le approvazioni delle bozze vengono assegnate in [!DNL Workfront] come descritto [Aggiungere utenti a una bozza](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md#add) in [Condividere una bozza in [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

* [!UICONTROL Coda]
* [!UICONTROL Argomento Coda]
* [!UICONTROL Tariffa] (visualizza la mansione) [!UICONTROL Tariffa di fatturazione] informazioni)
* [!UICONTROL Avviso di Promemoria]
* [!UICONTROL Report]
* [!UICONTROL Pool di Risorse]
* [!UICONTROL Rischio]
* [!UICONTROL Tipo di rischio]
* [!UICONTROL Pianificazione]
* [!UICONTROL Scorecard]
* [!UICONTROL Team]
* [!UICONTROL Modello]
* [!UICONTROL Attività modello]
* [!UICONTROL Indisponibilità]
   * Puoi generare rapporti sul tempo libero di un utente come indicato dall’utente nel suo profilo.

* [!UICONTROL Scheda orario]
* [!UICONTROL Timesheet Ricorrente]
* [!UICONTROL Gruppo di argomenti]
* [!UICONTROL Approvazione utente]
* [!UICONTROL Delega utente]

   * Puoi creare rapporti sugli utenti che sono stati delegati a eseguire attività e problemi di altri utenti mentre sono fuori sede. Questo rapporto mostra l’utente che è fuori sede e l’utente che svolge i propri compiti mentre è fuori sede.

* [!UICONTROL Decisioni degli utenti]

   * Puoi generare rapporti sul numero di decisioni prese dagli utenti su bozze e documenti nel mese corrente.

* [!UICONTROL Visualizza]
* [!UICONTROL Elemento di lavoro] (genera un rapporto per attività e problemi)
