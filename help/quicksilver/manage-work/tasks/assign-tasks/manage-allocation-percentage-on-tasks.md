---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Gestisci la percentuale di allocazione di utenti o ruoli sulle attività
description: La percentuale di allocazione rappresenta il tempo in cui una risorsa assegnata è pianificata per lavorare su un'attività in un giorno. È la percentuale di un giorno lavorativo (in base alla pianificazione dell'utente o del progetto) in cui una risorsa viene allocata per tutta la durata dell'attività.
author: Alina
feature: Work Management
exl-id: 82238dff-b95e-42e4-8e72-6247934b504d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '484'
ht-degree: 1%

---

# Gestisci la percentuale di allocazione di utenti o ruoli sulle attività

La percentuale di allocazione rappresenta il tempo in cui una risorsa assegnata è pianificata per lavorare su un&#39;attività in un giorno. È la percentuale di un giorno lavorativo (in base alla pianificazione dell&#39;utente o del progetto) in cui una risorsa viene allocata per tutta la durata dell&#39;attività.

>[!NOTE]
>
>Quando si assegnano gli utenti al lavoro, la loro disponibilità in base alle loro pianificazioni influisce sulle date previste e previste delle attività e dei problemi. Per informazioni sulle pianificazioni, consulta [Creare una pianificazione](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

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
   <td> <p>Lavoro o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica accesso alle attività</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Collaborare o autorizzazioni superiori per l'attività</p> <p>Modificare le autorizzazioni per aggiornare la percentuale di allocazione nella casella Modifica attività</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Considerazioni sulla modifica delle allocazioni percentuali per le attività

* Per impostazione predefinita, agli utenti viene assegnata una percentuale di tempo uguale per le attività a cui sono assegnati.
* È possibile modificare manualmente la percentuale di allocazione per gli utenti e i ruoli di lavoro assegnati alle attività solo quando il tipo di durata dell&#39;attività è Lavoro calcolato o Basato su sforzo.

   Per informazioni, consulta [Panoramica del tipo di durata e durata dell’attività](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

* Non è possibile modificare l&#39;allocazione percentuale per i team assegnati alle attività.
* Non è possibile modificare l&#39;allocazione percentuale per gli utenti e i ruoli di lavoro assegnati ai problemi.

## Modificare l&#39;allocazione dell&#39;utente o della percentuale del ruolo per un&#39;attività

1. Passare a un&#39;attività per le cui risorse si sta modificando l&#39;allocazione della percentuale.
1. Fai clic sul pulsante **Altro** menu ![](assets/qs-more-icon-on-an-object.png) accanto al nome dell’attività, quindi fai clic su **Modifica**.

   Oppure

   Fai clic sul pulsante **Assegnazioni** area nell&#39;intestazione dell&#39;attività, quindi fare clic su **Avanzate**.

1. Assicurati che **Tipo di durata** dell&#39;attività è una delle seguenti:

   * Lavoro Calcolato
   * Impegno Aggiuntivo

   >[!TIP]
   >
   >* Per il tipo di durata dell&#39;assegnazione calcolata, Workfront utilizza la formula seguente per calcolare la percentuale di allocazione di ciascun assegnatario: `Allocation Percentage = (Work Required / Number of days in the Duration) / Number of hours per work day / Number of assignees`.
   >* Per il tipo di durata semplice, puoi stimare le ore assegnate a ciascuna risorsa, non la percentuale di allocazione.


1. Fai clic su **Assegnazioni**, quindi modifica il **Allocazioni** per ciascun assegnatario.

   È possibile modificare solo la percentuale di allocazione per le assegnazioni di ruoli utente e processo.

   Non è possibile modificare la percentuale di allocazione per un team assegnato a un task.

   ![](assets/qs-advanced-assignments-box-with-duration-type-and-duration-350x251.png)

1. Fai clic su **Salva**.
