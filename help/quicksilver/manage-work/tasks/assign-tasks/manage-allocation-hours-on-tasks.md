---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Gestione delle ore di allocazione di utenti e ruoli sulle attività
description: Quando si assegnano utenti o ruoli a un'attività, questi vengono allocati per lavorare un certo numero di ore per completare l'attività. È possibile modificare manualmente la quantità di ore assegnate a ciascun utente o ruolo di lavoro quando viene assegnato a un'attività, quando il tipo di durata dell'attività è semplice.
author: Alina
feature: Work Management
exl-id: 2c0cd6ef-8719-4680-aa63-5e229de0f819
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 0%

---

# Gestione delle ore di allocazione di utenti e ruoli sulle attività

Quando si assegnano utenti o ruoli a un&#39;attività, questi vengono allocati per lavorare un certo numero di ore per completare l&#39;attività. È possibile modificare manualmente la quantità di ore assegnate a ciascun utente o ruolo di lavoro quando viene assegnato a un&#39;attività, quando il tipo di durata dell&#39;attività è semplice.

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
   <td> <p>Collaborare o autorizzazioni superiori per l'attività</p> <p>Modificare le autorizzazioni per aggiornare le ore di allocazione nella casella Modifica attività</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Considerazioni sulla modifica delle ore di allocazione per un&#39;attività

>[!IMPORTANT]
>
>Dopo aver modificato manualmente le allocazioni per ogni assegnazione per le attività, è possibile che l&#39;orario pianificato delle attività venga aggiornato di conseguenza. Per ulteriori informazioni, consulta la sezione . [Aggiorna le ore pianificate dell&#39;attività durante la gestione delle allocazioni degli utenti](../../../manage-work/tasks/task-information/planned-hours.md#update) nell&#39;articolo [Panoramica sull’orario pianificato](../../../manage-work/tasks/task-information/planned-hours.md).

* Il totale di ore assegnate alle singole risorse assegnate all&#39;attività rappresenta l&#39;orario pianificato dell&#39;attività.
* Se un&#39;attività è assegnata a un utente o a un ruolo, la quantità di ore assegnate all&#39;utente o al ruolo corrisponde alle ore pianificate dell&#39;attività.
* Nel caso di più assegnazioni, a ciascun utente o ruolo di lavoro viene assegnata una quantità uguale di ore per lavorare sull&#39;attività, per impostazione predefinita, se il tipo di durata dell&#39;attività è Semplice. Per ulteriori informazioni, consulta i seguenti articoli:

   * [Panoramica del tipo di durata e durata dell’attività](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)
   * [Panoramica sul tipo di durata: Semplice](../../../manage-work/tasks/taskdurtn/simple-duration-type.md)

* Quando l&#39;attività ha un tipo di durata semplice, è possibile modificare manualmente la quantità di ore assegnate per ogni utente o ruolo di lavoro per indicare che alcuni degli assegnatari dell&#39;attività potrebbero avere più tempo per lavorare su un&#39;attività rispetto ad altri.
* Non è possibile modificare la quantità di ore assegnate ai team assegnati alle attività.
* Non è possibile modificare manualmente l&#39;allocazione del ruolo utente o di lavoro per i problemi.
* È inoltre possibile gestire le allocazioni giornaliere, settimanali o mensili degli utenti a attività o problemi utilizzando il servizio di bilanciamento del carico di lavoro. Per ulteriori informazioni, consulta [Gestire le allocazioni di utenti nel load balancer](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## Modificare le ore di allocazione utente o ruolo per un&#39;attività

1. Passare a un&#39;attività per le cui assegnazioni si desidera modificare le ore di allocazione.
1. Fai clic sul pulsante **Altro** menu ![](assets/qs-more-icon-on-an-object.png) accanto al nome dell’attività, quindi fai clic su **Modifica**, quindi **Assegnazioni**.

   Oppure

   Fai clic sul pulsante **Assegnazioni** area nell&#39;intestazione dell&#39;attività, quindi fare clic su **Avanzate**.

1. Assicurati che **Tipo di durata** dell&#39;attività **Semplice**.
1. Modifica la **Allocazioni** per ciascun assegnatario. Si tratta di allocazioni totali per ogni assegnazione a questa attività, per l&#39;intera durata dell&#39;attività. Questo potrebbe anche aggiornare l’orario pianificato generale dell’attività.

   ![](assets/advanced-assignments-simple-duration-multiple-resources-nwe-350x198.png)

1. Fai clic su **Salva**.
