---
title: Crea tipi di record
description: I tipi di record sono i tipi di oggetto di Adobe Workfront Planning. In Workfront Planning è possibile creare tipi di record personalizzati che illustrano gli elementi di lavoro necessari nel ciclo di vita dell'organizzazione.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: ed1c4954-b338-4865-a7a9-5ba0192e7b37
source-git-commit: 9debb7c6d9df0f9f4962f3e66f146e5f605d20f0
workflow-type: tm+mt
source-wordcount: '898'
ht-degree: 2%

---


<!--this is linked to the UI in an empty workspace screen-->

# Crea tipi di record

{{planning-important-intro}}

I tipi di record sono i tipi di oggetto di Adobe Workfront Planning. In Workfront Planning è possibile creare tipi di record personalizzati che illustrano gli elementi relativi al lavoro necessari per il ciclo di vita dell&#39;organizzazione.

Per ulteriori informazioni sui tipi di record, vedere [Panoramica sui tipi di record](/help/quicksilver/planning/architecture/overview-of-record-types.md).

## Requisiti di accesso

+++ Espandere per visualizzare i requisiti di accesso per Workfront Planning.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Prodotti</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Piano Adobe Workfront*</p></td> 
   <td> 
<p>Uno dei seguenti piani di Workfront:</p> 
<ul><li>Seleziona</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning non è disponibile per i piani Workfront legacy</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Piano di pianificazione Adobe Workfront*</p></td> 
   <td> 
<p>Qualsiasi </p> 
<p>Per ulteriori informazioni su quanto incluso in ogni piano di Workfront Planning, contattare l'account manager Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Piattaforma Adobe Workfront</p></td> 
   <td> 
<p>Per poter accedere a tutte le funzionalità di Workfront Planning, l’istanza di Workfront della tua organizzazione deve essere integrata in Adobe Unified Experience.</p> 
<p>Per ulteriori informazioni, vedere <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Esperienza unificata di Adobe per Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licenza Adobe Workfront*</p></td> 
   <td><p> Standard</p>
   <p>Workfront Planning non è disponibile per le licenze Workfront legacy</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configurazione del livello di accesso</p></td> 
   <td> <p>Nessun controllo del livello di accesso per Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Autorizzazioni oggetto</p></td> 
   <td>   <p>Gestione delle autorizzazioni per un'area di lavoro</a> </p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p>  </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modello di layout</p></td> 
   <td> <p>A tutti gli utenti, inclusi gli amministratori di Workfront, deve essere assegnato un modello di layout che includa l'area Planning nel menu principale. </p> </td> 
  </tr> 
</tbody> 
</table>

*Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


<!--
OLD: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td> Adobe Workfront
   </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>Current: Plan</p>
   Or
   <p>New: Standard </p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> <p>There are no access level controls for Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
 </tbody>
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 
-->

## Considerazioni sulla creazione di tipi di record

* È possibile creare tipi di record in un&#39;area di lavoro nei modi seguenti:

   * Automaticamente:
      * Quando crei un’area di lavoro utilizzando un modello.

        Per informazioni, vedere [Creare aree di lavoro](/help/quicksilver/planning/architecture/create-workspaces.md).

     <!--* When you import them using an Excel or CSV file. 

            >[!IMPORTANT]
            >
            >This functionality has been temporarily removed since March 21, 2024. It will be enabled at a later date.-->

     <!--this should not ne known anymore: * When you add objects from another application to a linked record field of a record. This creates a read-only record type in Workfront Planning which is connected to object types from the original application. 
        For information about connecting record types with object types from another application, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md).
        For information about connecting objects with records, see [Connect records](/help/quicksilver/planning/records/connect-records.md). -->
   * Manualmente:

      * Da zero.

        Questo articolo descrive come creare tipi di record da zero.

* È possibile spostare tipi di record all&#39;interno di una sezione e da una sezione di un&#39;area di lavoro a un&#39;altra. Non è possibile spostare tipi di record da un&#39;area di lavoro a un&#39;altra.

## Creare tipi di record utilizzando un modello di area di lavoro

È possibile creare automaticamente i tipi di record quando si crea un&#39;area di lavoro utilizzando un modello di Workfront Planning. Ogni modello contiene tipi di record di esempio.

Quando si crea un&#39;area di lavoro da un modello, i tipi di record vengono raggruppati nelle sezioni seguenti:

* Tipi di record operativi
* Tassonomie

È possibile aggiungere manualmente tipi di record nelle sezioni Tipi di record operativi e Tassonomie.

Per informazioni sulla creazione di aree di lavoro, vedere [Creare aree di lavoro](/help/quicksilver/planning/architecture/create-workspaces.md).

Per informazioni sui tipi di record inclusi in ogni modello, vedere [Elenco dei modelli di area di lavoro](/help/quicksilver/planning/architecture/workspace-templates.md).

## Creare un tipo di record da zero

{{step1-to-planning}}

1. Fare clic sull&#39;area di lavoro in cui si desidera creare un tipo di record.

   Oppure

   Da un workspace, espandere la freccia rivolta verso il basso a destra del nome di un workspace esistente, cercare un workspace e selezionarlo quando viene visualizzato nell&#39;elenco.
1. (Facoltativo) Fai clic su **Aggiungi sezione** per aggiungere una nuova sezione all&#39;area di lavoro.
1. Fare clic su **Aggiungi tipo di record**.

   Viene visualizzata la casella Aggiungi tipo di record.
   <!--1. (Conditional) When creating record types by importing an Excel or CSV file is enabled, click **From scratch**. Otherwise, the **Add record type** box opens. -->

   ![](assets/add-record-type-box-with-appearance-options.png)

1. Aggiorna le seguenti informazioni:

   * Sostituire &quot;Tipo di record senza titolo&quot; con il nome del tipo di record futuro. <!--did they bring back the field label here and did they rename it to "Name"-->
   * **Descrizione**: aggiungere ulteriori informazioni sul tipo di record.
   * Selezionare un colore e una forma per l&#39;icona associata al tipo di record. Effettua le seguenti operazioni:
      * Selezionare un colore per identificare il nuovo tipo di record. Colore dell&#39;icona del tipo di record. Il grigio è selezionato per impostazione predefinita.
      * Seleziona un’icona dall’elenco, oppure inizia a digitare il nome di un’icona per descrivere ciò che rappresenta, quindi selezionala quando viene visualizzata. Icona del tipo di record. Per impostazione predefinita, viene selezionata un&#39;icona di file.

1. Fai clic su **Crea**.

   La scheda del tipo di record viene aggiunta alla sezione e all&#39;area di lavoro selezionate.
Sulla scheda viene visualizzata la descrizione del tipo di record.

   ![](assets/record-type-card-with-description.png)

1. (Facoltativo) Passa il puntatore del mouse sulla scheda del tipo di record, fai clic sull&#39;icona **Altro** ![](assets/more-menu.png) nell&#39;angolo superiore destro, quindi fai clic su **Modifica** per modificare le informazioni sul tipo di record.
1. (Facoltativo) Fare clic sulla scheda tipo di record per aprire la pagina tipo di record.

   ![](assets/operational-record-type-blank.png)

   Per impostazione predefinita, la pagina del tipo di record viene visualizzata nella vista tabella. Le colonne della tabella sono campi associati al nuovo tipo di record. Ogni riga è un record univoco da aggiungere.

   <!--TIP: If you import a record type from an Excel or CSV file, records are also imported.-->

   Per impostazione predefinita, i campi seguenti vengono visualizzati nelle colonne della vista tabella di un tipo di record operativo:

   * Nome
   * Descrizione
   * Data di inizio
   * Data di fine
   * Stato

1. (Facoltativo) Aggiorna il nome del tipo di record nell’intestazione della pagina

   Oppure

   Fai clic sull&#39;icona **Altro** ![](assets/more-menu.png) a destra del nome del tipo di record e fai clic su **Modifica** per rinominarlo o modificare le informazioni su di esso. Per ulteriori informazioni, vedere [Modifica tipi di record](/help/quicksilver/planning/architecture/edit-record-types.md).

1. (Facoltativo) Fare clic su **+ Nuovo record** per aggiungere record del tipo di record selezionato. Per ulteriori informazioni, vedere [Creare record](/help/quicksilver/planning/records/create-records.md).
1. (Facoltativo) Fai clic sull&#39;icona **+** nell&#39;angolo superiore destro della tabella per aggiungere altri campi al tipo di record.

   Per ulteriori informazioni sulla creazione dei campi, vedere [Creare i campi](/help/quicksilver/planning/fields/create-fields.md).

1. (Facoltativo) Fare clic sulla freccia rivolta a sinistra a sinistra del nome del tipo di record nell&#39;intestazione per tornare all&#39;area di lavoro selezionata.

1. (Facoltativo) Dall’area di lavoro, fai clic su una scheda del tipo di record e tieni premuto per trascinarla in un punto desiderato o per spostarla in un’altra sezione.

   Le modifiche vengono salvate automaticamente.

   Per ulteriori informazioni sull&#39;aggiunta di record, l&#39;eliminazione o la modifica di tipi di record o l&#39;aggiornamento della visualizzazione nella pagina del tipo di record, vedere gli articoli seguenti:

   * [Crea record](/help/quicksilver/planning/records/create-records.md)
   * [Elimina tipi di record](/help/quicksilver/planning/architecture/delete-record-types.md)
   * [Modifica tipi di record](/help/quicksilver/planning/architecture/edit-record-types.md)
   * [Gestisci visualizzazioni record](/help/quicksilver/planning/views/manage-record-views.md)

<!--
## Create record types by importing an Excel or CSV file

>[!IMPORTANT]
>
>This functionality has been temporarily removed since March 21, 2024. It will be enabled at a later date.

Consider the following when importing record types using an Excel or CSV file: 

* Each sheet of the Excel file becomes a record type. 
* The columns of each sheet become the fields associated with each record type. 
* Fields are unique for their respective record types. 
* Each row in each sheet becomes a unique record associated with its respective record type. 
* Each sheet of the Excel file should not exceed the following: 
    * 50,000 rows
    * 500 columns
* The Excel file should not be larger than 5MB.
* Empty sheets are not supported. 

To import record types using an Excel file: 

{{step1-to-planning}}

1. Click the workspace where you want to create record types, 

    Or

    From a workspace, expand the downward-pointing arrow to the right of an existing workspace name, search for a workspace, then select it when it displays in the list.
1. Click **Add record type**. 
1. Click **Excel/CSV**.
1. Drag and drop an Excel or CSV file previously saved on your computer, or click **Select a CSV or Excel file** to browse for one. 
1. Click **Review your data**.
    
    The Preview and edit box displays with the following information: 

    * The names of the sheets or of the future record types display in the left panel. Workfront Planning selects an icon and a color for each new record type by default.
    * The first sheet or record type is selected and the names of the fields associated with it display as the column headers. The type of each field is selected by default. 
    * Each row represents a new record. Only the first 10 records display in the Preview and edit box. 

    ![](assets/preview-and-edit-box.png)

1. (Optional) Click the name of each sheet in the left panel to review the information it contains. 

    >[!NOTE]
    >
    >    Sheets that are empty are not supported and are dimmed. 


1. (Optional) Click the **Select sheets to import** drop-down menu and deselect the sheets that you don't want to import. 

    ![](assets/select-sheets-to-import-drop-down-with-unselected.png)

    Sheets you deselected display with a gray background. 

1. Click **Import** when you are ready to import your file. 

    The following information imports in to Workfront Planning:

    * New record types
    * New fields associated with each record type
    * New records associated with each record type

    You can start managing fields and records on the record types pages. 
    
    Everyone with access to Workfront Planning can now view and edit the imported record types and their information.-->

