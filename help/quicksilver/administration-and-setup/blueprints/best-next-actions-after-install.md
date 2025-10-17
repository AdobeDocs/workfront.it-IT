---
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Azioni da intraprendere dopo l’installazione di una blueprint
description: Questo articolo illustra le operazioni da eseguire dopo l'installazione di una blueprint in [!DNL Adobe Workfront] per distribuire completamente la blueprint agli utenti del sistema.
author: Jenny
feature: System Setup and Administration
role: Admin
exl-id: 6e5da58f-105a-4edf-8fc1-65e8762d43c6
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '1135'
ht-degree: 0%

---

# Azioni da intraprendere dopo l’installazione di una blueprint

Questo articolo illustra le operazioni da eseguire dopo l&#39;installazione di una blueprint in [!DNL Adobe Workfront] per distribuire completamente la blueprint agli utenti del sistema.

* [Consigli sui modelli di progetto](#project-template-recommendations)
* [Raccomandazioni sulla struttura organizzativa](#organizational-structure-recommendations)
* [Raccomandazioni dashboard](#dashboard-recommendations)

## Consigli sui modelli di progetto {#project-template-recommendations}

Questa sezione contiene consigli per i modelli di progetto installati con i blueprint.

### Assegnare utenti ai nuovi ruoli e team creati {#assign-users-to-newly-created-roles-and-teams}

Ai ruoli e/o ai team creati durante il processo di installazione blueprint non vengono associati automaticamente utenti. Senza assegnare gli utenti ai nuovi ruoli o team aggiunti, si creerà lavoro per una funzione che nessuno sceglierà. In alcuni casi, potrebbe essere necessario creare nuovi utenti per ricoprire questi ruoli e team. Per informazioni sulla creazione di nuovi utenti, vedere [Aggiungi utenti](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

### Applicare un modulo personalizzato alle attività modello e modello {#apply-a-custom-form-to-the-template-and-the-template-tasks}

Il processo di installazione non associa il modello di progetto ad alcun modulo personalizzato. Se i progetti o le attività richiedono la compilazione di moduli o campi specifici per creare coerenza dei rapporti o se il modulo di richiesta digitale contiene campi che devono essere conservati a livello di progetto, è consigliabile associare le attività modello a tali moduli. Per informazioni, vedere [Aggiungere un modulo personalizzato a un oggetto](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

### Aggiorna le stime della durata e dell&#39;impegno dell&#39;attività del modello {#update-template-task-duration-and-effort-estimates}

Ogni attività del modello contiene una durata pianificata e una stima dell&#39;impegno pianificato. Queste stime fungono da punto di partenza per le durate e il tempo trascorso per queste attività. Tuttavia, le funzionalità, le competenze e il ritmo della tua organizzazione sono unici. È necessario rivedere la durata stimata di ogni attività e lo sforzo per adattarla in modo da riflettere le esigenze della propria organizzazione. Per informazioni, vedere [Gestire le informazioni sull&#39;attività nell&#39;area [!UICONTROL Panoramica dettagli attività]](../../manage-work/tasks/manage-tasks/task-information-in-overview.md).

### Associare un percorso milestone e le milestone {#associate-a-milestone-path-and-milestones}

Il processo di installazione non associa il modello di progetto a un percorso milestone. Applica un percorso milestone al modello e applica i milestone alle attività chiave nel modello per supportare le tue esigenze di reporting milestone. Per informazioni, vedere [Associa attività cardine alle attività](../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

### Eseguire il rollout del modello nel team {#roll-out-the-template-to-your-team}

Prepara materiali di formazione sia per i responsabili del lavoro che utilizzeranno questo modello che per i singoli collaboratori che eseguiranno il lavoro all’interno del modello di progetto.

### Creare o aggiornare rapporti e dashboard {#create-or-update-reports-and-dashboards}

Se la soluzione rappresenta un nuovo tipo di lavoro che l&#39;organizzazione non ha eseguito in precedenza in [!DNL Workfront], potrebbe essere necessario creare nuovi report e dashboard per supportare il lavoro. Per informazioni, vedere [Creare un report personalizzato](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) e [Creare un dashboard](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

Se la soluzione è simile al lavoro già in esecuzione in [!DNL Workfront], è necessario verificare che il lavoro venga inserito nei report e nei dashboard esistenti come previsto. Se non viene inserito nei rapporti esistenti, devi intervenire per aggiornare i filtri o creare nuovi rapporti.

## Raccomandazioni sulla struttura organizzativa {#organizational-structure-recommendations}

Questa sezione contiene consigli per gli elementi della struttura organizzativa installati con i blueprint.

### Aziende

Dopo aver installato una blueprint che include un’azienda:

* Aggiungi un modulo personalizzato per migliorare il record aziendale con dettagli utili (il modulo e i relativi dettagli sono univoci per te). Per informazioni, vedere [Aggiungere un modulo personalizzato a un oggetto](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).
* Se la società rappresenta un cliente, controlla le tariffe di sostituzione associate alla società. Per informazioni, vedere [Sostituire le tariffe di fatturazione dei ruoli a livello aziendale](../../administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).
* Se l’azienda rappresenta un cliente e sono presenti altri modelli di progetto univoci per l’organizzazione, prima associa i modelli di progetto alla società appena aggiunta. Per informazioni, vedere [Modifica modelli di progetto](../../manage-work/projects/create-and-manage-templates/edit-templates.md).
* Se l’azienda rappresenta un cliente o un fornitore, associa gli utenti esistenti dell’organizzazione esterna che potrebbero già trovarsi nell’ambiente. Per informazioni, vedere [Creare e modificare società](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).
* Se l’azienda rappresenta un cliente o un fornitore, crea altri utenti collaboratori per l’organizzazione esterna necessaria nel tuo ambiente per semplificare le comunicazioni, l’esecuzione del lavoro e le approvazioni. Per informazioni sulla creazione di nuovi utenti, vedere [Aggiungi utenti](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).
* Aggiorna le relazioni dell’organigramma per tutti gli utenti ora associati alla società appena aggiunta. Per informazioni, vedere [Creare referenti diretti](../../administration-and-setup/add-users/create-and-manage-users/create-direct-reports.md) e [Visualizzare l&#39;organigramma](../../people-teams-and-groups/work-directly-with-others/view-the-org-chart.md).

Per ulteriori informazioni sulle società, vedere [Creare e modificare le società](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

## Raccomandazioni dashboard {#dashboard-recommendations}

Questa sezione contiene consigli per dashboard e report installati con una blueprint.

### Aggiornare i dashboard appena creati per aggiungere/rimuovere i report

Le dashboard aggiunte da una blueprint dispongono di uno o più rapporti, pagine esterne o calendari. È probabile che non siano necessari tutti i report e gli altri elementi del dashboard oppure che sia necessario integrare il dashboard con report, pagine esterne e calendari esistenti prima che sia pronto per essere condiviso con altri utenti. Per informazioni, vedere [Aggiungere un report a un dashboard](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/add-report-dashboard.md).

### Aggiornare i nuovi rapporti creati per aggiungere/rimuovere colonne o criteri di filtro

I report distribuiti tramite una blueprint del dashboard non dispongono di tutte le colonne o i criteri di filtro per supportare la configurazione di [!DNL Workfront]. È previsto che i rapporti vengano modificati per adattarli agli standard. Per garantire la coerenza con altri rapporti dell’ambiente, è possibile aggiungere una colonna da includere in tutti i rapporti per l’oggetto elencato oppure alcuni criteri di filtro che limitano i risultati a un particolare tipo di progetto o gruppo di utenti. Per informazioni, vedere [Creare o modificare le visualizzazioni](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md) e [Creare o modificare i filtri](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

### Condividere dashboard o report con gli utenti

Se non si prevede di inserire il dashboard in un modello di layout, è consigliabile condividerlo con gli utenti che lo ritengono utile. Per informazioni, vedere [Condividere un dashboard](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md) e [Condividere un report](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

### Aggiungere le dashboard ai modelli di layout

Il modo migliore per rendere le informazioni disponibili ad altri utenti consiste nell’aggiungere dashboard ai modelli di layout. Identifica i modelli di layout delle persone che trarrebbero maggiori vantaggi dalla revisione regolare del dashboard e aggiungi il nuovo dashboard creato a tali modelli di layout. Per informazioni, vedere [Creare e gestire modelli di layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

### Aggiornare altre dashboard e altri rapporti

L’introduzione di una nuova dashboard e dei relativi rapporti può consentire di smantellare e adeguare altre dashboard e rapporti esistenti. Prenditi del tempo per esaminare i rapporti esistenti e individuare quelli superflui e contraddittori.

### Distribuire dati personalizzati ai moduli pertinenti

Alcuni rapporti inclusi in una blueprint del dashboard dispongono di campi dati personalizzati nella visualizzazione, nel filtro o nel raggruppamento del rapporto. In alcuni casi, la blueprint avrà anche un modulo a cui sono associati questi campi. Tuttavia, nella maggior parte dei casi i campi personalizzati non vengono applicati a un modulo personalizzato. Affinché le colonne, i filtri o i raggruppamenti funzionino correttamente, questi campi devono essere associati a maschere connesse a un record utente, progetto, attività o altro oggetto. Per informazioni, vedere [Creare un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
