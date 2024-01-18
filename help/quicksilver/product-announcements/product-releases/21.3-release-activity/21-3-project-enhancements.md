---
title: 21.3 Miglioramenti al progetto
description: 21.3 Miglioramenti al progetto
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 1df4ccdb-5b74-414c-a622-b0a5ed30a8c4
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1129'
ht-degree: 0%

---

# 21.3 Miglioramenti al progetto

Questa pagina descrive tutti i miglioramenti apportati all’ambiente di anteprima con la versione 21.3 di. Questi miglioramenti sono stati resi disponibili nell’ambiente di produzione la settimana del 21 luglio 2021.

Per un elenco di tutte le modifiche disponibili con la versione 21.3, consulta [Panoramica sulla versione 21.3](../../../product-announcements/product-releases/21.3-release-activity/21-3-release-overview.md).

## Associare un modello a un gruppo

>[!NOTE]
>
>Questa funzione è disponibile solo nella nuova esperienza Adobe Workfront.

Per semplificare il processo di creazione del progetto e per identificare più facilmente i gruppi proprietari dei modelli di progetto e generare rapporti su di essi, è stata aggiunta la possibilità di assegnare un gruppo a un modello di progetto.

Quando si assegna un gruppo a un modello di progetto, tutti i progetti creati dal modello vengono associati automaticamente al gruppo del modello. Per ulteriori informazioni, consulta [Modificare i modelli di progetto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

È inoltre possibile allegare un processo di approvazione di gruppo a un modello e ai relativi task di modello se il modello è associato al gruppo. Per ulteriori informazioni, consulta [Associa un processo di approvazione nuovo o esistente al lavoro](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Modifica più semplice dei campi nella sezione Dettagli

>[!NOTE]
>
>Questa funzione è disponibile solo nella nuova esperienza Adobe Workfront.

I seguenti miglioramenti consentono di modificare più facilmente le informazioni nella sezione Dettagli di qualsiasi oggetto:

* Una struttura grigia intorno a un campo quando si passa il puntatore su di esso indica che è modificabile.
* Puoi modificare i campi facendo clic una volta.

Prima di questo miglioramento non era chiaro quali campi fossero modificabili ed era necessario fare doppio clic per modificare un campo.

## Considerare i predecessori tra progetti durante il calcolo delle date di handoff

Con un nuovo miglioramento nel modo in cui Adobe Workfront calcola le date di trasferimento per le attività, ora vengono prese in considerazione le dipendenze tra progetti.

In precedenza, le date di handoff venivano calcolate solo in base ai predecessori dell&#39;attività dello stesso progetto.

Ora, per essere certi di disporre sempre di una data di trasferimento accurata per un&#39;attività con un predecessore per più progetti, è necessario ricalcolare la sequenza temporale del progetto dell&#39;attività successore. Dopo aver ricalcolato la sequenza temporale, le date di trasferimento dell&#39;attività vengono calcolate tenendo conto delle relazioni tra progetti delle attività.

Per ulteriori informazioni sulle date di handoff, consulta [Panoramica sulla data di handoff dell’attività](../../../manage-work/tasks/task-information/handoff-task-date.md).

## Aggiungi storie e problemi esistenti dalla bacheca Scrum

>[!NOTE]
>
>Questa funzione è disponibile solo nella nuova esperienza Adobe Workfront.

Ora puoi aggiungere una storia o un problema esistente direttamente dalla bacheca Scrum. In questo modo è più facile aggiungere brani esistenti all’iterazione corrente senza dover passare alla pagina del backlog.

Per ulteriori informazioni, consulta [Aggiungi storie e problemi dalla bacheca Scrum](../../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md).

## Aggiungi nuove storie e problemi dalla bacheca Scrum

>[!NOTE]
>
>Questa funzione è disponibile solo nella nuova esperienza Adobe Workfront.

Ora puoi creare una nuova storia o un nuovo problema direttamente dalla bacheca Scrum. In questo modo è più facile aggiungere rapidamente una nuova storia all&#39;iterazione corrente.

Per ulteriori informazioni, consulta [Aggiungi storie e problemi dalla bacheca Scrum](../../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md).

## Elimina storia o problema dal Kanban Board

>[!NOTE]
>
>Questa funzione è disponibile solo nella nuova esperienza Adobe Workfront.

Ora puoi eliminare una storia o un problema direttamente dalla bacheca Kanban facendo clic sull’icona Altro su una storia o su una scheda problema e selezionando Elimina. Quando elimini una storia o un problema, questa viene spostata nel Cestino per 30 giorni e può essere ripristinata solo dall&#39;amministratore di sistema.

Per ulteriori informazioni, consulta [Elimina storie o problemi dalla bacheca Kanban](../../../agile/use-kanban-in-an-agile-team/delete-story-from-kanban-board.md).

## Aggiornamenti nell’intestazione e nella bacheca delle storie della scheda Agile

>[!NOTE]
>
>Questa funzione è disponibile solo nella nuova esperienza Adobe Workfront.

Sulle schede Kanban e Scrum sono ora disponibili i seguenti miglioramenti:

* Le schede delle storie e le colonne della bacheca hanno una larghezza fissa, in modo che le dimensioni della scheda non cambiino se regolate le dimensioni della finestra del browser.
* La colonna Storie è stata rinominata in Storia principale.
* Ogni scheda ha un&#39;etichetta nella parte superiore per identificarla come storia principale, sottoattività (associata a una storia principale), storia (non associata a una storia principale) o problema.
* Lo sfondo separa visivamente le colonne.

Per ulteriori informazioni, consulta [Panoramica delle iterazioni](../../../agile/use-scrum-in-an-agile-team/iterations/iterations-overview.md).

## Raggruppa le preferenze per progetto, attività e problema

Come abbiamo comunicato in precedenza, abbiamo implementato personalizzazioni a livello di gruppo per le preferenze di progetto, attività e problema nelle fasi che precedono il 24 giugno 2021. Ora il rollout è completo e sono disponibili in Produzione per tutti i clienti.

Per ulteriori informazioni, consulta i seguenti articoli:

* [Configurare le preferenze di progetto per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)
* [Configurare le preferenze per attività e problemi per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)

## Consenti agli utenti esterni di approvare un documento

>[!NOTE]
>
>Questa funzione è disponibile solo nella nuova esperienza Adobe Workfront.

Ora puoi utilizzare indirizzi e-mail esterni per assegnare approvatori a un documento nella nuova esperienza Workfront.

In precedenza, era possibile aggiungere utenti esterni per indirizzo e-mail solo in Workfront Classic.

Per ulteriori informazioni, consulta [Richiedi approvazioni documenti](../../../review-and-approve-work/manage-approvals/request-document-approvals.md).

## Esportare informazioni dalla sezione Dettagli di un portfolio o programma

>[!NOTE]
>
>Questa funzione è stata rilasciata nell’ambiente di anteprima il 20 maggio 2021. Verrà rilasciato nell’ambiente di produzione il 3 giugno 2021.

>[!NOTE]
>
>Questa funzione è disponibile solo nella nuova esperienza Adobe Workfront.

È ora possibile esportare le informazioni in un file .pdf dalla sezione Dettagli dei portfolio e dei programmi. Prima di questo miglioramento, era possibile esportare le informazioni dalla sezione Dettagli solo da progetti, attività e problemi.

Per informazioni sull’esportazione di moduli personalizzati da un oggetto, consulta [Esportare moduli personalizzati e dettagli oggetto](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).

## Timestamp Data di completamento pianificata aggiunto nell’intestazione dell’oggetto

>[!NOTE]
>
>Questa funzione è disponibile solo nella nuova esperienza Adobe Workfront.

Per semplificare l’accesso, la comodità e la precisione, è stata aggiunta l’opzione per selezionare una marca temporale nell’intestazione Data di completamento pianificata per progetti, attività o problemi.

Prima di questo miglioramento, quando hai aggiornato la Data di completamento pianificata di un oggetto, Workfront ha selezionato la mezzanotte come ora predefinita. Ora puoi personalizzare l’ora e la data di completamento.

Per informazioni sulle intestazioni degli oggetti nella nuova esperienza Workfront, consulta [Nuove intestazioni oggetto](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).

## Aggiungere un modulo personalizzato a un oggetto senza modificarlo

>[!NOTE]
>
>Questa funzione è disponibile solo nella nuova esperienza Adobe Workfront.

È stato semplificato l&#39;aggiunta a un oggetto di un modulo personalizzato che verrà compilato da un altro utente o che verrà compilato successivamente. Il modulo non entra più in modalità di modifica automatica quando viene aggiunto. È sufficiente salvare il modulo vuoto nell’oggetto.

In precedenza, quando si aggiungeva un modulo personalizzato a un oggetto, la pagina passava alla modalità di modifica ed era necessario completare tutti i campi obbligatori nel modulo prima di poterlo salvare nell’oggetto. Ciò era scomodo quando il modulo doveva essere compilato da un altro utente o quando non si sapeva ancora cosa inserire in un campo obbligatorio del modulo.

Per informazioni sull&#39;aggiunta di un modulo personalizzato a un oggetto, vedere [Aggiungere un modulo personalizzato a un oggetto](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

