---
product-area: documents
navigation-topic: approvals
title: Introduzione all’integrazione Frame.io
description: Introduzione all’integrazione Frame.io.
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: b9a83bc2-4dd8-4c77-a2e7-385baa809b3b
source-git-commit: 8233bcad8409b6f293d365fe871338e643a410dc
workflow-type: tm+mt
source-wordcount: '921'
ht-degree: 0%

---

# Introduzione all’integrazione Frame.io

L&#39;integrazione Workfront e Frame.io assicura l&#39;allineamento di creativi, addetti al marketing e stakeholder con un flusso di lavoro omogeneo. Accedi agli aggiornamenti in tempo reale, evita il lavoro duplicato e assicurati che le risorse siano approvate prima del lancio.

Per ulteriori informazioni su Frame.io, vedere [Guida introduttiva a Frame.io](https://support.frame.io/en/collections/49298-getting-started).

È necessario che nell’istanza di Workfront siano configurate l’integrazione Workfront e Frame.io. Per ulteriori informazioni, vedere [Panoramica dell&#39;integrazione Frame.io](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/frame-int-overview.md#integration-requirements).

## Requisiti di integrazione

* Workfront e Frame.io devono essere distribuiti nella stessa organizzazione Identity Management System (IMS).

* Gli utenti possono appartenere a una sola istanza di Workfront all’interno dell’organizzazione IMS.

* L’istanza di Workfront deve essere abilitata sullo storage aziendale Adobe Unified Experience e Adobe.

* L’integrazione deve essere configurata da Adobe Professional Services.

## Avvio e pianificazione del lavoro in Workfront

I coordinatori dei progetti possono creare progetti e pianificare il lavoro in Workfront. I progetti creati in un’istanza con l’integrazione Frame.io abilitata utilizzano lo storage aziendale Adobe, che consente di archiviare e gestire le risorse all’interno dell’ecosistema Adobe.

Se la tua organizzazione dispone di una licenza Frame.io Enterprise, i progetti creati in Workfront sono visibili anche in Frame.io, consentendo agli utenti di interagire e caricare le risorse in entrambi i prodotti.

Per informazioni su Adobe Enterprise Storage o sui progetti in Frame.io, consulta

* [Panoramica di Workspace: progetti](https://help.frame.io/en/articles/9101001-workspace-overview#h_d9f8654895)
* [Panoramica sullo storage aziendale Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md)

## Rivedere e approvare le risorse

Al termine della risorsa, il coordinatore del progetto può avviare il processo formale di revisione e approvazione in Workfront.

Dopo aver creato il flusso di lavoro di approvazione, i revisori e gli approvatori possono utilizzare il visualizzatore Frame.io per aggiungere commenti e contrassegnare la risorsa. Possono anche prendere la decisione di approvazione nel visualizzatore Frame.io.

Per ulteriori informazioni sulla configurazione dei progetti, consulta

* [Creare un progetto](/help/quicksilver/manage-work/projects/create-projects/create-project.md)
* [Panoramica dell’integrazione Frame.io](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/frame-int-overview.md)

### Avviare revisioni e approvazioni formali in Workfront

I coordinatori dei progetti possono creare modelli di approvazione riutilizzabili o modelli di revisione e approvazione una tantum. Possono assegnare revisori, approvatori o una combinazione di entrambi:

* **I revisori** possono aggiungere commenti e contrassegnare le risorse. Una volta terminata, la recensione può essere contrassegnata come completata. Per far avanzare la risorsa nel processo di approvazione, non è necessario contrassegnare la revisione come completata.
* **Gli approvatori** possono aggiungere commenti e contrassegnare le risorse. Devono prendere la decisione di portare avanti il processo di approvazione.

#### Creare un flusso di lavoro di revisione e approvazione

Revisori e approvatori possono essere aggiunti a un flusso di lavoro di approvazione a utente singolo o a un modello di approvazione riutilizzabile:

* **Approvazioni per singolo utilizzo**: nel progetto o nell&#39;attività in cui risiede la risorsa, il coordinatore del progetto può assegnare revisori e approvatori e impostare una scadenza di completamento. Ai revisori e agli approvatori viene inviato un promemoria tramite e-mail 72 ore prima della scadenza, 24 ore prima della scadenza e quindi sulla scadenza stessa.

  Per ulteriori informazioni, vedere [Creare una richiesta di revisione o approvazione del documento](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

* **Modelli di approvazione**: nell&#39;area Configurazione di Workfront i coordinatori del progetto possono creare modelli di approvazione riutilizzabili. All’interno di un modello, gli utenti possono aggiungere revisori e approvatori e specificare un arco temporale di completamento. Quando il modello di approvazione viene applicato a una risorsa, la scadenza viene calcolata a partire dall’intervallo di tempo specificato.

  Una volta creato, un modello può essere applicato a una risorsa per iniziare il processo formale di revisione e approvazione in Workfront.

  Per ulteriori informazioni, vedere [Creare un modello di approvazione](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).


  ![Assegna modello](assets/assign-template.png)

### Rivedere e approvare le risorse nel visualizzatore Frame.io

Una volta avviato il flusso di lavoro di revisione e approvazione in Workfront, i revisori e gli approvatori possono accedere al visualizzatore Frame.io per aggiungere commenti, contrassegnare la risorsa e prendere una decisione.

Per ulteriori informazioni, vedere [Rivedere e approvare con il visualizzatore Frame.io](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/review-with-frame.md).

#### Accedere al visualizzatore Frame.io

Gli utenti possono accedere al visualizzatore Frame.io nei modi seguenti:

* Notifiche e-mail Workfront
* Il widget Approvazione personale nell’area Home di Workfront

>[!NOTE]
>
>Gli utenti esterni di Workfront ricevono una notifica tramite e-mail e viene richiesto di creare un accesso Frame.io per rivedere e approvare le risorse.

![apri il visualizzatore di frame dalla Home](assets/open-fio-viewwer.png)

#### Aggiungere commenti e contrassegnare le risorse

Nel visualizzatore Frame.io sono visibili commenti e markup di risorsa. Per ulteriori informazioni sull&#39;utilizzo del visualizzatore Frame.io, vedere [Commenti sul supporto](https://help.frame.io/en/articles/9105251-commenting-on-your-media).

#### Prendi una decisione

Una volta completata l&#39;attività di revisione, gli approvatori devono prendere una delle seguenti decisioni:

* **Approva**: la risorsa non necessita di modifiche ed è pronta per l&#39;uso.
* **Lavoro necessario**: la risorsa richiede modifiche e non è pronta per l&#39;uso. Una volta apportate le modifiche specificate, la risorsa deve essere caricata come nuova versione e passare attraverso un altro ciclo di approvazioni. <!--is the same approval workflow automatically applied? Does the coordinator have to do anything to get the approval going? -->

I revisori possono contrassegnare la revisione come completata all’interno di Workfront, ma questo non è necessario per far avanzare la risorsa nel processo di approvazione.

Per ulteriori informazioni sulle decisioni in Workfront, consulta [Panoramica sullo stato delle decisioni](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/document-approval-status.md).

![Visualizzatore frame e decisione](assets/decision-fio.png)


### Tracciare le metriche di revisione e approvazione

I coordinatori dei progetti possono monitorare lo stato di avanzamento di tutte le approvazioni in volo nell’area Home di Workfront o con rapporti personalizzati nei dashboard di Canvas:

* **Dashboard personalizzato**: crea un dashboard di report nell&#39;area Dashboard Canvas per visualizzare informazioni dettagliate e di alto livello su revisioni e approvazioni con funzionalità Unified Approvals. Per informazioni su come iniziare, vedere [Creare un dashboard di report per la revisione e le approvazioni](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md).
* **Widget Home delle metriche di approvazione del documento**: visualizza 2 grafici con informazioni sul tempo medio di approvazione e sulle decisioni, nonché visualizzazioni elenco delle approvazioni in sospeso e in ritardo.
  ![Tutte le approvazioni](assets/all-approvals.png)

## Inviare risorse finite a Adobe Experience Manager

È possibile utilizzare [!DNL Experience Manager Assets]&#x200B;&#x200B; per gestire e archiviare le risorse digitali che hanno superato il ciclo di revisione e approvazione. Questa integrazione consente di sfruttare le funzionalità di Adobe Experience Manager, Frame.io e Workfront per semplificare la gestione dei contenuti e i processi di collaborazione.

Per ulteriori informazioni, vedere [Utilizzare Adobe Experience Manager con l&#39;integrazione Frame.io](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/use-aem-with-frame.md).