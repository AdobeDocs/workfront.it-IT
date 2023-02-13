---
title: Aggiungere dati calcolati a un modulo personalizzato
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: In un modulo personalizzato è possibile creare un campo personalizzato calcolato che genera calcoli. A questo scopo, è necessario creare un’istruzione che utilizzi espressioni dati e nomi di campi esistenti, che possono essere campi personalizzati, campi di dati personalizzati calcolati e campi Workfront incorporati. Questa istruzione calcola i dati immessi e visualizza il risultato nel nuovo campo personalizzato calcolato.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 9174c4ef-3beb-4d47-9c5c-363f52105a2c
source-git-commit: e24a0408049e7eb2e7cb97833e7f41ea66e8131b
workflow-type: tm+mt
source-wordcount: '2563'
ht-degree: 0%

---

# Aggiungere dati calcolati a un modulo personalizzato

In un modulo personalizzato è possibile aggiungere un campo personalizzato calcolato che utilizza dati esistenti per generare nuovi dati quando il modulo personalizzato è associato a un oggetto.

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

Per informazioni sulla creazione di moduli personalizzati per la propria organizzazione e sul tipo di campi che è possibile associare, vedere [Creare o modificare un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

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
   <td> <p>Accesso amministrativo ai moduli personalizzati</p> <p>Per informazioni su come gli amministratori di Workfront concedono questo accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Consentire agli utenti l'accesso amministrativo a determinate aree</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o configurazioni del livello di accesso si dispone, contattare l&#39;amministratore Workfront.

## Aggiungere un campo calcolato a un modulo personalizzato {#add-a-calculated-field-to-a-custom-form}

Puoi utilizzare sia campi Workfront incorporati che campi personalizzati già creati.

>[!IMPORTANT]
>
>Prima di creare un nuovo campo personalizzato calcolato, identificare i campi esistenti da includere in modo da essere sicuri che i dati necessari per il calcolo siano presenti in Workfront.

1. Iniziare a creare o modificare un modulo personalizzato, come descritto in [Creare o modificare un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. Sulla **Aggiungi un campo** scheda , fai clic su **Calcolato**.

   Nell’area di visualizzazione a destra viene visualizzato il campo *12345*. Questo è solo un indicatore per ricordare che il campo è un campo personalizzato calcolato durante la creazione o la modifica del modulo personalizzato. Quando il modulo è associato a un oggetto e gli utenti lo stanno compilando, visualizzano il risultato del calcolo nel campo , mai il *12345* indicatore.

1. Specifica le seguenti informazioni per il campo calcolato:

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
        <li> <p>Come promemoria di ciò che è la formula e come funziona. Questa funzione è particolarmente utile se si prevede di utilizzare questo campo personalizzato calcolato su più moduli.</p> </li> 
        <li> <p>Come descrizione comando, gli utenti possono vedere quando passano il puntatore del mouse sul campo. In questa sezione viene aggiunto il testo da visualizzare nella descrizione comandi.</p> <p>Se non si desidera che visualizzino la formula nella descrizione comando, che potrebbe confondere per loro, è possibile nasconderla. Per istruzioni, vedere la riga della tabella "Visualizza formula nelle istruzioni" nella sezione <a href="#build-the-calculation-for-your-calculated-custom-field" class="MCXref xref">Genera il calcolo per il campo personalizzato calcolato</a> in questo articolo.</p> </li> 
       </ul> <p>Per informazioni sull’utilizzo dello stesso campo personalizzato calcolato in un nuovo modulo, consultare <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md#using-an-existing-calculated-custom-field-on-a-new-form" class="MCXref xref">Riutilizzare un campo personalizzato calcolato esistente in un modulo personalizzato</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Formato</td> 
      <td> <p>Il formato in cui si desidera memorizzare e visualizzare i risultati del campo.</p> <p>Se il campo viene utilizzato nei calcoli matematici, utilizza sempre un <strong>Numero</strong> o <strong>Valuta</strong> formato. Quando si seleziona Numero o Valuta, i numeri che iniziano con 0 vengono troncati automaticamente dal sistema.</p> 
      <p><b>IMPORTANTE</b>: Prima di scegliere un formato, considerare il formato corretto per il nuovo campo. Impossibile modificare il campo formato dopo il salvataggio del modulo personalizzato. La selezione del formato errato potrebbe inoltre avere un impatto sui calcoli futuri e sui valori aggregati nei raggruppamenti per report ed elenchi.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Continua su [Genera il calcolo per il campo personalizzato calcolato](#build-the-calculation-for-your-calculated-custom-field) in questo articolo.

## Genera il calcolo per il campo personalizzato calcolato {#build-the-calculation-for-your-calculated-custom-field}

1. Inizia a creare il campo personalizzato calcolato, come spiegato nella sezione [Aggiungere un campo calcolato a un modulo personalizzato](#add-a-calculated-field-to-a-custom-form) in questo articolo.

1. Fai clic su **Massimizza** per aprire **Editor di calcolo** e crea il calcolo.

   >[!INFO]
   >
   >**Esempio:** Utilizzando l’esempio nell’introduzione a questo articolo, è possibile creare un campo personalizzato calcolato denominato Profitto in un modulo personalizzato per progetti e attività. Questo campo può contenere un calcolo che visualizza la differenza tra Ricavo effettivo e Costo effettivo:
   >
   >`SUB({actualRevenue},{actualCost})`
   >
   >In questo esempio, `SUB` è l&#39;espressione e i campi a cui si fa riferimento sono `actualRevenue` e `actualCost`.

   Un calcolo inizia in genere con un’espressione, seguita da parentesi contenenti i campi a cui si desidera fare riferimento quando il modulo personalizzato viene associato a un oggetto. Per informazioni sulle espressioni disponibili, consulta [Espressioni dati calcolate](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

   Ogni campo deve essere circondato da parentesi graffe, come spiegato nella sezione [Sintassi necessaria nei campi personalizzati calcolati](#syntax-required-in-calculated-custom-fields) in questo articolo. Quando inizi a digitare il nome di un campo, il sistema formula suggerimenti e puoi selezionarne uno per inserirlo nel calcolo.

   È possibile fare riferimento a qualsiasi tipo di campo personalizzato in un calcolo, ad eccezione di due: Campo di testo con tipo di formattazione e Testo descrittivo. Per informazioni sui tipi di campi personalizzati, consulta [Aggiungere un campo personalizzato a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md)

1. Fare clic nella casella di testo di grandi dimensioni, quindi fare clic su **Espressioni** e **Campi** disponibili per aggiungerli al calcolo.

   È inoltre possibile iniziare a digitare un’espressione o un campo nella casella di testo di grandi dimensioni, quindi selezionarlo quando viene visualizzato. Ogni elemento viene visualizzato con un valore &quot;F&quot; per il campo o un valore &quot;E&quot; per l’espressione.

   Se si digita una parentesi di apertura, la parentesi di chiusura viene aggiunta automaticamente.

   >[!TIP]
   >
   >Per ottenere assistenza nel calcolo, è possibile effettuare una delle seguenti operazioni:
   > 
   >* Passa il puntatore del mouse su un&#39;espressione nel calcolo per visualizzare una descrizione, un esempio che illustra come utilizzarla e un collegamento &quot;Ulteriori informazioni&quot; per ulteriori informazioni nell&#39;articolo [Espressioni dati calcolate](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).
      >  ![](assets/hover-expression-help-text.jpg)
   >* Utilizza la codifica colore per identificare i componenti aggiunti. Le espressioni vengono visualizzate in blu e i campi in verde.
      >  ![](assets/colors-fields-expressions.jpg)
   >* Trova errori di calcolo, evidenziati in rosa, mentre vai. Puoi passare il cursore su un errore evidenziato per visualizzare una breve descrizione della sua causa.
      >  ![](assets/error-help.png)
   >* Nell’area sotto il calcolo, visualizzare in anteprima i risultati su un oggetto Workfront esistente.

   ><!--or by providing test values (NOT READY YET; CHANGE THIS SCREENSHOT WHEN IT IS)-->
   >  ![](assets/preview-calc.jpg)
   >* Fai riferimento alle espressioni in un calcolo lungo utilizzando i numeri di riga visualizzati a sinistra.


1. Fai clic su **Riduci a icona** al termine della creazione del calcolo per il campo personalizzato calcolato.

   >[!NOTE]
   >
   >Nell’area di visualizzazione a destra viene visualizzato il campo *12345.* Questo è solo un indicatore per ricordare che il campo è un campo personalizzato calcolato durante la creazione o la modifica del modulo personalizzato. Quando il modulo è associato a un oggetto e gli utenti lo stanno compilando, visualizzano il risultato del calcolo nel campo , mai il *12345* indicatore.

1. (Facoltativo) Utilizza una delle seguenti opzioni per configurare ulteriormente il campo personalizzato calcolato:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Aggiungi logica</td> 
      <td>È possibile aggiungere la logica di visualizzazione per determinare se il campo calcolato viene visualizzato, in base ad almeno una scelta effettuata da un utente in un campo di scelta multipla precedente (a discesa, caselle di selezione o pulsanti di scelta) durante la compilazione del modulo. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">Aggiungere logica di visualizzazione e ignorare la logica in un modulo personalizzato</a>. <p>Questa opzione è disponibile solo quando almeno una casella di controllo, un pulsante di scelta o un campo a discesa precede il campo personalizzato calcolato sul modulo. </p> <p>Ignora logica non disponibile per i campi personalizzati calcolati.</p> </td> 
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

1. Fai clic su **Fine** quando tutte le modifiche sono completate nel campo personalizzato calcolato.

   Oppure, fai clic su **Applica** per applicare le modifiche apportate al modulo, se si desidera continuare ad aggiungere campi personalizzati al modulo.

   Oppure, fai clic su **Salva e chiudi** quando tutte le modifiche sono completate nel modulo personalizzato.
1. Per verificare che il campo personalizzato calcolato funzioni correttamente, allegare il modulo personalizzato a un oggetto, quindi esaminare il risultato nel campo personalizzato calcolato.

   Per istruzioni su come allegare un modulo personalizzato, vedere [Aggiungere un modulo personalizzato a un oggetto](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

   Se si desidera continuare a creare il modulo personalizzato in altri modi, è possibile continuare con uno degli articoli seguenti:

   * [Aggiungere un campo personalizzato a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md)
   * [Posizionare campi e widget personalizzati in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Aggiunta o modifica di un widget di risorse in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [Riutilizzare un campo personalizzato calcolato esistente in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [Aggiungere logica di visualizzazione e ignorare la logica in un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [Anteprima e compilazione di un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)

## Sintassi necessaria nei campi personalizzati calcolati

Ogni campo deve utilizzare la sintassi illustrata di seguito, con parentesi graffe intorno al nome di ciascun campo. Quando inizi a digitare il nome di un campo, il sistema formula suggerimenti e puoi selezionarne uno per inserirlo nel calcolo. Se si immettono dati in un calcolo in modo errato, viene visualizzato un messaggio di avviso. Non è possibile salvare il modulo a meno che non si modifichi il calcolo per contenere campi validi e un&#39;espressione calcolata valida.

>[!NOTE]
>
>Attualmente, il sistema formula suggerimenti solo quando si inizia a digitare il nome di un campo a cui si desidera fare riferimento in un oggetto a cui verrà allegato il modulo personalizzato, non nell’oggetto principale dell’oggetto.

### Nomi dei campi surround con parentesi graffe

* Se si desidera che il calcolo faccia riferimento a un campo incorporato, il nome del campo deve essere racchiuso tra parentesi graffe.

Ad esempio: `{actualRevenue}`

I nomi dei campi sono sensibili all’uso di maiuscole e minuscole e devono essere visualizzati nel calcolo esattamente come sono visualizzati nel sistema Workfront.

* Se si desidera che il calcolo faccia riferimento a un campo personalizzato, il nome del campo deve essere racchiuso tra parentesi graffe e preceduto da `DE:` tra parentesi.

Ad esempio: `{DE:Profit}`

Il sistema elenca tutti i campi personalizzati tra cui è possibile scegliere quando si digita `DE:`.

* Se si desidera che il calcolo faccia riferimento a un campo che estrarrà i dati dal *parent* quando il modulo personalizzato è associato a un oggetto, è necessario precedere il nome del campo con il tipo di oggetto dell’oggetto principale, anche tra parentesi graffe.

   Ad esempio, se il modulo personalizzato è configurato in modo da funzionare con le attività e si desidera che il campo calcoli le entrate effettive dell’oggetto principale quando il modulo è associato a un’attività, è necessario indicare `Project` come tipo di oggetto del campo:

   `{project}.{actualRevenue}`

   Oppure, se si tratta di un campo personalizzato:

   `{project}.{DE:profit}`

   Se non si è sicuri di quale sarà il tipo di oggetto dell&#39;oggetto principale perché il valore personalizzato per è configurato per più tipi di oggetto, è possibile utilizzare la variabile filtro caratteri jolly `$$OBJCODE` per consentire il funzionamento del calcolo per ciascuno dei tipi possibili. Per ulteriori informazioni, consulta [Campi personalizzati calcolati nei moduli personalizzati con più oggetti](#calculated-custom-fields-in-multi-object-custom-forms) in questo articolo.

### Separa gli elementi con i periodi

Quando si fa riferimento a un oggetto correlato in un campo personalizzato calcolato, è necessario separare i nomi e gli attributi degli oggetti con i punti.

Ad esempio, in un modulo personalizzato di tipo task, per visualizzare il nome del proprietario del Portfolio in un campo personalizzato calcolato, digitare quanto segue:

`{project}.{porfolio}.{owner}`

Questo determinerebbe quanto segue: Dall’oggetto del modulo personalizzato (un’attività) è possibile accedere all’oggetto successivo relativo all’attività (un progetto). Da lì è possibile accedere all&#39;oggetto correlato successivo al progetto (un portfolio), quindi all&#39;oggetto correlato successivo al portfolio (il proprietario).

### Sintassi del nome per il riferimento a un campo personalizzato

Quando si fa riferimento a un altro campo personalizzato in un campo personalizzato calcolato, è necessario immettere il nome del campo visualizzato nell’interfaccia utente di Workfront.

Ad esempio, per fare riferimento all&#39;opzione selezionata in un campo personalizzato denominato sponsor esecutivo, digitare quanto segue:

`{DE:Executive sponsor}`

>[!NOTE]
>
>La sintassi di un campo typeahead è leggermente diversa da quella di altri tipi di campi, in quanto è necessario aggiungere `:name` alla fine.
>
>Ad esempio, per fare riferimento all&#39;opzione selezionata in un campo personalizzato typeahead denominato &quot;Executive sponsor&quot;, digitare:
>
>`{DE:Executive sponsor:name}`


## Campi personalizzati calcolati nei moduli personalizzati con più oggetti {#calculated-custom-fields-in-multi-object-custom-forms}

In un modulo personalizzato con più oggetti, i tipi di oggetto selezionati devono essere compatibili con tutti i campi a cui si fa riferimento nei campi personalizzati calcolati del modulo. In caso di incompatibilità, un messaggio ti avvisa di apportare modifiche.

>[!INFO]
>
>**Esempio:**
>
>In un modulo personalizzato configurato per l’utilizzo con il tipo di oggetto Task, è possibile creare un campo personalizzato calcolato denominato In Charge. È possibile configurarlo per fare riferimento al campo incorporato in modo che possa mostrare il nome dell’assegnatario principale incaricato ogni volta che il modulo è associato a un’attività:
>
>`{assignedTo}.{name}`
>
>Successivamente, aggiungere il tipo di oggetto Progetto al modulo personalizzato. Un messaggio di avviso indica che il tipo di oggetto Progetto non è compatibile con il campo personalizzato calcolato.

In questo caso, è possibile effettuare una delle seguenti operazioni:

* Rimuovere dal modulo personalizzato uno dei due elementi incompatibili, ovvero il tipo di oggetto o il campo personalizzato calcolato a cui si fa riferimento.
* Mantieni entrambi gli elementi e utilizza la variabile del filtro caratteri jolly `$$OBJCODE` come condizione in un&#39;espressione IF per creare due versioni diverse del campo In Charge . Questo consente al campo di funzionare correttamente, indipendentemente dal tipo di oggetto a cui è associato il modulo.

>[!INFO]
>
>**Esempio:** Anche se non è stato assegnato a: Campo Nome nei progetti, è presente un campo Proprietario integrato (che si riempie automaticamente con il nome della persona che ha creato il progetto, a meno che qualcuno non lo modifichi manualmente).
>
>Quindi, nel campo personalizzato In Charge, puoi utilizzare `$$OBJCODE` come mostrato di seguito, fare riferimento al campo Proprietario quando il modulo personalizzato è associato a un progetto e al campo Assegnato a: Campo Nome quando il modulo è associato a un’attività:
>
>`IF($$OBJCODE="PROJ",{owner}.{name},{assignedTo}.{name})`

Per ulteriori informazioni su variabili come `$$OBJCODE,` vedere [Variabili filtro caratteri jolly](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

## Aggiornamenti automatici dei campi personalizzati calcolati

I campi personalizzati calcolati su un oggetto vengono ricalcolati automaticamente quando si verificano le seguenti situazioni:

* Viene modificato un elemento dell’oggetto, ad esempio un calcolo giornaliero della timeline.
* Un utente modifica un altro campo a cui fa riferimento un campo personalizzato calcolato sull’oggetto.
* L&#39;espressione calcolata è vuota e il campo contiene un valore, che imposta il valore su null.

   >[!NOTE]
   >
   ><div>In un modulo personalizzato allegato a un oggetto, le istruzioni data e ora nei campi personalizzati calcolati vengono calcolate e salvate dall’Ora universale coordinata (UTC), non dalle configurazioni del fuso orario impostate per l’istanza dell’organizzazione e il profilo utente. I calcoli in un modulo personalizzato vengono generati in base ai singoli fusi orari di ciascun utente.</div>

