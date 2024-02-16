---
content-type: release-notes
navigation-topic: product-releases-archive
title: Attività sulla versione 2017.2 Beta 1
description: Questa pagina descrive tutte le modifiche disponibili nell’ambiente di anteprima con la versione 2017.2 Beta 1. La funzionalità in questa pagina è stata resa disponibile nell’ambiente di anteprima il 10 maggio 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 99812ed3-a300-478e-973f-b957382d934b
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1380'
ht-degree: 0%

---

# Attività sulla versione 2017.2 Beta 1

Questa pagina descrive tutte le modifiche disponibili nell’ambiente di anteprima con la versione 2017.2 Beta 1. La funzionalità in questa pagina è stata resa disponibile nell’ambiente di anteprima il 10 maggio 2017.

>[!IMPORTANT]
>
>La funzionalità descritta in questa pagina è soggetta a modifiche prima della disponibilità nell’ambiente di produzione.

La versione 2017.2 Beta 1 contiene miglioramenti sia per gli amministratori di Workfront che per altri utenti:

**Per gli amministratori:**

* [Ripristina documenti](#restore-documents)
* [Nuovo banner di anteprima con informazioni sulla versione](#new-preview-banner-with-release-information) 
* [Disponibilità di API 7](#api-7-availability)

**Per tutti gli utenti:**

* [Iscriviti ad attività e problemi](#subscribe-to-tasks-and-issues)
* [Miglioramenti alla programmazione delle risorse](#resource-scheduling-improvements)
* [Confronta bozze](#compare-proofs)
* [Nuovo campo per Pool di Risorse per Utenti e Progetti](#new-field-for-resource-pools-for-users-and-projects)
* [Aspetto aggiornato nell’elenco delle dashboard](#updated-look-and-feel-in-the-dashboard-list)
* [Rimozione della funzionalità delle annotazioni in Workfront](#removing-the-endorsements-functionality-in-workfront)
* [Riordinare le colonne in qualsiasi elenco con il trascinamento della selezione (funzionalità rimossa)](#reorder-columns-in-any-list-with-drag-and-drop-functionality-is-being-removed)

## Ripristina documenti {#restore-documents}

Gli amministratori di Workfront ora possono ripristinare singoli documenti eliminati negli ultimi 30 giorni. 

Prima di questa modifica, gli amministratori di Workfront potevano ripristinare solo progetti, attività e problemi (inclusi i documenti eliminati insieme al progetto, all’attività o al problema eliminato).

Per ulteriori informazioni, consulta [Ripristina elementi eliminati](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

## Nuovo banner di anteprima con informazioni sulla versione {#new-preview-banner-with-release-information}

Il banner blu nella parte superiore dell’ambiente Sandbox di anteprima ora mostra il nome della versione e il numero di versione dell’ambiente di anteprima. Facendo clic sul nome della versione si aprirà un articolo del sito di aiuto in cui è possibile trovare ulteriori informazioni sulla versione di anteprima corrente. Per ulteriori informazioni sull’ambiente Sandbox di anteprima, consulta [Ambiente Sandbox di anteprima di Adobe Workfront](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md) 

## Disponibilità di API 7 {#api-7-availability}

L’API 7 è ora disponibile e include oggetti nuovi e aggiornati.

Per ulteriori informazioni, consulta [Novità della versione 7 dell’API](../../../../wf-api/api/new-api-version-7.md).

## Iscriviti ad attività e problemi {#subscribe-to-tasks-and-issues}

Workfront invia notifiche sugli elementi a cui sei assegnato o di cui sei proprietario.

A partire dalla versione corrente, se desideri seguire elementi non assegnati a te ma che potrebbero influire sul tuo lavoro, puoi abbonarti.

È possibile iscriversi a problemi e attività per i quali si dispone delle autorizzazioni di visualizzazione minima. Quando un nuovo commento viene aggiunto al problema o all’attività a cui ti abboni, riceverai una notifica via e-mail.

Per ulteriori informazioni sull’abbonamento a problemi e attività, consulta [Iscriviti agli elementi in Adobe Workfront](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md)

## Miglioramenti alla programmazione delle risorse {#resource-scheduling-improvements}

>[!NOTE]
>
>Gli strumenti di pianificazione delle risorse sono stati dichiarati obsoleti e rimossi da Workfront con la versione 23.1. Per informazioni sulla programmazione delle risorse tramite il Bilanciatore dei carichi di lavoro, consulta [Panoramica del Bilanciatore dei carichi di lavoro](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Durante la pianificazione delle risorse sono disponibili i seguenti miglioramenti:

* [Visualizzare più elementi nella sequenza temporale di programmazione delle risorse in una singola visualizzazione](#view-more-items-on-the-resource-scheduling-timeline-in-a-single-view)
* [Configura il nome del progetto da visualizzare nelle attività e nei problemi nella timeline di programmazione](#configure-the-project-name-to-display-on-tasks-and-issues-on-the-scheduling-timeline)
* [Configura se le attività padre vengono visualizzate nella sequenza temporale di pianificazione](#configure-whether-parent-tasks-are-displayed-on-the-scheduling-timeline)
* [Espandere o comprimere più facilmente tutte le attività e i problemi nella sequenza temporale di pianificazione](#more-easily-expand-or-collapse-all-tasks-and-issues-on-the-scheduling-timeline)
* [Le informazioni su ruolo e utente rimangono nella parte superiore della timeline di programmazione durante lo scorrimento](#role-and-user-information-remains-at-the-top-of-the-scheduling-timeline-when-scrolling)

### Visualizzare più elementi nella sequenza temporale di programmazione delle risorse in una singola visualizzazione {#view-more-items-on-the-resource-scheduling-timeline-in-a-single-view}

Quando si programmano le risorse per un team o per progetti di cui si è il Responsabile risorse, le attività e i problemi occupano meno spazio verticale nella programmazione. Questo consente di visualizzare più attività e problemi in un’unica schermata.

Se decidi di visualizzare i nomi dei progetti per ogni attività e problema nella sequenza temporale di pianificazione, lo spazio verticale di ogni attività e problema viene espanso, con conseguente riduzione delle attività e dei problemi visualizzati in un’unica vista.

Per ulteriori informazioni sulla programmazione delle risorse, vedere &quot;Introduzione alla programmazione delle risorse&quot;.

### Configura il nome del progetto da visualizzare nelle attività e nei problemi nella timeline di programmazione {#configure-the-project-name-to-display-on-tasks-and-issues-on-the-scheduling-timeline}

Quando pianifichi le risorse per un team o per qualsiasi progetto di cui sei il Responsabile risorse, ora puoi configurare il nome del progetto in modo che venga visualizzato su ogni attività e problema nella tempistica di programmazione. In questo modo, gli utenti che visualizzano la timeline di programmazione possono vedere rapidamente il nome del progetto in cui si trova l’attività o il problema.

Per ulteriori informazioni, vedere &quot;Introduzione alla programmazione delle risorse&quot;.

### Configura se le attività padre vengono visualizzate nella sequenza temporale di pianificazione {#configure-whether-parent-tasks-are-displayed-on-the-scheduling-timeline}

Quando si programmano le risorse per i progetti di cui si è Responsabile risorse, è ora possibile specificare se le attività padre devono essere visualizzate sull&#39;indicatore cronologico della programmazione quando l&#39;opzione Modalità di completamento riepilogo sul progetto è impostata su Manuale.

Prima di questa modifica, le attività padre venivano sempre visualizzate nella sequenza temporale di programmazione quando la Modalità di completamento riepilogo del progetto era impostata su Manuale. 

Quando la Modalità di completamento riepilogo del progetto è impostata su Automatico, le attività padre non possono essere visualizzate nella sequenza temporale di programmazione. Questa esperienza non è cambiata.

Per ulteriori informazioni, vedere &quot;Introduzione alla programmazione delle risorse&quot;.

### Espandere o comprimere più facilmente tutte le attività e i problemi nella sequenza temporale di pianificazione {#more-easily-expand-or-collapse-all-tasks-and-issues-on-the-scheduling-timeline}

È disponibile un nuovo collegamento che consente di comprimere più facilmente tutte le attività e i problemi nella timeline di pianificazione.

Per ulteriori informazioni, vedere &quot;Introduzione alla programmazione delle risorse&quot;.

### Le informazioni su ruolo e utente rimangono nella parte superiore della timeline di programmazione durante lo scorrimento {#role-and-user-information-remains-at-the-top-of-the-scheduling-timeline-when-scrolling}

Ora, quando si scorre verso il basso nella timeline di pianificazione per visualizzare informazioni aggiuntive, il nome del ruolo e il nome utente rimangono nella parte superiore dell’area Utenti e ruoli nella timeline di pianificazione, semplificando la visualizzazione dell’utente e del ruolo a cui sono associate le attività e i problemi.

Prima di questa modifica, il nome del ruolo e il nome utente scorrono fuori dalla visualizzazione corrente.

Per ulteriori informazioni sulla programmazione delle risorse, vedere &quot;Introduzione alla programmazione delle risorse&quot;.

## Confronta bozze {#compare-proofs}

È ora possibile confrontare due bozze di documento all’interno di un singolo elenco di documenti, ad esempio all’interno della scheda Documenti in un progetto, un’attività, un problema, un portfolio o all’interno dell’area Documenti principale nella barra di navigazione globale. 

Le due bozze vengono visualizzate all&#39;interno dello strumento Revisione e approvazione ed è possibile eseguire la verifica di ogni documento confrontandoli in una visualizzazione affiancata.

Per ulteriori informazioni, consulta [Confronta bozze](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/compare-proofs.md).

## Nuovo campo per Pool di Risorse per Utenti e Progetti {#new-field-for-resource-pools-for-users-and-projects}

La versione R1.5 ha introdotto nell’ambiente di anteprima nuove funzionalità relative alla pianificazione delle risorse. Questa funzionalità consente di creare nuovi Pool di Risorse, ovvero insiemi di utenti.

Ora puoi associare questi Pool di Risorse ai progetti, oltre che agli utenti. Ora nel progetto e nell’oggetto utente viene visualizzato il nuovo campo &quot;Pool di Risorse&quot;.

Per ulteriori informazioni sui nuovi Pool di Risorse e su come associarli a progetti e utenti, consulta [Panoramica sui pool di risorse](../../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md)

## Aspetto aggiornato nell’elenco delle dashboard {#updated-look-and-feel-in-the-dashboard-list}

Ora, quando si visualizza un elenco di dashboard, l’aspetto è più moderno e scalabile.

In precedenza questa funzionalità era disponibile solo per gli utenti iscritti a Early Access. Ora questo è disponibile per tutti gli utenti nell’ambiente di anteprima. Sarà reso disponibile a tutti gli utenti nell’ambiente di produzione con la versione 2017.2. 

Per ulteriori informazioni sulle dashboard, consulta [Creare un dashboard](../../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## Rimozione della funzionalità delle annotazioni in Workfront {#removing-the-endorsements-functionality-in-workfront}

Durante la valutazione della funzionalità contenuta nel flusso di aggiornamento, è stato identificato che le approvazioni sono una funzione a bassa adozione e a basso utilizzo. Nella versione 2017.2, le seguenti funzionalità relative alle approvazioni verranno rimosse da Workfront a partire dalla versione 2017.2 (questa funzionalità non è più disponibile in Anteprima):

* La scheda Approvazioni nell’area del profilo utente;
* L&#39;oggetto Endorsements verrà rimosso da Esplora API; se si stanno estraendo report API per gli oggetti &quot;Endorsement&quot; o &quot;Condivisione di valutazione&quot;, le chiamate non saranno valide dopo la rimozione di questo oggetto.

Le seguenti funzionalità continueranno a essere presenti nell’applicazione web:

* La valutazione positiva di un utente da parte di un altro utente effettuata prima della rimozione di questa funzione rimarrà nel flusso di aggiornamento dell&#39;approvatore. 

Le approvazioni non sono state oggetto segnalabile, pertanto il reporting per questo oggetto non è stato modificato.

## Riordinare le colonne in qualsiasi elenco con il trascinamento della selezione (funzionalità rimossa) {#reorder-columns-in-any-list-with-drag-and-drop-functionality-is-being-removed}

La funzionalità per modificare l’ordine delle colonne in qualsiasi elenco trascinando una colonna da una posizione e rilasciandola in un’altra viene rimossa da Early Access nell’ambiente di produzione con la versione 2017.2 e non sarà più disponibile per alcun utente. 

Per ulteriori dettagli su questa funzionalità, consulta [Modifica la larghezza e l&#39;ordine delle colonne](../../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).
