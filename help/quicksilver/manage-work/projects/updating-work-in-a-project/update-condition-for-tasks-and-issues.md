---
product-area: projects
navigation-topic: update-work-in-a-project
title: Aggiorna condizione per attività e problemi
description: La condizione di un'attività o di un problema è un flag posizionato su di essa per indicare come sta andando. Questo è diverso dallo stato dell'elemento di lavoro, che indica lo stadio corrente dello sviluppo dell'elemento.
author: Alina
feature: Work Management
exl-id: 5d970af6-5996-4781-9b97-de02063dc32c
source-git-commit: 6bb6b834c5af8ad48179fc0d60b184d083b360e4
workflow-type: tm+mt
source-wordcount: '866'
ht-degree: 0%

---

# Aggiorna condizione per attività e problemi

La condizione di un&#39;attività o di un problema è un flag posizionato su di essa per indicare come sta andando. Questo è diverso dallo stato dell&#39;elemento di lavoro, che indica lo stadio corrente dello sviluppo dell&#39;elemento.

È possibile impostare la condizione di un&#39;attività o di un problema automaticamente o manualmente.

L’amministratore di Adobe Workfront può creare condizioni personalizzate per l’ambiente, come descritto in [Creare o modificare una condizione personalizzata](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md)

<!--You can manually update the Condition of a task or issue if you are assigned to it or if you have permissions to it, as described in the [Access requirements](#access-requirements) section of this article.-->

## Requisiti di accesso {#access-requirements}

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
   <td> 
   
   For the current licenses:
   <ul><li><p>Standard for tasks</p></li>
   <li><p>Contributor or higher for issues</p></li></ul>


   For legacy licenses:
   <ul><li><p>Work or higher for tasks</p></li>
   <li><p>Request or higher for issues</p></li></ul>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to projects</p> <p>Edit access to tasks and issues </p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions on tasks and issues to view their Condition</p>
   <p>Manage permissions on tasks and issues to update the Condition</p>
    <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
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
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Lavoro o superiore per le attività</p>
   <p>Richiesta o versione successiva di problemi</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Visualizzare o accedere in modo più rapido ai progetti</p> <p>Modificare l’accesso a attività e problemi </p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizza o autorizzazioni superiori per attività e problemi per visualizzarne la condizione</p>
   <p>Gestisci le autorizzazioni su attività e problemi per aggiornare la condizione</p>
    <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per sapere quale piano, tipo di licenza o accesso si dispone, contattare l&#39;amministratore Workfront.

## Individua lo stato delle attività e dei problemi

Le condizioni vengono visualizzate come flag associata a attività o problemi. Possono anche essere associati a un numero che può essere visualizzato nei rapporti invece che nell’etichetta. Per ulteriori informazioni sull&#39;associazione delle condizioni ai numeri, vedere [Creare o modificare una condizione personalizzata](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

È possibile individuare la condizione di attività e problemi nelle aree seguenti:

* Area Aggiornamenti attività e problemi, all’interno di un aggiornamento, quando sei assegnato all’attività o al problema.
* Rapporti ed elenchi quando si visualizza il campo Condizione in una visualizzazione o in un raggruppamento.

>[!NOTE]
>
>Quando la parola &quot;condizione&quot; viene visualizzata nel campo Nome campo di un rapporto di immissione scritture contabili, indica che la condizione di un elemento è stata aggiornata. Quando il campo Condizione viene tracciato nei rapporti Voci scritture contabili, i valori dei numeri nuovi e vecchi presentano il numero associato alla condizione anziché il nome. Se una condizione non è originariamente definita per un&#39;attività o un problema e successivamente la si aggiorna, la voce del giornale di registrazione che acquisisce l&#39;aggiornamento visualizzerà il valore del numero precedente del campo Condizione come -2.147.483.648.

## Aggiorna automaticamente la condizione aggiornando lo stato

Quando ti viene assegnato un’attività o un problema e fai clic su **Lavorare** , Avvia attività o Avvia problema o ne aggiorna lo stato, la condizione dell&#39;attività o il problema viene automaticamente modificato nella condizione predefinita associata a **Andando liscio**.

Per informazioni sull’utilizzo di una condizione personalizzata come condizione predefinita, consulta gli articoli  [Imposta una condizione personalizzata come predefinita per le attività e i problemi](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md) e [Impostare una condizione personalizzata come predefinita per i progetti](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md).

Per informazioni sulla modifica dello stato dell&#39;attività, vedere [Aggiorna stato attività](../../../manage-work/projects/updating-work-in-a-project/update-task-status.md).

Per informazioni sulla modifica dello stato del problema, consulta [Aggiorna lo stato del problema](../../../manage-work/projects/updating-work-in-a-project/update-issue-status.md).

Per informazioni sull&#39;impostazione del pulsante Work On It su un pulsante Start Task o Start Issues, vedere [Sostituire il pulsante Work On It con un pulsante Start](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).

## Aggiorna manualmente la condizione

È necessario essere assegnati a un&#39;attività o al problema oppure disporre delle autorizzazioni di gestione per potervi impostare la condizione.

L&#39;aggiornamento della condizione di un&#39;attività o di un problema varia a seconda che vi sia stata assegnata o meno:

* È possibile aggiornare la condizione nella scheda Aggiornamenti o in un elenco di attività o problemi se sono stati assegnati a loro.
* È possibile aggiornare la condizione solo in un elenco di attività o problemi se non è stato assegnato loro, ma se si dispone delle autorizzazioni di gestione per tali attività. In questo caso, non è possibile aggiornare la condizione nella scheda Aggiorna dell&#39;attività o del problema.

Per impostare manualmente la condizione di un&#39;attività o di un problema:

1. Passa a un&#39;attività o a un problema assegnato all&#39;utente per il quale desideri impostare la condizione.

   Oppure

   Vai a un elenco di attività o problemi a cui hai le autorizzazioni di gestione ma che non ti sono assegnate.

1. Modificare la condizione del problema o dell&#39;attività come segue:

   * Se sei assegnato all’attività o al problema e disponi delle autorizzazioni di gestione, nella **Aggiornamenti** scheda , fai clic su **Avvia un nuovo aggiornamento**, seleziona **Condizione** che rifletta nel modo migliore l&#39;esecuzione dell&#39;attività, digitare il motivo per la modifica della condizione in **Avvia un nuovo aggiornamento** area (facoltativa) , quindi fai clic su **Aggiorna**.

      ![](assets/change-condition-update-comment-350x141.png)

      >[!NOTE]
      >
      >Le condizioni possono essere personalizzate per il tuo ambiente, quindi potresti trovare più di tre opzioni per Condition nel tuo ambiente. I nomi delle Condizioni potrebbero essere diversi da quelli sopra elencati. Per informazioni sulla personalizzazione delle condizioni in Workfront, consulta [Creare o modificare una condizione personalizzata](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

      Per informazioni sulle funzionalità aggiuntive disponibili durante l&#39;aggiornamento di un elemento di lavoro, vedere [Aggiorna lavoro](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

      <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><p>(NOTE: drafted because I can't do this anymore)</p><p>If you have Manage permissions to the task or issue but are not assigned to it, perhaps as a project manager, add the <strong>Condition</strong> column to any view you use in a task or issue list, then set the <strong>Condition</strong> in inline edit and press Enter.</p><p><img src="assets/change-condition-in-list-view-350x142.png" style="width: 350;height: 142;"></p><p>For information about adding a column to a view, see <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Views overview in Adobe Workfront</a>.</p></li>   
     -->
