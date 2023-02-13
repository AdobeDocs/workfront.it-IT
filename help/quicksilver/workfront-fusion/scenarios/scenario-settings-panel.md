---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Pannello delle impostazioni dello scenario in Adobe Workfront Fusion
description: Questo articolo descrive le impostazioni disponibili nel [!UICONTROL impostazioni dello scenario] nel pannello [!DNL Adobe Workfront Fusion] scenari.
author: Becky
feature: Workfront Fusion
exl-id: 64a7a39a-f450-4eba-b4db-f31dd22aefdc
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '968'
ht-degree: 0%

---

# Il pannello delle impostazioni dello scenario in [!DNL Adobe Workfront Fusion]

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p><p>[!UICONTROL [!DNL Workfront Fusion] per automazione del lavoro </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</td> 
  </tr> 
 </tbody> 
</table>

Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, vedi [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Apri le impostazioni dello scenario

1. Apri l’editor dello scenario, come spiegato in [Editor di scenari in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-editor.md).
1. Fai clic sull’icona a forma di ingranaggio vicino all’angolo inferiore sinistro della pagina.

   ![](assets/scenario-settings-350x221.png)

   In [!UICONTROL Impostazioni dello scenario] pannello visualizzato, è possibile configurare diverse impostazioni avanzate per lo scenario.

## [!UICONTROL Consenti archiviazione esecuzioni incomplete]

Questa opzione determina il modo in cui [!DNL Adobe Workfront Fusion] procede se si verifica un errore durante l’esecuzione di uno scenario. Con questa opzione abilitata, lo scenario viene messo in pausa e spostato in [Visualizzare e risolvere le esecuzioni incomplete in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md). Questo ti dà la possibilità di risolvere il problema e continuare a eseguire da dove lo scenario è stato interrotto. Se questa opzione è disabilitata, l&#39;esecuzione dello scenario si interrompe e viene avviata una fase di rollback.

## [!UICONTROL Elaborazione sequenziale]

Questa opzione determina il modo in cui [!DNL Workfront Fusion] procede se si verifica un errore e l’esecuzione di uno scenario viene spostata in [Visualizzare e risolvere le esecuzioni incomplete in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md). Se la [!UICONTROL Elaborazione sequenziale] è abilitata, Workfront Fusion smette di elaborare completamente la sequenza di attività fino a quando tutte le esecuzioni incomplete non vengono risolte. Se la [!UICONTROL Elaborazione sequenziale] è disabilitata, lo scenario continua a essere eseguito in base alla sua pianificazione, accompagnato da ripetuti tentativi di eseguire nuovamente le esecuzioni incomplete.

Per ulteriori informazioni sulla pianificazione, vedi [Pianifica uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).

## I dati sono confidenziali

Una volta eseguito uno scenario, puoi visualizzare per impostazione predefinita le informazioni sui dati elaborati dai moduli nello scenario. Se non desideri memorizzare queste informazioni, abilita la [!UICONTROL I dati sono confidenziali] opzione .

Per ulteriori informazioni sulla visualizzazione delle informazioni, consulta [Flusso di esecuzione dello scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).

>[!IMPORTANT]
>
>Se si abilita questa opzione, potrebbe essere difficile risolvere gli errori che possono verificarsi durante l’esecuzione di uno scenario.

## Abilita perdita dati

Questa opzione ha a che fare con l&#39;abilitazione della perdita di dati se [!DNL Workfront Fusion] impossibile salvare un bundle nella coda di [Visualizzare e risolvere le esecuzioni incomplete in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md) (ad esempio, a causa della mancanza di spazio libero). Con questa opzione abilitata, i dati vengono persi per evitare interruzioni nell’esecuzione complessiva dello scenario. Ciò è utile per gli scenari in cui la priorità più elevata è l’esecuzione continua e i dati errati in arrivo non sono così importanti.

Oltre a ciò, durante l’esecuzione di uno scenario, un modulo può a volte incontrare un file di dimensioni maggiori della dimensione massima consentita. In questo caso, [!DNL Workfront Fusion] i proventi in conformità della definizione [!UICONTROL Abilita perdita dati] e viene visualizzato un messaggio di avviso.

Per ulteriori informazioni sulle dimensioni massime dei file, consulta [Informazioni sulla mappatura dei file in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/about-mapping-files.md).

Per ulteriori informazioni sugli avvisi, consulta [Errore di elaborazione in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

## [!UICONTROL commit automatico]

La [!UICONTROL commit automatico] Le impostazioni si applicano alle transazioni e definiscono il modo in cui elaborare uno scenario. Se l&#39;opzione di commit automatico è attivata, la fase di commit su ciascun modulo viene avviata immediatamente dopo il completamento della fase operativa. Se l’opzione di commit automatico è disabilitata, non si verifica alcun commit finché non vengono eseguite le operazioni per tutti i moduli (questa è la modalità predefinita).

Per ulteriori informazioni sulle transazioni, vedi [Esecuzione di scenari, cicli e fasi in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

## Numero massimo di cicli

L’impostazione di più cicli può essere utile quando si desidera evitare l’interruzione della connessione a un servizio di terze parti e assicurarsi che tutti i record vengano elaborati nell’ambito dell’esecuzione di un unico scenario.

* Se lo scenario inizia con un trigger di polling, l’impostazione definisce il numero massimo di cicli consentiti durante l’esecuzione dello scenario.

   Per ulteriori informazioni sui trigger di polling, vedi [Trigger di polling](../../workfront-fusion/modules/module-types.md#polling) in [Tipi di moduli](../../workfront-fusion/modules/module-types.md).

* Se lo scenario inizia con un trigger immediato, l’impostazione viene ignorata e tutti gli eventi in sospeso vengono elaborati durante un’esecuzione di un singolo scenario, un evento per ogni ciclo.

   Per ulteriori informazioni sugli attivatori istantanei, vedi [Trigger istantanei](../../workfront-fusion/modules/module-types.md#instant) in [Tipi di moduli](../../workfront-fusion/modules/module-types.md).

* Se lo scenario non inizia con un trigger (istantaneo/polling), viene sempre eseguito il numero massimo specificato di cicli.

>[!INFO]
>
>**Esempi:**  [!DNL Workfront] > [!UICONTROL Record di controllo] osserva i nuovi problemi che entrano in gioco, e [!DNL Workfront] >[!UICONTROL Converti oggetto] converte la nuova richiesta in un progetto e le assegna il modello appropriato.
>
>![](assets/scenario-settings-ex-1-350x157.png)
>
>A [!UICONTROL più cicli] viene applicata solo quando pianifichi l&#39;esecuzione dello scenario. Quando utilizzi la [!UICONTROL Esegui una volta] le impostazioni del ciclo sono prese in considerazione.
>
>### Il numero massimo di cicli è impostato su 1 (impostazione predefinita)
>
>![](assets/max-number-cycles-1-350x201.png)
>
>La [!UICONTROL Numero massimo di file restituiti] in [!UICONTROL Dropbox] >[!UICONTROL File di controllo] il modulo è impostato su `10`.
>
>![](assets/max-number-cycles-10-350x175.png)
>
>Se 100 richieste sono presentate a [!DNL Workfront]e [!UICONTROL Limite] Il campo è impostato su 10, quindi 90 file non vengono elaborati dopo un&#39;esecuzione di scenario. I 10 file successivi vengono elaborati nell’esecuzione successiva dello scenario pianificato.
>
>### Numero massimo di cicli impostato su 10
>
>La [!UICONTROL Numero massimo di file restituiti] in [!UICONTROL Dropbox] >[!UICONTROL File di controllo] il modulo è impostato su `10`.
>
>Se 100 file vengono aggiunti alla cartella Dropbox e al [!UICONTROL Numero massimo di file restituiti] l&#39;opzione è impostata su 10, poi 10 file vengono elaborati durante il primo ciclo, i successivi 10 file nel secondo ciclo, i successivi 10 file nel terzo ciclo e così via, fino all&#39;elaborazione di tutti i file.
>
>Tutti i file vengono elaborati in 1 esecuzione di scenario.
>
>I cicli già eseguiti sono disponibili nei dettagli Scenario:
>
>![](assets/scenario-detail-350x207.png)
>
>Per ulteriori informazioni su questa pagina, consulta [Dettagli scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-detail.md).

## Numero di errori consecutivi

Definisce il numero massimo di tentativi di esecuzione consecutivi prima che l&#39;esecuzione di uno scenario sia disattivata (escludendo [!UICONTROL DataError], [!UICONTROL DuplicateDataError] e [!UICONTROL ConnectionError]).

Per ulteriori informazioni sugli errori, vedi [Errore di elaborazione in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

>[!NOTE]
>
>Se uno scenario inizia con un trigger immediato, l’impostazione viene ignorata e lo scenario viene disattivato immediatamente dopo il primo errore.
