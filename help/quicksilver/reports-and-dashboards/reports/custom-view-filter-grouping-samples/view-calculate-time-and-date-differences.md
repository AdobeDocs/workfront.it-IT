---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Visualizza: calcolare le differenze di ora e data"'
description: 'È possibile calcolare la differenza tra quanto segue: MODIFICA ME.'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 548dd91f-02bc-43ed-8322-d0facf3488f0
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '633'
ht-degree: 0%

---

# Visualizza: calcolare le differenze di ora e data

>[!IMPORTANT]
>
>Non è possibile calcolare la differenza di ora e data in Adobe Workfront tra due oggetti diversi dello stesso tipo. Ad esempio, non è possibile calcolare la differenza di ora e data tra due date per due progetti, attività o problemi diversi.

Puoi calcolare la differenza tra i seguenti elementi:

* Differenza di ora e data tra due campi data sullo stesso oggetto
* Differenza di ora e data tra il campo di un oggetto e un altro campo dell&#39;oggetto principale

>[!TIP]
>
>Questi calcoli mostrano il numero di giorni tra le due date. Il risultato viene visualizzato in giorni. Viene inoltre presa in considerazione la marca temporale nel campo data, e il numero di giorni potrebbe essere seguito da decimali se le marche temporali non corrispondono. Se l’attività è stata completata in ritardo, il numero di giorni viene visualizzato come valore negativo.

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
   <td> <p>Accesso a rapporti, dashboard, calendari</p> <p>Modificare l’accesso a Filtri, Visualizzazioni, Gruppi</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Calcolare la differenza di ora e data tra due campi data sullo stesso oggetto

Ad esempio, è possibile calcolare la differenza tra la data di completamento pianificata e la data di completamento effettivo di un&#39;attività.

![](assets/view-planned-actual-completion-dates-datediff-column-350x92.png)

1. Passare a un elenco di attività.
1. Da **Visualizza** menu a discesa, fai clic su **Nuova vista**.

1. Fai clic su **Aggiungi colonna** e inizia a digitare &quot;Data completamento pianificata&quot; nel **Mostra in questa colonna** quindi selezionalo quando viene visualizzato nell’elenco.

1. Fai clic su **Aggiungi colonna** e inizia a digitare &quot;Data effettiva di completamento&quot; nel **Mostra in questa colonna** quindi selezionalo quando viene visualizzato nell’elenco.

1. Fai clic su **Aggiungi colonna**, quindi fai clic su **Passa alla modalità testo**.

1. Passa il puntatore del mouse sull’area della modalità testo e fai clic su **Fare clic per modificare il testo**.
1. Rimuovi il testo che trovi nella **Modalità testo** e sostituirlo con il seguente codice:

   ```
   displayname=Planned-Actual Completion Date<br>linkedname=direct<br>querysort=plannedCompletionDate<br>textmode=true<br>valueexpression=ROUND(DATEDIFF({plannedCompletionDate},{actualCompletionDate}),2)<br>valueformat=HTML
   ```

1. Fai clic su **Salva**, quindi **Salva visualizzazione**.

## Calcolare la differenza di ora e data tra il campo di un oggetto e un altro campo di un oggetto principale

Per un elenco degli oggetti e dei relativi elementi principali, vedere la sezione &quot;Comprensione dell’interdipendenza e della gerarchia degli oggetti&quot; in [Comprendere gli oggetti in Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).\
Ad esempio, è possibile calcolare la differenza tra la data di completamento pianificata di un&#39;attività e la data di completamento pianificata dell&#39;attività principale o del progetto su cui si trova l&#39;attività.

![](assets/view-project-planned-task-planned-completion-dates-datediff-column-350x184.png)

1. Passare a un elenco di attività.
1. Da **Visualizza** menu a discesa, fai clic su **Nuova vista**.

1. Fai clic su **Aggiungi colonna** e inizia a digitare &quot;Data completamento pianificato progetto&quot; o &quot;Data completamento padre&quot; nel **Mostra in questa colonna** quindi selezionalo quando viene visualizzato nell’elenco.

1. Fai clic su **Aggiungi colonna** e inizia a digitare &quot;Data completamento pianificata&quot; nel **Mostra in questa colonna** quindi selezionalo quando viene visualizzato nell’elenco.

1. Fai clic su **Aggiungi colonna**, quindi fai clic su **Passa alla modalità testo**.

1. Passa il puntatore del mouse sull’area della modalità testo e fai clic su **Fare clic per modificare il testo**.
1. Rimuovi il testo che trovi nella **Modalità testo** e sostituirlo con uno dei seguenti codici:

   * Per visualizzare la differenza tra la data di completamento pianificata del progetto e quella dell&#39;attività:

      ```
      displayname=Project Planned Completion - Task Planned Completion (Days)<br>textmode=true<br>valueexpression=ROUND(DATEDIFF({project}.{plannedCompletionDate},{plannedCompletionDate}),2)<br>valueformat=HTML
      ```

   * Per visualizzare la differenza tra la data di completamento pianificata dell&#39;attività padre e quella dell&#39;attività:

      ```
      valueexpression=ROUND(DATEDIFF({parent}.{plannedCompletionDate},{plannedCompletionDate}),2)<br>textmode=true<br>valueformat=HTML<br>displayname=Parent Planned Completion - Planned Completion (Days)
      ```

1. Fai clic su **Salva**, quindi **Salva visualizzazione**.
