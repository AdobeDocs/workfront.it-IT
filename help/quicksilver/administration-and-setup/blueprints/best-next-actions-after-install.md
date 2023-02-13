---
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Azioni da intraprendere dopo l’installazione di una blueprint
description: Questo articolo descrive cosa fare dopo aver installato una blueprint in [!DNL Adobe Workfront] per distribuire completamente la blueprint agli utenti del sistema.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 6e5da58f-105a-4edf-8fc1-65e8762d43c6
source-git-commit: d46eb98c443a421f340b1021972ddb89eda1966b
workflow-type: tm+mt
source-wordcount: '1139'
ht-degree: 0%

---

# Azioni da intraprendere dopo l’installazione di una blueprint

Questo articolo descrive cosa fare dopo aver installato una blueprint in [!DNL Adobe Workfront] per distribuire completamente la blueprint agli utenti del sistema.

* [Raccomandazioni sui modelli di progetto](#project-template-recommendations)
* [Raccomandazioni sulla struttura organizzativa](#organizational-structure-recommendations)
* [Raccomandazioni per dashboard](#dashboard-recommendations)

## Raccomandazioni sui modelli di progetto {#project-template-recommendations}

Questa sezione contiene raccomandazioni per i modelli di progetto installati con i progetti.

### Assegnare utenti a ruoli e team appena creati {#assign-users-to-newly-created-roles-and-teams}

I ruoli e/o i team creati durante il processo di installazione della blueprint non dispongono di utenti associati automaticamente. Senza assegnare gli utenti ai nuovi ruoli o team aggiunti, creerai il lavoro per una funzione che nessuno prenderà. In alcuni casi, potrebbe essere necessario creare nuovi utenti per compilare questi ruoli e team. Per informazioni sulla creazione di nuovi utenti, consulta [Aggiungi utenti](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

### Applicare un modulo personalizzato al modello e alle attività del modello {#apply-a-custom-form-to-the-template-and-the-template-tasks}

Il processo di installazione non associa il modello di progetto ad alcun modulo personalizzato. Se i progetti o le attività richiedono la compilazione di moduli o campi specifici per creare coerenza di reporting, oppure se il modulo di richiesta digitale contiene campi che devono essere mantenuti a livello di progetto, è consigliabile associare il modello o le attività del modello a tali moduli. Per informazioni, consulta [Aggiungere un modulo personalizzato a un oggetto](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

### Aggiorna le stime di durata e sforzo dell&#39;attività del modello {#update-template-task-duration-and-effort-estimates}

Ogni attività nel modello contiene una durata pianificata e una stima dello sforzo pianificato. Tali stime fungono da punto di partenza per le durate e il tempo impiegato per queste attività. Tuttavia, le capacità, le competenze e il ritmo della tua organizzazione sono unici. È necessario esaminare la durata e lo sforzo stimati di ogni attività per adattarla in base alle esigenze della propria organizzazione. Per informazioni, consulta [Gestire le informazioni sulle attività nel [!UICONTROL Panoramica dei dettagli attività] area](../../manage-work/tasks/manage-tasks/task-information-in-overview.md).

### Associare un percorso cardine e pietre miliari {#associate-a-milestone-path-and-milestones}

Il processo di installazione non associa il modello di progetto a un percorso cardine. Applica un percorso cardine al modello e applica le tappe fondamentali alle attività chiave nel modello per supportare le tue esigenze di reporting cardine. Per informazioni, consulta [Associa milestone alle attività](../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

### Implementare il modello nel team {#roll-out-the-template-to-your-team}

Prepara i materiali di formazione sia per i responsabili del lavoro che utilizzeranno questo modello sia per i singoli collaboratori che eseguiranno il lavoro all’interno del modello di progetto.

### Creare o aggiornare rapporti e dashboard {#create-or-update-reports-and-dashboards}

Se la soluzione rappresenta un nuovo tipo di lavoro che la tua organizzazione non ha eseguito in precedenza in [!DNL Workfront], potrebbe essere necessario creare nuovi report e dashboard per supportare il lavoro. Per informazioni, consulta [Creare un rapporto personalizzato](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) e [Creare un dashboard](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

Se la soluzione è simile al lavoro che hai già eseguito in [!DNL Workfront], quindi verifica che il lavoro venga inviato nei report e nelle dashboard esistenti come previsto. Se non viene incluso nel reporting esistente, procedi con l’aggiornamento dei filtri o la creazione di nuovi report.

## Raccomandazioni sulla struttura organizzativa {#organizational-structure-recommendations}

Questa sezione contiene raccomandazioni per gli elementi della struttura organizzativa installati con i progetti.

### Aziende

Dopo aver installato un modello che include un&#39;azienda:

* Aggiungi un modulo personalizzato per migliorare il record aziendale con dettagli utili (il modulo e i relativi dettagli sono univoci). Per informazioni, consulta [Aggiungere un modulo personalizzato a un oggetto](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).
* Se la società rappresenta un cliente, controlla i tassi di sostituzione associati alla società. Per informazioni, consulta [Escludere i tassi di fatturazione dei ruoli di lavoro a livello aziendale](../../administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).
* Se l’azienda rappresenta un cliente e sono presenti altri modelli di progetto univoci per organizzazione, prima di tutto, associa i modelli di progetto alla nuova società aggiunta. Per informazioni, consulta [Modificare i modelli di progetto](../../manage-work/projects/create-and-manage-templates/edit-templates.md).
* Se l’azienda rappresenta un client o un fornitore, associa gli utenti esistenti dell’organizzazione esterna che potrebbero essere già presenti nel tuo ambiente. Per informazioni, consulta [Creare e modificare aziende](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).
* Se l’azienda rappresenta un cliente o un fornitore, crea altri utenti collaboratori per l’organizzazione esterna di cui potresti aver bisogno nel tuo ambiente per semplificare la comunicazione, l’esecuzione del lavoro e le approvazioni. Per informazioni sulla creazione di nuovi utenti, consulta [Aggiungi utenti](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).
* Aggiorna le relazioni del grafico organizzativo per tutti gli utenti ora associati alla nuova società aggiunta. Per informazioni, consulta [Creare rapporti diretti](../../administration-and-setup/add-users/create-and-manage-users/create-direct-reports.md) e [Visualizza il grafico organizzativo](../../people-teams-and-groups/work-directly-with-others/view-the-org-chart.md).

Per ulteriori informazioni sulle aziende, consulta [Creare e modificare aziende](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

## Raccomandazioni per dashboard {#dashboard-recommendations}

Questa sezione contiene raccomandazioni per le dashboard e i report installati con una blueprint.

### Aggiornare le dashboard appena create per aggiungere/rimuovere rapporti

Le dashboard aggiunte da una blueprint hanno uno o più rapporti, pagine esterne o calendari. È probabile che non sarà necessario disporre di tutti i report e di altri elementi del dashboard, oppure sarà necessario aumentare il dashboard con i report esistenti, le pagine esterne e i calendari prima che sia pronto per la condivisione con altre persone. Per informazioni, consulta [Aggiungere un rapporto a un dashboard](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/add-report-dashboard.md).

### Aggiornare i report appena creati per aggiungere/rimuovere colonne o filtrare criteri

I report distribuiti tramite una blueprint del dashboard non dispongono di tutte le colonne o di criteri di filtro per supportare la configurazione di [!DNL Workfront]. È previsto che apporti alcune modifiche ai rapporti per adattarli ai tuoi standard. Per garantire la coerenza con gli altri rapporti presenti nell’ambiente, è possibile aggiungere una colonna da includere in tutti i rapporti per l’oggetto elencato o alcuni criteri di filtro che limitano i risultati a un particolare tipo di progetto o gruppo di utenti. Per informazioni, consulta [Creare o modificare visualizzazioni](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md) e [Creare o modificare filtri](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

### Condivisione di dashboard o rapporti con gli utenti

Se non si intende posizionare il dashboard su un modello di layout, è necessario condividerlo con gli utenti che lo riterranno utile. Per informazioni, consulta [Condivisione di un dashboard](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md) e [Condividere un rapporto](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

### Aggiungere le dashboard ai modelli di layout

Il modo migliore per rendere le informazioni disponibili ad altri utenti è quello di aggiungere dashboard ai modelli di layout. Identifica i modelli di layout delle persone che trarrebbero maggior vantaggio dalla revisione regolare del dashboard e aggiungi il dashboard appena creato a tali modelli di layout. Per informazioni, consulta [Creare e gestire modelli di layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

### Aggiornamento di altre dashboard e report

L’introduzione di una nuova dashboard e dei relativi rapporti potrebbe consentire di ritirarsi e modificare altri dashboard e report esistenti. Prenditi del tempo per rivedere i tuoi rapporti esistenti per identificare eventuali relazioni ridondanti e contraddittorie.

### Distribuire dati personalizzati nei moduli pertinenti

Alcuni rapporti inclusi in una blueprint del dashboard presentano campi di dati personalizzati nella visualizzazione, nel filtro o nel raggruppamento del rapporto. In alcuni casi, la blueprint avrà anche un modulo a cui questi campi sono associati. Tuttavia, spesso i campi personalizzati non vengono applicati a un modulo personalizzato. Affinché le colonne, i filtri o i raggruppamenti funzionino correttamente, questi campi devono essere associati a moduli collegati a un utente, a un progetto, a un&#39;attività o a un altro record di oggetti. Per informazioni, consulta [Aggiungere un campo personalizzato a un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md).
