---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "Visualizza: calcolare le differenze di data e ora"
description: 'È possibile calcolare la differenza tra i seguenti valori: MODIFICAMI.'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 548dd91f-02bc-43ed-8322-d0facf3488f0
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '650'
ht-degree: 0%

---

# Visualizza: calcolo delle differenze di data e ora

>[!IMPORTANT]
>
>Non puoi calcolare la differenza di data e ora in Adobe Workfront tra due oggetti diversi dello stesso tipo. Ad esempio, non è possibile calcolare la differenza di data e ora tra due date su due progetti, attività o problemi diversi.

Puoi calcolare la differenza tra i seguenti:

* Differenza di data e ora tra due campi data sullo stesso oggetto
* Differenza di data e ora tra il campo di un oggetto e un altro campo dell&#39;oggetto padre

>[!TIP]
>
>Questi calcoli visualizzano il numero di giorni tra le due date. Il risultato viene visualizzato in giorni. Viene considerata anche la marca temporale nel campo data e il numero di giorni potrebbe essere seguito da decimali se le marche temporali non corrispondono. Se l&#39;attività è stata completata in ritardo, il numero di giorni viene visualizzato come valore negativo.

## Requisiti di accesso

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
   <td> <p>Richiesta di modifica di una vista </p>
   <p>Pianificare la modifica di un rapporto</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari per modificare un rapporto</p> <p>Modificare l'accesso a Filtri, Viste, Raggruppamenti per modificare una vista</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

## Calcola la differenza di data e ora tra due campi data sullo stesso oggetto

È ad esempio possibile calcolare la differenza tra la data di completamento pianificata e la data di completamento effettiva di un&#39;attività.

![](assets/view-planned-actual-completion-dates-datediff-column-350x92.png)

1. Consente di passare a un elenco di attività.
1. Dalla sezione **Visualizza** menu a discesa, fai clic su **Nuova visualizzazione**.

1. Clic **Aggiungi colonna** e inizia a digitare &quot;Data di completamento pianificata&quot; nel **Mostra in questa colonna** quindi selezionarlo quando viene visualizzato nell&#39;elenco.

1. Clic **Aggiungi colonna** e inizia a digitare &quot;Data di completamento effettiva&quot; nel **Mostra in questa colonna** quindi selezionarlo quando viene visualizzato nell&#39;elenco.

1. Clic **Aggiungi colonna**, quindi fai clic su **Passa alla modalità testo**.

1. Passa il puntatore del mouse sull’area della modalità testo e fai clic su **Fare clic per modificare il testo**.
1. Rimuove il testo trovato in **Modalità testo** e sostituirlo con il seguente codice:

   ```
   displayname=Planned-Actual Completion Date<br>linkedname=direct<br>querysort=plannedCompletionDate<br>textmode=true<br>valueexpression=ROUND(DATEDIFF({plannedCompletionDate},{actualCompletionDate}),2)<br>valueformat=HTML
   ```

1. Clic **Salva**, quindi **Salva visualizzazione**.

## Calcola la differenza di data e ora tra il campo di un oggetto e un altro campo di un oggetto padre

Per un elenco degli oggetti e dei relativi elementi padre, vedere la sezione &quot;Informazioni sull&#39;interdipendenza e sulla gerarchia degli oggetti&quot; in [Comprendere gli oggetti in Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).\
È ad esempio possibile calcolare la differenza tra la data di completamento pianificata di un&#39;attività e la data di completamento pianificata dell&#39;attività padre o del progetto a cui appartiene l&#39;attività.

![](assets/view-project-planned-task-planned-completion-dates-datediff-column-350x184.png)

1. Consente di passare a un elenco di attività.
1. Dalla sezione **Visualizza** menu a discesa, fai clic su **Nuova visualizzazione**.

1. Clic **Aggiungi colonna** e inizia a digitare &quot;Data di completamento pianificata del progetto&quot; o &quot;Data di completamento principale&quot; nel **Mostra in questa colonna** quindi selezionarlo quando viene visualizzato nell&#39;elenco.

1. Clic **Aggiungi colonna** e inizia a digitare &quot;Data di completamento pianificata&quot; nel **Mostra in questa colonna** quindi selezionarlo quando viene visualizzato nell&#39;elenco.

1. Clic **Aggiungi colonna**, quindi fai clic su **Passa alla modalità testo**.

1. Passa il puntatore del mouse sull’area della modalità testo e fai clic su **Fare clic per modificare il testo**.
1. Rimuove il testo trovato in **Modalità testo** e sostituirlo con uno dei seguenti codici:

   * Per visualizzare la differenza tra la data di completamento pianificata del progetto e quella dell&#39;attività:

      ```
      displayname=Project Planned Completion - Task Planned Completion (Days)<br>textmode=true<br>valueexpression=ROUND(DATEDIFF({project}.{plannedCompletionDate},{plannedCompletionDate}),2)<br>valueformat=HTML
      ```

   * Per visualizzare la differenza tra la data di completamento pianificata dell&#39;attività padre e quella dell&#39;attività:

      ```
      valueexpression=ROUND(DATEDIFF({parent}.{plannedCompletionDate},{plannedCompletionDate}),2)<br>textmode=true<br>valueformat=HTML<br>displayname=Parent Planned Completion - Planned Completion (Days)
      ```

1. Clic **Salva**, quindi **Salva visualizzazione**.
