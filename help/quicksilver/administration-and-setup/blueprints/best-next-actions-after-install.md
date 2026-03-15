---
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Azioni da intraprendere dopo l’installazione di un progetto
description: Questo articolo descrive le operazioni da eseguire dopo l'installazione di un progetto in [!DNL Adobe Workfront] per distribuire completamente il progetto agli utenti del sistema.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 6e5da58f-105a-4edf-8fc1-65e8762d43c6
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '1135'
ht-degree: 0%

---

# Azioni da intraprendere dopo l’installazione di una blueprint

Questo articolo descrive le operazioni da eseguire dopo l&#39;installazione di un progetto in [!DNL Adobe Workfront] per distribuire completamente il progetto agli utenti del sistema.

* [Suggerimenti per i modelli di progetto](#project-template-recommendations)
* [Raccomandazioni sulla struttura organizzativa](#organizational-structure-recommendations)
* [Consigli sul dashboard](#dashboard-recommendations)

## Suggerimenti per i modelli di progetto {#project-template-recommendations}

Questa sezione contiene consigli sui modelli di progetto installati con i progetti.

### Assegnare gli utenti ai nuovi ruoli e team {#assign-users-to-newly-created-roles-and-teams}

Ai ruoli e/o ai team creati durante il processo di installazione del progetto non sono associati automaticamente utenti. Senza assegnare gli utenti ai ruoli o ai team appena aggiunti, si creerà lavoro per una funzione che nessuno sceglierà. In alcuni casi, potrebbe essere necessario creare nuovi utenti per assegnare questi ruoli e team. Per informazioni sulla creazione di nuovi utenti, vedere [Aggiungere utenti](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

### Applicare un modulo personalizzato al modello e alle attività del modello {#apply-a-custom-form-to-the-template-and-the-template-tasks}

Il processo di installazione non associa il modello di progetto ad alcun modulo personalizzato. Se i progetti o le attività richiedono moduli o campi specifici da compilare per garantire la coerenza delle relazioni o se il modulo di richiesta digitale contiene campi che devono essere conservati a livello di progetto, è consigliabile associare il modello o le attività modello a tali moduli. Per informazioni, vedere [Aggiungere un modulo personalizzato a un oggetto](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

### Aggiornamento delle stime della durata e dell&#39;impegno dell&#39;attività del modello {#update-template-task-duration-and-effort-estimates}

Ogni attività nel modello contiene una durata pianificata e una stima dell&#39;impegno pianificato. Queste stime fungono da punto di partenza per le durate e il tempo impiegato per queste attività. Tuttavia, le funzionalità, le competenze e il ritmo della tua organizzazione sono unici. È necessario rivedere la durata stimata e lo sforzo di ciascuna attività per adattarla alle esigenze dell&#39;organizzazione. Per informazioni, vedere [Gestire le informazioni sulle attività nell&#39;area [!UICONTROL Panoramica dei dettagli delle attività]](../../manage-work/tasks/manage-tasks/task-information-in-overview.md).

### Associare un percorso e le attività cardine {#associate-a-milestone-path-and-milestones}

Il processo di installazione non associa il modello di progetto a un percorso cardine. Applicare un percorso cardine al modello e applicare cardine alle attività chiave del modello per supportare le esigenze di reporting delle attività cardine. Per informazioni, vedere [Associare attività cardine alle attività](../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

### Distribuisci il modello nel team {#roll-out-the-template-to-your-team}

Prepara materiali di formazione sia per i responsabili del lavoro che utilizzeranno questo modello sia per i singoli collaboratori che eseguiranno il lavoro all&#39;interno del modello di progetto.

### Creazione o aggiornamento di report e dashboard {#create-or-update-reports-and-dashboards}

Se la soluzione rappresenta un nuovo tipo di lavoro che l&#39;organizzazione non ha eseguito in precedenza in [!DNL Workfront], potrebbe essere necessario creare nuovi report e dashboard per supportare il lavoro. Per informazioni, vedere [Creare un report personalizzato](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) e [Creare un dashboard](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

Se la soluzione è simile al lavoro già eseguito in [!DNL Workfront], è necessario verificare che il lavoro venga inserito nei report e nei dashboard esistenti come previsto. Se il report non viene inserito in quello esistente, esegui un’azione per aggiornare i filtri o creare nuovi report.

## Raccomandazioni sulla struttura organizzativa {#organizational-structure-recommendations}

Questa sezione contiene consigli sugli elementi della struttura organizzativa installati con i progetti.

### Aziende

Dopo aver installato un progetto che include una società:

* Aggiungi un modulo personalizzato per aggiungere ulteriori dettagli utili al record aziendale (il modulo e i relativi dettagli sono specifici per te). Per informazioni, vedere [Aggiungere un modulo personalizzato a un oggetto](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).
* Se l&#39;azienda rappresenta un cliente, esaminare i tassi di sostituzione associati all&#39;azienda. Per informazioni, vedere [Sostituire le tariffe di fatturazione del ruolo di processo a livello aziendale](../../administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).
* Se l&#39;azienda rappresenta un cliente e sono disponibili altri modelli di progetto univoci per tale organizzazione, è necessario innanzitutto associare i modelli di progetto all&#39;azienda appena aggiunta. Per informazioni, vedere [Modificare i modelli di progetto](../../manage-work/projects/create-and-manage-templates/edit-templates.md).
* Se l&#39;azienda rappresenta un cliente o un fornitore, associa gli utenti esistenti dell&#39;organizzazione esterna che potrebbero essere già presenti nel tuo ambiente. Per informazioni, vedere [Creare e modificare società](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).
* Se l&#39;azienda rappresenta un cliente o un fornitore, creare ulteriori utenti di collaboratore per l&#39;organizzazione esterna necessaria nell&#39;ambiente per semplificare le comunicazioni, l&#39;esecuzione del lavoro e le approvazioni. Per informazioni sulla creazione di nuovi utenti, vedere [Aggiungere utenti](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).
* Aggiorna le relazioni tra gli organigrammi per tutti gli utenti ora associati alla società appena aggiunta. Per informazioni, vedere [Creazione di report diretti](../../administration-and-setup/add-users/create-and-manage-users/create-direct-reports.md) e [Visualizzazione dell&#39;organigramma](../../people-teams-and-groups/work-directly-with-others/view-the-org-chart.md).

Per ulteriori informazioni sulle aziende, vedere [Creazione e modifica di aziende](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

## Consigli sul dashboard {#dashboard-recommendations}

Questa sezione contiene consigli per i dashboard e i report installati con un progetto.

### Aggiorna i dashboard appena creati per aggiungere/rimuovere report

I dashboard aggiunti da un progetto dispongono di uno o più report, pagine esterne o calendari. È probabile che non siano necessari tutti i report e gli altri elementi del dashboard oppure che sia necessario aggiungere al dashboard report esistenti, pagine esterne e calendari prima che sia pronto per la condivisione con altri utenti. Per informazioni, vedere [Aggiungere un report a un dashboard](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/add-report-dashboard.md).

### Aggiorna i report appena creati per aggiungere/rimuovere colonne o criteri di filtro

I report distribuiti tramite un progetto del dashboard non dispongono di tutte le colonne o dei criteri di filtro per supportare la configurazione di [!DNL Workfront]. Si prevede che verranno apportate alcune modifiche ai report in modo che siano in linea con gli standard. Per garantire la coerenza con altri report dell&#39;ambiente, è possibile aggiungere una colonna da includere in tutti i report per l&#39;oggetto elencato oppure alcuni criteri di filtro che limitano i risultati a un tipo di progetto o a un gruppo di utenti specifico. Per informazioni, vedere [Creare o modificare visualizzazioni](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md) e [Creare o modificare filtri](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

### Condividere dashboard o report con gli utenti

Se non si prevede di inserire il dashboard in un modello di layout, è consigliabile condividerlo con gli utenti che lo riterranno utile. Per informazioni, vedere [Condividere un dashboard](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md) e [Condividere un report](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

### Aggiungere i dashboard ai modelli di layout

Il modo migliore per rendere le informazioni disponibili agli altri utenti consiste nell&#39;aggiungere dashboard ai modelli di layout. Identificare i modelli di layout delle persone che trarrebbero maggiore vantaggio dalla revisione regolare del dashboard e aggiungere il dashboard appena creato a tali modelli di layout. Per informazioni, vedere [Creare e gestire modelli di layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

### Aggiornare altri dashboard e report

L’introduzione di un nuovo dashboard e dei relativi report può rendere possibile la rimozione e la modifica di altri dashboard e report esistenti. Prendetevi il tempo di esaminare i rapporti esistenti per individuare quelli ridondanti e contraddittori.

### Distribuire dati personalizzati nei moduli pertinenti

Alcuni report inclusi in una bozza del dashboard dispongono di campi dati personalizzati nella visualizzazione, nel filtro o nel raggruppamento del report. In alcuni casi, il modello includerà anche un modulo a cui sono associati questi campi. Nella maggior parte dei casi, tuttavia, i campi personalizzati non vengono applicati a un modulo personalizzato. Affinché le colonne, i filtri o i raggruppamenti funzionino correttamente, questi campi devono essere associati a moduli collegati a un record utente, progetto, attività o altro record oggetto. Per informazioni, vedere [Creare un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
