---
content-type: release-notes
navigation-topic: 2019-3-release-activity
title: Miglioramenti al progetto 2019.3
description: Questa pagina descrive tutte le modifiche Miglioramenti apportati al progetto con la versione 2019.3. È stato reso disponibile nell’ambiente di produzione la settimana del 19 agosto 2019.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 127d695c-74e4-45f9-b5f6-55c1d05935cf
source-git-commit: dd718ff8f497065018cdfb9592ff0804d7668bf8
workflow-type: tm+mt
source-wordcount: '1340'
ht-degree: 0%

---

# Miglioramenti al progetto 2019.3

Questa pagina descrive tutte le modifiche Miglioramenti apportati al progetto con la versione 2019.3. È stato reso disponibile nell’ambiente di produzione la settimana del 19 agosto 2019.

Per un elenco di tutte le modifiche apportate in 2019.3, consulta [Panoramica sull&#39;attività di rilascio di 2019.3](../../../../product-announcements/product-releases/quarterly-release-archive/2019.3-release-activity/2019-3-release-activity-overview.md).

## Modificare il tipo di visualizzazione di un campo in un modulo personalizzato

Ora è possibile modificare il tipo di visualizzazione di un campo in un modulo personalizzato.

Se ad esempio è stato creato un campo Caselle di controllo, è possibile modificarlo in un campo a discesa o in un campo Pulsanti di scelta. Questi tre tipi di visualizzazione dei campi sono intercambiabili.

In alternativa, se è stato creato un campo di testo a riga singola, è possibile modificarlo in un campo di testo paragrafo. Questi due tipi di visualizzazione dei campi sono intercambiabili.

In precedenza, per modificare il tipo di visualizzazione di un campo personalizzato, era necessario creare un nuovo campo ed eliminare quello precedente. Questo richiedeva il trasferimento dei dati, operazione che spesso richiedeva molto tempo.

>[!NOTE]
>
>Disponibilità anteprima: 9 agosto 2019
>
>Disponibilità della produzione: 30 agosto 2019

## Creazione di calendari e rapporti sulle ferie

Ora puoi vedere il tempo libero dell’utente per una migliore pianificazione ed esecuzione. Puoi anche aggiungere ai dashboard nuovi rapporti e calendari di ferie per una visualizzazione in tempo reale della disponibilità degli utenti.

>[!NOTE]
>
>Disponibilità anteprima: 9 agosto 2019
>
>Disponibilità della produzione: 30 agosto 2019

## Il filtro Apri ora mostra più risultati in un elenco di problemi

Quando si applica il filtro Apri a un elenco di problemi, l’elenco include i problemi che:

* È in stato Chiuso - In attesa di approvazione
* Sono associati a un oggetto di risoluzione

Prima di questa modifica, questi problemi non venivano inclusi nell’elenco quando si applicava il filtro Apri.

## Nuova esperienza durante la modifica in linea delle informazioni negli elenchi

Quando si modificano le informazioni in linea nei nuovi elenchi, le righe modificate vengono disattivate, ma le informazioni rimangono visibili. Prima di questa modifica, le righe modificate erano disattivate e le informazioni non erano visibili.

I nuovi elenchi sono disponibili nelle seguenti aree di Workfront:

* Elenchi di progetti e attività
* Scheda Ore per Progetti, Attività e Problemi

## Elenchi aggiornati per le schede Ore progetto, attività e problemi

Le viste elenco migliorate sono ora disponibili nelle schede Ore per progetti, attività e problemi.

Prima di questo miglioramento, i nuovi elenchi venivano applicati solo ai seguenti elementi:

* Un elenco di attività
* Un elenco di progetti

Per informazioni sulla visualizzazione degli elementi in un elenco, vedere [Introduzione agli elenchi in Adobe Workfront](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

## Modifica Gantt senza attivare una modalità di modifica speciale

È ora possibile modificare l&#39;elenco delle attività Diagramma di Gantt quando il salvataggio automatico è abilitato o meno. Non è possibile annullare le modifiche quando l&#39;interruttore è attivo. In questo caso, le modifiche apportate al progetto vengono salvate automaticamente.

Per informazioni sulla modifica del diagramma di Gantt dell&#39;elenco delle attività, vedere [Aggiornare le informazioni nell&#39;elenco delle attività Diagramma di Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md).

## Rimozione della scheda Problemi dal Kanban Board

Stiamo rimuovendo la scheda Issues (Problemi) dalla bacheca Kanban nella versione 19.3 Production (Produzione). Puoi comunque accedere alla scheda secondaria Problemi dal backlog sul Kanban Board.

## Rimozione delle schede Documenti e Problemi dalla pagina dei dettagli dell’iterazione

>[!NOTE]
>
>Questa modifica verrà applicata in produzione con la versione 2019.3. Non verrà effettuata nell’ambiente di anteprima prima del rilascio in produzione.

Stiamo rimuovendo le schede Documenti e Problemi dalla pagina dei dettagli dell’iterazione Agile:

* **Documenti:** tutti i documenti memorizzati nella scheda Documenti devono essere spostati prima del rilascio della produzione. Se non si riesce a spostare i documenti, non sarà più possibile accedervi.
* **Problemi:** questa scheda si trova in genere nel menu a discesa Altro. È comunque possibile accedere alla scheda secondaria Problemi dalla scheda Elementi di lavoro nell’iterazione.

## Considerare o ignorare l&#39;indisponibilità dell&#39;utente nelle date dell&#39;attività

È ora possibile decidere se consentire o meno all&#39;assegnatario principale di un&#39;attività di adeguare le date pianificate.

Puoi prendere questa decisione a livello di sistema, come amministratore di Workfront o a livello di progetto, come project manager.

Prima di questa modifica, l&#39;indisponibilità dell&#39;assegnatario principale ha sempre adeguato le date pianificate dell&#39;attività, se il vincolo dell&#39;attività consente la modifica delle date.

Per informazioni sull&#39;impostazione del tempo di inattività utente a livello di sistema, vedere [Configurare le preferenze di progetto a livello di sistema](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Per informazioni sull&#39;impostazione del tempo di inattività utente a livello di progetto, vedere [Modifica progetti](../../../../manage-work/projects/manage-projects/edit-projects.md).

>[!NOTE]
>
>Disponibilità anteprima: 22 luglio 2019
>
>Disponibilità della produzione: 9 agosto 2019

## Condizioni personalizzate

Ora puoi fare quanto segue per personalizzare le Condizioni utilizzate per progetti, attività e problemi e soddisfare meglio le esigenze della tua organizzazione:

* Crea condizioni personalizzate con etichette e colori personalizzati.
* Modificare l&#39;ordine delle condizioni negli elenchi a discesa in cui gli utenti li selezionano.
* Utilizzare le condizioni personalizzate create al posto delle condizioni predefinite incorporate che Workfront assegna automaticamente agli elementi di lavoro.
* Modifica i nomi e i colori delle Condizioni predefinite incorporate per progetti, attività e problemi.

Inoltre, se si dispone dei diritti per modificare un&#39;attività o un problema ma non si è assegnati a esso (ad esempio perché si sta controllando l&#39;attività), è ora possibile modificarne la condizione utilizzando la colonna Condizioni in una vista a elenco.

In precedenza, le Condizioni non potevano essere personalizzate o modificate e solo gli utenti potevano modificare la Condizione di un’attività o di un problema se vi erano assegnati.

Per ulteriori informazioni, vedere [Condizioni personalizzate](../../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).

>[!NOTE]
>
>Disponibilità anteprima: 4 luglio 2019
>
>Disponibilità della produzione: fine settembre o inizio ottobre

## Nuova notifica e-mail per i team

È disponibile una nuova notifica e-mail dell’evento per i team. I membri del team ricevono una notifica e-mail quando un progetto con attività assegnate al team diventa attivo. Questa impostazione è disattivata per impostazione predefinita.

In precedenza, i membri del gruppo non potevano ricevere notifiche quando i progetti in questione diventavano attivi.

Per ulteriori informazioni, consulta Notifiche: informazioni sui progetti a cui partecipo.

>[!NOTE]
>
>Disponibilità anteprima: 4 luglio 2019
>
>Disponibilità della produzione: 18 luglio 2019

## Gli aggiornamenti dei documenti vengono ora visualizzati nell&#39;oggetto e nel progetto associati

Quando si aggiunge un commento a un documento, l&#39;aggiornamento viene ora visualizzato nella scheda Aggiornamenti sia per il documento che per l&#39;oggetto a cui è associato il documento.

Se l&#39;oggetto fa parte di un progetto, il commento sul documento viene visualizzato anche nella scheda Aggiornamenti del progetto.

In precedenza, i commenti di aggiornamento venivano visualizzati solo nella scheda Aggiornamenti del documento.

Per ulteriori informazioni, vedere la sezione [Aggiorna lavoro](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#updates) nell&#39;articolo [Aggiorna lavoro](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

>[!NOTE]
>
>Disponibilità anteprima: 6 giugno 2019
>
>Disponibilità della produzione: 20 giugno 2019

## Visibilità nella pianificazione dell’indisponibilità di un utente quando lo assegna ad attività e problemi

Quando assegni un utente a un’attività o a un problema, ora puoi visualizzare un avviso in linea se l’utente selezionato presenta un’indisponibilità programmata in un qualsiasi momento tra le date pianificate dell’attività o del problema.

Per informazioni sull&#39;assegnazione delle attività, vedere [Assegna attività](../../../../manage-work/tasks/assign-tasks/assign-tasks-1.md)

Per informazioni sulle ferie, vedere [Configurare le ferie personali](../../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

>[!NOTE]
>
>Disponibilità anteprima: 30 maggio 2019
>
>Disponibilità della produzione: 13 giugno 2019

## Aggiungere campi che rappresentano oggetti in Forms personalizzato

Nel generatore di moduli personalizzati è stato creato un nuovo tipo di campo denominato Typeahead. Questo campo consente di aggiungere ai moduli personalizzati campi che rappresentano oggetti. Attualmente, l&#39;oggetto User è abilitato con Typeahead e altri oggetti saranno disponibili in futuro.

In precedenza, gli amministratori dovevano gestire manualmente gli utenti come opzioni individuali nei menu a discesa dei moduli personalizzati.

>[!NOTE]
>
>Disponibilità anteprima: 30 maggio 2019
>
>Disponibilità della produzione: 13 giugno 2019
>
>Prima della data di rilascio della produzione, i nuovi campi personalizzati non sono supportati in Mobile, Outlook, MS Teams e nell’integrazione nativa di Salesforce.
>
>In produzione, sono ora supportati i team Outlook e MS. Mobile è supportato dalla fine di giugno o dall’inizio di luglio; le integrazioni Salesforce sono supportate da giugno.

## Il Nuovo Campo &quot;Subject&quot; Della Richiesta È Stato Rinominato In &quot;Name&quot;

>[!NOTE]
>
>Questa funzione è stata rimossa e non sarà inclusa nella versione 2019.3.

Adesso, quando si invia una nuova richiesta a una coda di richieste, si immette il nome della richiesta nel campo &quot;Nome&quot; del nuovo modulo di richiesta.

Prima di questa modifica, inserisci il nome della richiesta nel campo &quot;Oggetto&quot;.

Per informazioni sulla creazione di richieste, vedere [Creare e inviare richieste Workfront](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

