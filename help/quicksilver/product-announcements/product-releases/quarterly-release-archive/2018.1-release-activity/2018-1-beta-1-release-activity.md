---
content-type: release-notes
navigation-topic: product-releases-archive
title: Attività sulla versione 2018.1 di Beta 1
description: Questa pagina descrive tutte le modifiche più recenti disponibili nell’ambiente di anteprima con la versione 2018.1 di Beta 1. La funzionalità di questa pagina è stata resa disponibile nell’ambiente di anteprima il 1° dicembre 2017. Sarà disponibile nell’ambiente di produzione a marzo 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: efcc2217-ab69-4ac4-8e9a-f811eba77d49
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1065'
ht-degree: 0%

---

# Attività sulla versione 2018.1 di Beta 1

Questa pagina descrive tutte le modifiche più recenti disponibili nell’ambiente di anteprima con la versione 2018.1 di Beta 1. La funzionalità di questa pagina è stata resa disponibile nell’ambiente di anteprima il 1° dicembre 2017. Sarà disponibile nell’ambiente di produzione a marzo 2018.

>[!IMPORTANT]
>
> La funzionalità descritta in questa pagina è soggetta a modifiche prima della disponibilità nell’ambiente di produzione.

Per un elenco di tutte le modifiche apportate in 2018.1, consulta  Panoramica dell&#39;attività della versione di [2018.1](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md).

La versione 2018.1 di Beta 1 contiene miglioramenti sia per gli amministratori di Workfront che per altri utenti:

**Per Amministratori**

* [Modello di layout aggiornato per supportare l&#39;area Home](#updated-layout-template-to-support-the-home-area)
* [Disattiva le notifiche e-mail di verifica inviate da Workfront](#disable-proofing-email-notifications-sent-from-workfront)
* [Nuove risorse aggiunte alle sottoscrizioni di eventi](#new-resources-added-to-event-subscriptions)

**Per Tutti Gli Utenti**

* [Area Home (Area di lavoro personale aggiornata)](#home-area-updated-my-work-area)
* [Visualizzazione dei dati di programmazione delle risorse nel Business Case e aggiornamento del Riepilogo del Business Case](#display-resource-planner-data-under-the-business-case-and-updated-business-case-summary)
* [Visualizza la percentuale di allocazione delle ore pianificate nella pianificazione risorse](#display-the-percentage-of-planned-hour-allocation-in-the-resource-planner)
* [I tipi di aggiornamento &quot;Automatico e In caso di modifica&quot; e &quot;Solo modifica&quot; attivano gli aggiornamenti agli oggetti padre contemporaneamente all&#39;aggiornamento delle attività](#the-automatic-and-on-change-and-change-only-update-types-trigger-updates-to-the-parent-objects-at-the-same-time-as-tasks-are-updated)
* [Snapshot della timeline disponibile nel diagramma di Gantt](#timeline-snapshot-available-in-the-gantt-chart)

## Area Home (area di lavoro personale aggiornata) {#home-area-updated-my-work-area}

La nuova area Home offre una visualizzazione alternativa migliorata degli stessi dati attualmente disponibili nell&#39;area Il mio lavoro. L&#39;area Home offre i seguenti vantaggi rispetto all&#39;area Il mio lavoro:

* Un&#39;interfaccia più semplice e intuitiva
* Prestazioni migliorate
* Aggiornare attività e problemi con la formattazione del testo RTF

## Modello di layout aggiornato per supportare l’area Home {#updated-layout-template-to-support-the-home-area}

In qualità di amministratore di Workfront, puoi determinare se gli utenti dell’organizzazione hanno accesso all’area Home configurando il modello di layout a cui sono assegnati. Gli utenti ai quali non è assegnato un modello di layout possono sempre accedere all’area Home.

Per ulteriori informazioni, vedere &quot;Creare e gestire modelli di layout&quot;.

## Disattiva le notifiche e-mail di verifica inviate da Workfront {#disable-proofing-email-notifications-sent-from-workfront}

Ora puoi configurare se gli utenti nella tua istanza di Workfront riceveranno notifiche e-mail da Workfront quando viene aggiunto un commento alla bozza.

In precedenza, le e-mail di verifica venivano sempre inviate da Workfront quando veniva fatto un commento su una bozza. Se le notifiche erano abilitate anche in Workfront Proof, gli utenti ricevevano notifiche duplicate. 

Per i clienti Workfront esistenti, Workfront è configurato per impostazione predefinita per inviare e-mail quando viene inserito un commento su una bozza.

Per informazioni su come disabilitare le notifiche e-mail relative alle bozze in Workfront in modo che le e-mail di verifica vengano inviate solo da Workfront Proof, consulta .  

## Visualizza i dati di programmazione delle risorse nel Business Case e nel Riepilogo del Business Case aggiornato {#display-resource-planner-data-under-the-business-case-and-updated-business-case-summary}

L&#39;area Budget risorse è ora disponibile nel Business Case di un progetto. In quest&#39;area è possibile esaminare le ore preventivate stimate per le risorse nella Programmazione risorse e il costo manodopera preventivato ad esse associato.

L&#39;area Stime risorse del Business Case è stata rinominata in Stime risorse legacy.

Come parte di questa modifica, il pannello di riepilogo Caso di business ora include informazioni finanziarie basate sia sulle stime delle risorse che sul budget delle risorse.

Prima di questa modifica, non era possibile visualizzare le informazioni di Programmazione delle risorse nel Business Case del progetto. È possibile visualizzare solo le informazioni relative alle Stime di risorse specificate nel Capacity Planner dei Pool di Risorse Legacy.

Per ulteriori informazioni sulla creazione di un caso aziendale, vedere [Creare un caso aziendale per un progetto](../../../../manage-work/projects/define-a-business-case/create-business-case.md).

## Visualizzare la percentuale di allocazione delle ore pianificate nella pianificazione risorse {#display-the-percentage-of-planned-hour-allocation-in-the-resource-planner}

La Vista utente della Programmazione delle risorse ora include una nuova colonna che consente di visualizzare l&#39;Allocazione delle ore pianificate come percentuale del totale delle ore disponibili per l&#39;utente e il ruolo.

Prima di questa modifica, era possibile visualizzare il totale delle ore pianificate e delle ore disponibili per gli utenti e le mansioni solo in colonne separate.

Per ulteriori informazioni sulla colonna Percentuale allocazione ore pianificate, vedere la sezione &quot;Visualizzazione della differenza tra le ore disponibili e quelle pianificate o FTE nella pianificazione risorse&quot; in [Panoramica sulla pianificazione risorse](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## I tipi di aggiornamento &quot;Automatico e in caso di modifica&quot; e &quot;Solo modifica&quot; attivano gli aggiornamenti agli oggetti padre contemporaneamente all&#39;aggiornamento delle attività {#the-automatic-and-on-change-and-change-only-update-types-trigger-updates-to-the-parent-objects-at-the-same-time-as-tasks-are-updated}

È stato modificato il modo in cui le attività padre e il progetto vengono aggiornati quando un oggetto di livello inferiore viene aggiornato in un progetto. Il momento in cui un oggetto padre viene aggiornato è determinato dal campo Tipo di aggiornamento di un progetto. È possibile selezionare uno dei seguenti tipi di aggiornamento:

* Automatico e con Modifica
* Solo Modifica
* Solo Automatico
* Solo Manuale

Ora, quando si selezionano i Tipi di aggiornamento &quot;Automatico e In modifica&quot; o &quot;Solo modifica&quot;, le modifiche applicate alle singole attività vengono applicate immediatamente anche all&#39;attività padre e al progetto.

Prima di questa modifica, era necessario aggiornare la pagina per assicurarsi che anche gli oggetti principali e la timeline del progetto fossero aggiornati.

Per ulteriori informazioni sul tipo di aggiornamento di un progetto, vedere [Selezionare il tipo di aggiornamento del progetto](../../../../manage-work/projects/manage-projects/select-project-update-type.md).

## Snapshot della timeline disponibile nel diagramma di Gantt {#timeline-snapshot-available-in-the-gantt-chart}

Ora puoi scorrere rapidamente fino a un determinato punto della durata di un progetto utilizzando la nuova istantanea della timeline nel diagramma di Gantt.

Quando si seleziona un intervallo di tempo più granulare per il diagramma di Gantt quando si visualizza un&#39;attività o un elenco di progetti, nella parte inferiore del diagramma viene visualizzata una barra di scorrimento orizzontale. Facendo clic sulla barra di scorrimento è possibile visualizzare l&#39;intera sequenza temporale del progetto in un&#39;istantanea. È possibile fare clic in un punto qualsiasi dello snapshot del diagramma di Gantt per passare a un punto specifico della durata del progetto.

Prima di questa modifica, era necessario scorrere orizzontalmente l&#39;intero diagramma di Gantt per trovare un determinato punto nel tempo, oppure era necessario ridurre la visualizzazione granulare.

Per ulteriori informazioni sulla visualizzazione delle informazioni nel diagramma di Gantt, vedere [Configurare la visualizzazione delle informazioni nel diagramma di Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

## Nuove risorse aggiunte alle sottoscrizioni di eventi {#new-resources-added-to-event-subscriptions}

Ora puoi creare sottoscrizioni di eventi per le seguenti risorse:

* **Spesa:** ti avvisa quando una spesa viene aggiunta o modificata.
* **Assegnazione:** invia una notifica quando un&#39;assegnazione viene aggiunta o modificata in un&#39;attività o in un problema per un utente, una mansione o un team.
* **Scheda orario:** ti avvisa quando una scheda orario viene inviata, rifiutata o approvata.

Per ulteriori informazioni sulle sottoscrizioni di eventi, vedere [API sottoscrizione eventi](../../../../wf-api/general/event-subs-api.md).
