---
title: Creare record importando informazioni da un file CSV o Excel
description: I record sono singole istanze di tipi di record, che sono i tipi di oggetto di Adobe Workfront Planning. In Workfront Planning è possibile creare record importando informazioni da un file CSV o Excel.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 940945df-391c-4672-9d9d-180d5028509b
source-git-commit: e26a3d0e283182e08902c263252c8d067838c23a
workflow-type: tm+mt
source-wordcount: '826'
ht-degree: 0%

---


# Creare record importando informazioni da un file CSV o Excel

<!--

<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

I record sono singole istanze di tipi di record, che sono i tipi di oggetto di Adobe Workfront Planning. In Workfront Planning è possibile creare record importando informazioni da un file CSV o Excel.

Per ulteriori informazioni sulla creazione di record, vedere [Crea record](/help/quicksilver/planning/records/create-records.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Pacchetto Adobe Workfront</p></td> 
   <td> 
<p>Qualsiasi pacchetto Workfront e Planning</p> <p>Qualsiasi flusso di lavoro e qualsiasi pacchetto di Planning</p>
<p>Per ulteriori informazioni su ciò che è incluso in ogni pacchetto Workfront Planning, contattare il rappresentante del proprio account Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Licenza Adobe Workfront</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr>

<tr> 
   <td role="rowheader"><p>Autorizzazioni oggetto</p></td> 
   <td> <p>Autorizzazioni Contribute o superiori per l'area di lavoro e il tipo di record in cui si importano i record. </p>
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p>
   </td> 
  </tr>  
</tbody> 
</table>

Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++  


<!--Old:
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
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
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
   <p>Edit access in Workfront for the object types that you want to create (projects, programs, and portfolios) as you connect them from new records  </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td> <p>Contribute or higher permissions to the workspace and record type where you want to add records. </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
   <p>Manage permissions to Workfront objects (portfolios) to add children objects (projects).</p>
   </td> 
  </tr> 
</tbody> 
</table> -->


## Considerazioni sull&#39;importazione di record utilizzando un file Excel o CSV

* Le intestazioni delle colonne di ciascun foglio diventano i campi associati ai record.
* Ogni riga di ogni foglio diventa un record univoco associato.
* Se il file di Excel contiene più fogli, vengono importate solo le informazioni di un foglio selezionate durante il processo di importazione.
* Il file non deve superare i seguenti valori:
   * 25.000 righe
   * 500 colonne
* Il file non deve superare i 5 MB.
* I fogli vuoti non sono supportati.
* I campi dei tipi seguenti non sono supportati e non possono essere mappati ai campi del foglio di importazione:

   * Campi di connessione ai tipi di oggetto Workfront e AEM Assets. È possibile eseguire il mapping solo dei campi di connessione ai tipi di record di Planning.
   * Campi di ricerca da record di Planning o oggetti Workfront e AEM Assets connessi
   * Campi formula
   * Data di creazione, Creato da
   * Data ultima modifica, Autore ultima modifica
   * Data di approvazione, Approvato da
   * People
   * Se viene importato un campo a selezione multipla o singola che dispone di più scelte rispetto a un campo simile in Planning, le opzioni aggiuntive vengono create durante l&#39;importazione. Solo gli utenti con le autorizzazioni di gestione per l&#39;area di lavoro possono importare nuove scelte.

## Creare record importando un file CSV o Excel

{{step1-to-planning}}

1. Fare clic sull&#39;area di lavoro in cui si desidera creare i record.

   Oppure

   Da un workspace, espandere la freccia rivolta verso il basso a destra del nome di un workspace esistente, cercare un workspace e selezionarlo quando viene visualizzato nell&#39;elenco.
1. Fare clic sulla scheda del tipo di record in cui si desidera importare i record.
1. Fai clic su **Nuovo record** nell&#39;angolo superiore destro della schermata.

   ![Scegliere la modalità di aggiunta dei record nella casella con tre pulsanti](assets/choose-way-to-add-records-three-button-box.png)
1. Fai clic su **Carica dal file**, quindi su **Continua**. <!--add screen shot when all three buttons are added - with the Submit a request button-->
1. Trascina e rilascia un file Excel o CSV salvato in precedenza sul computer, oppure fai clic su **Seleziona un file CSV o Excel** per cercarne uno.
1. Fare clic su **Anteprima e modifica**.
1. (Condizionale) Se il file importato contiene più di un foglio, selezionare il pulsante di opzione del foglio da importare nella casella **Seleziona un foglio da importare**, quindi fare clic su **Avanti**. In caso contrario, procedere al passaggio successivo.

   ![Selezionare un foglio per importare i record](assets/select-a-sheet-to-import-box.png)
1. In **Mappare i campi di Planning nelle intestazioni di colonna** selezionare il **campo di Planning** che corrisponde meglio alle informazioni in ciascuna colonna del foglio.

   ![Mappa i campi di Planning alle colonne durante l&#39;importazione dei record](assets/map-planning-fields-to-columns-when-importing-records.png)

   Ogni riga rappresenta un nuovo record. Nella casella Anteprima e modifica vengono visualizzati solo i primi 10 record.

   >[!TIP]
   >
   >Non tutti i tipi di campo sono supportati. Per ulteriori informazioni, vedere la sezione [Considerazioni sull&#39;importazione di record utilizzando un file Excel o CSV](#considerations-about-importing-records-using-an-excel-or-csv-file) in questo articolo.


1. (Facoltativo e condizionale) Se disponi delle autorizzazioni di gestione per l&#39;area di lavoro, seleziona **Crea opzioni mancanti** nell&#39;angolo inferiore sinistro dello schermo. Quando questa opzione è attivata, vengono aggiunte le scelte mancanti dei campi a selezione singola e multipla.

   >[!NOTE]
   >
   >Ad esempio, se il tipo di record selezionato dispone di un campo Stato a selezione singola con le opzioni Nuovo, In corso e Chiuso e un campo Stato importato da un file dispone anche di una scelta Stato in sospeso, viene aggiunta anche la scelta Stato in sospeso.
   >
   >Se non si dispone delle autorizzazioni Gestione per l&#39;area di lavoro, è possibile importare i record, ma le scelte aggiuntive non verranno create. Viene invece visualizzato il seguente messaggio nell&#39;angolo superiore destro della casella Mappa i campi di Planning sulle intestazioni di colonna: **Le scelte che non esistono nella connessione, i campi a selezione singola o multipla non verranno aggiunti**.

1. Fai clic su **Importa**.

   Le informazioni seguenti vengono importate in Workfront Planning:

   * Nuovi record visualizzati nella parte inferiore della vista tabella del tipo di record selezionato.
   * Nuovi valori di campo per i campi esistenti associati a ciascun record.
   * Nuove scelte di un campo a selezione multipla o singola non esistente in Planning.  <!--when we add connected records - add those here too-->

   È possibile iniziare a gestire campi e record nella pagina dei tipi di record.

   Tutti coloro che hanno accesso a Workfront Planning e all&#39;area di lavoro ora possono visualizzare e modificare i record importati e le relative informazioni.

   <!--when we add connected records and the info icon in the tool changes, also add those items to the Import step and to the NOTE above it-->
