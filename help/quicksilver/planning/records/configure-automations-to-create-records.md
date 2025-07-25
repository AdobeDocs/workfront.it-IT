---
title: Configurare Adobe Workfront Planning Automations
description: In Adobe Workfront Planning è possibile configurare automazioni che, se attivate, creano oggetti in Workfront o record in Workfront Planning. Gli oggetti e i record creati vengono automaticamente connessi ai record di Planning esistenti. Questo articolo descrive come gestire le automazioni, incluso come modificarle, disabilitarle o eliminarle.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: cde20e5a-15a2-413a-8de4-ccf6eeb4395f
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '1687'
ht-degree: 3%

---

# Configurare le automazioni di Adobe Workfront Planning

<!--add screen shots when UI is finalized AND redo all the steps - some things got changed and moved around-->

<!--you might need to add something about notifications and emails?!-->
<!--add a new section to this article to mention a new way to create objects: help/quicksilver/planning/records/create-records.md-->
<!-- add a new section to this article to mention a new way to create WF objects from Planning: help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md-->

<!-- if they give access to use the automation to people with LESS than Manage permissions to a workspace, split this article in two: the Configure section should be for admins and the "Use a Workfront Planning automation to create an object" should be for all other users-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

È possibile configurare le automazioni in Adobe Workfront Planning che, se attivate, creano oggetti in Workfront o record in Workfront Planning quando attivate da un record Planning. Gli oggetti o i record creati vengono automaticamente collegati ai record da cui si sta attivando l&#39;automazione.

È possibile configurare e attivare l&#39;automazione nella pagina del tipo di record in Workfront Planning.

Ad esempio, è possibile creare un&#39;automazione che accetta una campagna di Workfront Planning e crea un progetto in Workfront per tenere traccia dell&#39;avanzamento della campagna.

Questo articolo descrive come gestire le automazioni, tra cui come modificarle, disattivarle, eliminarle e attivarle per creare oggetti e record.

Per informazioni sulla creazione di record o oggetti mediante un&#39;automazione esistente, vedere [Creare oggetti mediante le automazioni dei record di Adobe Workfront Planning](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md).

## Requisiti di accesso

+++ Espandere per visualizzare i requisiti di accesso.

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
<p>Per poter accedere a Workfront Planning, l’istanza di Workfront della tua organizzazione deve essere integrata in Adobe Unified Experience.</p> 
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
   <p>Accesso di modifica con accesso a Crea oggetti in Workfront per i tipi di oggetto che si desidera creare (progetti, portfolio, programmi). </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Autorizzazioni oggetto</p></td> 
   <td> <p>Gestisci le autorizzazioni per l’area di lavoro e per il tipo di record in cui desideri creare automazioni. </p>
   <p>Gli amministratori di sistema dispongono delle autorizzazioni di gestione per tutte le aree di lavoro, incluse quelle che non hanno creato</p>
   </td> 
  </tr> 
</tbody> 
</table>

*Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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

      * Creazione di più progetti
      * Crea un progetto singolo
      * Crea progetto
      * Crea record
      * Crea programma
      * Crea portfolio
      * Crea gruppo

     >[!TIP]
     >
     >Dopo aver salvato l’automazione, non puoi più modificare l’azione selezionata in questo campo.

1. (Condizionale) A seconda dell’azione selezionata, aggiorna i campi seguenti:

   * **Crea un singolo progetto**: <!--replace to the left: Create a single project-->
      * **Campo connesso in cui viene creato il progetto**: campo connesso in cui verrà visualizzato il nuovo progetto. Questo è un campo obbligatorio.
      * **Modello di progetto**: selezionare un modello di progetto che verrà utilizzato da Workfront per creare il progetto.

   * Creazione di più progetti:
      * **Campo connesso in cui viene creato il progetto**: campo connesso in cui verrà visualizzato il nuovo progetto. Questo è un campo obbligatorio.
      * **Campo le cui scelte creeranno i record**: scegliere un campo a selezione multipla o singola dal tipo di record selezionato. Workfront crea un progetto per ogni scelta di campo attualmente selezionata nel record da cui si attiva l’automazione.

     >[!TIP]
     >
     >Un progetto viene creato solo per le opzioni attualmente selezionate nel campo a selezione multipla o singola del record da cui si sta eseguendo l’automazione e non per tutte le opzioni possibili per tale campo.
     >

      * **Usa lo stesso modello**: selezionare questa opzione per utilizzare lo stesso modello per ogni nuovo progetto. Se l&#39;opzione è deselezionata, selezionare un **modello di progetto** per ogni scelta di campo.
      * **Modello di progetto**: se è stata selezionata l&#39;opzione **Usa lo stesso modello**, selezionare un modello di progetto che verrà utilizzato da Workfront per creare i progetti.

   * **Crea portfolio**:
      * **Campo connesso in cui viene creato il portfolio**: campo connesso in cui verrà visualizzato il nuovo portfolio. Questo è un campo obbligatorio.
      * **Modulo personalizzato da allegare al nuovo portfolio**: selezionare un modulo personalizzato da allegare al nuovo portfolio. È necessario creare un modulo personalizzato portfolio prima di poterlo selezionare.
   * **Crea programma**:
      * **Campo connesso in cui viene creato il programma**: campo connesso in cui verrà visualizzato il nuovo programma. Questo è un campo obbligatorio.
      * **Portfolio programmi**: seleziona un portfolio in cui verrà aggiunto il nuovo programma. Questo è un campo obbligatorio.
      * **Modulo personalizzato da allegare al nuovo programma**: selezionare un modulo personalizzato da allegare al nuovo programma. È necessario creare un modulo personalizzato per il programma prima di selezionarlo.
   * **Crea gruppo**:
      * **Campo connesso in cui viene creato il gruppo**: campo connesso in cui verrà visualizzato il nuovo gruppo. Questo è un campo obbligatorio.
      * **Modulo personalizzato da allegare al nuovo gruppo**: selezionare un modulo personalizzato da allegare al nuovo programma. È necessario creare un modulo personalizzato per il programma prima di selezionarlo.
   * **Crea record**:
      * **Tipo di record**: selezionare il tipo di record da creare.

        Viene visualizzata la sottosezione **Settings**. Aggiorna i campi seguenti nella sottosezione **Impostazioni**:

         * **Campo nel tipo di record connesso in cui verrà visualizzato il record corrente**: questo è il campo connesso nel tipo di record selezionato per l&#39;azione in cui verrà visualizzato il record corrente.

        Ad esempio, se stai creando un’automazione da cui le campagne devono collegare i record di prodotto, questo è il campo connesso nel tipo di record Prodotto da cui verranno visualizzate le campagne, dopo che i prodotti sono stati creati utilizzando l’automazione.

        Questo è un campo obbligatorio.

        <!--submitted a change in functionality and UI text for this - revise??-->
Nell&#39;area **Mappa campi**, aggiorna le seguenti informazioni:

         * **Trasferisci da**: seleziona i campi dal tipo di record per il quale viene creata l&#39;automazione per eseguirne il mapping ai campi del tipo di record connesso.
         * **Trasferisci a**: seleziona dal nuovo record appena creato i campi che verranno compilati con le informazioni del record da cui stai eseguendo l&#39;automazione.

        >[!TIP]
        >
        >* I tipi di campo del tipo di record originale devono corrispondere ai tipi di campo del nuovo tipo di record creato.
        >* Se non si sceglie alcun campo, i nomi dei nuovi record saranno **Record senza titolo**.

1. (Facoltativo e condizionale) Se hai scelto di creare un record, fai clic su **Aggiungi campi** per mappare campi di ricerca aggiuntivi da un record all&#39;altro.
1. (Condizionale) Se non sono presenti campi di connessione tra il tipo di record originale e il tipo di record selezionato nel campo **Tipo di record**, fare clic su **Aggiungi campo connesso**.

   ![Impostazione automazione per creare un record](assets/automation-setup-create-record.png)

   Vengono creati i due campi seguenti:

   * È stato creato un nuovo campo di connessione denominato **Record connesso** per il tipo di record indicato nel campo **Tipo di record**.
   * Per il tipo di record per cui si sta configurando l&#39;automazione viene creato un nuovo campo di connessione con lo stesso nome di quello indicato nel campo **Tipo di record**.

     Ad esempio, se stai configurando un&#39;automazione per Campaigns per creare automaticamente un altro tipo di record denominato Brands e fai clic su **Aggiungi campo connesso**, vengono creati i seguenti campi:

      * Il campo di connessione **Record connesso** è stato creato per il tipo di record **Marchi**.
      * Il campo di connessione **Brands** è stato creato per il tipo di record **Campagne**.

1. (Facoltativo) Se nell&#39;area Azioni non sono presenti campi di connessione tra il tipo di record originale e l&#39;oggetto Workfront selezionato, fare clic su **Aggiungi campo connesso**.

   ![Installazione dell&#39;automazione per creare più progetti](assets/automation-setup-create-multiple-projects.png)

   Vengono creati i seguenti elementi:

   * Viene creato un nuovo campo di connessione denominato **Connected &lt; nome dell&#39;oggetto Workfront >** per il tipo di record per il quale si genera l&#39;automazione. Ad esempio, viene creato un campo **Progetto connesso** per il tipo di record per il quale si sta creando l&#39;automazione quando si sceglie di creare automaticamente i progetti.
   * Una nuova scheda del tipo di record viene aggiunta alla sezione Pianificazione di un progetto Workfront, in Workfront, con il nome del tipo di record per il quale si sta configurando l’automazione.

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

   1. Fai clic su **Modifica** per aggiornare le seguenti informazioni:

      * Fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) a destra del nome dell&#39;automazione, quindi fai clic su **Modifica** per modificare il nome dell&#39;automazione.
      * Qualsiasi campo nell&#39;automazione, ad eccezione del campo **Azioni**.

        >[!TIP]
        >
        >Non puoi modificare l’azione selezionata originariamente per un’automazione.


   1. Fare clic su **Disattiva** per rimuovere l&#39;automazione dalla vista tabella del record e impedire agli utenti di utilizzarla per creare record o oggetti.

      I record creati con un&#39;automazione disabilitata rimangono connessi al record selezionato originariamente.

      Per renderla nuovamente disponibile, fai clic di nuovo sul menu **Altro** ![Altro menu](assets/more-menu.png), quindi fai clic su **Attiva**.
   1. Fai clic su **Elimina** per eliminare l&#39;automazione. Non è possibile recuperare un’automazione eliminata.

      I record creati con un&#39;automazione eliminata rimangono connessi al record selezionato originariamente.
