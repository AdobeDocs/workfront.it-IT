---
title: Domande frequenti sui progetti
description: Questo articolo contiene le domande più frequenti sui progetti in Adobe Workfront.
author: Alina
feature: Work Management
exl-id: be262d72-f4e4-4426-a6bc-23499667fc97
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '636'
ht-degree: 1%

---

# Domande frequenti sui progetti

Di seguito sono riportate le domande frequenti sui progetti.

## Perché manca Inserisci attività sopra/sotto quando si fa clic con il pulsante destro del mouse su un’attività nell’elenco delle attività?

### Risposta

Per utilizzare le opzioni di inserimento, l&#39;elenco delle attività deve essere ordinato per numero. Per ordinare la colonna in base al numero, fare clic su **#** nell&#39;intestazione della colonna a sinistra di **Nome attività** per ripristinare l&#39;attività in base al numero.

## Qual è la data di completamento effettiva?

### Risposta

La data di completamento effettiva rappresenta la data e l&#39;ora in cui il lavoro viene completato. Per ulteriori informazioni, vedere [Panoramica della data di completamento effettiva del progetto](../../../manage-work/projects/planning-a-project/project-actual-completion-date.md).

## Perché manca il pulsante Rientro/Rientro negativo?

### Risposta

Per utilizzare il pulsante Rientro/Rientro negativo, verificare che le attività siano ordinate in base al numero dell&#39;attività e che non siano stati applicati raggruppamenti.

## Perché non posso cambiare lo stato del progetto in Completato?

Quando si tenta di contrassegnare il progetto come completato viene visualizzato il seguente messaggio di errore:

![Project_FAQ_Complete_Error_message.png](assets/project-faq-complete-error-message-350x138.png)

### Risposta

Non puoi cambiare lo stato di un progetto da completare se nel progetto è presente una delle seguenti condizioni:

* Attività o problemi incompleti
* Attività o problemi in attesa di approvazione

## Perché non posso cambiare lo stato del progetto da Completo a Corrente?

### Risposta

Se la modalità di completamento del progetto è impostata su Automatico, dopo il completamento di tutte le attività e i problemi, lo stato del progetto diventa automaticamente Completo e non è possibile modificarlo in nessun altro stato. La Modalità di completamento del progetto deve essere impostata su Manuale per poter portare un progetto completo su Corrente. Per informazioni, vedere [Lo stato del progetto non cambierà da Completo a Corrente](../../../manage-work/projects/tips-tricks-and-troubleshooting/project-status-does-not-change-from-complete-to-current.md).

## Perché non è possibile aggiungere un progetto a un Portfolio, anche se si dispone delle autorizzazioni corrette?

Anche se dispongo delle autorizzazioni corrette, il pulsante Aggiungi progetti non è presente nella scheda Progetti di Portfolio.

### Risposta

Questo problema è causato dallo stato di inattività di Portfolio. Per modificare lo stato di Portfolio:

1. Fai clic su **Dettagli Portfolio > Panoramica**.
1. Cambia **Stato** in **Attivo.**

1. Fai clic su **Salva**.\
   Il pulsante **Aggiungi progetti** deve essere ora visibile nella scheda **Progetti**.

## Quale accesso riceve un Responsabile risorse quando viene aggiunto a un progetto?

### Risposta

I responsabili delle risorse ricevono automaticamente l&#39;accesso Gestisci ai progetti. Se si rimuove l’utente dal ruolo Responsabile risorse, non viene rimosso il relativo accesso di gestione condivisione.

## Perché cambia lo stato del progetto quando aggiungo un gruppo?

### Risposta

Gli stati del progetto cambiano a causa degli stati predefiniti del gruppo. Quando si aggiunge un gruppo a un progetto, l&#39;elenco degli stati viene modificato in quello predefinito impostato per il gruppo.

Per ulteriori informazioni, vedere l&#39;articolo [Creare o modificare uno stato](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

## Cos&#39;è lo stato del budget?

### Risposta

Lo stato del budget indica se il progetto è stato aggiunto o meno al Capacity Planner e se il calcolo del budget è stato completato.

Di seguito sono riportati gli stati del budget:

* Non incluso: il progetto non viene aggiunto al Capacity Planner.
* Incluso ma non calcolato: il progetto viene aggiunto al Capacity Planner ma escluso dal calcolo del budget.
* Incluso e calcolato: il progetto viene aggiunto al Capacity Planner e incluso nel calcolo del budget.

## Perché non posso condividere un progetto di cui sono proprietario e per il quale dispongo delle autorizzazioni di gestione per un team? Non riesco a trovare il team nella finestra di dialogo di condivisione del progetto.

### Risposta

L’amministratore Adobe Workfront ti ha limitato alla visualizzazione delle sole Società, dei gruppi e dei team a cui appartieni nel tuo Livello di accesso di. Il team che stai cercando non è uno dei team a cui appartieni.

![Visualizza solo team, gruppi e società a cui appartengono](assets/view-only-team-groups-companies-they-belong-to-350x141.png)

Per informazioni su come consentire a un utente di visualizzare tutti i team nel sistema, vedere [Creare o modificare livelli di accesso personalizzati](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
