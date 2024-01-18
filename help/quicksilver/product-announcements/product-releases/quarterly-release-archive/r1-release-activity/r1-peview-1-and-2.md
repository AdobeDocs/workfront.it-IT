---
content-type: release-notes
navigation-topic: product-releases-archive
title: Anteprima R1 1 e 2
description: Questa pagina descrive tutte le modifiche disponibili nell’ambiente di anteprima con le versioni R1.1 e R1.2. La funzionalità in questa pagina è stata resa disponibile nell’ambiente di anteprima il 19 gennaio 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 65219cf1-809f-4d8e-a858-01f7881064d7
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1143'
ht-degree: 2%

---

# Anteprima R1 1 e 2

Questa pagina descrive tutte le modifiche disponibili nell’ambiente di anteprima con le versioni R1.1 e R1.2. La funzionalità in questa pagina è stata resa disponibile nell’ambiente di anteprima il 19 gennaio 2017.

Per un elenco di tutte le modifiche apportate in R1, vedere [Panoramica dell’attività sulla versione R1](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/r1-release-activity-overview.md). 

## Ripristina progetti, attività e problemi dal cestino 

Gli amministratori di Workfront ora possono ripristinare progetti, attività e problemi eliminati negli ultimi 30 giorni. Tutte le informazioni associate al progetto, all&#39;attività o al problema vengono ripristinate, inclusi i documenti e i dati personalizzati.

Sono disponibili nuove opzioni per configurare cosa accade alle ore registrate per un progetto, un’attività o un problema eliminato. Per ulteriori informazioni, consulta [La configurazione influisce sulle ore di eliminazione e ripristino di un oggetto](../../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md).

Per ulteriori informazioni sul ripristino di oggetti in Workfront, vedere [Ripristina elementi eliminati](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

Per informazioni su come visualizzare progetti, attività e problemi ripristinati di recente, vedi [Visualizza elemento ripristinato](../../../../administration-and-setup/manage-workfront/manage-deleted-items/view-restored-items.md).

## Diagramma di approvazione mostra la rappresentazione visiva dei passaggi di approvazione precedenti, correnti e futuri

Ora, quando un’approvazione è in sospeso per un progetto, un’attività o un problema, viene visualizzato un diagramma. Il diagramma di approvazione mostra la fase corrente del processo di approvazione (in sospeso) e consente inoltre di visualizzare rapidamente le fasi di approvazione precedenti e future senza passare alla scheda Approvazioni.

Prima di questa modifica, le informazioni sui passaggi di approvazione erano disponibili solo nella scheda Approvazioni all’interno del progetto, dell’attività o del problema e venivano visualizzate solo in una vista a elenco anziché a diagramma. Queste informazioni sono ancora disponibili e non modificate nella scheda Approvazioni.

Nei progetti, le informazioni sull’approvazione vengono visualizzate nell’intestazione accanto al titolo del progetto. Per le attività e i problemi, le informazioni sull’approvazione vengono visualizzate nel pannello di destra.

Per ulteriori informazioni, consulta [Approvazione del lavoro](../../../../review-and-approve-work/manage-approvals/approving-work.md) in  [Approvazione del lavoro](../../../../review-and-approve-work/manage-approvals/approving-work.md).

## Configura gli oggetti da aggiornare in attesa di approvazione

Quando un progetto, un’attività o un problema è in attesa di approvazione, ora puoi configurare se gli utenti possono:

* Modifica il modulo personalizzato di un progetto, attività o problema in attesa di approvazione.\
  Per informazioni su come configurare progetti, attività e problemi da modificare in attesa di approvazione, consulta [Configurare le impostazioni di approvazione globali](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md)

* Aggiungi problemi a un progetto in attesa di approvazione.\
  Per informazioni su come configurare i progetti in modo che gli utenti possano aggiungere problemi quando il progetto è in attesa di approvazione, consulta [Configurare le preferenze di progetto a livello di sistema](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Modifica attività e problemi in un progetto in attesa di approvazione.\
  Per informazioni su come configurare i progetti per consentire agli utenti di modificare attività e problemi quando il progetto è in attesa di approvazione, consulta [Configurare le preferenze di progetto a livello di sistema](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Prima di questa modifica, non era possibile modificare progetti, attività e problemi in attesa di approvazione; inoltre, non era possibile aggiungere problemi a progetti in attesa di approvazione e non era possibile modificare attività e problemi in progetti in attesa di approvazione.

## Assegnare modelli di layout ai gruppi

È ora possibile assegnare modelli di layout ai gruppi.

Prima di questa modifica, era possibile assegnare modelli di layout a utenti, team e mansioni. L&#39;assegnazione di un modello di layout ai gruppi ha la priorità di assegnazione più bassa. 

Per ulteriori informazioni, vedere &quot;Creazione e gestione di modelli di layout&quot;.

## Modifiche alle notifiche utente per modifica in blocco

La funzionalità è cambiata in seguito alla modifica in blocco delle impostazioni di notifica e-mail dell’utente. Quando selezioni più utenti per modificare le impostazioni delle e-mail di notifica, vengono modificate solo le notifiche specifiche che stai aggiornando per tutti gli utenti selezionati. Tutte le impostazioni delle notifiche e-mail non modificate rimangono invariate per tutti gli utenti selezionati, anche se sono diverse da utente a utente. 

Prima di questa modifica, le impostazioni di notifica e-mail selezionate erano state salvate e tutte le altre impostazioni di notifica non modificate erano state deselezionate al momento del salvataggio delle modifiche. 

Per ulteriori informazioni, consulta &quot;Modifica delle impostazioni di notifica degli utenti in blocco&quot; in [Modifica le tue notifiche e-mail](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## È stato aggiornato l’aspetto di diverse notifiche e-mail

L’aspetto delle seguenti notifiche e-mail è stato aggiornato con una nuova interfaccia utente:

* Assegnazione problema
* Conferma modifiche data
* Un progetto a cui partecipo diventa attivo
* Decisione di approvazione delle parti interessate
* Completamento di un&#39;attività predecessore a task dipendenti
* In attesa di approvazione (progetto, attività, problemi)
* Modifica stato su progetti, attività, problemi

Ricordati di aggiornare l’indirizzo e-mail associato al tuo account per poter testare questa funzionalità, poiché la Sandbox di anteprima cancella gli indirizzi e-mail su tutti gli utenti.    Per ulteriori informazioni sulle notifiche e-mail, consulta [Notifiche Adobe Workfront](../../../../workfront-basics/using-notifications/wf-notifications.md).  

## Nuove opzioni di riepilogo e-mail per diverse aree di notifica

Nelle seguenti aree di notifica è stata aggiunta l’opzione &quot;Riepilogo giornaliero&quot;:

* Informazioni sui progetti a cui collaboro
* Informazioni sui progetti di cui sono sponsor
* Informazioni sull&#39;approvazione
* Informazioni sul lavoro assegnato a me
* Comunicazione

Per ulteriori informazioni, consulta [Notifiche Adobe Workfront](../../../../workfront-basics/using-notifications/wf-notifications.md).  Ricordati di aggiornare l’indirizzo e-mail associato al tuo account per poter testare questa funzionalità, poiché la Sandbox di anteprima cancella gli indirizzi e-mail su tutti gli utenti. 

## Rendi pubblico un gruppo

Quando rendi pubblico un gruppo, ora puoi aggiungerlo agli utenti senza esserne il proprietario. Per poter modificare gli utenti è necessario disporre dell&#39;accesso di amministratore.

Per ulteriori informazioni su come rendere pubblico un gruppo, vedere [Creare un gruppo](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#making-a-group-public) sezione in [Creare un gruppo](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

## Condividere l’URL di un oggetto nell’app mobile 

Ora puoi condividere l’URL sui seguenti oggetti nell’app mobile Workfront:

* Progetti
* Attività
* Problemi
* Schede orario
* Documenti

È possibile condividere un URL di un oggetto nelle seguenti applicazioni:

* SMS
* E-mail
* Unità di archiviazione (ad esempio unità iCloud)
* Un&#39;altra applicazione installata, ad esempio Notes, Facebook
* È possibile copiare un collegamento all&#39;oggetto negli Appunti e incollarlo successivamente in qualsiasi altra applicazione. 

## Guida sensibile al contesto nella configurazione

Tutte le aree del menu Configurazione sono state aggiornate con un&#39;icona Aiuto nell&#39;angolo superiore destro dell&#39;area. Questa icona fornisce un collegamento a un articolo del sito della Guida relativo a tale area. Alcune sezioni all’interno delle aree di Configurazione sono state aggiornate anche con l’icona Aiuto. 

## Aggiungi tariffe di spesa più precise

Ora è possibile aggiungere tassi di spesa più esatti durante la creazione dei tipi di spesa. Le tariffe di spesa possono contenere fino a 4 caratteri dopo il decimale (ad esempio, 1,0375). Ciò significa che qualsiasi campo che utilizza questo tasso può essere più preciso.

Prima di questa modifica, le tariffe di spesa potevano contenere solo fino a 2 caratteri dopo il decimale (ad esempio, 1,03).

Per ulteriori informazioni sulla creazione delle tariffe di spesa, consulta [Creare tipi di spesa personalizzati](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-custom-expense-types.md).

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Updated Look and Improved Performance in the Tasks&nbsp;List (by request only)</h2>
-->

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
This feature focuses primarily on improving the performance of large lists of tasks. The interface of tasks lists has been updated, but delivers the same functionality as the existing tasks list. You can have access to the new tasks list only if you request it. For more information about how to request access to the new tasks list, see Testing Tasks Lists (Beta).
</MadCap:conditionalText>
-->

 

## Registrazione webinar R1 Preview 1 e 2 Release

Questo webinar è stato presentato dal team di preparazione alla versione di Workfront il 19 gennaio 2017. Questo webinar si è concentrato sulle modifiche di versione del 2017 e ha trattato le nuove funzionalità disponibili per il test in Anteprima.
