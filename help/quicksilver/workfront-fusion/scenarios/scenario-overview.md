---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Panoramica sullo scenario Adobe Workfront Fusion
description: Adobe Workfront Fusion richiede una licenza Adobe Workfront Fusion oltre a una licenza Adobe Workfront.
author: Becky
feature: Workfront Fusion
exl-id: 13d6230d-51f6-4f68-8697-30f8ce6c8599
source-git-commit: f8ea4a1c40cd3fc4664a5a3b1c3a900e874d78b1
workflow-type: tm+mt
source-wordcount: '644'
ht-degree: 0%

---

# Panoramica dello scenario [!DNL Adobe Workfront Fusion]

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] richiede una licenza [!DNL Adobe Workfront Fusion] oltre a [!DNL Adobe Workfront license].

>[!IMPORTANT]
>
>[!DNL Workfront Fusion] scenari non devono essere confusi con [!DNL Workfront Scenario Planner] scenari. Per informazioni sugli scenari [!DNL Workfront Scenario Planner], vedere [The [!DNL Scenario Planner] overview](../../scenario-planner/scenario-planner-overview.md).

Il ruolo di [!DNL Adobe Workfront Fusion] consiste nell&#39;automatizzare i processi in modo da potersi concentrare su nuove attività anziché ripetere più volte le stesse attività. Funziona tramite il collegamento di azioni all’interno e tra app e servizi per creare uno scenario che trasferisce e trasforma automaticamente i dati. Lo scenario in cui si creano controlli i dati in un’app o in un servizio ed elabora tali dati in modo da fornire il risultato desiderato.

Uno scenario è costituito da una serie di moduli che indicano come i dati devono essere trasformati all’interno di un’app o trasferiti tra app e servizi web.

## Panoramica degli elementi dello scenario

Uno scenario è costituito da elementi diversi. Comprendere la terminologia di tali elementi semplifica l’utilizzo della documentazione.

### Scenario

Uno **scenario** è una serie di passaggi automatizzati creati dall&#39;utente per spostare e manipolare i dati. Il termine &quot;scenario&quot; si riferisce all&#39;intero gruppo di fasi collegate.

![Scenario](assets/entire-scenario-scenario.png)

### Trigger

Uno scenario inizia con un **trigger**. Il trigger controlla i dati nuovi e aggiornati e avvia lo scenario quando si applicano determinate condizioni configurate nel modulo. Gli attivatori possono essere configurati per avviare uno scenario secondo una pianificazione (polling) o ogni volta che si verificano modifiche ai dati (istantanei).

![Trigger](assets/scenario-trigger.png)

### Modulo

Il trigger è seguito da **moduli**. Un modulo rappresenta un singolo passaggio in uno scenario che esegue un’azione specifica. I moduli sono configurati e concatenati tra loro per creare scenari.

![Modulo](assets/scenario-module.png)

### Percorso

Uno scenario può essere diviso in **route**. Una route è una sezione dello scenario che può essere o meno utilizzata per un determinato bundle di dati. Le route vengono configurate utilizzando un modulo router e filtri.

![Route](assets/scenario-route.png)

### Segmento scenario

Un segmento di scenario è una sezione di uno scenario costituita da una serie di moduli contigui che si connettono tutti alla stessa applicazione. I segmenti di scenario spesso rappresentano un breve flusso di lavoro nell’applicazione.

![Segmento scenario](assets/scenario-segment.png)

### Connettore

Un connettore è il set di moduli per una determinata applicazione. Workfront Fusion offre connettori per molte applicazioni di lavoro comuni, come Workfront, Salesforce e Jira, nonché connettori generici che possono essere utilizzati per qualsiasi servizio web.

![Connettori](assets/scenario-connectors.png)



## Esempio: automazione dei processi in [!DNL Adobe Workfront]

>[!NOTE]
>
>Questa funzionalità è disponibile per le seguenti licenze:
>
>* [!UICONTROL [!DNL Workfront Fusion] per automazione lavoro]
>* [!UICONTROL [!DNL Workfront Fusion] per l&#39;automazione e l&#39;integrazione del lavoro]

[!DNL Workfront Fusion] consente di automatizzare flussi di lavoro semplici o complessi all&#39;interno di [!DNL Workfront], risparmiando tempo e assicurando che il processo venga eseguito in modo coerente.

In questo esempio, lo scenario si attiva quando un campo specificato cambia in un&#39;attività o in un problema in [!DNL Workfront]. Quando viene attivato, lo scenario ottiene informazioni nel progetto correlato e crea un aggiornamento personalizzato per una persona assegnata a un ruolo specifico nel progetto.

![](assets/fusion-template-example-350x102.png)

## Esempio: connessione di [!DNL Workfront] a un&#39;altra app o servizio Web

>[!NOTE]
>
>Questa funzionalità è disponibile per la seguente licenza:
>
>* [!UICONTROL [!DNL Workfront Fusion] per l&#39;automazione e l&#39;integrazione del lavoro]
>

[!DNL Workfront Fusion] può anche connettersi ad altre app e servizi Web. È possibile accedere, importare, manipolare o esportare dati da altre applicazioni, integrandoli con Workfront o tra loro. Molte applicazioni dispongono di connettori [!DNL Workfront Fusion] dedicati. Se non è presente alcun connettore dedicato per l&#39;applicazione a cui si desidera accedere, è possibile utilizzare i moduli [!UICONTROL HTTP] o [!UICONTROL SOAP] di [!DNL Workfront Fusion] per connettersi all&#39;applicazione tramite la relativa API.

In questo esempio, lo scenario viene attivato quando un utente viene aggiunto a un foglio di calcolo [!DNL Excel]. Lo scenario controlla se l&#39;utente si trova in [!DNL Workfront]. In caso contrario, l&#39;utente verrà creato in [!DNL Workfront] e il relativo ID utente Workfront verrà nuovamente aggiunto al foglio di calcolo.

![](assets/fusion-integration-example--350x171.png)

Per un elenco dei connettori dedicati, vedere [App e relativi moduli](../../workfront-fusion/apps-and-their-modules/apps-and-their-modules.md).

>[!IMPORTANT]
>
>[!DNL Adobe Workfront Fusion] può connettersi a quasi tutti i servizi Web. Se l&#39;app che si desidera utilizzare non dispone di un connettore [!DNL Workfront Fusion] dedicato, è possibile utilizzare i seguenti moduli per connettersi direttamente al servizio Web:
>
>* [[!UICONTROL moduli HTTP]](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md)
>* Modulo [[!UICONTROL SOAP]](../../workfront-fusion/apps-and-their-modules/soap-module.md)
>* [[!UICONTROL JSON] moduli](../../workfront-fusion/apps-and-their-modules/json-modules.md)
>
