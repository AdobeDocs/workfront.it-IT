---
product-area: projects
navigation-topic: approvals
title: Connettere Workfront e Frame.io
description: Workfront utilizza Frame.io nel processo di revisione e approvazione per incontrare le persone che desiderano lavorare. La gestione e l'approvazione del progetto vengono gestite in Workfront e il processo di revisione viene eseguito in Frame.io.
author: Courtney
feature: Work Management, Digital Content and Documents
source-git-commit: cf8501ff21dc9f3a3c66d8e98555986f18aeaa80
workflow-type: tm+mt
source-wordcount: '632'
ht-degree: 0%

---


# Connettere Workfront e Frame.io

Workfront utilizza Frame.io nel processo di revisione e approvazione per incontrare le persone che desiderano lavorare. La gestione e l&#39;approvazione del progetto vengono gestite in Workfront e il processo di revisione viene completato in Frame.io. Per configurare correttamente l’integrazione, devi completare tutte le sezioni seguenti:

* [Collegare un gruppo Workfront a un team Frame.io](#connect-a-workfront-group-to-a-frameio-team)
* [Creazione di un progetto Workfront e aggiunta di un gruppo connesso](#create-a-workfront-project-and-add-a-connected-group)

Il contenuto di questo articolo fa riferimento alla funzionalità di approvazione dei documenti aggiornata, disponibile solo per account specifici. Per informazioni sui processi di approvazione standard, vedi gli articoli elencati in [Approvazioni lavoro](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

## Requisiti di accesso

* Per utilizzare le funzionalità descritte in questo articolo, è necessario eseguire l’onboarding manuale dell’organizzazione. Per ulteriori informazioni, consulta [Integrazione alfa nativa di Adobe Workfront e Frame.io: panoramica](/help/quicksilver/product-announcements/betas/frame-io-wf-integration-alpha/frame-io-wf-integration-alpha-overview.md).


## Collegare un gruppo Workfront a un team Frame.io

Questa funzione verrà attivamente migliorata per la disponibilità generale a maggio.

### Prerequisiti

* Crea un team Frame.io da mappare a un gruppo Workfront.
* Trova il token sviluppatore API per il team. Per ulteriori informazioni, consulta [Token per sviluppatori](https://developer.frame.io/docs/getting-started/authentication#developer-tokens) sul sito per sviluppatori Frame.io.

### Collegare un gruppo Workfront a un team Frame.io

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Gruppi**.
1. Scegliete un gruppo esistente o fate clic su **Crea gruppo**.
1. Nel pannello a sinistra, fai clic su **Connetti a Frame.io**.
   ![](assets/connect-frame-group.png)
1. Immetti il token di sviluppo API.
1. Clic **Avvia connessione**.
1. (Condizionale) Se siete l&#39;amministratore di più account Frame.io, selezionate l&#39;account che desiderate utilizzare.

## Creazione di un progetto Workfront e aggiunta di un gruppo connesso

Dopo aver connesso un gruppo Workfront a un team Frame.io, è necessario creare un progetto con tale gruppo connesso.

### Prerequisiti

* È necessario disporre di un gruppo Workfront connesso a un team Frame.io come spiegato nella sezione precedente.

### Creazione di un progetto Workfront e aggiunta di un gruppo connesso

{{step1-to-projects}}

1. Crea un nuovo progetto da zero o da un modello. Per informazioni su come creare un progetto, consulta [Creare un progetto](/help/quicksilver/manage-work/projects/create-projects/create-project.md).

1. Nel pannello a sinistra, individua **Dettagli progetto**.

1. Trova il **Gruppo** sul lato destro dello schermo e rimuovere il gruppo Predefinito.

1. Nel menu a discesa, individua il gruppo desiderato. I gruppi connessi con Frame.io visualizzano l&#39;icona Frame.io.
   ![](assets/add-frame-group.png)

1. Apporta qualsiasi altra modifica alla configurazione del progetto.

1. Fai clic su **Salva modifiche**.

1. Passare alla sezione successiva.

### Aggiungi un’attività e imposta lo stato di integrazione su Attivo

>[!NOTE]
>
>Le sottoattività non sono attualmente supportate nei progetti Frame.io connessi.


1. Creare le attività da compilare in Frame.io

1. Seleziona le attività necessarie, quindi fai clic su **Modifica**.

1. Scorri fino a **Forms personalizzato** e trovare il modulo di integrazione Frame.io.

   >[!IMPORTANT]
   >
   >Affinché questo modulo venga visualizzato, è necessario assegnare un gruppo Frame.io connesso nell&#39;area Project Details (Dettagli progetto). Per ulteriori informazioni, consulta [Creazione di un progetto Workfront e aggiunta di un gruppo connesso](#create-a-workfront-project-and-add-a-connected-group) in questo articolo.


1. Abilita **Stato di integrazione dell&#39;attività** e scegliere **Attivo**.
   ![](assets/frame-custom-form.png)

1. Clic **Salva modifiche**. Accanto al nome del progetto viene visualizzata l&#39;icona Frame.io.

1. Assegnare utenti o team alle attività.

   >[!NOTE]
   >
   >Gli utenti o i team aggiunti alle attività vengono aggiunti anche al progetto Frame.io.

1. Caricare documenti o descrizioni nella sezione Documenti progetto.

Il progetto non è ancora connesso, devi passare alla sezione successiva per completare l’integrazione.

### Abilitare il progetto in Frame.io

1. Modifica lo stato del progetto da **Pianificazione** a **Corrente** o uno stato personalizzato uguale a corrente. In questo modo viene completata l&#39;integrazione e vengono generati il progetto, le attività ed eventuali documenti in Frame.io.

L’icona Frame.io accanto al nome del progetto diventa viola e segnala il successo dell’integrazione. Gli utenti ricevono un’e-mail per invitarli al progetto Frame.io.

>[!IMPORTANT]
>
>Una volta connesso il progetto per Frame.io, le modifiche apportate al gruppo di progetti non vengono riportate in Frame.io.


