---
content-type: release-notes
navigation-topic: product-releases-archive
title: Attività sulla versione 2018.3 di Beta 2
description: Questa pagina descrive tutte le modifiche più recenti disponibili nell’ambiente di anteprima con la versione 2018.3 di Beta 2. La funzionalità sarà disponibile nell’ambiente di anteprima il 1° agosto 2018. I miglioramenti della bozza rilasciati con Beta 2 saranno disponibili nell’ambiente di anteprima mercoledì 18 luglio. Sarà disponibile nell’ambiente di produzione a novembre 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 97945661-e97d-43c8-b564-624c4388de2f
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '908'
ht-degree: 0%

---

# Attività sulla versione 2018.3 di Beta 2

Questa pagina descrive tutte le modifiche più recenti disponibili nell’ambiente di anteprima con la versione 2018.3 di Beta 2. La funzionalità sarà disponibile nell’ambiente di anteprima il 1° agosto 2018. I miglioramenti della bozza rilasciati con Beta 2 saranno disponibili nell’ambiente di anteprima mercoledì 18 luglio. Sarà disponibile nell’ambiente di produzione a novembre 2018.

>[!NOTE]
>
> La funzionalità descritta in questa pagina è soggetta a modifiche prima della disponibilità nell’ambiente di produzione.

Per un elenco di tutte le modifiche apportate nel 2018.3, consulta  Panoramica sull&#39;attività della versione di [2018.3](../../../../product-announcements/product-releases/quarterly-release-archive/2018.3-release-activity/2018-3-release-activity-overview.md).

La versione 2018.3 di Beta 2 contiene miglioramenti sia per gli amministratori di Workfront che per altri utenti:

**Per Amministratori**

* [Aggiornare l’indirizzo e-mail nel profilo utente come amministratore di gruppo](#update-the-email-address-in-the-user-profile-as-a-group-administrator)

**Per Tutti Gli Utenti**

* [Visualizza le approvazioni delegate a me nell&#39;area Home](#view-approvals-delegated-to-me-in-the-home-area)
* [Esporta dati per un determinato periodo nella pianificazione risorse](#export-data-for-a-given-period-in-the-resource-planner)
* [I Totali Giornalieri Ora Vengono Visualizzati In Rosso Quando L&#39;Utente È Sovrassegnato](#daily-totals-now-display-in-red-when-the-user-is-overallocated)
* [Le attività e i problemi sono nascosti nella sequenza temporale di pianificazione quando ridotti a icona](#tasks-and-issues-are-hidden-on-the-scheduling-timeline-when-minimized)
* [Filtra commenti e risposte per utente nel visualizzatore di bozze](#filter-comments-and-replies-by-user-in-the-proofing-viewer)
* [Commento su un intervallo di metraggio in una bozza video](#comment-on-a-range-of-footage-in-a-video-proof)
* [Nuovo strumento polilinea per il markup dei commenti nel visualizzatore di bozze](#new-polyline-tool-for-comment-markup-in-the-proofing-viewer)
* [Rimozione Flash per condivisione report, calendario e documenti](#flash-removal-for-report-calendar-and-document-sharing)

## Aggiornare l’indirizzo e-mail nel profilo utente come amministratore di gruppo {#update-the-email-address-in-the-user-profile-as-a-group-administrator}

Ora puoi aggiornare gli indirizzi e-mail per gli utenti che appartengono a un gruppo che amministri. 

In precedenza, solo gli amministratori di Workfront potevano aggiornare gli indirizzi e-mail per altri utenti. 

Per ulteriori informazioni, vedere [Amministratori di gruppi](../../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

## Visualizza le approvazioni delegate a me nell’area Home {#view-approvals-delegated-to-me-in-the-home-area}

Ora puoi utilizzare l’area Home per visualizzare le approvazioni di progetti, attività e problemi che ti sono state delegate.

Prima di questa modifica, era possibile visualizzare le approvazioni delegate solo nell’area Il mio lavoro.

Per ulteriori informazioni, vedere [Delegare la richiesta di approvazione](../../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md).

## Esporta dati per un determinato periodo nella pianificazione risorse {#export-data-for-a-given-period-in-the-resource-planner}

Durante l’esportazione delle informazioni nella Programmazione risorse viene ora visualizzata una nuova finestra che consente di selezionare un arco temporale specifico per il file esportato.

Prima di questo miglioramento, era possibile esportare solo le informazioni visualizzate sullo schermo.

Per ulteriori informazioni sull&#39;esportazione dei dati dalla Programmazione delle risorse, vedere [Panoramica sulla navigazione di Programmazione delle risorse](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md) nell&#39;articolo [Panoramica sulla navigazione di Programmazione delle risorse](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md).

## I totali giornalieri ora vengono visualizzati in rosso quando l’utente è sovrassegnato {#daily-totals-now-display-in-red-when-the-user-is-overallocated}

>[!NOTE]
>
>Gli strumenti di pianificazione delle risorse sono stati dichiarati obsoleti e rimossi da Workfront con la versione 23.1. Per informazioni sulla pianificazione delle risorse tramite il Bilanciatore dei carichi di lavoro, vedere [Panoramica del Bilanciatore dei carichi di lavoro](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Quando un utente è sovrassegnato, i totali giornalieri per i giorni in cui l’utente è sovrassegnato ora vengono visualizzati in rosso. Questa opzione viene visualizzata solo quando l’opzione Mostra i totali per le ore pianificate giornaliere è abilitata nelle impostazioni della timeline di programmazione. Prima di questo miglioramento, esisteva un indicatore rosso per i giorni in cui l’utente era sovrassegnato, ma i totali giornalieri venivano visualizzati senza evidenziazione rossa.

Per ulteriori informazioni sulle allocazioni utente, vedere &quot;Gestire le allocazioni utente nelle aree Pianificazione&quot;.

## Le attività e i problemi sono nascosti nella timeline di programmazione quando ridotti a icona {#tasks-and-issues-are-hidden-on-the-scheduling-timeline-when-minimized}

Quando riduci a icona le attività e i problemi nella sequenza temporale della pianificazione, questi vengono ora nascosti per gli utenti e i ruoli se l’opzione Mostra totali ore pianificate giornaliere è abilitata nelle impostazioni. Le attività e i problemi nell’area Non assegnato vengono visualizzati in una visualizzazione compressa.

In precedenza, quando si riducevano le attività e i problemi, le attività e i problemi rimanevano nella timeline di pianificazione per gli utenti e i ruoli, ma venivano visualizzati in una visualizzazione compressa.

Per ulteriori informazioni su come ridurre al minimo le attività e i problemi nella sequenza temporale di pianificazione, consulta  &quot;Introduzione alla pianificazione delle risorse&quot;.

## Filtrare commenti e risposte per utente nel visualizzatore di bozze {#filter-comments-and-replies-by-user-in-the-proofing-viewer}

È ora possibile includere le risposte quando si filtrano i commenti creati dagli utenti specificati. Questa funzione ti consente di concentrarti su tutti i feedback ricevuti da un revisore importante, ad esempio un cliente o un project manager.

In precedenza, il filtro per utente era limitato ai soli commenti creati (avviati) dai revisori specificati.

## Commento su un intervallo di riprese in una bozza video {#comment-on-a-range-of-footage-in-a-video-proof}

È possibile creare un commento per una serie di riprese in una bozza video. Questa funzione è utile, ad esempio, quando è necessario indicare che un segmento di metraggio deve essere ripreso o rimosso.

In precedenza, era possibile creare un commento solo per un singolo punto su una timeline video.

## Nuovo strumento Polilinea per il markup di commenti nel visualizzatore di bozze {#new-polyline-tool-for-comment-markup-in-the-proofing-viewer}

È ora possibile utilizzare il markup polilinea per disegnare linee e forme segmentate quando si aggiunge un commento a una bozza. È possibile creare una linea segmentata aperta o una forma chiusa. Questo strumento è particolarmente utile quando si lavora con immagini complesse, ad esempio tecniche o architetturali.

In precedenza, quando si contrassegnava una bozza per aggiungere un commento, era possibile disegnare un rettangolo, una linea retta, una linea a mano libera, una forma o una freccia.

## Rimozione Flash per condivisione report, calendario e documenti {#flash-removal-for-report-calendar-and-document-sharing}

Il Flash è stato rimosso dalle seguenti finestre di dialogo di condivisione in Workfront:

* Report
* Calendari
* Documenti

Puoi comunque condividere questi oggetti come in precedenza, ma ora l’esperienza non si basa più sul Flash.
