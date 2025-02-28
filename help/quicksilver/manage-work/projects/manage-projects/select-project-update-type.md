---
product-area: projects
navigation-topic: manage-projects
title: Seleziona il tipo di aggiornamento del progetto
description: Selezionando un Tipo di aggiornamento per un progetto, è possibile controllare la frequenza con cui le modifiche apportate alla sequenza temporale del progetto vengono salvate nelle attività padre o nel progetto.
author: Alina
feature: Work Management
exl-id: ffdfffec-d217-4daa-9849-cb0c794992c0
source-git-commit: f21fd0761d942916039f6364e62f489a07217bfe
workflow-type: tm+mt
source-wordcount: '710'
ht-degree: 0%

---

# Seleziona il tipo di aggiornamento del progetto

Selezionando un Tipo di aggiornamento per un progetto, è possibile controllare la frequenza con cui le modifiche apportate alla sequenza temporale del progetto vengono salvate nelle attività padre o nel progetto.

Quando la sequenza temporale del progetto viene aggiornata, viene ricalcolata in base alle modifiche apportate al progetto, alle relative attività o alle modifiche apportate a un altro progetto da cui dipende la sequenza temporale.

Ad esempio, le seguenti modifiche alle attività del progetto attivano un aggiornamento della timeline  del progetto:

* Aggiornare le date delle attività
* Modificare le relazioni dei predecessori delle attività
* Consente di modificare le relazioni padre-figlio, aggiungendo o rimuovendo assegnazioni e modificando il vincolo attività o il tipo di durata.

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
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modifica accesso ai progetti</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un progetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

## Aggiornare il tipo di aggiornamento di un progetto

Quando le attività vengono aggiornate, gli oggetti padre (attività padre o progetto) vengono aggiornati all&#39;ora indicata dal Tipo di aggiornamento.  Per specificare un tipo di aggiornamento per il progetto:

1. Vai al progetto di cui desideri specificare il Tipo di aggiornamento.
1. Fai clic sull&#39;icona Altro ![Altro](assets/more-icon.png) accanto al nome del progetto, quindi fai clic su **Modifica** .

1. Fare clic su **Progetto** **Impostazioni**.

   ![](assets/update-type-field-on-project-edit-box-nwe-350x378.png)

1. Nel campo **Tipo di aggiornamento**, selezionare se si desidera che Workfront calcoli automaticamente la sequenza temporale del progetto ogni giorno, quando viene apportata una modifica oppure se si desidera che il project manager la calcoli manualmente.

   Seleziona tra le opzioni nell’elenco seguente. 

   >[!IMPORTANT]
   >
   >Se la timeline di un progetto è più lunga di 15 anni, Workfront non la calcola automaticamente o in caso di modifica. Il tipo di aggiornamento di un progetto di durata superiore a 15 anni è sempre Manuale.

   * **Automatico e alla modifica:** Questa è l&#39;impostazione predefinita. La timeline del progetto viene aggiornata ogni volta che si verifica una modifica nel progetto o in un altro progetto da cui dipende. Anche la timeline del progetto viene aggiornata ogni notte. \
     Si tratta dell’impostazione consigliata in quanto garantisce che la timeline del progetto sia sempre aggiornata.

     Quando si aggiorna un&#39;attività o un progetto e si attiva un ricalcolo della sequenza temporale, tutte le date disponibili vengono visualizzate immediatamente, consentendo di continuare a lavorare. Nei progetti con più di 100 attività, le date che richiedono calcoli più lunghi vengono disattivate.

     ![](assets/dates-dimmed-when-insline-editing-350x146.png)

     Questo indica che il ricalcolo non è ancora terminato e che le date sono soggette a modifiche.

   * **Solo modifica:** la sequenza temporale del progetto viene aggiornata ogni volta che si verifica una modifica nel progetto o in un altro progetto da cui dipende la sequenza temporale. Gli aggiornamenti pianificati non vengono eseguiti.\
     È possibile selezionare questa opzione se si è preoccupati delle prestazioni del sistema e se raramente si verificano modifiche nel progetto o in altri progetti da cui dipende la sequenza temporale.

   * **Solo automatico:** La sequenza temporale del progetto viene aggiornata ogni notte e non viene aggiornata immediatamente dopo le modifiche apportate.\
     È possibile selezionare questa opzione se si è preoccupati delle prestazioni del sistema e se si verificano molte modifiche ogni giorno nel progetto o in altri progetti da cui dipende la sequenza temporale.

     >[!NOTE]
     >
     >Un progetto non viene ricalcolato automaticamente ogni notte se si trova nello stato Pianificazione. Viene ricalcolato solo in seguito a modifica.

   * **Solo manuale:** la sequenza temporale del progetto viene aggiornata solo quando si seleziona l&#39;opzione **Ricalcola sequenze temporali**, come descritto nella sezione &quot;Ricalcolo manuale&quot; nell&#39;articolo [Ricalcola sequenze temporali del progetto](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).\
     È possibile selezionare questa opzione se si apportano contemporaneamente molte modifiche al progetto e si desidera che il ricalcolo della sequenza temporale venga eseguito dopo che tutte le modifiche sono state apportate (anziché dopo ogni singola modifica).

1. Fai clic su **Salva**.
