---
product-area: projects
navigation-topic: update-work-in-a-project
title: Applica stati al lavoro associato a un gruppo
description: Se un progetto è associato a un gruppo, è possibile applicare sia gli stati a livello di sistema che uno stato personalizzato associato a tale gruppo al progetto, all'attività o ai problemi del progetto.
author: Alina
feature: Work Management
exl-id: 7564ab6a-8ddf-4e76-8e45-d59f9cf8d38b
source-git-commit: f21fd0761d942916039f6364e62f489a07217bfe
workflow-type: tm+mt
source-wordcount: '353'
ht-degree: 0%

---

# Applica stati al lavoro associato a un gruppo

<!--
Alina, I moved this out of an admin article about statuses (Create and customize statuses)
-->

Se un progetto è associato a un gruppo, puoi applicare al progetto sia gli stati a livello di sistema che uno stato personalizzato associato a tale gruppo, oppure le attività e i problemi relativi a tale progetto. Per informazioni sugli stati dei gruppi in Adobe Workfront, vedere [Creare o modificare uno stato](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

>[!TIP]
>
>È possibile associare solo i progetti ai gruppi. I problemi e le attività ereditano il gruppo dal progetto a cui appartengono.

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
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
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
   <td> <p>Qualsiasi</p> </td> 
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
   <td> <p>Gestire le autorizzazioni per il progetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

## Aggiorna gruppo di progetti e stato

Quando si aggiorna il Gruppo per un progetto, le opzioni disponibili per lo Stato delle attività, dei problemi o del progetto cambiano in modo che corrispondano al gruppo.

1. Passare a un progetto o crearne uno nuovo, come descritto in [Creare un progetto](../../../manage-work/projects/create-projects/create-project.md).
1. Fai clic sull&#39;icona **Altro** ![Altro icona](assets/more-icon.png), quindi fai clic su **Modifica**.

1. Nella casella **Modifica progetto** visualizzata nella parte inferiore della sezione **Panoramica**, selezionare il gruppo nel menu a discesa **Gruppo**.

1. Nel menu a discesa **Stato**, seleziona lo stato personalizzato.

   >[!NOTE]
   >
   >Se si seleziona un gruppo diverso nel menu a discesa **Gruppo**, gli stati personalizzati nel menu **Stato** cambiano automaticamente in modo da essere correlati al nuovo gruppo.
   >
   >
   >![](assets/status-drop-down-expanded-with-custom-statuses-for-project-nwe.png)   >
   >

1. Seleziona lo stato del progetto. Gli stati personalizzati creati e applicati a tale gruppo vengono visualizzati nell’elenco.
