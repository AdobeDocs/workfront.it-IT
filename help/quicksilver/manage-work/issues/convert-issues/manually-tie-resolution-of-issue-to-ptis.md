---
product-area: projects
navigation-topic: convert-issues
title: Associare manualmente la risoluzione di un problema ad altri problemi, attività o progetti
description: È possibile collegare manualmente la risoluzione di un problema alla risoluzione di un progetto, un’attività o un problema senza convertire il problema. Il problema diventa uno degli oggetti risolvibili del progetto, dell'attività o del problema selezionato. In questo caso, una modifica dello stato del progetto, dell’attività o del problema determina una modifica dello stato del problema originale.
author: Alina
feature: Work Management
exl-id: f57f67cb-60b3-4a95-9963-fa339e542551
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '518'
ht-degree: 4%

---

# Collegare manualmente la risoluzione di un problema ad altri problemi, attività o progetti

<!--Audited: 08/2025-->

È possibile collegare manualmente la risoluzione di un problema alla risoluzione di un progetto, un’attività o un problema senza convertire il problema. Il problema diventa uno degli oggetti risolvibili del progetto, dell&#39;attività o del problema selezionato. In questo caso, una modifica dello stato del progetto, dell’attività o del problema determina una modifica dello stato del problema originale.

>[!TIP]
>
>Quando si associa la risoluzione di un problema alla risoluzione di un altro oggetto, non è più possibile modificare manualmente lo stato del problema originale.

Per ulteriori informazioni sulla risoluzione e la risoluzione degli oggetti, vedere [Panoramica sugli oggetti risolvibili e risolvibili](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

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
   <td><p>Collaboratore o versione successiva</p> 
   <p>Richiedi o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica l'accesso a Issues, Tasks, Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per il problema collegato a un altro problema, attività o progetto</p> <p>Visualizza o consente di accedere ad altre autorizzazioni per il problema, l'attività o il progetto aggiunto al problema esistente</p>  </td> 
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
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Request or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Issues, Tasks, Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the issue you link to another issue, task, or project</p> <p>View or higher permissions to the issue, task, or project you add to the existing issue</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Prerequisiti

Prima di iniziare, è necessario:

* Si è verificato un problema la cui risoluzione si desidera collegare alla risoluzione di un altro problema, attività o progetto

* Hai un problema, un&#39;attività o un progetto aggiuntivo

## Associare la risoluzione di un problema alla risoluzione di un altro problema, attività o progetto

1. Passare a un problema la cui risoluzione si desidera associare alla risoluzione di un altro problema o alla risoluzione di un&#39;attività o di un progetto.
1. Fai clic su **Dettagli problema** nel pannello a sinistra, quindi espandi l&#39;area **Panoramica**.

   ![Icona Dettagli problema](assets/qs-issue-details-icon-expanded-with-overview-section-350x462.png)

1. Fai clic sul campo **Risolto da** e seleziona uno dei seguenti tipi di oggetti di risoluzione:

   * **Progetto**
   * **Attività**
   * **Problema**

   A seconda dell’oggetto selezionato, vengono visualizzati i campi seguenti:

   * **Progetto risolutivo**
   * **Attività risolutiva**
   * **Problema risolutivo**

1. Inizia a digitare il nome di un progetto, attività o problema specifico nel campo **Progetto risolutivo**, **Attività** o **Problema**, quindi fai clic su di esso quando viene visualizzato nell&#39;elenco.

   >[!NOTE]
   >
   >Non è possibile collegare la risoluzione di un problema all&#39;attività o al progetto in cui si trova il problema. L&#39;attività o il progetto del problema non viene visualizzato nei campi Attività risolutiva o Attività risolutiva.


1. Fai clic su **Salva modifiche**.

   Il problema originale diventa l&#39;oggetto risolvibile per il progetto, l&#39;attività o il problema selezionato nei passaggi 4 e 5. Ciò significa che il problema originale viene completato quando viene completato l’oggetto di risoluzione (il progetto, l’attività o il problema a cui l’hai collegato).

   >[!NOTE]
   >
   >Un progetto, un&#39;attività o un problema può presentare più problemi come oggetti risolvibili.
