---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Creazione di assegnazioni avanzate
description: È possibile gestire le assegnazioni di task o di problemi utilizzando le assegnazioni avanzate.
author: Alina
feature: Work Management
exl-id: 09780f78-4eb8-404d-859b-d066d462776d
source-git-commit: 3f5e5e9832fc33d39ea5dfbbc513b80adbf113f5
workflow-type: tm+mt
source-wordcount: '1135'
ht-degree: 0%

---

# Creazione di assegnazioni avanzate

È possibile gestire le assegnazioni di task o di problemi utilizzando le assegnazioni avanzate.

È possibile modificare le seguenti informazioni sull&#39;assegnazione quando si eseguono assegnazioni avanzate:

* Assegna gli utenti all’attività o al problema (che può essere eseguito al di fuori di un’assegnazione avanzata).
* Adegua e ridistribuisci il numero di ore assegnate a ciascun assegnatario.
* Determinare quale utente deve essere designato come proprietario o come principale assegnatario dell&#39;attività o del problema.
* Specificare il ruolo che ogni utente deve svolgere quando si lavora sull&#39;attività o sul problema.

>[!NOTE]
>
>Quando si assegnano gli utenti al lavoro, la loro disponibilità in base alle loro pianificazioni influisce sulle date previste e previste delle attività e dei problemi. Per informazioni sulle pianificazioni, consulta [Creare una pianificazione](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

## Aree di Adobe Workfront in cui è possibile effettuare assegnazioni avanzate

Questo articolo descrive come accedere alle assegnazioni avanzate nell&#39;intestazione dell&#39;attività o del problema.

Inoltre, è possibile effettuare assegnazioni avanzate nelle seguenti aree di Workfront:

* Negli elenchi e nei rapporti quando il campo Assegnazioni viene visualizzato nella visualizzazione.
* Nella sezione Assegnazioni durante la modifica di un&#39;attività. Per ulteriori informazioni, consulta [Modifica delle attività](../../../manage-work/tasks/manage-tasks/edit-tasks.md).
* Nell&#39;intestazione dell&#39;attività o del problema, nell&#39;area Assegnazioni.
* Nel servizio di bilanciamento del carico di lavoro. Per ulteriori informazioni, consulta [Assegnare il lavoro manualmente utilizzando il bilanciamento del carico di lavoro](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-manually.md).

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
   <td> <p>Modifica l'accesso alle attività e ai problemi</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Contribuire o autorizzazioni superiori a un'attività o un problema</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Esecuzione di assegnazioni avanzate

1. Passa al progetto in cui desideri assegnare un’attività o un problema.
1. Fai clic su **Attività** o **Problemi** nel pannello a sinistra, fai clic sul nome di un’attività o di un problema nell’elenco.

   >[!TIP]
   >
   >È possibile effettuare assegnazioni avanzate direttamente nell&#39;attività o nell&#39;elenco dei problemi se sono assegnate due o più persone. Fai clic all’interno del **Assegnazioni** sulla stessa riga dell&#39;attività o del problema, quindi fai clic sul **Icona Persone** per aprire la finestra Assegnazioni avanzate. Passa al passaggio 5 per continuare a creare assegnazioni avanzate.\
   >![](assets/nwe-advanced-assignments-350x55.png)   >

1. Fai clic su **Assegna a** in **Assegnazioni** campo nell’intestazione dell’attività o del problema

   Oppure

   Fare clic sul nome delle assegnazioni se l&#39;attività o il problema è già assegnato.

1. Fai clic su **Avanzate**.

   ![](assets/advanced-assignments-link-from-task-header-nwe-350x267.png)

1. In **Cercare persone, ruoli e team** inizia a digitare il nome di un utente, di un ruolo o di un team, quindi fai clic sul nome quando viene visualizzato nell’elenco a discesa.

   >[!NOTE]
   >
   >Se il nome dell’utente contiene un carattere speciale, è necessario includere il carattere speciale nel campo di ricerca.

1. (Facoltativo) Continua ad aggiungere assegnatari nel **Cercare persone, ruoli o team** per aggiungere più risorse all&#39;attività o al problema.

   >[!TIP]
   >
   >* È possibile assegnare più utenti, ruoli o team. È possibile assegnare solo utenti attivi, ruoli e team.
   >
   >
   >* Quando aggiungi un&#39;assegnazione utente, osserva l&#39;avatar, il ruolo principale dell&#39;utente o il relativo indirizzo e-mail per distinguere tra utenti con nomi identici. Gli utenti devono essere associati ad almeno un ruolo di lavoro per visualizzarlo durante l&#39;aggiunta.
   >
   >
   >* Se un utente, un ruolo di lavoro o un team è stato assegnato prima della disattivazione, rimangono assegnati all&#39;elemento di lavoro. In questo caso, si consiglia quanto segue:
      >   
      >   * Riassegna l&#39;elemento di lavoro alle risorse attive.
      >   * Associare gli utenti di un team disattivato a un team attivo e riassegnare l&#39;elemento di lavoro al team attivo.


1. Per ogni utente nel **Assegnatario** , specifica le seguenti informazioni:


   * **Proprietario**: Passa il puntatore del mouse sul nome dell&#39;assegnatario e fai clic su **Rendi primario** nel campo Proprietario se si desidera contrassegnare l&#39;assegnatario come proprietario dell&#39;attività o del problema. Una casella di controllo verde indica che l&#39;utente specificato è il contatto principale dell&#39;attività o del problema. Adobe Workfront contrassegna il primo ruolo utente o di lavoro assegnato a un&#39;attività o a un problema come Proprietario o Assegnazione principale. Impossibile designare un team come proprietario principale di un&#39;attività o di un problema.

      >[!IMPORTANT]
      >
      >A seconda della configurazione delle preferenze di progetto da parte dell’amministratore di Workfront o dell’amministratore di gruppo, Workfront potrebbe utilizzare la pianificazione del proprietario dell’attività per calcolare la cronologia dell’attività quando a tale attività sono assegnati più utenti. Per informazioni su più assegnazioni di attività, consulta la sezione &quot;Assegnare più utenti a un’attività&quot; nell’articolo [Assegnare le attività](../../../manage-work/tasks/assign-tasks/assign-tasks.md).

   * **Allocazioni** : Quando il tipo di durata di un&#39;attività è Semplice, specificare il numero di ore in cui ogni utente o ruolo di lavoro deve essere assegnato all&#39;attività. La somma di tutte le ore assegnate per ogni utente è uguale al numero nel **Orari pianificati** campo nella parte inferiore della colonna Allocazioni. In tutti gli altri casi, specificare la percentuale di tempo (o allocazione) che l&#39;assegnatario deve trascorrere per risolvere l&#39;attività o il problema.

      <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: make sure this is right in the new UI for both classic and QS???)</p>   
     -->

      >[!TIP]
      >
      >
      >   
      >   
      >   * Dopo aver modificato manualmente le allocazioni di assegnazione per le attività, è possibile che l&#39;orario pianificato delle attività venga aggiornato di conseguenza. Per ulteriori informazioni, consulta la sezione &quot;Aggiornare le ore pianificate delle attività durante la gestione delle allocazioni degli utenti&quot; nell’articolo [Panoramica sull’orario pianificato](../../../manage-work/tasks/task-information/planned-hours.md).
      >   * Non è possibile modificare manualmente le allocazioni di assegnazione in caso di problemi.
      >   * Non è possibile modificare manualmente le allocazioni per i team assegnati alle attività.


   * **Ruolo dell&#39;assegnatario:** Selezionare il ruolo che l&#39;utente deve utilizzare per completare l&#39;assegnazione.  Per impostazione predefinita viene visualizzato il Ruolo principale dell’utente. Fare clic nella casella Ruolo assegnatario per selezionare un altro ruolo.  Quando si assegna prima l’attività o il problema a un ruolo e quindi si aggiunge un utente che può svolgere tale ruolo come seconda assegnazione, l’elenco degli utenti consigliati viene filtrato per gli utenti che possono svolgere i ruoli già assegnati all’attività e al problema.

      ![](assets/advanced-assignments-box-select-a-role-350x243.png)

   * **Tipo di durata**: Questa opzione è disponibile solo per le attività. Fare clic sul nome del tipo di durata e selezionare un tipo di durata dal menu a discesa. Per informazioni sui tipi di durata, consulta [Panoramica del tipo di durata e durata dell’attività](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

   * **Durata:** È possibile aggiornare questo campo per un&#39;attività quando si dispone delle autorizzazioni di gestione per l&#39;attività.

      Per ulteriori informazioni, consulta [Panoramica del tipo di durata e durata dell’attività](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md). Quando si modificano in serie le informazioni sull&#39;assegnazione, viene visualizzata una finestra di dialogo simile per assegnare utenti, ore, allocazione e proprietario dell&#39;attività.

   * **Orari pianificati**: Quando il tipo di durata è Assegnazione calcolata o Semplice, aggiornare il numero di ore pianificate. Di conseguenza, le percentuali di allocazione o le ore per ogni risorsa vengono distribuite in modo uniforme. Workfront calcola le ore pianificate quando il tipo di durata è Lavoro calcolato o Sforzo guidato. Per ulteriori informazioni, consulta [Panoramica del tipo di durata e durata dell’attività](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

      ![](assets/qs-advanced-assignments-box-with-duration-type-and-duration-350x251.png)

1. Fai clic su **Salva**.
