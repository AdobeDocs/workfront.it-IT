---
title: Panoramica di Adobe Maestro
description: Adobe Maestro è una nuova offerta di Adobe Workfront. Puoi creare aree di lavoro completamente personalizzabili per definire flussi di lavoro che soddisfino le esigenze di ogni unità organizzativa dell’azienda.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: b1d6e0b3-e6d4-46d1-a6a2-4b8b73f7d3f7
source-git-commit: ec6a12f2ffbacabac6124ec3a7d85a3ba292e621
workflow-type: tm+mt
source-wordcount: '1845'
ht-degree: 1%

---

# Panoramica di Adobe Maestro

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

<!--see the separate article I wrote to have the PMs vet it for this: https://adobe-my.sharepoint.com/personal/alinaw_adobe_com/_layouts/15/doc.aspx?sourcedoc={79f94807-3d73-4015-afc0-5c016fc63cfc}&action=edit-->

<!--all the links are hidden for now, so I can share this with customer zero. Activate the links before making this public. -->

<!-- remove the references to closed beta from the entire article-->

<!--update the video in the IMPORTANT below, when we have something better, especially after Open Beta - remove it-->

>[!IMPORTANT]
>
>Le informazioni contenute in questo articolo si riferiscono a Adobe Maestro che è una nuova offerta di Adobe.
>
>Attualmente, Adobe Maestro fa parte di un programma beta aperto a un numero limitato di clienti.
>
>Contatta il rappresentante del tuo account per ulteriori informazioni su come partecipare al programma beta per Maestro.
>[Guarda un video dimostrativo di Adobe Maestro](https://video.tv.adobe.com/v/3424253/){target=_blank}

## Introduzione a Adobe Maestro

Adobe Maestro è una nuova offerta di Adobe Workfront. L&#39;obiettivo di Maestro è quello di dare visibilità completa ai dettagli operativi di un&#39;organizzazione e di rispondere alle domande aziendali critiche in ogni fase del ciclo di vita della gestione del lavoro.

I team e la leadership hanno bisogno di risposte chiare a domande come:

* Quante campagne sono in esecuzione nell’area EMEA per il quarto trimestre?
* Esistono sovrapposizioni di pubblico tra campagne simultanee?
* Quanto stanno andando bene i programmi di sensibilizzazione in questo momento?
* Come si presentano le risorse per una particolare campagna? Chi di loro deve ancora essere approvato?

Per rispondere a queste domande, la leadership ha bisogno di una soluzione che possa fornire una visione olistica di ogni fase del lavoro, dalla pianificazione all&#39;esecuzione, dalla consegna alla misurazione dei risultati. Attualmente, le organizzazioni dispongono di strumenti che possono coprire alcune parti del processo, ma molte non hanno buone connessioni con tutte le fasi del lavoro, né possono fornire risultati in modo affidabile.

Di seguito sono riportate alcune delle principali funzionalità di Maestro:

* Risolvere il problema della gestione del lavoro in tutte le fasi e per tutte le parti interessate che partecipano al processo di lavoro.
* Personalizzare completamente i flussi di lavoro, dalla scelta dei tipi di oggetto (o di record) utilizzati dall&#39;organizzazione alla configurazione del modo in cui questi oggetti si collegano l&#39;uno all&#39;altro.
* Collegamento a tipi di oggetto da altri sistemi, creando un framework coerente per tutti i processi.

## Accesso necessario per utilizzare Maestro durante il programma beta chiuso

>[!IMPORTANT]
>
>Attualmente, non ci sono livelli di accesso o autorizzazioni associati agli utenti o alle informazioni in Maestro. Tutti gli utenti possono visualizzare, modificare ed eliminare tutte le informazioni che qualsiasi altro utente aggiunge a Maestro.

Per ulteriori informazioni sull’accesso necessario per utilizzare Maestro, consulta [Panoramica dell’accesso Adobe Maestro](../maestro/access/access-overview.md).

<!-- hidden the table after I moved the content to the Access overview article: 

You must have the following access to use Adobe Maestro: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. Contact your account representative to inquire about this new offering. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader">Access level</td>
   <td> <p>Any</p>  
</td>
  </tr>

<tr>
   <td role="rowheader">Layout template</td>
   <td> <p>Your system administrator must add the Maestro area in your layout template. For information, see <a href="../maestro/access/grant-access.md">Grant access to Adobe Maestro</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

************* Activate note when going to GA: 

>[!NOTE]
>
>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). 
-->

## Terminologia Maestro

Anche se Maestro fa parte di Workfront, viene fornito con concetti e terminologia proprietari. Assicurati di conoscere i concetti di Maestro prima di iniziare a configurare Maestro per la tua organizzazione.

La struttura per Maestro è completamente personalizzabile. È possibile creare tutti i tipi di record, i relativi attributi e qualsiasi campo ad essi associato in base alle esigenze specifiche dell&#39;organizzazione.

Di seguito sono riportati i principali oggetti e concetti di Maestro:

* **Workspace**: raccolta di tipi di record e tassonomie che definiscono il ciclo di vita operativo di una determinata organizzazione. Un’area di lavoro è l’area di lavoro di un’unità organizzativa.

  Un’istanza di Workfront può avere un massimo di 1.000 aree di lavoro.

  ![](assets/marketing-workspace-with-record-type-taxonomies-opening-page.png)

  Per ulteriori informazioni, consulta [Creare aree di lavoro](../maestro/architecture-and-fields/create-workspaces.md).

* **Tipo di record**: tipo di oggetto principale Maestro.

  A differenza di Workfront, dove i tipi di oggetto sono predefiniti, in Maestro è possibile creare tipi di oggetto personalizzati.

  In Workfront, ad esempio, sono già stati creati i tipi di oggetto Programma, Portfolio, Progetto, Attività o Problema.

  In Maestro, puoi creare qualsiasi tipo di record che soddisfi i flussi di lavoro della tua organizzazione. Successivamente è possibile definire la relazione tra i tipi di record o le dipendenze tra le maschere.

  Per ulteriori informazioni, consulta [Panoramica dei tipi di record operativi e delle tassonomie](../maestro/architecture-and-fields/overview-of-record-types-and-taxonomies.md).

  Maestro ha i seguenti tipi di record:

   * **Tipo di record operativo**: tipo di record che rappresenta piani strategici, iniziative o lavoro eseguito.

     ![](assets/operational-record-type-blank.png)

     Ad esempio, Campaign, Activity, Program possono essere tipi di record operativi.

     Per ulteriori informazioni, consulta [Crea tipi di record](../maestro/architecture-and-fields/create-record-types.md).

   * **Tassonomia**: tipo di record che acquisisce gli attributi relativi a un tipo di record operativo.

     ![](assets/taxonomy-record-type-blank.png)

     Sebbene la creazione delle tassonomie sia identica alla creazione dei tipi di record operativi, Maestro distingue tra un tipo di record operativo e un tipo di record tassonomia. Lo scopo delle tassonomie è migliorare i tipi di record operativi. <!--this is no longer true, but might be later?!: A taxonomy is a record without dates, like a static list of attributes.-->

     Ad esempio, Pubblico, Area o Indirizzo possono essere tipi di record di tipo tassonomia.

     Per ulteriori informazioni, consulta [Creare tipi di record di tassonomia](../maestro/architecture-and-fields/create-a-taxonomy.md).

* **Registra**: istanza di un tipo di record Maestro. Un record può fare riferimento a un tipo di record operativo o a una tassonomia.

  ![](assets/records-highlighted-in-campaign-record-type-list.png)
  ![](assets/records-highlighted-in-region-taxonomy-type-list.png)

  Dopo aver aggiunto un tipo di record a un&#39;area di lavoro, è possibile iniziare ad aggiungere record di tale tipo nella pagina del tipo di record.

  Ad esempio, &quot;Campagna&quot; può essere un tipo di record operativo e &quot;Campagna estiva per EMEA&quot; è un record del tipo di record Campagna

  Oppure

  &quot;Regione&quot; è un tipo di record di tassonomia, mentre &quot;Americhe-America Latina&quot; o &quot;EMEA - Europa centrale&quot; sono record di tassonomia.

  Per ulteriori informazioni, consulta [Crea record](../maestro/records/create-records.md).

* **Modello area di lavoro**: puoi creare un’area di lavoro utilizzando modelli predefiniti. È possibile utilizzare i tipi di record, le tassonomie e i campi predefiniti inclusi in un modello oppure aggiungere record personalizzati.

  ![](assets/workspaces-page-with-templates-thumbnails.png)

  Maestro viene fornito con un modello di area di lavoro di vendita, marketing e gestione dei prodotti.

  Per ulteriori informazioni, consulta [Creare aree di lavoro](../maestro/architecture-and-fields/create-workspaces.md).

* **Campi**: i campi sono attributi che è possibile aggiungere ai tipi di record operativi o di tassonomia che contengono informazioni sul tipo di record. <!--check the shot below, "Connection" needs to be in lowercase-->

  ![](assets/drop-down-list-of-record-fields.png)

  Considerazioni sui campi Maestro:

   * I campi aggiunti per un tipo di record vengono automaticamente associati a tutti i record di quel tipo e possono essere utilizzati per acquisire dati su tali record.

   * I campi vengono visualizzati come colonne nella visualizzazione Tabella applicata a una pagina del tipo di record. Vengono inoltre visualizzati nella pagina Dettagli del record.

   * I campi sono univoci per un tipo di record e non vengono trasferiti da un tipo di record a un altro.

   * I campi Maestro sono completamente personalizzabili e sono accessibili solo in Maestro. Non puoi accedere ai campi Maestro da Workfront.

  Per ulteriori informazioni, consulta [Crea campi](../maestro/architecture-and-fields/create-fields.md)

  Per impostazione predefinita, un nuovo tipo di record operativo è associato ai seguenti campi predefiniti:

   * Nome
   * Descrizione
   * Data di inizio
   * Data di fine
   * Stato

  Per impostazione predefinita, a un campo Nome è associato un nuovo tipo di record di tassonomia.

  Puoi creare campi personalizzati dei seguenti tipi:

   * Testo a riga singola
   * Paragrafo
   * Selezione multipla
   * Selezione singola
   * Data
   * Numero
   * Percentuale
   * Valuta
   * Casella di controllo
   * Persone
   * Creato da
   * Data di creazione
   * Ultima modifica eseguita da
   * Data ultima modifica

* **Tipi di record collegati**, **Record collegati**, e **Campi record collegati**: puoi creare una connessione tra le seguenti entità:

   * Due tipi di record Maestro
   * Un tipo di record Maestro e un tipo di oggetto progetto, programma, portfolio, società o gruppo Workfront.

  ![](assets/new-connection-tab-with-workfront-option.png)

  Dopo aver stabilito una connessione tra i tipi di record, è possibile collegare tra loro singoli record di tali tipi. La connessione tra i record viene visualizzata come campo record collegato.

* **Campi collegati** (o campi di ricerca): dopo aver stabilito la connessione tra due tipi di record e aver collegato i singoli record, è possibile fare riferimento ai campi dei record collegati nel record da cui si sta effettuando la connessione.

  ![](assets/add-lookup-fields-modal.png)

  Per informazioni sul collegamento di tipi di record, record e sulla creazione di campi collegati, vedere gli articoli seguenti:

   * [Connetti tipi di record](../maestro/architecture-and-fields/connect-record-types.md)
   * [Collega record](../maestro/records/connect-records.md)

<!--not yet:* Fields are reusable across Record Types.  -->

* **Visualizzazioni**: i record vengono visualizzati nella rispettiva pagina del tipo di record in diversi tipi di visualizzazioni.

  ![](assets/view-types-drop-down-from-record-type-list.png)

  Le visualizzazioni contengono impostazioni personalizzate di un tipo di visualizzazione specifico, ad esempio l&#39;elenco di campi (colonne), un elenco di record (righe), il relativo ordine, un filtro e un raggruppamento applicati o applicabili.

  Di seguito sono riportati i tipi di visualizzazione che è possibile applicare alla pagina del tipo di record:

   * **Vista tabella**: visualizza i record e i relativi campi in un formato tabella. Le righe della tabella sono i singoli record e le colonne sono i campi record. Questa è la vista predefinita.

     ![](assets/table-view-example.png)

   * **Vista Timeline**: visualizza i record che contengono almeno due campi Data in una sequenza temporale cronologica.

     ![](assets/grouping-applied-in-timeline-view.png)

  Per ulteriori informazioni, consulta [Gestire le visualizzazioni record](../maestro/views/manage-record-views.md).


## Limitazioni dell’oggetto Maestro

La tabella seguente mostra i limiti per il numero di oggetti che è possibile creare in Maestro. Le limitazioni sono soggette a cambiamento mentre ci spostiamo nelle fasi successive dello sviluppo di Maestro.

| Oggetto Maestro | Limite |
|-------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------:|
| Numero di aree di lavoro per un’istanza Workfront | 1,000 |
| Numero di tipi di record per un&#39;area di lavoro | 1.000 (incluse le tassonomie per il workspace o gli oggetti importati da applicazioni di terze parti) |
| Numero di record per un tipo di record | 10,000 |
| Numero di campi per un tipo di record o una tassonomia | 500 |
| Numero di caratteri per un campo di testo | 1.000 caratteri |
| Dimensione del file che è possibile incollare in una tabella del tipo di record | 1MB |
| Dimensione del file che è possibile importare tramite l’API per una tabella del tipo di record | 1.5MB |
| Frequenza con cui è possibile effettuare richieste API | 200 richieste al minuto |
| Dimensione del file CSV di Excel che puoi importare in una tabella | 5MB |

## Abilita Maestro per gli utenti nella tua istanza Workfront

La tua organizzazione deve iscriversi al programma beta chiuso Adobe Maestro prima di poter accedere a Maestro. Per informazioni sull’iscrizione al programma beta, contatta il rappresentante del tuo account.

Per ulteriori informazioni su come concedere l’accesso a e consentire ad altri di utilizzare Maestro, consulta [Concedere l’accesso a Adobe Maestro](../maestro/access/grant-access.md).

<!--hidden this after moved it to a separate article

After your organization has been enrolled in the Maestro beta program, you can add the Maestro area for other users by using a layout template. 

To share the Maestro area using a layout template: 

1. Log in to Workfront as a system administrator.  

1. Add the Maestro icon to the Main Menu using a Layout Template. For information, see [Customize the Main Menu using a layout template](../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md). 

1. Assign the  layout template to the users that you want to have access to Maestro.For information, see [Assign users to a layout template](../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

    All users who can access Maestro in their Main Menu can start creating workspaces, records types, records, and fields.  
  -->


## Individua Maestro

Assicurati che la tua organizzazione abbia ricevuto l’accesso a Maestro e che l’amministratore di sistema o di gruppo abbia aggiunto l’area Maestro al tuo menu principale.

Per individuare Maestro:

1. Accedi ad Adobe Workfront.

1. Fai clic su **Menu principale** ![](assets/main-menu-workfront.png) nell&#39;angolo superiore destro o fare clic sul pulsante **Menu principale** ![](assets/main-menu-shell.png) nell’angolo in alto a sinistra, se disponibile.

1. Clic **Maestro** ![](assets/maestro-icon.png).

   Si apre l&#39;area Maestro Workspaces.

1. (Facoltativo e consigliato) Continua con alcune delle seguenti azioni, per costruire la tua struttura di lavoro in Maestro:

   1. Crea un’area di lavoro da zero o utilizzando un modello.

   1. Aggiungere tipi di record al nuovo workspace.

   1. Aggiungere tassonomie alle nuove aree di lavoro.

   1. Fare clic sul nome di un tipo di record per aprire la pagina del record. Per impostazione predefinita, la pagina record viene visualizzata nella vista Tabella.

   1. Personalizzare la vista Tabella effettuando una delle seguenti operazioni:

      * Aggiungere altri campi al tipo di record facendo clic sul pulsante **+** nell’angolo in alto a destra. Le colonne nella visualizzazione sono campi associati al tipo di record.
      * Aggiungere record facendo clic sul pulsante **+** nell’angolo in basso a sinistra. Le righe nella visualizzazione sono record univoci del tipo di record selezionato.
      * Clic **Filtri** per filtrare le informazioni visualizzate nella pagina tipo di record.

   1. Fare clic sul nome di un record per visualizzare ulteriori informazioni nella pagina Dettagli del record.

   1. Creare una vista Timeline dalla **Visualizza** nell&#39;angolo superiore destro della pagina del tipo di record.

   1. Personalizza la visualizzazione della timeline aggiornando Filtri, Raggruppamenti o Impostazioni.

## Funzioni attualmente disponibili in Maestro

La tabella seguente illustra le principali funzioni che saranno disponibili in Maestro e la tempistica della loro disponibilità. L&#39;elenco non include tutte le funzionalità.

| Funzionalità | Disponibile ora | Disponibile a breve | Nella ricerca |
|----------------------------------------------------|:-----------------------------:|:--------------------------------:|:----------------:|
| Creare aree di lavoro | ✓ |                                  |                  |
| Creare tipi di record operativi | ✓ |                                  |                  |
| Creare tassonomie | ✓ |                                  |                  |
| Creare singoli record denominati e tassonomie | ✓ |                                  |                  |
| Creare campi personalizzati del record | ✓ |                                  |                  |
| Importare tipi di record e campi utilizzando un file Excel o CSV | ✓ |                                  |                  |
| Collega record | ✓ |                                  |                  |
| Visualizzare i record in una tabella | ✓ |                                  |                  |
| Visualizzare i record in un indicatore cronologico | ✓ |                                  |                  |
| Filtra record | ✓ |                                  |                  |
| Raggruppa i record nella visualizzazione timeline | ✓ |                                  |                  |
| Raggruppa i record nella vista tabella |                               | ✓ |                  |
| Ordinare i record nella vista tabella | ✓ |                                 |                  |
| Ordinare i record nella visualizzazione timeline |                               | ✓ |                  |
| Ordinare i raggruppamenti nella vista tabella |                               | ✓ |                  |
| Ordinare i raggruppamenti nella visualizzazione timeline |                               | ✓ |                  |
| Connettere le aree di lavoro |                               | ✓ |                  |
| Collegare i record Maestro e le tassonomie | ✓ |
| Cerca record nella vista tabella | ✓ |   |
| Collegare i record Maestro a progetti, programmi, portafogli, aziende, gruppi Workfront | ✓ |                                 |                  |
| Pagina Dettagli record | ✓ |                                  |                  |
| Aggiornare il layout della pagina Dettagli record |                               | ✓ |                  |
| Livelli di accesso e autorizzazioni | | ✓ |  |
| Inviare richieste |                               |                                  | ✓ |
| Descrizione creativa |                               |                                  | ✓ |
| Personalizzare il colore e l&#39;icona di un record | ✓ |                                  |                 |
<!--
Add another row for Rich text formatting:


|     Rich Text formatting for Paragraph fields                                 |      ✓                         |                                  |                 |
-->

## Attività di rilascio Maestro

Stiamo rilasciando regolarmente nuove funzioni a Maestro. Per un elenco aggiornato delle funzioni rilasciate, consulta [Attività di rilascio Adobe Maestro](../maestro/release-activity.md).

<!--moved the contents of this whole section to its own article: release-activity.md, in the same folder

This section lists the features and patches that have been released after the launch of the Maestro closed beta program, on May 22, 2023. 

The features are released weekly and are listed in the order of their release, with the most recent first. Customers who are participating in the Maestro closed beta program can access all features in their Preview and Production environments. 

### Week of September 4, 2023

#### Connect Maestro records with Workfront companies and groups

Preview and production: September 5, 2023  

You can now connect a Maestro record with Workfront companies and groups. You must first create a connection between a Maestro record type and the Workfront companies and groups object types. Then, you can connect a single Maestro record of the selected record type to individual Workfront companies and groups.  

Consider the following:  

* You must create a connection between Maestro record types and Workfront companies and groups for each Workspace.  

* You cannot connect taxonomy record types with Workfront object types. 

* You can connect multiple Maestro records to the same Workfront company or group, and multiple companies or groups to the same Maestro record.  

* You cannot edit companies or groups in Maestro. All company or group changes performed in Workfront are visible in Maestro, when reviewing the Maestro linked records.  

#### URL support for single-line text fields 

Preview and production: September 7, 2023 

For better visibility when working with links in the Table view, we have added support for URLs in single-line text fields. Using URLs to other websites or external drives when updating a single-line text field, now identifies them as links and allows you to click them from the table.  

### Week of August 28, 2023

#### Field visibility menu for the Table View toolbar

Preview and production: August 31, 2023

To display the right information on a given set of records, especially if you intend to share the view with others who need to see some but not all fields of a record type, you can now select which fields (or columns) to display and which to hide in the Table view.  

You can hide or show individual fields, from each header of the field columns, or you can manage all fields of the record type from a setting in the table view toolbar.  

### Week of August 21, 2023

#### Connect Maestro records to programs and portfolios 

Preview and production: August 24, 2023

You can now connect a Maestro record with Workfront programs and portfolios. You must first create a connection between a Maestro record type and a program or portfolio which creates a connected field. Then, you can connect any Maestro records from all other record types within the same workspace to specific programs and portfolios which will create a read-only Workfront Program or Workfront Portfolio record type in the same workspace. Consider the following:

* Workfront connector record types are unique for each workspace. 
* You can connect multiple Maestro records to the same Workfront program or portfolio, and multiple programs and portfolios to the same Maestro record. 
* You cannot edit programs and portfolios in Maestro. All program and portfolio changes performed in Workfront are visible in Maestro, when reviewing the linked records. 

#### New sorting functionality for the table view

Preview and production: August 24, 2023

You can now sort records in the table view of a record type page. 
The following capabilities are now available: 

* Sorting at the table-level, where you can sort by multiple fields at the same time. 
* Sorting at the column or field-level, where you can sort by an individual field at a time.

#### Improvements to the timeline view: new look-and-feel for groupings and the Compact/ Standard view switch

Preview and production: August 24, 2023

We have introduced the following improvements to the timeline view: 

* You can now display the timeline view in the following modes:

    * Standard: Displays records in separate lines.
    * Compact: Display the records whose dates don't intersect on the same line. 

* We have changed the look-and-feel of the grouping lines in the timeline view to display above the timeline of the records they contain. Prior to this improvement, the grouping lines displayed across the entire length of the timeline.

### Week of August 14, 2023

#### Reorder columns in the table view

You can now reorder columns in the Maestro table view. Consider the following when reordering columns: 

* The Name field is always the first field in the table view of a record type page 

* You cannot move the Name field to another position 

* The Name field is frozen and is not part of the horizontal scroll. 

#### Horizontal scroll for timeline view

You can now scroll horizontally in the timeline view of a record type. 

### Week of August 7, 2023

#### Import record types from an Excel file 

Preview and production: August 10, 2023

You can now import an Excel file to create record types in a workspace. The sheets of the file become the record types, and the columns of the file become their respective fields.  

#### Improved experience for connecting record types and projects 

Preview and production: August 10, 2023

We have improved the way you connect record types, including connecting to Workfront projects. As part of this improvement, we made the following changes when adding a field for a record type from the table view:  

* Removed the Relationship-type field from the "New field" tab.  

* Add a "New connection" tab where you can directly select the record or object type you want to connect to, eliminating the need for a Relationship-type field. 

### Week of July 10, 2023

#### Update the appearance of a record type

Preview and production: July 13, 2023

You can now select a custom icon for a record type, as well as a custom color for the record type icon.  

#### New Checkbox field type

Preview and production: July 13, 2023 

You can now add a Checkbox field type to Maestro record types. You can use the Checkbox field type to add a single checkbox option to a record. You can use this field to indicate a specific attribute or status for that particular record. For example, you can use it as a flag for tracking completion, approval, or any other binary attribute for each record.  

### Week of June 26, 2023

#### Quick activation of the contextual menu in a table

Preview and production: June 28, 2023
 
We have enabled the ability to activate the contextual menu by right-clicking anywhere in a record row, when viewing the records in the table view or a record type. You can now quickly view, delete, or copy a link to the record's Details page when you access the contextual menu from anywhere in the table view of a record type. Prior to this enhancement, the contextual menu was accessible only from the More menu in the Name column of a record.  

### Week of June 19, 2023

#### Record field names are unique

We have introduced a requirement now that the field names of a Maestro record type should have unique names. Fields that belong to different record types do not have to have unique names.  

### Week of June 5, 2023

#### Connect Maestro records with Workfront projects

Preview and production: June 5, 2023

You can now connect a Maestro record with Workfront projects. You must first create a connector Maestro record type to establish the connection between Maestro records and Workfront projects. Then, you can connect any Maestro records from all other record types to the connector record using the Relationship field. Consider the following:

* You must have a connector record type for Workfront for each Workspace. 
* You can connect multiple Maestro records to the same Workfront project, and multiple projects to the same Maestro record. 
* You cannot edit projects in Maestro. All project changes performed in Workfront are visible in Maestro, when reviewing the linked records. 

### Week of May 29, 2023

#### Two-date requirement for creating a Timeline view

Preview and production: May 31, 2023  

You must have at least two date fields associated with a record type in order to create a Timeline view. 
-->
