---
product-area: projects
navigation-topic: update-work-in-a-project
title: Aggiorna stato attività
description: È possibile aggiornare lo stato di un'attività per informare gli altri su dove si trova l'attività (e sul progetto complessivo) e come si sta muovendo.
author: Alina
feature: Work Management
exl-id: e1efc676-e110-486e-91dc-f521421575e8
source-git-commit: 6bb6b834c5af8ad48179fc0d60b184d083b360e4
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 1%

---

# Aggiorna stato attività

È possibile aggiornare lo stato di un&#39;attività per informare gli altri su dove si trova l&#39;attività (e sul progetto complessivo) e come si sta muovendo.

Gli stati predefiniti sono Nuovo, In corso e Completa. L’amministratore Adobe Workfront può aggiungere stati personalizzati per la tua organizzazione. Per ulteriori informazioni, consulta [Creare o modificare uno stato](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

È possibile aggiornare manualmente gli stati delle attività oppure consentire a Workfront di aggiornarli automaticamente quando si verificano determinate azioni.

## Requisiti di accesso

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard</p> 
   Or
   <p>Legacy license: Work or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the task</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Per aggiornare manualmente le attività, è necessario disporre del seguente accesso:

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
   <td> <p>Modifica accesso alle attività</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per l’attività</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Aggiorna manualmente lo stato dell&#39;attività

Quando si aggiorna lo stato di un&#39;attività, è inoltre possibile digitare una spiegazione sul nuovo stato e modificare altre informazioni sull&#39;attività, ad esempio la data di scadenza.

1. Passare a un&#39;attività a cui si desidera aggiornare lo stato.
1. Fai clic sul pulsante **Stato** nell&#39;intestazione dell&#39;attività e selezionare un nuovo stato.
1. (Facoltativo) Effettua una delle seguenti operazioni per fornire informazioni aggiuntive sull&#39;aggiornamento, quindi fai clic su **Aggiorna** o, se l’attività ha **Completa** stato, fai clic su **Fatto:**

   * Per aggiungere una nota sull&#39;aggiornamento, vai alla sezione **Aggiornamenti** area e fai clic su **Avvia un nuovo aggiornamento**, quindi digita la nota.

   * Per informare alcuni utenti dell’aggiornamento, digita i loro nomi nel **Notifica** casella visualizzata quando si digita una nota relativa all&#39;aggiornamento. Per ulteriori informazioni, consulta [Assegnare tag agli altri utenti in caso di aggiornamenti](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).
   * Per aggiornare la condizione dell&#39;attività, fare clic su **Seleziona condizione** a destra del **Notifica** Questa casella viene visualizzata quando si digita una nota sull&#39;aggiornamento, quindi selezionare la condizione che riflette al meglio la condizione corrente dell&#39;attività.

   * Per aggiornare la data di commit dell&#39;attività, espandere la **Data impegno** calendario a discesa e selezionare una nuova data di commit.
   * Per fornire un&#39;indicazione visiva del completamento dell&#39;attività, trascinare la bolla sotto Percentuale completata o fare doppio clic su di essa per immettere un valore percentuale.\
      ![](assets/drag-the-progress-bar-350x155.png)

## Aggiorna automaticamente lo stato dell&#39;attività

Workfront aggiorna automaticamente lo stato esistente di un&#39;attività a uno stato diverso quando si verificano le azioni elencate nella tabella seguente.

>[!NOTE]
>
>Gli stati nella tabella seguente sono stati predefiniti del sistema. L’amministratore di Workfront o un amministratore di gruppo può rinominare gli stati nell’istanza di Workfront. Per informazioni sulla creazione e la gestione degli stati in Workfront, consulta [Creare o modificare uno stato](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Azione</td> 
   <td>Stato originale</td> 
   <td>Nuovo stato</td> 
  </tr> 
  <tr> 
   <td>Aggiorna la percentuale di completamento dell'attività al 100%</td> 
   <td>Novità o in corso</td> 
   <td>Completato</td> 
  </tr> 
  <tr> 
   <td>Aggiorna la percentuale di completamento dell'attività dal 100% a un numero inferiore</td> 
   <td>Completato</td> 
   <td>In corso</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>Fare clic sul pulsante Avvia attività per accettare di lavorare su un'attività assegnata</span> </td> 
   <td><span>Nuovo</span> </td> 
   <td> <p>Qualsiasi stato associato al pulsante Start Task nelle impostazioni Home Team.</p> <p>Per informazioni sulla sostituzione del pulsante Lavora su di esso con un pulsante Avvia attività, vedere <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Sostituire il pulsante Work On It con un pulsante Start</a></span>.</p> <p>Suggerimento: <span>Clic</span> <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">Pulsante Annulla</span>dopo aver fatto clic su Avvia attività, lo stato viene ripristinato su Nuovo. </p> </td> 
  </tr> 
 </tbody> 
</table>
