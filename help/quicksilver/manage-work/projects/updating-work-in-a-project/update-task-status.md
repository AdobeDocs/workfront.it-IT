---
product-area: projects
navigation-topic: update-work-in-a-project
title: Aggiorna stato attività
description: È possibile aggiornare lo stato di un'attività per informare gli altri utenti sulla posizione dell'attività (e del progetto complessivo) e sull'avanzamento dell'attività.
author: Alina
feature: Work Management
exl-id: e1efc676-e110-486e-91dc-f521421575e8
source-git-commit: b02c81873d84946f8db54bcf9a1a464de38781de
workflow-type: tm+mt
source-wordcount: '681'
ht-degree: 1%

---

# Aggiorna stato attività

È possibile aggiornare lo stato di un&#39;attività per informare gli altri utenti sulla posizione dell&#39;attività (e del progetto complessivo) e sull&#39;avanzamento dell&#39;attività.

Gli stati predefiniti sono Nuovo (New), In corso (In Progress) e Completo (Complete). Il tuo amministratore Adobe Workfront può aggiungere stati personalizzati per la tua organizzazione. Per ulteriori informazioni, consulta [Creare o modificare uno stato](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

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

Per aggiornare manualmente le attività, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Lavoro o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modifica l'accesso alle Attività</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per l’attività</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

## Considerazioni sull&#39;aggiornamento dello stato delle attività

* Quando si contrassegna un&#39;attività come Completata, la percentuale di completamento dell&#39;attività viene aggiornata al 100%.
* Esistono i seguenti scenari per le attività padre:
   * Non è possibile aggiornare lo stato di un&#39;attività padre a Completo quando la modalità di completamento riepilogo del progetto è impostata su Automatico e le sottoattività non sono completate.
   * È possibile aggiornare lo stato di un&#39;attività padre impostandolo su Completo quando la modalità di completamento riepilogo del progetto è impostata su Manuale e le sottoattività sono completate o incomplete.

  Per ulteriori informazioni, consulta [Modifica progetti](../manage-projects/edit-projects.md).

## Aggiorna manualmente lo stato delle attività

Quando si aggiorna lo stato di un&#39;attività, è inoltre possibile digitare una spiegazione relativa al nuovo stato e modificare altre informazioni dell&#39;attività, ad esempio la data di scadenza.

1. Passare a un&#39;attività a cui si è assegnati per la quale si desidera aggiornare lo stato.
1. Fai clic su **Stato** nell&#39;intestazione dell&#39;attività e selezionare un nuovo stato.
1. (Facoltativo) Effettua una delle seguenti operazioni per fornire informazioni aggiuntive sull’aggiornamento, quindi fai clic su **Aggiorna** o, se l&#39;attività ha **Completa** stato, fai clic su **Fine:**

   * Per aggiungere una nota sull&#39;aggiornamento, passare alla **Aggiornamenti** e fai clic su **Avvia un nuovo aggiornamento**, quindi digita la nota.

   * Per avvisare alcuni utenti dell’aggiornamento, digita i loro nomi nel **Notifica** visualizzata quando si digita una nota sull&#39;aggiornamento. Per ulteriori informazioni, consulta [Assegna tag ad altri utenti in caso di aggiornamenti](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).
   * Per aggiornare la condizione dell&#39;attività, fare clic su **Seleziona condizione** a destra del **Notifica** (vengono visualizzate quando si digita una nota sull&#39;aggiornamento), quindi selezionare la condizione che meglio riflette la condizione corrente dell&#39;attività.

   * Per aggiornare la data di conferma dell&#39;attività, espandere **Conferma data** e selezionare una nuova Data di conferma.
   * Per fornire un’indicazione visiva del completamento dell’attività, trascina la bolla sotto Percentuale completata o fai doppio clic su di essa per immettere un valore percentuale.\
     ![](assets/drag-the-progress-bar-350x155.png)

## Aggiorna automaticamente lo stato delle attività

Workfront aggiorna automaticamente lo stato esistente di un&#39;attività a un altro stato quando si verificano le azioni elencate nella tabella seguente.

>[!NOTE]
>
>Gli stati riportati nella tabella seguente sono stati di sistema predefiniti. L’amministratore di Workfront o un amministratore di gruppo può rinominare gli stati nell’istanza di Workfront. Per informazioni sulla creazione e la gestione degli stati in Workfront, consulta [Creare o modificare uno stato](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

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
   <td>Nuovo o in corso</td> 
   <td>Completato</td> 
  </tr> 
  <tr> 
   <td>Aggiorna la percentuale di completamento dell'attività da 100% a un numero inferiore</td> 
   <td>Completato</td> 
   <td>In corso</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>Fare clic sul pulsante Avvia attività per accettare di lavorare su un'attività assegnata all'utente</span> </td> 
   <td><span>Nuovo</span> </td> 
   <td> <p>Qualsiasi stato associato al pulsante Avvia attività nelle impostazioni del team predefinito.</p> <p>Per informazioni sulla sostituzione del pulsante Lavoraci con un pulsante Avvia attività, vedere <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Sostituire il pulsante Lavoraci con un pulsante Start</a></span>.</p> <p>Suggerimento <span>Clic</span> <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">il pulsante Annulla</span>dopo aver fatto clic su Avvia attività, lo stato viene ripristinato su Nuovo. </p> </td> 
  </tr> 
 </tbody> 
</table>
