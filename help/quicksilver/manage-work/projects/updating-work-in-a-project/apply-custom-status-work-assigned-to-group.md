---
product-area: projects
navigation-topic: update-work-in-a-project
title: Applicare gli stati al lavoro associato a un gruppo
description: Se un progetto è associato a un gruppo, puoi applicare al progetto, all’attività o ai problemi relativi a tale progetto sia lo stato a livello di sistema che uno stato personalizzato associato a tale gruppo.
author: Alina
feature: Work Management
exl-id: 7564ab6a-8ddf-4e76-8e45-d59f9cf8d38b
source-git-commit: 6bb6b834c5af8ad48179fc0d60b184d083b360e4
workflow-type: tm+mt
source-wordcount: '351'
ht-degree: 0%

---

# Applicare gli stati al lavoro associato a un gruppo

<!--
Alina, I moved this out of an admin article about statuses (Create and customize statuses)
-->

Se un progetto è associato a un gruppo, puoi applicare al progetto sia lo stato a livello di sistema che uno stato personalizzato associato a tale gruppo, oppure attività e problemi relativi al progetto. Per informazioni sugli stati del gruppo in Adobe Workfront, vedi [Creare o modificare uno stato](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

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
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
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
   <td> <p>Gestisci le autorizzazioni per il progetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Aggiorna gruppo e stato del progetto

Quando si aggiorna il gruppo per un progetto, le opzioni disponibili per lo stato delle attività, dei problemi o del progetto cambiano in base al gruppo.

1. Vai a un progetto o crea un nuovo progetto, come descritto in [Creare un progetto](../../../manage-work/projects/create-projects/create-project.md).
1. Fai clic sul pulsante **Altro** icona ![](assets/more-icon.png), quindi fai clic su **Modifica**.

1. In **Modifica progetto** che viene visualizzato, vicino alla parte inferiore del **Panoramica** , seleziona il gruppo nella sezione **Gruppo** menu a discesa.

1. In **Stato** dal menu a discesa, seleziona lo stato personalizzato.

   >[!NOTE]
   >
   >Se selezioni un gruppo diverso nel **Gruppo** nel menu a discesa, gli stati personalizzati **Stato** il menu viene modificato automaticamente in modo da essere correlato al nuovo gruppo.
   >
   >
   >![](assets/status-drop-down-expanded-with-custom-statuses-for-project-nwe.png)   >

1. Seleziona lo stato del progetto. Nell’elenco vengono visualizzati gli stati personalizzati creati e applicati al gruppo.
