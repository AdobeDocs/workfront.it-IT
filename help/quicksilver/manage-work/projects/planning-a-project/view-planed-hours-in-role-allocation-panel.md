---
product-area: projects
navigation-topic: plan-a-project
title: Visualizza le ore pianificate per il progetto nel pannello Allocazione ruoli
description: È possibile visualizzare l'allocazione dei ruoli per tutte le mansioni assegnate agli elementi di lavoro in un progetto nel pannello Allocazione ruoli del progetto.
author: Alina, Lisa
feature: Work Management
exl-id: 76f70cb6-f707-4a73-bc81-e755e2d0a33d
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 5%

---

# Visualizza le ore pianificate per il progetto nel pannello Allocazione ruoli

È possibile visualizzare l&#39;allocazione dei ruoli per tutte le mansioni assegnate agli elementi di lavoro in un progetto nel pannello Allocazione ruoli del progetto.

>[!NOTE]
>
>Questo articolo si riferisce alla visualizzazione dei ruoli associati alle attività e ai problemi su un progetto e delle relative ore pianificate allocate nel pannello Allocazione ruoli di un progetto. Per informazioni sulla riconciliazione delle ore pianificate con le ore delle iniziative tramite il pannello Allocazione ruoli quando si utilizza Adobe Workfront Scenario Planner, vedi:
>
>* [Mostra allocazione ruoli per progetti e iniziative nell&#39;elenco attività](../../../scenario-planner/show-role-allocation-task-list-nwe.md)
>* [Mostra allocazione ruoli per progetti e iniziative nel Bilanciatore dei carichi di lavoro](../../../scenario-planner/show-role-allocation-workload-balancer.md)
>
>  Per visualizzare le ore di iniziativa nel pannello Allocazione ruoli, è necessario disporre di una licenza di Pianificazione scenario. Per informazioni sulla Pianificazione scenario, vedere [Introduzione alla Pianificazione scenario](../../../scenario-planner/get-started-with-scenario-planning.md).
>
>Se la tua azienda ha acquistato Adobe Scenario Planner in passato, è stata esentata dalla clausola di salvaguardia. La Pianificazione scenario non è più disponibile per l&#39;acquisto.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Adobe Workfront Ultimate</p>
   <p>Ultimate flusso di lavoro Adobe</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> 
   <p>Chiaro o superiore</p>
   <p>Revisione o successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Accesso ai progetti di visualizzazione o superiore</p>
   <p>Modifica l'accesso a Scenario Planner per aggiornare le ore sulle iniziative</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizza o autorizzazioni superiori per il progetto</p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

able style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Review or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects</p> <p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions on the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Prerequisiti

Devi avere i seguenti:

* Attività o problemi assegnati a mansioni o a utenti associati a una mansione.

  >[!TIP]
  >
  >Se le attività o i problemi vengono revocati, assegnati a team o assegnati a utenti senza mansione, le ore pianificate del progetto nel pannello Allocazione mansioni sono pari a zero.

* Attività e problemi con una durata superiore a zero.

## Visualizza le ore pianificate per il progetto nel pannello Allocazione ruoli

{{step1-to-projects}}

1. Fai clic sul nome di un progetto per accedervi. Viene visualizzata la pagina Progetto.
1. Fai clic su una delle seguenti opzioni nel pannello a sinistra:

   * **Attività**
   * **Bilanciamento del carico di lavoro**

1. Fai clic sull&#39;icona **Mostra allocazione ruoli** ![Mostra icona allocazione ruoli](assets/show-role-allocation-icon.png).

   Viene visualizzato il pannello Allocazione ruoli.

   ![Pannello Allocazione ruoli con solo ore pianificate](assets/role-allocation-panel-planned-hours-only-350x316.png)

1. Rivedi le seguenti informazioni nel pannello **Allocazione ruoli**:

   | Campo | Descrizione |
   |---|---|
   | **Mansione** | Ruoli assegnati ad attività e problemi sul progetto. Possono essere ruoli assegnati direttamente ad attività e problemi o ruoli associati agli utenti assegnati ad attività e problemi sul progetto. |
   | **Ore pianificate** | Il numero totale di ore pianificate dalle attività e dai problemi assegnati a mansioni o utenti associati a una mansione sul progetto. |

