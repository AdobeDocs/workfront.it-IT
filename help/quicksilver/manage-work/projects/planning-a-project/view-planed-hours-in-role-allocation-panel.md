---
product-area: projects
navigation-topic: plan-a-project
title: Visualizza le ore pianificate del progetto nel pannello Assegnazione ruolo
description: Puoi visualizzare l’allocazione dei ruoli per tutti i ruoli di lavoro assegnati agli elementi di un progetto nel pannello Assegnazione ruolo del progetto.
author: Alina
feature: Work Management
exl-id: 76f70cb6-f707-4a73-bc81-e755e2d0a33d
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '468'
ht-degree: 0%

---

# Visualizza le ore pianificate del progetto nel pannello Assegnazione ruolo

Puoi visualizzare l’allocazione dei ruoli per tutti i ruoli di lavoro assegnati agli elementi di un progetto nel pannello Assegnazione ruolo del progetto.

>[!NOTE]
>
>Questo articolo fa riferimento alla visualizzazione dei ruoli di lavoro associati alle attività e ai problemi di un progetto e delle ore pianificate assegnate nel pannello Assegnazione ruolo di un progetto. Per informazioni sulla riconciliazione delle ore pianificate con le iniziative che utilizzano il pannello Assegnazione ruoli quando si utilizza il planner scenario di Adobe Workfront, consulta quanto segue:
>
>* [Mostra l&#39;allocazione dei ruoli per progetti e iniziative nell&#39;elenco dei task](../../../scenario-planner/show-role-allocation-task-list-nwe.md)
>* [Mostra l’allocazione dei ruoli per progetti e iniziative nel servizio di bilanciamento del carico di lavoro](../../../scenario-planner/show-role-allocation-workload-balancer.md)
>
>  Per visualizzare le ore di iniziativa nel pannello Assegnazione ruoli , devi disporre di una licenza per planner scenario. Per informazioni sul planner dello scenario, consulta [Guida introduttiva a Scenario Planner](../../../scenario-planner/get-started-with-scenario-planning.md) .

## Requisiti di accesso

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Light or higher</p> 
   Or
   <p>Legacy license: Review or higher</p> 
   </td> 
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
</table>

-->

Devi disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Revisione o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Visualizzare o accedere in modo più rapido ai progetti</p> <p>Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizza o autorizzazioni superiori per il progetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Prerequisiti

Devi disporre dei seguenti elementi:

* Attività o problemi assegnati ai ruoli o agli utenti associati a un ruolo di lavoro.

   >[!TIP]
   Se le attività o i problemi non vengono assegnati, assegnati ai team o assegnati a utenti privi di ruolo, nel pannello Assegnazione ruolo l’orario pianificato del progetto è zero.

* Attività e problemi con una durata superiore a zero.

## Visualizza le ore pianificate del progetto nel pannello Assegnazione ruolo

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Progetti**.
1. Fai clic sul nome di un progetto per accedervi. Viene aperta la pagina Progetto .
1. Fai clic su una delle seguenti opzioni nel pannello a sinistra:

   * **Attività**
   * **Bilanciamento del carico di lavoro**

1. Fai clic sul pulsante **Mostra allocazione ruolo** icona ![](assets/show-role-allocation-icon.png).

   Viene visualizzato il pannello Assegnazione ruolo .

   ![](assets/role-allocation-panel-planned-hours-only-350x316.png)

1. Consulta le seguenti informazioni nella sezione **Assegnazione ruolo** pannello: |Campo | Descrizione | |—|—| | **Ruolo** |Ruoli di lavoro assegnati alle attività e ai problemi del progetto. Questi possono essere ruoli di lavoro assegnati direttamente alle attività e ai problemi o ai ruoli di lavoro associati agli utenti assegnati a attività e problemi del progetto.  | | **Orari pianificati** |Numero totale di ore pianificate dalle attività e dai problemi assegnati ai ruoli di lavoro o agli utenti associati a un ruolo di lavoro nel progetto. |



