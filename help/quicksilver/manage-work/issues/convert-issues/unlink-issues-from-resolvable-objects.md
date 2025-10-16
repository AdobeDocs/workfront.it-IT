---
product-area: projects
navigation-topic: convert-issues
title: Scollega i problemi dai loro oggetti risolutivi
description: Quando si crea un progetto o un’attività convertendo un problema in progetto o in un’attività, è possibile mantenere il problema originale. L’amministratore di Adobe Workfront deve abilitare questa preferenza affinché tu possa disporre di questa opzione durante la conversione del problema. Per ulteriori informazioni sulla conversione dei problemi in progetti e attività, consulta Panoramica sulla conversione dei problemi in Adobe Workfront.
author: Alina
feature: Work Management
exl-id: c18160e5-9f95-4575-a1b3-b4f7e5334844
source-git-commit: 0542587bb3254dec5664de493c1c321528cf7f3e
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 0%

---

# Scollega i problemi dai relativi oggetti risolutivi

<!--Audited: 08/2025-->

Quando si crea un progetto o un’attività convertendo un problema in progetto o in un’attività, è possibile mantenere il problema originale. L’amministratore di Adobe Workfront deve abilitare questa preferenza affinché tu possa disporre di questa opzione durante la conversione del problema.\
Per ulteriori informazioni sulla conversione dei problemi in progetti e attività, vedere [Panoramica sulla conversione dei problemi in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

Quando decidi di mantenere il problema convertito nel progetto o nell’attività, la sua risoluzione è associata al progetto o all’attività. Il problema diventa l’oggetto risolvibile del progetto o dell’attività. Il progetto o l&#39;attività sono gli oggetti risolutivi del problema.

Puoi anche collegare manualmente un problema a un altro. Il secondo problema diventa l’oggetto risolutivo per il primo problema, in questo caso.\
Per ulteriori informazioni sulla risoluzione di oggetti, vedere [Panoramica sulla risoluzione e la risoluzione di oggetti](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

>[!TIP]
>
>Non è possibile modificare lo stato del problema, poiché cambia automaticamente con lo stato dell&#39;oggetto risolutivo.

È possibile scollegare la risoluzione di un problema da quella di un progetto, attività o problema rimuovendo il progetto, l’attività o il problema dal problema.

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
   <td> <p>Collaboratore o versione successiva</p>
   <p>Richiedi o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazione del livello di accesso</td> 
   <td> <p>Modifica l'accesso alle Issues</p> <p>Visualizza accesso ad attività e progetti</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni sul problema</p> <p>Visualizza autorizzazioni per l'attività o il progetto</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
   <td> <p>Request or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to Issues</p> <p>View access to Tasks and&nbsp;Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions on the issue</p> <p>View permissions on the task or project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Scollegare un problema da un progetto, un’attività o un problema

1. Passa al problema collegato a un progetto, un’attività o un problema.
1. Fai clic sulla sezione **Dettagli problema**.
1. Vai all&#39;area **Panoramica** della sezione **Dettagli problema**.
1. Nel campo **Risolto da**, rimuovere il tipo di oggetto risolvibile.\
   Un problema può essere risolto da un progetto, un’attività o un problema.

   Questo rimuove l’oggetto di risoluzione dal problema.

1. Fai clic su **Salva** **Modifiche**.\
   Il problema non è più collegato a un progetto, un’attività o un problema e ora puoi risolverlo in modo indipendente.
