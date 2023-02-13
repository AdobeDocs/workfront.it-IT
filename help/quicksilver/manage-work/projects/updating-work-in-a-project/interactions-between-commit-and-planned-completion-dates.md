---
product-area: projects
navigation-topic: update-work-in-a-project
title: Interazioni tra la data di commit e la data di completamento pianificata
description: Sia il completamento pianificato che le date di commit indicano quando l'attività deve essere completata. Ma differiscono a causa di chi imposta ogni data.
author: Alina
feature: Work Management
exl-id: 1709c60c-ac75-48eb-9226-ec2cf556ebf0
source-git-commit: 6bb6b834c5af8ad48179fc0d60b184d083b360e4
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 1%

---

# Interazioni tra la data di commit e la data di completamento pianificata

<!--
this article has mostly information that is repeated from the articles linked from here. I left it in here for searchability's sake.
-->

Sia il completamento pianificato che le date di commit indicano quando l&#39;attività deve essere completata. Ma differiscono a causa di chi imposta ogni data.

## Panoramica della data di commit e della data di completamento pianificata

Sono presenti date di completamento e di commit pianificati sia per le attività che per i problemi.

La tabella seguente contiene informazioni sulla differenza tra le date di completamento programmato e di commit:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Conferma data</td> 
   <td> <p>La data di commit è la data in cui la persona assegnata a un'attività o a un problema stima manualmente che avrà completato l'attività o il problema.</p> <p>Per informazioni sulle date di commit, vedi <a href="../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">Panoramica sulla data del commit</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Data di completamento Pianificata</td> 
   <td> <p>La data di completamento pianificata mostra quando il proprietario del progetto prevede il completamento dell'attività o del problema. Può essere impostato manualmente dal proprietario del progetto o da chiunque disponga delle autorizzazioni di gestione per l’attività o il problema oppure può essere calcolato automaticamente da Adobe Workfront.</p> <p>Per ulteriori informazioni sulle date di completamento pianificato, vedere <a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Panoramica dell'attività Data completamento pianificata</a></p> </td> 
  </tr> 
 </tbody> 
</table>

## Interazioni tra la data di commit e la data di completamento pianificata

Quando il proprietario del progetto crea e assegna un&#39;attività o un problema, l&#39;attività o il problema avrà le seguenti caratteristiche:

* Una Data Di Completamento Pianificata
* Nessuna data di esecuzione

L&#39;assegnatario che lavora sull&#39;attività o sul problema può aggiornare manualmente la data di commit o aggiornarla automaticamente accettando di lavorarci sopra. Questo è un modo visivo per indicare al proprietario del progetto quando sarebbe realistico per loro completare l’attività o il problema.

>[!TIP]
>
>Solo l&#39;assegnatario può aggiornare la data di commit di un&#39;attività o di un problema.

L&#39;assegnatario che modifica la data di commit non modifica automaticamente la data di completamento pianificata. Anche il contrario è vero: la modifica della data di completamento pianificata non modificherà la data di commit.

Quando la data di commit viene modificata in una data successiva alla data di completamento pianificata, al proprietario del progetto viene notificato che si è verificata questa modifica e potrebbe influire sulla cronologia del progetto.

Se la data di commit offerta dall&#39;assegnatario è accettabile per il proprietario del progetto, deve aggiornare manualmente la data di completamento pianificata sull&#39;attività o sul problema. Per ulteriori informazioni, consulta i seguenti articoli:

* [Panoramica sulla data del commit](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)
* [Aggiorna date di commit su attività e problemi](../../../manage-work/projects/updating-work-in-a-project/update-commit-date-on-tasks-and-issues.md)
