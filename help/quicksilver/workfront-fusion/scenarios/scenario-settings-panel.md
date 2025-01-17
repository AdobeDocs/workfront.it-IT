---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Pannello delle impostazioni dello scenario in Adobe Workfront Fusion
description: La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione. Questo articolo è stato dichiarato obsoleto, ma contiene un collegamento al nuovo articolo che descrive questa funzionalità.
author: Becky
feature: Workfront Fusion
exl-id: 64a7a39a-f450-4eba-b4db-f31dd22aefdc
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1266'
ht-degree: 0%

---

# Pannello impostazioni scenario in [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione.
>
>Le informazioni contenute in questo articolo sono ora disponibili nell’articolo:
>
>* [Configura impostazioni scenario](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/configure-scenario-settings/configure-scenario-settings.html)
>
>Aggiorna eventuali segnalibri.
>
>Questo articolo non è più in fase di aggiornamento e verrà rimosso nel prossimo futuro.

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
   <p>Requisito licenza legacy: [!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione lavoro], [!UICONTROL [!DNL Workfront Fusion] per automazione lavoro]</p>
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

## Apri le impostazioni dello scenario

1. Aprire l&#39;editor dello scenario, come spiegato in [Editor dello scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-editor.md).
1. Fai clic sull’icona a forma di ingranaggio nell’angolo inferiore sinistro della pagina.

   ![](assets/scenario-settings-350x221.png)

   Nel pannello [!UICONTROL Impostazioni scenario] visualizzato, puoi configurare varie impostazioni avanzate per lo scenario.

## [!UICONTROL Consenti l&#39;archiviazione di esecuzioni incomplete]

Questa opzione determina il modo in cui [!DNL Adobe Workfront Fusion] procede se si verifica un errore durante l&#39;esecuzione di uno scenario. Con questa opzione abilitata, lo scenario viene sospeso e spostato in [Visualizza e risolve le esecuzioni incomplete in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md). Questo consente di risolvere il problema e continuare l’esecuzione dal punto in cui lo scenario è stato interrotto. Se questa opzione è disabilitata, l’esecuzione dello scenario si interrompe e viene avviata una fase di rollback.

## [!UICONTROL Elaborazione sequenziale]

Questa opzione forza tutte le esecuzioni in ordine ed è principalmente rilevante per i webhook e per le esecuzioni incomplete.

Quando l’elaborazione sequenziale è abilitata, le esecuzioni parallele dello scenario vengono disabilitate.

### Webhook istantanei

Se un trigger del webhook è configurato come `instant` e &quot;Elaborazione sequenziale&quot; è abilitata, tutti i payload istantanei del webhook verranno messi in coda ed elaborati nell&#39;ordine in cui arrivano. Questo può essere utile quando si elaborano eventi da sistemi esterni in un ordine esatto.

>[!NOTE]
>
>Si verificheranno ritardi di elaborazione automatici quando ogni payload viene elaborato prima dell’avvio del successivo.

### Esecuzioni incomplete

Se è abilitata anche l’opzione &quot;Esecuzioni incomplete&quot;, se si verifica un errore durante l’esecuzione di uno scenario, quest’ultimo viene messo in pausa. Si verifica quindi una delle seguenti situazioni:

* Se l&#39;opzione di elaborazione sequenziale è **enabled**, Workfront Fusion interrompe l&#39;elaborazione della sequenza preesistente fino alla risoluzione di tutte le esecuzioni incomplete.
* Se l&#39;opzione di elaborazione sequenziale è **disabilitata**, lo scenario continua a essere eseguito in base alla pianificazione, accompagnata da ripetuti tentativi di eseguire nuovamente le esecuzioni incomplete.

Per ulteriori informazioni sulle esecuzioni incomplete, vedere [Visualizzare e risolvere le esecuzioni incomplete in Adobe Workfront Fusion](/help/quicksilver/workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

<!--

This option determines how [!DNL Workfront Fusion] proceeds if an error occurs and the execution of a scenario is moved to the [View and resolve incomplete executions in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md). If the [!UICONTROL Sequential processing] option is enabled, Workfront Fusion stops processing the task sequence altogether until all incomplete executions are resolved. If the [!UICONTROL Sequential processing] option is disabled, the scenario continues to run according to its schedule, accompanied by repeated attempts to rerun the incomplete executions.-->

>[!NOTE]
>
>L’elaborazione sequenziale può causare un ritardo nell’esecuzione di uno scenario. Se vi sono ancora esecuzioni incomplete nella coda quando si attiva uno scenario immediato o quando uno scenario pianificato è impostato per l’esecuzione, tale scenario verrà eseguito dopo che tutte le esecuzioni prima di essere nella coda sono state completate.
>
>Se il caso di utilizzo per gli scenari non richiede l’elaborazione sequenziale, si consiglia di disabilitare l’opzione di elaborazione sequenziale.

Per ulteriori informazioni sulla pianificazione, vedere [Pianificare uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).

## I dati sono riservati

Una volta eseguito uno scenario, per impostazione predefinita puoi visualizzare informazioni sui dati elaborati dai moduli nello scenario. Se non si desidera archiviare queste informazioni, abilitare l&#39;opzione [!UICONTROL Dati riservati].

Per ulteriori informazioni sulla visualizzazione delle informazioni, vedere [Flusso di esecuzione dello scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).

>[!IMPORTANT]
>
>Se abiliti questa opzione, potrebbe essere difficile risolvere gli errori che possono verificarsi durante l’esecuzione di uno scenario.

## Abilita perdita di dati

Questa opzione ha a che fare con l&#39;abilitazione della perdita di dati se [!DNL Workfront Fusion] non riesce a salvare un bundle nella coda di [Visualizza e risolvere le esecuzioni incomplete in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md) (ad esempio, a causa di una mancanza di spazio libero). Se questa opzione è abilitata, i dati vengono persi per evitare interruzioni nell’esecuzione complessiva dello scenario. Questo è utile per gli scenari in cui la priorità più alta è l’esecuzione continua e i dati errati in arrivo non sono così importanti.

Inoltre, durante l’esecuzione di uno scenario, a volte un modulo può incontrare un file di dimensioni superiori alla dimensione massima consentita. In questo caso, [!DNL Workfront Fusion] procede in conformità con l&#39;impostazione dell&#39;opzione [!UICONTROL Abilita perdita di dati] e viene visualizzato un messaggio di avviso.

Per ulteriori informazioni sulle dimensioni massime dei file, vedere [Informazioni sui file di mapping in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/about-mapping-files.md).

Per ulteriori informazioni sugli avvisi, vedere [Errore di elaborazione in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

## [!UICONTROL Commit automatico]

Le impostazioni di [!UICONTROL Auto commit] si applicano alle transazioni e definiscono la modalità di elaborazione di uno scenario. Se l&#39;opzione Auto commit è attiva, la fase di commit su ciascun modulo inizia immediatamente dopo il completamento della fase operativa. Se l&#39;opzione Auto commit è disattivata, non viene eseguito alcun commit finché non vengono eseguite operazioni per tutti i moduli (questa è la modalità predefinita).

Per ulteriori informazioni sulle transazioni, vedere [Esecuzione dello scenario, cicli e fasi in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

## Numero massimo di cicli

L&#39;impostazione di più cicli può essere utile quando si desidera evitare l&#39;interruzione della connessione a un servizio di terze parti e assicurarsi che tutti i record vengano elaborati nell&#39;ambito dell&#39;esecuzione dello scenario.

* Se lo scenario inizia con un trigger di polling, l’impostazione definisce il numero massimo di cicli consentiti durante l’esecuzione dello scenario.

  Per ulteriori informazioni sui trigger di polling, vedere [trigger di polling](../../workfront-fusion/modules/module-types.md#polling) in [Tipi di moduli](../../workfront-fusion/modules/module-types.md).

* Se lo scenario inizia con un trigger immediato, l’impostazione viene ignorata e tutti gli eventi in sospeso vengono elaborati durante l’esecuzione di un singolo scenario, un evento per ogni ciclo.

  Per ulteriori informazioni sui trigger istantanei, vedere [Trigger istantanei](../../workfront-fusion/modules/module-types.md#instant) in [Tipi di moduli](../../workfront-fusion/modules/module-types.md).

* Se lo scenario non inizia con un trigger (istantaneo/polling), viene sempre eseguito il numero massimo specificato di cicli.

>[!INFO]
>
>**Esempi:** [!DNL Workfront] > [!UICONTROL Osserva il record] verifica la presenza di nuovi problemi e [!DNL Workfront] >[!UICONTROL Converti oggetto] converte la nuova richiesta in un progetto e le assegna il modello appropriato.
>
>![](assets/scenario-settings-ex-1-350x157.png)
>
>L&#39;impostazione [!UICONTROL altri cicli] viene applicata solo quando si pianifica l&#39;esecuzione dello scenario. Quando si utilizza il pulsante [!UICONTROL Esegui una volta], vengono prese in considerazione le impostazioni del ciclo.
>
>### Il numero massimo di cicli è impostato su 1 (impostazione predefinita)
>
>![](assets/max-number-cycles-1-350x201.png)
>
>Il numero massimo di file restituiti [!UICONTROL nel modulo [!UICONTROL Workfront] >[!UICONTROL Osserva record] è impostato su `10`.]
>Se vengono inviate 100 richieste a [!DNL Workfront] e il campo [!UICONTROL Limit] è impostato su 10, 90 file vengono lasciati non elaborati dopo l&#39;esecuzione di uno scenario. I successivi 10 file vengono elaborati nella successiva esecuzione pianificata dello scenario.
>
>### Numero massimo di cicli impostato su 10
>
>Il numero massimo di file restituiti [!UICONTROL nel modulo [!UICONTROL Dropbox] >[!UICONTROL File di controllo] è impostato su `10`.]
>
>Se vengono aggiunti 100 file alla cartella di Dropbox e l&#39;opzione [!UICONTROL Numero massimo di file restituiti] è impostata su 10, vengono elaborati 10 file durante il primo ciclo, i successivi 10 file nel secondo ciclo, i successivi 10 file nel terzo ciclo e così via, fino a quando tutti i file non vengono elaborati.
>
>Tutti i file vengono elaborati entro 1 esecuzione dello scenario.
>
>Puoi visualizzare i cicli già eseguiti nei dettagli dello scenario:
>
>![](assets/scenario-detail-350x207.png)
>
>Per ulteriori informazioni su questa pagina, vedere [Dettagli scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-detail.md).

## Numero di errori consecutivi

Definisce il numero massimo di tentativi di esecuzione consecutivi prima che l&#39;esecuzione di uno scenario venga disattivata (esclusi [!UICONTROL DataError], [!UICONTROL DuplicateDataError] e [!UICONTROL ConnectionError]).

Per ulteriori informazioni sugli errori, vedere [Errore di elaborazione in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

>[!NOTE]
>
>Se uno scenario inizia con un trigger immediato, l’impostazione viene ignorata e lo scenario viene disattivato immediatamente dopo il primo errore.
