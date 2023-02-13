---
product-area: projects
navigation-topic: use-predecessors
title: Creare una relazione predecessore nell'elenco delle attività
description: È possibile utilizzare le attività predecessori (o solo i predecessori) per collegare le attività che dipendono da altre attività da avviare o completare. Ad esempio, non si desidera ospitare una parte (attività dipendente) prima di inviare gli inviti (attività predecessore).
author: Alina
feature: Work Management
exl-id: a84d88ac-8dd4-4952-b83f-02fafa61e68b
source-git-commit: 420ba180dd0bfd53514c58f77ca9897ba9797320
workflow-type: tm+mt
source-wordcount: '640'
ht-degree: 0%

---

# Creare una relazione predecessore nell&#39;elenco delle attività

È possibile utilizzare le attività predecessori (o solo i predecessori) per collegare le attività che dipendono da altre attività da avviare o completare. Ad esempio, non si desidera ospitare una parte (attività dipendente) prima di inviare gli inviti (attività predecessore).

Questo articolo illustra come creare predecessori nell&#39;elenco delle attività.

È possibile visualizzare i predecessori delle attività nelle seguenti aree di Adobe Workfront:

* Nell&#39;elenco delle attività della colonna Predecessori.
* Nel diagramma di Gantt
* Nella sezione Predecessori di un&#39;attività dipendente

Per ulteriori informazioni, consulta [Panoramica dei predecessori delle attività](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Requisiti di accesso

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
   <td> <p>Modifica l’accesso a Attività e Progetti</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestisci le autorizzazioni per le attività e il progetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Creare un predecessore

1. Vai a un progetto.
1. Fai clic su **Attività** nel pannello a sinistra.
1. Assicurati che nella visualizzazione corrente sia visualizzata la **Predecessore** colonna.

   Se nella visualizzazione non viene visualizzata la colonna Predecessori, modificare una visualizzazione corrispondente o aggiungere la colonna alla visualizzazione.

1. Selezionare l&#39;attività da designare come attività dipendente.
1. Fai clic all’interno del **Predecessori** colonna.
1. Digitare il numero dell&#39;attività da designare come predecessore dell&#39;attività selezionata, quindi premere **Invio**.

   L&#39;icona predecessore diventa verde quando l&#39;attività predecessore è contrassegnata come completata. Questo indica che l&#39;attività dipendente è pronta per il lavoro.

   Per ulteriori informazioni sui tipi di relazione disponibili nella colonna Predecessori, vedere [Panoramica dei predecessori delle attività](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md) in [Panoramica dei predecessori delle attività](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Visualizza dettagli predecessore

È possibile visualizzare rapidamente i dettagli del predecessore dall&#39;elenco delle attività.

1. Nell’elenco delle attività, passa il puntatore del mouse sul numero del predecessore nel **Predecessori** colonna.

   Viene visualizzata una casella con i dettagli del predecessore.

   ![Dettagli predecessore](assets/predecessor-details-in-task-list.png)

   Vengono visualizzati i seguenti dettagli:

   **Nome predecessore:** Nome del predecessore a cui viene fatto riferimento. È incluso il numero dell&#39;attività del predecessore. Fare clic sul nome dell&#39;attività per aprirla. Nell’esempio precedente, il predecessore è Produzione/Esecuzione/Consegna.

   **Nome progetto:** Nome del progetto in cui risiede il predecessore. Il progetto viene identificato come progetto corrente se il predecessore appartiene agli stessi progetti dell’attività o come progetto incrociato, se il predecessore appartiene a un progetto diverso. Nell’esempio precedente, il nome del progetto è Digital Asset Production (Integrated) - Project. Per ulteriori informazioni sui predecessori tra progetti, consulta [Creare predecessori tra progetti](../../tasks/use-prdcssrs/cross-project-predecessors.md).

   È possibile espandere i dettagli del progetto per visualizzare le date di inizio e fine pianificate del progetto, la relativa condizione, lo stato, la percentuale di completamento e il proprietario. Per un progetto trasversale, potete quindi fare clic su **Vedi Progetto** per aprire il progetto.

   **ID:** Numero di riferimento del progetto in cui si trova il predecessore.

   **Inizio pianificato:** Data inizio pianificata dell&#39;attività predecessore.

   **Fine pianificata:** Data di completamento pianificata dell&#39;attività predecessore.

   **Numero di predecessori:** Numero di predecessori del predecessore a cui si fa riferimento. Nell&#39;esempio precedente, il predecessore a cui si fa riferimento ha un predecessore.

   **Numero di successori:** Numero di attività successive (o dipendenti) per il predecessore a cui si fa riferimento. Nell&#39;esempio precedente, il predecessore a cui si fa riferimento ha 1 successore.
