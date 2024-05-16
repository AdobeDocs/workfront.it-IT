---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Gestire la percentuale di allocazione di utenti o ruoli sulle attività
description: La percentuale di allocazione rappresenta la quantità di tempo in cui una risorsa assegnata deve lavorare su un'attività in un giorno. Rappresenta la percentuale di un giorno lavorativo (in base alla programmazione dell'utente o del progetto) in cui una risorsa viene allocata per l'intera durata dell'attività.
author: Alina
feature: Work Management
exl-id: 82238dff-b95e-42e4-8e72-6247934b504d
source-git-commit: 0d525df9beacc989ec3c1c695a7757dff0ad77b3
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 1%

---

# Gestire la percentuale di allocazione di utenti o ruoli sulle attività

<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti oppure nell’ambiente di produzione per i clienti che hanno abilitato le versioni rapide.</span>

<span class="preview">Per informazioni sulle versioni rapide, consulta [Abilitare o disabilitare le versioni rapide per la tua organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">Per informazioni sulla versione corrente, consulta [Panoramica sulla versione del terzo trimestre 2024](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).</span>

La percentuale di allocazione rappresenta la quantità di tempo in cui una risorsa assegnata deve lavorare su un&#39;attività in un giorno. Rappresenta la percentuale di un giorno lavorativo (in base alla programmazione dell&#39;utente o del progetto) in cui una risorsa viene allocata per l&#39;intera durata dell&#39;attività.

>[!NOTE]
>
>Quando si assegnano gli utenti al lavoro, la loro disponibilità in base alle loro pianificazioni influisce sulle date pianificate e previste delle attività e dei problemi. Per informazioni sulle pianificazioni, consulta [Creare una pianificazione](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

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
   <td> <p>Autorizzazioni di contribuzione o di livello superiore per l'attività</p> <p>Modificare le autorizzazioni per aggiornare la percentuale di allocazione nella casella Modifica attività</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

## Considerazioni sulla modifica delle allocazioni percentuali per le attività

* Per impostazione predefinita, agli utenti viene assegnata una percentuale di tempo uguale per le attività a cui sono assegnati.
* È possibile modificare manualmente la percentuale di allocazione per gli utenti e i ruoli assegnati alle attività solo quando il tipo di durata dell&#39;attività è Lavoro calcolato o Basato sulle risorse.

  Per informazioni, consulta [Panoramica sulla durata e sul tipo di durata dell&#39;attività](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

* Non è possibile modificare la percentuale di allocazione per i team assegnati alle attività.
* Non puoi modificare la percentuale di allocazione per utenti e mansioni assegnati ai problemi.

## Modificare l&#39;allocazione percentuale di utenti o ruoli per un&#39;attività

1. Passare a un&#39;attività per la quale si desidera modificare la percentuale di allocazione delle risorse.
1. Fai clic su **Altro** menu ![](assets/qs-more-icon-on-an-object.png) accanto al nome dell&#39;attività, quindi fare clic su **Modifica**.

   Oppure

   Fai clic su **Assegnazioni** nell’intestazione dell’attività, quindi fai clic su **Avanzate**.

1. Assicurati che **Tipo di durata** dell&#39;attività è una delle seguenti:

   * Lavoro Calcolato
   * Impegno Aggiuntivo

   >[!TIP]
   >
   >* Per il tipo di durata dell&#39;assegnazione calcolata, Workfront utilizza la formula seguente per calcolare la percentuale di allocazione di ciascun assegnatario: `Allocation Percentage = (Work Required / Number of days in the Duration) / Number of hours per work day / Number of assignees`.
   >* Per il tipo di durata semplice, è possibile stimare le ore assegnate a ciascuna risorsa, non la percentuale di allocazione.

1. Clic **Assegnazioni**, quindi modifica il **Allocazioni** per ogni assegnatario dell’attività.

   È possibile modificare solo la percentuale di allocazione per le assegnazioni utente e ruolo.

   Non è possibile modificare la percentuale di allocazione per un team assegnato a un&#39;attività.

   Immagine di esempio nell’ambiente di produzione:
   ![](assets/qs-advanced-assignments-box-with-duration-type-and-duration-350x251.png)

   <span class="preview">Immagine di esempio nell’ambiente di anteprima:</span>
   ![Modifica percentuale di allocazione](assets/advanced-assignments-allocation-percentage.png)

1. Fai clic su **Salva**.
