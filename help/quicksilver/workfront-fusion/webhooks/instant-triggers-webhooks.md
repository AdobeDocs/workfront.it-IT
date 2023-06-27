---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: Trigger istantanei (webhook) in [!DNL Adobe Workfront Fusion]
description: Molti servizi forniscono webhook per inviare notifiche istantanee ogni volta che si verifica una certa modifica nel servizio. Per elaborare queste notifiche, ti consigliamo di utilizzare trigger istantanei. Questo articolo descrive l’utilizzo e la funzionalità dei trigger istantanei in Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 13b3a1bf-9856-4d2c-b1a5-13b044a7c2e5
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '903'
ht-degree: 0%

---

# Trigger istantanei (webhook) in [!DNL Adobe Workfront Fusion]

Molti servizi forniscono webhook per inviare notifiche istantanee ogni volta che si verifica una certa modifica nel servizio. Per elaborare queste notifiche, ti consigliamo di utilizzare trigger istantanei. È possibile riconoscerli facilmente in [!DNL Adobe Workfront Fusion] a causa del tag:

![](assets/instant-350x256.png)

Se il servizio non fornisce webhook, è necessario utilizzare i trigger di polling per eseguire periodicamente il polling del servizio.

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

## Visualizzare la coda di un webhook

Tutti i messaggi provenienti dai webhook in ingresso vengono memorizzati nella coda del webhook.

1. Clic **[!UICONTROL Webhook]** nel menu a sinistra.
1. Individuare il webhook per il quale si desidera visualizzare la coda.
1. Fai clic sul pulsante con l’icona di un camion e il numero di webhook ricevuti.

   ![](assets/webhooks-truck-icon.png)

   >[!NOTE]
   >
   >I dati del webhook in ingresso vengono sempre memorizzati nella coda indipendentemente da come hai impostato l’opzione [!UICONTROL Dati] è riservato (descritto in [Il pannello delle impostazioni dello scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md)). Non appena i dati vengono elaborati in uno scenario, vengono eliminati definitivamente dal sistema.

## Pianificazione dei trigger istantanei

Se lo scenario contiene un trigger immediato, puoi pianificarne l’esecuzione immediata:

![](assets/schedule-setting-350x185.png)

In questo caso, lo scenario verrà eseguito immediatamente quando [!DNL Workfront Fusion] riceve nuovi dati dal servizio. Dopo l’esecuzione dello scenario, viene conteggiato il numero totale di webhook in attesa nella coda e lo scenario esegue tutti i cicli in cui sono presenti, elaborando un webhook per ciclo. Per ulteriori informazioni, consulta [Esecuzione di scenari, cicli e fasi in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

>[!NOTE]
>
>* Un ciclo non è lo stesso di un&#39;esecuzione di uno scenario. Possono essere presenti più cicli in 1 esecuzione dello scenario.
>* Quando esegui uno scenario con un trigger immediato pianificato come immediato, si applicano le seguenti eccezioni:
>
>     * L&#39;intervallo tra due esecuzioni non è soggetto all&#39;intervallo minimo in base al piano tariffario.
>
>       Ad esempio, una volta che lo scenario termina la sua esecuzione, la coda del webhook viene nuovamente controllata. Se sono presenti webhook in sospeso, lo scenario viene eseguito immediatamente di nuovo, elaborando nuovamente tutti i webhook in sospeso.
>   
>     * L’impostazione dello scenario Numero massimo di cicli viene ignorata e impostata su 100, il che significa che non più di 100 webhook in sospeso verranno elaborati durante un’unica esecuzione dello scenario (alla velocità di 1 evento per ogni ciclo).
>


Se utilizzi un’impostazione diversa da [!UICONTROL Immediatamente], lo scenario viene eseguito agli intervalli specificati. Poiché è possibile raccogliere più webhook nella coda durante l’intervallo, si consiglia di impostare [[!UICONTROL Numero massimo di cicli]](../../workfront-fusion/scenarios/scenario-settings-panel.md#maximum) a un valore più alto del valore predefinito 1 per elaborare più webhook in un’esecuzione dello scenario:

1. Fai clic su [!UICONTROL Impostazioni scenario] icona ![](assets/gear-icon-settings.png) in fondo allo scenario.
1. In **[!UICONTROL Impostazioni scenario]** nella casella visualizzata, digitare un numero nella casella **[!UICONTROL Numero massimo di cicli]** per indicare il numero di webhook dalla coda che si desidera eseguire ogni volta che si esegue lo scenario.

## Limiti di tariffa

L&#39;attuale limite di velocità è di 5 webhook al secondo. Se il limite viene superato, viene restituito un codice di stato 429.

## Scadenza dei webhook inattivi

Un webhook che non è stato assegnato ad alcuno scenario per più di 120 ore viene rimosso.

## Payload del webhook

[!DNL Workfront Fusion] memorizza i payload del webhook per 30 giorni. Se si accede a un payload del webhook più di 30 giorni dopo la sua creazione, viene generato l’errore &quot;[!UICONTROL Impossibile leggere il file dall&#39;archivio.]&quot;

## Gestione degli errori

Quando si verifica un errore nello scenario con un trigger istantaneo, lo scenario:

* Si arresta immediatamente - quando lo scenario è impostato per l’esecuzione [!UICONTROL Immediatamente].
* Si interrompe dopo 3 tentativi non riusciti (3 errori) quando lo scenario è impostato per l’esecuzione come pianificato.

Se si verifica un errore durante l’esecuzione dello scenario, il webhook viene rimesso in coda durante la fase di rollback dell’attivatore istantaneo. In una situazione di questo tipo, puoi correggere lo scenario ed eseguirlo nuovamente. Per ulteriori informazioni, consulta [Rollback](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback) nell’articolo [Esecuzione di scenari, cicli e fasi in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

Se nello scenario è presente un modulo di risposta Webhook, l’errore viene inviato alla risposta Webhook. Il modulo di risposta Webhook viene sempre eseguito per ultimo (nel caso in cui [!UICONTROL Commit automatico] nelle impostazioni dello scenario non è abilitata). Per ulteriori informazioni, consulta [Risposta ai webhook](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md#respondi) nell’articolo [Webhook](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md).

## Webhook personalizzati

Puoi creare webhook personalizzati. Per ulteriori informazioni, consulta [Webhook](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md).

## Disattivazione webhook

I webhook vengono disattivati automaticamente se si applica una delle seguenti condizioni:

* Il webhook non è stato connesso ad alcuno scenario per più di 5 giorni
* Il webhook viene utilizzato solo in scenari inattivi, che sono stati inattivi per più di 30 giorni.

I webhook disattivati vengono eliminati e annullati automaticamente se non sono connessi ad alcun scenario e se sono in stato disattivato da oltre 30 giorni.


