---
title: Aggiungere dati calcolati a un modulo personalizzato con il generatore di moduli legacy
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: In un modulo personalizzato è possibile creare un campo personalizzato calcolato che genera calcoli. A questo scopo, è necessario creare un'istruzione che utilizzi espressioni di dati e i nomi dei campi esistenti, che possono essere campi personalizzati, campi di dati personalizzati calcolati e campi Workfront incorporati. Questa istruzione calcola i dati immessi e visualizza il risultato nel nuovo campo personalizzato calcolato.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 9174c4ef-3beb-4d47-9c5c-363f52105a2c
source-git-commit: 6b2a2160b5daaa94374707bad4b026daa13edf06
workflow-type: tm+mt
source-wordcount: '2911'
ht-degree: 0%

---

# Aggiungere dati calcolati a un modulo personalizzato con il generatore di moduli legacy

<!--Audited: 01/2024-->

{{form-designer-default}}

In un modulo personalizzato è possibile aggiungere un campo personalizzato calcolato che utilizza dati esistenti per generare nuovi dati quando il modulo personalizzato viene allegato a un oggetto.

A questo scopo, è necessario creare un&#39;istruzione che utilizzi espressioni di dati e i nomi dei campi esistenti, che possono essere campi personalizzati, campi di dati personalizzati calcolati e campi Adobe Workfront incorporati.

Questa istruzione calcola i dati immessi e visualizza il risultato nel nuovo campo personalizzato calcolato.

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

Per informazioni sulla creazione di moduli personalizzati per l’organizzazione e sul tipo di campi che è possibile associare a essi, consulta [Creare o modificare un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>piano Adobe Workfront</p> </td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td><p>Corrente: Piano</p>
   Oppure
   <p>Nuovo: Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configurazione del livello di accesso</p></td> 
   <td> <p>Accesso amministrativo ai moduli personalizzati</p> </p> </td> 
  </tr>  
 </tbody> 
</table>

*Per conoscere la pianificazione, il tipo di licenza o le configurazioni del livello di accesso disponibili, contattare l&#39;amministratore Workfront. Per ulteriori informazioni sui requisiti di accesso, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Aggiungere un campo calcolato a un modulo personalizzato {#add-a-calculated-field-to-a-custom-form}

Puoi utilizzare sia i campi Workfront incorporati che i campi personalizzati già creati nell’espressione di un campo personalizzato calcolato.

>[!IMPORTANT]
>
>Prima di creare un campo personalizzato calcolato, identificare i campi esistenti che si desidera includere in modo da essere certi che i dati necessari per il calcolo siano presenti in Workfront.

1. Iniziare a creare o modificare un modulo personalizzato, come descritto in [Creare o modificare un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. Il giorno **Aggiungi un campo** , fare clic su **Calcolato**.

   Nell’area di visualizzazione a destra, il campo mostra il valore di riempimento 12345. Questo è un indicatore per ricordarti che il campo è un campo personalizzato calcolato durante la creazione o la modifica del modulo personalizzato. Quando il modulo viene allegato a un oggetto e gli utenti lo compilano, il risultato del calcolo viene visualizzato nel campo e non nel valore 12345.

1. Specifica le seguenti informazioni per il campo calcolato:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Etichetta</td> 
      <td>Digitare un'etichetta per il campo. Questo è ciò che gli utenti visualizzano quando utilizzano il modulo personalizzato. Il campo <b>Nome</b>, che viene compilato automaticamente e corrisponde all’Etichetta, viene referenziato da Workfront nei rapporti. Questo è un campo obbligatorio.</td> 
     </tr>

   <tr> 
   <td role="rowheader">Nome</td> 
   <td>Per impostazione predefinita, il nome di un campo è uguale al nome dell'etichetta. Tuttavia, è possibile modificare il Nome di un campo in modo che sia diverso da Etichetta di un campo. Il campo <b>Nome</b> Nei rapporti di Workfront viene fatto riferimento a. Questo è un campo obbligatorio.</td> 
   </tr>

   <tr> 
     <td role="rowheader" id="instructions">Istruzioni</td> 
      <td> <p>Aggiungi testo per fornire informazioni aggiuntive sul campo e sulla formula in esso contenuta.</p>
      <p>Puoi anche incollare qui la formula utilizzata nel calcolo del campo personalizzato. In questo caso, è consigliabile innanzitutto aggiornare il calcolo del campo personalizzato, quindi copiare l'espressione finale dal campo Calcolo e incollarla nel campo Istruzioni. </p>


   Questo può essere utile nei seguenti modi:
   <ul> 
      <li> <p>Come promemoria di cosa è la formula e come funziona. Questa opzione è particolarmente utile se si intende utilizzare il campo personalizzato calcolato in più moduli.</p> </li> 
       <li> <p>Come descrizione comando gli utenti possono vedere quando passano il cursore sul campo. È possibile aggiungere qui qualsiasi testo che si desidera visualizzare nella descrizione comando.</p> </li> 
       </ul>
       <p>Se non si desidera che gli utenti visualizzino la formula nella descrizione comando, il che potrebbe confonderli, non aggiungerla al campo Istruzioni. Utilizzare invece l'impostazione "Visualizza formula nelle istruzioni" per visualizzare o nascondere la formula, come descritto in questo articolo <a href="#build-the-calculation-for-your-calculated-custom-field">Genera il calcolo per il campo personalizzato calcolato</a> in questo articolo.</p>

   <p>Per informazioni sull'utilizzo dello stesso campo personalizzato calcolato in un nuovo modulo, vedere <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md#using-an-existing-calculated-custom-field-on-a-new-form" class="MCXref xref">Riutilizzare un campo personalizzato calcolato esistente in un modulo personalizzato</a>.</p>

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Formato</td> 
      <td> <p>Il formato in cui si desidera memorizzare e visualizzare i risultati del campo.</p> <p>Se si prevede di utilizzare il campo nei calcoli matematici, utilizzare sempre un <strong>Numero</strong> o un <strong>Valuta</strong> formato. Quando selezionate Numero (Number) o Valuta (Currency), il sistema tronca automaticamente i numeri che iniziano con 0.</p> 
      <p><b>IMPORTANTE</b>: <p>Prima di scegliere un formato, considerare il formato corretto per il nuovo campo. Impossibile modificare il campo di formato dopo il salvataggio del modulo personalizzato. La selezione del formato errato potrebbe inoltre influire sui calcoli futuri e sui valori aggregati nei raggruppamenti di report ed elenchi.</p>
      <p><strong>NOTA:</strong> I campi calcolati con un formato Valuta non devono includere virgolette. (Ad esempio, utilizzare 800.00 e non "800.00"). L’utilizzo delle virgolette può causare conseguenze impreviste a causa di sfumature con la formattazione della lingua per i tipi di valuta.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Continua ad aggiornare le informazioni sui campi personalizzati, come descritto nella sezione [Genera il calcolo per il campo personalizzato calcolato](#build-the-calculation-for-your-calculated-custom-field) in questo articolo.

## Genera il calcolo per il campo personalizzato calcolato {#build-the-calculation-for-your-calculated-custom-field}

1. Inizia a creare il campo personalizzato calcolato, come descritto nella sezione [Aggiungere un campo calcolato a un modulo personalizzato](#add-a-calculated-field-to-a-custom-form) in questo articolo.

1. Clic **Ingrandisci** per aprire **Editor calcoli** e genera i calcoli.

   >[!INFO]
   >
   >**Esempio:** Utilizzando l’esempio riportato nell’introduzione di questo articolo, puoi creare un campo personalizzato calcolato denominato Profitto in un modulo personalizzato per progetti e attività. Questo campo può contenere un calcolo che visualizza la differenza tra Ricavo effettivo e Costo effettivo:
   >
   >`SUB({actualRevenue},{actualCost})`
   >
   >In questo esempio, `SUB` è l’espressione e i campi di riferimento sono `actualRevenue` e `actualCost`.

   Un calcolo inizia in genere con un&#39;espressione, seguita da parentesi contenenti i campi a cui si desidera fare riferimento quando il modulo personalizzato viene allegato a un oggetto. Per informazioni sulle espressioni disponibili, vedi [Panoramica delle espressioni di dati calcolati](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

   Ogni campo deve essere circondato da parentesi graffe, come spiegato nella sezione [Sintassi richiesta nei campi personalizzati calcolati](#syntax-required-in-calculated-custom-fields) in questo articolo. Quando si inizia a digitare il nome di un campo, il sistema formula dei suggerimenti ed è possibile selezionarne uno per inserirlo nel calcolo.

   >[!NOTE]
   >
   >   Non è possibile fare riferimento a campi dei tipi seguenti in un calcolo: 
   >   
   >   * Campo di testo con formattazione
   >   * Testo descrittivo.
   >   
   >   Per informazioni sui tipi di campi personalizzati, vedi [Aggiungere un campo personalizzato a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md).

1. Fare clic nella casella di testo grande della casella Editor calcoli, quindi fare clic su Cerca o Espandi e selezionare un&#39;opzione dalla casella **Espressioni** e **Campi** a destra della casella di testo. Questo le aggiunge al calcolo.

   È inoltre possibile iniziare a digitare un&#39;espressione o un campo nella casella di testo grande, quindi selezionarlo quando viene visualizzato. Ogni elemento viene visualizzato con una &quot;F&quot; per il campo o una &quot;E&quot; per l’espressione.

   Se si digita una parentesi aperta, la parentesi chiusa viene aggiunta automaticamente.

   >[!TIP]
   >
   >Per ottenere informazioni sui calcoli, eseguire una delle operazioni seguenti:
   > 
   >* Passa il puntatore del mouse su un&#39;espressione nel calcolo per visualizzare una descrizione, un esempio che mostra come può essere utilizzata e un collegamento &quot;Ulteriori informazioni&quot; per ulteriori informazioni nell&#39;articolo [Panoramica delle espressioni di dati calcolati](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).
   >  ![](assets/hover-expression-help-text.jpg)
   >* Utilizza la codifica a colori per identificare i componenti aggiunti. Le espressioni vengono visualizzate in blu e i campi in verde.
   >  ![](assets/colors-fields-expressions.jpg)
   >* Individuare gli errori di calcolo, evidenziati in rosa. Puoi passare il cursore del mouse su un errore evidenziato per visualizzarne una breve descrizione della causa.
   >  ![](assets/error-help.png)
   >* In **Anteprima su un oggetto esistente** sotto il calcolo, iniziare a digitare il nome di un oggetto Workfront e selezionarlo quando viene visualizzato nell&#39;elenco. In questo modo è possibile visualizzare un&#39;anteprima dell&#39;aspetto del campo quando il modulo viene allegato all&#39;oggetto.
   ><!--or by providing test values (NOT READY YET; CHANGE THIS SCREENSHOT WHEN IT IS)-->
   >  ![](assets/preview-calc.jpg)
   >* Riferimento alle espressioni in un calcolo lungo utilizzando i numeri di riga visualizzati a sinistra.

1. Clic **Riduci a icona** al termine della creazione del calcolo per il campo personalizzato calcolato.

   >[!NOTE]
   >
   >Nell’area di visualizzazione a destra, il campo mostra il valore di riempimento 12345. Questo è un indicatore per ricordarti che il campo è un campo personalizzato calcolato durante la creazione o la modifica del modulo personalizzato. Quando il modulo viene allegato a un oggetto e gli utenti lo compilano, il risultato del calcolo viene visualizzato nel campo e non nel valore 12345.

1. (Facoltativo) Utilizza una delle seguenti opzioni per configurare ulteriormente il campo personalizzato calcolato:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Aggiungi logica</td> 
      <td>È possibile aggiungere Logica di visualizzazione per determinare se il campo calcolato viene visualizzato, in base ad almeno una scelta effettuata da un utente in un campo a scelta multipla precedente (a discesa, caselle di controllo o pulsanti di scelta) durante la compilazione del modulo. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">Aggiungere logica di visualizzazione e logica di salto a un modulo personalizzato</a>. <p>Questa opzione è disponibile solo quando almeno una casella di controllo, un pulsante di opzione o un campo a discesa precede il campo personalizzato calcolato nel modulo. </p> <p>La logica di salto non è disponibile per i campi personalizzati calcolati.</p> </td> 
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

1. Clic **Fine** quando tutte le modifiche sono state completate nel campo personalizzato calcolato.

   Oppure fai clic su **Applica** per applicare le modifiche apportate al modulo fino ad ora se si desidera continuare ad aggiungere campi personalizzati al modulo.

   Oppure fai clic su **Salva e chiudi** quando tutte le modifiche sono state completate nel modulo personalizzato.
1. Per verificare che il campo personalizzato calcolato funzioni correttamente, allega il modulo personalizzato a un oggetto, quindi controlla il risultato nel campo personalizzato calcolato.

   Per istruzioni su come allegare un modulo personalizzato, vedi [Aggiungere un modulo personalizzato a un oggetto](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

   Se si desidera continuare a creare il modulo personalizzato in altri modi, è possibile passare a uno dei seguenti articoli:

   * [Aggiungere un campo personalizzato a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md)
   * [Posizionare campi e widget personalizzati in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Aggiungere o modificare un widget di risorse in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [Riutilizzare un campo personalizzato calcolato esistente in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [Aggiungere logica di visualizzazione e logica di salto a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [Anteprima e completamento di un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)

## Sintassi richiesta nei campi personalizzati calcolati

Ogni campo utilizzato in un campo calcolato personalizzato deve utilizzare la sintassi illustrata di seguito, con parentesi graffe intorno a ogni nome di campo. Quando si inizia a digitare il nome di un campo, il sistema formula dei suggerimenti ed è possibile selezionarne uno per inserirlo nel calcolo. Se si immettono dati in un calcolo in modo errato, verrà visualizzato un messaggio di avviso. Non è possibile salvare il modulo a meno che non si modifichi il calcolo in modo che contenga campi validi e un&#39;espressione calcolata valida.

>[!NOTE]
>
>Attualmente, il sistema formula suggerimenti solo quando si inizia a digitare il nome di un campo a cui si desidera fare riferimento su un oggetto a cui verrà allegato il modulo personalizzato, non sul padre dell&#39;oggetto.

### Racchiudi nomi campi con parentesi graffe

* Se si desidera che il calcolo faccia riferimento a un campo incorporato, il nome del campo deve essere racchiuso tra parentesi graffe e deve essere formattato come nel database di Workfront. Non è possibile utilizzare il nome dei campi così come vengono visualizzati nell’interfaccia di Workfront.

Ad esempio: `{actualRevenue}`

I nomi dei campi sono sensibili all&#39;uso di maiuscole e minuscole e devono essere visualizzati nel formato Camel case, come nel sistema Workfront.

* Se si desidera che il calcolo faccia riferimento a un campo personalizzato, il nome del campo deve essere racchiuso tra parentesi graffe e preceduto da `DE:` tra parentesi. I campi personalizzati fanno distinzione tra maiuscole e minuscole e devono essere formattati come appaiono nell’interfaccia di Workfront.

Ad esempio: `{DE:Profit}`

Il sistema elenca tutti i campi personalizzati tra cui è possibile scegliere quando si digita `DE:`.

* Se si desidera che il calcolo faccia riferimento a un campo che estrae dati dall&#39;oggetto padre quando il modulo personalizzato viene allegato a un oggetto, è necessario anteporre al nome del campo il tipo di oggetto dell&#39;oggetto padre, anche tra parentesi graffe.

  Ad esempio, se il modulo personalizzato è configurato per l&#39;utilizzo con le attività e si desidera che il campo calcoli le entrate effettive dell&#39;oggetto padre quando il modulo viene allegato a un&#39;attività, è necessario indicare `project` come tipo di oggetto del campo:

  `{project}.{actualRevenue}`

  Oppure, se si tratta di un campo personalizzato:

  `{project}.{DE:profit}`

  Se non si è certi del tipo di oggetto dell&#39;oggetto padre perché il modulo personalizzato è configurato per più tipi di oggetto, è possibile utilizzare la variabile filtro con caratteri jolly `$$OBJCODE` per consentire il funzionamento del calcolo per ciascuno dei tipi possibili. Per ulteriori informazioni, consulta [Campi personalizzati calcolati nei moduli personalizzati con più oggetti](#calculated-custom-fields-in-multi-object-custom-forms) in questo articolo.

### Separa elementi con periodi

Quando si fa riferimento a un oggetto correlato in un campo personalizzato calcolato, è necessario separare i nomi degli oggetti e gli attributi con i punti.

In un modulo personalizzato di tipo attività, ad esempio, per visualizzare il nome del proprietario del Portfolio in un campo personalizzato calcolato, digitare quanto segue:

`{project}.{porfolio}.{owner}`

Il sistema recupera le informazioni nei seguenti passaggi (nell&#39;ordine indicato):

1. Dall’oggetto del modulo personalizzato (un’attività), quindi
1. Accedere all&#39;elemento padre dell&#39;attività o a un altro oggetto correlato (progetto), quindi
1. Accedere all&#39;oggetto padre o a un altro oggetto correlato del progetto (un portfolio), quindi
1. Accedere al successivo oggetto correlato al portfolio (il proprietario del portfolio).

### Sintassi del nome per il riferimento a un campo personalizzato

Quando si fa riferimento a un altro campo personalizzato in un campo personalizzato calcolato, è necessario immettere il nome del campo visualizzato nell&#39;interfaccia di Workfront.

Ad esempio, per fare riferimento all’opzione selezionata in un campo personalizzato denominato Executive sponsor, digita quanto segue:

`{DE:Executive sponsor}`

>[!NOTE]
>
>La sintassi di un campo automatico è diversa da quella di altri tipi di campi, in quanto è necessario aggiungere `:name` alla fine.
>
>Ad esempio, per fare riferimento all’opzione selezionata in un campo typeahead personalizzato denominato &quot;Executive sponsor&quot;, digita:
>
>`{DE:Executive sponsor:name}`

## Campi personalizzati calcolati nei moduli personalizzati con più oggetti {#calculated-custom-fields-in-multi-object-custom-forms}

In un modulo personalizzato con più oggetti, i tipi di oggetto selezionati devono essere compatibili con tutti i campi a cui si fa riferimento nei campi personalizzati calcolati del modulo. In caso di incompatibilità, un messaggio ti avvisa di apportare le modifiche necessarie.

>[!INFO]
>
>**Esempio:**
>
>In un modulo personalizzato configurato per l&#39;utilizzo con il tipo di oggetto Task, viene creato un campo personalizzato calcolato denominato In carica. Puoi configurarlo per fare riferimento al campo incorporato in modo che possa visualizzare il nome dell’assegnatario principale responsabile ogni volta che il modulo viene allegato a un’attività:
>
>`{assignedTo}.{name}`
>
>Successivamente, si aggiunge il tipo di oggetto Project al modulo personalizzato. Un messaggio di avviso indica che il tipo di oggetto Project non è compatibile con il campo personalizzato calcolato.

In questo caso, puoi effettuare una delle seguenti operazioni:

* Rimuovere uno dei due elementi incompatibili dal modulo personalizzato, ovvero il tipo di oggetto o il campo personalizzato calcolato di riferimento.
* Mantieni entrambi gli elementi e utilizza la variabile di filtro con caratteri jolly `$$OBJCODE` come condizione in un&#39;espressione IF per creare due versioni diverse del campo In carica. Questo consente al campo di funzionare correttamente, indipendentemente dal tipo di oggetto a cui è associato il modulo.

>[!INFO]
>
>**Esempio:** Sebbene nei progetti non sia presente il campo Assegnato a: Nome, è disponibile un campo Proprietario predefinito che viene automaticamente compilato con il nome della persona che ha creato il progetto, a meno che questa impostazione non venga modificata manualmente.
>
>Quindi, nel campo personalizzato In carica, puoi utilizzare `$$OBJCODE` come mostrato di seguito per fare riferimento al campo Proprietario quando il modulo personalizzato è allegato a un progetto e al campo Assegnato a: Nome quando il modulo è allegato a un’attività:
>
>`IF($$OBJCODE="PROJ",{owner}.{name},{assignedTo}.{name})`

Per ulteriori informazioni su variabili come `$$OBJCODE,` vedi [Panoramica delle variabili filtro con caratteri jolly](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

## Aggiornamenti automatici dei campi personalizzati calcolati

I campi personalizzati calcolati su un oggetto vengono ricalcolati automaticamente quando si verificano le seguenti condizioni:

* Un elemento nell’oggetto cambia, ad esempio un calcolo della sequenza temporale giornaliera.
* Qualcuno modifica un altro campo a cui fa riferimento un campo personalizzato calcolato sull’oggetto.
* L&#39;espressione calcolata è vuota e il campo contiene un valore, che imposta il valore su null.

  >[!NOTE]
  >
  >In un modulo personalizzato allegato a un oggetto, le istruzioni di data e ora nei campi personalizzati calcolati vengono calcolate e salvate in base al Coordinated Universal Time (UTC), non in base alle configurazioni del fuso orario impostate per l’istanza della tua organizzazione e il tuo profilo utente. Tuttavia, i calcoli in un modulo personalizzato vengono visualizzati in base al singolo fuso orario di ciascun utente.
