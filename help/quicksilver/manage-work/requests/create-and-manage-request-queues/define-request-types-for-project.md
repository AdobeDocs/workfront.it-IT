---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: Definire i tipi di richiesta per un progetto
description: Puoi organizzare il tipo di problemi o richieste connessi ad Adobe Workfront per tipo di richiesta.
author: Alina
feature: Work Management
exl-id: 627749bb-a8d7-4cc2-9d11-237811f82eb8
source-git-commit: 9b6552fe496a1602786cdc6b6050d02cd367a531
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 2%

---

# Definire i tipi di richiesta per un progetto

Puoi organizzare il tipo di problemi o richieste connessi ad Adobe Workfront per tipo di richiesta.

Questa organizzazione è utile per ragioni di reporting e per aiutare gli utenti a comprendere che tipo di lavoro imprevisto potrebbe verificarsi durante la durata di un progetto.

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
   <td role="rowheader"><a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md">Panoramica sulle licenze</a>*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modifica accesso ai progetti</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un progetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

## Prerequisiti

Prima di iniziare, è necessario effettuare le seguenti operazioni:

* Avere o creare un progetto

  Per informazioni sulla creazione di progetti, consulta [Creare un progetto](../../../manage-work/projects/create-projects/create-project.md).

## Considerazioni sui tipi di richiesta

* Puoi specificare il tipo di problemi o richieste che possono essere registrati in un progetto quando configuri il **Dettagli coda** area per il progetto.
* Per poter definire i tipi di richiesta per un progetto, non è necessario abilitare il progetto come coda di richieste. Qualsiasi problema registrato per un progetto può essere etichettato con un diverso Tipo di richiesta.
* Se aggiungi Argomenti coda al progetto, devi definire Tipi di richiesta su ciascun argomento della coda per visualizzarlo quando aggiungi un nuovo problema o una nuova richiesta. Per ulteriori informazioni, consulta [Crea argomenti coda](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

## Definire i tipi di problemi o richieste per un progetto

1. Clic **Progetti** nel menu principale. ![](assets/main-menu-icon.png)

1. Fai clic sul nome del progetto per aprirlo.
1. Nel pannello a sinistra, fai clic su **Dettagli coda**.
1. In **Proprietà coda** , seleziona la sezione **Tipi di richieste** vuoi per il progetto.

   >[!NOTE]
   >
   >È necessario selezionare almeno un tipo di richiesta. Puoi selezionare più tipi di richiesta.

   Selezionare uno dei tipi seguenti:

   * Segnalazione Bug
   * Richiesta di Modifica
   * Problema
   * Richiesta

   >[!TIP]
   >
   >L&#39;amministratore di Workfront potrebbe aver rinominato alcune di queste opzioni. Per informazioni, consulta [Configurare i tipi di richiesta](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md).

1. Fai clic su **Salva**.

   I tipi di richiesta specificati saranno disponibili per la selezione quando si immette un nuovo problema in un&#39;attività o in un progetto oppure quando si invia una nuova richiesta al progetto, se il progetto è abilitato come coda di richieste.
