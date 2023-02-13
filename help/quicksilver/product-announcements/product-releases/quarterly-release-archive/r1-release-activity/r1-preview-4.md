---
content-type: release-notes
navigation-topic: product-releases-archive
title: Anteprima R1 4
description: Questa pagina descrive tutte le modifiche disponibili nell’ambiente Anteprima con la versione R1.4. La funzionalità di questa pagina è stata resa disponibile nell’ambiente Anteprima il 15 febbraio 2017.
author: Luke
feature: Product Announcements
exl-id: 2945e058-74dd-4cc3-9d6c-e5618ee7041c
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '849'
ht-degree: 0%

---

# Anteprima R1 4

Questa pagina descrive tutte le modifiche disponibili nell’ambiente Anteprima con la versione R1.4. La funzionalità di questa pagina è stata resa disponibile nell’ambiente Anteprima il 15 febbraio 2017.

Per un elenco di tutte le modifiche apportate in R1, vedi [Versione Workfront R1](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/workfront-r1-release.md).

## Approvazioni di progetti, attività e problemi aggiornate

Durante la creazione di processi di approvazione per progetti, attività e approvazioni dei problemi, sono ora disponibili i seguenti miglioramenti e modifiche: 

* I &quot;passi&quot; di approvazione sono ora chiamati &quot;stadi&quot; di approvazione.
* Includere più tipi di approvatori per fase.\
   Ciò include utenti, team e ruoli di lavoro.\
   Prima di questa modifica, era possibile includere solo più approvatori dello stesso tipo. Ad esempio, è possibile includere più ruoli di lavoro, ma non un ruolo di lavoro e un team.

* Sono state rimosse le seguenti limitazioni preesistenti relative alla modifica dei processi di approvazione globale esistenti:

   * Il processo di approvazione modificato si riflette solo sugli oggetti di tutto il sistema in cui il processo di approvazione non è ancora iniziato o il processo di approvazione non è stato modificato. Gli oggetti in cui il processo di approvazione è già stato avviato o il processo di approvazione è stato modificato non vengono aggiornati con le modifiche apportate.
   * Non è possibile modificare lo stato che determina l&#39;avvio dell&#39;approvazione.

* Aspetto aggiornato.

Per ulteriori informazioni sulla creazione dei processi di approvazione, consulta [Creazione di un processo di approvazione per gli elementi di lavoro](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

Quando si associa un processo di approvazione a un progetto, un&#39;attività o un problema, sono ora disponibili i seguenti miglioramenti e modifiche:

* Aspetto aggiornato.
* Il diagramma di approvazione viene visualizzato nella scheda Approvazioni , mostrando una rappresentazione visiva dei passaggi di approvazione precedenti, correnti e futuri.

Per ulteriori informazioni sull&#39;associazione delle approvazioni a progetti, attività e problemi, consulta [Associa un processo di approvazione nuovo o esistente al lavoro](../../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Modificare lo stato di un progetto direttamente dalla pagina Progetto

Non è più necessario modificare un progetto per modificarne lo stato. Ora puoi modificare lo stato di un progetto direttamente dalla pagina principale del progetto.

Per ulteriori informazioni, consulta [Modificare lo stato di un progetto](../../../../manage-work/projects/manage-projects/change-project-status.md).

## Pianificare gli utenti per la disattivazione

Ora puoi pianificare la disattivazione degli utenti in una data futura.

Prima di questo miglioramento, era possibile disattivare manualmente un utente solo immediatamente.

La pianificazione di un utente da disattivare può essere utile in diversi scenari. Ad esempio, se crei utenti in Workfront assunti temporaneamente, puoi impostarli per essere disattivati al termine del contratto.

Questa funzione è disponibile anche per utenti che effettuano modifiche in serie. 

Per ulteriori informazioni sulla pianificazione degli utenti per la disattivazione, consulta [Disattivare o riattivare un utente](../../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md) e [Aggiungi utenti](../../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Nuove opzioni di digest e-mail per &quot;Azioni necessarie&quot;

L’opzione di consegna Daily Digest è ora disponibile nell’area &quot;Azione necessaria&quot; delle impostazioni Notifiche.

Per ulteriori informazioni, consulta [Attivare o disattivare le notifiche degli eventi personali](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Ricorda di aggiornare l’indirizzo e-mail associato al tuo account per poter testare questa funzionalità. Questo è necessario perché la Sandbox Anteprima cancella gli indirizzi e-mail su tutti gli utenti.

## Miglioramento Cestino: Registrato nell’aggiornamento del flusso e ricevere notifiche e-mail

Sono stati aggiunti i seguenti miglioramenti durante il ripristino di progetti, attività e problemi eliminati:

* Ora ricevi una notifica e-mail dopo il ripristino di un oggetto.\
   In qualità di amministratore di Workfront, ora ricevi una notifica e-mail dopo il ripristino di un progetto, un’attività o un problema precedentemente eliminato. La notifica e-mail ti informa sullo stato del processo di ripristino.\
   Per ulteriori informazioni sul ripristino degli oggetti in Workfront, vedere [Ripristina elementi eliminati](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

* Quando l&#39;oggetto viene ripristinato, l&#39;eliminazione e il ripristino dell&#39;oggetto vengono ora registrati nel flusso di aggiornamento dell&#39;oggetto stesso e nel flusso di aggiornamento dell&#39;oggetto principale.\
   In precedenza, solo l&#39;eliminazione veniva registrata nel flusso di aggiornamento dell&#39;oggetto principale.\
   Ad esempio, quando l’attività viene ripristinata, viene aggiunto un messaggio al flusso di aggiornamento sia del progetto che dell’attività stessa, a indicare che l’attività è stata ripristinata. (Le eliminazioni e i ripristini non vengono registrati nelle sottoattività. Le informazioni relative alle eliminazioni e ai ripristini delle sottoattività sono disponibili solo per le attività principali.)\
   Per ulteriori informazioni, consulta [Ripristina elementi eliminati](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

 

## Finestra di dialogo aggiornata per la gestione dell’appartenenza al gruppo

È disponibile una nuova interfaccia per la gestione di gruppi e sottogruppi che offre un’esperienza più semplice e intuitiva.

Il campo Proprietari del gruppo e il campo Membri del gruppo vengono ora combinati in un unico campo, con un elenco di membri del gruppo elencati di seguito. Inoltre, è possibile filtrare l&#39;elenco dei membri del gruppo e modificare se si tratta di un proprietario o di un membro. 

Per ulteriori informazioni sull&#39;aggiunta di sottogruppi ai gruppi e sulla designazione degli utenti come membri o proprietari di gruppi di gruppi, vedere [Creare un gruppo](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) e [Creare un gruppo](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md). 

 

## Copiare il testo nell’app mobile

Puoi copiare il testo nei seguenti campi di tutti gli oggetti visibili nell’app mobile:

* Nome
* Descrizione
* Numero di riferimento
* Commenti

Questa funzionalità deve essere rilasciata agli app store iOS e Android la settimana del 13 febbraio.
