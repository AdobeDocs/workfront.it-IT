---
product-area: projects;user-management
navigation-topic: manage-projects
title: Rimuovi utenti dai progetti
description: Puoi rimuovere utenti da un progetto quando non sono più coinvolti nel completamento del lavoro sul progetto.
author: Alina
feature: Work Management
exl-id: 3a75c78d-faed-41cd-a0a4-59504bb981af
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# Rimuovere utenti dai progetti

Puoi rimuovere utenti da un progetto quando non sono più coinvolti nel completamento del lavoro sul progetto. La rimozione degli utenti dai progetti ha implicazioni sulle assegnazioni di attività e problemi, nonché sui ruoli di progetto. Gli utenti rimossi smettono di ricevere le notifiche destinate al team di progetto. Per ulteriori informazioni sulle notifiche per i team di progetto, vedere [Tipi di notifica eventi](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Gli utenti associati a un progetto sono elencati nell’area Persone di un progetto. Rappresenta il team del progetto. Per ulteriori informazioni sul team di progetto, vedere [Panoramica team di progetto](../../../manage-work/projects/planning-a-project/project-team-overview.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> <p>Standard</p> 
   <p>Piano</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica accesso ai progetti</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni sul progetto</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions on the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Effetti della rimozione su attività, problemi e progetti esistenti

Quando un utente viene rimosso da un progetto, possono essere interessati tutti i problemi o le attività ad esso assegnati, a seconda che l’attività o il problema sia stato completato al momento della rimozione dell’utente:

* **Se l&#39;elemento non è stato completato quando l&#39;utente viene rimosso:** L&#39;elemento viene riassegnato a una mansione se una mansione è già stata assegnata o è assegnato alla mansione che l&#39;utente stava svolgendo sull&#39;elemento. Se all&#39;elemento o all&#39;utente non è stata assegnata una mansione, è necessario riassegnare manualmente l&#39;elemento.
* **Se l&#39;elemento viene completato quando l&#39;utente viene rimosso:** Il nome dell&#39;utente rimosso rimane nell&#39;elemento.
* **Se l&#39;utente ha rimosso è anche il creatore di un progetto:** Il progetto non viene rimosso dall&#39;elenco **Progetti ai quali sono assegnato** nell&#39;area Progetti. Il progetto viene rimosso dagli elenchi di tutti gli altri utenti che filtrano il progetto in base al campo Inserito da.
* **Se l&#39;utente è il proprietario del progetto o lo sponsor:** L&#39;utente rimane nel suo ruolo di sponsor o proprietario del progetto.

## Rimuovere utenti da un progetto e Team di progetto

È possibile rimuovere utenti da un progetto rimuovendoli dalla squadra del progetto.

Quando gli utenti svolgono i ruoli in un progetto, diventano parte del Team di progetto.

Quando rimuovi gli utenti dai loro ruoli sul progetto, questi rimangono parte del team del progetto.

Per informazioni sui ruoli degli utenti in un progetto, vedere [Gestione del team di progetto](../planning-a-project/manage-project-team.md).

Per rimuovere utenti dalla squadra del progetto:

1. Vai al progetto in cui desideri rimuovere gli utenti.

1. Fai clic su **Persone** nel pannello a sinistra, quindi seleziona gli utenti da rimuovere.

1. Fai clic sull&#39;icona **Rimuovi** ![Rimuovi elemento](assets/remove-icon---x-in-circle.png) nella parte superiore dell&#39;elenco degli utenti.

1. Fare clic su **Sì, Rimuovi utenti selezionati** per confermare la rimozione.

   Gli utenti vengono rimossi dal team del progetto e da tutte le attività o i problemi incompleti a cui potrebbero essere assegnati. Non ricevono più le notifiche destinate al team di progetto.
