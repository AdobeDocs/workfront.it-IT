---
product-area: projects
navigation-topic: use-predecessors
title: Creare relazioni predecessori concatenando attività
description: In Adobe Workfront è possibile creare relazioni con i predecessori in diversi modi. Un metodo consiste nel concatenare le attività.
author: Alina
feature: Work Management
exl-id: 38ea13a5-ab95-4617-a47f-9dde5f752fb4
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 0%

---

# Creare relazioni predecessori concatenando attività

In Adobe Workfront è possibile creare relazioni con i predecessori in diversi modi. Un metodo consiste nel concatenare le attività.

Per informazioni sulle attività predecessore, vedere [Panoramica sui predecessori delle attività](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

Tramite il concatenamento delle attività, è possibile consentire al sistema di creare automaticamente le relazioni predecessori per le attività selezionate, anziché creare manualmente una relazione per ogni attività. È comunque possibile utilizzare tipi di relazione predecessore diversi tra le attività.

## Requisiti di accesso

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
   <td> <p>Modifica accesso ad attività e progetti</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per le attività e il progetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

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
