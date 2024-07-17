---
product-area: projects
navigation-topic: use-predecessors
title: Creare una relazione predecessore nell'elenco delle attività
description: È possibile utilizzare le attività predecessore (o solo i predecessori) per collegare attività che dipendono da altre attività per iniziare o completare. Ad esempio, non si desidera ospitare una parte (attività dipendente) prima di inviare gli inviti (attività predecessore).
author: Alina
feature: Work Management
exl-id: a84d88ac-8dd4-4952-b83f-02fafa61e68b
source-git-commit: 811eb1453c140808b0d6c5d9a3b4a0729cb16b2d
workflow-type: tm+mt
source-wordcount: '720'
ht-degree: 0%

---

# Creare una relazione predecessore nell&#39;elenco delle attività

È possibile utilizzare le attività predecessore (o solo i predecessori) per collegare attività che dipendono da altre attività per iniziare o completare. Ad esempio, non si desidera ospitare una parte (attività dipendente) prima di inviare gli inviti (attività predecessore).

In questo articolo viene illustrato come creare predecessori nell&#39;elenco delle attività.

Puoi visualizzare i predecessori delle attività nelle seguenti aree di Adobe Workfront:

* Nell&#39;elenco delle attività nella colonna Predecessori.
* Nel diagramma di Gantt
* Nella sezione Predecessori di un&#39;attività dipendente

Per ulteriori informazioni, vedere [Panoramica sui predecessori delle attività](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Nuovo: Standard </p><p>Corrente: Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modifica accesso ad attività e progetti</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per le attività e il progetto</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront. Per ulteriori informazioni sui requisiti di accesso, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Creare un predecessore

1. Vai a un progetto.
1. Fai clic su **Attività** nel pannello a sinistra.
1. Verifica che nella visualizzazione corrente sia visualizzata la colonna **Predecessore**.

   Se nella vista non viene visualizzata la colonna Predecessori, passare a una vista che la visualizza oppure aggiungere la colonna alla vista.

1. Selezionare l&#39;attività da designare come attività dipendente.
1. Fai clic su nella colonna **Predecessori**.
1. Digitare il numero dell&#39;attività da designare come predecessore dell&#39;attività selezionata, quindi premere **Invio**.

   >[!TIP]
   >
   >Per aggiungere un predecessore per più progetti, effettuate le seguenti operazioni:
   >
   >1. Fare clic sull&#39;icona **Modalità pianificazione** e scegliere **Salvataggio automatico**.
   >
   >1. Digitare il numero di riferimento del progetto del predecessore seguito dai due punti e il numero dell&#39;attività. Digitare ad esempio: 765021:12. Indica che il numero di riferimento del progetto del predecessore è 765021 e che il predecessore è il numero di attività 12 sul progetto.
   >
   >1. Aggiungi il tipo di dipendenza per questo predecessore. Per ulteriori informazioni, consulta [Creare predecessori per più progetti](/help/quicksilver/manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).
   >
   >Premere **Invio**.
   >
   >**IMPORTANTE**
   >
   >Non è possibile aggiungere un predecessore per più progetti quando l&#39;elenco delle attività viene visualizzato in modalità Salvataggio manuale.

   L&#39;icona del predecessore diventa verde quando l&#39;attività predecessore è contrassegnata come completata. Questo indica che l&#39;attività dipendente è pronta per il lavoro.

   Per ulteriori informazioni sui tipi di relazione disponibili nella colonna Predecessori, vedere [Panoramica sui predecessori delle attività](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md) in [Panoramica sui predecessori delle attività](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Visualizza dettagli predecessore

È possibile visualizzare rapidamente i dettagli sul predecessore dall&#39;elenco delle attività.

1. Nell&#39;elenco delle attività, passa il cursore sul numero del predecessore nella colonna **Predecessori**.

   Viene visualizzata una casella con i dettagli del predecessore.

   ![Dettagli predecessore](assets/predecessor-details-in-task-list.png)

   Vengono visualizzati i seguenti dettagli:

   **Nome predecessore:** Il nome del predecessore a cui si fa riferimento. È incluso il numero dell’attività del predecessore. Fare clic sul nome dell&#39;attività per aprirla. Nell’esempio precedente, il predecessore è Produzione/Esecuzione/Consegna.

   **Nome progetto:** Il nome del progetto in cui risiede il predecessore. Il progetto viene identificato come progetto corrente se il predecessore appartiene agli stessi progetti dell&#39;attività oppure come progetto incrociato se il predecessore appartiene a un progetto diverso. Nell’esempio precedente, il nome del progetto è Produzione di risorse digitali (integrata) - Progetto. Per ulteriori informazioni sui predecessori tra progetti, vedi [Creare predecessori tra progetti](../../tasks/use-prdcssrs/cross-project-predecessors.md).

   Puoi espandere i dettagli del progetto per visualizzare le date di inizio e fine pianificate del progetto, la condizione, lo stato, la percentuale di completamento e il proprietario. Per un progetto incrociato, puoi quindi fare clic su **Visualizza progetto** per aprire il progetto.

   **ID:** Il numero di riferimento del progetto in cui si trova il predecessore.

   **Inizio pianificato:** Data di inizio pianificata dell&#39;attività predecessore.

   **Fine pianificata:** la data di completamento pianificata dell&#39;attività predecessore.

   **Numero di predecessori:** Numero di predecessori a cui si fa riferimento per il predecessore. Nell’esempio precedente, il predecessore a cui si fa riferimento ha 1 predecessore.

   **Numero di successori:** Numero di attività successore (o dipendenti) per il predecessore a cui si fa riferimento. Nell’esempio precedente, il predecessore a cui si fa riferimento ha 1 successore.
