---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Eseguire l’esperto di punteggio scenario
description: Gestisci scenari bloccati in [!DNL Adobe Workfront Fusion]
author: Becky
feature: Workfront Fusion
hide: true
hidefromtoc: true
source-git-commit: ed100c6ba32a6fbff6fa68ac7a4bfb38db861b17
workflow-type: tm+mt
source-wordcount: '295'
ht-degree: 0%

---

# Eseguire l’esperto di valutazione degli scenari in Adobe Workfront Fusion

L’esperto di valutazione degli scenari può aiutarti a garantire che lo scenario sia configurato nel modo che segue le best practice. Controlla lo scenario e fornisce consigli per la sua struttura e organizzazione.

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
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione lavoro] </p><p>[!UICONTROL [!DNL Workfront Fusion] per automazione lavoro] </p>  </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</td> 
  </tr> 
 </tbody> 
</table>

Per conoscere il piano, il tipo di licenza o l&#39;accesso disponibili, contattare l&#39;amministratore [!DNL Workfront].

Per informazioni sulle [!DNL Adobe Workfront Fusion] licenze, vedere [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

Eseguire l’esperto di punteggio scenario

1. Fai clic sulla scheda **[!UICONTROL Scenario]** nel pannello a sinistra.
1. Selezionare lo scenario in cui si desidera eseguire l&#39;esperto punteggio scenario.
1. Fai clic in un punto qualsiasi dello scenario per accedere all’editor scenario.
1. Fai clic sull&#39;icona Esperto punteggio scenario ![Esperto punteggio scenario](assets/scoring-expert-icon.png) nella parte inferiore dello schermo.

   Viene visualizzato il pannello Esperto punteggio scenario.
1. Fare clic su **Valuta**.

L’esperto di punteggio dello scenario restituisce un punteggio su 10 e mostra quali controlli sono stati superati o non riusciti. Se un controllo non è riuscito, l’esperto di valutazione dello scenario fornisce consigli su come garantire che lo scenario soddisfi questi controlli.

![Punteggio scenario](assets/scenario-score.png)

## Controlli punteggio scenario

L’esperto di valutazione degli scenari utilizza i seguenti controlli:

* Lo scenario deve essere denominato.
* Tutti i moduli devono essere etichettati.
* Lo scenario deve essere eseguito in base a una pianificazione impostata.

  Per istruzioni, consulta [Pianificare uno scenario](/help/quicksilver/workfront-fusion/scenarios/schedule-a-scenario.md).
* La dimensione del blueprint dello scenario deve essere inferiore a 5 MB.

  Per ulteriori informazioni, vedere [Guardrail delle prestazioni di Fusion](/help/quicksilver/workfront-fusion/get-started/fusion-performance-guardrails.md#scenarios).
* Se viene utilizzato un modulo di attivazione immediata di Workfront, deve essere filtrato.

  Per istruzioni, vedere [Filtri sottoscrizioni eventi nel modulo  [!DNL Workfront] > [!UICONTROL Osserva eventi]](/help/quicksilver/workfront-fusion/apps-and-their-modules/workfront-modules.md#event-subscription-filters-in-the-workfront--watch-events-module).





