---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Panoramica dello scenario Adobe Workfront Fusion
description: Adobe Workfront Fusion richiede una licenza Adobe Workfront Fusion oltre a una licenza Adobe Workfront.
author: Becky
feature: Workfront Fusion
exl-id: 13d6230d-51f6-4f68-8697-30f8ce6c8599
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] panoramica dello scenario

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] richiede un [!DNL Adobe Workfront Fusion] oltre a una licenza [!DNL Adobe Workfront license].

>[!IMPORTANT]
>
>[!DNL Workfront Fusion] gli scenari non devono essere confusi con [!DNL Workfront Scenario Planner] scenari. Per informazioni su [!DNL Workfront Scenario Planner] scenari, vedi [La [!DNL Scenario Planner] panoramica](../../scenario-planner/scenario-planner-overview.md).

Il ruolo [!DNL Adobe Workfront Fusion] automatizza i processi in modo da poterti concentrare su nuove attività anziché ripetere più e più volte le stesse attività. Funziona tramite il collegamento di azioni all’interno e tra app e servizi per creare uno scenario che trasferisca e trasformi automaticamente i tuoi dati. Lo scenario in cui crei orologi i dati in un&#39;app o in un servizio ed elabora tali dati per fornire il risultato desiderato.

Uno scenario è composto da una serie di moduli che indicano come i dati devono essere trasformati all&#39;interno di un&#39;app o trasferiti tra app e servizi web.

## Esempio: Automazione dei processi in [!DNL Adobe Workfront]

>[!NOTE]
>
>Questa funzionalità è disponibile per le seguenti licenze:
>
>* [!UICONTROL [!DNL Workfront Fusion] per l&#39;automazione del lavoro]
>* [!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro]
>


[!DNL Workfront Fusion] consente di automatizzare flussi di lavoro semplici o complessi all’interno di [!DNL Workfront], risparmiando tempo e assicurando che il processo venga eseguito in modo coerente.

In questo esempio, lo scenario si attiva quando un campo specificato cambia in un&#39;attività o in un problema in [!DNL Workfront]. Quando viene attivato, lo scenario ottiene le informazioni nel progetto correlato e crea un aggiornamento personalizzato per una persona assegnata a un ruolo specifico sul progetto.

![](assets/fusion-template-example-350x102.png)

## Esempio: Collegamento [!DNL Workfront] a un&#39;altra app o a un altro servizio Web

>[!NOTE]
>
>Questa funzionalità è disponibile per la seguente licenza:
>
>* [!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro]
>


[!DNL Workfront Fusion] può anche connettersi ad altre app e ad altri servizi web. Puoi accedere, importare, manipolare o esportare dati da altre applicazioni, integrandoli con Workfront o tra loro. Molte applicazioni hanno dedicato [!DNL Workfront Fusion] connettori Se non esiste un connettore dedicato per l&#39;applicazione a cui si desidera accedere, è possibile utilizzare [!DNL Workfront Fusion]s [!UICONTROL HTTP] o [!UICONTROL SOAP] moduli per la connessione all’applicazione tramite la relativa API.

In questo esempio, lo scenario si attiva quando un utente viene aggiunto a un [!DNL Excel] foglio di calcolo. Lo scenario verifica se l’utente è in [!DNL Workfront]. In caso contrario, lo scenario crea l’utente in [!DNL Workfront] e aggiunge nuovamente il proprio ID utente Workfront al foglio di calcolo.

![](assets/fusion-integration-example--350x171.png)

Per un elenco dei connettori dedicati, consulta [App e loro moduli](../../workfront-fusion/apps-and-their-modules/apps-and-their-modules.md).

>[!IMPORTANT]
>
>[!DNL Adobe Workfront Fusion] può connettersi a quasi tutti i servizi web. Se l&#39;app con cui vuoi lavorare non ha un [!DNL Workfront Fusion] connettore, è possibile utilizzare i seguenti moduli per connettersi direttamente al servizio Web:
>
>* [[!UICONTROL HTTP] moduli](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md)
>* [[!UICONTROL SOAP] modulo](../../workfront-fusion/apps-and-their-modules/soap-module.md)
>* [[!UICONTROL JSON] moduli](../../workfront-fusion/apps-and-their-modules/json-modules.md)
>

