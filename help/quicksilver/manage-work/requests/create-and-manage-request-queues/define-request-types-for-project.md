---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: Definire i tipi di richiesta per un progetto
description: Puoi organizzare il tipo di problemi o richieste connessi ad Adobe Workfront per tipo di richiesta.
author: Alina
feature: Work Management
exl-id: 627749bb-a8d7-4cc2-9d11-237811f82eb8
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/fOdoie2wI-EHoKmQTHy0cDaVipi6XYE1JgMHdX6-Tbo
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: c10f2e93-7a58-4212-aa24-684c265ebe76
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 354
ht-degree: 16%

---

# Definire tipi di richiesta per un progetto

<!-- Audited: 6/2025 -->

Puoi organizzare il tipo di problemi o richieste connessi ad Adobe Workfront per tipo di richiesta. Ciò è utile per ragioni di reporting e per aiutare gli utenti a comprendere che tipo di lavoro imprevisto potrebbe verificarsi durante il ciclo di vita di un progetto.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td>
    <p>Standard</p>
    <p>Piano</p></td>  
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica accesso ai progetti</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
   <td> <p>Gestire le autorizzazioni per un progetto</p></td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

Prima di iniziare, è necessario effettuare le seguenti operazioni:

* Disporre di o creare un progetto.

  Per informazioni sulla creazione di progetti, vedere [Creare un progetto](../../../manage-work/projects/create-projects/create-project.md).

## Considerazioni sui tipi di richiesta

* È possibile specificare il tipo di problemi o richieste che è possibile registrare in un progetto quando si configura l&#39;area Dettagli coda per il progetto.
* Per poter definire i tipi di richiesta per un progetto, non è necessario abilitare il progetto come coda di richieste. Qualsiasi problema registrato per un progetto può essere etichettato con un diverso Tipo di richiesta.
* Se aggiungi Argomenti coda al progetto, devi definire Tipi di richiesta su ciascun argomento della coda per visualizzarlo quando aggiungi un nuovo problema o una nuova richiesta. Per ulteriori informazioni, consulta [Creare argomenti di coda](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

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
