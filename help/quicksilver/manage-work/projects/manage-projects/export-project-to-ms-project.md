---
product-area: projects
navigation-topic: manage-projects
title: Esportare un progetto in un progetto Microsoft
description: Puoi esportare i progetti Adobe Workfront in Microsoft Project.
author: Alina
feature: Work Management
exl-id: 3f0f3644-a763-4b72-a93a-85af8626b5b3
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 0%

---

# Esportare un progetto in un progetto Microsoft

Puoi esportare i progetti Adobe Workfront in Microsoft Project. 

>[!IMPORTANT]
>
>* Non tutti i campi di Workfront vengono trasferiti nel file di progetto di Microsoft.\
>  Per ulteriori informazioni sulla compatibilità dei campi tra Workfront e Microsoft Project, vedere l&#39;articolo [Mappatura dei campi di Microsoft Project ai progetti Adobe Workfront](../../../manage-work/projects/manage-projects/map-ms-project-fields-to-workfront.md).
>* È consigliabile limitare il numero di trasferimenti di progetti da un&#39;applicazione all&#39;altra. 
>

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> <p>Chiaro o superiore</p>
   <p>Revisione o successiva</p>

</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Accesso ai progetti di visualizzazione o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p> Visualizza o autorizzazioni superiori per il progetto</p></td> 
  </tr> 
 </tbody> 
</table>

*Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

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
   <td> <p>Review or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p> View or higher permissions to the project</p> <p>For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Esportare un progetto da Workfront a Microsoft Project

Puoi esportare un progetto da Workfront dalla pagina del progetto o da un elenco o rapporto di progetto.

1. Vai al progetto da esportare e fai clic sull&#39;icona **Altro** ![Altro menu](assets/qs-more-menu.png) a destra del nome del progetto

   ![Altro menu a discesa](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   Oppure

   Vai a un elenco o a un report di progetti e seleziona un progetto, quindi fai clic sull&#39;icona Altro ![Menu Altro](assets/qs-more-menu.png) nella parte superiore dell&#39;elenco.

   ![Menu Altro espanso](assets/more-menu-expanded-in-a-list-one-project-selected-nwe.png)

1. Fare clic su **Esporta MS Project**.

   Il progetto viene scaricato come file XML nel computer ed è pronto per essere importato in Microsoft Project. 
