---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Creare uno scenario di integrazione pratica in Adobe Workfront Fusion
description: Questo articolo descrive come creare uno scenario di integrazione con Adobe Workfront Fusion. Gli scenari di integrazione collegano app separate, consentendo il flusso dei dati attraverso applicazioni diverse.
author: Becky
feature: Workfront Fusion
exl-id: 643bb1d5-d7bc-402b-8ed1-9ca9a30e4560
source-git-commit: f11af8d9d1e5fa65c2efb4d882d25f9e13784611
workflow-type: tm+mt
source-wordcount: '2139'
ht-degree: 0%

---

# Creare uno scenario di integrazione pratica in Adobe Workfront Fusion

Questo articolo descrive come creare uno scenario di integrazione con Adobe Workfront Fusion. Gli scenari di integrazione collegano app separate, consentendo il flusso dei dati attraverso applicazioni diverse.

Per creare uno scenario di integrazione, l&#39;organizzazione deve disporre di una licenza [!DNL Workfront Fusion for Work Automation and Integration].

Per istruzioni sulla creazione di uno scenario di automazione solo Workfront, vedere [Creare uno scenario di automazione in Adobe Workfront Fusion](../../workfront-fusion/get-started/create-a-practice-automation-scenario.md)

Per ulteriori informazioni sulle licenze Workfront Fusion, vedere [Licenze Adobe Workfront Fusion](../../workfront-fusion/get-started/license-automation-vs-integration.md).

>[!NOTE]
>
>L’organizzazione potrebbe non consentire l’accesso a Google Sheets. In questo caso, non sarà possibile impostare questa integrazione, ma le informazioni presentate qui possono essere utilizzate come esempio generale del funzionamento degli scenari di integrazione.

## Requisiti di accesso

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] piano*</td> 
   <td> <p>[!DNL Pro] o superiore</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td>
   <p>Requisiti di licenza correnti: nessun requisito di licenza [!DNL Workfront Fusion].</p>
   <p>Oppure</p>
   <p>Requisito licenza legacy: [!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>
   <p>Fabbisogno prodotto corrente: se si dispone del piano [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront], l'organizzazione deve acquistare [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo. [!DNL Workfront Fusion] è incluso nel piano [!UICONTROL Ultimate] [!DNL Workfront].</p>
   <p>Oppure</p>
   <p>Requisiti del prodotto legacy: la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Per conoscere il piano, il tipo di licenza o l&#39;accesso disponibili, contattare l&#39;amministratore [!DNL Workfront].

Per informazioni sulle [!DNL Adobe Workfront Fusion] licenze, vedere [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Creare uno scenario di esercitazione

Il ruolo di [!DNL Adobe Workfront Fusion] consiste nell&#39;automatizzare i processi in modo da potersi concentrare su nuove attività anziché ripetere più volte le stesse attività. Funziona tramite il collegamento di azioni all’interno e tra app e servizi per creare uno scenario che trasferisce e trasforma automaticamente i dati. Lo scenario in cui si creano controlli i dati in un’app o in un servizio ed elabora tali dati in modo da fornire il risultato desiderato.

Uno scenario è costituito da una serie di moduli che indicano come i dati devono essere trasformati all’interno di un’app o trasferiti tra app e servizi web.

Per spiegare come creare uno scenario e rafforzare le best practice durante l&#39;utilizzo di [!DNL Workfront Fusion], questo articolo illustra la procedura dettagliata. Verrà creato uno scenario che crea un nuovo record in [!DNL Workfront] per ogni riga in un foglio di calcolo [!DNL Google Sheets].

![](assets/finished-scenario-1-350x180.png)

>[!TIP]
>
>Uno scenario simile sarebbe utile se si disponesse di un foglio di calcolo che elenca i progetti da elaborare utilizzando i progetti in [!DNL Workfront]. Lo scenario potrebbe &quot;guardare&quot; il foglio di calcolo per le nuove righe e aggiungere un nuovo progetto in [!DNL Workfront] per ciascuna.

La creazione di uno scenario è costituita da diverse attività principali:

## Scegli le app e assegna un nome allo scenario

1. Scarica questo [foglio di calcolo](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion/Fusion+Practice+Scenario+Sample+Sheet.xlsx), quindi caricalo sul tuo [!DNL Google Drive] per utilizzarlo in questo esercizio.

   Oppure

   Crea o trova il tuo semplice foglio di calcolo [!DNL Google Sheets] simile a questo:

   ![](assets/spreadsheet-headers-350x55.png)

1. Accedi al tuo account [!DNL Workfront Fusion].
1. Fai clic su **[!UICONTROL Scenari]** ![](assets/scenarios-icon.png) nel pannello a sinistra.

   >[!NOTE]
   >
   >Se il pannello di navigazione a sinistra o le relative icone non sono visibili, fare clic sull&#39;icona Menu ![Menu](assets/main-menu-icon-left-nav.png).

   Nel pannello grigio [!UICONTROL Cartelle] visualizzato, puoi organizzare gli scenari in cartelle.

   Nella parte superiore dell&#39;area principale a destra è possibile visualizzare **[!UICONTROL Tutti]** gli scenari generati, **[!UICONTROL Scenari attivi]** e **[!UICONTROL Scenari inattivi]** e **[!UICONTROL Concetti]**, che richiedono ulteriore lavoro prima che [!DNL Workfront Fusion] possa classificarli come attivi o inattivi.

<!--
   ![](assets/scenarios-left-panel-350x215.png)
-->

1. Nel pannello [!UICONTROL Cartelle], fai clic sull&#39;icona ![](assets/add-folder-icon.png) di **[!UICONTROL Aggiungi cartella]**, quindi digita un nome come &quot;Scenari di esercitazione&quot; per la tua prima cartella.

1. Apri la cartella, quindi fai clic su **[!UICONTROL Crea un nuovo scenario]** nell&#39;angolo superiore destro della pagina.

   La pagina di destinazione visualizzata consente di precaricare le app che desideri utilizzare nello scenario che stai per creare.

1. Per questo esercizio, cerca e seleziona l&#39;app **[!UICONTROL Google Sheets]**.
1. Fai clic su **[!UICONTROL Continua]** nell&#39;angolo superiore destro.

   Viene visualizzato l&#39;editor dello scenario, contenente un modulo vuoto al centro, l&#39;app [!DNL Google Sheets] precaricata e alcune opzioni nella barra degli strumenti nella parte inferiore.

<!--
   ![](assets/scenario-editor-350x235.png)
-->

Quando si inizia a creare un nuovo scenario, è consigliabile iniziare con la creazione di un nome.

1. Seleziona il nome del segnaposto **[!UICONTROL Nuovo scenario]** nell&#39;angolo superiore sinistro, quindi digita un nome come &quot;Esercitazione scenario 1&quot;.
1. Continua con [Aggiungi e configura il primo modulo](#add-and-configure-the-first-module) di seguito.

## Aggiungere e configurare il primo modulo

Il modulo vuoto con un punto interrogativo rappresenta il modulo trigger da aggiungere. Questo modulo avvia lo scenario ogni volta che viene eseguito. L’icona dell’orologio sul modulo vuoto indica che si tratta di un modulo pianificato.

![](assets/empty-module.png)

Questo modulo conterrà i dati che si desidera controllare nello scenario.

1. Fai clic sul modulo vuoto per scegliere l’app dalla quale selezionare un modulo.

   L’app precaricata in precedenza viene visualizzata accanto al modulo vuoto. È possibile aggiungere altre app con moduli utilizzando la casella [!UICONTROL Cerca].

   ![](assets/pre-loaded-apps-350x139.png)

1. Fare clic su **[!DNL Google Sheets]**.

   L&#39;elenco viene modificato in modo da visualizzare tutti i moduli [!DNL Google Sheets] che è possibile utilizzare come modulo trigger.

1. Fare clic sul modulo trigger **[!UICONTROL Controlla i record]**.

   Ora devi stabilire una connessione autenticata al tuo account Google. Ogni modulo che aggiungi a uno scenario deve avere una connessione alla relativa app.

1. Nella casella **[!DNL Google Sheets]**, in **[!UICONTROL Connessione]**, fare clic su **[!UICONTROL Aggiungi]**, quindi digitare un nome per la connessione, ad esempio &quot;Account Google di Olivia&quot;, quindi fare clic su **[!UICONTROL Continua]**.
1. Autentica la connessione nella finestra visualizzata.

   Il processo di autenticazione di una connessione può variare leggermente da un’app all’altra. Potrebbe essere necessario accedere all’app. In genere è necessario fare clic su un pulsante **[!UICONTROL Consenti]**. Se hai bisogno di aiuto, consulta [Panoramica delle connessioni](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

## Configurare il primo modulo

Dopo aver connesso [!DNL Workfront Fusion] all&#39;account [!DNL Google Sheets], è possibile specificare un foglio di calcolo [!DNL Google Sheets] a cui si ha accesso e i dati che si desidera elaborare con il primo modulo.

1. Workfront Fare clic sulla casella **[!UICONTROL Foglio di calcolo]**, quindi selezionare il **[!UICONTROL Fusion practice scenario] #1** nell&#39;elenco visualizzato.

   Questo foglio di calcolo contiene 2 fogli (schede), pertanto è necessario specificare quale foglio contiene i dati desiderati:

1. Nell&#39;elenco a discesa **[!UICONTROL Foglio]**, selezionare **[!UICONTROL Progetti]**.

   Il foglio di calcolo contiene intestazioni che il modulo deve utilizzare per identificare i dati che si desidera elaborare:

   ![](assets/spreadsheet-headers-350x55.png)

1. Lascia **[!UICONTROL Sì]** selezionato per **[!UICONTROL La tabella contiene intestazioni]**.

1. Nella casella **[!UICONTROL Riga con intestazioni]** è possibile specificare un intervallo di righe che si desidera includere, ma lasciare l&#39;intervallo A1:Z1 predefinito per questo esercizio.
1. Nella casella **[!UICONTROL Limite]** digitare 1.

   In questo modo, ogni volta che esegui lo scenario, il modulo elaborerà solo 1 riga nel foglio di calcolo. Questo è utile per semplificare le esecuzioni dei test durante la creazione dello scenario.

1. Fare clic su **[!UICONTROL OK]**.

   Nella casella **[!UICONTROL Scegli da dove iniziare]** viene richiesto di specificare la posizione nel foglio di calcolo in cui si desidera avviare l&#39;elaborazione del modulo.

1. Fai clic su **[!UICONTROL Scegli manualmente]**, seleziona l&#39;opzione in alto nell&#39;elenco visualizzato, quindi fai clic su **[!UICONTROL OK]**.
1. Fare clic con il pulsante destro del mouse sul modulo, scegliere **[!UICONTROL Rinomina]**, quindi digitare un nome che descriva le operazioni che si desidera vengano eseguite dal modulo, ad esempio &quot;Osserva l&#39;elenco dei progetti&quot;, quindi scegliere **[!UICONTROL OK]**.

   Il nome viene visualizzato appena sotto il modulo. Di seguito, [!DNL Workfront Fusion] include una breve descrizione del tipo di azione eseguita dal modulo.

   ![](assets/module-renamed-350x388.png)

1. Continua con [Aggiungi e configura il secondo modulo](#add-and-configure-the-second-module).

## Aggiungere e configurare il secondo modulo

1. Fare clic sul cerchio parziale a destra del del modulo per **[!UICONTROL Aggiungere un altro modulo]**.

   Il secondo modulo deve essere un modulo [!DNL Workfront], ma non è stata precaricata l&#39;app [!DNL Workfront].

1. Per trovare l&#39;app [!DNL Workfront], inizia a digitare &quot;[!DNL Workfront]&quot; e fai clic sull&#39;app quando viene visualizzata.
1. Nell&#39;elenco dei moduli [!DNL Workfront] visualizzati fare clic su **[!UICONTROL Crea record]**.

1. Come in precedenza con l&#39;app Google Sheets, fare clic su **[!UICONTROL Aggiungi]** nella casella [!DNL Workfront] per aggiungere una connessione tra Workfront Fusion e Workfront.

   Ora inizieremo a specificare cosa fare con i dati del foglio di calcolo.

1. Fare clic su **[!UICONTROL Tipo di record]**, quindi selezionare **[!UICONTROL Progetto]** perché si desidera creare un progetto in [!DNL Workfront] utilizzando una riga del foglio di calcolo.

   >[!TIP]
   >
   >Puoi trovare **[!UICONTROL Project]** nell&#39;elenco se inizi a digitare la parola &quot;[!UICONTROL project].&quot;

   La casella si espande per visualizzare tutti i campi disponibili del progetto [!DNL Workfront] in cui è possibile inserire le informazioni trovate dal primo modulo.

   Stiamo per utilizzare il campo **[!UICONTROL Name]**: questo modulo deve denominare ogni progetto in [!DNL Workfront] utilizzando il testo nella riga [!UICONTROL Google Sheets] corrispondente.

1. Trova e fai clic sul campo **[!UICONTROL Nome]**.

   >[!TIP]
   >
   >È possibile utilizzare **Cmd+F** ([!DNL Mac] OS) o **Ctrl-F**([!DNL Windows] OS) per trovare rapidamente un campo.

   Verrà aperto l&#39;elenco delle variabili che è possibile utilizzare nel campo **[!UICONTROL Name]** per definire il nome di ogni progetto creato in Workfront.

   ![](assets/list-of-available-variables-350x261.png)

   Tieni presente che le variabili nella parte superiore dell’elenco corrispondono alle intestazioni di colonna nel foglio di calcolo.

   ![](assets/spreadsheet-headers-marked-350x55.png)

   ![](assets/list-of-available-variables-marked-350x320.png)

1. Fare clic sulla variabile **[!UICONTROL Nome progetto personale (A)]** per aggiungerla al campo **[!UICONTROL Nome]**.

   Hai appena mappato il tuo primo dato per questo scenario.

   Mappare un altro elemento di dati dal foglio di calcolo a [!DNL Workfront]: la data di inizio di ciascun progetto.

1. Trova e fai clic sul campo **[!UICONTROL Data inizio pianificata]**, quindi fai clic sulla variabile **[!UICONTROL Data inizio pianificata (E)]**, per estrarre i dati da quella colonna nel foglio di calcolo.

1. Fare clic su **[!UICONTROL OK]**.

   Ora avete uno scenario di lavoro.

1. Assegna al secondo modulo un nome come &quot;Crea progetto Workfront&quot;, quindi continua con [Verifica lo scenario](#test-the-scenario).

## Verifica lo scenario

Prima di attivare lo scenario, è importante testarlo eseguendolo almeno una volta e visualizzando i risultati. Questo ti aiuta a capire come i dati scorrono attraverso lo scenario e a trovare eventuali errori.

Per creare un progetto in Workfront, abbiamo scelto di elaborare 1 riga dal foglio di calcolo. Se esegui lo scenario, questo è ciò che dovrebbe accadere.

1. Fai clic su **[!UICONTROL Esegui una volta]** nell&#39;angolo inferiore sinistro dell&#39;editor scenari.
1. Al termine dell&#39;esecuzione dello scenario, fare clic sulla bolla sopra il modulo [!DNL Google Sheets].

   ![](assets/click-bubble.png)

   Nella casella visualizzata è possibile visualizzare informazioni sul bundle di dati elaborati dal modulo, inclusi i dati effettivi estratti dal foglio di calcolo per la riga iniziale.

   ![](assets/execution-inspector-g-sheets-350x637.png)

1. Fare clic sul fumetto del controllo di esecuzione sopra il modulo [!DNL Workfront] per visualizzare l&#39;input delle informazioni e l&#39;output, che è l&#39;ID del progetto creato in [!DNL Workfront]

   ![](assets/execution-inspector-wf-350x384.png)

   Per ulteriori informazioni su come leggere le informazioni sull’esecuzione di uno scenario, consulta i seguenti articoli:

   * Per informazioni generali, vedere [Flusso di esecuzione dello scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).
   * Per informazioni sui bundle elaborati, vedere [Esecuzione scenario, cicli e fasi in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

1. Vai a [!DNL Workfront] e cerca &quot;soho downtown loft&quot; per vedere il progetto creato dallo scenario. Questa era l’ultima riga del foglio di calcolo.
1. In [!DNL Workfront Fusion], fai clic su **[!UICONTROL Salva]** ![](assets/save-icon.png) nell&#39;angolo inferiore sinistro per salvare l&#39;avanzamento dello scenario.

   >[!IMPORTANT]
   >
   >Risparmia spesso quando affili e testa uno scenario.

## Finalizza lo scenario e testalo di nuovo

È ancora necessario configurare lo scenario per creare progetti per tutte le altre righe nel foglio di calcolo.

1. Fare clic sul modulo **[!UICONTROL Righe controllo]** creato per i fogli Google.
1. Cambia il **[!UICONTROL limite]** in 100.

   Specificando un numero maggiore del numero di righe che si sa essere nel foglio di calcolo si assicura che lo scenario acquisirà tutte le righe.

1. Fare clic con il pulsante destro del mouse sul modulo **[!UICONTROL Righe controllo]**, scegliere **[!UICONTROL Scegli da dove iniziare]**, fare clic su **[!UICONTROL Tutte]** e quindi su **[!UICONTROL OK]**.

1. Fai clic su **[!UICONTROL Esegui una volta]** e osserva cosa accade nelle bolle della finestra di ispezione dell&#39;esecuzione.

   Il modulo [!DNL Google] Fogli **[!UICONTROL Osserva righe]** viene eseguito una sola volta per leggere tutte le righe. Il modulo **[!UICONTROL Crea record]** di Workfront viene quindi eseguito 20 volte per creare un progetto per ciascuna delle restanti 20 righe del foglio di calcolo.

1. Fare clic sul fumetto del controllo di esecuzione per il modulo [!DNL Workfront] per visualizzare tutte le 20 operazioni, quindi fare clic su una delle operazioni per visualizzare le informazioni sul progetto creato.
1. Fai clic su **[!UICONTROL Salva]** ![](assets/save-icon.png) nell&#39;angolo inferiore sinistro.
1. Vai a [!DNL Workfront] per visualizzare i progetti creati dallo scenario.

>[!TIP]
>
>È consigliabile aggiungere note su ciascun modulo in modo facoltativo ma utile.
>
>1. Fare clic con il pulsante destro del mouse sul modulo [!DNL Workfront], quindi scegliere **[!UICONTROL Aggiungi nota]**.
>1. Nella nota visualizzata, digita una panoramica del modulo.
>
>    Questa funzione è utile perché non è necessario aprire il modulo in modo continuativo per verificarne il funzionamento. Ad esempio, puoi digitare &quot;Crea un progetto con Nome, Data di inizio pianificata e Priorità mappata dal foglio di calcolo&quot;.
>
>    Per il modulo [!UICONTROL Google Sheets], è possibile digitare qualcosa di simile a &quot;Osserva elenco progetti per le nuove righe/progetti aggiunti&quot;.
>
>    È possibile aggiungere più note per un modulo.
>
>1. Chiudi l&#39;area **[!UICONTROL Note]**.
>
>    Dopo aver aggiunto una nota a uno scenario, un punto arancione viene visualizzato sull&#39;icona **[!UICONTROL Note]** ![](assets/notes-icon-w-dot.png) nella parte inferiore dell&#39;editor dello scenario.
>
>1. Fai clic sull&#39;icona **[!UICONTROL Note]** ![](assets/notes-icon-w-dot.png) per visualizzare le note.
>



## Attiva lo scenario

Se si trattasse di uno scenario da utilizzare per i dati reali, l’ultima cosa da fare è attivarlo. Dopo aver attivato uno scenario, per impostazione predefinita viene eseguito ogni 15 minuti. Puoi modificare questa impostazione definendo quando e con quale frequenza desideri che venga eseguita.

Per ulteriori informazioni sull&#39;attivazione degli scenari, vedere [Attivare o disattivare uno scenario in Adobe Workfront Fusion](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

Per informazioni sulle pianificazioni, consulta [Pianificare uno scenario in Adobe Workfront Fusion](../../workfront-fusion/scenarios/schedule-a-scenario.md).
