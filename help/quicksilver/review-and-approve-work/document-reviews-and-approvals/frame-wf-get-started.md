---
product-area: documents
navigation-topic: approvals
title: Introduzione alla revisione e all’approvazione delle risorse con Frame.io
description: Ulteriori informazioni sul processo di revisione e approvazione formale nell’utilizzo di Workfront e Frame.io.
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
hide: true
hidefromtoc: true
exl-id: 68b91aad-af76-473f-861d-da846fdfb84c
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '1165'
ht-degree: 0%

---

# Introduzione alla revisione e all’approvazione delle risorse con Frame.io

Il nuovo flusso di lavoro di revisione e approvazione delle risorse è basato su una stretta integrazione tra Workfront e Frame.io. Questa integrazione prende il meglio di ciò che ogni prodotto ha da offrire e li combina per creare un’esperienza che consenta a tutti coloro che sono coinvolti nella creazione di contenuti di lavorare nei loro strumenti, avendo accesso a commenti, file e aggiornamenti di stato, il tutto sincronizzato in tempo reale tra i due sistemi.

Per ulteriori informazioni su Frame.io, vedere [Guida introduttiva a Frame.io](https://support.frame.io/en/collections/49298-getting-started).

## Avvio e pianificazione del lavoro in Workfront

L&#39;amministratore di Workfront abilita l&#39;integrazione tra Workfront e Frame.io configurando l&#39;account predefinito Frame.io nell&#39;area Setup e quindi designando gli utenti Frame.io in Workfront. Questo consente al coordinatore di pianificare e avviare il lavoro utilizzando i progetti Workfront e i flussi di lavoro di revisione e approvazione formali.

### Configura l&#39;account Frame.io predefinito [!BADGE Disponibile a breve]{type=Informative}

Gli amministratori di Workfront avviano l’integrazione di Workfront e Frame.io aggiungendo un account Frame.io predefinito nell’area Setup di Workfront. Una volta configurato l&#39;account Frame.io predefinito, tutti i progetti creati in Workfront avranno un progetto mirror creato in Frame.io.

>[!IMPORTANT]
>
>Questa funzione sarà presto disponibile. Per il momento, gli account Frame.io vengono aggiunti manualmente dal team Workfront. Per assistenza, contatta il rappresentante del tuo account Adobe.

<!--For more information, see [Configure the [!DNL Workfront] and [!DNL Frame.io] integration](/help/quicksilver/administration-and-setup/configure-integrations/configure-wf-and-frame.md).

 in procedure article we need to cover how groups work with projects and how the frame account is associated with a group. And that accounts other than the default can be added on a 1:1 basis using the dev token. -->

### Abilita utenti Frame.io disponibili ora

Gli utenti Workfront che utilizzano regolarmente Frame.io devono essere contrassegnati come utenti Frame.io. Gli amministratori di Workfront possono designare gli utenti Frame.io nel profilo utente di Workfront.

>[!TIP]
>
>Consigliamo di abilitare gli utenti che lavorano regolarmente in strumenti creativi e caricano risorse da rivedere e approvare come utenti Frame.io.

Quando un utente viene contrassegnato come utente Frame.io in Workfront e viene aggiunto a un progetto:

* Vengono aggiunti come collaboratori in Frame.io.
* Possono inviare le risorse da Frame.io a Workfront per la revisione e l’approvazione formali.
* Possono visualizzare informazioni nella cartella di sincronizzazione unidirezionale da Workfront. [!BADGE In arrivo]{type=Informative}

Per ulteriori informazioni, vedere [Configurare l&#39;integrazione [!DNL Workfront] e [!DNL Frame.io] ](/help/quicksilver/administration-and-setup/configure-integrations/configure-wf-and-frame.md).

![Utente con frame abilitato](assets/Frame-enabled-user.png)


### Creare un progetto connesso con Frame.io

Una volta aggiunto l&#39;account Frame.io predefinito e designati gli utenti Frame.io, i coordinatori del progetto possono creare progetti Workfront collegati con Frame.io. Quando si crea un progetto connesso, è possibile

* **Assegna utenti Frame.io alle attività**: gli utenti abilitati Frame.io ricevono una notifica tramite e-mail quando vengono assegnati a un&#39;attività Workfront, segnalando che il lavoro è da completare.
* **Condividi il progetto con gli utenti Frame.io**: quando un progetto viene condiviso con utenti abilitati per Frame.io, questi hanno accesso al progetto sia in Workfront che in Frame.io.
* **Condividi materiali creativi con Frame.io**: i coordinatori del progetto possono inviare istruzioni e materiali da Workfront direttamente all&#39;utente creativo in Frame.io utilizzando una cartella di progetto di sincronizzazione unidirezionale. [!BADGE In arrivo]{type=Informative}
* **Traccia l&#39;avanzamento dell&#39;attività**: i creativi possono inviare le risorse finite e contrassegnare le attività come completate, il tutto senza uscire da Frame.io.

Per ulteriori informazioni, vedere [Creare un progetto connesso con Frame.io](/help/quicksilver/manage-work/projects/create-projects/create-frame-connected-project.md).


## Creazione di contenuti e collaborazione in Frame.io

I creativi possono rimanere nei loro strumenti di scelta e avere la libertà di creare, iterare e condurre revisioni tra pari all&#39;interno di Frame.io.

Quando un contenuto creativo viene aggiunto a un progetto connesso, è possibile effettuare le seguenti operazioni in Frame.io:

<!--* Access instructions from the project coordinator -->
* Condurre verifiche informali tra pari
* Inviare risorse finite a Workfront per la revisione e l’approvazione formali
* Modificare lo stato di un&#39;attività o contrassegnarla come completata
* Carica nuove versioni e inviale di nuovo per l&#39;approvazione <!--do they have to send to frame.io again?-->

Per ulteriori informazioni su Frame.io, vedere [Sono stato invitato a collaborare a un progetto](https://support.frame.io/en/articles/11125-i-ve-been-invited-to-collaborate-on-a-project).

## Rivedere e approvare le risorse

Una volta che un creativo invia una risorsa completata a Workfront da Frame.io, il coordinatore del progetto può avviare il processo formale di revisione e approvazione in Workfront.

Dopo aver creato il flusso di lavoro di approvazione, i revisori e gli approvatori tornano a Frame.io per aggiungere commenti e contrassegnare la risorsa. Possono anche prendere la decisione di approvazione nel visualizzatore Frame.io.

### Avviare revisioni e approvazioni formali in Workfront

I coordinatori dei progetti possono creare modelli di approvazione riutilizzabili o modelli di revisione e approvazione una tantum. Tutte le attività di revisione e approvazione in Frame.io vengono registrate anche in Workfront.

I coordinatori dei progetti hanno la possibilità di assegnare revisori, approvatori o una combinazione di entrambi:

* **I revisori** possono aggiungere commenti e contrassegnare le risorse. Una volta terminata, la recensione può essere contrassegnata come completata. Per far avanzare la risorsa nel processo di approvazione, non è necessario contrassegnare la revisione come completata.
* **Gli approvatori** possono aggiungere commenti e contrassegnare le risorse. Devono prendere la decisione di portare avanti il processo di approvazione.


#### Creare un flusso di lavoro di revisione e approvazione

Revisori e approvatori possono essere aggiunti a un flusso di lavoro di approvazione a utente singolo o a un modello di approvazione riutilizzabile:

* **Approvazioni per singolo utilizzo**: nel progetto o nell&#39;attività in cui risiede la risorsa, il coordinatore del progetto può assegnare revisori e approvatori e impostare una scadenza di completamento. Ai revisori e agli approvatori viene inviato un promemoria tramite e-mail 72 e 24 ore prima della scadenza, oltre che sulla scadenza stessa.

  Per ulteriori informazioni, consulta * [Creare una richiesta di revisione o approvazione per una risorsa Frame.io](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-request-for-frame-asset.md).

* **Modelli di approvazione**: nell&#39;area Configurazione di Workfront i coordinatori del progetto possono creare modelli di approvazione riutilizzabili. All’interno di un modello, gli utenti possono aggiungere revisori e approvatori e specificare un arco temporale di completamento. Quando il modello di approvazione viene applicato a una risorsa, la scadenza viene calcolata a partire dall’intervallo di tempo specificato.

  Una volta creato, un modello può essere applicato alle risorse inviate da Frame.io per avviare il processo formale di revisione e approvazione in Workfront.

  Per ulteriori informazioni, vedere [Creare un modello di approvazione](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)


![Assegna modello](assets/assign-template.png)


#### Accedere al visualizzatore Frame.io

Gli utenti possono accedere al visualizzatore Frame.io nei modi seguenti:

* Notifiche e-mail Workfront
* Il widget Approvazione personale nella nuova area Home di Workfront
  ![In attesa della mia approvazione](assets/awaiting-my-approval.png)

>[!NOTE]
>
>Gli utenti esterni di Workfront ricevono una notifica tramite e-mail e viene richiesto di creare un accesso Frame.io per rivedere e approvare le risorse.

#### Aggiungere commenti e contrassegnare le risorse

Tutti i commenti aggiunti nel visualizzatore Frame.io vengono registrati anche nella scheda Aggiornamenti di Workfront. Le risposte effettuate in Workfront non vengono visualizzate in Frame.io. I commenti contrassegnati come &quot;Solo team&quot; nel visualizzatore Frame.io non verranno visualizzati nella scheda Aggiornamenti di Workfront.

#### Prendi una decisione

Una volta completata l&#39;attività di revisione, gli approvatori devono prendere una delle seguenti decisioni:

* **Approva**: la risorsa non necessita di modifiche ed è pronta per l&#39;uso.
* **Approva con modifiche**: la risorsa richiede modifiche ed è pronta per l&#39;uso una volta apportate. Non è necessaria un&#39;ulteriore approvazione.
* **Lavoro necessario**: la risorsa richiede modifiche e non è pronta per l&#39;uso. Una volta apportate le modifiche specificate, la risorsa deve essere caricata come nuova versione e passare attraverso un altro ciclo di approvazioni. <!--is the same approval workflow automatically applied? Does the coordinator have to do anything to get the approval going? -->

I revisori possono contrassegnare la revisione come completata all&#39;interno del visualizzatore Frame.io, ma questo non è necessario per far avanzare la risorsa nel processo di approvazione.

Per ulteriori informazioni sulle decisioni in Workfront, consulta [Panoramica sullo stato delle decisioni](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/document-approval-status.md).

![Visualizzatore frame e decisione](assets/frame-viewer-and-decision.png)


<!-- upload assets directly to workfront to be reviewed in Frame.io/ Will have to send manually at first

Reviewer/approver needs to go through email to get to frame vier
-->

### Tracciare le metriche di revisione e approvazione

I coordinatori dei progetti possono monitorare lo stato di avanzamento di tutte le approvazioni in volo nell’area Home di Workfront con il seguente widget:

* **Tutte le approvazioni**: visualizza 2 grafici con informazioni sul tempo medio di approvazione e sulle decisioni, nonché visualizzazioni elenco delle approvazioni in sospeso e in ritardo.
  ![Tutte le approvazioni](assets/all-approvals.png)
