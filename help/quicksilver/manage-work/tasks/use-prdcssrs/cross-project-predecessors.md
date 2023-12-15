---
product-area: projects
navigation-topic: use-predecessors
title: Creare predecessori per più progetti
description: Un predecessore di Progetto Incrociato è un'attività da cui dipende un'altra attività (denominata attività successore) in un altro progetto. Il predecessore è l'attività che ha la priorità rispetto all'attività dipendente (successore). Ad esempio, è possibile creare una relazione che richiede che l'attività predecessore sia contrassegnata come Completa prima che l'attività dipendente possa iniziare.
author: Alina
feature: Work Management
exl-id: 7e29e589-e0a5-437e-935d-d5bc1b268594
source-git-commit: 4e3cafafb121371249fb73f2f001477bdbad2d77
workflow-type: tm+mt
source-wordcount: '766'
ht-degree: 0%

---

# Creare predecessori per più progetti

<!--Audited: 12/2023-->

Un predecessore di un progetto incrociato è un&#39;attività da cui dipende un&#39;altra attività (denominata attività successore) in un altro progetto. Il predecessore è l&#39;attività che ha la priorità rispetto all&#39;attività dipendente (successore). Ad esempio, è possibile creare una relazione che richiede che l&#39;attività predecessore sia contrassegnata come Completa prima che l&#39;attività dipendente possa iniziare.

Adobe Workfront consente di far dipendere le attività da quelle di altri progetti, proprio come permette ai predecessori all’interno di un singolo progetto.

>[!INFO]
>
>Ad esempio, una società di scavi dispone di una sola backhoe e due progetti hanno attività che richiedono l&#39;utilizzo della backhoe. Il project manager può impostare l&#39;attività del primo progetto come predecessore dell&#39;attività del secondo progetto. Questo mostra che il secondo progetto può iniziare a utilizzare la backhoe al termine del primo progetto.

Quando si collegano progetti tramite predecessori di progetti incrociati, le date del progetto principale (quello che ha l&#39;attività predecessore) influiranno sul progetto secondario (quello che ha l&#39;attività successore).

>[!TIP]
>
>Per visualizzare le date aggiornate per il progetto secondario, è necessario ricalcolare le tempistiche dei progetti. Per ulteriori informazioni sul ricalcolo delle timeline, consulta [Configurare i ricalcoli della sequenza temporale per i progetti](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

Per ulteriori informazioni sulle relazioni predecessori, vedere [Panoramica dei predecessori delle attività](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Requisiti di accesso

<!--drafted - replace table for P&P:

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
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the tasks and the projects</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

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
  <td> <p>Nuovo: Standard </p>
 <p>oppure</p> 
<p>Corrente: Piano </p> 
</td> 
 </tr>   <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modifica accesso ad attività e progetti</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per le attività e i progetti</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

## Creare un predecessore per più progetti

1. Vai all’attività che sarà il tuo successore (attività dipendente).
1. Clic **Predecessori** nel pannello a sinistra.
1. Clic **Aggiungi Predecessore.**
1. In **Progetto principale** , inizia a digitare il nome del progetto che contiene l&#39;attività che si desidera sia il predecessore dell&#39;attività corrente.
1. Fare clic sul nome quando viene visualizzato nell&#39;elenco a discesa.
1. In **Attività** , inizia a digitare il nome dell&#39;attività che dovrà essere il predecessore dell&#39;attività corrente.
1. Specificare le informazioni seguenti per definire la relazione tra il predecessore e l&#39;attività dipendente:

   * **Tipo di dipendenza:** Selezionare la relazione che l&#39;attività predecessore deve avere con l&#39;attività dipendente. La relazione predefinita è &quot;Finish-Start&quot;, ovvero l&#39;attività predecessore deve terminare prima che l&#39;attività dipendente possa iniziare. Per ulteriori informazioni sui vari tipi di dipendenza, vedere [Panoramica dei tipi di relazione tra attività](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md)

   * **Lag:** Specificare il tempo che deve trascorrere dopo il completamento di un predecessore imposto fino a quando l&#39;attività dipendente può iniziare. Per ulteriori informazioni sui vari tipi di ritardo, consulta [Panoramica sui tipi di ritardo](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

   * **Imposto:** Quando questa opzione è selezionata, la relazione di dipendenza tra le due attività non può essere aggirata dagli utenti che iniziano le attività in anticipo. Se, ad esempio, si applica una relazione tra l&#39;Attività A e l&#39;Attività B, l&#39;Attività B non può essere avviata fino al completamento dell&#39;Attività A. Per ulteriori informazioni sull&#39;applicazione dei predecessori, vedere [Imponi predecessori](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

     Quando questa opzione non è selezionata, la dipendenza viene trattata come un suggerimento agli utenti. Ad esempio, gli utenti possono avviare l&#39;Attività B prima del completamento dell&#39;Attività A.

1. Fai clic su **Salva**.

   Le attività con un predecessore per più progetti visualizzano il numero di riferimento del progetto a cui appartiene il predecessore e il numero dell&#39;attività, separati da due punti, nella colonna Predecessori di un elenco di attività.

   ![Predecessore tra progetti](assets/cross-project-predecessor-in-list-view.png)

   L&#39;icona del predecessore diventa verde quando l&#39;attività predecessore è contrassegnata come completata. Questo indica che l&#39;attività dipendente è pronta per il lavoro.

   Passa il cursore del mouse su questo valore per ottenere ulteriori informazioni sul predecessore, sul progetto e sulle date. Fai clic sul predecessore tra progetti nella casella dei dettagli per aprire l’attività.

   Fai clic su accanto alla parte superiore della finestra che compare al passaggio del mouse per visualizzare ulteriori informazioni sul progetto del predecessore.

   Clic **Vedi Progetto** per aprire il progetto del predecessore.

   ![Dettagli predecessore di più progetti](assets/cross-project-predecessor-details.png)

   >[!TIP]
   >
   >   Il **Vedi Progetto** Questa opzione è visibile solo quando si visualizza un predecessore per più progetti.

