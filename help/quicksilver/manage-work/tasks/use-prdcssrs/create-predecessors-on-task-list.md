---
product-area: projects
navigation-topic: use-predecessors
title: Creare una relazione predecessore nell'elenco delle attività
description: È possibile utilizzare le attività predecessore (o solo i predecessori) per collegare attività che dipendono da altre attività per iniziare o completare. Ad esempio, non si desidera ospitare una parte (attività dipendente) prima di inviare gli inviti (attività predecessore).
author: Alina
feature: Work Management
exl-id: a84d88ac-8dd4-4952-b83f-02fafa61e68b
source-git-commit: a92c85ad5f58700138d7750423cc3d134d980a9e
workflow-type: tm+mt
source-wordcount: '642'
ht-degree: 0%

---

# Creare una relazione predecessore nell&#39;elenco delle attività

<!-- Audited: 5/2025 -->

È possibile utilizzare le attività predecessore (o solo i predecessori) per collegare attività che dipendono da altre attività per iniziare o completare. Ad esempio, non si desidera ospitare una parte (attività dipendente) prima di inviare gli inviti (attività predecessore).

In questo articolo viene illustrato come creare predecessori nell&#39;elenco delle attività.

Puoi visualizzare i predecessori delle attività nelle seguenti aree di Adobe Workfront:

* Nell&#39;elenco delle attività nella colonna Predecessori.
* Nel diagramma di Gantt.
* Nella sezione Predecessori di un&#39;attività dipendente.

Per ulteriori informazioni, vedere [Panoramica sui predecessori delle attività](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Requisiti di accesso

+++ Espandere per visualizzare i requisiti di accesso.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> <p>Standard </p><p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica accesso ad attività e progetti</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per le attività e il progetto</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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
   >1. Aggiungi il tipo di dipendenza per questo predecessore. Per ulteriori informazioni, consulta [Creare predecessori per più progetti](/help/quicksilver/manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).
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
