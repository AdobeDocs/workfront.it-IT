---
content-type: release-notes
navigation-topic: product-releases-archive
title: Anteprima R1 4
description: Questa pagina descrive tutte le modifiche disponibili nell’ambiente di anteprima con la versione R1.4. La funzionalità in questa pagina è stata resa disponibile nell’ambiente di anteprima il 15 febbraio 2017.
author: Luke
feature: Product Announcements
exl-id: 2945e058-74dd-4cc3-9d6c-e5618ee7041c
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '847'
ht-degree: 0%

---

# Anteprima R1 4

Questa pagina descrive tutte le modifiche disponibili nell’ambiente di anteprima con la versione R1.4. La funzionalità in questa pagina è stata resa disponibile nell’ambiente di anteprima il 15 febbraio 2017.

Per un elenco di tutte le modifiche apportate in R1, vedere [Versione di Workfront R1](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/workfront-r1-release.md).

## Sono state aggiornate le approvazioni di progetti, attività e problemi

Durante la creazione dei processi di approvazione per le approvazioni di progetti, attività e problemi, sono ora disponibili i seguenti miglioramenti e modifiche: 

* I &quot;Passaggi&quot; di approvazione sono ora denominati &quot;Passaggi&quot; di approvazione.
* Include più tipi di approvatori per fase.\
  Ciò include utenti, team e ruoli.\
  Prima di questa modifica, era possibile includere solo più approvatori dello stesso tipo. Ad esempio, puoi includere più mansioni, ma non una mansione e un team.

* Sono state rimosse le seguenti limitazioni preesistenti relative alla modifica dei processi di approvazione globali esistenti:

   * Il processo di approvazione modificato si riflette solo sugli oggetti in tutto il sistema in cui il processo di approvazione non è ancora iniziato o in cui non è stato modificato. Gli oggetti in cui il processo di approvazione è già iniziato o in cui è stato modificato non vengono aggiornati con le modifiche apportate.
   * Non puoi modificare lo stato che determina quando inizia l’approvazione.

* Aspetto aggiornato.

Per ulteriori informazioni sulla creazione di processi di approvazione, consulta [Creare un processo di approvazione per gli elementi di lavoro](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

Quando si associa un processo di approvazione a un progetto, un’attività o un problema, sono ora disponibili i seguenti miglioramenti e modifiche:

* Aspetto aggiornato.
* Nella scheda Approvazioni viene visualizzato un diagramma di approvazione che mostra una rappresentazione visiva dei passaggi di approvazione precedenti, correnti e futuri.

Per ulteriori informazioni sull&#39;associazione delle approvazioni a progetti, attività e problemi, vedi [Associa un processo di approvazione nuovo o esistente al lavoro](../../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Modificare lo stato di un progetto direttamente dalla pagina del progetto

Non è più necessario modificare un progetto per cambiarne lo stato. Ora puoi modificare lo stato di un progetto direttamente dalla pagina principale.

Per ulteriori informazioni, consulta [Modificare lo stato di un progetto](../../../../manage-work/projects/manage-projects/change-project-status.md).

## Pianifica utenti per la disattivazione

Ora puoi pianificare la disattivazione degli utenti in una data futura.

Prima di questo miglioramento, era possibile disattivare un utente solo manualmente immediatamente.

La pianificazione della disattivazione di un utente può essere utile in diversi scenari. Ad esempio, se crei utenti in Workfront che vengono assunti temporaneamente, puoi impostarli per essere disattivati al termine del contratto.

Questa funzione è disponibile anche per gli utenti che eseguono modifiche in serie. 

Per ulteriori informazioni sulla pianificazione della disattivazione degli utenti, consulta [Disattivare o riattivare un utente](../../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md) e [Aggiungi utenti](../../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Nuove opzioni di riepilogo e-mail per &quot;Azioni necessarie&quot;

L’opzione di consegna Riepilogo giornaliero è ora disponibile nell’area &quot;Azione richiesta&quot; delle impostazioni delle notifiche.

Per ulteriori informazioni, consulta [Modifica le tue notifiche e-mail](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Ricorda di aggiornare l’indirizzo e-mail associato al tuo account per poter testare questa funzionalità. Questo è necessario perché la Sandbox di anteprima cancella gli indirizzi e-mail su tutti gli utenti.

## Miglioramento del cestino: registrato nel flusso di aggiornamento e notifica e-mail di ricezione

Sono stati aggiunti i seguenti miglioramenti durante il ripristino di progetti, attività e problemi eliminati:

* Dopo aver ripristinato un oggetto, ora ricevi una notifica e-mail.\
  In qualità di amministratore di Workfront, ora ricevi una notifica e-mail dopo aver ripristinato un progetto, un’attività o un problema precedentemente eliminato. La notifica e-mail ti informa sullo stato del processo di ripristino.\
  Per ulteriori informazioni sul ripristino di oggetti in Workfront, vedere [Ripristina elementi eliminati](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

* Quando l&#39;oggetto viene ripristinato, l&#39;eliminazione e il ripristino dell&#39;oggetto vengono ora registrati nel flusso di aggiornamento dell&#39;oggetto stesso e nel flusso di aggiornamento dell&#39;oggetto padre.\
  In precedenza, nel flusso di aggiornamento dell&#39;oggetto padre veniva registrata solo l&#39;eliminazione.\
  Ad esempio, quando l&#39;attività viene ripristinata, al flusso di aggiornamento del progetto e dell&#39;attività viene aggiunto un messaggio che indica che l&#39;attività è stata ripristinata. Le eliminazioni e i ripristini non vengono registrati nelle sottoattività. Le informazioni relative all&#39;eliminazione e al ripristino di sottoattività sono disponibili solo per le attività padre.)\
  Per ulteriori informazioni, consulta [Ripristina elementi eliminati](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

 

## Finestra di dialogo aggiornata per la gestione dell&#39;appartenenza al gruppo

La nuova interfaccia per la gestione dei gruppi e dei sottogruppi offre un’esperienza più semplice e intuitiva.

I campi Proprietari gruppo e Membri gruppo sono ora combinati in un unico campo, con un elenco di membri del gruppo elencato di seguito. È inoltre possibile filtrare l&#39;elenco dei membri del gruppo e specificare se si tratta di un proprietario o di un membro. 

Per ulteriori informazioni sull&#39;aggiunta di sottogruppi ai gruppi e sulla designazione di utenti come membri o proprietari di gruppi, vedere [Creare un gruppo](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) e [Creare un gruppo](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md). 

 

## Copiare testo nell’app mobile

Puoi copiare il testo nei seguenti campi di tutti gli oggetti visibili nell’app mobile:

* Nome
* Descrizione
* Numero di riferimento
* Commenti

Questa funzionalità dovrebbe essere rilasciata agli app store iOS e Android la settimana del 13 febbraio.
