---
title: Creazione di oggetti Workfront mediante Adobe Workfront Planning Record Automations
description: In Workfront Planning è possibile configurare automazioni che, se attivate, creano oggetti in Workfront.
hide: true
hidefromtoc: true
exl-id: c669217a-40e2-471f-951d-93157a34f1ee
source-git-commit: 00e58ea9a207037b701e1be010c2c4c2995d60e0
workflow-type: tm+mt
source-wordcount: '1252'
ht-degree: 3%

---

# Creazione di oggetti mediante le automazioni dei record di Adobe Workfront Planning

<!--add screen shots when UI is finalized AND redo all the steps - some things got changed and moved around-->
<!--when you make this public, add this to the metadata above (and take the "hide" tags out):

feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog

-->

<!-- if they give access to use the automation to people with LESS than Manage permissions to a workspace, split this article in two: the Configure section should be for admins and the "Use a Workfront Planning automation to create an object" should be for all other users-->

In Adobe Workfront Planning è possibile configurare automazioni che, se attivate, creano oggetti in Workfront o Workfront Planning.

Puoi configurare e attivare l’automazione nella pagina del record. L&#39;oggetto creato viene connesso al record Planning e inserito nel campo specificato nell&#39;automazione.

Ad esempio, è possibile creare un&#39;automazione che accetta una campagna di Workfront Planning e crea un progetto in Workfront per tenere traccia dell&#39;avanzamento della campagna. Il progetto sarà collegato alla campagna di pianificazione di Workfront.

Per ulteriori informazioni sui record connessi, vedere [Panoramica sui record connessi](/help/quicksilver/planning/records/connected-records-overview.md).

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
   <td> <p>Consente di gestire le autorizzazioni per l'area di lavoro a cui si desidera aggiungere record. </p>  
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

* Il nome del nuovo oggetto o record corrisponde al nome del record da cui è stato creato.
* Se nel record utilizzato per l&#39;automazione sono già connessi oggetti dello stesso tipo nel campo a cui si desidera aggiungere nuovi oggetti, i nuovi oggetti vengono aggiunti al campo di connessione e anche gli oggetti esistenti rimangono connessi.

## Configurare un&#39;automazione in Workfront Planning

È necessario configurare un&#39;automazione in Workfront Planning prima di poterla utilizzare per creare oggetti.

{{step1-to-planning}}

1. Fare clic su una scheda del tipo di record, quindi sul nome di un record.

   Viene visualizzata la pagina del tipo di record.
1. Fai clic sul menu **Altro** ![](assets/more-menu.png) a destra del nome del tipo di record, quindi fai clic su **Gestisci automazioni**.

   Viene visualizzato l’elenco delle automazioni disponibili.

1. Fai clic su **Nuova automazione** nell&#39;angolo superiore destro dello schermo. Viene visualizzata la casella **Nuova automazione**.
1. Aggiorna i campi seguenti:

   * Sostituisci **Automazione senza titolo** con il testo che desideri visualizzare sul pulsante di automazione. Gli utenti faranno clic su questo pulsante quando utilizzano l’automazione per creare un oggetto Workfront.
   * **Descrizione**: aggiungere una descrizione per identificare lo scopo dell&#39;automazione.

1. Nella pagina dei dettagli dell&#39;automazione, aggiorna i campi seguenti nella sezione **Triggers**:

   * **Trigger**: selezionare l&#39;azione che attiverà l&#39;automazione. Selezionare ad esempio **Pulsante clic**. <!--update this step with a list of all possible triggers; right not only Button click is available-->

1. Aggiorna i campi seguenti nella sezione **Azioni**:
   * **Tipo di oggetto**: selezionare l&#39;oggetto da creare con l&#39;automazione. Questo è un campo obbligatorio.

     È possibile creare i seguenti oggetti dai record di Workfront Planning:

      * Progetto
      * Portfolio
      * Programma
      * Gruppo
      * Inserimento
1. (Condizionale) A seconda del tipo di oggetto da creare, aggiorna i campi seguenti:

   * **Progetto**:
      * **Campo connesso in cui viene creato l&#39;oggetto**: campo connesso in cui verrà visualizzato il nuovo progetto. Questo campo è obbligatorio
      * **Modello da cui creare il progetto**: selezionare un modello di progetto che verrà utilizzato da Workfront per creare il progetto.
   * **Portfolio**:
      * **Campo connesso in cui viene creato l&#39;oggetto**: campo connesso in cui verrà visualizzato il nuovo portfolio. Questo è un campo obbligatorio.
      * **Modulo personalizzato da allegare al nuovo portfolio**: selezionare un modulo personalizzato da allegare al nuovo portfolio. È necessario creare un modulo personalizzato portfolio prima di poterlo selezionare.
   * **Programma**:
      * **Campo connesso in cui viene creato l&#39;oggetto**: campo connesso in cui verrà visualizzato il nuovo programma. Questo è un campo obbligatorio.
      * **Portfolio programmi**: seleziona un portfolio in cui verrà aggiunto il nuovo programma. Questo è un campo obbligatorio.
      * 
         * **Modulo personalizzato da allegare al nuovo programma**: selezionare un modulo personalizzato da allegare al nuovo programma. È necessario creare un modulo personalizzato per il programma prima di selezionarlo.
   * **Gruppo**:
      * **Campo connesso in cui viene creato l&#39;oggetto**: campo connesso in cui verrà visualizzato il nuovo gruppo. Questo è un campo obbligatorio.
      * **Modulo personalizzato da allegare al nuovo gruppo**: selezionare un modulo personalizzato da allegare al nuovo programma. È necessario creare un modulo personalizzato per il programma prima di selezionarlo.
   * **Record**:
      * **Tipo di record connesso**: selezionare il tipo di record che si desidera creare.
      * **Campo connesso in cui viene creato il record**: campo connesso in cui verrà visualizzato il nuovo record. Questo è un campo obbligatorio.
      * **Campo mappa**: selezionare i campi dal tipo di record per il quale viene creata l&#39;automazione per eseguirne il mapping ai campi del tipo di record connesso.
      * **Al campo record connesso**: selezionare dal record connesso i campi corrispondenti ai campi del tipo di record per cui si crea l&#39;automazione.
1. (Facoltativo e condizionale) Se non si dispone di un campo connessione per un tipo di oggetto Workfront, fare clic sull&#39;icona **Crea un campo connessione** ![](assets/create-a-connection-field-icon.png) per aggiungere un campo.
1. (Facoltativo e condizionale) Se hai scelto di aggiungere un record, fai clic su **Aggiungi** nell&#39;area **Mappa campi** per aggiungere e mappare campi aggiuntivi, quindi seleziona un campo a **Trasferisci da** e un campo a **Trasferisci a** per indicare quale campo del record selezionato originariamente deve essere visualizzato in quale campo del record connesso.
1. Fai clic su **Salva**.

   L’automazione viene visualizzata nell’elenco delle automazioni ed è disponibile per l’utilizzo nei record.
1. (Facoltativo) Per modificare, disabilitare o eliminare un&#39;automazione, effettuare le seguenti operazioni:

   Nell&#39;elenco delle automazioni, passare il puntatore del mouse sul nome di un&#39;automazione salvata, quindi fare clic sul menu **Altro** ![](assets/more-menu.png) e scegliere una delle opzioni seguenti:

   * **Modifica**: aggiorna le informazioni e configura i campi nell&#39;automazione.
   * **Disabilita**: l&#39;automazione non verrà visualizzata come opzione nella barra degli strumenti della vista tabella dei record e gli utenti non potranno più utilizzarla per creare record o oggetti. Per renderla nuovamente disponibile, fai clic di nuovo sul menu **Altro** ![](assets/more-menu.png), quindi fai clic su **Attiva**.
   * **Elimina**: l&#39;automazione viene eliminata e non può essere ripristinata. I record creati con l&#39;automazione rimangono collegati al record selezionato originariamente.

## Utilizzare un&#39;automazione di Workfront Planning per creare un oggetto

1. In Workfront Planning aprire la pagina del tipo di record contenente i record che si desidera utilizzare per creare oggetti Workfront.
1. Aprire la vista tabella.
1. Selezionare uno o più record.

   Nella parte inferiore della tabella viene visualizzata una barra blu con pulsanti aggiuntivi, inclusi i pulsanti di automazione.
1. Fai clic sul pulsante di automazione nell’angolo inferiore destro dello schermo.

   ![Pulsante di automazione](assets/automation-custom-button.png)

   Il nuovo oggetto viene visualizzato nel campo connesso indicato nella configurazione del pulsante di automazione.

   >[!NOTE]
   >
   >È consigliabile verificare che l&#39;oggetto sia stato creato e connesso come previsto.

1. (Facoltativo) Fare clic sul nuovo oggetto nel campo connesso. Viene visualizzata la pagina dell&#39;oggetto e potete apportare ulteriori modifiche al nuovo oggetto.

<!--you might need to add something about notifications and emails?!-->
