---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Conversione di portfolio legacy in Adobe Cloud Storage
description: Converti i portfolio di archiviazione legacy di Workfront in Adobe Cloud Storage dall’area Preferenze di archiviazione in Preferenze di sistema.
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 1e6380b0422efdd98449ab1e74cadb4f330917f1
workflow-type: tm+mt
source-wordcount: '358'
ht-degree: 9%

---

# Conversione di portfolio legacy in Adobe Cloud Storage

In qualità di amministratore di Workfront, puoi convertire i portfolio di archiviazione Workfront legacy esistenti in archiviazione cloud Adobe dall’area Preferenze di archiviazione in Preferenze di sistema. Una volta convertito, il portfolio si comporta come qualsiasi altro portfolio di archiviazione cloud Adobe.

Per ulteriori informazioni sul comportamento dei portfolio convertiti e sugli effetti sugli oggetti figlio, vedere [Portabilità degli oggetti](/help/quicksilver/review-and-approve-work/workfront-storage.md#object-portability) in [Passare a Workfront nell&#39;archiviazione cloud Adobe](/help/quicksilver/review-and-approve-work/workfront-storage.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td><p>Qualsiasi pacchetto flusso di lavoro</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td><p>Standard</p> <p>Piano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td>Devi essere un amministratore di Workfront. </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prima di convertire un portfolio

Prima di convertire un portafoglio di storage Workfront legacy, considera quanto segue:

* La conversione influisce solo sul portfolio stesso. I progetti e i programmi secondari che utilizzano lo storage Workfront legacy rimangono sullo storage legacy.

  >[!NOTE]
  >
  >Un programma legacy secondario viene convertito automaticamente in Adobe Cloud Storage solo quando qualcuno vi aggiunge manualmente un progetto Adobe Cloud Storage.
* I documenti e le cartelle di documenti del portfolio rimangono sullo storage legacy di Workfront dopo la conversione.
* Dopo la conversione, non è possibile aggiungere al portfolio progetti di storage Workfront legacy.

## Conversione di portfolio legacy in Adobe Cloud Storage

Per convertire uno o più portfolio di archiviazione Workfront legacy in Adobe Cloud Storage:

{{step-1-to-setup}}

1. Seleziona **Sistema** nel menu di navigazione a sinistra, quindi seleziona **Preferenze**.

1. Scorri verso il basso fino alla sezione **Preferenze di archiviazione**.

1. Nel campo **Seleziona i portfolio da convertire in Adobe Cloud Storage**, seleziona uno o più portfolio di archiviazione Workfront legacy.

1. Fai clic su **Salva**.

   Viene visualizzato un messaggio di conferma che descrive cosa accade quando un portfolio viene convertito:

   * Non è più possibile spostare i progetti di storage Workfront legacy nel portfolio.
   * Tutti i nuovi progetti creati nel portfolio utilizzano l’archiviazione cloud Adobe.
   * Frame.io è il visualizzatore di documenti nei progetti di archiviazione cloud Adobe del portfolio.
   * I progetti secondari che utilizzano lo storage legacy Workfront rimangono sullo storage legacy.
   * I programmi secondari rimangono nell&#39;archiviazione legacy.

1. Fai clic su **Converti** per confermare.

   I portfolio selezionati vengono convertiti nell’archiviazione cloud di Adobe.
