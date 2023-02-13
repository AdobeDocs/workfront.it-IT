---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Creare uno scenario di integrazione pratica in Adobe Workfront Fusion
description: Questo articolo descrive come creare uno scenario di integrazione con Adobe Workfront Fusion. Gli scenari di integrazione collegano app separate tra loro, consentendo al flusso di dati attraverso applicazioni diverse.
author: Becky
feature: Workfront Fusion
exl-id: 643bb1d5-d7bc-402b-8ed1-9ca9a30e4560
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '2076'
ht-degree: 0%

---

# Creare uno scenario di integrazione pratica in Adobe Workfront Fusion

Questo articolo descrive come creare uno scenario di integrazione con Adobe Workfront Fusion. Gli scenari di integrazione collegano app separate tra loro, consentendo al flusso di dati attraverso applicazioni diverse.

Per creare uno scenario di integrazione, l’organizzazione deve disporre di un [!DNL Workfront Fusion for Work Automation and Integration] licenza.

Per istruzioni su come creare uno scenario di automazione solo Workfront, vedi [Creare uno scenario di automazione pratica in Adobe Workfront Fusion](../../workfront-fusion/get-started/create-a-practice-automation-scenario.md)

Per ulteriori informazioni sulle licenze Workfront Fusion, vedi [Licenze Adobe Workfront Fusion](../../workfront-fusion/get-started/license-automation-vs-integration.md).

>[!NOTE]
>
>L’organizzazione potrebbe non consentire l’accesso ai fogli Google. In questo caso, non sarà possibile impostare questa integrazione, ma le informazioni qui presentate possono essere utilizzate come esempio generale del funzionamento degli scenari di integrazione.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</td> 
  </tr> 
 </tbody> 
</table>

Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, vedi [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Creare uno scenario di esercitazione

Il ruolo [!DNL Adobe Workfront Fusion] automatizza i processi in modo da poterti concentrare su nuove attività anziché ripetere più e più volte le stesse attività. Funziona tramite il collegamento di azioni all’interno e tra app e servizi per creare uno scenario che trasferisca e trasformi automaticamente i tuoi dati. Lo scenario in cui crei orologi i dati in un&#39;app o in un servizio ed elabora tali dati per fornire il risultato desiderato.

Uno scenario è composto da una serie di moduli che indicano come i dati devono essere trasformati all&#39;interno di un&#39;app o trasferiti tra app e servizi web.

Per spiegare come creare uno scenario e rafforzare le best practice durante l’utilizzo [!DNL Workfront Fusion], questo articolo illustra il processo passo dopo passo. Creeremo uno scenario che crea un nuovo record in [!DNL Workfront] per ogni riga in un [!DNL Google Sheets] foglio di calcolo.

![](assets/finished-scenario-1-350x180.png)

>[!TIP]
>
>Uno scenario come questo sarebbe utile se avessi un foglio di calcolo in cui sono elencati i progetti su cui è necessario lavorare utilizzando i progetti in [!DNL Workfront]. Lo scenario potrebbe &quot;guardare&quot; il foglio di calcolo per nuove righe e aggiungere un nuovo progetto in [!DNL Workfront] per ciascuno di essi.

La creazione di uno scenario è costituita da diverse attività principali:

## Scegli le app e assegna un nome allo scenario

1. Scarica questo [foglio](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion/Fusion+Practice+Scenario+Sample+Sheet.xlsx), quindi caricalo sul tuo [!DNL Google Drive] per l&#39;utilizzo durante l&#39;esercizio.

   Oppure

   Crea o trova il tuo semplice [!DNL Google Sheets] foglio di calcolo simile a questo:

   ![](assets/spreadsheet-headers-350x55.png)

1. Accedi al tuo [!DNL Workfront Fusion] conto.
1. Fai clic su **[!UICONTROL Scenari]** ![](assets/scenarios-icon.png) nel pannello a sinistra.

   Nel pannello a sinistra visualizzato, puoi organizzare gli scenari in cartelle.

   Nella parte superiore dell&#39;area principale a destra, è possibile visualizzare **[!UICONTROL Tutto]** scenari creati, **[!UICONTROL Scenari attivi]** e **[!UICONTROL Scenari inattivi]** e **[!UICONTROL Concetti]**, che sono scenari che richiedono un po&#39; più di lavoro prima di [!DNL Workfront Fusion] possono classificarli come attivi o inattivi.

   ![](assets/scenarios-left-panel-350x215.png)

1. Nel pannello a sinistra, fai clic sul pulsante **[!UICONTROL Aggiungi cartella]** icona ![](assets/add-folder-icon.png), quindi digita un nome come &quot;Scenari di esercitazione&quot; per la prima cartella.

1. Apri la cartella, quindi fai clic su **[!UICONTROL Creare un nuovo scenario]** nell’angolo superiore destro della pagina.

   La pagina di destinazione visualizzata ti consente di precaricare le app che desideri utilizzare nello scenario da generare.

1. Per questo esercizio, cerca e seleziona la **[!UICONTROL Fogli Google]** app.
1. Fai clic su **[!UICONTROL Continua]** nell&#39;angolo in alto a destra.

   Viene visualizzato l’editor dello scenario, contenente un modulo vuoto al centro, il [!DNL Google Sheets] app precaricata e alcune opzioni nella barra degli strumenti in basso.

   ![](assets/scenario-editor-350x235.png)

   Quando si inizia a creare un nuovo scenario, è bene iniziare creando un nome per esso.

1. Seleziona la **[!UICONTROL Nuovo scenario]** nome del segnaposto nell&#39;angolo in alto a sinistra, quindi digitare un nome come &quot;Scenario di esercitazione 1&quot;.
1. Continua con [Aggiungi e configura il primo modulo](#add-and-configure-the-first-module) sotto.

## Aggiungi e configura il primo modulo

Il modulo vuoto con punto interrogativo rappresenta il modulo trigger da aggiungere. Questo modulo avvierà lo scenario ogni volta che viene eseguito. L’icona dell’orologio nel modulo vuoto indica che si tratta di un modulo pianificato.

![](assets/empty-module.png)

Questo modulo conterrà i dati per i quali si desidera che lo scenario venga controllato.

1. Fai clic sul modulo vuoto per scegliere l’app da cui selezionare un modulo.

   L’app precaricata viene visualizzata accanto al modulo vuoto. Puoi aggiungere qualsiasi altra app con moduli utilizzando [!UICONTROL Ricerca] scatola.

   ![](assets/pre-loaded-apps-350x139.png)

1. Clic **[!DNL Google Sheets]**.

   L’elenco viene modificato per visualizzare tutti [!DNL Google Sheets] moduli utilizzabili come modulo trigger.

1. Fai clic sul modulo trigger **[!UICONTROL Cerca record]**.

   Ora devi stabilire una connessione autenticata al tuo account Google. Ogni modulo che aggiungi a uno scenario deve avere una connessione alla relativa app.

1. In **[!DNL Google Sheets]** box, sotto **[!UICONTROL Connessione]**, fai clic su **[!UICONTROL Aggiungi]**, quindi digita un nome per la connessione, ad esempio &quot;l&#39;account Google di Olivia&quot;, quindi fai clic su **[!UICONTROL Continua]**.
1. Autentica la connessione nella finestra visualizzata.

   Il processo di autenticazione di una connessione può variare un po&#39; tra le app. Potrebbe essere necessario accedere all’app. In genere è necessario fare clic su un **[!UICONTROL Consenti]** pulsante . Se hai bisogno di aiuto, consulta [Informazioni sulla connessione [!DNL Adobe Workfront Fusion] a un&#39;app o a un servizio](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

## Configura il primo modulo

Dopo la connessione [!DNL Workfront Fusion] al tuo [!DNL Google Sheets] è possibile specificare un [!DNL Google Sheets] foglio di calcolo a cui hai accesso e i dati a cui desideri che venga elaborato il primo modulo.

1. Fai clic sul pulsante **[!UICONTROL Foglio di calcolo]** quindi seleziona la **[!UICONTROL Scenario pratico Workfront Fusion] #1** nell’elenco visualizzato.

   Questo foglio di calcolo contiene 2 fogli (schede), quindi è necessario specificare quale foglio contiene i dati desiderati:

1. In **[!UICONTROL Foglio]** elenco a discesa, seleziona **[!UICONTROL Progetti]**.

   Il nostro foglio di calcolo contiene intestazioni e vogliamo che il modulo le utilizzi per identificare i dati che desideri elaborare:

   ![](assets/spreadsheet-headers-350x55.png)

1. Esci **[!UICONTROL Sì]** selezionato per **[!UICONTROL La tabella contiene intestazioni]**.

1. In **[!UICONTROL Riga con intestazioni]** È possibile specificare un intervallo di righe da includere, ma lasciamo lì il valore predefinito A1:Z1 per questo esercizio.
1. In **[!UICONTROL Limite]** casella, tipo 1.

   In questo modo, ogni volta che esegui lo scenario, il modulo elabora solo 1 riga nel foglio di calcolo. Questa opzione è utile per semplificare le esecuzioni dei test durante la creazione dello scenario.

1. Fai clic su **[!UICONTROL OK]**.

   La **[!UICONTROL Scegli da dove iniziare]** viene richiesto di specificare la posizione nel foglio di calcolo in cui si desidera avviare l&#39;elaborazione del modulo.

1. Fai clic su **[!UICONTROL Scegli manualmente]**, seleziona l’opzione superiore nell’elenco visualizzato, quindi fai clic su **[!UICONTROL OK]**.
1. Fai clic con il pulsante destro del mouse sul modulo e fai clic su **[!UICONTROL Rinomina]**, quindi digita un nome che descriva le operazioni che desideri eseguire dal modulo (ad esempio &quot;Guarda l’elenco dei progetti&quot;), quindi fai clic su **[!UICONTROL OK]**.

   Il nome viene visualizzato sotto il modulo. Sotto questo, [!DNL Workfront Fusion] include una breve descrizione del tipo di azione eseguita dal modulo.

   ![](assets/module-renamed-350x388.png)

1. Continua con [Aggiungi e configura il secondo modulo](#add-and-configure-the-second-module).

## Aggiungi e configura il secondo modulo

1. Fai clic sul cerchio parziale a destra del modulo a **[!UICONTROL Aggiungi un altro modulo]**.

   Questo secondo modulo deve essere un [!DNL Workfront] modulo, ma non abbiamo precaricato il [!DNL Workfront] app.

1. Per trovare il [!DNL Workfront] app, inizia a digitare &quot;[!DNL Workfront]&quot; e fai clic sull&#39;app quando viene visualizzata.
1. Nell&#39;elenco di [!DNL Workfront] moduli visualizzati, fai clic su **[!UICONTROL Crea record]**.

1. Come prima con l&#39;app Google Sheets, fai clic su **[!UICONTROL Aggiungi]** in [!DNL Workfront] per aggiungere una connessione tra Workfront Fusion e Workfront.

   Ora inizieremo a specificare cosa vogliamo fare con i dati dal foglio di calcolo.

1. Fai clic su **[!UICONTROL Tipo di record]**, quindi seleziona **[!UICONTROL Progetto]** perché vogliamo creare un progetto in [!DNL Workfront] utilizzo di una riga dal foglio di calcolo.

   >[!TIP]
   >
   >È possibile trovare **[!UICONTROL Progetto]** nell&#39;elenco se si inizia a digitare la parola &quot;[!UICONTROL progetto].&quot;

   La casella si espande per visualizzare tutte le opzioni disponibili [!DNL Workfront] campi del progetto in cui è possibile inserire le informazioni trovate dal primo modulo.

   Useremo il **[!UICONTROL Nome]** campo: vogliamo che questo modulo nomini ogni progetto in [!DNL Workfront] utilizzando il testo nel corrispondente [!UICONTROL Fogli Google] fila.

1. Trova e fai clic sul pulsante **[!UICONTROL Nome]** campo .

   >[!TIP]
   >
   >È possibile utilizzare **Comando+F** ([!DNL Mac] OS) o **Ctrl+F**([!DNL Windows] OS) per trovare rapidamente un campo.

   Viene visualizzato l’elenco delle variabili utilizzabili in **[!UICONTROL Nome]** per definire il nome di ciascun progetto creato in Workfront.

   ![](assets/list-of-available-variables-350x261.png)

   Le variabili situate nella parte superiore dell’elenco corrispondono alle intestazioni di colonna nel foglio di calcolo.

   ![](assets/spreadsheet-headers-marked-350x55.png)

   ![](assets/list-of-available-variables-marked-350x320.png)

1. Fai clic sulla variabile **[!UICONTROL Nome Progetto (A)]** per aggiungerlo al **[!UICONTROL Nome]** campo .

   Hai appena mappato la tua prima parte di dati per questo scenario.

   Mappare un altro elemento di dati dal foglio di calcolo su [!DNL Workfront]: la data di inizio di ciascun progetto.

1. Trova e fai clic sul pulsante **[!UICONTROL Data di inizio prevista]** quindi fai clic sul campo **[!UICONTROL Data di inizio prevista (E)]** per estrarre i dati da quella colonna nel foglio di calcolo.

1. Fai clic su **[!UICONTROL OK]**.

   Ora avete uno scenario di lavoro.

1. Assegna al secondo modulo un nome, ad esempio &quot;Crea progetto Workfront&quot;, quindi continua con [Verificare lo scenario](#test-the-scenario).

## Verificare lo scenario

Prima di attivare lo scenario, è importante testarlo eseguendo almeno una volta e visualizzando i risultati. Questo ti aiuta a capire come i dati scorrono nello scenario e trovare eventuali errori.

Abbiamo scelto di elaborare 1 riga dal foglio di calcolo per creare un progetto in Workfront. Se esegui lo scenario, questo è ciò che dovrebbe accadere.

1. Fai clic su **[!UICONTROL Esegui una volta]** nell’angolo in basso a sinistra dell’editor di scenari.
1. Al termine dello scenario, fai clic sulla bolla sopra la [!DNL Google Sheets] modulo .

   ![](assets/click-bubble.png)

   Nella casella visualizzata, puoi visualizzare informazioni sul bundle di dati elaborato dal modulo, compresi i dati effettivi estratti dal foglio di calcolo per la riga con cui hai iniziato.

   ![](assets/execution-inspector-g-sheets-350x637.png)

1. Fai clic sulla bolla dell’ispettore di esecuzione sopra la [!DNL Workfront] modulo per visualizzare l’input delle informazioni e l’output, corrispondente all’ID del progetto ora creato in [!DNL Workfront]

   ![](assets/execution-inspector-wf-350x384.png)

   Per ulteriori informazioni su come leggere le informazioni sull’esecuzione di scenari, consulta i seguenti articoli:

   * Per informazioni generali, consulta [Flusso di esecuzione dello scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).
   * Per informazioni sui bundle elaborati, vedi [Esecuzione di scenari, cicli e fasi in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

1. Vai a [!DNL Workfront] e cercare &quot;soho downtown loft&quot; per vedere il progetto che lo scenario ha creato. Questa era l’ultima riga del foglio di calcolo.
1. In [!DNL Workfront Fusion], fai clic su **[!UICONTROL Salva]** ![](assets/save-icon.png) nell’angolo in basso a sinistra per salvare l’avanzamento dello scenario.

   >[!IMPORTANT]
   >
   >Puoi salvare spesso durante l’elaborazione e il test di uno scenario.

## Completare lo scenario e testarlo nuovamente

È comunque necessario configurare lo scenario per creare progetti per tutte le altre righe nel foglio di calcolo.

1. Fai clic sul pulsante **[!UICONTROL Righe di controllo]** modulo creato per Google Sheets.
1. Modificare la **[!UICONTROL Limite]** a 100.

   Specificando un numero maggiore del numero di righe che si conoscono nel foglio di calcolo si assicura che lo scenario acquisirà tutte.

1. Fai clic con il pulsante destro del mouse sul pulsante **[!UICONTROL Righe di controllo]** modulo, fai clic su **[!UICONTROL Scegli da dove iniziare]**, fai clic su **[!UICONTROL Tutto]**, quindi fai clic su **[!UICONTROL OK]**.

1. Fai clic su **[!UICONTROL Esegui una volta]** e guardate cosa succede nelle bolle dell&#39;ispettore dell&#39;esecuzione.

   La [!DNL Google] Fogli **[!UICONTROL Righe di controllo]** Il modulo viene eseguito una volta per leggere tutte le righe. Poi il Workfront **[!UICONTROL Crea record]** Il modulo viene eseguito 20 volte per creare un progetto per ciascuna delle 20 righe rimanenti nel foglio di calcolo.

1. Fai clic sulla bolla dell’ispettore di esecuzione per il [!DNL Workfront] modulo per visualizzare tutte e 20 le operazioni, quindi fare clic su una delle operazioni per visualizzare le informazioni sul progetto creato.
1. Fai clic su **[!UICONTROL Salva]** ![](assets/save-icon.png) nell&#39;angolo in basso a sinistra.
1. Vai a [!DNL Workfront] per visualizzare i progetti creati dallo scenario.

>[!TIP]
>
>Si consiglia di aggiungere note su ciascun modulo in modo facoltativo ma utile.
>
>1. Fai clic con il pulsante destro del mouse sul pulsante [!DNL Workfront] modulo, quindi fai clic su **[!UICONTROL Aggiungi una nota]**.
>1. Nella nota visualizzata, digita una panoramica per il modulo.

>
>   Questo è utile perché non dovrai aprire continuamente il modulo per vedere cosa fa. Puoi digitare qualcosa come &quot;Crea un progetto con Nome, Data inizio pianificata e Priorità mappate dal foglio di calcolo&quot;.
>
>   Per [!UICONTROL Fogli Google] modulo, puoi digitare qualcosa come &quot;Visualizza elenco progetti per nuove righe/progetti aggiunti&quot;.
>
>   È possibile aggiungere più note per un modulo.
>
>1. Chiudi **[!UICONTROL Note]** area.
>
>   Dopo aver aggiunto una nota a uno scenario, viene visualizzato un punto arancione **[!UICONTROL Note]** icona ![](assets/notes-icon-w-dot.png) nella parte inferiore dell&#39;editor dello scenario.
>
>1. Fai clic sul pulsante **[!UICONTROL Note]** icona ![](assets/notes-icon-w-dot.png) per visualizzare le note.

>




## Attiva lo scenario

Se si trattasse di uno scenario che utilizzeresti per dati reali, l&#39;ultima cosa che faresti è attivarlo. Dopo aver attivato uno scenario, per impostazione predefinita viene eseguito ogni 15 minuti. Puoi modificare questa impostazione definendo quando e con quale frequenza desideri che venga eseguita.

Per ulteriori informazioni sull&#39;attivazione degli scenari, vedi [Attivare o disattivare uno scenario in Adobe Workfront Fusion](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

Per informazioni sulle pianificazioni, consulta [Pianificare uno scenario in Adobe Workfront Fusion](../../workfront-fusion/scenarios/schedule-a-scenario.md).
