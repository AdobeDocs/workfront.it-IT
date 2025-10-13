---
product-area: projects
navigation-topic: manage-issues
title: Aggiorna automaticamente gli stati dei problemi da In attesa di feedback a In corso
description: Quando il contatto principale di un problema aggiorna il problema aggiornando un campo (incluso un campo personalizzato) o aggiungendo un commento, lo stato del problema viene aggiornato automaticamente in In corso.
author: Alina
feature: Work Management
exl-id: f94bb644-910f-4b46-80fd-fecbdf9cb18a
source-git-commit: 393f858ba3711b367cf06ad846ea60be0d6d9034
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 0%

---

# Aggiorna automaticamente gli stati dei problemi da In attesa di feedback a In corso

<!--Audited: 109/2025-->

Quando il contatto principale di un problema aggiorna il problema aggiornando un campo (incluso un campo personalizzato) o aggiungendo un commento, lo stato del problema viene aggiornato automaticamente in In corso.

Affinché la modifica automatica dello stato avvenga, sono necessari i seguenti elementi:

* Il problema deve essere aggiunto utilizzando una coda di richieste.

  Per informazioni sulla creazione di code di richieste, vedere la sezione [Creare e gestire code di richieste](../../../manage-work/requests/create-and-manage-request-queues/create-manage-request-queues.md).

  Per informazioni sull&#39;invio di richieste a una coda di richieste, vedere [Creare e inviare richieste Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

* I Dettagli coda nella coda richieste devono avere le seguenti impostazioni:
   * **Quando qualcuno effettua una richiesta, concedi automaticamente** è impostato su **Accesso a Contribute**
   * **Modifica stato** è selezionato

  ![I dettagli coda consentono a Contribute di accedere e modificare lo stato selezionato.](assets/queuedetails-contributeaccess-changestatus.png)

  >[!IMPORTANT]
  >
  >  Quando si imposta una coda di richieste, è possibile definire l’accesso dei contatti principali ai problemi inviati.
  >
  >Quando deselezioni l’impostazione Modifica stato durante la configurazione della coda di richieste, ricorda che gli amministratori di sistema hanno sempre accesso per modificare lo stato dei problemi, anche se l’opzione Modifica stato è deselezionata nelle impostazioni della coda di richieste.

  Per ulteriori informazioni sui dettagli della coda, vedere [Creare una coda di richieste](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

* Il problema deve essere nello stato In attesa di feedback.
* È necessario uno stato AWF (Await Feedback) disponibile per i problemi a livello di sistema.

  Per ulteriori informazioni sugli stati a livello di sistema, vedere [Creare o modificare uno stato](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
