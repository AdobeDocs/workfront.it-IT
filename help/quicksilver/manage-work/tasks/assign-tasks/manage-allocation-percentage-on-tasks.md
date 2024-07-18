---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Gestire la percentuale di allocazione di utenti o ruoli sulle attività
description: La percentuale di allocazione rappresenta la quantità di tempo in cui una risorsa assegnata deve lavorare su un'attività in un giorno. Rappresenta la percentuale di un giorno lavorativo (in base alla programmazione dell'utente o del progetto) in cui una risorsa viene allocata per l'intera durata dell'attività.
author: Alina
feature: Work Management
exl-id: 82238dff-b95e-42e4-8e72-6247934b504d
source-git-commit: 830ad0411084844ace1e1e543c3ebefcb558af80
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 1%

---

# Gestire la percentuale di allocazione di utenti o ruoli sulle attività

La percentuale di allocazione rappresenta la quantità di tempo in cui una risorsa assegnata deve lavorare su un&#39;attività in un giorno. Rappresenta la percentuale di un giorno lavorativo (in base alla programmazione dell&#39;utente o del progetto) in cui una risorsa viene allocata per l&#39;intera durata dell&#39;attività.

>[!NOTE]
>
>Quando si assegnano gli utenti al lavoro, la loro disponibilità in base alle loro pianificazioni influisce sulle date pianificate e previste delle attività e dei problemi. Per informazioni sulle pianificazioni, vedere [Creare una pianificazione](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Nuovo: Standard</p> 
   <p>Corrente: Lavoro o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica l'accesso alle Attività</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Autorizzazioni Contribute o superiori per l’attività</p> <p>Modificare le autorizzazioni per aggiornare la percentuale di allocazione nella casella Modifica attività</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni, consulta [Requisiti di accesso per la documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerazioni sulla modifica delle allocazioni percentuali per le attività

* Per impostazione predefinita, agli utenti viene assegnata una percentuale di tempo uguale per le attività a cui sono assegnati.
* È possibile modificare manualmente la percentuale di allocazione per gli utenti e i ruoli assegnati alle attività solo quando il tipo di durata dell&#39;attività è Lavoro calcolato o Basato sulle risorse.

  Per informazioni, vedere [Panoramica sulla durata e sul tipo di durata dell&#39;attività](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

* Non è possibile modificare la percentuale di allocazione per i team assegnati alle attività.
* Non puoi modificare la percentuale di allocazione per utenti e mansioni assegnati ai problemi.

## Modificare l&#39;allocazione percentuale di utenti o ruoli per un&#39;attività

1. Passare a un&#39;attività per la quale si desidera modificare la percentuale di allocazione delle risorse.
1. Fai clic sul menu **Altro** ![](assets/qs-more-icon-on-an-object.png) accanto al nome dell&#39;attività, quindi fai clic su **Modifica**.

   Oppure

   Fai clic sull&#39;area **Assegnazioni** nell&#39;intestazione dell&#39;attività, quindi fai clic su **Avanzate**.

1. Assicurati che il **Tipo di durata** dell&#39;attività sia uno dei seguenti:

   * Lavoro Calcolato
   * Impegno Aggiuntivo

   >[!TIP]
   >
   >* Per il tipo di durata dell&#39;assegnazione calcolata, Workfront utilizza la formula seguente per calcolare la percentuale di allocazione di ciascun assegnatario: `Allocation Percentage = (Work Required / Number of days in the Duration) / Number of hours per work day / Number of assignees`.
   >* Per il tipo di durata semplice, è possibile stimare le ore assegnate a ciascuna risorsa, non la percentuale di allocazione.

1. Fai clic su **Assegnazioni**, quindi modifica le **Allocazioni** per ogni assegnatario dell&#39;attività.

   È possibile modificare solo la percentuale di allocazione per le assegnazioni utente e ruolo.

   Non è possibile modificare la percentuale di allocazione per un team assegnato a un&#39;attività.

   ![Modifica percentuale di allocazione](assets/advanced-assignments-allocation-percentage.png)

1. Fai clic su **Salva**.
