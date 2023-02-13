---
title: 21.3 Miglioramenti al progetto
description: 21.3 Miglioramenti al progetto
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 1df4ccdb-5b74-414c-a622-b0a5ed30a8c4
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '1122'
ht-degree: 0%

---

# 21.3 Miglioramenti al progetto

Questa pagina descrive tutti i miglioramenti apportati a Project con la versione 21.3 nell’ambiente di anteprima. Questi miglioramenti sono stati resi disponibili nell&#39;ambiente di produzione la settimana del 21 luglio 2021.

Per un elenco di tutte le modifiche disponibili con la versione 21.3, vedi [Panoramica sulla versione 21.3](../../../product-announcements/product-releases/21.3-release-activity/21-3-release-overview.md).

## Associare un modello a un gruppo

>[!NOTE]
>
>Questa funzione è disponibile solo nella nuova esperienza Adobe Workfront.

Per semplificare il processo di creazione del progetto e per identificare e segnalare più facilmente i gruppi di appartenenza a cui appartengono i modelli di progetto, abbiamo aggiunto la possibilità di assegnare un gruppo a un modello di progetto.

Quando assegni un gruppo a un modello di progetto, tutti i progetti creati dal modello vengono associati automaticamente al gruppo del modello. Per ulteriori informazioni, consulta [Modificare i modelli di progetto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

Inoltre, è possibile allegare un processo di approvazione del gruppo a un modello e alle relative attività del modello se il modello è associato al gruppo. Per ulteriori informazioni, consulta [Associa un processo di approvazione nuovo o esistente al lavoro](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Modifica più semplice dei campi nella sezione Dettagli

>[!NOTE]
>
>Questa funzione è disponibile solo nella nuova esperienza Adobe Workfront.

I seguenti miglioramenti consentono di modificare più facilmente le informazioni nella sezione Dettagli di qualsiasi oggetto:

* Un contorno grigio intorno a un campo quando lo si passa sopra indica che è modificabile.
* È possibile modificare i campi facendo clic su di essi una volta.

Prima di questo miglioramento non era chiaro quali campi erano modificabili ed era necessario fare doppio clic per modificare un campo.

## Considera i predecessori tra progetti durante il calcolo delle date di abbandono

Con un nuovo miglioramento nel modo in cui Adobe Workfront calcola le date di consegna per le attività, vengono ora prese in considerazione le dipendenze tra progetti.

In precedenza, le date di abbandono venivano calcolate solo in base ai predecessori dell’attività dello stesso progetto.

Ora, per avere sempre una data precisa di consegna per un&#39;attività con un predecessore tra progetti, è necessario ricalcolare la cronologia del progetto dell&#39;attività successore. Dopo aver ricalcolato la timeline, le date di abbandono dell&#39;attività vengono calcolate tenendo conto delle dipendenze tra progetti delle attività.

Per ulteriori informazioni sulle date di consegna, vedi [Panoramica sulla data di sospensione attività](../../../manage-work/tasks/task-information/handoff-task-date.md).

## Aggiungi storie e problemi esistenti dalla scheda Scrum

>[!NOTE]
>
>Questa funzione è disponibile solo nella nuova esperienza Adobe Workfront.

È ora possibile aggiungere una storia o un problema esistente direttamente dalla bacheca Scrum. In questo modo è più semplice aggiungere storie esistenti all’iterazione corrente senza dover passare alla pagina di backlog.

Per ulteriori informazioni, consulta [Aggiungi storie e problemi dalla bacheca di Scrum](../../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md).

## Aggiungi nuove storie e nuovi problemi dalla Scrum board

>[!NOTE]
>
>Questa funzione è disponibile solo nella nuova esperienza Adobe Workfront.

È ora possibile creare una nuova storia o un nuovo problema direttamente dalla bacheca di Scrum. In questo modo è più facile aggiungere rapidamente un nuovo brano all&#39;iterazione corrente.

Per ulteriori informazioni, consulta [Aggiungi storie e problemi dalla bacheca di Scrum](../../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md).

## Elimina storia o problema dalla scheda Kanban

>[!NOTE]
>
>Questa funzione è disponibile solo nella nuova esperienza Adobe Workfront.

Per eliminare una storia o un problema direttamente dalla bacheca Kanban, fate clic sull&#39;icona Altro su una storia o una scheda del problema e selezionate Elimina. Quando si elimina un brano o un problema, questo viene spostato nel Cestino per 30 giorni e può essere recuperato solo dall&#39;amministratore di sistema.

Per ulteriori informazioni, consulta [Eliminare storie o problemi dalla bacheca Kanban](../../../agile/use-kanban-in-an-agile-team/delete-story-from-kanban-board.md).

## Aggiornamenti dell&#39;intestazione della scheda Agile e della scheda narrativa

>[!NOTE]
>
>Questa funzione è disponibile solo nella nuova esperienza Adobe Workfront.

Nelle bacheche Kanban e Scrum sono ora disponibili i seguenti miglioramenti:

* Le schede della storia e le colonne della bacheca hanno una larghezza fissa, in modo che le dimensioni della scheda non vengano modificate se si regola la dimensione della finestra del browser.
* La colonna Storie è stata rinominata Storia padre.
* Ogni scheda ha un&#39;etichetta nella parte superiore per identificarla come storia padre, sottoattività (associata a una storia padre), storia (non associata a una storia padre) o problema.
* L’ombreggiatura dello sfondo separa visivamente le colonne.

Per ulteriori informazioni, consulta [Panoramica delle iterazioni](../../../agile/use-scrum-in-an-agile-team/iterations/iterations-overview.md).

## Raggruppare le preferenze relative a progetti, attività ed problemi

Come comunicato in precedenza, sono state implementate personalizzazioni a livello di gruppo per progetti, attività e preferenze di rilascio in più fasi fino al 24 giugno 2021. Ora il rollout è completo e sono disponibili in Produzione per tutti i clienti.

Per ulteriori informazioni, consulta i seguenti articoli:

* [Configurare le preferenze di progetto per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)
* [Configurare le preferenze per attività e problemi per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)

## Consenti agli utenti esterni di approvare un documento

>[!NOTE]
>
>Questa funzione è disponibile solo nella nuova esperienza Adobe Workfront.

È ora possibile utilizzare indirizzi e-mail esterni per assegnare gli approvatori a un documento nella nuova esperienza Workfront.

In precedenza, era possibile aggiungere utenti esterni solo per indirizzo e-mail in Workfront Classic.

Per ulteriori informazioni, consulta [Richiedere l&#39;approvazione del documento](../../../review-and-approve-work/manage-approvals/request-document-approvals.md).

## Esporta informazioni dalla sezione Dettagli di un portfolio o di un programma

>[!NOTE]
>
>Questa funzione è stata rilasciata nell’ambiente Preview il 20 maggio 2021. Il rilascio verrà effettuato il 3 giugno 2021 nell’ambiente di produzione.

>[!NOTE]
>
>Questa funzione è disponibile solo nella nuova esperienza Adobe Workfront.

È ora possibile esportare in un file .pdf informazioni dalla sezione Dettagli di portfolio e programmi. Prima di questo miglioramento, era possibile esportare informazioni dalla sezione Dettagli solo da progetti, attività e problemi.

Per informazioni sull’esportazione di moduli personalizzati da un oggetto, vedere [Esportare moduli personalizzati e dettagli dell’oggetto](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).

## Aggiunta della marca temporale della data di completamento pianificata nell’intestazione dell’oggetto

>[!NOTE]
>
>Questa funzione è disponibile solo nella nuova esperienza Adobe Workfront.

Per semplificare l’accesso, la comodità e l’accuratezza, è stata aggiunta l’opzione per selezionare una marca temporale nella data di completamento pianificata dell’intestazione dei progetti, delle attività o dei problemi.

Prima di questo miglioramento, quando si aggiornava la Data di completamento pianificata di un oggetto, Workfront selezionava la mezzanotte come ora predefinita. Ora è possibile personalizzare l’ora e la data di completamento.

Per informazioni sulle intestazioni degli oggetti nella nuova esperienza Workfront, vedi [Nuove intestazioni oggetto](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).

## Aggiungere un modulo personalizzato a un oggetto senza modificarlo

>[!NOTE]
>
>Questa funzione è disponibile solo nella nuova esperienza Adobe Workfront.

Abbiamo semplificato l’aggiunta a un oggetto di un modulo personalizzato che verrà compilato da un altro utente o che verrà compilato successivamente. Il modulo non passa più automaticamente alla modalità di modifica quando viene aggiunto. È sufficiente salvare il modulo vuoto nell’oggetto.

Precedentemente, quando si aggiungeva un modulo personalizzato a un oggetto, la pagina passava alla modalità di modifica ed era necessario completare tutti i campi obbligatori del modulo prima di salvarlo nell’oggetto. Ciò era scomodo quando il modulo era destinato a essere compilato da un altro utente o quando non si sapeva ancora cosa inserire un campo obbligatorio nel modulo.

Per informazioni sull’aggiunta di un modulo personalizzato a un oggetto, consultare [Aggiungere un modulo personalizzato a un oggetto](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

