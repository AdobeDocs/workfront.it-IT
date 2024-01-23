---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Pannello delle impostazioni dello scenario in Adobe Workfront Fusion
description: Questo articolo descrive le impostazioni disponibili nel [!UICONTROL impostazioni scenario] nel tuo pannello [!DNL Adobe Workfront Fusion] scenari.
author: Becky
feature: Workfront Fusion
exl-id: 64a7a39a-f450-4eba-b4db-f31dd22aefdc
source-git-commit: 4d9832d0870c3fccf847c3932ad4f985a62b9672
workflow-type: tm+mt
source-wordcount: '1097'
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
   <td>
   <p>Fabbisogno di licenza corrente: No [!DNL Workfront Fusion] requisito di licenza.</p>
   <p>Oppure</p>
   <p>Requisito licenza legacy: [!UICONTROL [!DNL Workfront Fusion] per l'automazione e l'integrazione del lavoro], [!UICONTROL [!DNL Workfront Fusion] per automazione lavoro]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>
   <p>Fabbisogno prodotto corrente: se si dispone di [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront] Pianifica, la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare la funzionalità descritta in questo articolo. [!DNL Workfront Fusion] è incluso in [!UICONTROL Ultimate] [!DNL Workfront] piano.</p>
   <p>Oppure</p>
   <p>Requisiti del prodotto legacy: la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare la funzionalità descritta in questo articolo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, consulta [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Apri le impostazioni dello scenario

1. Apri l’editor dello scenario, come spiegato in [Editor scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-editor.md).
1. Fai clic sull’icona a forma di ingranaggio nell’angolo inferiore sinistro della pagina.

   ![](assets/scenario-settings-350x221.png)

   In [!UICONTROL Impostazioni scenario] che viene visualizzato, puoi configurare varie impostazioni avanzate per lo scenario.

## [!UICONTROL Consenti l’archiviazione di esecuzioni incomplete]

Questa opzione determina come [!DNL Adobe Workfront Fusion] procede se si verifica un errore durante l&#39;esecuzione di uno scenario. Con questa opzione abilitata, lo scenario viene messo in pausa e spostato in [Visualizzare e risolvere le esecuzioni incomplete in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md). Questo consente di risolvere il problema e continuare l’esecuzione dal punto in cui lo scenario è stato interrotto. Se questa opzione è disabilitata, l’esecuzione dello scenario si interrompe e viene avviata una fase di rollback.

## [!UICONTROL Elaborazione sequenziale]

Questa opzione determina come [!DNL Workfront Fusion] procede se si verifica un errore e l&#39;esecuzione di uno scenario viene spostata in [Visualizzare e risolvere le esecuzioni incomplete in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md). Se il [!UICONTROL Elaborazione sequenziale] se questa opzione è attivata, Workfront Fusion interrompe completamente l&#39;elaborazione della sequenza di attività fino a quando non vengono risolte tutte le esecuzioni incomplete. Se il [!UICONTROL Elaborazione sequenziale] l’opzione è disabilitata, lo scenario continua a essere eseguito in base alla sua pianificazione, accompagnato da ripetuti tentativi di eseguire nuovamente le esecuzioni incomplete.

>[!NOTE]
>
>L’elaborazione sequenziale può causare un ritardo nell’esecuzione di uno scenario. Se vi sono ancora esecuzioni incomplete nella coda quando si attiva uno scenario immediato o quando uno scenario pianificato è impostato per l’esecuzione, tale scenario verrà eseguito dopo che tutte le esecuzioni prima di essere nella coda sono state completate.
>
>Se il caso di utilizzo per gli scenari non richiede l’elaborazione sequenziale, si consiglia di disabilitare l’opzione di elaborazione sequenziale.

Per ulteriori informazioni sulla pianificazione, consulta [Pianificare uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).

## I dati sono riservati

Una volta eseguito uno scenario, per impostazione predefinita puoi visualizzare informazioni sui dati elaborati dai moduli nello scenario. Se non si desidera memorizzare queste informazioni, abilitare [!UICONTROL I dati sono riservati] opzione.

Per ulteriori informazioni sulla visualizzazione delle informazioni, vedere [Flusso di esecuzione dello scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).

>[!IMPORTANT]
>
>Se abiliti questa opzione, potrebbe essere difficile risolvere gli errori che possono verificarsi durante l’esecuzione di uno scenario.

## Abilita perdita di dati

Questa opzione ha a che fare con l&#39;abilitazione della perdita di dati se [!DNL Workfront Fusion] impossibile salvare un bundle nella coda di [Visualizzare e risolvere le esecuzioni incomplete in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md) (ad esempio, a causa della mancanza di spazio libero). Se questa opzione è abilitata, i dati vengono persi per evitare interruzioni nell’esecuzione complessiva dello scenario. Questo è utile per gli scenari in cui la priorità più alta è l’esecuzione continua e i dati errati in arrivo non sono così importanti.

Inoltre, durante l’esecuzione di uno scenario, a volte un modulo può incontrare un file di dimensioni superiori alla dimensione massima consentita. In questo caso, [!DNL Workfront Fusion] proventi conformemente alla fissazione del [!UICONTROL Abilita perdita di dati] e viene visualizzato un messaggio di avviso.

Per ulteriori informazioni sulle dimensioni massime dei file, vedere [Informazioni sulla mappatura dei file in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/about-mapping-files.md).

Per ulteriori informazioni sugli avvisi, consulta [Errore di elaborazione in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

## [!UICONTROL Commit automatico]

Il [!UICONTROL Commit automatico] Le impostazioni si applicano alle transazioni e definiscono la modalità di elaborazione di uno scenario. Se l&#39;opzione Auto commit è attiva, la fase di commit su ciascun modulo inizia immediatamente dopo il completamento della fase operativa. Se l&#39;opzione Auto commit è disattivata, non viene eseguito alcun commit finché non vengono eseguite operazioni per tutti i moduli (questa è la modalità predefinita).

Per ulteriori informazioni sulle transazioni, consulta [Esecuzione di scenari, cicli e fasi in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

## Numero massimo di cicli

L&#39;impostazione di più cicli può essere utile quando si desidera evitare l&#39;interruzione della connessione a un servizio di terze parti e assicurarsi che tutti i record vengano elaborati nell&#39;ambito dell&#39;esecuzione dello scenario.

* Se lo scenario inizia con un trigger di polling, l’impostazione definisce il numero massimo di cicli consentiti durante l’esecuzione dello scenario.

  Per ulteriori informazioni sui trigger di polling, consulta [Trigger di polling](../../workfront-fusion/modules/module-types.md#polling) in [Tipi di moduli](../../workfront-fusion/modules/module-types.md).

* Se lo scenario inizia con un trigger immediato, l’impostazione viene ignorata e tutti gli eventi in sospeso vengono elaborati durante l’esecuzione di un singolo scenario, un evento per ogni ciclo.

  Per ulteriori informazioni sui trigger istantanei, consulta [Trigger istantanei](../../workfront-fusion/modules/module-types.md#instant) in [Tipi di moduli](../../workfront-fusion/modules/module-types.md).

* Se lo scenario non inizia con un trigger (istantaneo/polling), viene sempre eseguito il numero massimo specificato di cicli.

>[!INFO]
>
>**Esempi:**  [!DNL Workfront] > [!UICONTROL Record di verifica] osserva i nuovi problemi che si presentano e [!DNL Workfront] >[!UICONTROL Converti oggetto] converte la nuova richiesta in un progetto e le assegna il modello appropriato.
>
>![](assets/scenario-settings-ex-1-350x157.png)
>
>A [!UICONTROL altri cicli] L&#39;impostazione viene applicata solo quando si pianifica l&#39;esecuzione dello scenario. Quando si utilizza [!UICONTROL Esegui una volta] , vengono prese in considerazione le impostazioni del ciclo.
>
>### Il numero massimo di cicli è impostato su 1 (impostazione predefinita)
>
>![](assets/max-number-cycles-1-350x201.png)
>
>Il [!UICONTROL Numero massimo di file restituiti] nel [!UICONTROL Dropbox] >[!UICONTROL Guarda i file] è impostato su `10`.
>
>![](assets/max-number-cycles-10-350x175.png)
>
>Se vengono inviate 100 richieste a [!DNL Workfront]e [!UICONTROL Limite] è impostato su 10, quindi 90 file vengono lasciati non elaborati dopo l’esecuzione di uno scenario. I successivi 10 file vengono elaborati nella successiva esecuzione pianificata dello scenario.
>
>### Numero massimo di cicli impostato su 10
>
>Il [!UICONTROL Numero massimo di file restituiti] nel [!UICONTROL Dropbox] >[!UICONTROL Guarda i file] è impostato su `10`.
>
>Se vengono aggiunti 100 file alla cartella di Dropbox e al [!UICONTROL Numero massimo di file restituiti] l&#39;opzione è impostata su 10, quindi vengono elaborati 10 file durante il primo ciclo, i successivi 10 file nel secondo ciclo, i successivi 10 file nel terzo ciclo e così via, fino a quando tutti i file non vengono elaborati.
>
>Tutti i file vengono elaborati entro 1 esecuzione dello scenario.
>
>Puoi visualizzare i cicli già eseguiti nei dettagli dello scenario:
>
>![](assets/scenario-detail-350x207.png)
>
>Per ulteriori informazioni su questa pagina, consulta [Dettagli dello scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-detail.md).

## Numero di errori consecutivi

Definisce il numero massimo di tentativi di esecuzione consecutivi prima che l’esecuzione di uno scenario venga disattivata (escludendo [!UICONTROL DataError], [!UICONTROL DuplicateDataError] e [!UICONTROL ErroreConnessione]).

Per ulteriori informazioni sugli errori, consulta [Errore di elaborazione in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

>[!NOTE]
>
>Se uno scenario inizia con un trigger immediato, l’impostazione viene ignorata e lo scenario viene disattivato immediatamente dopo il primo errore.
