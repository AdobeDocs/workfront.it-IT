---
product-area: documents
navigation-topic: approvals
title: Panoramica sulla revisione e sull’approvazione delle risorse
description: Ulteriori informazioni sul processo di revisione e approvazione formale in Workfront.
author: Courtney
feature: Work Management, Digital Content and Documents
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
exl-id: 68b91aad-af76-473f-861d-da846fdfb84c
source-git-commit: 959bd3cab0de8b76c94fad1be5b6b2b8b7ae904b
workflow-type: tm+mt
source-wordcount: '908'
ht-degree: 0%

---

# Panoramica sulla revisione e sull’approvazione delle risorse

Il nuovo flusso di lavoro di revisione e approvazione delle risorse si basa su una stretta integrazione tra Workfront e Frame.io. Questa integrazione prende il meglio di ciò che ogni prodotto ha da offrire e lo combina per creare un’esperienza che consenta a tutti gli utenti coinvolti nella creazione di contenuti di lavorare nei loro strumenti preferiti, avendo accesso a commenti, file e aggiornamenti di stato sincronizzati in tempo reale tra i due sistemi.

Per ulteriori informazioni su Frame.io, consultate [Guida introduttiva a Frame.io](https://support.frame.io/en/collections/49298-getting-started).

## Avvio e pianificazione del lavoro in Workfront

L&#39;amministratore di Workfront abilita l&#39;integrazione tra Workfront e Frame.io configurando l&#39;account predefinito Frame.io nell&#39;area Setup e quindi designando gli utenti Frame.io in Workfront. Questo consente al coordinatore di pianificare e avviare il lavoro utilizzando i progetti Workfront e i flussi di lavoro di revisione e approvazione formali.

### Configurare un account Frame.io predefinito

Gli amministratori di Workfront avviano l’integrazione di Workfront e Frame.io aggiungendo un account Frame.io predefinito nell’area Setup di Workfront. Una volta configurato l&#39;account Frame.io predefinito, tutti i progetti creati in Workfront avranno un progetto mirror creato in Frame.io.

Per ulteriori informazioni, consulta [].

<!-- in procedure article we need to cover how groups work with projects and how the frame account is associated with a group. And that accounts other than the default can be added on a 1:1 basis using the dev token. -->

### Abilita utenti Frame.io

Gli utenti Workfront che utilizzano regolarmente Frame.io devono essere contrassegnati come utenti Frame.io. Gli amministratori di Workfront possono designare gli utenti Frame.io nel profilo utente di Workfront.

Quando un utente viene contrassegnato come utente Frame.io in Workfront e viene aggiunto a un progetto,

* Vengono aggiunti come collaboratori in Frame.io
* Possono inviare le risorse da Frame.io a Workfront per la revisione e l’approvazione formali
* Possono visualizzare informazioni nella cartella di sincronizzazione unidirezionale da Workfront

>[!TIP]
>
>Consigliamo di abilitare gli utenti che lavorano regolarmente in strumenti creativi e caricano risorse da rivedere e approvare come utenti Frame.io.

Per ulteriori informazioni, consulta [].

![](assets/Frame-enabled-user.png)


### Creare un progetto connesso con Frame.io

Una volta aggiunto l&#39;account Frame.io predefinito e designati gli utenti Frame.io, i coordinatori del progetto possono creare progetti Workfront collegati con Frame.io. Quando si crea un progetto connesso, è possibile

* **Assegnare utenti Frame.io alle attività**: gli utenti abilitati Frame.io ricevono una notifica tramite e-mail quando vengono assegnati a un’attività, segnalando che c’è del lavoro da completare.
* **Condividere il progetto con gli utenti di Frame.io**: i progetti condivisi con gli utenti abilitati Frame.io consentono loro di accedere al progetto all’interno di Frame.io.
* **Condividi materiali creativi con Frame.io**: puoi inviare istruzioni e materiali da Workfront direttamente all’utente creativo in Frame.io utilizzando una cartella di progetto per la sincronizzazione unidirezionale.
* **Tracciare l’avanzamento dell’attività**: i creativi possono inviare risorse finite e contrassegnare le attività come completate senza uscire da Frame.io.

Per ulteriori informazioni, consulta [].

<!--Preassign approval templates to tasks coming in the future-->


## Creazione di contenuti e collaborazione in Frame.io

I creativi possono rimanere nei loro strumenti di scelta e avere la libertà di creare, iterare e condurre revisioni tra pari all&#39;interno di Frame.io.

Quando un contenuto creativo viene aggiunto a un progetto connesso, è possibile eseguire le operazioni seguenti senza uscire da Frame.io:

* Istruzioni di accesso dal coordinatore del progetto
* Condurre verifiche informali tra pari
* Inviare risorse finite a Workfront per la revisione e l’approvazione formali
* Modificare lo stato di un&#39;attività o contrassegnarla come completata
<!-- * Notification of decision
* Upload new versions of connected assets marked as needs more work < will automatically connect>-->

Per ulteriori informazioni sulla revisione delle risorse in Frame.io, consulta

## Rivedere e approvare le risorse

Una volta che un creativo invia una risorsa completata a Workfront da Frame.io, il coordinatore del progetto può avviare il processo formale di revisione e approvazione in Workfront.

Dopo aver creato l’approvazione, gli utenti tornano a Frame.io per aggiungere commenti e contrassegnare la risorsa. Possono anche prendere una decisione di approvazione nel visualizzatore Frame.io.

### Avviare revisioni e approvazioni formali in Workfront

I coordinatori dei progetti possono creare modelli di approvazione riutilizzabili e modelli di revisione una tantum nell&#39;area Configurazione di Workfront. Tutte le attività di revisione e approvazione effettuate in Frame.io vengono registrate anche in Workfront.

#### Aggiungi revisori e approvatori

I coordinatori dei progetti hanno la possibilità di assegnare revisori, approvatori o una combinazione di entrambi:

* **Revisori** può aggiungere commenti e contrassegnare le risorse. Una volta terminata, la recensione può essere contrassegnata come completata. <!--example of when to add reviewers-->
* **Approvatori** può aggiungere commenti e contrassegnare le risorse. Devono prendere la decisione di portare avanti il processo di approvazione.


#### Creare un flusso di lavoro di revisione e approvazione

Revisori e approvatori possono essere aggiunti a un flusso di lavoro di approvazione a utilizzo singolo o a un modello di approvazione:

<!--can also assign teams and set deadline-->
E-mail - e-mail con scadenza 72, 24 e in scadenza.

* **Approvazioni per singolo utilizzo**: imposta le scadenze di approvazione

* **Modelli di approvazione**
Nell’area Configurazione di Workfront, gli utenti con una licenza Standard possono creare modelli di approvazione riutilizzabili. All’interno di un modello, gli utenti possono specificare un intervallo di tempo e aggiungere revisori e approvatori. <!--do we want to mention any upcoming plans here? -->

  Una volta creato, un modello può essere applicato alle risorse inviate da Frame.io per avviare il processo formale di revisione e approvazione in Workfront.
  ![](assets/assign-template.png)

<!-- can set timreframe which calculates deadline once approval is started. >

    For more information, see [Create and manage Approval Templates](/)<!--don't forget link-->

* Caricare una risorsa da Workfront e inviarla al frame per la revisione e l&#39;approvazione - Disponibile a breve?

### Approvare le risorse in Frame.io

Le parti interessate possono rivedere e approvare le risorse collegate con il visualizzatore Frame.io.

#### Accedere al visualizzatore Frame.io

Gli utenti possono accedere al visualizzatore Frame.io nei modi seguenti:

* Il widget In attesa della mia approvazione nella nuova Home di Workfront
* Notifiche e-mail di Workfront.

Agli utenti esterni di Workfront verrà richiesto di creare un accesso Frame.io per rivedere e approvare le risorse.

#### Commenta e contrassegna risorse

Tutti i commenti aggiunti nel visualizzatore Frame.io vengono registrati anche nella scheda Workfront Update. Le risposte effettuate in Workfront non vengono visualizzate in Frame.io. I commenti contrassegnati Solo team non verranno visualizzati nella scheda Aggiornamenti di Workfront.

#### Prendi una decisione

Gli approvatori devono prendere una delle seguenti decisioni:

* Approva: questo
* Approva con modifiche
* Azioni da intraprendere

I revisori possono contrassegnare la loro revisione come completata all&#39;interno dei visualizzatori Frame.io.

<!-- include screenshot from frame.io-->



<!-- upload assets directly to workfront to be reviewed in Frame.io/ Will have to send manually at first

Reviewer/approver needs to go through email to get to frame vier
-->


### Tracciare le metriche di revisione e approvazione

Widget nel report sulla velocità di approvazione dell&#39;abitazione?

<!--
### Published approved assets to Adobe Experience Manager Assets

Use the native integration to send approved assets to AEM.
-->


## Esempio di flusso di lavoro per l’approvazione delle risorse della campagna

intro para?

![](assets/example-workflow.png) <!-- probbly need a different version of this but add something similar rather than typing all out?-->
