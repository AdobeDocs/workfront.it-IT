---
title: Aggiunta di campi calcolati con la finestra di progettazione del modulo
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: È possibile aggiungere un campo personalizzato calcolato che utilizza dati esistenti per generare nuovi dati quando il modulo personalizzato viene associato a un oggetto.
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 6e06e7892542c7dd96b6bf8b857583333efc883d
workflow-type: tm+mt
source-wordcount: '2317'
ht-degree: 0%

---


# Aggiunta di campi calcolati con la finestra di progettazione del modulo

È possibile aggiungere un campo personalizzato calcolato che utilizza dati esistenti per generare nuovi dati quando il modulo personalizzato viene associato a un oggetto.

Un campo personalizzato calcolato può contenere:

* Un semplice riferimento a un singolo campo incorporato.

   >[!INFO]
   >
   > **Esempio:** Per calcolare i ricavi generati dai progetti e dalle attività, è possibile creare un campo personalizzato calcolato contenente il campo incorporato Entrate effettive. Quando un utente allega il modulo personalizzato a un progetto o a un&#39;attività, nel campo vengono visualizzate le entrate relative al progetto o all&#39;attività.

* Espressione che fa riferimento a uno o più campi. Possono essere campi personalizzati, altri campi personalizzati calcolati e campi incorporati.

   >[!INFO]
   >
   >**Esempio:** Per calcolare il profitto generato da progetti e attività, è possibile creare un campo personalizzato calcolato denominato Profitto contenente un&#39;espressione matematica che sottrae il costo dai ricavi.
   >
   >A questo scopo, puoi utilizzare l’espressione matematica SUB (sottrazione) con i campi Workfront incorporati Costo effettivo e Ricavo effettivo.
   >
   >Nei passaggi seguenti, puoi vedere come eseguire questo esempio.


## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>piano Adobe Workfront*</p> </td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td>Piano</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Accesso amministrativo ai moduli personalizzati</p> <p>Per informazioni su come gli amministratori di Workfront concedono questo accesso, consulta <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Consentire agli utenti l'accesso amministrativo a determinate aree</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o configurazioni del livello di accesso si dispone, contattare l&#39;amministratore Workfront.

## Riutilizzare un campo personalizzato calcolato esistente in un modulo personalizzato

È possibile utilizzare lo stesso campo personalizzato calcolato nei moduli personalizzati che appartengono a oggetti diversi. Ad esempio, è possibile utilizzare il campo calcolato Profitto creato per il modulo personalizzato del progetto in un modulo personalizzato dell’attività.

Quando si utilizza un campo personalizzato calcolato esistente, il calcolo non viene trasferito nel nuovo modulo. È necessario aggiungere nuovamente il calcolo, sullo stesso campo, nel nuovo modulo personalizzato.

È inoltre possibile utilizzare un calcolo diverso per lo stesso campo nel nuovo modulo. Mantenere lo stesso nome per il campo personalizzato calcolato assicura coerenza e coerenza nella convenzione di denominazione.

>[!IMPORTANT]
>
>Le modifiche nelle espressioni calcolate possono rendere obsoleto il valore del campo sugli oggetti. Per visualizzare sempre il calcolo aggiornato in questi campi, effettuare una delle seguenti operazioni:
>
>* Dopo aver salvato un oggetto in cui sono stati modificati i dati in un modulo personalizzato allegato, fare clic sull’icona Altro ![](assets/more-icon.png) nella pagina principale dell’oggetto, quindi Ricalcola espressioni personalizzate.
>* Selezionare l’opzione Ricalcola espressioni personalizzate quando si modificano gli oggetti in blocco.
>* Selezionare l’opzione Aggiorna calcoli precedenti durante la modifica di un campo personalizzato calcolato in un modulo personalizzato.


Per riutilizzare un campo personalizzato calcolato esistente:

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Fai clic su **Forms personalizzato** nel pannello a sinistra.

   <!-- >[!TIP]
    >
    >In the view that appears, you can review all custom forms and custom fields that have been created for your organization. You can also see who created each form and the fields that are associated with it. -->

1. Fai clic su **Nuovo modulo personalizzato.**
1. Selezionare i tipi di oggetto a cui si desidera associare il modulo personalizzato, quindi fare clic su **Continua**.

1. In alto a sinistra nella schermata, fai clic su **Libreria campi**.

   ![](assets/field-library.png)

1. Utilizza la casella di ricerca o espandi la **Calcolato** per individuare il campo calcolato desiderato, trascinare il campo in cui si desidera visualizzarlo nel modulo personalizzato.

1. (Facoltativo) Ripeti il passaggio precedente per aggiungere altri campi.

   >[!NOTE]
   >
   >È possibile aggiungere fino a 500 campi e widget in un singolo modulo personalizzato. Tuttavia, è possibile che si verifichi un peggioramento delle prestazioni in presenza di più di 100 moduli, a seconda della complessità del modulo.
   >
   >
   >Esempi di moduli complessi includono moduli con parametri a cascata, campi di dati personalizzati calcolati e opzioni con più valori in un singolo campo.

1. Per salvare le modifiche, fai clic su **Applica** e passare a un&#39;altra sezione per continuare a creare il modulo.

   oppure

   Fai clic su **Salva e chiudi**.

## Aggiungi un nuovo campo calcolato

>[!IMPORTANT]
>
>Prima di creare un nuovo campo personalizzato calcolato, identificare i campi esistenti da includere in modo da essere sicuri che i dati necessari per il calcolo siano presenti in Workfront.

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Fai clic su **Forms personalizzato** nel pannello a sinistra.

   <!-- >[!TIP]
    >
    >In the view that appears, you can review all custom forms and custom fields that have been created for your organization. You can also see who created each form and the fields that are associated with it. -->

1. Fai clic su **Nuovo modulo personalizzato.**
1. Selezionare i tipi di oggetto a cui si desidera associare il modulo personalizzato, quindi fare clic su **Continua**.

1. Sul lato sinistro dello schermo, trova **Calcolato** e trascinarlo in una sezione dell&#39;area di lavoro.

   ![](assets/drag-field-to-section.png)

1. Sul lato destro della schermata, configura le opzioni disponibili per il tipo di campo personalizzato che si sta aggiungendo:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Etichetta</td> 
      <td>Digita un’etichetta per il campo. Questo è ciò che verrà visualizzato dagli utenti quando utilizzano il modulo personalizzato. Il campo <b>Nome</b>, a cui viene fatto automaticamente riferimento in nei rapporti di .</td> 
     </tr> 
     <tr> 
      <td role="rowheader" id="instructions">Istruzioni</td> 
      <td> Per impostazione predefinita, la formula creata per il campo è memorizzata qui. È possibile aggiungere del testo per fornire ulteriori informazioni sul campo e sulla formula in esso contenuta. Questo può essere utile in due modi: 
       <ul> 
      <li><p>Come promemoria di ciò che è la formula e come funziona. Questa funzione è particolarmente utile se si prevede di utilizzare questo campo personalizzato calcolato su più moduli.</p> </li> 
      <li> <p>Come descrizione comando, gli utenti possono vedere quando passano il puntatore del mouse sul campo. In questa sezione viene aggiunto il testo da visualizzare nella descrizione comandi.</p> <p>Se non si desidera che visualizzino la formula nella descrizione comando, che potrebbe confondere per loro, è possibile nasconderla.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Formato</td> 
      <td> <p>Formato in cui memorizzare e visualizzare i risultati del campo.</p> <p>Se il campo viene utilizzato nei calcoli matematici, utilizza sempre un <strong>Numero</strong> o <strong>Valuta</strong> formato. Quando si seleziona Numero o Valuta, i numeri che iniziano con 0 vengono troncati automaticamente dal sistema.</p> 
      <p><b>IMPORTANTE</b>: Prima di scegliere un formato, considerare il formato corretto per il nuovo campo. Impossibile modificare il campo formato dopo il salvataggio del modulo personalizzato. La selezione del formato errato potrebbe inoltre avere un impatto sui calcoli futuri e sui valori aggregati nei raggruppamenti per report ed elenchi.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. In **Calcolo** inizia a costruire il calcolo:
   1. Fai clic su **Massimizza** per aprire l&#39;Editor calcoli e generare il calcolo.</p>
Un calcolo inizia in genere con un’espressione, seguita da parentesi contenenti i campi a cui si desidera fare riferimento quando il modulo personalizzato viene associato a un oggetto.

      Ogni campo deve essere circondato da parentesi graffe. Quando inizi a digitare il nome di un campo, il sistema formula suggerimenti e puoi selezionarne uno per inserirlo nel calcolo.

+++ **Espandi per visualizzare la sintassi richiesta nei campi personalizzati calcolati**

      Ogni campo deve utilizzare la sintassi illustrata di seguito, con parentesi graffe intorno al nome di ciascun campo. Quando inizi a digitare il nome di un campo, il sistema formula suggerimenti e puoi selezionarne uno per inserirlo nel calcolo. Se i dati immessi in un calcolo non sono corretti, viene visualizzato un messaggio di avviso. Non è possibile salvare il modulo a meno che non si modifichi il calcolo per contenere campi validi e un&#39;espressione calcolata valida.

      >[!NOTE]
      >
      >Attualmente, il sistema formula suggerimenti solo quando si inizia a digitare il nome di un campo a cui si desidera fare riferimento in un oggetto a cui verrà allegato il modulo personalizzato. I campi dell’oggetto principale non sono consigliati.

      **Nomi dei campi surround con parentesi graffe**

      * Se si desidera che il calcolo faccia riferimento a un campo incorporato, il nome del campo deve essere racchiuso tra parentesi graffe.

         Ad esempio: `{actualRevenue}`

         I nomi dei campi sono sensibili all’uso di maiuscole e minuscole e devono essere visualizzati nel calcolo esattamente come sono visualizzati nel sistema Workfront.

         Passa a [Esplora API di Workfront](https://developer.adobe.com/workfront/api-explorer/) per identificare i nomi dei campi che possono essere utilizzati nei calcoli.

      * Se si desidera che il calcolo faccia riferimento a un campo personalizzato, il nome del campo deve essere racchiuso tra parentesi graffe e preceduto da `DE:` tra parentesi.

         Ad esempio: `{DE:Profit}`

         Il sistema elenca tutti i campi personalizzati tra cui è possibile scegliere quando si digita `DE:`.

         * Se si desidera che il calcolo faccia riferimento a un campo che estrarrà i dati dal *parent* quando il modulo personalizzato è associato a un oggetto, è necessario precedere il nome del campo con il tipo di oggetto dell’oggetto principale, anche tra parentesi graffe.

         Ad esempio, se il modulo personalizzato è configurato in modo da funzionare con le attività e si desidera che il campo calcoli le entrate effettive dell’oggetto principale quando il modulo è associato a un’attività, è necessario indicare `Project` come tipo di oggetto del campo:

         `{project}.{actualRevenue}`

         Oppure, se si tratta di un campo personalizzato:

         `{project}.{DE:profit}`

         **Separa gli elementi con i periodi**

         Quando si fa riferimento a un oggetto correlato in un campo personalizzato calcolato, è necessario separare i nomi e gli attributi degli oggetti con i punti.

         Ad esempio, in un modulo personalizzato di tipo task, per visualizzare il nome del proprietario del Portfolio in un campo personalizzato calcolato, digitare quanto segue:

         `{project}.{porfolio}.{owner}`

         Questo determinerebbe quanto segue: Dall’oggetto del modulo personalizzato (un’attività) è possibile accedere all’oggetto successivo relativo all’attività (un progetto). Da lì è possibile accedere all’oggetto correlato successivo al progetto (un portfolio), quindi fare riferimento ai campi definiti per l’oggetto portfolio (il proprietario)

         **Sintassi del nome per il riferimento a un campo personalizzato**

         Quando si fa riferimento a un altro campo personalizzato in un campo personalizzato calcolato, è necessario immettere il nome del campo così come viene visualizzato nell’interfaccia utente di Workfront.

         Ad esempio, per fare riferimento all&#39;opzione selezionata in un campo personalizzato denominato sponsor esecutivo, digitare quanto segue:

         `{DE:Executive sponsor}`

         >[!NOTE]
         >
         >La sintassi di un campo typeahead è leggermente diversa da quella di altri tipi di campi, in quanto è necessario aggiungere `:name` alla fine.
         >
         >Ad esempio, per fare riferimento all&#39;opzione selezionata in un campo personalizzato typeahead denominato &quot;Executive sponsor&quot;, digitare:
         >
         >`{DE:Executive sponsor:name}`


         **Campi personalizzati calcolati nei moduli personalizzati con più oggetti**

         In un modulo personalizzato con più oggetti, i tipi di oggetto selezionati devono essere compatibili con almeno un campo a cui si fa riferimento nei campi personalizzati calcolati del modulo. I campi non compatibili con l’oggetto verranno visualizzati N/D sul modulo.

         Per garantire che il campo calcolato presenti un risultato corretto per tutti i tipi di oggetto, è necessario utilizzare `$$OBJCODE` per definire un calcolo per ciascun tipo di oggetto.

         >[!INFO]
         >
         >**Esempio:**
         >
         >In un modulo personalizzato configurato per lavorare con progetti, attività e problemi, è possibile utilizzare la formula seguente per visualizzare il tipo di oggetto:
         >
         >`IF($$OBJCODE="PROJ","This is a project",IF($$OBJCODE="TASK","This is a task","This is an issue"))`
         >
         >Su un progetto il campo mostrerà &quot;Questo è un progetto&quot;, su un&#39;attività mostrerà &quot;Questo è un compito&quot;, e su un problema dirà &quot;Questo è un problema&quot;.


         >[!INFO]
         >
         >**Esempio:** Anche se non è stato assegnato a: Campo Nome nei progetti, è presente un campo Proprietario integrato (che si riempie automaticamente con il nome della persona che ha creato il progetto, a meno che qualcuno non lo modifichi manualmente).
         >
         >Quindi, nel campo personalizzato In Charge, puoi utilizzare `$$OBJCODE` come mostrato di seguito, fare riferimento al campo Proprietario quando il modulo personalizzato è associato a un progetto e al campo Assegnato a: Campo Nome quando il modulo è associato a un’attività:
         >
         >`IF($$OBJCODE="PROJ",{owner}.{name},{assignedTo}.{name})`

         Per ulteriori informazioni su variabili come `$$OBJCODE,` vedere [Variabili filtro caratteri jolly](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

         **Aggiornamenti automatici dei campi personalizzati calcolati**

         I campi personalizzati calcolati su un oggetto vengono ricalcolati automaticamente quando si verificano le seguenti situazioni:

         * Viene modificato un elemento dell’oggetto, ad esempio un calcolo giornaliero della timeline.
         * Un utente modifica un altro campo a cui fa riferimento un campo personalizzato calcolato sull’oggetto.
         * L&#39;espressione calcolata è vuota e il campo contiene un valore, che imposta il valore su null.

            >[!NOTE]
            >
            ><div>In un modulo personalizzato allegato a un oggetto, le istruzioni data e ora nei campi personalizzati calcolati vengono calcolate e salvate dall’Ora universale coordinata (UTC), non dalle configurazioni del fuso orario impostate per l’istanza dell’organizzazione e il profilo utente. I calcoli in un modulo personalizzato vengono generati in base ai singoli fusi orari di ciascun utente.</div>

+++
   1. Fare clic nella casella di testo di grandi dimensioni, quindi fare clic su **Espressioni** e **Campi** disponibili per aggiungerli al calcolo.

      È inoltre possibile iniziare a digitare un’espressione o un campo nella casella di testo di grandi dimensioni, quindi selezionarlo quando viene visualizzato. Ogni elemento viene visualizzato con un valore &quot;F&quot; per il campo o un valore &quot;E&quot; per l’espressione.

      Se si digita una parentesi di apertura, la parentesi di chiusura viene aggiunta automaticamente.

+++ **Espandi per visualizzare suggerimenti utili**
      >[!TIP]
      >
      >Per ottenere assistenza nel calcolo, è possibile effettuare una delle seguenti operazioni:
      > 
      >* Passa il puntatore del mouse su un&#39;espressione nel calcolo per visualizzare una descrizione, un esempio che illustra come utilizzarla e un collegamento &quot;Ulteriori informazioni&quot; per ulteriori informazioni nell&#39;articolo [Espressioni dati calcolate](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).
         >  ![](assets/hover-expression-help-text.jpg)
      >* Utilizza la codifica colore per identificare i componenti aggiunti. Le espressioni vengono visualizzate in blu e i campi in verde.
         >  ![](assets/colors-fields-expressions.jpg)
      >* Trova errori di calcolo, evidenziati in rosa, mentre vai. Puoi passare il cursore su un errore evidenziato per visualizzare una breve descrizione della sua causa.
         >  ![](assets/error-help.png)
      >* Nell’area sotto il calcolo, visualizzare in anteprima i risultati su un oggetto Workfront esistente.
         ><!--or by providing test values (NOT READY YET; CHANGE THIS SCREENSHOT WHEN IT IS)-->

         >  ![](assets/preview-calc.jpg)
      >* Fai riferimento alle espressioni in un calcolo lungo utilizzando i numeri di riga visualizzati a sinistra.


+++
   1. Fai clic su **Riduci a icona** al termine della creazione del calcolo per il campo personalizzato calcolato.

   1. (Facoltativo) Utilizza una delle seguenti opzioni per configurare ulteriormente il campo personalizzato calcolato:

      <table style="table-layout:auto">
   <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Aggiungi logica</td> 
      <td>È possibile aggiungere la logica di visualizzazione per determinare se il campo calcolato viene visualizzato, in base ad almeno una scelta effettuata da un utente in un campo di scelta multipla precedente (a discesa, caselle di selezione o pulsanti di scelta) durante la compilazione del modulo. <!-- For more information, see <a href="Need to add link for new article when it's written" class="MCXref xref">Add display logic and skip logic to a custom form</a>.--> <p>Questa opzione è disponibile solo quando almeno una casella di controllo, un pulsante di scelta o un campo a discesa precede il campo personalizzato calcolato sul modulo. </p> <p>Ignora logica non disponibile per i campi personalizzati calcolati.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aggiorna calcoli precedenti</td> 
      <td>Quando si modifica un campo personalizzato calcolato esistente, è possibile selezionare questa opzione per attivare un aggiornamento nel calcolo quando si salva il modulo personalizzato. Questo accade solo una volta quando si salva il modulo personalizzato. L’opzione torna al suo stato disabilitato dopo averlo fatto.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Visualizza la formula nelle istruzioni</td> 
      <td>Lasciare attivata questa opzione se si desidera che gli utenti che compilano il modulo personalizzato visualizzino la formula del campo quando passano il puntatore del mouse sul campo. Per ulteriori informazioni, consulta <a href="#instructions" class="MCXref xref">Istruzioni</a> prima in questa tabella.</td> 
     </tr> 
    </tbody> 
   </table>

1. Per salvare le modifiche, fai clic su **Applica** e passare a un&#39;altra sezione per continuare a creare il modulo.

   oppure

   Fai clic su **Salva e chiudi**.


