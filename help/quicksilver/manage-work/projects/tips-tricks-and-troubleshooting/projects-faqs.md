---
title: Domande frequenti sui progetti
description: Domande frequenti sui progetti
author: Alina
draft: Probably
feature: Work Management
exl-id: be262d72-f4e4-4426-a6bc-23499667fc97
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 0%

---

# Domande frequenti sui progetti

Di seguito sono riportate le domande frequenti sui progetti.

## Perché manca l&#39;opzione Inserisci attività sopra/sotto quando si fa clic con il pulsante destro del mouse su un&#39;attività nell&#39;elenco delle attività?

### Risposta

Per utilizzare le opzioni di inserimento, l&#39;elenco delle attività deve essere ordinato in base al numero. Per ordinare la colonna in base al numero, fare clic su **#** nell’intestazione della colonna a sinistra di **Nome attività** per riordinare l&#39;attività per numero.

## Qual è la data effettiva di completamento?

### Risposta

La data di completamento effettivo rappresenta la data e l&#39;ora del completamento del lavoro. Per ulteriori informazioni, consulta [Panoramica della data di completamento effettivo del progetto](../../../manage-work/projects/planning-a-project/project-actual-completion-date.md).

## Perché manca il pulsante rientro/rientro?

### Risposta

Per utilizzare il pulsante rientro/rientro, assicurarsi che le attività siano ordinate in base al numero dell&#39;attività e che non siano applicati gruppi.

## Perché non posso cambiare lo stato del progetto in Completato?

Ricevo il seguente messaggio di errore quando si tenta di contrassegnare il progetto come completo:

![Project_FAQ_Complete_Error_message.png](assets/project-faq-complete-error-message-350x138.png)

### Risposta

Non è possibile modificare lo stato di un progetto da completare se nel progetto è presente uno dei seguenti elementi:

* Attività o problemi incompleti
* Attività o problemi relativi allo stato di approvazione in sospeso

## Perché non posso cambiare lo stato del progetto da Completa a Corrente?

### Risposta

Se la modalità di completamento del progetto è impostata su Automatico, una volta completati tutti i task e i problemi, lo stato del progetto diventa automaticamente Completo e non è possibile modificarlo in nessun altro stato. La modalità di completamento del progetto deve essere impostata su Manuale per poter trasformare un progetto completo in Corrente. Per informazioni, consulta [Lo stato del progetto non cambia da Completa a Corrente](../../../manage-work/projects/tips-tricks-and-troubleshooting/project-status-does-not-change-from-complete-to-current.md).

## Perché non posso aggiungere un progetto a un Portfolio, anche se dispongo delle autorizzazioni corrette per farlo?

Sebbene io disponga delle autorizzazioni corrette, nella scheda Progetti del Portfolio manca il pulsante Aggiungi progetti .

### Risposta

Questo è causato dall&#39;inattivo stato del Portfolio. Per modificare lo stato del Portfolio:

1. Fai clic su **Dettagli Portfolio > Panoramica**.
1. Modificare la **Stato** a **Attivo.**

1. Fai clic su **Salva**.\
   La **Aggiungi progetti** ora il pulsante deve essere visibile sul **Progetti** scheda .

## Che accesso riceve un Resource Manager quando viene aggiunto a un progetto?

### Risposta

I responsabili risorse ricevono automaticamente Gestione accesso ai progetti. La rimozione dell&#39;utente dal ruolo Gestione risorse non rimuove l&#39;accesso alla condivisione di Gestione.

## Perché lo stato del progetto cambia quando aggiungo un gruppo?

### Risposta

Gli stati del progetto cambiano a causa degli stati predefiniti del gruppo. Quando aggiungi un gruppo a un progetto, questo modifica l’elenco degli stati negli stati predefiniti impostati per il gruppo.

Per ulteriori informazioni, consulta l’articolo [Creare o modificare uno stato](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

## Che cos&#39;è lo stato del budget?

### Risposta

Lo stato del budget mostrerà se il progetto è attualmente aggiunto al planner della capacità e se il calcolo del budget è stato completato.

Di seguito sono riportati gli Stati budget:

* Non incluso - Il progetto non viene aggiunto al planner di capacità.
* Incluso ma non calcolato - Il progetto viene aggiunto al Planner capacità ma viene escluso dal calcolo del budget.
* Incluso e calcolato - Il progetto viene aggiunto al Planner capacità e incluso nel calcolo del budget.

## Perché non posso condividere un progetto per il quale sono il proprietario e in cui dispongo delle autorizzazioni di gestione con un team? Non riesco semplicemente a trovare il team nella finestra di dialogo di condivisione del progetto.

### Risposta

L’amministratore di Adobe Workfront ti ha limitato a visualizzare solo le società, i gruppi e i team a cui appartieni nel tuo livello di accesso di . Il team a cui stai cercando non è uno dei team a cui appartieni.

![](assets/view-only-team-groups-companies-they-belong-to-350x141.png)

Per informazioni sull&#39;abilitazione di un utente alla visualizzazione di tutti i team nel sistema, vedi [Creare o modificare livelli di accesso personalizzati](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
