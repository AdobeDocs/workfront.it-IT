---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: Definire i tipi di richiesta per un progetto
description: Puoi organizzare il tipo di problemi o richieste connessi ad Adobe Workfront per tipo di richiesta.
author: Alina
feature: Work Management
exl-id: 627749bb-a8d7-4cc2-9d11-237811f82eb8
source-git-commit: abf5f21281b05dedfecbe71c6ffbf54ee69e2460
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 2%

---

# Definire i tipi di richiesta per un progetto

<!-- Audited: 6/2025 -->

Puoi organizzare il tipo di problemi o richieste connessi ad Adobe Workfront per tipo di richiesta. Ciò è utile per ragioni di reporting e per aiutare gli utenti a comprendere che tipo di lavoro imprevisto potrebbe verificarsi durante il ciclo di vita di un progetto.

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
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td>
    <p>Nuovo: Standard</p>
    <p>Corrente: Piano</p></td>  
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica accesso ai progetti</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un progetto</p></td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

Prima di iniziare, è necessario effettuare le seguenti operazioni:

* Disporre di o creare un progetto.

  Per informazioni sulla creazione di progetti, vedere [Creare un progetto](../../../manage-work/projects/create-projects/create-project.md).

## Considerazioni sui tipi di richiesta

* È possibile specificare il tipo di problemi o richieste che è possibile registrare in un progetto quando si configura l&#39;area Dettagli coda per il progetto.
* Per poter definire i tipi di richiesta per un progetto, non è necessario abilitare il progetto come coda di richieste. Qualsiasi problema registrato per un progetto può essere etichettato con un diverso Tipo di richiesta.
* Se aggiungi Argomenti coda al progetto, devi definire Tipi di richiesta su ciascun argomento della coda per visualizzarlo quando aggiungi un nuovo problema o una nuova richiesta. Per ulteriori informazioni, vedere [Creare argomenti coda](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

## Definire i tipi di problemi o richieste per un progetto

{{step1-to-projects}}

1. Nella pagina **Progetti**, seleziona un progetto.
1. Nel pannello a sinistra, fai clic su **Dettagli coda**.
1. Nella sezione **Proprietà coda** selezionare i **Tipi di richiesta** desiderati per il progetto:
   * Segnalazione Bug
   * Ordine di modifica
   * Problema
   * Richiesta

   >[!NOTE]
   >
   >* È necessario selezionare almeno un tipo di richiesta. Puoi selezionare più tipi.
   >* L&#39;amministratore di Workfront potrebbe aver rinominato alcune di queste opzioni. Per informazioni, vedere [Configurare i tipi di richiesta](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md).

1. Fai clic su **Salva**. I tipi di richiesta specificati saranno disponibili per la selezione quando si immette un nuovo problema in un&#39;attività o in un progetto oppure quando si invia una nuova richiesta al progetto (se il progetto è abilitato come coda di richieste).
