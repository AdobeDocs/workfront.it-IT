---
content-type: release-notes
keywords: note,trimestrale,aggiornamento
navigation-topic: product-releases
title: Miglioramenti a Project Management 21.1
description: Questa pagina descrive tutti i miglioramenti apportati alla gestione dei progetti con la versione 21.1 nell’ambiente di anteprima. Questi miglioramenti saranno resi disponibili nell'ambiente di produzione la settimana del 15 febbraio 2021.
author: Luke
feature: Product Announcements
exl-id: 95e75a28-5ac2-4d1d-acc3-dbc0b295b28f
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '972'
ht-degree: 1%

---

# Miglioramenti a Project Management 21.1

Questa pagina descrive tutti i miglioramenti apportati alla gestione dei progetti con la versione 21.1 nell’ambiente di anteprima. Questi miglioramenti saranno resi disponibili nell&#39;ambiente di produzione la settimana del 15 febbraio 2021.

Per un elenco di tutte le modifiche disponibili con la versione 21.1, vedi [Panoramica sulla versione 21.1](../../../product-announcements/product-releases/21.1-release-activity/21-1-release-overview.md).

## Esportazione disponibile nella sezione Metriche di un progetto

Per condividere più facilmente lo stato e l’avanzamento di un progetto, ora puoi esportare l’intero dashboard nella sezione Metriche di un progetto in un file .png.

Per ulteriori informazioni, consulta [Panoramica delle metriche del progetto](../../../manage-work/projects/manage-projects/project-metrics.md).

Questa funzione è ora inclusa nella [Nozioni di base sul planner per la nuova esperienza Workfront, parte 3: Gestire un progetto](https://one.workfront.com/s/learningpath3/planner-fundamentals-for-the-new-workfront-experience-part-3-manage-a-project-MCG6OJL724XRBLHBXEAKGAUZOJ6U) percorso di apprendimento su Workfront One.

## Percentuale di completamento dell&#39;aggiornamento del problema quando il progetto o l&#39;attività sono stati convertiti dall&#39;aggiornamento del problema

Abbiamo aggiornato il modo in cui funziona la percentuale di completamento dei problemi per i problemi che sono stati convertiti in progetti o attività. Con la nuova funzionalità, quando un problema viene convertito in un&#39;attività o in un progetto, la percentuale di completamento del problema viene aggiornata in sincronia con la percentuale di completamento dell&#39;attività o del progetto di risoluzione quando lo stato &quot;Aggiorna automaticamente il problema risolvibile quando lo stato dell&#39;impostazione Risolvi l&#39;oggetto cambia&quot; viene attivato dalla configurazione.

Per informazioni sulla conversione dei problemi, vedi [Panoramica sulla risoluzione e risoluzione di oggetti](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

## Nuovo elenco Richieste inviate

Per consentirti di gestire le richieste inviate in modo più semplice e coerente, abbiamo rimosso le sezioni Richieste inviate e Tutte le richieste nell’area Richieste e le abbiamo sostituite con un nuovo elenco Inviato. L’elenco ha un aspetto familiare che corrisponde a tutti gli altri elenchi nel sistema, consentendo di filtrare diverse categorie di richieste inviate e di cercare rapidamente una richiesta che potrebbe essere difficile trovare.

Per informazioni su come individuare le richieste inviate, vedi [Individua richieste inviate](../../../manage-work/requests/create-requests/locate-submitted-requests.md).

Questa funzione è ora inclusa nella [Nozioni di base dei collaboratori per la nuova esperienza Workfront](https://one.workfront.com/s/learningpath1/collaborator-fundamentals-for-the-new-workfront-experience-MCY5AMOQQTGFDVZB4ODS6TXCYE2A) percorso di apprendimento su Workfront One.

Questa funzione è ora inclusa nella [Richieste nella nuova esperienza Workfront](https://one.workfront.com/s/learningpath3/core-team-requests-in-the-new-workfront-experience-MCHWSSDWRFC5EKXFBXTQ6MJNKE7E) percorso di apprendimento su Workfront One.

## Campi rimossi dalla pagina Nuova richiesta

>[!NOTE]
>
>Rimosso dal rilascio.

Nell’ambito della riprogettazione della pagina Nuova richiesta, sono stati aggiornati i campi Nuovo problema impostati nella sezione Impostazione coda di un progetto.

I campi Nuovo problema seguenti vengono visualizzati solo quando si crea un problema dalla sezione Problemi del progetto. Non vengono visualizzati quando si invia un problema utilizzando una coda di richiesta nell’area Richieste:

* Gravità
* Lavoro Necessario
* Data di inizio pianificata
* URL
* Assegnato a
* Ruolo
* Team

I campi Assegnato a, Ruolo lavoro e Team sono stati sostituiti con il nuovo campo Assegnazioni nella pagina Nuova richiesta, per designare in modo efficiente un utente, un ruolo o un team in un campo comune durante l’invio di una nuova richiesta.

Per informazioni sulla definizione dei campi nuovi problemi per un progetto, consulta [Creare una coda di richiesta](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

## Nuova esperienza durante l’invio di richieste nell’area Richieste

>[!NOTE]
>
>rimosso dal rilascio; resterà in Anteprima e rilascerà in Produzione con 21.2.

Per garantire la coerenza con la nuova esperienza Workfront e creare efficienze durante l’invio delle richieste, abbiamo riprogettato la casella Nuova richiesta nell’area Richieste . Di seguito sono riportati alcuni dei miglioramenti apportati:

* Interfaccia utente coerente con il resto della nuova esperienza Workfront
* Eliminazione dell&#39;area Nuove richieste per un&#39;esperienza più semplice e intuitiva
* Un modo nuovo ed efficiente di allegare i documenti alle richieste

Possibilità di condividere un collegamento alla coda delle richieste, al gruppo di argomenti o all&#39;argomento della coda mentre si immette la richiesta.

Per informazioni sull&#39;invio delle richieste, vedi [Creare e inviare richieste Workfront](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

## Condividere un collegamento a una coda di richiesta quando si invia una richiesta

>[!NOTE]
>
>rimosso dal rilascio; resterà in Anteprima e rilascerà in Produzione con 21.2.

Ora è possibile condividere un collegamento a una coda di richiesta, a un gruppo di argomenti o a un argomento della coda Durante la creazione di una richiesta.

Prima di inviare una nuova richiesta, puoi copiare un collegamento alla coda di richiesta, al gruppo di argomenti o all’argomento della coda della richiesta e condividerlo con altri utenti o incorporarlo in un dashboard.

Per informazioni sulla condivisione di un collegamento a una coda di richiesta durante l’invio di una richiesta, consulta [Condividere un collegamento a una coda di richiesta](../../../manage-work/requests/create-requests/share-link-to-request-queue.md).

## Cercare un gruppo da assegnare a un progetto e visualizzarne i dettagli

Ora è più facile assicurarsi di identificare il gruppo corretto quando si assegna un gruppo a un progetto. Passa il puntatore del mouse sul nome di un gruppo che si trova nella casella Gruppo, quindi fai clic sull&#39;icona info visualizzata accanto al nome per visualizzare la descrizione comando Dettagli gruppo.

Questa descrizione include la gerarchia dei gruppi sopra l’eventuale gruppo e gli amministratori del gruppo.

A seconda dei dettagli configurati per il gruppo, potresti anche visualizzare il Business Leader del gruppo e la relativa descrizione.

Queste informazioni consentono di selezionare il gruppo giusto da assegnare al progetto.

Per ulteriori informazioni, consulta [Gestire le informazioni nell’area Panoramica del progetto](../../../manage-work/projects/manage-projects/understand-project-overview-area.md).

## Nuovo rapporto Delega utenti

In precedenza, le informazioni per le delegazioni di attività, problemi e approvazione dei progetti potevano essere visualizzate solo dal delegato nella propria area principale. Per consentire ad altri utenti di visualizzare queste informazioni, ora gli utenti del piano possono creare il rapporto Delega utenti, che indica:

* Utente che ha delegato queste approvazioni a un altro utente
* Quale utente ha delegato queste approvazioni
* Data di inizio e di fine di queste delegazioni

Per ulteriori informazioni, consulta [Creare un rapporto Delega utenti](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-user-delegation-report.md).
