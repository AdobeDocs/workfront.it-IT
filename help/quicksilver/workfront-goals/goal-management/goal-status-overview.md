---
content-type: overview;reference
product-previous: workfront-goals
navigation-topic: goal-management
title: Panoramica sullo stato dell'obiettivo negli obiettivi di Adobe Workfront
description: Gli stati dell’obiettivo indicano se un obiettivo è attivo e attualmente registra l’avanzamento, o se è inattivo, redatto o già raggiunto.
author: Alina
feature: Workfront Goals
exl-id: dc70dfac-2bdd-41ab-b316-0cd20f749423
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '825'
ht-degree: 4%

---

# Panoramica sullo stato dell&#39;obiettivo negli obiettivi di Adobe Workfront

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
>Contatta il tuo account manager Workfront per saperne di più su una licenza di Workfront Obiettivi .

Per ulteriori informazioni sull&#39;accesso agli obiettivi di Workfront, vedi [Requisiti per l&#39;utilizzo degli obiettivi di Workfront](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).


Gli stati dell’obiettivo indicano se un obiettivo è attivo e attualmente registra l’avanzamento, o se è inattivo, redatto o già raggiunto.

## Considerazione durante l’aggiornamento degli stati dell’obiettivo negli obiettivi di Workfront

* Non puoi aggiornare manualmente lo stato degli obiettivi creati o condivisi con te. Lo stato degli obiettivi viene aggiornato in base alle azioni eseguite sull’obiettivo. Ad esempio, l&#39;attivazione di un obiettivo cambia lo stato Bozza in Attivo.
* Esistono alcune restrizioni e talvolta non è possibile modificare lo stato di un obiettivo in un altro stato, in base alle seguenti regole:

   | Da/A | Bozza | Attivi | Inattiva | Chiuso |
   |---|---|---|---|---|
   | Bozza | - | Sì | No | No |
   | Attivi | No | - | Sì | Sì |
   | Inattiva | No | Sì | - | No |
   | Chiuso | No | Sì | No | - |

* L&#39;apertura di un obiettivo chiuso aggiorna anche il progresso dell&#39;obiettivo.
* Alcune azioni eseguite su un obiettivo ne aggiornano anche lo stato. Per informazioni su come aggiornare gli stati dell’obiettivo, consulta i seguenti articoli:

   * [Creare obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/goal-management/create-goals.md)
   * [Attivare gli obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/goal-management/activate-goals.md)
   * [Eliminare e disattivare gli obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/goal-management/delete-and-deactivate-goals.md)
   * [Chiudere e riaprire gli obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/goal-management/close-and-reopen-goals.md)

## Panoramica degli stati dell’obiettivo negli obiettivi di Workfront

Per informazioni sulla creazione degli obiettivi di Workfront, vedi [Creare obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/goal-management/create-goals.md).

Per informazioni sull’attivazione degli obiettivi, vedi [Attivare gli obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/goal-management/activate-goals.md).

Gli obiettivi possono avere uno dei seguenti stati in Obiettivi di Workfront:

* [Bozza](#draft)
* [Attivi](#active)
* [Inattiva](#inactive)
* [Chiuso](#closed)

### Bozza {#draft}

* Questo è lo stato predefinito per un nuovo obiettivo creato. Per informazioni sulla creazione degli obiettivi, vedi [Creare obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/goal-management/create-goals.md).
* Gli obiettivi di Workfront non registrano i progressi su un obiettivo elaborato.
* Non è possibile aggiornare l&#39;avanzamento di un obiettivo di una bozza.
* Non è possibile chiudere o disattivare gli obiettivi di bozza perché non dispongono di informazioni sull&#39;avanzamento.
* Gli obiettivi elaborati non contribuiscono al calcolo del progresso di altri obiettivi e non sono presi in considerazione nei grafici.
* Gli obiettivi elaborati vengono visualizzati nelle seguenti aree degli obiettivi di Workfront:

   * Elenco obiettivi
   * Sezione Allineamento obiettivo (solo come obiettivo allineato)


>[!IMPORTANT]
>
>Dopo aver modificato lo stato di un obiettivo in qualsiasi altro stato, l&#39;obiettivo non può più essere posizionato in stato Bozza.

### Attivi {#active}

* È possibile attivare un obiettivo abbozzo solo quando lo si associa a un risultato, a un&#39;attività o ad un altro obiettivo. L&#39;attivazione dell&#39;obiettivo ne modifica lo stato in Attivo. Per informazioni sull’attivazione degli obiettivi, vedi [Attivare gli obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/goal-management/activate-goals.md).
* Obiettivi di Workfront registra i progressi relativi agli obiettivi attivi.
* Gli obiettivi attivi contribuiscono al calcolo dello stato di avanzamento di altri obiettivi e sono presi in considerazione nei grafici.
* Gli obiettivi attivi vengono visualizzati nelle seguenti aree di Obiettivi di Workfront:

   * Elenco obiettivi
   * Sezione Allineamento obiettivo
   * Lo stato di avanzamento degli obiettivi attivi viene visualizzato nei grafici

* Puoi riattivare un obiettivo chiuso o inattivo.

### Inattiva {#inactive}

* È possibile disattivare un obiettivo attivo quando il proprietario ha smesso di utilizzarlo temporaneamente o permanentemente. È possibile conservarlo per informazioni storiche. Lo stato dell’obiettivo viene aggiornato in Inattivo.

   Per informazioni sulla disattivazione degli obiettivi, consulta la sezione &quot;Disattivare gli obiettivi&quot; nell’articolo [Eliminare e disattivare gli obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/goal-management/delete-and-deactivate-goals.md).

* Non è possibile disattivare un obiettivo elaborato o chiuso.
* Puoi riattivare un obiettivo inattivo e continuare a lavorarci.
* Obiettivi di Workfront non calcola l&#39;avanzamento degli obiettivi inattivi.
* Non è possibile aggiornare l&#39;avanzamento di un obiettivo inattivo.
* Gli obiettivi inattivi non contribuiscono al calcolo del progresso di altri obiettivi e non vengono presi in considerazione nei grafici.
* Gli obiettivi inattivi hanno una storia di progresso perché una volta erano attivi, a differenza degli obiettivi elaborati.
* Gli obiettivi inattivi vengono visualizzati nelle seguenti aree di Obiettivi di Workfront:

   * Elenco obiettivi
   * Sezione Allineamento obiettivo (solo come obiettivi allineati)

### Chiuso {#closed}

* È possibile chiudere un obiettivo quando si desidera indicare che lo si è raggiunto o che non si sta più lavorando su di esso né lo si farà in futuro. Per informazioni sulla chiusura degli obiettivi, vedi [Chiudere e riaprire gli obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/goal-management/close-and-reopen-goals.md).

   >[!TIP]
   >
   >Se in seguito si prevede di lavorare su un obiettivo non ancora raggiunto, è consigliabile modificare lo stato in Inattivo anziché Chiuso.

* Non è possibile raggiungere obiettivi mai attivati, come gli obiettivi prefissati.
* Puoi riaprire un obiettivo chiuso e continuare a lavorarci.
* Obiettivi di Workfront smette di registrare l&#39;avanzamento sugli obiettivi chiusi.
* Non è possibile aggiornare l&#39;avanzamento di un obiettivo chiuso.
* Gli obiettivi chiusi vengono visualizzati nella seguente area di Obiettivi di Workfront:

   * Elenco obiettivi
   * Sezione Allineamento obiettivo (solo come obiettivi allineati)
   * Le informazioni provenienti da obiettivi chiusi sono inoltre prese in considerazione nella sezione Grafici.
