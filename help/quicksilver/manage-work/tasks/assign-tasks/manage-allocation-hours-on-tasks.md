---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Gestire le ore di allocazione di utenti e ruoli sulle attività
description: Quando si assegnano utenti o ruoli a un’attività, questi vengono assegnati in modo da lavorare un determinato numero di ore per completare l’attività. È possibile modificare manualmente la quantità di ore assegnate a ciascun utente o mansione quando viene assegnato a un'attività, quando il tipo di durata dell'attività è Semplice.
author: Alina
feature: Work Management
exl-id: 2c0cd6ef-8719-4680-aa63-5e229de0f819
source-git-commit: dd015fc356f65cc3d00a1c88ca0a8f2268283606
workflow-type: tm+mt
source-wordcount: '582'
ht-degree: 0%

---

# Gestire le ore di allocazione di utenti e ruoli sulle attività

Quando si assegnano utenti o ruoli a un’attività, questi vengono assegnati in modo da lavorare un determinato numero di ore per completare l’attività. È possibile modificare manualmente la quantità di ore assegnate a ciascun utente o mansione quando viene assegnato a un&#39;attività, quando il tipo di durata dell&#39;attività è Semplice.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Lavoro o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modifica l'accesso alle Attività</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Autorizzazioni Contribute o superiori per l’attività</p> <p>Modificare le autorizzazioni per aggiornare le ore di allocazione nella casella Modifica attività</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

## Considerazioni sulla modifica delle ore di allocazione per un&#39;attività

>[!IMPORTANT]
>
>Dopo aver modificato manualmente le allocazioni per ogni assegnazione sulle attività, le ore pianificate delle attività potrebbero essere aggiornate di conseguenza. Per ulteriori informazioni, consulta la sezione [Aggiornare le ore pianificate per l&#39;attività durante la gestione delle allocazioni utente](../../../manage-work/tasks/task-information/planned-hours.md#update) nell&#39;articolo [Panoramica sulle ore pianificate](../../../manage-work/tasks/task-information/planned-hours.md).

* Il totale delle ore assegnate alle singole risorse assegnate all&#39;attività rappresenta le ore pianificate dell&#39;attività.
* Se a un&#39;attività è assegnato un utente o un ruolo, la quantità di ore assegnate all&#39;utente o al ruolo corrisponde alle ore pianificate dell&#39;attività.
* In caso di assegnazioni multiple, a ciascun utente o mansione viene assegnato un numero uguale di ore per lavorare sull&#39;attività, per impostazione predefinita, se il tipo di durata dell&#39;attività è Semplice. Per ulteriori informazioni, consulta i seguenti articoli:

   * [Panoramica della durata e del tipo di durata dell&#39;attività](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)
   * [Panoramica sul tipo di durata: semplice](../../../manage-work/tasks/taskdurtn/simple-duration-type.md)

* Quando l&#39;attività ha un tipo di durata semplice, è possibile modificare manualmente la quantità di ore allocate per ogni utente o mansione per indicare che alcuni degli assegnatari dell&#39;attività potrebbero avere più tempo per lavorare su un&#39;attività rispetto ad altri.
* Non è possibile modificare la quantità di ore assegnate ai team assegnati alle attività.
* Non è possibile modificare manualmente l’allocazione di utenti o mansioni per i problemi.
* Puoi anche gestire le allocazioni giornaliere, settimanali o mensili degli utenti alle attività o ai problemi utilizzando il Bilanciatore dei carichi di lavoro. Per ulteriori informazioni, consulta [Gestire le allocazioni utente nel Bilanciatore dei carichi di lavoro](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## Modificare le ore di allocazione utente o ruolo per un&#39;attività

1. Passare a un&#39;attività per la quale si desidera modificare le ore di allocazione.
1. Fai clic sul menu **Altro** ![](assets/qs-more-icon-on-an-object.png) accanto al nome dell&#39;attività, quindi fai clic su **Modifica**, quindi su **Assegnazioni**.

   Oppure

   Fai clic sull&#39;area **Assegnazioni** nell&#39;intestazione dell&#39;attività, quindi fai clic su **Avanzate**.

1. Assicurarsi che il **Tipo di durata** dell&#39;attività sia **Semplice**.
1. Modifica le **Allocazioni** per ogni assegnatario dell&#39;attività. Si tratta delle allocazioni complessive per ogni assegnazione a questa attività, per l&#39;intera durata dell&#39;attività. Questo potrebbe anche aggiornare le ore pianificate complessive dell&#39;attività.

   ![Modifica allocazioni](assets/advanced-assignments-duration-type-allocations.png)

1. Fai clic su **Salva**.
