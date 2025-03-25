---
title: Creazione di oggetti Workfront mediante Adobe Workfront Planning Record Automations
description: In Adobe Workfront Planning è possibile configurare automazioni che, se attivate, creano oggetti in Workfront o record in Workfront Planning. Gli oggetti e i record creati vengono automaticamente connessi ai record di Planning esistenti. Questo articolo descrive come gestire le automazioni, tra cui come modificarle, disattivarle, eliminarle e attivarle per creare oggetti e record.
hide: true
hidefromtoc: true
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: c669217a-40e2-471f-951d-93157a34f1ee
source-git-commit: 15ddf6b4d82ccc694ec7a6c60d8e2d5b6b3645d6
workflow-type: tm+mt
source-wordcount: '1811'
ht-degree: 2%

---

# Creazione di oggetti mediante le automazioni dei record di Adobe Workfront Planning

<!--add screen shots when UI is finalized AND redo all the steps - some things got changed and moved around-->

<!--you might need to add something about notifications and emails?!-->
<!--add a new section to this article to mention a new way to create objects: help/quicksilver/planning/records/create-records.md-->
<!-- add a new section to this article to mention a new way to create WF objects from Planning: help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md-->

<!-- if they give access to use the automation to people with LESS than Manage permissions to a workspace, split this article in two: the Configure section should be for admins and the "Use a Workfront Planning automation to create an object" should be for all other users-->

<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo i rilasci mensili in Produzione, le stesse funzioni sono disponibili nell’ambiente di Produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedere [Abilitare o disabilitare le versioni rapide per l&#39;organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

È possibile configurare le automazioni in Adobe Workfront Planning che, se attivate, creano oggetti in Workfront o record in Workfront Planning quando attivate da un record Planning. Gli oggetti o i record creati vengono automaticamente collegati ai record da cui si sta attivando l&#39;automazione.

È possibile configurare e attivare l&#39;automazione nella pagina del tipo di record in Workfront Planning. L&#39;oggetto connesso creato viene inserito nel campo connesso del tipo di record da cui viene eseguita l&#39;automazione.

Ad esempio, è possibile creare un&#39;automazione che accetta una campagna di Workfront Planning e crea un progetto in Workfront per tenere traccia dell&#39;avanzamento della campagna. Il progetto sarà collegato alla campagna di pianificazione di Workfront nel campo Progetto connesso della campagna.

Per ulteriori informazioni sui record connessi, vedere [Panoramica sui record connessi](/help/quicksilver/planning/records/connected-records-overview.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso.

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
   <td role="rowheader"><p>Pacchetto Adobe Workfront Planning*</p></td> 
   <td> 
<p>Qualsiasi </p> 
<p>Per ulteriori informazioni su quanto incluso in ogni piano di Workfront Planning, contattare l'account manager Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Piattaforma Adobe Workfront</p></td> 
   <td> 
<p>Per poter accedere a tutte le funzionalità di Workfront Planning, l’istanza di Workfront della tua organizzazione deve essere integrata in Adobe Unified Experience.</p> 
<p>Per ulteriori informazioni, vedere <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Esperienza unificata Adobe per Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licenza Adobe Workfront*</p></td> 
   <td> Standard
   <p>Workfront Planning non è disponibile per le licenze Workfront legacy</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configurazione del livello di accesso</p></td> 
   <td> <p>Nessun controllo del livello di accesso per Adobe Workfront Planning</p> 
   <p>Modifica l'accesso in Workfront per i tipi di oggetto che desideri creare (progetti, portfolio, programmi). </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Autorizzazioni oggetto</p></td> 
   <td> <p>Autorizzazioni di Contribute o di livello superiore per l'area di lavoro <!--<span class="preview">and record type</span>--> in cui si desidera creare oggetti. </p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p>
   <p>Gestisci le autorizzazioni per gli oggetti Workfront (portfolio) per aggiungere oggetti figlio (progetti).</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modello di layout</p></td> 
   <td> <p>A tutti gli utenti, inclusi gli amministratori di Workfront, deve essere assegnato un modello di layout che includa l'area Planning nel menu principale </p> </td> 
  </tr> 
</tbody> 
</table>

*Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Considerazioni sulla creazione di oggetti e record mediante un&#39;automazione

* Il nome dell&#39;oggetto o del record creato da un&#39;automazione è uguale al nome del record da cui è stato creato.
* I nuovi oggetti o record non sostituiscono quelli esistenti nello stesso campo. Attivando più volte la stessa automazione per lo stesso record, vengono aggiunti i nuovi oggetti o record nello stesso campo connesso del record originale, oltre a quelli creati in precedenza.

<!--hide this for now; they are trying to remove this militation: * The automation adds additional objects only in the Many to many or One to many connection type fields. In the all other cases, the automation creates the object, but it does not connect it to the original record from which the automation is triggered.-->

## Configurare un&#39;automazione in Workfront Planning

È necessario configurare un&#39;automazione per un tipo di record in Workfront Planning prima di poterla utilizzare per creare oggetti.

{{step1-to-planning}}

1. Fare clic su una scheda del tipo di record, quindi sul nome di un record.

   Viene visualizzata la pagina del tipo di record.
1. Fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) a destra del nome del tipo di record, quindi fai clic su **Gestisci automazioni**.

   Viene visualizzato l&#39;elenco delle automazioni disponibili per il tipo di record selezionato.

1. Fai clic su **Nuova automazione** nell&#39;angolo superiore destro dello schermo. Viene visualizzata la casella **Nuova automazione**.
1. Aggiorna i campi seguenti:

   * Sostituisci **Automazione senza titolo** con il testo che desideri visualizzare sul pulsante di automazione. Gli utenti faranno clic su questo pulsante quando utilizzano l&#39;automazione per creare un oggetto Workfront o un record Planning.
   * **Descrizione**: aggiungere una descrizione per identificare lo scopo dell&#39;automazione.
1. Fai clic su **Salva**.
Viene visualizzata la pagina dei dettagli dell’automazione.

1. Nella pagina dei dettagli dell&#39;automazione, aggiorna i campi seguenti nella sezione **Triggers**:

   * **Trigger**: selezionare l&#39;azione che attiverà l&#39;automazione. Selezionare ad esempio **Pulsante clic**. <!--update this step with a list of all possible triggers; right now only Button click is available-->

1. Aggiorna i campi seguenti nella sezione **Azioni**: <!--submitted bugs for these fields - see if they need changing here-->
   * **Azioni**: selezionare l&#39;azione che si desidera venga eseguita da Workfront quando si attiva l&#39;automazione. Questo campo è obbligatorio.
Selezionare una delle azioni seguenti:

      * Crea gruppo
      * Crea programma
      * Crea portfolio
      * Crea progetto
      * Crea record

     >[!TIP]
     >
     >Dopo aver salvato l’automazione, non puoi più modificare l’azione selezionata in questo campo.

1. (Condizionale) A seconda dell’azione selezionata, aggiorna i campi seguenti:

   * **Crea progetto**:
      * **Campo connesso in cui viene creato l&#39;oggetto**: campo connesso in cui verrà visualizzato il nuovo progetto. Questo è un campo obbligatorio.
      * **Modello di progetto**: selezionare un modello di progetto che verrà utilizzato da Workfront per creare il progetto.
   * **Crea portfolio**:
      * **Campo connesso in cui viene creato l&#39;oggetto**: campo connesso in cui verrà visualizzato il nuovo portfolio. Questo è un campo obbligatorio.
      * **Modulo personalizzato da allegare al nuovo portfolio**: selezionare un modulo personalizzato da allegare al nuovo portfolio. È necessario creare un modulo personalizzato portfolio prima di poterlo selezionare.
   * **Crea programma**:
      * **Campo connesso in cui viene creato l&#39;oggetto**: campo connesso in cui verrà visualizzato il nuovo programma. Questo è un campo obbligatorio.
      * **Portfolio programmi**: seleziona un portfolio in cui verrà aggiunto il nuovo programma. Questo è un campo obbligatorio.
      * **Modulo personalizzato da allegare al nuovo programma**: selezionare un modulo personalizzato da allegare al nuovo programma. È necessario creare un modulo personalizzato per il programma prima di selezionarlo.
   * **Crea gruppo**:
      * **Campo connesso in cui viene creato l&#39;oggetto**: campo connesso in cui verrà visualizzato il nuovo gruppo. Questo è un campo obbligatorio.
      * **Modulo personalizzato da allegare al nuovo gruppo**: selezionare un modulo personalizzato da allegare al nuovo programma. È necessario creare un modulo personalizzato per il programma prima di selezionarlo.
   * **Crea record**:
      * **Tipo di record**: selezionare il tipo di record da creare.

     Viene visualizzata la sottosezione **Settings**. Aggiorna i campi seguenti nella sottosezione **Impostazioni**:

      * **Campo nel tipo di record connesso in cui verrà visualizzato il record corrente**: questo è il campo connesso nel tipo di record selezionato per l&#39;azione in cui verrà visualizzato il record corrente.

     Ad esempio, se stai creando un’automazione da cui le campagne devono collegare i record di prodotto, questo è il campo connesso nel tipo di record Prodotto da cui verranno visualizzate le campagne, dopo che i prodotti sono stati creati utilizzando l’automazione.

     Questo è un campo obbligatorio.

     <!--submitted a change in functionality and UI text for this - revise??-->
      * **Mappa campi**
         * **Trasferisci da**: seleziona i campi dal tipo di record per il quale viene creata l&#39;automazione per eseguirne il mapping ai campi del tipo di record connesso.
         * **Trasferisci a**: seleziona dal nuovo record appena creato i campi che verranno compilati con le informazioni del record da cui stai eseguendo l&#39;automazione.

     >[!TIP]
     >
     >I tipi di campo del tipo di record originale devono corrispondere ai tipi di campo del nuovo tipo di record creato.

1. (Facoltativo e condizionale) Se hai scelto di creare un record, fai clic su **Aggiungi campi** per mappare campi di ricerca aggiuntivi da un record all&#39;altro.
1. (Condizionale) Se hai selezionato di creare un record e non sono presenti campi di connessione tra il tipo di record originale e il tipo di record selezionato nell&#39;area **Azioni**, fai clic sull&#39;icona del punto interrogativo a destra del **Campo del tipo di record connesso in cui verrà visualizzato il campo** del record corrente, quindi fai clic sull&#39;icona **Aggiungi** ![Crea un&#39;icona del campo di connessione](assets/create-a-connection-field-icon.png) per aggiungere un campo di connessione.

   Il nuovo campo viene creato automaticamente per il tipo di record selezionato nell&#39;area **Azioni** e denominato **Record connesso**.

   Un campo connesso per il tipo di record selezionato viene creato anche nel tipo di record originale da cui si sta configurando l&#39;automazione.
1. (Facoltativo e condizionale) Se hai selezionato di creare un oggetto Workfront e non disponi di un campo di connessione per il tipo di oggetto Workfront selezionato, fai clic sull&#39;icona del punto interrogativo a destra del campo **Connected field where the &lt; Workfront object type name > is created** field e fai clic sull&#39;icona **Add** ![Create a connection field icon](assets/create-a-connection-field-icon.png) per aggiungere un campo di connessione.

   ![Icona punto interrogativo per aggiungere campi connessi nelle automazioni con Workfront](assets/question-mark-icon-to-add-connected-fields-in-automations-with-workfront.png)

   Il nuovo campo viene creato automaticamente e denominato **Connected &lt; nome oggetto Workfront >**. Ad esempio, quando per il record viene creato un campo connesso a un portfolio, questo viene denominato &quot;Portfolio connesso&quot;.

1. Fai clic su **Salva** nell&#39;angolo superiore destro della pagina dei dettagli di automazione.

   L’automazione viene visualizzata nell’elenco delle automazioni ed è disponibile per l’utilizzo nei record.

## Gestione delle automazioni esistenti

{{step1-to-planning}}

1. Fare clic su una scheda del tipo di record, quindi sul nome di un record.

   Viene visualizzata la pagina del tipo di record.
1. Fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) a destra del nome del tipo di record, quindi fai clic su **Gestisci automazioni**.

   Viene visualizzato l&#39;elenco delle automazioni disponibili per il tipo di record selezionato.

1. (Facoltativo) Per modificare, disabilitare o eliminare un&#39;automazione, effettuate una delle seguenti operazioni:

   1. Dall&#39;elenco delle automazioni, passa il puntatore sul nome di un&#39;automazione salvata, quindi fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png).

   1. Fai clic su **Modifica** per aggiornare le informazioni sui campi e configurarli nell&#39;automazione.

      >[!TIP]
      >
      >   Non puoi modificare l’azione selezionata originariamente per un’automazione.


   1. Fare clic su **Disattiva** per rimuovere l&#39;automazione dalla vista tabella del record e impedire agli utenti di utilizzarla per creare record o oggetti.

   I record creati con un&#39;automazione disabilitata rimangono connessi al record selezionato originariamente.

   Per renderla nuovamente disponibile, fai clic di nuovo sul menu **Altro** ![Altro menu](assets/more-menu.png), quindi fai clic su **Attiva**.
   1. Fai clic su **Elimina** per eliminare l&#39;automazione. Non è possibile recuperare un’automazione eliminata.

   I record creati con un&#39;automazione eliminata rimangono connessi al record selezionato originariamente.

## Utilizzare un&#39;automazione di Workfront Planning per creare un oggetto o un record

1. In Workfront Planning aprire la pagina del tipo di record contenente l&#39;automazione che si desidera utilizzare per creare e collegare automaticamente record o oggetti.
1. Aprire la vista tabella.
1. Selezionare uno o più record.

   Nella parte inferiore della tabella viene visualizzata una barra blu con pulsanti aggiuntivi, inclusi i pulsanti di automazione.
1. Fai clic sul pulsante di automazione nell’angolo inferiore destro dello schermo.

   ![Pulsante di automazione](assets/automation-custom-button.png)

   Si verificano le seguenti situazioni:

   * Se l’automazione ha creato un oggetto o un record, nella parte inferiore dello schermo viene visualizzato un messaggio di conferma.

   * Il nuovo oggetto viene visualizzato nel campo connesso indicato nella configurazione del pulsante di automazione. Potrebbe essere necessario aggiornare la pagina prima di visualizzare il nuovo oggetto.

   * Il record da cui stai attivando l’automazione viene aggiunto al campo connesso del nuovo record.

   >[!NOTE]
   >
   >È consigliabile verificare che gli oggetti o i record siano stati creati e connessi come previsto.

1. (Facoltativo) Fare clic sul nuovo oggetto nel campo connesso. Viene visualizzata la pagina dell&#39;oggetto e potete apportare ulteriori modifiche al nuovo oggetto.

<!--ORIGINAL AUTOMATION FUNCTIONALITY - BEFORE FEB. 20, 2025

You can configure automations in Adobe Workfront Planning that, when activated, create objects in Workfront or records in Workfront Planning when triggered from a Planning record. The created objects or records are automatically connected to the records you are triggering the automation from. 

You can configure and activate the automation in the record type's page in Workfront Planning. The connected object that is created is placed in the connected field of the record type you run the automation from. 

For example, you could create an automation that takes a Workfront Planning campaign and creates a project in Workfront to track that campaign's progress. The project would be connected to the Workfront Planning campaign in the Connected Project field on the campaign.

For more information on connected records, see [Connected records overview](/help/quicksilver/planning/records/connected-records-overview.md).

## Access requirements

+++ Expand to view access requirements.. 

You must have the following access to perform the steps in this article:  

 <table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access all the capabilities of Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td> Standard
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p> 
   <p>Edit access in Workfront for the object types that you want to create (projects, portfolios, programs). </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td> <p>Manage permissions to the workspace you want to add records to. </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
   <p>Manage permissions to Workfront objects (portfolios) to add children objects (projects).</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layout template</p></td> 
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Planning area in the Main Menu </p> </td> 
  </tr> 
</tbody> 
</table> 

 *For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).   

+++


## Considerations about creating objects and records using an automation

* The new object or record name is the same as the record name from which you create it. 
* New objects or records don't override existing ones in the same field. Triggering the same automation multiple times for the same records adds the new objects or records in the same connected field of the original record, in addition to the ones created before. 
* The automation adds additional objects only in the Many to many or One to many connection type fields. In the all other cases, the automation creates the object, but it does not connect it to the original record from which the automation is triggered. 

## Configure an automation in Workfront Planning

You must configure an automation for a record type in Workfront Planning, before you can use it to create objects.

{{step1-to-planning}}

1. Click a record type card, then click the name of a record. 

   The record type page opens. 
1. Click the **More** menu ![More menu](assets/more-menu.png) to the right of the record type name, then click **Manage automations**. 

   The list of available automations for the selected record type opens.

1. Click **New automation** in the upper-right corner of the screen. The **New automation** box opens.
1. Update the following fields:

   * Replace **Untitled automation** with the text that you want to appear on the automation button. Users will click this button when using the automation to create a Workfront object or a Planning record.
   * **Description**: Add a description to identify the purpose of the automation.
1. Click **Save**.
   The automation details page opens. 

1. On the automation's details page, update the following fields in the **Triggers** section: 

   * **Trigger**: Select the action that will trigger the automation. For example, select **Button click**. (********update this step with a list of all possible triggers; right not only Button click is available***********)

1. Update the following fields in the **Actions** section: <********submitted bugs for these fields - see if they need changing here*********)
   * **Object type**: Select the object that you want the automation to create. This is a required field.
      
      You can create the following objects from Workfront Planning records: 

      * Project
      * Portfolio
      * Program
      * Group
      * Record

      >[!TIP]
      >
      >After you saved the automation, you can no longer change the object type in this field.

1. (Conditional) Depending on what type of object you want to create, update the following fields:


   * **Project**: 
      * **Connected field where the object is created**: This is the connected field where the new project will display. This is a required field. 
      * **Template from which to create the project**: Select a project template that Workfront will use to create the project.  
   * **Portfolio**:
      * **Connected field where the object is created**: This is the connected field where the new portfolio will display. This is a required field.
      * **Custom form to attach to the new portfolio**: Select a custom form to attach to the new portfolio. You must create a portfolio custom form before you can select it. 
   * **Program**: 
      * **Connected field where the object is created**: This is the connected field where the new program will display. This is a required field.
      * **Program portfolio**: Select a portfolio where the new program will be added. This is a required field.
      * **Custom form to attach to the new program**: Select a custom form to attach to the new program. You must create a program custom form before you can select it. 
   * **Group**:
      * **Connected field where the object is created**: This is the connected field where the new group will display. This is a required field.
      * **Custom form to attach to the new group**: Select a custom form to attach to the new program. You must create a program custom form before you can select it. 
   * **Record**: 
      * **Connected record type**: Select the record type you want to create. 
      * **Connected field where the record is created**: This is the connected field where the new record will display. This is a required field. (******this might need revision as right now it shows the field on the connected record table where the current record will display; submitted a bug to correct this label*********)
      * **Map fields**
         * **Transfer from**: Select fields from the record type the automation is created for to map them to the fields of the connected record type. 
      * **Transfer to**: Select fields from the newly created record that will populate with information from the record you are running the automation from. 
1. (Optional and conditional) If you selected to create a record, click **Add fields** to map additional lookup fields from one record to another.
1. (Optional and conditional) If you don't have a connection field for a Workfront object type, click the **Create a connection field** icon ![Create a connection field icon](assets/create-a-connection-field-icon.png) to add a field.

   The new field is automatically created and named **Connected < Workfront object name >**. For example, when a portfolio connected field is created for the record, it is named "Connected portfolio." 

1. Click **Save** in the upper-right corner of the automation details page. 

   The automation displays on the list of automations, and is available to use in records.
1. (Optional) To edit, disable, or delete an automation, do the following:

   1. From the list of automations, hover over the name of a saved automation, then click the **More** menu ![More menu](assets/more-menu.png).

   1. Click **Edit** to update information about and configure fields on the automation.
   1. Click **Disable** to remove the automation from the table view and prevent users from using it to create records or objects. To make it available again, click the **More** menu ![More menu](assets/more-menu.png) again, then click **Activate**.
   1. Click **Delete** to delete the automation. A deleted automation cannot be recovered. Records that have been created using the automation remain connected to the record originally selected.  

## Use a Workfront Planning automation to create an object or a record

1. In Workfront Planning, open the record type page that contains the records you want to use to create Workfront objects or Planning records. 
1. Open the table view. 
1. Select one or more records.
   
   A blue bar displays at the bottom of the table with additional buttons, including automation buttons. 
1. Click the automation button near the lower-right corner of the screen. 

   ![Automation button](assets/automation-custom-button.png)

   A confirmation message displays at the bottom of the screen, if the automation successfully created an object or a record. 

   The new object displays in the connected field you indicated in the setup of the automation button. You might need to refresh your page before viewing the new object. 

   >[!NOTE]
   >
   >We recommend checking that the object was created and connected as expected.

1. (Optional) Click the new object in the connected field. The object page opens and you can make additional changes to the new object. 

-->

