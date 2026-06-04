---
product-area: projects
navigation-topic: use-predecessors
title: Creare una relazione predecessore nell’elenco delle attività
description: È possibile utilizzare le attività predecessore (o solo i predecessori) per collegare attività che dipendono da altre attività per iniziare o completare. Ad esempio, non si desidera ospitare una parte (attività dipendente) prima di inviare gli inviti (attività predecessore).
author: Alina
feature: Work Management
exl-id: a84d88ac-8dd4-4952-b83f-02fafa61e68b
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/g3YIX403qRoqtgg5KmQW2c2lRKr9Mlg-DIc9uFGphPs
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
source-wordcount: 628
ht-degree: 9%

---

# Creare una relazione predecessore nell’elenco delle attività

<!-- Audited: 5/2025 -->

È possibile utilizzare le attività predecessore (o solo i predecessori) per collegare attività che dipendono da altre attività per iniziare o completare. Ad esempio, non si desidera ospitare una parte (attività dipendente) prima di inviare gli inviti (attività predecessore).

In questo articolo viene illustrato come creare predecessori nell&#39;elenco delle attività.

Puoi visualizzare i predecessori delle attività nelle seguenti aree di Adobe Workfront:

* Nell&#39;elenco delle attività nella colonna Predecessori.
* Nel diagramma di Gantt.
* Nella sezione Predecessori di un&#39;attività dipendente.

Per ulteriori informazioni, consulta [Panoramica dei predecessori delle attività](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

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

<!--
Old:

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
   <td> <p>Standard </p><p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the tasks and the project</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

## Creare un predecessore

{{step1-to-projects}}

1. Selezionare un progetto nella pagina **Progetti**.
1. Fai clic su **Attività** nel pannello a sinistra.
1. Nel menu a discesa **Visualizzazioni**, seleziona una visualizzazione che visualizzi la colonna **Predecessore** oppure aggiungi la colonna alla visualizzazione corrente.

1. Selezionare l&#39;attività da designare come attività dipendente.
1. Fai clic all&#39;interno della colonna **Predecessori** dell&#39;attività.
1. Digitare il numero dell&#39;attività da designare come predecessore dell&#39;attività selezionata, quindi premere **Invio**.

   >[!TIP]
   >
   >Per aggiungere un predecessore per più progetti, effettuate le seguenti operazioni:
   >
   >1. Fare clic sull&#39;icona **Modalità pianificazione** e scegliere **Salvataggio automatico**.
   >
   >1. Digita il Numero di riferimento del progetto del predecessore seguito da due punti e dal numero dell’attività. Digitare ad esempio *765021:12* indica che il numero di riferimento del progetto del predecessore è 765021 e che il predecessore è l&#39;attività numero 12 nel progetto.
   >
   >1. Aggiungi il tipo di dipendenza per questo predecessore. Per ulteriori informazioni, consulta [Creare predecessori tra progetti](/help/quicksilver/manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).
   >
   >1. Premere **Invio**.
   >
   >**IMPORTANTE**
   >
   >Non puoi aggiungere un predecessore per più progetti quando l’elenco delle attività viene visualizzato in modalità Salvataggio manuale.

   L&#39;icona del predecessore diventa verde quando l&#39;attività predecessore è contrassegnata come completata. Questo indica che l&#39;attività dipendente è pronta per il lavoro.

   Per ulteriori informazioni sui tipi di relazione disponibili nella colonna Predecessori, vedere [Panoramica sui predecessori delle attività](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Visualizza dettagli predecessore

È possibile visualizzare rapidamente i dettagli sul predecessore dall&#39;elenco delle attività.

1. Nell&#39;elenco delle attività, passa il cursore sul numero del predecessore nella colonna **Predecessori**. Viene visualizzata una casella con i dettagli del predecessore.

   ![Dettagli predecessore](assets/predecessor-details-in-task-list.png)

   Vengono visualizzati i seguenti dettagli:

   **Nome predecessore:** Il nome del predecessore a cui si fa riferimento. È incluso il numero dell’attività del predecessore. Fare clic sul nome dell&#39;attività per aprirla.

   **Nome progetto:** Il nome del progetto in cui risiede il predecessore. Il progetto viene identificato come progetto corrente se il predecessore appartiene agli stessi progetti dell&#39;attività oppure come progetto incrociato se il predecessore appartiene a un progetto diverso. Per ulteriori informazioni sui predecessori tra progetti, vedi [Creare predecessori tra progetti](../../tasks/use-prdcssrs/cross-project-predecessors.md).

   Puoi espandere i dettagli del progetto per visualizzare le date di inizio e fine pianificate del progetto, la condizione, lo stato, la percentuale di completamento e il proprietario. Per un progetto incrociato, puoi quindi fare clic su **Visualizza progetto** per aprire il progetto.

   **ID:** Il numero di riferimento del progetto in cui si trova il predecessore.

   **Inizio pianificato:** Data di inizio pianificata dell&#39;attività predecessore.

   **Fine pianificata:** la data di completamento pianificata dell&#39;attività predecessore.

   **Numero di predecessori:** Numero di predecessori a cui si fa riferimento per il predecessore.

   **Numero di successori:** Numero di attività successore (o dipendenti) per il predecessore a cui si fa riferimento.
