---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Crea uno scenario di automazione dell'esercitazione in [!DNL Adobe Workfront Fusion]
description: La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione. Questo articolo è stato dichiarato obsoleto, ma contiene un collegamento al nuovo articolo che descrive questa funzionalità.
author: Becky
feature: Workfront Fusion
exl-id: f6a6eb28-9b0b-48ea-af11-f55009a01178
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1562'
ht-degree: 0%

---

# Crea uno scenario di automazione dell&#39;esercitazione in [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione.
>
>Le informazioni contenute in questo articolo sono ora disponibili nell’articolo:
>
>* [Flusso di lavoro per la creazione di uno scenario](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/plan-a-scenario/create-a-scenario-workflow.html)
>
>Aggiorna eventuali segnalibri.
>
>Questo articolo non è più in fase di aggiornamento e verrà rimosso nel prossimo futuro.

Gli scenari di automazione automatizzano i processi Workfront, inclusa la manipolazione e la trasformazione dei dati. Questo articolo illustra il processo di creazione di uno scenario che cerca un progetto e quindi restituisce tutte le attività associate a tale progetto.

<!-- not sure why these are here?
For instructions on building an integration scenario that connects separate apps, see [Create a practice integration scenario in Adobe Workfront Fusion](../../workfront-fusion/get-started/create-a-practice-scenario.md).

For more information on functionality available with each Workfront Fusion license, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md).

-->

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
  <tbody>  
    <tr>  
      <td>piano Adobe Workfront</td>  
      <td>Qualsiasi</td>  
    </tr>  
    <tr>  
      <td>Licenza Adobe Workfront</td>  
      <td>
        Nuovo: Standard<br>
        Oppure<br>
        Corrente: Lavoro o versione successiva
      </td>  
    </tr>  
    <tr>  
      <td>Licenza Adobe Workfront Fusion</td>  
      <td> 
        Corrente: nessun requisito di licenza Workfront Fusion.<br>
        Oppure<br>
        Legacy: qualsiasi
      </td>  
    </tr>  
    <tr>  
      <td>Prodotto</td>  
      <td> 
        Nuovo: selezionare o Prime Workfront Plan: l’organizzazione deve acquistare Adobe Workfront Fusion.<br>
        Piano Ultimate Workfront: Workfront Fusion è incluso.<br>
        Oppure<br>
        Corrente: la tua organizzazione deve acquistare Adobe Workfront Fusion.
      </td>  
    </tr> 
  </tbody>  
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Per informazioni sulle [!DNL Adobe Workfront Fusion] licenze, vedere [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

+++

## Creare uno scenario di automazione

[!DNL Adobe Workfront Fusion] consente di concentrarsi su attività importanti automatizzando quelle ripetitive. Crea scenari che gestiscono automaticamente i dati tra varie app e servizi.

Ogni scenario è costituito da moduli che guidano il modo in cui i dati vengono elaborati all’interno di un’app o trasferiti tra app e servizi diversi. Ad esempio, è possibile creare uno scenario in Fusion per trovare automaticamente un progetto [!DNL Workfront] ed elencarne le attività. In questo modo, Fusion consente di risparmiare tempo e fatica gestendo le attività di routine.

Questa esercitazione consente di creare uno scenario in cui viene eseguita la ricerca di un progetto [!DNL Workfront] e vengono restituite le attività del progetto.

![](assets/create-practice-scenario-wf-only-350x157.png)

### Prima di iniziare

Crea un progetto con le attività in Workfront che puoi utilizzare per questo esercizio. Non è necessario eseguire alcuna configurazione aggiuntiva al di fuori dell’aggiunta di attività al progetto.

Per informazioni sulla creazione di un progetto in Workfront, consulta xxx.

### 1. Creare e denominare lo scenario

1. Accedi al tuo account [!DNL Workfront Fusion].
1. Fai clic su **[!UICONTROL Scenari]** ![](assets/scenarios-icon.png) nel pannello a sinistra.

   >[!NOTE]
   >
   >Se il pannello di navigazione a sinistra o le relative icone non sono visibili, fare clic sull&#39;icona Menu ![Menu](assets/main-menu-icon-left-nav.png).

1. Nel pannello [!UICONTROL **Cartelle**], fai clic sull&#39;icona ![](assets/add-folder-icon.png) di **[!UICONTROL Aggiungi cartella]**, quindi digita un nome come &quot;Scenari di esercitazione&quot; per la tua prima cartella.

1. Apri la cartella, quindi fai clic su **[!UICONTROL Crea un nuovo scenario]** nell&#39;angolo superiore destro della pagina.

1. Per questo esercizio, seleziona l&#39;app **[!DNL Adobe Workfront]**, quindi fai clic su **Cerca** nella parte inferiore.


1. Seleziona il nome del segnaposto **[!UICONTROL Nuovo scenario]** nell&#39;angolo superiore sinistro, quindi digita un nome come &quot;Esercitazione scenario 1&quot;.

   ![](assets/name-the-scenario.png)

1. Continua con [Connetti il primo modulo](#2-connect-the-first-module) di seguito.

### 2. Collegare il primo modulo

Ora devi stabilire una connessione autenticata al tuo account [!DNL Workfront]. Ogni modulo che aggiungi a uno scenario deve avere una connessione alla relativa app.

1. Nella casella **[!DNL Workfront]**, in **[!UICONTROL Connessione]**, fare clic su **[!UICONTROL Aggiungi]**, quindi digitare un nome per la connessione, ad esempio &quot;Account Workfront di Olivia&quot;, quindi fare clic su **[!UICONTROL Continua]**.
1. Autentica la connessione nella finestra visualizzata.

   Il processo di autenticazione di una connessione può variare leggermente da un’app all’altra. Il seguente processo è specifico di [!DNL Workfront], ma è simile a molte app:

   1. Immetti il dominio [!DNL Workfront], quindi fai clic su **[!UICONTROL Continua]**.
   1. Accedi a [!DNL Workfront].
   1. Esaminare l&#39;accesso richiesto da [!DNL Workfront Fusion], quindi fare clic su **[!UICONTROL Consenti accesso]**.

   Se hai bisogno di aiuto, consulta [Panoramica delle connessioni](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

### 3. Configurare il primo modulo

Dopo aver connesso [!DNL Workfront Fusion] all&#39;account [!DNL Workfront], è possibile specificare un progetto [!DNL Workfront] a cui si ha accesso e i dati che si desidera vengano elaborati dal primo modulo.

1. Nella casella [!UICONTROL Tipo di record] selezionare **[!UICONTROL Progetto]**. Questo imposta il modulo in modo che esegua la ricerca solo nei progetti.

   >[!TIP]
   >
   >Puoi trovare **[!UICONTROL Project]** nell&#39;elenco se inizi a digitare la parola &quot;[!UICONTROL project].&quot;

1. Nella casella **[!UICONTROL Set di risultati]** selezionare **[!UICONTROL Primo record corrispondente]**. In questo modo il modulo restituirà solo il primo record che soddisfa i criteri. Per questo esempio, è necessario restituire un solo record.
1. Nell&#39;area **[!UICONTROL Criteri di ricerca]** verrà impostato un filtro per restituire il progetto specifico:

   | Campo | Azione |
   |--------|-------------|
   | Campi dei criteri di ricerca | Seleziona il campo di cui desideri cercare i valori. Per questo esempio, selezionare **[!UICONTROL Nome]**. |
   | Criteri di ricerca | Nel primo menu a discesa, seleziona **[!UICONTROL Nome]**. |
   | Operatori di base | Nel secondo elenco a discesa, selezionare [!UICONTROL Contiene (senza distinzione maiuscole/minuscole)]. Questo consente al modulo di trovare i progetti il cui nome contiene le parole scelte, anche se non si inserisce il nome completo o si inserisce il nome con lettere maiuscole non corrette. |
   | Casella di testo | Immetti una parola o una frase che sai essere nel nome del progetto che stai cercando. |

+++ Espandi per visualizzare un esempio su schermo.
   ![](assets/search-name.png)
+++

1. Nell&#39;elenco **[!UICONTROL Output]** selezionare i campi che si desidera vengano generati dal modulo. Per questo esempio, selezionare i campi **[!UICONTROL ID]** e **[!UICONTROL Nome]**.

   >[!TIP]
   >
   >È possibile utilizzare **Cmd+F** ([!DNL Mac] OS) o **Ctrl-F** ([!DNL Windows] OS) per trovare rapidamente un campo.

1. Fare clic su **[!UICONTROL OK]**.

   >[!NOTE]
   >
   >Poiché non si tratta di un modulo trigger, non puoi scegliere dove avviarlo. Quando utilizzi un modulo trigger, ora puoi selezionare dove avviarlo.
   >
   >
   >Per ulteriori informazioni, vedere [Scegliere la posizione di inizio di un modulo trigger in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/choose-where-trigger-module-starts.md).

1. Fare clic con il pulsante destro del mouse sul modulo, scegliere **[!UICONTROL Rinomina]**, quindi digitare un nome che descriva le operazioni che si desidera vengano eseguite dal modulo, ad esempio &quot;Cerca progetto&quot;, quindi fare clic su **[!UICONTROL OK]**.

   Il nome viene visualizzato appena sotto il modulo. Di seguito, [!DNL Workfront Fusion] include una breve descrizione del tipo di azione eseguita dal modulo.

   ![](assets/module-renamed-wf.png)

1. Continua con [Aggiungi e configura il secondo modulo](#add-and-configure-the-second-module).

### 4. Aggiungere e configurare il secondo modulo

1. Fare clic sul cerchio parziale a destra del del modulo per **[!UICONTROL Aggiungere un altro modulo]**.
1. Selezionare [!DNL Workfront] dall&#39;elenco delle applicazioni, quindi scegliere il modulo di ricerca **[!UICONTROL Leggi record correlati]**.
1. Nella casella **[!UICONTROL Connessione]** selezionare la connessione creata per il modulo precedente. È necessario assicurarsi che questo modulo utilizzi la stessa connessione del modulo precedente.
1. Fai clic su **[!UICONTROL Tipo di record]**, quindi seleziona **[!UICONTROL Progetto]**, perché desideri leggere i record relativi a un progetto.

   >[!TIP]
   >
   >Puoi trovare **[!UICONTROL Progetto]** nell&#39;elenco se inizi a digitare la parola &quot;progetto&quot;.

1. Fare clic sul campo **[!UICONTROL ID record padre]**. Questo campo richiede l&#39;ID Workfront del progetto da cui si desidera restituire le attività.

   Facendo clic sul campo viene aperto l&#39;elenco delle variabili che è possibile utilizzare nel campo **[!UICONTROL ID record padre]** per identificare il progetto in Workfront.

   ![](assets/list-of-available-variables-wf-350x368.png)

1. Fare clic sulla variabile **[!UICONTROL ID]** per aggiungerla al campo **[!UICONTROL ID record padre]**. Questo consente di utilizzare l’ID restituito dal primo modulo come identificatore del progetto con cui vuoi lavorare nel secondo modulo, in modo che le attività restituite appartengano a quel progetto.
1. Nel campo **[!UICONTROL Raccolte]**, seleziona **[!UICONTROL Attività]**. Questo indica che il modulo deve restituire le attività associate al progetto scelto.
1. Nel campo **[!UICONTROL Output]**, selezionare **[!UICONTROL Id]** e **[!UICONTROL Nome]**.
1. Fai clic su **[!UICONTROL OK]**

   Ora avete uno scenario di lavoro.

1. Assegna al secondo modulo un nome come &quot;Attività di ritorno associate al progetto&quot;, quindi continua con [Verifica lo scenario](#test-the-scenario).

## Verifica lo scenario

Prima di attivare lo scenario, è importante testarlo eseguendolo almeno una volta e visualizzando i risultati. Questo ti aiuta a capire come i dati scorrono attraverso lo scenario e a trovare eventuali errori.

Abbiamo scelto di restituire 1 progetto e le attività associate a quel progetto. Se esegui lo scenario, questo è ciò che dovrebbe accadere.

1. Fai clic su **[!UICONTROL Esegui una volta]** nell&#39;angolo inferiore sinistro dell&#39;editor scenari.
1. Al termine dell’esecuzione dello scenario, fai clic sulla bolla sopra il primo modulo.

   ![](assets/click-bubble.png)

   Nella casella visualizzata, puoi visualizzare informazioni sul bundle di dati elaborati dal modulo, inclusi i dati effettivi estratti dal progetto restituito dal modulo.

   ![](assets/execution-inspector-wf-only-first-350x423.png)

1. Fare clic sull&#39;indicatore del controllo di esecuzione sopra il secondo modulo per visualizzare l&#39;input delle informazioni e l&#39;output, ovvero una raccolta di attività contenute nel progetto.

   ![](assets/execution-inspector-wf-only-second-350x738.png)

   Per ulteriori informazioni su come leggere le informazioni sull’esecuzione di uno scenario, consulta i seguenti articoli:

   * Per informazioni generali, vedere [Flusso di esecuzione dello scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).
   * Per informazioni sui bundle elaborati, vedere [Esecuzione scenario, cicli e fasi in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

1. In [!DNL Workfront Fusion], fai clic su **[!UICONTROL Salva]** ![](assets/save-icon.png) nell&#39;angolo inferiore sinistro per salvare l&#39;avanzamento dello scenario.

   >[!IMPORTANT]
   >
   >Risparmia spesso quando affili e testa uno scenario.

>[!TIP]
>
>È consigliabile aggiungere note su ciascun modulo in modo facoltativo ma utile.
>
>1. Fare clic con il pulsante destro del mouse su un modulo di [!DNL Workfront], quindi scegliere **[!UICONTROL Aggiungi nota]**.
>1. Nella nota visualizzata, digita una panoramica del modulo.
>
>    È possibile aggiungere più note per un modulo.
>
>1. Chiudi l&#39;area **[!UICONTROL Note]**.
>
>     Dopo aver aggiunto una nota a uno scenario, un punto arancione viene visualizzato sull&#39;icona **[!UICONTROL Note]** ![](assets/notes-icon-w-dot.png) nella parte inferiore dell&#39;editor dello scenario.
>
>1. Fai clic sull&#39;icona **[!UICONTROL Note]** ![](assets/notes-icon-w-dot.png) per visualizzare le note.
>

## Attiva lo scenario

Questo scenario di esempio non ha un modulo trigger. Se si trattasse di uno scenario da utilizzare per dati reali, inizierebbe con un modulo trigger e l’ultima cosa da fare è attivarlo. Dopo aver attivato uno scenario, per impostazione predefinita viene eseguito ogni 15 minuti. Puoi modificare questa impostazione definendo quando e con quale frequenza desideri che venga eseguita.

Per ulteriori informazioni sull&#39;attivazione degli scenari, vedere [Attivare o disattivare uno scenario in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

Per informazioni sulle pianificazioni, vedere [Pianificare uno scenario in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).
