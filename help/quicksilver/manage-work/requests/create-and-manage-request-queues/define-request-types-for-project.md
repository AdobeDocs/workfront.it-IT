---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: Definire i tipi di richiesta per un progetto
description: Puoi organizzare il tipo di problemi o richieste che sono connessi in Adobe Workfront per tipo di richiesta.
author: Alina
feature: Work Management
exl-id: 627749bb-a8d7-4cc2-9d11-237811f82eb8
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 2%

---

# Definire i tipi di richiesta per un progetto

Puoi organizzare il tipo di problemi o richieste che sono connessi in Adobe Workfront per tipo di richiesta.

Questa organizzazione è utile per motivi di reporting e per aiutare gli utenti a comprendere che tipo di lavoro imprevisto può verificarsi durante la durata di un progetto.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">piano Adobe Workfront</a>*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FAdministration_and_Setup%2FAdd_users%2FAccess_levels_and_object_permissions%2Fwf-licenses.html&amp;_LANG=en" target="_blank">Licenza Adobe Workfront</a>*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica accesso a progetti</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un progetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Prerequisiti

Prima di iniziare, devi

* Avere o creare un progetto

   Per informazioni sulla creazione di progetti, consulta [Creare un progetto](../../../manage-work/projects/create-projects/create-project.md).

## Considerazioni sui tipi di richieste

* Puoi specificare il tipo di problemi o richieste che possono essere registrati su un progetto quando configuri il **Dettagli coda** area del progetto.
* Non è necessario abilitare il progetto come coda di richiesta per poter definire i tipi di richiesta per un progetto. Qualsiasi problema registrato per un progetto può essere etichettato con un tipo di richiesta diverso.
* Se si aggiungono argomenti sulla coda al progetto, è necessario definire i tipi di richieste in ogni argomento della coda per visualizzarlo quando si aggiunge un nuovo problema o richiesta. Per ulteriori informazioni, consulta [Crea argomenti coda](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

## Definire i tipi di problema o di richiesta per un progetto

1. Fai clic su **Progetti** nel menu principale. ![](assets/main-menu-icon.png)

1. Fai clic sul nome del progetto per aprirlo.
1. Nel pannello a sinistra, fai clic su **Dettagli coda**.
1. In **Proprietà coda** seleziona la sezione **Tipi di richieste** tu vuoi il progetto.

   >[!NOTE]
   >
   >È necessario che sia selezionato almeno un tipo di richiesta. Puoi selezionare più tipi di richiesta.

   Seleziona uno dei seguenti tipi:

   * Segnalazione Bug
   * Richiesta di Modifica
   * Problema
   * Richiesta

   >[!TIP]
   >
   >È possibile che l’amministratore di Workfront abbia rinominato alcune di queste opzioni. Per informazioni, consulta [Configurare i tipi di richiesta](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md).

1. Fai clic su **Salva**.

   I tipi di richiesta specificati saranno disponibili per selezionare quando si immette un nuovo problema su un&#39;attività o un progetto o quando si invia una nuova richiesta al progetto, se il progetto è abilitato come coda di richiesta.
