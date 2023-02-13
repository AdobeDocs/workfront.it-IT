---
product-area: projects
navigation-topic: manage-issues
title: Aggiorna automaticamente gli stati dei problemi da In attesa del feedback a In corso
description: Quando il contatto primario di un problema effettua un aggiornamento del problema aggiornando un campo (incluso un campo personalizzato) o aggiungendo un commento, lo stato del problema si aggiorna automaticamente a In corso.
author: Alina
feature: Work Management
exl-id: f94bb644-910f-4b46-80fd-fecbdf9cb18a
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 0%

---

# Aggiorna automaticamente gli stati dei problemi da In attesa del feedback a In corso

Quando il contatto primario di un problema effettua un aggiornamento del problema aggiornando un campo (incluso un campo personalizzato) o aggiungendo un commento, lo stato del problema si aggiorna automaticamente a In corso.

Affinché si verifichi questa modifica automatica dello stato, è necessario quanto segue:

* Il problema deve essere immesso tramite una coda di richiesta.

   Per informazioni sulla creazione delle code di richiesta, consulta la sezione [Creare e gestire le code di richieste](../../../manage-work/requests/create-and-manage-request-queues/create-manage-request-queues.md) sezione . Per informazioni sulla creazione delle richieste, vedi [Creare e inviare richieste Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

* I dettagli coda nella coda delle richieste devono avere le seguenti impostazioni:
   * **Quando qualcuno effettua una richiesta, concede automaticamente** è impostato su **Accesso a Contribute**
   * **Cambia stato** è selezionato in Impostazioni avanzate

   ![Dettagli coda consente di selezionare l&#39;opzione Accesso e Modifica stato di Contribute.](assets/queuedetails-contributeaccess-changestatus.png)

   Per ulteriori informazioni sui dettagli della coda, consulta [Creare una coda di richiesta](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

* Il problema deve essere in attesa dello stato Feedback .
* È necessario che sia disponibile uno stato Await Feedback (AWF) per problemi a livello di sistema.

   Per ulteriori informazioni sugli stati a livello di sistema, consulta [Creare o modificare uno stato](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
