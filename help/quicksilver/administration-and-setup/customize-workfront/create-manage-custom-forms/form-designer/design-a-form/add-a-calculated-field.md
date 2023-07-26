---
title: Aggiungere campi calcolati con il progettista del modulo
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: È possibile aggiungere un campo personalizzato calcolato che utilizza dati esistenti per generare nuovi dati quando il modulo personalizzato viene allegato a un oggetto.
author: Courtney
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 407aae49-4bc3-4364-a794-7e170a57a6d3
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '2317'
ht-degree: 0%

---

# Aggiungere campi calcolati con il progettista del modulo

È possibile aggiungere un campo personalizzato calcolato che utilizza dati esistenti per generare nuovi dati quando il modulo personalizzato viene allegato a un oggetto.

Un campo personalizzato calcolato può contenere:

* Un semplice riferimento a un singolo campo incorporato.

  >[!INFO]
  >
  > **Esempio:** Per calcolare i ricavi generati dai progetti e dalle attività, è possibile creare un campo personalizzato calcolato contenente il campo predefinito Ricavi effettivi. Quando un utente allega il modulo personalizzato a un progetto o a un’attività, nel campo vengono visualizzate le entrate relative al progetto o all’attività.

* Espressione che fa riferimento a uno o più campi. Possono essere campi personalizzati, altri campi personalizzati calcolati e campi incorporati.

  >[!INFO]
  >
  >**Esempio:** Per calcolare il profitto generato dai progetti e dalle attività, è possibile creare un campo personalizzato calcolato denominato Profitto contenente un&#39;espressione matematica che sottrae il costo dai ricavi.
  >
  >A tale scopo, è possibile utilizzare l&#39;espressione matematica SUB (sottrazione) con i campi incorporati di Workfront Costo effettivo e Ricavo effettivo.
  >
  >Nei passaggi seguenti puoi vedere come può essere eseguito questo esempio.


## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Piano Adobe Workfront*</p> </td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td>Piano</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Accesso amministrativo ai moduli personalizzati</p> <p>Per informazioni sulle modalità di concessione dell'accesso da parte degli amministratori di Workfront, vedere <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Concedere agli utenti l'accesso amministrativo a determinate aree</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;Per informazioni sulle configurazioni di piano, tipo di licenza o livello di accesso disponibili, contattare l&#39;amministratore Workfront.

## Riutilizzare un campo personalizzato calcolato esistente in un modulo personalizzato

È possibile utilizzare lo stesso campo personalizzato calcolato nei moduli personalizzati che appartengono a oggetti diversi. È ad esempio possibile utilizzare il campo calcolato Profitto creato per il modulo personalizzato del progetto in un modulo personalizzato per le attività.

Quando si utilizza un campo personalizzato calcolato esistente, il calcolo non viene trasferito nel nuovo modulo. È necessario aggiungere nuovamente il calcolo nello stesso campo del nuovo modulo personalizzato.

È inoltre possibile avere un calcolo diverso per lo stesso campo nel nuovo modulo. Mantenere lo stesso nome per il campo personalizzato calcolato garantisce coerenza e uniformità nella convenzione di denominazione.

>[!IMPORTANT]
>
>Le modifiche nelle espressioni calcolate possono causare l’obsolescenza del valore del campo sugli oggetti. Per essere certi di visualizzare sempre il calcolo aggiornato in questi campi, effettuare una delle seguenti operazioni:
>
>* Dopo aver salvato un oggetto in cui sono stati modificati dati in un modulo personalizzato allegato, fare clic sull&#39;icona Altro ![](assets/more-icon.png) nella pagina principale dell&#39;oggetto, quindi Ricalcola espressioni personalizzate.
>* Selezionare l&#39;opzione Ricalcola espressioni personalizzate quando si modificano oggetti in blocco.
>* Selezionare l&#39;opzione Aggiorna calcoli precedenti durante la modifica di un campo personalizzato calcolato in un modulo personalizzato.

Per riutilizzare un campo personalizzato calcolato esistente:

1. Fai clic su **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Clic **Forms personalizzato** nel pannello a sinistra.

   <!-- >[!TIP]
    >
    >In the view that appears, you can review all custom forms and custom fields that have been created for your organization. You can also see who created each form and the fields that are associated with it. -->

1. Clic **Nuovo modulo personalizzato.**
1. Seleziona i tipi di oggetto a cui desideri allegare il modulo personalizzato, quindi fai clic su **Continua**.

1. In alto a sinistra nella schermata, fai clic su **Libreria campi**.

   ![](assets/field-library.png)

1. Utilizza la casella di ricerca o espandi il **Calcolato** per individuare il campo calcolato necessario, quindi trascinare il campo nel punto in cui si desidera visualizzarlo nel modulo personalizzato.

1. (Facoltativo) Ripeti il passaggio precedente per aggiungere altri campi.

   >[!NOTE]
   >
   >È possibile aggiungere fino a 500 campi e widget in un singolo modulo personalizzato. Tuttavia, il calo delle prestazioni può verificarsi quando in un modulo esistono più di 100 moduli, a seconda della complessità.
   >
   >
   >Esempi di moduli complessi includono moduli con parametri a catena, campi di dati personalizzati calcolati e opzioni con più valori in un singolo campo.

1. Per salvare le modifiche, fai clic su **Applica** e passare a un&#39;altra sezione per continuare a creare il modulo.

   oppure

   Clic **Salva e chiudi**.

## Aggiungi un nuovo campo calcolato

>[!IMPORTANT]
>
>Prima di creare un nuovo campo personalizzato calcolato, identificare i campi esistenti che si desidera includere in modo da essere certi che i dati necessari per il calcolo siano presenti in Workfront.

1. Fai clic su **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Clic **Forms personalizzato** nel pannello a sinistra.

   <!-- >[!TIP]
    >
    >In the view that appears, you can review all custom forms and custom fields that have been created for your organization. You can also see who created each form and the fields that are associated with it. -->

1. Clic **Nuovo modulo personalizzato.**
1. Seleziona i tipi di oggetto a cui desideri allegare il modulo personalizzato, quindi fai clic su **Continua**.

1. Sul lato sinistro dello schermo, trovare **Calcolato** e trascinarlo in una sezione dell’area di lavoro.

   ![](assets/drag-field-to-section.png)

1. Sul lato destro della schermata, configura le opzioni disponibili per il tipo di campo personalizzato che stai aggiungendo:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Etichetta</td> 
      <td>Digitare un'etichetta per il campo. Questo è ciò che gli utenti vedranno quando utilizzano il modulo personalizzato. Il campo <b>Nome</b>, che viene compilato automaticamente, viene inserito come riferimento da Workfront nei rapporti.</td> 
     </tr> 
     <tr> 
      <td role="rowheader" id="instructions">Istruzioni</td> 
      <td> Per impostazione predefinita, la formula creata per il campo viene memorizzata qui. È possibile aggiungere testo per fornire informazioni aggiuntive sul campo e sulla formula in esso contenuta. Questo può essere utile in due modi: 
       <ul> 
      <li><p>Come promemoria di cosa è la formula e come funziona. Questa opzione è particolarmente utile se si intende utilizzare il campo personalizzato calcolato in più moduli.</p> </li> 
      <li> <p>Come descrizione comando gli utenti possono vedere quando passano il cursore sul campo. Aggiungere qui il testo che si desidera visualizzare nella descrizione comando.</p> <p>Se non si desidera che la formula venga visualizzata nella descrizione comando, il che potrebbe confonderli, è possibile nasconderla.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Formato</td> 
      <td> <p>Il formato in cui si desidera memorizzare e visualizzare i risultati del campo.</p> <p>Se il campo viene utilizzato nei calcoli matematici, utilizzare sempre un <strong>Numero</strong> o un <strong>Valuta</strong> formato. Quando selezionate Numero (Number) o Valuta (Currency), il sistema tronca automaticamente i numeri che iniziano con 0.</p> 
      <p><b>IMPORTANTE</b>: prima di scegliere un formato, considera il formato corretto per il nuovo campo. Impossibile modificare il campo di formato dopo il salvataggio del modulo personalizzato. La selezione del formato errato potrebbe inoltre influire sui calcoli futuri e sui valori aggregati nei raggruppamenti di report ed elenchi.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. In **Calcolo** , iniziare a creare il calcolo:
   1. Clic **Ingrandisci** per aprire l&#39;Editor di calcolo e generare il calcolo.</p>
Un calcolo inizia in genere con un&#39;espressione, seguita da parentesi contenenti i campi a cui si desidera fare riferimento quando il modulo personalizzato viene allegato a un oggetto.

      Ogni campo deve essere racchiuso tra parentesi graffe. Quando si inizia a digitare il nome di un campo, il sistema formula dei suggerimenti ed è possibile selezionarne uno per inserirlo nel calcolo.

+++ **Espandi per visualizzare la sintassi richiesta nei campi personalizzati calcolati**

      Ogni campo deve utilizzare la sintassi illustrata di seguito, con parentesi graffe intorno al nome di ogni campo. Quando si inizia a digitare il nome di un campo, il sistema formula dei suggerimenti ed è possibile selezionarne uno per inserirlo nel calcolo. Se si immettono dati in un calcolo in modo errato, viene visualizzato un messaggio di avviso. Non è possibile salvare il modulo a meno che non si modifichi il calcolo in modo che contenga campi validi e un&#39;espressione calcolata valida.

      >[!NOTE]
      >
      >Attualmente, il sistema formula suggerimenti solo quando si inizia a digitare il nome di un campo a cui si desidera fare riferimento in un oggetto a cui verrà allegato il modulo personalizzato. I campi dell&#39;oggetto padre non sono consigliati.

      **Racchiudi nomi campi con parentesi graffe**

      * Se si desidera che il calcolo faccia riferimento a un campo incorporato, il nome del campo deve essere racchiuso tra parentesi graffe.

        Ad esempio: `{actualRevenue}`

        I nomi dei campi fanno distinzione tra maiuscole e minuscole e devono essere visualizzati nel calcolo esattamente come appaiono nel sistema Workfront.

        Accedi a [Esplora API di Workfront](https://developer.adobe.com/workfront/api-explorer/) per identificare i nomi dei campi che possono essere utilizzati nei calcoli.

      * Se si desidera che il calcolo faccia riferimento a un campo personalizzato, il nome del campo deve essere racchiuso tra parentesi graffe e preceduto da `DE:` tra parentesi.

        Ad esempio: `{DE:Profit}`

        Il sistema elenca tutti i campi personalizzati tra cui è possibile scegliere quando si digita `DE:`.

         * Se vuoi che il calcolo faccia riferimento a un campo che estrae dati da *principale* oggetto quando il modulo personalizzato viene allegato a un oggetto, è necessario anteporre al nome del campo il tipo di oggetto dell&#39;oggetto padre, tra parentesi graffe.

        Ad esempio, se il modulo personalizzato è configurato per l&#39;utilizzo con le attività e si desidera che il campo calcoli le entrate effettive dell&#39;oggetto padre quando il modulo viene allegato a un&#39;attività, è necessario indicare `Project` come tipo di oggetto del campo:

        `{project}.{actualRevenue}`

        Oppure, se si tratta di un campo personalizzato:

        `{project}.{DE:profit}`

        **Separa elementi con periodi**

        Quando si fa riferimento a un oggetto correlato in un campo personalizzato calcolato, è necessario separare i nomi degli oggetti e gli attributi con i punti.

        In un modulo personalizzato di tipo attività, ad esempio, per visualizzare il nome del proprietario del Portfolio in un campo personalizzato calcolato, digitare quanto segue:

        `{project}.{porfolio}.{owner}`

        Questo determinerebbe quanto segue: Dall’oggetto del modulo personalizzato (un’attività), è possibile accedere all’oggetto successivo correlato all’attività (un progetto). Da qui, puoi accedere al successivo oggetto correlato al progetto (un portfolio), quindi fare riferimento ai campi definiti per l’oggetto portfolio (il proprietario)

        **Sintassi del nome per il riferimento a un campo personalizzato**

        Quando si fa riferimento a un altro campo personalizzato in un campo personalizzato calcolato, è necessario immettere il nome del campo visualizzato nell&#39;interfaccia utente di Workfront.

        Ad esempio, per fare riferimento all’opzione selezionata in un campo personalizzato denominato Executive sponsor, digita quanto segue:

        `{DE:Executive sponsor}`

        >[!NOTE]
        >
        >La sintassi di un campo typeahead è leggermente diversa da quella di altri tipi di campi, in quanto è necessario aggiungere `:name` alla fine.
        >
        >Ad esempio, per fare riferimento all’opzione selezionata in un campo typeahead personalizzato denominato &quot;Executive sponsor&quot;, digita:
        >
        >`{DE:Executive sponsor:name}`


        **Campi personalizzati calcolati nei moduli personalizzati con più oggetti**

        In un modulo personalizzato con più oggetti, i tipi di oggetto selezionati devono essere compatibili con almeno un campo a cui si fa riferimento nei campi personalizzati calcolati del modulo. I campi non compatibili con l’oggetto visualizzeranno N/D nel modulo.

        Per garantire che il campo calcolato visualizzi un risultato corretto per tutti i tipi di oggetto, è necessario utilizzare `$$OBJCODE` per definire un calcolo per ciascun tipo di oggetto.

        >[!INFO]
        >
        >**Esempio:**
        >
        >In un modulo personalizzato configurato per l’utilizzo con progetti, attività e problemi, è possibile utilizzare la formula seguente per visualizzare il tipo di oggetto:
        >
        >`IF($$OBJCODE="PROJ","This is a project",IF($$OBJCODE="TASK","This is a task","This is an issue"))`
        >
        >Su un progetto, il campo mostra &quot;Questo è un progetto&quot;, su un’attività mostra &quot;Questa è un’attività&quot; e su un problema dice &quot;Questo è un problema&quot;.


        >[!INFO]
        >
        >**Esempio:** Sebbene nei progetti non sia presente il campo Assegnato a: Nome, è disponibile un campo Proprietario predefinito che viene automaticamente compilato con il nome della persona che ha creato il progetto, a meno che questa impostazione non venga modificata manualmente.
        >
        >Quindi, nel campo personalizzato In carica, puoi utilizzare `$$OBJCODE` come mostrato di seguito per fare riferimento al campo Proprietario quando il modulo personalizzato è allegato a un progetto e al campo Assegnato a: Nome quando il modulo è allegato a un’attività:
        >
        >`IF($$OBJCODE="PROJ",{owner}.{name},{assignedTo}.{name})`

        Per ulteriori informazioni su variabili come `$$OBJCODE,` vedi [Variabili filtro con caratteri jolly](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

        **Aggiornamenti automatici dei campi personalizzati calcolati**

        I campi personalizzati calcolati su un oggetto vengono ricalcolati automaticamente quando si verificano le seguenti condizioni:

         * Un elemento nell’oggetto cambia, ad esempio un calcolo della sequenza temporale giornaliera.
         * Qualcuno modifica un altro campo a cui fa riferimento un campo personalizzato calcolato sull’oggetto.
         * L&#39;espressione calcolata è vuota e il campo contiene un valore, che imposta il valore su null.

           >[!NOTE]
           >
           ><div>In un modulo personalizzato allegato a un oggetto, le istruzioni di data e ora nei campi personalizzati calcolati vengono calcolate e salvate in base al tempo UTC (Coordinated Universal Time) e non in base alle configurazioni del fuso orario impostate per l’istanza della tua organizzazione e il tuo profilo utente. I calcoli in un modulo personalizzato vengono generati in base ai singoli fusi orari degli utenti.</div>

+++

   1. Fare clic nella casella di testo grande, quindi fare clic su **Espressioni** e **Campi** che sono disponibili per aggiungerli al calcolo.

      È inoltre possibile iniziare a digitare un&#39;espressione o un campo nella casella di testo grande, quindi selezionarlo quando viene visualizzato. Ogni elemento viene visualizzato con una &quot;F&quot; per il campo o una &quot;E&quot; per l’espressione.

      Se si digita una parentesi aperta, la parentesi chiusa viene aggiunta automaticamente.

+++ **Espandi per visualizzare suggerimenti utili**
      >[!TIP]
      >
      >Per ottenere informazioni sui calcoli, eseguire una delle operazioni seguenti:
      > 
      >* Passa il puntatore del mouse su un&#39;espressione nel calcolo per visualizzare una descrizione, un esempio che mostra come può essere utilizzata e un collegamento &quot;Ulteriori informazioni&quot; per ulteriori informazioni nell&#39;articolo [Espressioni dati calcolate](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).
      >  ![](assets/hover-expression-help-text.jpg)
      >* Utilizza la codifica a colori per identificare i componenti aggiunti. Le espressioni vengono visualizzate in blu e i campi in verde.
      >  ![](assets/colors-fields-expressions.jpg)
      >* Individuare gli errori di calcolo, evidenziati in rosa. Puoi passare il cursore del mouse su un errore evidenziato per visualizzarne una breve descrizione della causa.
      >  ![](assets/error-help.png)
      >* Nell&#39;area sottostante il calcolo, visualizzare in anteprima i risultati di un oggetto Workfront esistente.
      ><!--or by providing test values (NOT READY YET; CHANGE THIS SCREENSHOT WHEN IT IS)-->
      >  ![](assets/preview-calc.jpg)
      >* Riferimento alle espressioni in un calcolo lungo utilizzando i numeri di riga visualizzati a sinistra.

+++
   1. Clic **Riduci a icona** al termine della creazione del calcolo per il campo personalizzato calcolato.

   1. (Facoltativo) Utilizza una delle seguenti opzioni per configurare ulteriormente il campo personalizzato calcolato:

      <table style="table-layout:auto">
   <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Aggiungi logica</td> 
      <td>È possibile aggiungere Logica di visualizzazione per determinare se il campo calcolato viene visualizzato, in base ad almeno una scelta effettuata da un utente in un campo a scelta multipla precedente (a discesa, caselle di controllo o pulsanti di scelta) durante la compilazione del modulo. <!-- For more information, see <a href="Need to add link for new article when it's written" class="MCXref xref">Add display logic and skip logic to a custom form</a>.--> <p>Questa opzione è disponibile solo quando almeno una casella di controllo, un pulsante di opzione o un campo a discesa precede il campo personalizzato calcolato nel modulo. </p> <p>La logica di salto non è disponibile per i campi personalizzati calcolati.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aggiorna calcoli precedenti</td> 
      <td>Quando modifichi un campo personalizzato calcolato esistente, puoi selezionare questa opzione per attivare un aggiornamento nel calcolo quando salvi il modulo personalizzato. Questo accade una sola volta quando si salva il modulo personalizzato. L’opzione torna al suo stato disabilitato dopo che l’hai fatto.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Visualizza la formula nelle istruzioni</td> 
      <td>Lascia attiva questa opzione se desideri che gli utenti che compilano il modulo personalizzato visualizzino la formula del campo al passaggio del mouse sul campo. Per ulteriori informazioni, consulta le informazioni su <a href="#instructions" class="MCXref xref">Istruzioni</a> in questa tabella.</td> 
     </tr> 
    </tbody> 
   </table>

1. Per salvare le modifiche, fai clic su **Applica** e passare a un&#39;altra sezione per continuare a creare il modulo.

   oppure

   Clic **Salva e chiudi**.
