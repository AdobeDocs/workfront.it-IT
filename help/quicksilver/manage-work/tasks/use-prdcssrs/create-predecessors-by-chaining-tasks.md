---
product-area: projects
navigation-topic: use-predecessors
title: Creare relazioni con i predecessori tramite il concatenamento di attività
description: In Adobe Workfront è possibile creare relazioni con i predecessori in diversi modi. Un metodo consiste nel concatenare le attività.
author: Alina
feature: Work Management
exl-id: 38ea13a5-ab95-4617-a47f-9dde5f752fb4
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---

# Creare relazioni predecessori concatenando attività

In Adobe Workfront è possibile creare relazioni con i predecessori in diversi modi. Un metodo consiste nel concatenare le attività.

Per informazioni sulle attività predecessore, vedere [Panoramica sui predecessori delle attività](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

Tramite il concatenamento delle attività, è possibile consentire al sistema di creare automaticamente le relazioni predecessori per le attività selezionate, anziché creare manualmente una relazione per ogni attività. È comunque possibile utilizzare tipi di relazione predecessore diversi tra le attività.

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
   <td><p>Standard</p> 
   <p>Piano</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica accesso ad attività e progetti</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per le attività e il progetto</p></td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> 
   <p>Standard </p>
    <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the tasks and the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Attività concatenate per creare relazioni predecessori

1. Passare al progetto contenente le attività da concatenare.
1. Fai clic su **Attività** nel pannello a sinistra.
1. (Condizionale) Seleziona **Salvataggio automatico** nell&#39;angolo superiore destro dell&#39;elenco delle attività, quindi seleziona le attività da concatenare.

   ![](assets/nwe-autosave-icon-on-highlighted-350x295.png)

   >[!IMPORTANT]
   >
   >Non è possibile concatenare i task in un elenco di task quando si salvano manualmente le modifiche apportate ai task o si utilizza la modalità Pianificazione sequenza temporale per salvare i task.

1. Fare clic con il pulsante destro del mouse sulle attività selezionate, quindi scegliere **Catena**.
1. Selezionare uno dei seguenti tipi di dipendenza:

   * **Fine-Inizio**
   * **Fine-Fine**
   * **Inizio-Inizio**
   * **Inizio-Fine**

   Per ulteriori informazioni sui tipi di relazione predecessore, vedere [Panoramica sui tipi di relazione tra attività](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. (Facoltativo) Fare clic su **Rimuovi catena** se alcune attività sono state precedentemente concatenate.

   >[!CAUTION]
   >
   >Solo i predecessori sequenziali vengono rimossi utilizzando l&#39;opzione di rimozione dalla catena durante la modifica in serie delle attività.

   Le attività selezionate sono ora collegate da relazioni predecessori.
