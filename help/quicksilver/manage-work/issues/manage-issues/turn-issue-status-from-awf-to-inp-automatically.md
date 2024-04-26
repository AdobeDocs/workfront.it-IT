---
product-area: projects
navigation-topic: manage-issues
title: Aggiorna automaticamente gli stati dei problemi da In attesa di feedback a In corso
description: Quando il contatto principale di un problema aggiorna il problema aggiornando un campo (incluso un campo personalizzato) o aggiungendo un commento, lo stato del problema viene aggiornato automaticamente in In corso.
author: Alina
feature: Work Management
exl-id: f94bb644-910f-4b46-80fd-fecbdf9cb18a
source-git-commit: 948cd81908df3174eb985d1c65533077d3ef5d49
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 0%

---

# Aggiorna automaticamente gli stati dei problemi da In attesa di feedback a In corso

Quando il contatto principale di un problema aggiorna il problema aggiornando un campo (incluso un campo personalizzato) o aggiungendo un commento, lo stato del problema viene aggiornato automaticamente in In corso.

Affinché la modifica automatica dello stato avvenga, è necessario quanto segue:

* Il problema deve essere immesso tramite una coda di richieste.

  Per informazioni sulla creazione di code di richieste, vedere [Creare e gestire le code di richieste](../../../manage-work/requests/create-and-manage-request-queues/create-manage-request-queues.md) sezione. Per informazioni sulla creazione delle richieste, consulta [Creare e inviare richieste Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

* I Dettagli coda nella coda richieste devono avere le seguenti impostazioni:
   * **Quando qualcuno effettua una richiesta, concedi automaticamente** è impostato su **Contribuisci accesso**
   * **Modifica stato** è selezionato in Impostazioni avanzate

  ![I dettagli coda consentono l&#39;accesso a Contribute e l&#39;opzione Modifica stato è selezionata.](assets/queuedetails-contributeaccess-changestatus.png)

  >[!IMPORTANT]
  >
  >  Quando si imposta una coda di richieste, è possibile definire l’accesso dei contatti principali ai problemi inviati.
  >
  >Quando deselezioni l’impostazione Modifica stato durante la configurazione della coda di richieste, ricorda che gli amministratori di sistema hanno sempre accesso per modificare lo stato dei problemi, anche se l’opzione Modifica stato è deselezionata nelle impostazioni della coda di richieste.

  Per ulteriori informazioni sui dettagli della coda, vedere [Creare una coda di richieste](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

* Il problema deve essere nello stato In attesa di feedback.
* È necessario uno stato AWF (Await Feedback) disponibile per i problemi a livello di sistema.

  Per ulteriori informazioni sugli stati a livello di sistema, consulta [Creare o modificare uno stato](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
