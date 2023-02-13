---
product-area: projects;user-management
navigation-topic: manage-projects
title: Rimuovere utenti dai progetti
description: Puoi rimuovere gli utenti da un progetto quando non sono più coinvolti nel completamento del lavoro sul progetto.
author: Alina
feature: Work Management
exl-id: 3a75c78d-faed-41cd-a0a4-59504bb981af
source-git-commit: 301c86152340a184345bd39cec77fdcf28258196
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 0%

---

# Rimuovere utenti dai progetti

Puoi rimuovere gli utenti da un progetto quando non sono più coinvolti nel completamento del lavoro sul progetto. La rimozione degli utenti dai progetti ha implicazioni sulle assegnazioni di attività e problemi, nonché sui ruoli di progetto. Gli utenti rimossi cessano di ricevere le notifiche destinate al team di progetto. Per ulteriori informazioni sulle notifiche per i team di progetto, vedi [Notifiche di eventi disponibili in Adobe Workfront](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Gli utenti associati a un progetto sono elencati nell’area Persone di un progetto. Rappresentano il team di progetto. Per ulteriori informazioni sul team di progetto, consulta [Panoramica del team di progetto](../../../manage-work/projects/planning-a-project/project-team-overview.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica accesso a progetti</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestisci le autorizzazioni per il progetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per sapere quale piano, tipo di licenza o accesso si dispone, contattare l&#39;amministratore Workfront.

## Come la rimozione di un utente influisce su attività, problemi e progetti esistenti

Quando un utente viene rimosso da un progetto, le attività o i problemi ad esso assegnati potrebbero essere influenzati, a seconda che l&#39;attività o il problema sia stato completato al momento della rimozione dell&#39;utente:

* **Se l’elemento non viene completato quando l’utente viene rimosso:** L&#39;elemento viene riassegnato a un ruolo di lavoro se un ruolo di lavoro è già stato assegnato oppure viene assegnato al ruolo di lavoro che l&#39;utente stava svolgendo sull&#39;elemento. Se all&#39;elemento o all&#39;utente non è stato assegnato un ruolo, è necessario riassegnare manualmente l&#39;elemento.
* **Se l’elemento viene completato quando l’utente viene rimosso:** Il nome dell&#39;utente rimosso rimane sull&#39;elemento.
* **Se l’utente rimosso è anche il creatore di un progetto:** Il progetto non viene rimosso dalle **Progetti in corso** nell’area Progetti . Il progetto viene rimosso dagli elenchi per tutti gli altri utenti che filtrano il progetto in base al campo Inserito da .
* **Se l’utente è il proprietario o sponsor del progetto:** L’utente rimane nel suo ruolo di sponsor o proprietario del progetto.

## Rimuovere utenti da un progetto e dal team di progetto

Puoi rimuovere gli utenti da un progetto rimuovendoli dal team del progetto.

Quando gli utenti svolgono ruoli in un progetto, diventano parte del team di progetto.

Quando rimuovi gli utenti dai loro ruoli nel progetto, rimangono parte del team del progetto.

Per informazioni sui ruoli degli utenti in un progetto, consulta [Gestione del team del progetto](../planning-a-project/manage-project-team.md).

Per rimuovere gli utenti dal team del progetto:

1. Passa al progetto in cui desideri rimuovere gli utenti.

1. Fai clic su **Persone** nel pannello a sinistra, seleziona gli utenti da rimuovere. Potrebbe essere necessario fare clic su **Mostra altro**, quindi **Persone**.

1. Fai clic sul pulsante **Rimuovi** icona  ![Rimuovi elemento](assets/remove-icon---x-in-circle.png) nella parte superiore dell’elenco degli utenti.

1. Fai clic su **Sì, Rimuovi utenti selezionati** per confermare la rimozione.

   Gli utenti vengono rimossi dal team del progetto e da eventuali attività o problemi incompleti a cui potrebbero essere assegnati. Non ricevono più le notifiche destinate al team di progetto.
