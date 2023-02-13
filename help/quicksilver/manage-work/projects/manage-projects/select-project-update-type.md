---
product-area: projects
navigation-topic: manage-projects
title: Seleziona il tipo di aggiornamento del progetto
description: Selezionando un tipo di aggiornamento per un progetto, puoi controllare la frequenza con cui vengono salvate le modifiche apportate alla timeline del progetto sulle attività principali o sul progetto.
author: Alina
feature: Work Management
exl-id: ffdfffec-d217-4daa-9849-cb0c794992c0
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 0%

---

# Seleziona il tipo di aggiornamento del progetto

Selezionando un tipo di aggiornamento per un progetto, puoi controllare la frequenza con cui vengono salvate le modifiche apportate alla timeline del progetto sulle attività principali o sul progetto.

Quando la timeline del progetto viene aggiornata, viene ricalcolata in base alle modifiche apportate al progetto, alle sue attività o alle modifiche apportate a un altro progetto da cui dipende la timeline.

Ad esempio, le seguenti modifiche alle attività del progetto attivano un aggiornamento della timeline del progetto:

* Aggiornare le date delle attività
* Modificare le relazioni predecessori delle attività
* Modificare le relazioni padre-figlio, aggiungere o rimuovere assegnazioni oltre a modificare il vincolo di attività o il tipo di durata.

## Requisiti di accesso

<!-- drafted for P&P:

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
   <td> <p>Current license: Standard</p> 
   Or
   <p>Legacy license: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

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
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica accesso a progetti</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un progetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Aggiornare il tipo di aggiornamento di un progetto

Quando le attività vengono aggiornate, i relativi oggetti principali (attività principali o progetto) vengono aggiornati al momento indicato dal tipo di aggiornamento.  Per specificare un tipo di aggiornamento per il progetto:

1. Passa al progetto di cui desideri specificare il tipo di aggiornamento.
1. Fai clic sul menu Altro ![](assets/more-icon.png) accanto al nome del progetto, fai clic su **Modifica** .

1. Fai clic su  **Progetto** **Impostazioni**.

   ![](assets/update-type-field-on-project-edit-box-nwe-350x378.png)

1. In **Tipo di aggiornamento** selezionare se si desidera che Workfront calcoli automaticamente la timeline del progetto ogni giorno, in caso di modifica o se si desidera che il project manager la calcoli manualmente.

   Seleziona dalle opzioni nell’elenco seguente. 

   >[!IMPORTANT]
   >
   >Se la timeline di un progetto ha una durata superiore a 15 anni, Workfront non calcola la timeline in modo automatico o quando cambia. Il tipo di aggiornamento di un progetto per un periodo superiore a 15 anni è sempre Manuale.

   * **Automatico e On Change:** Questa è l’impostazione predefinita. La timeline del progetto viene aggiornata ogni volta che si verifica una modifica nel progetto o in un altro progetto da cui dipende la timeline. La timeline del progetto viene aggiornata ogni notte. \
      Questa è l’impostazione consigliata in quanto assicura che la timeline del progetto sia sempre aggiornata.

      Quando si aggiorna un&#39;attività o un progetto e si attiva il ricalcolo della timeline, vengono visualizzate immediatamente tutte le date disponibili, consentendo di continuare a lavorare. Nei progetti con più di 100 attività, le date che richiedono calcoli più lunghi vengono disattivate.

      ![](assets/dates-dimmed-when-insline-editing-350x146.png)

      Questo indica che il ricalcolo non è ancora completato e che le date sono soggette a modifiche.

   * **Solo modifica:** La timeline del progetto viene aggiornata ogni volta che si verifica una modifica nel progetto o in un altro progetto da cui dipende la timeline; gli aggiornamenti pianificati non si verificano.\
      È possibile selezionare questa opzione se si è preoccupati delle prestazioni del sistema e se si verificano raramente modifiche nel progetto o in altri progetti da cui dipende la timeline.

   * **Solo automatico:** La tempistica del progetto viene aggiornata ogni notte; non viene aggiornato immediatamente dopo le modifiche.\
      È possibile selezionare questa opzione se si è preoccupati delle prestazioni del sistema e se si verificano molte modifiche quotidiane nel progetto o in altri progetti da cui dipende la timeline.

      >[!NOTE]
      >
      >Un progetto non viene ricalcolato automaticamente ogni notte se è in stato di pianificazione. Ricalcola solo al cambiamento.

   * **Solo manuale:** La timeline del progetto viene aggiornata solo quando selezioni l’opzione per **Ricalcola timeline**, come descritto nella sezione &quot;Ricalcolo manuale&quot; dell&#39;articolo [Ricalcolare le timeline dei progetti](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).\
      È possibile selezionare questa opzione se si apportano più modifiche al progetto contemporaneamente e si desidera che il ricalcolo della timeline si verifichi dopo che sono state apportate tutte le modifiche (anziché dopo ogni singola modifica).

1. Fai clic su **Salva**.
