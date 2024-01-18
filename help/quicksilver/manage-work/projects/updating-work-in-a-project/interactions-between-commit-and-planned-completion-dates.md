---
product-area: projects
navigation-topic: update-work-in-a-project
title: Interazioni tra la data di conferma e la data di completamento pianificata
description: Sia le date di completamento pianificate che le date di conferma indicano quando l'attività deve essere completata. Ma differiscono a causa di chi imposta ogni data.
author: Alina
feature: Work Management
exl-id: 1709c60c-ac75-48eb-9226-ec2cf556ebf0
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 1%

---

# Interazioni tra la data di conferma e la data di completamento pianificata

<!--
this article has mostly information that is repeated from the articles linked from here. I left it in here for searchability's sake.
-->

Sia le date di completamento pianificate che le date di conferma indicano quando l&#39;attività deve essere completata. Ma differiscono a causa di chi imposta ogni data.

## Panoramica della data di conferma e della data di completamento pianificata

Le date pianificate di completamento e commit esistono sia per le attività che per i problemi.

La tabella seguente contiene informazioni sulla differenza tra le date di conferma e di completamento pianificato:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Conferma data</td> 
   <td> <p>La Data conferma è la data entro la quale la persona assegnata a un’attività o a un problema stima manualmente che avrà completato l’attività o il problema.</p> <p>Per informazioni sulle date di conferma, vedere <a href="../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">Panoramica sulla data di conferma</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Data di completamento Pianificata</td> 
   <td> <p>La Data di completamento pianificata mostra quando il proprietario del progetto prevede che l’attività o il problema sia completato. Può essere impostata manualmente dal proprietario del progetto o da chiunque abbia le autorizzazioni di Gestione per l’attività o il problema, oppure può essere calcolata automaticamente da Adobe Workfront.</p> <p>Per ulteriori informazioni sulle date di completamento pianificate, consulta <a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Panoramica della data di completamento pianificata dell'attività</a></p> </td> 
  </tr> 
 </tbody> 
</table>

## Interazioni tra la data di conferma e la data di completamento pianificata

Quando il proprietario del progetto crea e assegna un’attività o un problema, l’attività o il problema avrà i seguenti elementi:

* Una data di completamento pianificata
* Nessuna data di esecuzione

L’assegnatario che lavora sull’attività o sul problema può aggiornare manualmente la Data di conferma o automaticamente accettando di lavorarci. Questo è un modo visivo per indicare al proprietario del progetto quando sarebbe realistico per lui completare l’attività o il problema.

>[!TIP]
>
>Solo l’assegnatario può aggiornare la Data di conferma di un’attività o di un problema.

L’assegnatario che modifica la Data di conferma non modifica automaticamente la Data di completamento pianificata. Anche il contrario è vero: la modifica della Data di completamento pianificata non modificherà la Data impegno.

Quando la data di conferma diventa una data successiva alla data di completamento pianificata, il proprietario del progetto riceve una notifica che indica che la modifica si è verificata e che potrebbe influire sulla sequenza temporale del progetto, se il proprietario del progetto utilizza l’esperienza di commento legacy. Questa funzionalità non è supportata nella nuova esperienza di aggiunta di commenti. Per ulteriori informazioni, consulta [Nuova esperienza di commento](/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

Se la Data impegno offerta dall’assegnatario è accettabile per il proprietario del progetto, deve aggiornare manualmente la Data di completamento pianificata sull’attività o sul problema. Per ulteriori informazioni, consulta i seguenti articoli:

* [Panoramica sulla data di conferma](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)
* [Aggiorna le date di conferma per attività e problemi](../../../manage-work/projects/updating-work-in-a-project/update-commit-date-on-tasks-and-issues.md)
