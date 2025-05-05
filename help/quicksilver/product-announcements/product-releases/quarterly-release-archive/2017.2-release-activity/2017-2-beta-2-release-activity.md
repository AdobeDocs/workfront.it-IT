---
content-type: release-notes
navigation-topic: product-releases-archive
title: Attività sulla versione 2017.2 di Beta 2
description: Questa pagina descrive tutte le modifiche disponibili nell’ambiente di anteprima con la versione 2017.2 di Beta 2. La funzionalità di questa pagina è stata resa disponibile nell’ambiente di anteprima il 24 maggio 2017. Sarà disponibile nell’ambiente di produzione tra la fine di luglio e l’inizio di agosto 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 0aa8d61e-cf8c-46a7-b093-a0dbc90d37fd
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '792'
ht-degree: 0%

---

# Attività sulla versione 2017.2 di Beta 2

Questa pagina descrive tutte le modifiche disponibili nell’ambiente di anteprima con la versione 2017.2 di Beta 2. La funzionalità di questa pagina è stata resa disponibile nell’ambiente di anteprima il 24 maggio 2017. Sarà disponibile nell’ambiente di produzione tra la fine di luglio e l’inizio di agosto 2017.

>[!IMPORTANT]
>
>La funzionalità descritta in questa pagina è soggetta a modifiche prima della disponibilità nell’ambiente di produzione.

Per un elenco di tutte le modifiche apportate in 2017.2, consulta [Panoramica delle attività sulla versione 2017.2](../../../../product-announcements/product-releases/quarterly-release-archive/2017.2-release-activity/2017-2-release-activity-overview.md).

La versione 2017.2 di Beta 2 contiene miglioramenti sia per gli amministratori di Workfront che per altri utenti:

**Per gli amministratori:**

* [Miglioramento API: abbonamenti agli eventi](#api-enhancement-event-subscriptions)

**Per Tutti Gli Utenti:**

* [Abbonati ai progetti](#subscribe-to-projects)
* [Annulla iscrizione a elementi da e-mail](#unsubscribe-from-items-from-email)
* [Configura la visualizzazione delle attività cardine nel Diagramma di Gantt](#configure-how-milestones-are-displayed-on-the-gantt-chart)
* [Modelli per gruppi di risorse](#resource-pools-templates)
* [Visualizzare le versioni dei documenti sottoposti a bozza in Workfront](#view-versions-of-proofed-documents-within-workfront)
* [Nuovo oggetto richiedente nel report Approvazione bozza](#new-requester-object-in-proof-approval-report)

## Miglioramento API: abbonamenti agli eventi {#api-enhancement-event-subscriptions}

Quando si verifica un&#39;azione su un oggetto Workfront supportato dalle sottoscrizioni di eventi, ora puoi configurare Workfront per inviare una risposta all&#39;endpoint desiderato. Ciò significa che le integrazioni possono interagire con l’API di Workfront in tempo reale.

Per ulteriori informazioni, vedere [API sottoscrizione eventi](../../../../wf-api/general/event-subs-api.md). 

## Abbonati ai progetti {#subscribe-to-projects}

È ora possibile aggiungere nuovi commenti ai progetti per i quali non si fa parte del team di progetto. Prima di questa versione, era possibile abbonarsi solo a commenti su problemi e attività.

Per ulteriori informazioni sulla sottoscrizione agli elementi, vedere [Sottoscrizione agli elementi in Adobe Workfront](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md)

## Annulla iscrizione a elementi da e-mail {#unsubscribe-from-items-from-email}

Puoi annullare l’iscrizione agli elementi utilizzando il collegamento &quot;Annulla iscrizione&quot; presente nell’e-mail di iscrizione. In precedenza, era possibile annullare l’abbonamento solo a un elemento dall’interfaccia di Workfront.

Per ulteriori informazioni sull&#39;annullamento dell&#39;abbonamento alle e-mail, consulta la sezione &quot;Rinuncia alle notifiche e-mail&quot; in [Notifiche Adobe Workfront](../../../../workfront-basics/using-notifications/wf-notifications.md) 

## Configurare la modalità di visualizzazione delle milestone nel diagramma di Gantt {#configure-how-milestones-are-displayed-on-the-gantt-chart}

***CORREZIONE &#x200B;**: questa funzione non è attualmente disponibile nell&#39;ambiente Sandbox di anteprima. Il rilascio è previsto in una data successiva, nel corso del mese di giugno 2017.*

Sono ora disponibili due opzioni per visualizzare le informazioni sulle milestone in un diagramma di Gantt. Puoi configurare uno o entrambi i seguenti indicatori milestone:

* Rombi milestone (icona)

  Questa icona viene visualizzata nel diagramma di Gantt dopo qualsiasi attività associata a un&#39;attività cardine.

* Linee milestone

  Dopo un&#39;attività associata all&#39;attività cardine viene visualizzata una linea per tutte le attività del diagramma di Gantt.

Prima di questa modifica, era disponibile una sola opzione per consentire la visualizzazione delle Milestone in un diagramma di Gantt, denominata &quot;Milestone&quot;. Questa opzione consente di attivare sia l&#39;icona del rombo della milestone che la linea della milestone. Non è stato possibile separare questi indicatori. Le due opzioni sono ora disponibili in tutti i diagrammi di Gantt, compresi tutti gli elenchi e i rapporti dei progetti. 

Per ulteriori informazioni sulla configurazione della visualizzazione delle informazioni nel diagramma di Gantt, vedere [Configurare la visualizzazione delle informazioni nel diagramma di Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

## Modelli per gruppi di risorse {#resource-pools-templates}

È ora possibile specificare i gruppi di risorse per i modelli. Prima di questa versione, era possibile associare i Pool di Risorse solo a utenti e progetti.

Per ulteriori informazioni sui gruppi di risorse, vedere [Panoramica sui gruppi di risorse](../../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md)

## Visualizzare le versioni dei documenti bozza in Workfront {#view-versions-of-proofed-documents-within-workfront}

Ora è possibile visualizzare le bozze da tutte le versioni di un documento revisionato nell’interfaccia di Workfront. 

Prima di questa modifica, era possibile visualizzare solo la versione più recente del documento revisionato.

Gli utenti che non dispongono di una licenza di verifica possono:

* Aprire una bozza in una versione precedente di un documento revisionato

Gli utenti con una licenza di verifica possono eseguire una delle operazioni seguenti:

* Aprire una bozza in una versione precedente di un documento revisionato
* Visualizzare i dettagli della bozza in una versione precedente di un documento revisionato

Per ulteriori informazioni, vedere [Gestire le versioni dei documenti](../../../../documents/managing-documents/manage-document-versions.md) in [Gestire le versioni dei documenti](../../../../documents/managing-documents/manage-document-versions.md).

## Nuovo oggetto richiedente nel report Approvazione bozza {#new-requester-object-in-proof-approval-report}

Ora, quando si crea un rapporto Proof Approval (Approvazione della bozza), è presente un nuovo oggetto Requester. Questo oggetto consente di creare rapporti sulle informazioni relative all’utente che ha richiesto l’approvazione della bozza. 

Il nuovo oggetto Requester nel report Proof Approval (Approvazione bozza) contiene tutti i campi disponibili con l&#39;oggetto User esistente in altri tipi di report sugli oggetti.

>[!NOTE]
>
> Queste informazioni sono disponibili nel rapporto solo dal momento in cui questa funzione è stata introdotta per la prima volta nei rispettivi ambienti di anteprima o produzione; le informazioni nei rapporti relativi all’oggetto richiedente precedenti all’introduzione di questa funzionalità non sono disponibili.

È possibile accedere all&#39;oggetto Requester durante la creazione di un report Proof Approval, come descritto in [Creare un report personalizzato](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Per ulteriori informazioni sul report degli oggetti Proof Approvals, vedere la sezione [Comprendere gli oggetti in Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) in [Comprendere gli oggetti in Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).
