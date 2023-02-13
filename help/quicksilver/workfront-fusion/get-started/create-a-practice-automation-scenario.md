---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Crea uno scenario di automazione pratica in [!DNL Adobe Workfront Fusion]
description: Questo articolo descrive come creare uno scenario di automazione con Adobe Workfront Fusion. Gli scenari di automazione automatizzano i processi di Workfront, inclusi la manipolazione e la trasformazione dei dati. In questo esempio viene descritto il processo di creazione di uno scenario per la ricerca di un progetto e vengono quindi restituite tutte le attività associate a tale progetto.
author: Becky
feature: Workfront Fusion
exl-id: f6a6eb28-9b0b-48ea-af11-f55009a01178
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '1782'
ht-degree: 0%

---

# Crea uno scenario di automazione pratica in [!DNL Adobe Workfront Fusion]

Questo articolo descrive come creare uno scenario di automazione con Adobe Workfront Fusion. Gli scenari di automazione automatizzano i processi di Workfront, inclusi la manipolazione e la trasformazione dei dati. In questo esempio viene descritto il processo di creazione di uno scenario per la ricerca di un progetto e vengono quindi restituite tutte le attività associate a tale progetto.

Per istruzioni su come creare uno scenario di integrazione per la connessione di app separate, vedi [Creare uno scenario di integrazione pratica in Adobe Workfront Fusion](../../workfront-fusion/get-started/create-a-practice-scenario.md).

Per ulteriori informazioni sulle funzionalità disponibili con ciascuna licenza Workfront Fusion, vedi [Licenze Adobe Workfront Fusion](../../workfront-fusion/get-started/license-automation-vs-integration.md).

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p><p>[!UICONTROL [!DNL Workfront Fusion] per automazione del lavoro</p>  </td> 
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
Questo esempio illustra il processo di creazione di uno scenario che cerca un [!DNL Workfront] e restituisce le attività nel progetto.

![](assets/create-practice-scenario-wf-only-350x157.png)

La creazione di uno scenario è costituita da diverse attività principali:

## Scegli le app e assegna un nome allo scenario

1. Accedi al tuo [!DNL Workfront Fusion] conto.
1. Fai clic su **[!UICONTROL Scenari]** ![](assets/scenarios-icon.png) nel pannello a sinistra.

   Nel pannello a sinistra visualizzato, puoi organizzare gli scenari in cartelle.

   Nella parte superiore dell&#39;area principale a destra, è possibile visualizzare **[!UICONTROL Tutto]** scenari creati, **[!UICONTROL Scenari attivi]**, **[!UICONTROL Scenari inattivi]** e **[!UICONTROL Concetti]**. I concetti sono scenari che necessitano di altro lavoro prima [!DNL Workfront Fusion] possono classificarli come attivi o inattivi.

   ![](assets/scenarios-left-panel-350x215.png)

1. Nel pannello a sinistra, fai clic sul pulsante **[!UICONTROL Aggiungi cartella]** icona ![](assets/add-folder-icon.png), quindi digita un nome come &quot;Scenari di esercitazione&quot; per la prima cartella.

1. Apri la cartella, quindi fai clic su **[!UICONTROL Creare un nuovo scenario]** nell’angolo superiore destro della pagina.

   La pagina di destinazione visualizzata ti consente di precaricare le app che desideri utilizzare nello scenario da generare.

1. Per questo esercizio, cerca e seleziona la **[!DNL Workfront]** app.
1. Fai clic su **[!UICONTROL Continua]** nell&#39;angolo in alto a destra.

   Viene visualizzato l’editor dello scenario, contenente un modulo vuoto al centro, il [!DNL Workfront] app precaricata e alcune opzioni nella barra degli strumenti in basso.

   ![](assets/scenario-editor-350x235.png)

   Quando si inizia a creare un nuovo scenario, è bene iniziare creando un nome per esso.

1. Seleziona la **[!UICONTROL Nuovo scenario]** nome del segnaposto nell&#39;angolo in alto a sinistra, quindi digitare un nome come &quot;Scenario di esercitazione 1&quot;.
1. Continua con [Aggiungi e configura il primo modulo](#add-and-configure-the-first-module) sotto.

## Aggiungi e configura il primo modulo

Il modulo vuoto con punto interrogativo rappresenta il modulo trigger da aggiungere. Questo modulo avvierà lo scenario ogni volta che viene eseguito. L’icona dell’orologio nel modulo vuoto indica che si tratta di un modulo pianificato.

![](assets/empty-module.png)

Questo modulo conterrà i dati per i quali si desidera che lo scenario venga controllato.

Per questo esempio, non stiamo utilizzando un modulo trigger. Invece, questo scenario inizia con una ricerca.

1. Fai clic sul modulo vuoto per scegliere l’app da cui selezionare un modulo.

   L’app precaricata viene visualizzata accanto al modulo vuoto. Puoi aggiungere qualsiasi altra app con moduli utilizzando [!UICONTROL Ricerca] scatola.

   ![](assets/pre-loaded-app-wf-350x172.png)

1. Clic **[!DNL Workfront]**.

   L’elenco viene modificato per visualizzare tutti [!DNL Workfront] moduli utilizzabili come modulo trigger.

1. Fai clic sul modulo di ricerca **[!UICONTROL Ricerca]**.

   Ora è necessario stabilire una connessione autenticata al [!DNL Workfront] conto. Ogni modulo che aggiungi a uno scenario deve avere una connessione alla relativa app.

1. In **[!DNL Workfront]** box, sotto **[!UICONTROL Connessione]**, fai clic su **[!UICONTROL Aggiungi]**, quindi digita un nome per la connessione, ad esempio &quot;l&#39;account Workfront di Olivia&quot;, quindi fai clic su **[!UICONTROL Continua]**.
1. Autentica la connessione nella finestra visualizzata.

   Il processo di autenticazione di una connessione può variare un po&#39; tra le app. Il seguente processo è specifico per [!DNL Workfront], ma il processo è simile a molte app.

   1. Inserisci il tuo [!DNL Workfront] dominio, quindi fai clic su **[!UICONTROL Continua]**.
   1. Accedi a [!DNL Workfront].
   1. Esamina l’accesso che [!DNL Workfront Fusion] richiede, quindi fai clic su **[!UICONTROL Consenti accesso]**.

   Se hai bisogno di aiuto, consulta [Informazioni sulla connessione [!DNL Adobe Workfront Fusion] a un&#39;app o a un servizio](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

## Configura il primo modulo

Dopo la connessione [!DNL Workfront Fusion] al tuo [!DNL Workfront] è possibile specificare un [!DNL Workfront] richiedi la coda di accesso e i dati a cui desideri che il primo modulo possa elaborare.

1. In [!UICONTROL Tipo di record] casella, seleziona **[!UICONTROL Progetto]**. In questo modo il modulo viene impostato per cercare solo i progetti.

   >[!TIP]
   >
   >È possibile trovare **[!UICONTROL Progetto]** nell&#39;elenco se si inizia a digitare la parola &quot;[!UICONTROL progetto].&quot;

1. In **[!UICONTROL Set di risultati]** casella, seleziona **[!UICONTROL Primo record corrispondente]**. In questo modo il modulo restituisce solo il primo record trovato che soddisfa i criteri. Per questo esempio, è necessario restituire un solo record.
1. In **[!UICONTROL Criteri di ricerca]** verrà impostato un filtro per restituire il progetto specifico.

   1. Nella prima casella sotto [!UICONTROL Criteri di ricerca], seleziona il campo di cui desideri cercare i valori. Per questo esempio, seleziona **[!UICONTROL Nome]**.
   1. Per l’operatore, seleziona [!UICONTROL Contiene (senza distinzione maiuscole/minuscole)]. Questo consente al modulo di trovare progetti con le parole selezionate nel nome, anche se non si immette l’intero nome, o di inserire il nome con l’maiuscolo (ad esempio tutti i maiuscoli).
   1. Nell&#39;ultimo campo in [!UICONTROL Criteri di ricerca], immetti una parola o una frase che sai essere nel nome del progetto che stai cercando.

1. In **[!UICONTROL Uscite]** seleziona i campi che desideri vengano generati dal problema. Per questo esempio, seleziona la **[!UICONTROL ID]** e **[!UICONTROL Nome]** campi.

   >[!TIP]
   >
   >È possibile utilizzare **Comando+F** ([!DNL Mac] OS) o **Ctrl+F** ([!DNL Windows] OS) per trovare rapidamente un campo.

1. Fai clic su **[!UICONTROL OK]**.

   >[!NOTE]
   >
   >(Solo informativo) Poiché non si tratta di un modulo trigger, non è possibile scegliere dove avviarlo. Quando utilizzi un modulo trigger, ora selezioni dove avviarlo.
   >
   >
   >Per ulteriori informazioni, consulta [Scegli dove inizia il modulo trigger [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/choose-where-trigger-module-starts.md).

1. Fai clic con il pulsante destro del mouse sul modulo e fai clic su **[!UICONTROL Rinomina]**, quindi digita un nome che descriva le operazioni che desideri eseguire dal modulo (ad esempio &quot;Cerca progetto&quot;), quindi fai clic su **[!UICONTROL OK]**.

   Il nome viene visualizzato sotto il modulo. Sotto questo, [!DNL Workfront Fusion] include una breve descrizione del tipo di azione eseguita dal modulo.

   ![](assets/module-renamed-wf.png)

1. Continua con [Aggiungi e configura il secondo modulo](#add-and-configure-the-second-module).

## Aggiungi e configura il secondo modulo

1. Fai clic sul cerchio parziale a destra del modulo a **[!UICONTROL Aggiungi un altro modulo]**.
1. Seleziona [!DNL Workfront] dall&#39;elenco delle applicazioni, quindi scegliere il modulo di ricerca **[!UICONTROL Leggi record correlati]**.
1. È già stata creata una connessione a [!DNL Workfront] per il modulo precedente. Non è necessario crearlo di nuovo qui, ma è necessario assicurarsi che questo modulo utilizzi la stessa connessione del modulo precedente.\
   In **[!UICONTROL Connessione]** selezionare la connessione creata per il modulo precedente.
1. Fai clic su **[!UICONTROL Tipo di record]**, quindi seleziona **[!UICONTROL Progetto]** perché vogliamo leggere i record relativi a un progetto.

   >[!TIP]
   >
   >È possibile trovare **[!UICONTROL Progetto]** nell&#39;elenco se si inizia a digitare la parola &quot;progetto&quot;.

1. Fai clic sul pulsante **[!UICONTROL ID record padre]** campo . Questo campo richiede l’ID Workfront del progetto da cui si desidera restituire le attività.

   Fai clic sul campo per aprire l’elenco delle variabili utilizzabili in **[!UICONTROL ID record padre]** per identificare il progetto in Workfront.

   ![](assets/list-of-available-variables-wf-350x368.png)

1. Fai clic sulla variabile **[!UICONTROL ID]** per aggiungerlo al **[!UICONTROL ID record padre]** campo . Questo consente di utilizzare l’ID restituito dal primo modulo come identificatore del progetto con cui si desidera lavorare nel secondo modulo, in modo che le attività restituite appartengano a quel progetto.
1. In **[!UICONTROL Raccolte]** campo , seleziona **[!UICONTROL Attività]**. Indica che il modulo deve restituire le attività associate al progetto selezionato.
1. Fai clic su **[!UICONTROL OK]**

   Ora avete uno scenario di lavoro.

1. Assegna al secondo modulo un nome, ad esempio &quot;Restituisci le attività associate al progetto&quot;, quindi continua con [Verificare lo scenario](#test-the-scenario).

## Verificare lo scenario

Prima di attivare lo scenario, è importante testarlo eseguendo almeno una volta e visualizzando i risultati. Questo ti aiuta a capire come i dati scorrono nello scenario e trovare eventuali errori.

Abbiamo scelto di restituire 1 progetto, così come le attività associate a tale progetto. Se esegui lo scenario, questo è ciò che dovrebbe accadere.

1. Fai clic su **[!UICONTROL Esegui una volta]** nell’angolo in basso a sinistra dell’editor di scenari.
1. Al termine dell&#39;esecuzione dello scenario, fai clic sulla bolla sopra il primo modulo.

   ![](assets/click-bubble.png)

   Nella casella visualizzata, puoi visualizzare informazioni sul bundle di dati elaborato dal modulo, compresi i dati effettivi estratti dal progetto restituito dal modulo.

   ![](assets/execution-inspector-wf-only-first-350x423.png)

1. Fare clic sulla bolla dell&#39;ispettore di esecuzione sopra il secondo modulo per visualizzare l&#39;input delle informazioni e l&#39;output, ovvero una raccolta di attività contenute nel progetto.

   ![](assets/execution-inspector-wf-only-second-350x738.png)

   Per ulteriori informazioni su come leggere le informazioni sull’esecuzione di scenari, consulta i seguenti articoli:

   * Per informazioni generali, consulta [Flusso di esecuzione dello scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).
   * Per informazioni sui bundle elaborati, vedi [Esecuzione di scenari, cicli e fasi in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

1. In [!DNL Workfront Fusion], fai clic su **[!UICONTROL Salva]** ![](assets/save-icon.png) nell’angolo in basso a sinistra per salvare l’avanzamento dello scenario.

   >[!IMPORTANT]
   >
   >Puoi salvare spesso durante l’elaborazione e il test di uno scenario.

>[!TIP]
>
>Si consiglia di aggiungere note su ciascun modulo in modo facoltativo ma utile.
>
>1. Fai clic con il pulsante destro del mouse su un [!DNL Workfront] modulo, quindi fai clic su **[!UICONTROL Aggiungi una nota]**.
>1. Nella nota visualizzata, digita una panoramica per il modulo.

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

Questo scenario di esempio non dispone di un modulo trigger. Se si trattasse di uno scenario che utilizzeresti per dati reali, inizierebbe con un modulo trigger, e l&#39;ultima cosa che faresti è attivarlo. Dopo aver attivato uno scenario, per impostazione predefinita viene eseguito ogni 15 minuti. Puoi modificare questa impostazione definendo quando e con quale frequenza desideri che venga eseguita.

Per ulteriori informazioni sull&#39;attivazione degli scenari, vedi [Attiva o disattiva uno scenario in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

Per informazioni sulle pianificazioni, consulta [Pianifica uno scenario in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).
