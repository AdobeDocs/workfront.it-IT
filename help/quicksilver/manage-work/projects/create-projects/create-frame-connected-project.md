---
product-area: projects
navigation-topic: create-projects
title: Creare un progetto connesso con Frame.io
description: Un progetto è una grande unità di lavoro in Adobe Workfront. Puoi creare progetti da zero, utilizzare un modello o convertire problemi o attività in progetti.
author: Courtney
feature: Work Management
source-git-commit: 089173acb8fecd920ca096c5bf9c6ee61910c20b
workflow-type: tm+mt
source-wordcount: '1158'
ht-degree: 1%

---


# Creare un progetto connesso con Frame.io

L’integrazione Workfront e Frame.io consente di creare progetti in Workfront che si riflettono in Frame.io, fornendo un’esperienza di revisione e approvazione fluida.

Quando un progetto Workfront è connesso con Frame.io, è possibile

* **Assegnare utenti Frame.io alle attività**: gli utenti abilitati Frame.io ricevono una notifica tramite e-mail quando vengono assegnati a un’attività Workfront, segnalando che c’è lavoro da completare.
* **Condividere il progetto con gli utenti di Frame.io**: quando un progetto viene condiviso con utenti abilitati a Frame.io, questi hanno accesso al progetto sia in Workfront che in Frame.io.
* **Condividi materiali creativi con Frame.io**: i coordinatori del progetto possono inviare istruzioni e materiali da Workfront direttamente all’utente creativo in Frame.io utilizzando una cartella di progetto per la sincronizzazione unidirezionale. [!BADGE Disponibile a breve]{type=Informative}
* **Tracciare l’avanzamento dell’attività**: i creativi possono inviare risorse finite e contrassegnare le attività come completate, il tutto senza uscire da Frame.io.

## Requisiti di accesso

>[!IMPORTANT]
>
>Questa funzionalità è disponibile solo per le organizzazioni che sono state caricate in [!DNL Adobe Admin Console].

Devi avere i seguenti:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> <p>Standard</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica accesso ai progetti</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Quando crei un progetto, ricevi automaticamente le autorizzazioni di gestione per il progetto.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Prerequisiti

* Configurare l&#39;account Frame.io predefinito nell&#39;area di configurazione di Workfront
* Abilitare gli utenti Frame.io nel profilo utente di Workfront

Per ulteriori informazioni sui prerequisiti di cui sopra, consulta [Configurare [!DNL Workfront] e [!DNL Frame.io] integrazione](/help/quicksilver/administration-and-setup/configure-integrations/configure-wf-and-frame.md).


## Crea un nuovo modello di progetto

Durante la creazione di un nuovo modello, è possibile immettere le informazioni per tutte le attività e per le impostazioni del progetto future. Queste informazioni verranno quindi trasferite a qualsiasi progetto creato dal modello.

I progetti in Frame.io sono organizzati per team, che sono collegati a gruppi Workfront. È consigliabile utilizzare un modello di progetto per creare progetti connessi, in quanto è possibile impostare il gruppo di progetti prima di.

Se si sceglie di creare il progetto da zero, Workfront aggiunge automaticamente il gruppo di progetto Predefinito e il progetto mirror Frame.io viene creato nel team predefinito in Frame.io.

>[!NOTE]
>
>L’aggiornamento del gruppo dopo la creazione del progetto non modifica il team Frame.io.


### Creare il modello e specificare il gruppo di progetti

{{step1-to-templates}}

1. Clic **Nuovo modello**.
1. Digita un nome per il modello, quindi premi **Invio** per salvare il nome.
1. Nel pannello a sinistra, fai clic su **Dettagli Modello**.
1. In **Associazione modello** , assicurati di specificare un gruppo. Se non aggiungete un gruppo, viene aggiunto il gruppo di progetto predefinito e il progetto in Frame.io viene creato nel team predefinito corrispondente in Frame.io.

Passare alla sezione successiva.

![](assets/template-group.png)

### Aggiungere attività e assegnare utenti abilitati per Frame.io

1. Nel pannello a sinistra, fai clic su **Attività modello**.
1. Clic **Inizia ad aggiungere le attività modello** per aggiungere rapidamente attività al modello. È possibile configurare ulteriori impostazioni in un secondo momento.

   Oppure

   Clic **Crea Attività Modello** per aggiungere un&#39;attività alla volta e configurare altre impostazioni.
   ![](assets/add-tasks-to-template.png)
1. Aggiungi un nome attività.
1. In **Assegnazioni** , assegnare utenti o team. Se assegnate un utente abilitato Frame.io, singolarmente o in un team, gli verrà concesso l&#39;accesso collaboratore al progetto Frame.io e riceverà una notifica tramite e-mail relativa all&#39;attività nel progetto Frame.io. Da tale e-mail, possono partecipare al progetto Frame.io e iniziare a lavorare.
1. Ripetere i passaggi 1 e 2 in base alle esigenze.

Passare alla sezione successiva.

### Configura ulteriori dettagli modello

Workfront dispone di solide funzionalità di gestione dei progetti. È consigliabile utilizzare [Modificare i modelli di progetto](/help/quicksilver/manage-work/projects/create-and-manage-templates/edit-templates.md) articolo per configurare le seguenti aree del modello:

* Panoramica
* Finanz
* Moduli personalizzati
* Impostazione progetto
* Impostazioni attività
* Impostazioni problema
* Accesso

### Creare un progetto dal modello

Dopo aver creato un modello, puoi utilizzarlo per creare progetti.

{{step1-to-projects}}

1. Clic **Nuovo progetto da modello**.
1. Utilizzando la casella di ricerca, inizia a digitare il nome del modello necessario.
1. Seleziona il nome del modello, quindi fai clic su **Usa modello**.
   ![](assets/find-your-template.png)
1. Modifica le impostazioni del progetto in base alle esigenze, quindi fai clic su **Crea progetto**.
1. Nel pannello a sinistra, fai clic su **Documenti**.
1. Utilizzare la cartella di sincronizzazione unidirezionale per condividere automaticamente il materiale creativo con Frame.io. [!BADGE Disponibile a breve]{type=Informative}

   >[!NOTE]
   >
   >Questa funzione è attualmente in fase di sviluppo. Per condividere informazioni con gli utenti in Frame.io, caricate i file nella scheda Documento. Quando lo stato del progetto è impostato su Corrente, questi file vengono inviati automaticamente a Frame.io.

1. Nell’intestazione del progetto, modifica il progetto da **Pianificazione** a **Corrente**.

Dopo la creazione del progetto e il caricamento delle risorse da parte dei creativi, puoi assegnare un flusso di lavoro di revisione e approvazione alla risorsa in Workfront. Per ulteriori informazioni, consulta [Creare una richiesta di revisione o approvazione documento](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md). <!-- name may need to change -->

## Crea un nuovo progetto da zero

Se necessario, puoi creare un nuovo progetto da zero.

>[!IMPORTANT]
>
>* I progetti in Frame.io sono organizzati per team, che sono collegati a gruppi Workfront. È consigliabile utilizzare un modello di progetto per creare progetti connessi, in quanto è possibile impostare il gruppo di progetti prima di.
>
>
>* Se si sceglie di creare il progetto da zero, Workfront aggiunge automaticamente il gruppo di progetto Predefinito e il progetto mirror Frame.io viene creato nel team predefinito in Frame.io.
>
>L’aggiornamento del gruppo dopo la creazione del progetto non modifica il team Frame.io.

### Creare il progetto

{{step1-to-projects}}

1. Clic **Nuovo progetto**.
1. Digita un nome per il progetto, quindi premi **Invio** per salvare il nome.

Passare alla sezione successiva.

### Aggiungere attività e assegnare utenti abilitati per Frame.io

1. Nel pannello a sinistra, fai clic su **Attività**.
1. Clic **Inizia ad aggiungere attività** per aggiungere rapidamente attività al progetto. È possibile configurare ulteriori impostazioni in un secondo momento.

   Oppure

   Clic **Crea Attività** per aggiungere un&#39;attività alla volta e configurare altre impostazioni.
   ![](assets/add-project-tasks.png)
1. Aggiungi un nome attività.
1. In **Assegnazioni** , assegnare utenti o team. Se assegnate un utente abilitato Frame.io, singolarmente o in un team, gli verrà concesso l&#39;accesso collaboratore al progetto Frame.io e riceverà una notifica tramite e-mail relativa all&#39;attività nel progetto Frame.io. Da tale e-mail, possono partecipare al progetto Frame.io e iniziare a lavorare.
1. Ripetere i passaggi 1 e 2 in base alle esigenze.

Passare alla sezione successiva.

### Carica materiali creativi

1. Nel pannello a sinistra, fai clic su **Documenti**.
1. Utilizzare la cartella di sincronizzazione unidirezionale per condividere automaticamente il materiale creativo con Frame.io. [!BADGE Disponibile a breve]{type=Informative}

   >[!NOTE]
   >
   >Questa funzione è attualmente in fase di sviluppo. Per condividere informazioni con gli utenti in Frame.io, caricate i file nella scheda Documento. Quando lo stato del progetto è impostato su Corrente, questi file vengono inviati automaticamente a Frame.io

Passare alla sezione successiva.

### Configura ulteriori dettagli del progetto

Workfront dispone di solide funzionalità di gestione dei progetti. È consigliabile utilizzare [Modifica progetti](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md) articolo per configurare le seguenti aree del progetto:

* Panoramica
* Finanz
* Moduli personalizzati
* Impostazione progetto
* Impostazioni attività
* Impostazioni problema
* Accesso

### Imposta il progetto sulla versione corrente

1. Nell&#39;intestazione del progetto modificare il progetto da Planning a Corrente.
Dopo la creazione del progetto e il caricamento delle risorse da parte dei creativi, puoi assegnare un flusso di lavoro di revisione e approvazione alla risorsa in Workfront.

Dopo la creazione del progetto e il caricamento delle risorse da parte dei creativi, puoi assegnare un flusso di lavoro di revisione e approvazione alla risorsa in Workfront.

Per ulteriori informazioni, consulta [Creare una richiesta di revisione o approvazione documento](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md). <!-- name may need to change -->