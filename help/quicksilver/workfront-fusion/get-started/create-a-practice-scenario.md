---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Creare uno scenario di integrazione pratica in Adobe Workfront Fusion
description: Questo articolo descrive come creare uno scenario di integrazione con Adobe Workfront Fusion. Gli scenari di integrazione collegano app separate, consentendo il flusso dei dati attraverso applicazioni diverse.
author: Becky
feature: Workfront Fusion
exl-id: 643bb1d5-d7bc-402b-8ed1-9ca9a30e4560
source-git-commit: 99a8ad82c5fb2fb3f6adce9ff037086523be9b02
workflow-type: tm+mt
source-wordcount: '2094'
ht-degree: 0%

---

# Creare uno scenario di integrazione pratica in Adobe Workfront Fusion

Questo articolo descrive come creare uno scenario di integrazione con Adobe Workfront Fusion. Gli scenari di integrazione collegano app separate, consentendo il flusso dei dati attraverso applicazioni diverse.

Per creare uno scenario di integrazione, l’organizzazione deve disporre di un [!DNL Workfront Fusion for Work Automation and Integration] licenza.

Per istruzioni sulla creazione di uno scenario di automazione solo Workfront, consulta [Creazione di uno scenario di automazione delle esercitazioni in Adobe Workfront Fusion](../../workfront-fusion/get-started/create-a-practice-automation-scenario.md)

Per ulteriori informazioni sulle licenze di Workfront Fusion, consulta [Licenze Adobe Workfront Fusion](../../workfront-fusion/get-started/license-automation-vs-integration.md).

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] per l'automazione e l'integrazione del lavoro] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare la funzionalità descritta in questo articolo.</td> 
  </tr> 
 </tbody> 
</table>

Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, consulta [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Creare uno scenario di esercitazione

Il ruolo di [!DNL Adobe Workfront Fusion] automatizzare i processi in modo da potersi concentrare su nuove attività anziché ripetere più volte le stesse attività. Funziona tramite il collegamento di azioni all’interno e tra app e servizi per creare uno scenario che trasferisce e trasforma automaticamente i dati. Lo scenario in cui si creano controlli i dati in un’app o in un servizio ed elabora tali dati in modo da fornire il risultato desiderato.

Uno scenario è costituito da una serie di moduli che indicano come i dati devono essere trasformati all’interno di un’app o trasferiti tra app e servizi web.

Spiegare come creare uno scenario e rafforzare le best practice durante l’utilizzo [!DNL Workfront Fusion], questo articolo illustra il processo in modo dettagliato. Creeremo uno scenario che crea un nuovo record in [!DNL Workfront] per ogni riga in una [!DNL Google Sheets] foglio di calcolo.

![](assets/finished-scenario-1-350x180.png)

>[!TIP]
>
>Uno scenario simile sarebbe utile se disponessi di un foglio di calcolo in cui sono elencati i progetti da elaborare utilizzando i progetti in [!DNL Workfront]. Lo scenario potrebbe &quot;guardare&quot; il foglio di calcolo per nuove righe e aggiungere un nuovo progetto in [!DNL Workfront] per ciascuno di essi.

La creazione di uno scenario è costituita da diverse attività principali:

## Scegli le app e assegna un nome allo scenario

1. Scarica questo [foglio di calcolo](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion/Fusion+Practice+Scenario+Sample+Sheet.xlsx), quindi caricalo sul tuo [!DNL Google Drive] da utilizzare in questo esercizio.

   Oppure

   Creare o trovare semplici [!DNL Google Sheets] foglio di calcolo simile a questo:

   ![](assets/spreadsheet-headers-350x55.png)

1. Accedi al tuo [!DNL Workfront Fusion] account.
1. Clic **[!UICONTROL Scenari]** ![](assets/scenarios-icon.png) nel pannello a sinistra.

   >[!NOTE]
   >
   >Se il pannello di navigazione a sinistra o le relative icone non sono visibili, fare clic sul menu ![Menu](assets/main-menu-icon-left-nav.png) icona.

   In grigio [!UICONTROL Cartelle] che viene visualizzato, puoi organizzare gli scenari in cartelle.

   Nella parte superiore dell&#39;area principale a destra è possibile visualizzare **[!UICONTROL Tutti]** scenari creati, il tuo **[!UICONTROL Scenari attivi]** e **[!UICONTROL Scenari inattivi]**, e **[!UICONTROL Concetti]**, che sono scenari che richiedono ancora un po’ di lavoro prima [!DNL Workfront Fusion] può classificarli come attivi o inattivi.

<!--
   ![](assets/scenarios-left-panel-350x215.png)
-->

1. In [!UICONTROL Cartelle] fare clic sul pulsante **[!UICONTROL Aggiungi cartella]** icona ![](assets/add-folder-icon.png), quindi digitare un nome come &quot;Scenari di esercitazione&quot; per la prima cartella.

1. Apri la cartella, quindi fai clic su **[!UICONTROL Crea un nuovo scenario]** nell’angolo superiore destro della pagina.

   La pagina di destinazione visualizzata consente di precaricare le app che desideri utilizzare nello scenario che stai per creare.

1. Per questo esercizio, cerca e seleziona la **[!UICONTROL Fogli Google]** app.
1. Clic **[!UICONTROL Continua]** nell’angolo superiore destro.

   Viene visualizzato l’editor dello scenario, contenente un modulo vuoto al centro, il [!DNL Google Sheets] app precaricata e alcune opzioni nella barra degli strumenti nella parte inferiore.

<!--
   ![](assets/scenario-editor-350x235.png)
-->

Quando si inizia a creare un nuovo scenario, è consigliabile iniziare con la creazione di un nome.

1. Seleziona la **[!UICONTROL Nuovo scenario]** nome segnaposto nell&#39;angolo superiore sinistro, quindi digitare un nome come &quot;Esercitazione scenario 1&quot;.
1. Continua con [Aggiungere e configurare il primo modulo](#add-and-configure-the-first-module) di seguito.

## Aggiungere e configurare il primo modulo

Il modulo vuoto con un punto interrogativo rappresenta il modulo trigger da aggiungere. Questo modulo avvia lo scenario ogni volta che viene eseguito. L’icona dell’orologio sul modulo vuoto indica che si tratta di un modulo pianificato.

![](assets/empty-module.png)

Questo modulo conterrà i dati che si desidera controllare nello scenario.

1. Fai clic sul modulo vuoto per scegliere l’app dalla quale selezionare un modulo.

   L’app precaricata in precedenza viene visualizzata accanto al modulo vuoto. Puoi aggiungere altre app che dispongono di moduli utilizzando [!UICONTROL Ricerca] casella.

   ![](assets/pre-loaded-apps-350x139.png)

1. Clic **[!DNL Google Sheets]**.

   L’elenco viene modificato in visualizza tutto [!DNL Google Sheets] moduli utilizzabili come modulo trigger.

1. Fai clic sul modulo di attivazione **[!UICONTROL Controlla i record]**.

   Ora devi stabilire una connessione autenticata al tuo account Google. Ogni modulo che aggiungi a uno scenario deve avere una connessione alla relativa app.

1. In **[!DNL Google Sheets]** casella, sotto **[!UICONTROL Connessione]**, fai clic su **[!UICONTROL Aggiungi]**, quindi digita un nome per la connessione, ad esempio &quot;Account Google di Olivia&quot;, quindi fai clic su **[!UICONTROL Continua]**.
1. Autentica la connessione nella finestra visualizzata.

   Il processo di autenticazione di una connessione può variare leggermente da un’app all’altra. Potrebbe essere necessario accedere all’app. In genere è necessario fare clic su un **[!UICONTROL Consenti]** pulsante. Se hai bisogno di aiuto, consulta [Informazioni sulla connessione [!DNL Adobe Workfront Fusion] a un’app o a un servizio](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

## Configurare il primo modulo

Dopo la connessione [!DNL Workfront Fusion] al tuo [!DNL Google Sheets] account, è possibile specificare un [!DNL Google Sheets] foglio di calcolo a cui hai accesso e i dati che desideri elaborare con il primo modulo.

1. Fai clic su **[!UICONTROL Foglio di calcolo]** , quindi selezionare il **[!UICONTROL Scenario di esercitazione di Workfront Fusion] #1** nell&#39;elenco visualizzato.

   Questo foglio di calcolo contiene 2 fogli (schede), pertanto è necessario specificare quale foglio contiene i dati desiderati:

1. In **[!UICONTROL Foglio]** elenco a discesa, seleziona **[!UICONTROL Progetti]**.

   Il foglio di calcolo contiene intestazioni che il modulo deve utilizzare per identificare i dati che si desidera elaborare:

   ![](assets/spreadsheet-headers-350x55.png)

1. Esci **[!UICONTROL Sì]** selezionato per **[!UICONTROL La tabella contiene le intestazioni]**.

1. In **[!UICONTROL Riga con intestazioni]** , è possibile specificare un intervallo di righe da includere, lasciando tuttavia l&#39;intervallo A1:Z1 predefinito per questo esercizio.
1. In **[!UICONTROL Limite]** digitare 1.

   In questo modo, ogni volta che esegui lo scenario, il modulo elaborerà solo 1 riga nel foglio di calcolo. Questo è utile per semplificare le esecuzioni dei test durante la creazione dello scenario.

1. Clic **[!UICONTROL OK]**.

   Il **[!UICONTROL Scegli da dove iniziare]** richiede di specificare la posizione nel foglio di calcolo in cui si desidera avviare l&#39;elaborazione del modulo.

1. Clic **[!UICONTROL Scegli manualmente]**, seleziona l’opzione in alto nell’elenco visualizzato, quindi fai clic su **[!UICONTROL OK]**.
1. Fai clic con il pulsante destro del mouse sul modulo e fai clic su **[!UICONTROL Rinomina]**, quindi digita un nome che descriva le operazioni che desideri eseguire il modulo (ad esempio, &quot;Guarda l’elenco dei progetti&quot;), quindi fai clic su **[!UICONTROL OK]**.

   Il nome viene visualizzato appena sotto il modulo. Sotto, [!DNL Workfront Fusion] include una breve descrizione del tipo di azione eseguita dal modulo.

   ![](assets/module-renamed-350x388.png)

1. Continua con [Aggiungere e configurare il secondo modulo](#add-and-configure-the-second-module).

## Aggiungere e configurare il secondo modulo

1. Fare clic sul cerchio parziale a destra della sezione del modulo per **[!UICONTROL Aggiungi un altro modulo]**.

   Questo secondo modulo deve essere un [!DNL Workfront] , ma non è stato precaricato il [!DNL Workfront] app.

1. Per trovare [!DNL Workfront] app, inizia a digitare &quot;[!DNL Workfront]&quot; e fai clic sull’app quando viene visualizzata.
1. Nell&#39;elenco di [!DNL Workfront] moduli visualizzati, fai clic su **[!UICONTROL Crea record]**.

1. Come hai fatto in precedenza con l’app Google Sheets, fai clic su **[!UICONTROL Aggiungi]** nel [!DNL Workfront] per aggiungere una connessione tra Workfront Fusion e Workfront.

   Ora inizieremo a specificare cosa fare con i dati del foglio di calcolo.

1. Clic **[!UICONTROL Tipo di record]**, quindi seleziona **[!UICONTROL Progetto]** perché vogliamo creare un progetto in [!DNL Workfront] utilizzando una riga del foglio di calcolo.

   >[!TIP]
   >
   >Puoi trovare **[!UICONTROL Progetto]** nell’elenco, se inizi a digitare la parola &quot;[!UICONTROL progetto].&quot;

   La casella si espande per visualizzare tutte le [!DNL Workfront] nei campi del progetto in cui è possibile inserire le informazioni presenti nel primo modulo.

   Utilizzeremo il **[!UICONTROL Nome]** campo: vogliamo che questo modulo denomini ogni progetto in [!DNL Workfront] utilizzando il testo nella [!UICONTROL Fogli Google] riga.

1. Trova e fai clic su **[!UICONTROL Nome]** campo.

   >[!TIP]
   >
   >È possibile utilizzare **Cmd+F** ([!DNL Mac] OS) o **Ctrl+F**([!DNL Windows] OS) per trovare rapidamente un campo.

   Viene aperto l’elenco delle variabili che puoi utilizzare nel **[!UICONTROL Nome]** per definire il nome di ciascun progetto creato in Workfront.

   ![](assets/list-of-available-variables-350x261.png)

   Tieni presente che le variabili nella parte superiore dell’elenco corrispondono alle intestazioni di colonna nel foglio di calcolo.

   ![](assets/spreadsheet-headers-marked-350x55.png)

   ![](assets/list-of-available-variables-marked-350x320.png)

1. Fai clic sulla variabile **[!UICONTROL Nome progetto personale (A)]** per aggiungerlo al **[!UICONTROL Nome]** campo.

   Hai appena mappato il tuo primo dato per questo scenario.

   Mappa un altro elemento di dati dal foglio di calcolo a [!DNL Workfront]: la data di inizio di ciascun progetto.

1. Trova e fai clic su **[!UICONTROL Data Inizio Pianificata]** , quindi fare clic sul pulsante **[!UICONTROL Data Inizio Pianificato (E)]** per estrarre i dati da tale colonna nel foglio di calcolo.

1. Clic **[!UICONTROL OK]**.

   Ora avete uno scenario di lavoro.

1. Assegna al secondo modulo un nome come &quot;Crea progetto Workfront&quot;, quindi continua con [Verifica lo scenario](#test-the-scenario).

## Verifica lo scenario

Prima di attivare lo scenario, è importante testarlo eseguendolo almeno una volta e visualizzando i risultati. Questo ti aiuta a capire come i dati scorrono attraverso lo scenario e a trovare eventuali errori.

Per creare un progetto in Workfront, abbiamo scelto di elaborare 1 riga dal foglio di calcolo. Se esegui lo scenario, questo è ciò che dovrebbe accadere.

1. Clic **[!UICONTROL Esegui una volta]** nell’angolo inferiore sinistro dell’editor di scenari.
1. Al termine dell’esecuzione dello scenario, fai clic sulla bolla sopra la [!DNL Google Sheets] modulo.

   ![](assets/click-bubble.png)

   Nella casella visualizzata è possibile visualizzare informazioni sul bundle di dati elaborati dal modulo, inclusi i dati effettivi estratti dal foglio di calcolo per la riga iniziale.

   ![](assets/execution-inspector-g-sheets-350x637.png)

1. Fare clic sull&#39;indicatore del controllo di esecuzione sopra il [!DNL Workfront] per visualizzare l’input delle informazioni e l’output, che è l’ID del progetto ora creato in [!DNL Workfront]

   ![](assets/execution-inspector-wf-350x384.png)

   Per ulteriori informazioni su come leggere le informazioni sull’esecuzione di uno scenario, consulta i seguenti articoli:

   * Per informazioni generali, consulta [Flusso di esecuzione dello scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).
   * Per informazioni sui bundle elaborati, consulta [Esecuzione di scenari, cicli e fasi in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

1. Vai a [!DNL Workfront] e cerca &quot;soho downtown loft&quot; per vedere il progetto che lo scenario ha creato. Questa era l’ultima riga del foglio di calcolo.
1. In entrata [!DNL Workfront Fusion], fai clic su **[!UICONTROL Salva]** ![](assets/save-icon.png) nell’angolo in basso a sinistra per salvare i progressi sullo scenario.

   >[!IMPORTANT]
   >
   >Risparmia spesso quando affili e testa uno scenario.

## Finalizza lo scenario e testalo di nuovo

È ancora necessario configurare lo scenario per creare progetti per tutte le altre righe nel foglio di calcolo.

1. Fai clic su **[!UICONTROL Righe di controllo]** modulo creato per i fogli di Google.
1. Modificare il **[!UICONTROL Limite]** a 100.

   Specificando un numero maggiore del numero di righe che si sa essere nel foglio di calcolo si assicura che lo scenario acquisirà tutte le righe.

1. Fare clic con il pulsante destro del mouse **[!UICONTROL Righe di controllo]** modulo, fai clic su **[!UICONTROL Scegli da dove iniziare]**, fai clic su **[!UICONTROL Tutti]**, quindi fai clic su **[!UICONTROL OK]**.

1. Clic **[!UICONTROL Esegui una volta]** e guardate cosa succede nelle bolle dell&#39;ispettore dell&#39;esecuzione.

   Il [!DNL Google] Fogli **[!UICONTROL Righe di controllo]** viene eseguito una volta per leggere tutte le righe. Poi il Workfront **[!UICONTROL Crea record]** Il modulo viene eseguito 20 volte per creare un progetto per ciascuna delle restanti 20 righe del foglio di calcolo.

1. Fare clic sulla bolla del controllo di esecuzione per [!DNL Workfront] per visualizzare tutte le 20 operazioni, quindi fare clic su una delle operazioni per visualizzare le informazioni sul progetto creato.
1. Clic **[!UICONTROL Salva]** ![](assets/save-icon.png) nell&#39;angolo inferiore sinistro.
1. Vai a [!DNL Workfront] per visualizzare i progetti creati dallo scenario.

>[!TIP]
>
>È consigliabile aggiungere note su ciascun modulo in modo facoltativo ma utile.
>
>1. Fare clic con il pulsante destro del mouse [!DNL Workfront] , quindi fai clic su **[!UICONTROL Aggiungi una nota]**.
>1. Nella nota visualizzata, digita una panoramica del modulo.
>
>    Questa funzione è utile perché non è necessario aprire il modulo in modo continuativo per verificarne il funzionamento. Ad esempio, puoi digitare &quot;Crea un progetto con Nome, Data di inizio pianificata e Priorità mappata dal foglio di calcolo&quot;.
>
>    Per [!UICONTROL Fogli Google] &quot;Osserva l’elenco dei progetti per le nuove righe o i nuovi progetti aggiunti&quot;.
>
>    È possibile aggiungere più note per un modulo.
>
>1. Chiudi **[!UICONTROL Note]** area.
>
>    Dopo aver aggiunto una nota a uno scenario, sulla schermata viene visualizzato un punto arancione **[!UICONTROL Note]** icona ![](assets/notes-icon-w-dot.png) nella parte inferiore dell’editor dello scenario.
>
>1. Fai clic su **[!UICONTROL Note]** icona ![](assets/notes-icon-w-dot.png) per visualizzare le note.
>



## Attiva lo scenario

Se si trattasse di uno scenario da utilizzare per i dati reali, l’ultima cosa da fare è attivarlo. Dopo aver attivato uno scenario, per impostazione predefinita viene eseguito ogni 15 minuti. Puoi modificare questa impostazione definendo quando e con quale frequenza desideri che venga eseguita.

Per ulteriori informazioni sull’attivazione degli scenari, consulta [Attivare o disattivare uno scenario in Adobe Workfront Fusion](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

Per informazioni sulle pianificazioni, consulta [Pianificazione di uno scenario in Adobe Workfront Fusion](../../workfront-fusion/scenarios/schedule-a-scenario.md).
