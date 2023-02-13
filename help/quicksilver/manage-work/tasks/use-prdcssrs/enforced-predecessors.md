---
product-area: projects
navigation-topic: use-predecessors
title: Applica predecessori
description: I predecessori sono attività alle quali altri compiti dipendono per il completamento. Le relazioni predecessori influiscono sulle date di inizio e completamento delle attività e, in ultima analisi, sulla cronologia del progetto.
author: Alina
feature: Work Management
exl-id: c3242b92-9036-4770-a073-2a9c393b97fd
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 0%

---

# Applica predecessori

I predecessori sono attività alle quali altri compiti dipendono per il completamento. Le relazioni predecessori influiscono sulle date di inizio e completamento delle attività e, in ultima analisi, sulla cronologia del progetto.

Per informazioni sui predecessori, consulta [Panoramica dei predecessori delle attività](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

Impostando le relazioni predecessori tra le attività, è possibile definire il modo in cui l&#39;inizio o la fine di un&#39;attività dipendente dipende dall&#39;inizio o dalla fine delle attività predecessori. Questo viene fatto utilizzando diversi tipi di dipendenza.

Per informazioni sui tipi di dipendenza, consulta [Panoramica dei tipi di dipendenza dell&#39;attività](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

## Panoramica dei predecessori applicati

>[!IMPORTANT]
>
>È necessario applicare i predecessori per richiedere che le relazioni predecessori siano rispettate. Senza imporre i predecessori, le attività dipendenti possono iniziare e terminare indipendentemente dall&#39;inizio e dalla fine dei predecessori, indipendentemente dai tipi di dipendenza.

È possibile applicare la relazione predecessore quando si impostano i predecessori su un progetto.

Se viene applicato un predecessore, l&#39;attività successore non può iniziare prima del completamento del predecessore. Ad esempio, per applicare una relazione Fine-Inizio tra l&#39;attività A e l&#39;attività B, l&#39;attività B non può essere avviata (lo stato deve rimanere Nuovo e la percentuale di completamento deve rimanere 0%) finché l&#39;attività A non viene contrassegnata come completata. Le relazioni di applicazione si applicano a tutti i tipi di predecessori.

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
   <td> <p>Modifica l’accesso a Attività e Progetti</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestisci le autorizzazioni per le attività e il progetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Applica un predecessore a livello di attività

1. Passare all&#39;attività successore di cui si desidera applicare il predecessore.
1. Fai clic su **Predecessori** nel pannello a sinistra, quindi fai clic su **Aggiungi predecessore**. Potrebbe essere necessario fare clic su **Mostra altro**, quindi **Predecessori**.
1. (Condizionale) Per aggiungere un predecessore tra progetti diversi, rimuovi il nome del progetto nel **Progetto padre** e sostituiscilo con un altro progetto.
1. Specifica il nome dell&#39;attività o delle attività predecessori nella **Attività** campo .
1. Specifica la **Tipo di dipendenza** tra queste due attività.

   Il valore predefinito **Tipo di dipendenza** è **Fine-Inizio**.

1. Seleziona la **Impiegato** per applicare il predecessore.
1. Fai clic su **Salva**.

## Applica un predecessore in un elenco di attività

1. Passare a un elenco di attività di un progetto.
1. Da **Visualizza** menu a discesa, seleziona il **Vista standard**.

1. Prendi nota del numero di attività che definirai come predecessore.
1. Trovare l&#39;attività successore di cui si desidera applicare il predecessore.
1. In **Predecessori** inizia a immettere il numero dell&#39;attività predecessore seguita da &quot;e&quot;. Ad esempio, digitare &quot;1e&quot; per aggiungere il numero 1 dell&#39;attività come predecessore dell&#39;attività selezionata.
1. Fai clic su Invio per salvare le informazioni del predecessore per l’attività.

   ![predecessore_forzato_in_list.png](assets/predecessor-enforced-in-list-350x308.png)
