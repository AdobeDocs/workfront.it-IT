---
content-type: release-notes
navigation-topic: product-releases-archive
title: Attività sulla versione 2017.3 di Beta 1
description: Questa pagina descrive tutte le modifiche più recenti disponibili nell’ambiente di anteprima con la versione 2017.3. La funzionalità di questa pagina è stata resa disponibile nell’ambiente di anteprima il 9 agosto 2017. Sarà disponibile nell’ambiente di produzione all’inizio di novembre 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 33a91c25-98ec-4f08-b444-4e11e05e464b
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1426'
ht-degree: 0%

---

# Attività sulla versione 2017.3 di Beta 1

Questa pagina descrive tutte le modifiche più recenti disponibili nell’ambiente di anteprima con la versione 2017.3. La funzionalità di questa pagina è stata resa disponibile nell’ambiente di anteprima il 9 agosto 2017. Sarà disponibile nell’ambiente di produzione all’inizio di novembre 2017.

>[!IMPORTANT]
>
> La funzionalità descritta in questa pagina è soggetta a modifiche prima della disponibilità nell’ambiente di produzione.

Per un elenco di tutte le modifiche apportate nel 2017.3, consulta  Panoramica sull&#39;attività della versione [2017.3](../../../../product-announcements/product-releases/quarterly-release-archive/2017.3-release-activity/2017-3-release-activity-overview.md).

La versione 2017.3 di Beta 1 contiene miglioramenti sia per gli amministratori di Workfront che per altri utenti:

**Per gli amministratori:**

* [Impedisci L&#39;Eliminazione Di Attività E Problemi Durante La Registrazione Delle Ore](#prevent-tasks-and-issues-from-being-deleted-when-hours-are-logged)
* [Rimozione dell&#39;impostazione di &quot;Accesso anticipato&quot; dall&#39;area di installazione](#removal-of-the-early-access-setting-from-the-setup-area)
* [Modifica indirizzo e-mail predefinito di Workfront](#workfront-default-email-address-change)

**Per Tutti Gli Utenti:**

* [Miglioramenti alla pianificazione delle risorse](#resource-scheduling-improvements)
* [Schermo widescreen](#widescreen-display)
* [Ridimensiona e riordina colonne in report ed elenchi](#resize-and-reorder-columns-in-reports-and-lists)
* [Cancella opzione dati personalizzati durante la copia di attività e problemi](#clear-custom-data-option-when-copying-tasks-and-issues)
* [Crea un progetto direttamente da un modello](#create-a-project-directly-from-a-template)
* [Notifica in-app per gli oggetti sottoscritti](#in-app-notification-for-subscribed-objects)
* [@Tagging Attualmente non disponibile nell&#39;ambiente di anteprima](#tagging-currently-not-available-in-the-preview-environment)
* [Includi informazioni sull&#39;allocazione utente nel report Utilizzo di un progetto](#include-user-allocation-information-in-the-utilization-report-on-a-project)

## Miglioramenti alla programmazione delle risorse {#resource-scheduling-improvements}

>[!NOTE]
>
>Gli strumenti di pianificazione delle risorse sono stati dichiarati obsoleti e rimossi da Workfront con la versione 23.1. Per informazioni sulla pianificazione delle risorse tramite il Bilanciatore dei carichi di lavoro, vedere [Panoramica del Bilanciatore dei carichi di lavoro](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Sono disponibili i seguenti miglioramenti alla pianificazione delle risorse quando si pianificano risorse per un team, per un progetto o per più progetti come responsabile delle risorse:

* [Visualizza area di pianificazione in modalità a schermo intero](#view-scheduling-area-in-full-screen-mode)
* [Altre opzioni intervallo date per visualizzare l&#39;area di programmazione risorse](#more-date-range-options-for-viewing-the-resource-scheduling-area)
* [Visualizza date previste nella sequenza temporale di programmazione](#view-projected-dates-on-the-scheduling-timeline)

### Visualizza area di pianificazione in modalità a schermo intero {#view-scheduling-area-in-full-screen-mode}

La timeline di programmazione può essere visualizzata in modalità a schermo intero, consentendo di visualizzare più informazioni in un&#39;unica schermata. 

Per ulteriori informazioni, vedere &quot;Introduzione alla programmazione delle risorse&quot;.

### Altre opzioni di intervallo date per visualizzare l&#39;area Programmazione risorse {#more-date-range-options-for-viewing-the-resource-scheduling-area}

Durante la visualizzazione della sequenza temporale della programmazione, è possibile visualizzare le seguenti opzioni aggiuntive per l&#39;intervallo di date:

* Visualizzazione per giorno singolo
* Visualizzazione a 4 settimane
* Visualizzazione a 6 settimane

Prima di questa modifica, era possibile visualizzare la sequenza temporale della pianificazione solo in una visualizzazione a 1, 2 o 3 settimane. Questi intervalli di date sono ancora disponibili in aggiunta ai nuovi intervalli di date.

Quando si visualizza la sequenza temporale della programmazione in una visualizzazione a giorno singolo, non è possibile visualizzare le allocazioni utente (comprese le ore totali giornaliere).

Per ulteriori informazioni, vedere &quot;Introduzione alla programmazione delle risorse&quot;.

### Visualizza date previste nella sequenza temporale di programmazione {#view-projected-dates-on-the-scheduling-timeline}

Ora puoi configurare la timeline di programmazione in modo da visualizzare le Date previste invece delle Date pianificate per le attività e i problemi. 

Prima di questa modifica, le attività e i problemi nella timeline di programmazione mostravano solo le Date Pianificate.

Quando si visualizzano le Date previste nella sequenza temporale della programmazione, non è possibile visualizzare le allocazioni utente (comprese le ore totali giornaliere).

Per ulteriori informazioni, vedere &quot;Introduzione alla programmazione delle risorse&quot;.

## Schermo widescreen {#widescreen-display}

Quando si visualizza uno dei seguenti oggetti in Workfront, l&#39;intera finestra del browser viene riempita automaticamente:

* Progetti
* Attività
* Problemi
* Report
* Dashboard
* Calendari

Prima di questa modifica, erano presenti due barre laterali bianche su entrambi i lati dell&#39;area visualizzata. Ora la visualizzazione widescreen si adatta dinamicamente alla larghezza dello schermo e della finestra del browser.

## Ridimensionare e riordinare le colonne nei report e negli elenchi {#resize-and-reorder-columns-in-reports-and-lists}

È ora possibile riordinare e ridimensionare le colonne di un report o di un elenco, senza dover modificare il report. Questa funzionalità è stata rimossa con l’esclusione dell’ambiente di accesso anticipato all’inizio di quest’anno. È in fase di reintroduzione.)

Questa funzionalità non è disponibile per gli elenchi o i report del dashboard, poiché tali elenchi sono stati riprogettati in una nuova struttura della griglia dati. Con questa versione, questa funzionalità sarà attivata per tutti gli altri elenchi.

Per ulteriori informazioni sul ridimensionamento e sul riordinamento delle colonne, vedere [Modificare la larghezza e l&#39;ordine delle colonne](../../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

## Cancella opzione Dati personalizzati durante la copia di attività e problemi {#clear-custom-data-option-when-copying-tasks-and-issues}

Quando copi un’attività o un problema, ora puoi selezionare un’opzione per cancellare tutti i dati personalizzati. Quando si sceglie di cancellare i dati personalizzati di un’attività o di un problema, il modulo viene copiato nel nuovo elemento, ma i dati personalizzati nel modulo non lo sono. La cancellazione dei dati personalizzati influisce anche sui moduli personalizzati allegati ai documenti allegati agli elementi o ai moduli personalizzati allegati alle spese dell’attività.

Prima di questa modifica, i dati personalizzati inclusi in un modulo personalizzato venivano copiati anche nel nuovo elemento quando copiavi l’attività o il problema. 

Per ulteriori informazioni sulla copia delle attività, vedere [Copia e duplica attività](../../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

Per ulteriori informazioni sulla copia dei problemi, vedi [Copia problemi](../../../../manage-work/issues/manage-issues/copy-issues.md).

## Creare un progetto direttamente da un modello {#create-a-project-directly-from-a-template}

Ora puoi creare un progetto da un modello, a livello di modello.

Prima di questa modifica, era possibile creare un progetto da un modello solo nella scheda Progetti dell&#39;area Progetti di Workfront, utilizzando l&#39;opzione **Nuovo progetto da modello**.

Per ulteriori informazioni sulla creazione di un progetto da un modello, vedere [Creare un progetto utilizzando un modello](../../../../manage-work/projects/create-projects/create-project-from-template.md).

## Impedisci l&#39;eliminazione di attività e problemi durante la registrazione delle ore {#prevent-tasks-and-issues-from-being-deleted-when-hours-are-logged}

Ora puoi configurare Workfront in modo da consentire o impedire l’eliminazione di attività e problemi con ore registrate.

Prima di questa modifica, quando hai eliminato un’attività o un problema per il quale erano state registrate ore, le ore sono state eliminate insieme all’attività o al problema oppure spostate nel progetto, a seconda delle Preferenze di Scheda orario e ore.

Per ulteriori informazioni sull&#39;eliminazione delle attività, vedere [Elimina attività](../../../../manage-work/tasks/manage-tasks/delete-tasks.md).

Per ulteriori informazioni sull&#39;eliminazione dei problemi, vedere [Elimina problemi](../../../../manage-work/issues/manage-issues/delete-issues.md).

Per ulteriori informazioni sull&#39;abilitazione delle impostazioni di sistema per l&#39;eliminazione di attività e problemi, vedere [Configurare le preferenze relative a attività e problemi a livello di sistema](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## Rimozione dell&#39;impostazione &quot;Accesso anticipato&quot; dall&#39;area di configurazione {#removal-of-the-early-access-setting-from-the-setup-area}

È in corso la rimozione dell’impostazione che consentiva agli amministratori di Workfront di iscrivere gli utenti a partecipare all’ambiente di accesso anticipato. Questa funzionalità è obsoleta dalla fine del 2016. Non sono state rilasciate nuove funzionalità in Early Access nel 2017 e tutte le funzioni rimanenti in tale ambiente sono state spostate in Produzione.

Prima di questa modifica, gli amministratori di Workfront potevano comunque aggiungere utenti all’ambiente di accesso anticipato, anche se non vi erano nuove funzioni di accesso.

## Modifica indirizzo e-mail predefinito di Workfront {#workfront-default-email-address-change}

L&#39;indirizzo di posta elettronica predefinito per la posta in uscita di Workfront è stato modificato da [noreply@attask.com](mailto:noreply@attask.com) a [noreply@my.workfront.com](mailto:noreply@workfront.com).

Se attualmente filtri le e-mail inviate da Workfront, devi modificare il filtro per riflettere il nuovo indirizzo predefinito. 

La modifica dell’indirizzo predefinito non ha alcun effetto sugli indirizzi e-mail di Workfront configurati. 

Per ulteriori informazioni, consulta .

## Notifica in-app per oggetti sottoscritti {#in-app-notification-for-subscribed-objects}

Quando un utente fa un commento su progetti, attività e problemi a cui sei abbonato, ora ricevi una notifica in-app. Per ulteriori informazioni sulle notifiche in-app di abbonamento, consulta [Visualizzare e gestire le notifiche in-app](../../../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

A seconda delle funzioni abilitate dall’amministratore di Workfront, puoi anche ricevere notifiche e-mail per gli elementi abbonati. Puoi annullare facilmente l&#39;iscrizione a un elemento tramite un collegamento in un&#39;e-mail di iscrizione, come descritto in [Notifiche di Adobe Workfront](../../../../workfront-basics/using-notifications/wf-notifications.md).

Prima di questa modifica, ricevevi sempre una notifica e-mail per gli elementi in abbonamento e non c’era alcuna opzione per ricevere una notifica in-app.

Anche se puoi disabilitare l’e-mail di abbonamento, non puoi disabilitare le notifiche in-app per gli elementi abbonati. Per ulteriori informazioni, vedere [Configurare le notifiche degli eventi per tutti gli utenti del sistema](../../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

Per ulteriori informazioni sulla sottoscrizione agli elementi, vedere [Sottoscrizione agli elementi in Adobe Workfront](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md).

## @Tagging attualmente non disponibile nell’ambiente di anteprima {#tagging-currently-not-available-in-the-preview-environment}

Quando si utilizza la funzionalità Formato RTF per il flusso di aggiornamento, non è possibile utilizzare temporaneamente il simbolo @ per assegnare tag ad altri utenti nel flusso di aggiornamento per i seguenti oggetti nell’ambiente di anteprima:

* Progetto
* Attività
* Problema
* Scheda orario

Puoi comunque assegnare tag ad altri facendo clic sull&#39;icona **Includi altri su questo aggiornamento**.

Per ulteriori informazioni, consulta [Assegnare tag ad altri in occasione di aggiornamenti](../../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

## Includi informazioni sull&#39;allocazione utente nel report Utilizzo di un progetto {#include-user-allocation-information-in-the-utilization-report-on-a-project}

>[!NOTE]
>
>Gli strumenti di pianificazione delle risorse sono stati dichiarati obsoleti e rimossi da Workfront con la versione 23.1. Per informazioni sulla pianificazione delle risorse tramite il Bilanciatore dei carichi di lavoro, vedere [Panoramica del Bilanciatore dei carichi di lavoro](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Il rapporto Utilizzo di un progetto ora considera se le ore pianificate sono state riallocate per l&#39;intera durata di un&#39;attività. Quando l&#39;allocazione utente per le ore è stata modificata (come descritto in &quot;Gestire le allocazioni utente nelle aree Programmazione&quot;), i dati nel report Utilizzo possono essere influenzati se le date selezionate nel report Utilizzo contengono solo una parte di un task.

Per ulteriori informazioni, vedere [Panoramica del report Utilizzo risorse](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).
