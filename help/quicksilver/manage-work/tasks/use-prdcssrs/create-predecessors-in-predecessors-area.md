---
product-area: projects
navigation-topic: use-predecessors
title: Creare una relazione predecessore utilizzando l’area Predecessori
description: È possibile utilizzare le attività predecessore (o solo i predecessori) per collegare attività che dipendono da altre attività per iniziare o completare.
author: Alina
feature: Work Management
exl-id: 68774286-da24-409a-bbd8-eb18dfe75063
TQID: https://experienceleague.adobe.com/BOZkyUl3TKCzpbjbLnUcMQZjM-1laW-TSsVptvBP-0U
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 422
ht-degree: 8%

---

# Creare una relazione predecessore utilizzando l’area Predecessori

<!-- Audited: 5/2025 -->

È possibile utilizzare le attività predecessore (o solo i predecessori) per collegare attività che dipendono da altre attività per iniziare o completare. Ad esempio, non si desidera ospitare una parte (attività dipendente) prima di inviare gli inviti (attività predecessore).

Questo articolo mostra come impostare i predecessori utilizzando la scheda Predecessori all’interno di un’attività.

Per informazioni sull&#39;impostazione dei predecessori in un elenco di attività, vedere [Creare una relazione predecessore nell&#39;elenco attività](../../../manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).

Puoi visualizzare i predecessori delle attività nelle seguenti aree di Adobe Workfront:

* Nella sezione Predecessori delle attività dipendenti
* Nel diagramma di Gantt
* Nell&#39;elenco delle attività nella colonna Predecessori

Per informazioni sui predecessori, vedere [Panoramica sui predecessori delle attività](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

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
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td><p>Standard</p> 
   <p>Piano</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica accesso ad attività e progetti</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
   <td> <p>Gestire le autorizzazioni per le attività e il progetto</p></td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creare un predecessore per un&#39;attività

La creazione di un predecessore per un&#39;attività di progetto tramite l&#39;area Predecessori è simile alla creazione di predecessori per un&#39;attività modello su un modello.

Per creare un&#39;attività predecessore per un&#39;attività di progetto:

1. Passare all&#39;attività che si desidera designare come attività dipendente.

1. Nel pannello a sinistra, fai clic su **Predecessori**.

1. Nella sezione **Predecessori**, fai clic su **Aggiungi predecessore**. Viene visualizzata la finestra di dialogo **Aggiungi predecessore**.

1. (Facoltativo) Per aggiungere un predecessore per più progetti, sostituisci il nome del progetto nel campo **Progetto principale** con un altro progetto.

   Per informazioni, consulta [Creare predecessori per più progetti](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).

   >[!TIP]
   >
   >Non è possibile creare predecessori tra modelli per le attività modello.


1. Nel campo **Attività** digitare il nome dell&#39;attività o delle attività che si desidera designare come predecessori, quindi selezionarle quando vengono visualizzate nel menu a discesa.

1. Selezionare un **tipo di dipendenza**.

   Per informazioni, vedere [Panoramica dei tipi di relazione tra attività](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. Immetti un valore di **Lag**.

   Per informazioni, vedere &#x200B;[Panoramica sui tipi di Lag](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

   ![Finestra di dialogo Aggiungi predecessore](assets/add-predecessor-dialog-box.png)

1. Selezionare la casella di controllo **Imposto** se si desidera applicare la relazione predecessore tra le due attività.

   Per informazioni, vedere [Imponi predecessori](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

1. Fai clic su **Salva**.

1. (Facoltativo) Per rimuovere un predecessore, selezionalo dall&#39;elenco dei predecessori, quindi fai clic sull&#39;icona **Rimuovi** ![Rimuovi icona](assets/remove-or-delete-icon.png).

   Il predecessore viene rimosso dall’elenco. L&#39;attività predecessore non viene eliminata dal relativo progetto.
