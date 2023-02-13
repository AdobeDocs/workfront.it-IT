---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Guida introduttiva ai risultati e alle attività in Obiettivi di Adobe Workfront
description: Per attivare un obiettivo, devi aggiungere risultati, attività o obiettivi allineati. Questo aggiorna lo stato dell'obiettivo da Bozza a Attivo e inizia a registrare l'avanzamento sull'obiettivo.
author: Alina
feature: Workfront Goals
exl-id: 64fa0aef-cb92-465a-9b74-d863fc232fd1
source-git-commit: afc2124a7fd0d9d52c04be1c174fdba314beec7a
workflow-type: tm+mt
source-wordcount: '812'
ht-degree: 0%

---

# Guida introduttiva ai risultati e alle attività in Obiettivi di Adobe Workfront

<!--drafted for P&P new model: the note at the top will need to be replaced with this:    
    
Your organization must have the following to use the functionality described in this article:    
    
* For the legacy plan and license structure:     
    
  * A Pro or higher [Adobe Workfront plan](https://www.workfront.com/plans).     
  * An Adobe Workfront Goals license in addition to a Workfront license.    
    
* For the current plan and license structure:    
    
  * An Ultimate plan     
        
    Or    
        
    An additional license for Adobe Workfront Goals for the Prime or Select Adobe Workfront plans. <is there a link we can add here for the plans and what they contain?!>    
    
Contact your Workfront account manager to learn about a Workfront Goals license.    
    
For additional information about access to Workfront Goals, see [Requirements to use Workfront Goals](../workfront-goals/goal-management/access-needed-for-wf-goals.md).    
-->

>[!NOTE]
>
>Per utilizzare la funzionalità descritta in questo articolo, l’organizzazione deve disporre delle seguenti caratteristiche:
>
>* A Pro o superiore [piano Adobe Workfront](https://www.workfront.com/plans).
>* Una licenza Adobe Workfront Obiettivi oltre a una licenza Workfront.
>
>  Contatta il tuo account manager Workfront per saperne di più su una licenza di Workfront Obiettivi .
>
>Per ulteriori informazioni sull&#39;accesso agli obiettivi di Workfront, vedi [Requisiti per l&#39;utilizzo degli obiettivi di Workfront](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).


Quando crei un obiettivo, l&#39;obiettivo ha lo stato Bozza. Per informazioni sulla creazione degli obiettivi, vedi [Creare obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/goal-management/create-goals.md).

Per iniziare a registrare l&#39;avanzamento su un obiettivo, è necessario attivarlo. Per attivare l&#39;obiettivo e modificarne lo stato in Attivo, è innanzitutto necessario aggiungere quanto segue:

* Risultato
* Un’attività
* Un progetto
* Un obiettivo allineato

Dopo aver aggiunto almeno uno di questi elementi, puoi attivare l’obiettivo. È necessario aggiornare i risultati e le attività degli obiettivi per indicare l’avanzamento dell’obiettivo.


>[!IMPORTANT]
>
> Un obiettivo non può avere più di 1000 attività, risultati, progetti o obiettivi allineati.</span>

Questo articolo fornisce una panoramica delle attività e dei risultati. Per informazioni sull&#39;allineamento degli obiettivi, vedi [Allineamento degli obiettivi negli obiettivi di Adobe Workfront](../../workfront-goals/goal-alignment/goal-alignment.md). Per informazioni sulla connessione dei progetti agli obiettivi, vedi [Aggiungere progetti agli obiettivi in Obiettivi di Adobe Workfront](../results-and-activities/connect-projects-to-goals-overview.md).

## Panoramica dei risultati

<!--
<p> This will have additional types in the future - add another section for types?)</p>
-->

I risultati misurano il progresso dell’obiettivo o quanto è vicino al raggiungimento di esso. In qualità di proprietario dell’obiettivo, puoi anche possedere il risultato. Un risultato al tuo obiettivo può anche essere assegnato a un altro utente.

Per informazioni sull’aggiunta di risultati agli obiettivi, consulta [Aggiungere risultati agli obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/results-and-activities/add-results-to-goals.md).

Puoi aggiungere risultati ai tuoi obiettivi o obiettivi che appartengono ad altre entità della tua organizzazione.

Quando si lavora con i risultati, considera quanto segue:

* Rispondono alla domanda, &quot;Come faccio a sapere quando il mio obiettivo sarà completo?&quot;
* Sono indicatori metrici. Puoi scegliere tra le seguenti opzioni per indicare un avanzamento per il risultato:

   <!--
  this might change (jira, Salesforce, etc))
  -->

   * Valuta
   * Numero
   * Percentuale

Per ulteriori informazioni sui risultati, consulta l’elenco delle somiglianze tra risultati e attività nella sezione [Somiglianze tra risultati, attività e progetti](#similarities-between-results-activities-and-projects) in questo articolo.

## Panoramica delle attività

<!--
This will have additional types in the future - add another section for types?
-->

Le attività, come i risultati, sono specifiche e misurabili, e in genere includono un indicatore di percentuale completa. In qualità di proprietario dell’obiettivo, puoi anche possedere le attività associate all’obiettivo. Un’attività sull’obiettivo può anche essere assegnata a un utente diverso.

Per informazioni sull’aggiunta di attività agli obiettivi, consulta [Aggiungere attività agli obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/results-and-activities/add-activities-to-goals.md).

Quando associ le attività ai tuoi obiettivi, considera quanto segue:

* Rispondono alla domanda: &quot;Cosa raggiungerò quando l&#39;obiettivo sarà completo?&quot;
* Le attività sono voci personalizzate che possono essere pensate più in termini di complete o incomplete. Devono essere aggiornati manualmente per indicare la percentuale di completamento dell’attività fino a questo momento.

<!--
* You can associate the following activities with goals:

  <table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Manual progress bar </td> 
     <td> <p>Custom entries that can be thought of more in terms of complete or incomplete. They must be manually updated.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader"><p>Project</p></td> 
     <td> <p>Existing projects that you have at least permissions to View and are not in a status of Dead. They are updated automatically, based on the progress of their work items. </p> <p>The projects must exist before associating them with the goal. You can associate a project with multiple goals. For information about adding projects to goals, see <a href="../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md" class="MCXref xref">Add projects to goals in Adobe Workfront Goals</a>.</p>
     <p><span class="preview">In the Preview environment, projects are separate progress indicators, independent from activities. Adding projects to a goal in the Preview environment is different from adding activities. For more information, see <a href="../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md" class="MCXref xref">Add projects to goals in Adobe Workfront Goals</a>.</span></p>
      </td> 
    </tr> 
   </tbody> 
  </table>
-->
<!--drafted for goal redesign: For THE PRODUCTION RELEASE: remove the projects in this article altogether.-->

Per ulteriori informazioni sui risultati e le attività, consulta l’elenco delle somiglianze tra risultati e attività nella sezione [Somiglianze tra risultati, attività e progetti](#similarities-between-results-activities-and-projects) in questo articolo.

## Somiglianze tra risultati, attività e progetti {#similarities-between-results-activities-and-projects}

I risultati, le attività e i progetti sono indicatori di avanzamento degli obiettivi.

Esistono alcune differenze nella gestione dei progetti rispetto al modo in cui gestisci i risultati e le attività. Per informazioni sull’aggiunta di progetti agli obiettivi, consulta [Aggiungere attività agli obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/results-and-activities/add-activities-to-goals.md). Per informazioni sui progetti collegati agli obiettivi, vedi [Aggiungere progetti agli obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).

Oltre ai risultati, alle attività e ai progetti, puoi anche associare gli obiettivi figlio a un obiettivo. Gli obiettivi figlio sono anche un tipo di indicatore di progresso per un obiettivo. Per informazioni, consulta [Allineare gli obiettivi collegandoli negli obiettivi di Adobe Workfront](../goal-alignment/align-goals-by-connecting-them.md). Il progresso degli indicatori di avanzamento dell&#39;obiettivo figlio guida anche il progresso dell&#39;obiettivo padre.

La tabella seguente mostra le somiglianze e le differenze tra risultati, attività e progetti, come indicatori di obiettivo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b><p>Funzione</p></b></td> 
   <td><b><p>Risultati</p></b></td> 
   <td><b><p>Attività</p></b></td> 
   <td> <p><strong>Progetti</strong> </p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td><span style="font-weight: normal;">È possibile personalizzare il nome dell’oggetto nell’interfaccia di Workfront</span> </td> 
   <td>✔</td> 
   <td>✔</td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>Puoi aggiungerli agli obiettivi del passato.</td> 
   <td>✔</td> 
   <td>✔</td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>Puoi associare più risultati, attività o progetti con lo stesso obiettivo. </td> 
   <td>✔</td> 
   <td>✔</td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>Puoi associarne uno a più obiettivi.</td> 
   <td> </td> 
   <td> </td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>I loro progressi vengono presi in considerazione nel calcolo dell'avanzamento dell'obiettivo. </td> 
   <td>✔</td> 
   <td>✔</td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>Devono essere aggiornati manualmente in Obiettivi di Workfront</td> 
   <td>✔</td> 
   <td>✔</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Devono essere completati alla data di fine dell'obiettivo</td> 
   <td>✔</td> 
   <td>✔</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Possono essere assegnati solo a un utente e non a un team, gruppo o azienda. </td> 
   <td>✔</td> 
   <td>✔</td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>Sono specifici e misurabili e in genere includono numeri impostati che indicano il loro progresso. </td> 
   <td>✔</td> 
   <td>✔</td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>Offrono un intervallo di valori tra i valori iniziale e finale che illustra la vicinanza al raggiungimento di tali valori. La vicinanza al valore finale calcola un valore di avanzamento per l'obiettivo. </td> 
   <td>✔</td> 
   <td>✔</td> 
   <td>✔</td> 
  </tr> 
 </tbody> 
</table>
