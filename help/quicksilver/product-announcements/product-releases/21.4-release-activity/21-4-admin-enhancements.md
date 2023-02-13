---
title: Miglioramenti dell’amministratore 21.4
description: Miglioramenti dell’amministratore 21.4
author: Luke
draft: Probably
feature: Product Announcements, System Setup and Administration
exl-id: fc85b4c2-4a76-4226-9120-11635b03aa4e
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '1882'
ht-degree: 0%

---

# Miglioramenti dell’amministratore 21.4

Questa pagina descrive tutti i miglioramenti apportati dall’amministratore all’ambiente Preview con la versione 21.4. Questi miglioramenti saranno resi disponibili nell&#39;ambiente di produzione la settimana del 4 ottobre 2021.

Per un elenco di tutte le modifiche disponibili con la versione 21.4, vedi [Panoramica sulla versione 21.4](../../../product-announcements/product-releases/21.4-release-activity/21.4-release-overview.md).

## Per gli amministratori: Vedere quali gruppi sono associati a un processo di approvazione

Per identificare i gruppi associati ai processi di approvazione del sistema, è stata aggiunta una colonna Nome gruppo alla visualizzazione Standard nella pagina Approvazioni in Configurazione. Ora è possibile visualizzare queste informazioni senza dover creare una visualizzazione personalizzata.

Per informazioni sui processi di approvazione, consulta [Panoramica del processo di approvazione](../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

Per informazioni sulla gestione dei processi di approvazione dei gruppi, consulta [Processi di approvazione a livello di gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md).

## Novità per gli amministratori: I gruppi possono configurare le proprie preferenze per la scheda attività e l&#39;ora

>[!NOTE]
>
>Inizialmente, in Produzione, questa funzionalità sarà disponibile come parte di un rollout graduale solo per i clienti sul cluster 4. Questa nota verrà aggiornata man mano che la funzionalità diventa disponibile per altri cluster.

In un&#39;organizzazione di grandi dimensioni, alcuni gruppi potrebbero dover configurare le preferenze relative alla scheda attività e alle ore in modo indipendente per adattarsi ai flussi di lavoro univoci, anziché ereditare le preferenze configurate da un amministratore a livello di sistema. Ora gli amministratori di Workfront possono sbloccare una scheda attività e una preferenza oraria per tutti i gruppi del sistema in modo che possano configurarla autonomamente.

Questa funzionalità è stata aggiunta di recente anche per le preferenze del progetto e per le preferenze relative a attività ed emissioni.

Per informazioni su come un amministratore di Workfront sblocca una scheda attività e una preferenza oraria, consulta la sezione . [Sblocca le preferenze della scheda attività e dell&#39;ora per i gruppi](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md#lock) nell&#39;articolo [Configurare le preferenze relative a schede attività e ora](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Per informazioni su come un amministratore di gruppo configura l&#39;attività sbloccata e genera le preferenze per un gruppo, consulta [Configurare le preferenze relative a schede attività e ora per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

## Novità per gli amministratori di Workfront: Configurare modelli di layout per gli utenti con provisioning automatico nella nuova esperienza Workfront

Ora è possibile configurare modelli di layout nella nuova esperienza Workfront per gli utenti con provisioning automatico. Nel menu a discesa Attributo utente Workfront in cui mappate gli attributi utente (Configurazione > Sistema > Single Sign-On), è ora disponibile una nuova voce di menu &quot;Modello di layout NWE&quot; per effettuare questa configurazione. In precedenza, era possibile configurare modelli di layout per gli utenti con provisioning automatico solo in Workfront Classic.

Per istruzioni sulla mappatura degli attributi utente, consulta [Mappatura degli attributi utente e provisioning automatico dei nuovi utenti](../../../administration-and-setup/add-users/create-and-manage-users/map-user-attributes.md).

## Nuovo campo visualizza i gruppi a cui appartengono gli utenti

Ora è facile scoprire a quali gruppi appartengono i tuoi utenti. In un rapporto o in una visualizzazione in cui sono elencati gli utenti, è possibile creare una colonna utilizzando il nuovo campo Altri gruppi . Questo campo elenca i gruppi in cui ogni utente è membro.

Per informazioni sull’utilizzo dei rapporti e delle visualizzazioni, consulta [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) e [Panoramica delle visualizzazioni in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## La pagina dei dettagli Blueprint ora visualizza un&#39;immagine

Nella pagina dei dettagli di ogni blueprint viene ora visualizzata un’immagine del modello di progetto installato con la blueprint. L&#39;immagine fornisce un&#39;anteprima del contenuto della blueprint in modo che tu sappia cosa stai per installare. Facoltativamente, puoi visualizzare in anteprima l&#39;immagine completa nel browser o scaricare l&#39;immagine.

Per ulteriori informazioni, consulta [Panoramica delle blueprint](../../../administration-and-setup/blueprints/blueprints-overview.md).

![](assets/blueprint-detailspage.png)

## Preferenze Blueprint per nuovi problemi

Per alcune blueprint sono ora disponibili nuove preferenze per i problemi. Sono installati per impostazione predefinita, ma puoi scegliere di non installare le preferenze quando configuri i dettagli di installazione.

Le preferenze includono gruppi di argomenti della coda, argomenti della coda e regole di indirizzamento per raccogliere le informazioni corrette quando viene inviato un problema o una richiesta e inviare il problema o la richiesta al ruolo o al team di lavoro corretto. L’utilizzo delle preferenze consente di creare coerenza nel modo in cui i nuovi problemi o richieste vengono acquisiti sui progetti.

Tieni presente che l’utilizzo di queste preferenze non trasforma i progetti creati dal modello in code di richiesta.

Per ulteriori informazioni, consulta [Configurare una blueprint](../../../administration-and-setup/blueprints/configure-template-package.md).

## Novità per gli amministratori dei gruppi: Visualizzare e gestire gli elementi eliminati e ripristinati di recente di un gruppo

>[!NOTE]
>
>Questa funzione è disponibile solo nella nuova esperienza Adobe Workfront.

Stiamo continuando a semplificare la gestione dei gruppi e degli oggetti associati in un’unica posizione. Ora è possibile visualizzare e lavorare con gli elementi eliminati e ripristinati di recente da un gruppo dall&#39;area Gruppi. In questo modo non dovrai passare all’area Eliminato di recente o Ripristinato di recente in Configurazione per gestire tali elementi. E mantiene l&#39;elenco degli elementi del gruppo con cui si sta lavorando separatamente dagli altri elementi cancellati e ripristinati nel sistema.

Per ulteriori informazioni, consulta [Visualizzare e gestire gli elementi eliminati di un gruppo di recente](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-deleted-objects.md) e [Visualizzare e gestire gli elementi ripristinati di recente di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-restored-objects.md).

## Novità per gli amministratori dei gruppi: Le preferenze del gruppo ora influiscono sui modelli di gruppo

È ora più facile assicurarsi che i modelli di progetto del gruppo soddisfino le esigenze del gruppo. Quando si assegna un nuovo modello di progetto a un gruppo al momento della creazione, il modello eredita le seguenti impostazioni dalle preferenze di progetto e attività del gruppo:

* Metodo Indicizzazione Performance
* Tipo di Condizione
* Pianificazione da
* Tempo di inattività dell&#39;utente
* Tipo di aggiornamento
* Accedere alle impostazioni della sezione

Quando si crea una nuova attività modello all&#39;interno di un modello di progetto associato a un gruppo, l&#39;attività modello eredita le seguenti impostazioni dalle preferenze dell&#39;attività del gruppo:

* Tipo di Durata
* Tipo di Reddito
* Tipo Cst

In precedenza, i modelli di progetto e le attività dei modelli di progetto ereditavano queste impostazioni dalle preferenze di progetto e attività impostate a livello di sistema.

Se si crea un modello o un&#39;attività modello senza un gruppo, ad esempio dalla pagina Modelli principale, le impostazioni di cui sopra vengono ereditate dalle preferenze di progetto e attività a livello di sistema. Tuttavia, se successivamente si assegna un gruppo all&#39;attività modello o modello, le preferenze del gruppo non lo influiscono.

Per ulteriori informazioni, consulta la sezione Modalità di applicazione delle preferenze ai modelli e alle attività dei modelli nell’articolo [Creare e modificare i modelli di progetto di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).

## Novità per gli amministratori: Individuazione dei moduli personalizzati che utilizzano un campo personalizzato

Ora è più semplice modificare un campo personalizzato in un modulo personalizzato. Con un solo clic nel modulo personalizzato è possibile trovare informazioni su qualsiasi altro modulo personalizzato che utilizza anche il campo . È importante valutare se tali moduli necessitano di regolazioni per poter continuare a funzionare correttamente dopo aver apportato le modifiche.

Per ulteriori informazioni, consulta [Visualizza tutti i moduli personalizzati che utilizzano un campo o un widget personalizzato specifico](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-custom-forms-that-use-a-particular-custom-field.md).

## Novità per gli amministratori dei gruppi: Blocca e sblocca le preferenze di progetto, attività ed emissione di un gruppo

Ora puoi verificare che tutti i sottogruppi del gruppo utilizzino le stesse impostazioni di preferenza oppure puoi consentire loro di configurare un’impostazione di preferenza per i propri flussi di lavoro univoci.

* Dopo che un amministratore di Workfront sblocca una preferenza a livello di sistema, puoi configurarla e bloccarla per tutti i sottogruppi del gruppo. Anche se è ancora possibile riconfigurare la preferenza bloccata, gli amministratori dei sottogruppi inferiori non possono farlo per i loro gruppi.

   Al contrario, puoi sbloccare una preferenza per il gruppo. Questo consente agli amministratori dei sottogruppi di configurarlo per i progetti, le attività o i problemi specifici del flusso di lavoro degli utenti.

   Per ulteriori informazioni, consulta [Bloccare o sbloccare un progetto, un&#39;attività o una preferenza di problema per i sottogruppi](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).

* Se sei un amministratore di Workfront, non è necessario accedere all’area Gruppi per configurare le preferenze di un sottogruppo. Nell’area Preferenze progetto principale, Preferenze attività e problemi o Preferenze foglio presenze e ore è possibile utilizzare la casella di ricerca nella parte superiore della pagina per trovare il sottogruppo e configurarne le preferenze.

   Per ulteriori informazioni, consulta [Configurare le preferenze di progetto per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) e [Configurare le preferenze per attività e problemi per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

## Novità per gli amministratori dei gruppi: Creare e modificare modelli dall’area Gruppi

>[!NOTE]
>
>Questa funzione è disponibile solo nella nuova esperienza Workfront.

Continuiamo a semplificare la gestione dei gruppi e degli oggetti associati in un’unica posizione. Ora è possibile visualizzare e utilizzare i modelli di un gruppo dall’area Gruppi in Configurazione. In questo modo non dovrai passare all’area Modelli per gestire i modelli di un gruppo. E mantiene l&#39;elenco dei modelli di gruppo su cui stai lavorando separatamente dagli altri in tutto il sistema.

Per ulteriori informazioni, consulta [Creare e modificare i modelli di progetto di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).

## Immettere e salvare le informazioni in un modulo personalizzato allegato alla volta

>[!NOTE]
>
>Questa funzione è disponibile solo nella nuova esperienza Adobe Workfront.

È ora più semplice fornire informazioni nella sezione Dettagli per un oggetto: Digitare e salvare le informazioni in un singolo campo personalizzato o in un’area espandibile (ad esempio Panoramica e Contabilità), anche se i campi obbligatori in altri moduli personalizzati dell’oggetto non sono ancora stati compilati.

Precedentemente, quando si immettevano informazioni in un modulo personalizzato o in un’area espandibile per un oggetto, tutti i moduli personalizzati associati all’oggetto venivano in modalità di modifica e tutti i campi obbligatori dovevano essere completati prima di salvare le modifiche. Si è verificato un problema se non è stato possibile completare un campo obbligatorio perché era destinato a un altro utente.

Se si desidera modificare tutti i moduli personalizzati e le aree espandibili nella sezione Dettagli di un oggetto, è possibile fare clic su Modifica tutto nel nuovo menu Modifica aggiunto all&#39;icona Modifica. In alternativa, è possibile fare clic su un nome nello stesso menu per scorrere il modulo o la sezione personalizzata in cui si desidera apportare le modifiche

>[!NOTE]
>
>Questa funzione è stata originariamente rilasciata in Anteprima con la versione 21.3.

Per semplificare la gestione e il controllo indipendente dei flussi di lavoro da parte di tutti i livelli di un’organizzazione, abbiamo introdotto la possibilità di creare e gestire gli stati per i sottogruppi. Ora, dalla sezione Gruppi in Configurazione, è possibile effettuare le seguenti operazioni per i gruppi amministrati a qualsiasi livello:

* Creare, modificare, eliminare e nascondere uno stato per un gruppo
* Blocca uno stato per qualsiasi gruppo in modo che tutti i sottogruppi inferiori al gruppo possano utilizzarlo allo stesso modo
* Sblocca uno stato per qualsiasi gruppo in modo che gli amministratori dei sottogruppi inferiori possano personalizzarlo per soddisfare le loro esigenze specifiche
* Imposta lo stato predefinito del gruppo
* Riordinare e nascondere la visualizzazione degli stati del gruppo sugli oggetti

Anche gli amministratori di Workfront possono eseguire queste operazioni (per tutti i gruppi).

In precedenza, questa funzionalità era disponibile solo per i gruppi di livello superiore.

Per ulteriori informazioni, consulta [Gestire gli stati dei gruppi](../../../administration-and-setup/manage-groups/manage-group-statuses/manage-group-statuses.md).

## Novità per gli amministratori di Workfront: Migrazione personalizzata dei modelli di layout da Workfront Classic alla nuova esperienza Workfront

>[!NOTE]
>
>Questa funzione è stata rilasciata nell’ambiente Preview il 1° luglio 2021. Verrà rilasciato nell’ambiente di produzione il 15 luglio 2021.

Per facilitare la gestione dei modelli di layout mentre gli utenti passano all’utilizzo della nuova esperienza Workfront, è stato creato un pulsante che consente di migrare i modelli di layout da Workfront Classic alla nuova esperienza senza ricorrere all’Assistenza clienti Workfront.

In precedenza, solo l’Assistenza clienti Workfront poteva migrare i modelli di layout da Workfront Classic alla nuova esperienza Workfront.

## Quando si associa un modello a un gruppo, selezionare un processo di approvazione del gruppo in Dettagli coda e Argomenti coda

È stata aggiunta una nuova opzione al processo di associazione di un modello a un gruppo. Ora è possibile selezionare i processi di approvazione specifici per il gruppo per i problemi nei dettagli della coda del modello o in uno dei relativi argomenti della coda.

In 21.3, quando si aggiunge la possibilità di associare un modello di gruppo a un gruppo, è possibile selezionare un processo di approvazione specifico per gruppo nel modello, ma non è stato possibile farlo in Dettagli coda o Argomenti coda del modello.

Per ulteriori informazioni, consulta [Associa un processo di approvazione nuovo o esistente al lavoro](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
