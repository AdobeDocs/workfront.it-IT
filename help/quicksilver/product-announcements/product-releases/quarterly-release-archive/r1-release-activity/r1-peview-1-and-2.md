---
content-type: release-notes
navigation-topic: product-releases-archive
title: Anteprima 1 e 2 R1
description: Questa pagina descrive tutte le modifiche disponibili nell’ambiente Preview con le versioni R1.1 e R1.2. La funzionalità di questa pagina è stata resa disponibile nell’ambiente Anteprima il 19 gennaio 2017.
author: Luke
feature: Product Announcements
exl-id: 65219cf1-809f-4d8e-a858-01f7881064d7
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1133'
ht-degree: 2%

---

# Anteprima 1 e 2 R1

Questa pagina descrive tutte le modifiche disponibili nell’ambiente Preview con le versioni R1.1 e R1.2. La funzionalità di questa pagina è stata resa disponibile nell’ambiente Anteprima il 19 gennaio 2017.

Per un elenco di tutte le modifiche apportate in R1, vedi [Panoramica dell’attività di rilascio di R1](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/r1-release-activity-overview.md). 

## Ripristinare progetti, attività e problemi dal Cestino 

Gli amministratori di Workfront possono ora ripristinare progetti, attività e problemi che sono stati eliminati negli ultimi 30 giorni. Tutte le informazioni associate al progetto, all&#39;attività o al problema vengono ripristinate, inclusi documenti e dati personalizzati.

Sono inoltre disponibili nuove opzioni per la configurazione di ciò che accade alle ore registrate rispetto a un progetto, un&#39;attività o un problema eliminato. Per ulteriori informazioni, consulta [La configurazione influisce sulle ore in cui un oggetto viene eliminato e ripristinato](../../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md).

Per ulteriori informazioni sul ripristino degli oggetti in Workfront, vedere [Ripristina elementi eliminati](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

Per informazioni su come visualizzare progetti, attività e problemi recentemente ripristinati, consulta [Visualizza elemento ripristinato](../../../../administration-and-setup/manage-workfront/manage-deleted-items/view-restored-items.md).

## Il diagramma di approvazione mostra la rappresentazione visiva dei passaggi di approvazione precedenti, correnti e futuri

Ora quando un&#39;approvazione è in sospeso per un progetto, un&#39;attività o un problema, viene visualizzato un diagramma. Il diagramma di approvazione mostra il passaggio corrente nel processo di approvazione (in sospeso) e consente inoltre di visualizzare rapidamente i passaggi di approvazione precedenti e futuri senza passare alla scheda Approvazioni .

Prima di questa modifica, le informazioni sui passaggi di approvazione erano disponibili solo nella scheda Approvazioni all&#39;interno del progetto, dell&#39;attività o del problema e venivano visualizzate solo in una vista a elenco anziché in una vista a diagramma. (Queste informazioni sono ancora disponibili e rimaste invariate nella scheda Approvazioni .)

Nei progetti, le informazioni di approvazione vengono visualizzate nell’intestazione accanto al titolo del progetto. Per attività e problemi, le informazioni di approvazione vengono visualizzate nel pannello di destra.

Per ulteriori informazioni, consulta [Approvazione del lavoro](../../../../review-and-approve-work/manage-approvals/approving-work.md) in  [Approvazione del lavoro](../../../../review-and-approve-work/manage-approvals/approving-work.md).

## Configurare gli oggetti da aggiornare in attesa di approvazione

Quando un progetto, un&#39;attività o un problema è in attesa di approvazione, ora puoi configurare se gli utenti possono:

* Modificare la forma personalizzata di un progetto, un&#39;attività o un problema in attesa di approvazione.\
   Per informazioni su come configurare progetti, attività e problemi da modificare durante l&#39;approvazione in attesa, consulta [Configurare le impostazioni di approvazione globali](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md)

* Aggiungi i problemi a un progetto in attesa di approvazione.\
   Per informazioni su come configurare i progetti per consentire agli utenti di aggiungere problemi quando il progetto è in attesa di approvazione, consulta [Configurare le preferenze del progetto a livello di sistema](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Modifica attività e problemi all’interno di un progetto in attesa di approvazione.\
   Per informazioni su come configurare progetti per consentire agli utenti di modificare attività e problemi quando il progetto è in attesa di approvazione, consulta [Configurare le preferenze del progetto a livello di sistema](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Prima di tale modifica non era possibile modificare progetti, attività e problemi in attesa di approvazione; inoltre, non è stato possibile aggiungere problemi ai progetti in attesa di approvazione e non è stato possibile modificare attività e problemi all’interno di progetti in attesa di approvazione.

## Assegnare modelli di layout ai gruppi

È ora possibile assegnare modelli di layout ai gruppi.

Prima di questa modifica, era possibile assegnare modelli di layout a utenti, team e ruoli di lavoro. L&#39;assegnazione di un modello di layout ai gruppi ha il rango più basso nella priorità di assegnazione del modello di layout. 

Per ulteriori informazioni, vedere &quot;Creazione e gestione di modelli di layout&quot;.

## Modifiche alle notifiche utente per la modifica in serie

La funzionalità è cambiata in seguito alla modifica collettiva delle impostazioni di notifica tramite e-mail degli utenti. Quando selezioni più utenti per modificare le loro impostazioni e-mail di notifica, vengono modificate solo le notifiche specifiche che stai aggiornando per tutti gli utenti selezionati. Tutte le impostazioni di notifica e-mail rimaste invariate rimangono invariate per tutti gli utenti selezionati, anche se sono diverse da utente a utente. 

Prima di questa modifica, le impostazioni di notifica e-mail selezionate venivano salvate e tutte le altre impostazioni di notifica rimaste invariate venivano deselezionate al momento del salvataggio delle modifiche. 

Per ulteriori informazioni, consulta &quot;Modifica in blocco delle impostazioni di notifica utente&quot; in [Attivare o disattivare le notifiche degli eventi personali](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## Aspetto aggiornato di diverse notifiche e-mail

L’aspetto delle seguenti notifiche e-mail è stato aggiornato con una nuova interfaccia utente:

* Assegnazione dei problemi
* Modifiche alla data del commit
* Quando si cambia lo stato del progetto da Idea/Approvato/Richiesta/Pianificazione ad Attuale, invia una Email alla squadra
* Decisione di approvazione alle parti interessate
* Completamento attività predecessore a dipendenti di attività
* Approvazione in sospeso (progetto, attività, problemi)
* Modifica dello stato di progetti, attività, problemi

Ricorda di aggiornare l’indirizzo e-mail associato al tuo account per poter testare questa funzionalità, in quanto la Sandbox Anteprima cancella gli indirizzi e-mail su tutti gli utenti.    Per ulteriori informazioni sulle notifiche e-mail, vedi [Notifiche Adobe Workfront](../../../../workfront-basics/using-notifications/wf-notifications.md).  

## Nuove opzioni di riepilogo e-mail per diverse aree di notifica

Sono state aggiunte le seguenti aree di notifica con l’opzione &quot;Riepilogo giornaliero&quot;:

* Informazioni sui progetti
* Informazioni sui progetti di cui sono sponsor
* Informazioni sull&#39;approvazione
* Informazioni sul lavoro assegnato a me
* Comunicazione

Per ulteriori informazioni, consulta [Notifiche Adobe Workfront](../../../../workfront-basics/using-notifications/wf-notifications.md).  Ricorda di aggiornare l’indirizzo e-mail associato al tuo account per poter testare questa funzionalità, in quanto la Sandbox Anteprima cancella gli indirizzi e-mail su tutti gli utenti. 

## Rendi pubblico un gruppo

Quando si rende pubblico un gruppo, è ora possibile aggiungerlo agli utenti senza essere proprietario del gruppo. Per poter modificare gli utenti dovrai disporre dell’accesso amministrativo per gli utenti.

Per ulteriori informazioni su come rendere pubblico un gruppo, consulta la [Creare un gruppo](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#making-a-group-public) sezione [Creare un gruppo](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

## Condividere l’URL di un oggetto nell’app mobile 

Ora puoi condividere l’URL sui seguenti oggetti nell’app mobile Workfront:

* Progetti
* Attività
* Problemi
* Schede orario
* Documenti

Puoi condividere un URL di un oggetto nelle seguenti applicazioni:

* Messaggio di testo
* E-mail
* Unità di archiviazione (ad esempio unità iCloud)
* Un&#39;altra applicazione installata (ad esempio, Note, Facebook)
* Puoi copiare un collegamento all’oggetto negli Appunti e incollarlo in un secondo momento in un’altra applicazione. 

## Guida sensibile al contesto nella configurazione

Tutte le aree del menu Configurazione sono state aggiornate con un&#39;icona Aiuto nell&#39;angolo superiore destro dell&#39;area. Questa icona fornisce un collegamento a un articolo del sito della Guida relativo a tale area. Anche alcune sezioni all’interno delle aree di installazione sono state aggiornate con l’icona Aiuto . 

## Aggiungi tariffe più precise

Ora è possibile aggiungere tassi di spesa più esatti quando si creano tipi di spesa. Le percentuali di spesa possono contenere fino a 4 caratteri dopo il decimale (ad esempio, 1.0375). Ciò significa che tutti i campi che utilizzano questo tasso possono essere più precisi.

Prima di questa modifica, i tassi di spesa potevano contenere solo fino a 2 caratteri dopo il decimale (ad esempio, 1,03).

Per ulteriori informazioni sulla creazione dei tassi di spesa, vedere [Crea tipi di spesa personalizzati](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-custom-expense-types.md).

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Updated Look and Improved Performance in the Tasks&nbsp;List (by request only)</h2>
-->

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
This feature focuses primarily on improving the performance of large lists of tasks. The interface of tasks lists has been updated, but delivers the same functionality as the existing tasks list. You can have access to the new tasks list only if you request it. For more information about how to request access to the new tasks list, see Testing Tasks Lists (Beta).
</MadCap:conditionalText>
-->

 

## Registrazione webinar R1 Preview 1 e 2 versione

Questo Webinar è stato presentato dal team di preparazione alla versione di Workfront il 19 gennaio 2017. Questo webinar si è concentrato sulle modifiche alla versione nel 2017 e ha trattato le nuove funzionalità disponibili per il test in Anteprima.
