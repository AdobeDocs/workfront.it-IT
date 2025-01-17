---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: Trigger istantanei (webhook) in [!DNL Adobe Workfront Fusion]
description: La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione. Questo articolo è stato dichiarato obsoleto, ma contiene un collegamento al nuovo articolo che descrive questa funzionalità.
author: Becky
feature: Workfront Fusion
exl-id: 13b3a1bf-9856-4d2c-b1a5-13b044a7c2e5
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '971'
ht-degree: 0%

---

# Trigger istantanei (webhook) in [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione.
>
>Le informazioni contenute in questo articolo sono ora disponibili negli articoli:
>
>* [Trigger istantanei (webhook)](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/modules/webhooks-reference.html)
>* [Visualizza la coda di un webhook](https://experienceleague.adobe.com/docs/workfront-fusion/using/manage-scenarios/view-webhook-queue.html)
>
>Aggiorna eventuali segnalibri.
>
>Questo articolo non è più in fase di aggiornamento e verrà rimosso nel prossimo futuro.

Molti servizi forniscono webhook per inviare notifiche istantanee ogni volta che si verifica una certa modifica nel servizio. Per elaborare queste notifiche, ti consigliamo di utilizzare trigger istantanei. Puoi riconoscerli facilmente in [!DNL Adobe Workfront Fusion] a causa del loro tag:

![](assets/instant-350x256.png)

Se il servizio non fornisce webhook, è necessario utilizzare i trigger di polling per eseguire periodicamente il polling del servizio.

Per un video introduttivo ai webhook in Workfront Fusion, vedi:

* [Introduzione ai webhook](https://video.tv.adobe.com/v/3427025/){target=_blank}
* [Webhook intermedi](https://video.tv.adobe.com/v/3427030/){target=_blank}

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

## Visualizzare la coda di un webhook

Tutti i messaggi provenienti dai webhook in ingresso vengono memorizzati nella coda del webhook.

1. Fai clic su **[!UICONTROL Webhook]** nel menu a sinistra.
1. Individuare il webhook per il quale si desidera visualizzare la coda.
1. Fai clic sul pulsante con l’icona di un camion e il numero di webhook ricevuti.

   ![](assets/webhooks-truck-icon.png)

   >[!NOTE]
   >
   >I dati del webhook in ingresso vengono sempre memorizzati nella coda indipendentemente da come hai impostato l&#39;opzione [!UICONTROL Dati] come confidenziale (descritta in [Pannello impostazioni scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md)). Non appena i dati vengono elaborati in uno scenario, vengono eliminati definitivamente dal sistema.

## Pianificazione dei trigger istantanei

Se lo scenario contiene un trigger immediato, puoi pianificarne l’esecuzione immediata:

![](assets/schedule-setting-350x185.png)

In questo caso, lo scenario verrà eseguito immediatamente quando [!DNL Workfront Fusion] riceve nuovi dati dal servizio. Dopo l’esecuzione dello scenario, viene conteggiato il numero totale di webhook in attesa nella coda e lo scenario esegue tutti i cicli in cui sono presenti, elaborando un webhook per ciclo. Per ulteriori informazioni, vedere [Esecuzione dello scenario, cicli e fasi in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

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


Se utilizzi un&#39;impostazione di pianificazione diversa da [!UICONTROL Immediatamente], lo scenario viene eseguito agli intervalli specificati. Poiché è possibile raccogliere più webhook nella coda durante l&#39;intervallo, si consiglia di impostare il [[!UICONTROL numero massimo di cicli]](../../workfront-fusion/scenarios/scenario-settings-panel.md#maximum) su un valore superiore al valore predefinito 1 per elaborare più webhook in un&#39;esecuzione dello scenario:

1. Fai clic sull&#39;icona ![](assets/gear-icon-settings.png) delle [!UICONTROL impostazioni scenario] nella parte inferiore dello scenario.
1. Nella casella **[!UICONTROL Impostazioni scenario]** visualizzata digitare un numero nella casella **[!UICONTROL Numero massimo di cicli]** per indicare il numero di webhook dalla coda che si desidera eseguire ogni volta che si esegue lo scenario.

## Limiti di tariffa

L&#39;attuale limite di velocità è di 5 webhook al secondo. Se il limite viene superato, viene restituito un codice di stato 429.

## Scadenza dei webhook inattivi

Un webhook che non è stato assegnato ad alcuno scenario per più di 120 ore viene rimosso.

## Payload del webhook

[!DNL Workfront Fusion] memorizza i payload del webhook per 30 giorni. L&#39;accesso a un payload del webhook dopo più di 30 giorni dalla creazione genera l&#39;errore &quot;[!UICONTROL Impossibile leggere il file dall&#39;archivio.]&quot;

## Gestione degli errori

Quando si verifica un errore nello scenario con un trigger istantaneo, lo scenario:

* Si arresta immediatamente quando lo scenario è impostato per l&#39;esecuzione [!UICONTROL Immediata].
* Si interrompe dopo 3 tentativi non riusciti (3 errori) quando lo scenario è impostato per l’esecuzione come pianificato.

Se si verifica un errore durante l’esecuzione dello scenario, il webhook viene rimesso in coda durante la fase di rollback dell’attivatore istantaneo. In una situazione di questo tipo, puoi correggere lo scenario ed eseguirlo nuovamente. Per ulteriori informazioni, vedere [Rollback](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback) nell&#39;articolo [Esecuzione dello scenario, cicli e fasi in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

Se nello scenario è presente un modulo di risposta Webhook, l’errore viene inviato alla risposta Webhook. Il modulo di risposta Webhook viene sempre eseguito per ultimo (nel caso in cui l&#39;opzione [!UICONTROL Conferma automatica] nelle impostazioni dello scenario non sia abilitata). Per ulteriori informazioni, vedere [Risposta ai webhook](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md#respondi) nell&#39;articolo [Webhook](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md).

## Webhook personalizzati

Puoi creare webhook personalizzati. Per ulteriori informazioni, vedere [Webhook](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md).

## Disattivazione webhook

I webhook vengono disattivati automaticamente se si applica una delle seguenti condizioni:

* Il webhook non è stato connesso ad alcuno scenario per più di 5 giorni
* Il webhook viene utilizzato solo in scenari inattivi, che sono stati inattivi per più di 30 giorni.

I webhook disattivati vengono eliminati e annullati automaticamente se non sono connessi ad alcun scenario e se sono in stato disattivato da oltre 30 giorni.


