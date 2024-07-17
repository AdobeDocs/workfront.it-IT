---
title: 21.4 Miglioramenti per gli amministratori
description: 21.4 Miglioramenti per gli amministratori
author: Luke
draft: Probably
feature: Product Announcements, System Setup and Administration
recommendations: noDisplay, noCatalog
exl-id: fc85b4c2-4a76-4226-9120-11635b03aa4e
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1891'
ht-degree: 0%

---

# 21.4 Miglioramenti per gli amministratori

Questa pagina descrive tutti i miglioramenti per gli amministratori apportati con la versione 21.4 all’ambiente di anteprima. Questi miglioramenti saranno resi disponibili nell’ambiente di produzione la settimana del 4 ottobre 2021.

Per un elenco di tutte le modifiche disponibili con la versione 21.4, consulta la [Panoramica sulla versione 21.4](../../../product-announcements/product-releases/21.4-release-activity/21-4-release-overview.md).

## Per gli amministratori: scopri i gruppi associati a un processo di approvazione

Per aiutarti a individuare i gruppi associati ai processi di approvazione nel tuo sistema, abbiamo aggiunto una colonna Nome gruppo alla vista Standard nella pagina Approvazioni in Configurazione. Ora è possibile visualizzare queste informazioni senza dover creare una visualizzazione personalizzata.

Per informazioni sui processi di approvazione, vedere [Panoramica sui processi di approvazione](../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

Per informazioni sulla gestione dei processi di approvazione del gruppo, vedere [Processi di approvazione a livello di gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md).

## Novità per gli amministratori: i gruppi possono configurare le proprie preferenze per le ore e le schede orario

>[!NOTE]
>
>Inizialmente, in Produzione, questa funzionalità sarà disponibile come parte di un rollout graduale solo per i clienti sul Cluster 4. Questa nota verrà aggiornata man mano che la funzionalità sarà disponibile per altri cluster.

In un’organizzazione di grandi dimensioni, alcuni gruppi potrebbero dover configurare le preferenze delle ore e delle schede orario in modo indipendente per adattarsi ai propri flussi di lavoro univoci, anziché ereditare le preferenze configurate da un amministratore a livello di sistema. Ora gli amministratori di Workfront possono sbloccare una scheda orario e una preferenza per le ore per tutti i gruppi del sistema in modo da poterla configurare autonomamente.

Questa funzionalità è stata aggiunta di recente anche per le preferenze del progetto e per le preferenze di attività e problemi.

Per informazioni su come un amministratore di Workfront sblocca una preferenza di tipo scheda orario e ora, vedere la sezione [Sbloccare le preferenze di tipo scheda orario e ora per i gruppi](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md#lock) nell&#39;articolo [Configurare le preferenze di tipo scheda orario e ora](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Per informazioni su come un amministratore di gruppo configura le attività sbloccate e le preferenze relative ai problemi per un gruppo, vedere [Configurare le preferenze relative alle ore e alle schede orario per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

## Novità per gli amministratori di Workfront: configura modelli di layout per gli utenti con provisioning automatico nella nuova esperienza Workfront

Ora puoi configurare i modelli di layout nella nuova esperienza Workfront per gli utenti con provisioning automatico. Nel menu a discesa Attributi utente di Workfront in cui mappate gli attributi utente (Configurazione > Sistema > Single Sign-On), è ora disponibile una nuova voce di menu &quot;Nuovo modello di layout&quot; per effettuare questa configurazione. In precedenza, era possibile configurare modelli di layout per gli utenti con provisioning automatico solo in Workfront Classic.

Per istruzioni sulla mappatura degli attributi utente, consulta [Mappare gli attributi utente ed eseguire il provisioning automatico dei nuovi utenti](../../../administration-and-setup/add-users/create-and-manage-users/map-user-attributes.md).

## Nel nuovo campo vengono visualizzati i gruppi a cui appartengono gli utenti

Ora è facile scoprire a quali gruppi appartengono i tuoi utenti. In un report o in una visualizzazione in cui sono elencati gli utenti, è possibile creare una colonna utilizzando il nuovo campo Altri gruppi. Questo campo elenca i gruppi di cui è membro ogni utente.

Per informazioni sull&#39;utilizzo di report e visualizzazioni, vedere [Creare un report personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) e [Visualizzazioni in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## Nella pagina dei dettagli Blueprint viene ora visualizzata un’immagine

Nella pagina dei dettagli di ogni blueprint ora viene visualizzata un’immagine del modello di progetto installato con la blueprint. L’immagine fornisce un’anteprima del contenuto della blueprint in modo da sapere cosa stai per installare. Facoltativamente, puoi visualizzare l’anteprima dell’immagine completa nel browser o scaricarla.

Per ulteriori informazioni, consulta [Panoramica blueprint](../../../administration-and-setup/blueprints/blueprints-overview.md).

![](assets/blueprint-detailspage.png)

## Preferenze blueprint per nuovi problemi

Sono ora disponibili nuove preferenze per alcuni blueprint. Vengono installati per impostazione predefinita, ma è possibile rinunciare all’installazione delle preferenze quando si configurano i dettagli di installazione.

Le preferenze includono gruppi di argomenti della coda, argomenti della coda e regole di routing per raccogliere le informazioni corrette quando viene inviato un problema o una richiesta e inviare il problema o la richiesta alla mansione o al team corretti. L’utilizzo delle preferenze consente di creare coerenza nel modo in cui i nuovi problemi o richieste vengono acquisiti sui progetti.

L’utilizzo di queste preferenze non fa sì che i progetti creati dal modello vengano inseriti nelle code di richiesta.

Per ulteriori informazioni, vedere [Configurare una blueprint](../../../administration-and-setup/blueprints/configure-template-package.md).

## Novità per gli amministratori di gruppi: visualizzazione e gestione degli elementi eliminati e ripristinati di recente in un gruppo

>[!NOTE]
>
>Questa funzione è disponibile solo nella nuova esperienza Adobe Workfront.

Stiamo continuando a semplificare la gestione dei gruppi e degli oggetti associati in un’unica posizione. Ora puoi visualizzare e lavorare con gli elementi eliminati e ripristinati di recente da un gruppo dall’area Gruppi. In questo modo è possibile evitare di dover passare all&#39;area Recently Deleted o Recently Restored in Configurazione per gestire tali elementi. Inoltre, l&#39;elenco degli elementi del gruppo con cui si sta lavorando è separato dagli altri elementi eliminati e ripristinati nel sistema.

Per ulteriori informazioni, vedere [Visualizzare e gestire gli elementi eliminati di recente da un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-deleted-objects.md) e [Visualizzare e gestire gli elementi ripristinati di recente da un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-restored-objects.md).

## Novità per gli amministratori di gruppi: le preferenze di gruppo ora influiscono sui modelli di gruppo

È ora più semplice assicurarsi che i modelli di progetto del gruppo soddisfino le esigenze del gruppo. Quando si assegna un nuovo modello di progetto a un gruppo al momento della creazione, il modello eredita le impostazioni seguenti dalle preferenze di progetto e attività del gruppo:

* Metodo indice prestazioni
* Tipo di condizione
* Pianifica da
* Indisponibilità utente
* Tipo di aggiornamento
* Impostazioni sezione di accesso

Quando si crea una nuova attività modello all&#39;interno di un modello di progetto associato a un gruppo, l&#39;attività modello eredita le impostazioni seguenti dalle preferenze attività del gruppo:

* Tipo di Durata
* Tipo di Reddito
* Tipo Cst

In precedenza, i modelli di progetto e le attività dei modelli di progetto ereditavano queste impostazioni dalle preferenze di progetto e attività impostate a livello di sistema.

Se si crea un modello o un&#39;attività modello senza un gruppo, ad esempio dalla pagina principale Modelli, le impostazioni di cui sopra vengono ereditate dalle preferenze di progetto e attività a livello di sistema. Tuttavia, se in seguito si assegna un gruppo all&#39;attività modello o modello, le preferenze del gruppo non hanno effetto su di esso.

Per ulteriori informazioni, vedere la sezione Applicazione delle preferenze ai modelli e alle attività modello nell&#39;articolo [Creare e modificare i modelli di progetto di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).

## Novità per gli amministratori: scopri i moduli personalizzati che utilizzano un campo personalizzato

Ora è più semplice modificare un campo personalizzato in un modulo personalizzato. Con un solo clic nel modulo personalizzato, puoi scoprire tutti gli altri moduli personalizzati che utilizzano il campo. È importante valutare se tali moduli avranno bisogno di modifiche per continuare a funzionare correttamente dopo la modifica.

Per ulteriori informazioni, vedere [Visualizzare tutti i moduli personalizzati che utilizzano un determinato campo personalizzato o widget](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-custom-forms-that-use-a-particular-custom-field.md).

## Novità per gli amministratori di gruppi: blocco e sblocco delle preferenze di progetto, attività e problema per un gruppo

Ora puoi fare in modo che tutti gli utenti dei sottogruppi sotto il gruppo utilizzino le stesse impostazioni di preferenza, oppure puoi consentire loro di configurare un’impostazione di preferenza per i loro flussi di lavoro univoci.

* Dopo che un amministratore di Workfront ha sbloccato una preferenza a livello di sistema, è possibile configurarla e quindi bloccarla per tutti i sottogruppi del gruppo. Anche se è ancora possibile riconfigurare la preferenza bloccata, gli amministratori dei sottogruppi inferiori non possono farlo per i loro gruppi.

  Al contrario, è possibile sbloccare una preferenza per il gruppo. Questo consente agli amministratori di sottogruppi di configurarlo in base alle esigenze specifiche di progetto, attività o flusso di lavoro dei problemi dei propri utenti.

  Per ulteriori informazioni, vedere [Bloccare o sbloccare un progetto, un&#39;attività o una preferenza di problema per i sottogruppi](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).

* Se sei un amministratore di Workfront, non è necessario passare all’area Gruppi per configurare le preferenze di un sottogruppo. Nell’area principale Preferenze progetto, Preferenze attività e problemi o Preferenze schede orario e ore puoi utilizzare la casella di ricerca nella parte superiore della pagina per trovare il sottogruppo e configurarne le preferenze.

  Per ulteriori informazioni, consulta [Configurare le preferenze del progetto per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) e [Configurare le preferenze per attività e problemi per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

## Novità per gli amministratori di gruppi: creare e modificare modelli dall’area Gruppi

>[!NOTE]
>
>Questa funzione è disponibile solo nella nuova esperienza Workfront.

Stiamo continuando a semplificare la gestione dei gruppi e degli oggetti associati in un&#39;unica posizione. Ora è possibile visualizzare e lavorare con i modelli di un gruppo dall’area Gruppi in Configurazione. In questo modo non è più necessario passare all&#39;area Modelli per gestire i modelli di un gruppo. Inoltre, l&#39;elenco dei modelli di gruppo su cui si sta lavorando è separato dagli altri in tutto il sistema.

Per ulteriori informazioni, vedere [Creare e modificare i modelli di progetto di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).

## Immetti e salva le informazioni in un modulo personalizzato allegato alla volta

>[!NOTE]
>
>Questa funzione è disponibile solo nella nuova esperienza Adobe Workfront.

È ora più semplice fornire informazioni nella sezione Dettagli per un oggetto: digita e salva le informazioni in un singolo campo personalizzato o in un&#39;area espandibile (ad esempio Panoramica e Dati finanziari), anche se i campi obbligatori in altri moduli personalizzati sull&#39;oggetto non sono ancora stati compilati.

In precedenza, quando si immettevano informazioni in un modulo personalizzato o in un&#39;area espandibile per un oggetto, tutti i moduli personalizzati allegati all&#39;oggetto entravano in modalità di modifica e tutti i campi obbligatori dovevano essere completati prima di poter salvare le modifiche. Si è verificato un problema se non è stato possibile completare un campo obbligatorio perché destinato a un altro utente.

Se si desidera modificare tutti i moduli personalizzati e le aree espandibili nella sezione Dettagli di un oggetto, è possibile fare clic su Modifica tutto nel nuovo menu Modifica aggiunto all&#39;icona Modifica. In alternativa, è possibile scegliere un nome dallo stesso menu per scorrere fino al modulo o alla sezione personalizzata in cui si desidera apportare le modifiche

>[!NOTE]
>
>Questa funzione è stata originariamente rilasciata in Anteprima con la versione 21.3.

Per semplificare la gestione e il controllo indipendente dei flussi di lavoro da parte di tutti i livelli dell’organizzazione, è stata introdotta la possibilità di creare e gestire gli stati dei sottogruppi. Ora, dalla sezione Gruppi in Configurazione, è possibile effettuare le seguenti operazioni per i gruppi che si amministrano a qualsiasi livello:

* Creare, modificare, eliminare e nascondere uno stato per un gruppo
* Blocca uno stato per qualsiasi gruppo in modo che tutti i sottogruppi inferiori possano utilizzarlo nello stesso modo
* Sblocca uno stato per qualsiasi gruppo in modo che gli amministratori dei sottogruppi inferiori possano personalizzarlo in base alle loro esigenze specifiche
* Impostare uno stato di gruppo come predefinito
* Riordinare e nascondere la visualizzazione degli stati dei gruppi sugli oggetti

Anche gli amministratori di Workfront possono eseguire queste operazioni (per tutti i gruppi).

In precedenza, questa funzionalità era disponibile solo per i gruppi di primo livello.

Per ulteriori informazioni, vedere [Gestire gli stati dei gruppi](../../../administration-and-setup/manage-groups/manage-group-statuses/manage-group-statuses.md).

## Novità per gli amministratori di Workfront: migrazione autonoma dei modelli di layout da Workfront Classic alla nuova esperienza Workfront

>[!NOTE]
>
>Questa funzione è stata rilasciata nell’ambiente di anteprima il 1° luglio 2021. Verrà rilasciato nell’ambiente di produzione il 15 luglio 2021.

Per aiutarti a gestire i modelli di layout quando gli utenti passano all’utilizzo della nuova esperienza Workfront, abbiamo creato un pulsante che puoi utilizzare per migrare i modelli di layout da Workfront Classic alla nuova esperienza senza affidarti all’Assistenza clienti di Workfront.

In precedenza, solo l’Assistenza clienti Workfront poteva migrare i modelli di layout da Workfront Classic alla nuova esperienza Workfront.

## Quando si associa un modello a un gruppo, selezionare un processo di approvazione di gruppo in Dettagli coda e Argomenti coda

È stata aggiunta una nuova opzione al processo di associazione di un modello a un gruppo. Ora è possibile selezionare i processi di approvazione specifici del gruppo per i problemi nei Dettagli coda del modello o in uno dei relativi Argomenti coda.

Nella versione 21.3, quando è stata aggiunta la possibilità di associare un modello di gruppo a un gruppo, è possibile selezionare un processo di approvazione specifico per il gruppo nel modello, ma non è possibile farlo nei Dettagli coda o Argomenti coda del modello.

Per ulteriori informazioni, vedere [Associa un processo di approvazione nuovo o esistente a un lavoro](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
