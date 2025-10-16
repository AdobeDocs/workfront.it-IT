---
content-type: overview;reference
product-previous: workfront-goals
navigation-topic: goal-management
title: Panoramica sullo stato degli obiettivi in Obiettivi di Adobe Workfront
description: Gli stati obiettivo indicano se un obiettivo è attivo e sta registrando l’avanzamento, oppure se è inattivo, bozza o già raggiunto.
author: Alina
feature: Workfront Goals
exl-id: dc70dfac-2bdd-41ab-b316-0cd20f749423
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '793'
ht-degree: 4%

---

# Panoramica sullo stato degli obiettivi in Obiettivi di Adobe Workfront

<!--Audited: 4/2025-->

>[!NOTE]
>
>La tua azienda potrebbe scegliere di continuare a utilizzare gli obiettivi di Adobe Workfront se ha acquistato questo pacchetto in passato. Per ulteriori dettagli, rivolgiti al rappresentante del tuo account.
>
>Adobe Workfront Goals non è più disponibile per l’acquisto.
>
>Per ulteriori informazioni sull&#39;accesso agli obiettivi di Workfront, vedere [Requisiti per l&#39;utilizzo degli obiettivi di Workfront](/help/quicksilver/workfront-goals/goal-management/access-needed-for-wf-goals.md).

<!--Old:

>[!IMPORTANT]
>
>Your organization must have the following to use the functionality described in this article:
>
>* For the new plan and license structure:
>
>   * The Ultimate Workfront plan 
>    
>* For the current plan and license structure: 
>
>   * A Pro or higher Workfront plan
>   * An Adobe Workfront Goals license in addition to a Workfront license.
>
>Contact your Workfront account manager to learn about a Workfront Goals license.    
> 
>For additional information about access to Workfront Goals, see [Requirements to use Workfront Goals](/help/quicksilver/workfront-goals/goal-management/access-needed-for-wf-goals.md).   -->

## Considerazione durante l’aggiornamento degli stati degli obiettivi in Obiettivi di Workfront

* Non puoi aggiornare manualmente lo stato degli obiettivi che hai creato o che sono stati condivisi con te. Lo stato degli obiettivi viene aggiornato in base alle azioni eseguite sull’obiettivo. Ad esempio, l&#39;attivazione di un obiettivo modifica lo stato Bozza in Attivo.
* Esistono alcune restrizioni e a volte non è possibile modificare lo stato di un obiettivo in un altro stato, in base alle seguenti regole:

  | Da/A | Bozza | Attivo | Inattiva | Chiuso |
  |---|---|---|---|---|
  | Bozza | - | Sì | No | No |
  | Attivo | No | - | Sì | Sì |
  | Inattiva | No | Sì | - | No |
  | Chiuso | No | Sì | No | - |

* L’apertura di un obiettivo chiuso aggiorna anche l’avanzamento dell’obiettivo.
* Alcune azioni eseguite su un obiettivo aggiornano anche il relativo stato. Per informazioni su come aggiornare gli stati degli obiettivi, vedi i seguenti articoli:

   * [Crea obiettivi in Obiettivi Adobe Workfront](../../workfront-goals/goal-management/create-goals.md)
   * [Attiva obiettivi in Obiettivi Adobe Workfront](../../workfront-goals/goal-management/activate-goals.md)
   * [Elimina e disattiva obiettivi in Obiettivi Adobe Workfront](../../workfront-goals/goal-management/delete-and-deactivate-goals.md)
   * [Chiudere e riaprire gli obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/goal-management/close-and-reopen-goals.md)

## Panoramica degli stati degli obiettivi in Obiettivi di Workfront

Per informazioni sulla creazione degli obiettivi di Workfront, vedere [Creare gli obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/goal-management/create-goals.md).

Per informazioni sull&#39;attivazione degli obiettivi, vedere [Attivare gli obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/goal-management/activate-goals.md).

Gli obiettivi possono avere uno dei seguenti stati in Obiettivi Workfront:

* [Bozza](#draft)
* [Attivo](#active)
* [Inattivo](#inactive)
* [Chiuso](#closed)

### Bozza {#draft}

* Questo è lo stato predefinito per un obiettivo appena creato. Per informazioni sulla creazione degli obiettivi, vedere [Creare gli obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/goal-management/create-goals.md).
* Obiettivi Workfront non registra l’avanzamento su un obiettivo bozza.
* Non è possibile aggiornare l’avanzamento di una bozza di obiettivo.
* Non è possibile chiudere o disattivare gli obiettivi bozza perché mancano le informazioni sull&#39;avanzamento.
* Gli obiettivi prefissati non contribuiscono al calcolo del progresso di altri obiettivi e non vengono presi in considerazione nei grafici.
* Gli obiettivi bozza vengono visualizzati nelle seguenti aree di Obiettivi Workfront:

   * Elenco obiettivi
   * Sezione Allineamento obiettivo (solo come obiettivo allineato)


>[!IMPORTANT]
>
>Dopo aver modificato lo stato di un obiettivo in qualsiasi altro stato, l’obiettivo non può più essere posizionato in stato Bozza.

### Attivo {#active}

* È possibile attivare un obiettivo abbozzato solo quando lo si associa a un risultato, a un&#39;attività o vi si allinea un altro obiettivo. L’attivazione dell’obiettivo ne modifica lo stato in Attivo. Per informazioni sull&#39;attivazione degli obiettivi, vedere [Attivare gli obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/goal-management/activate-goals.md).
* Obiettivi Workfront registra l’avanzamento degli obiettivi attivi.
* Gli obiettivi attivi contribuiscono al calcolo del progresso di altri obiettivi e vengono presi in considerazione nei grafici.
* Gli obiettivi attivi vengono visualizzati nelle seguenti aree di Obiettivi Workfront:

   * Elenco obiettivi
   * Sezione Allineamento obiettivo
   * L’avanzamento degli obiettivi attivi viene visualizzato nei grafici

* Puoi riattivare un obiettivo chiuso o inattivo.

### Inattiva {#inactive}

* Puoi disattivare un obiettivo attivo quando il proprietario smette di lavorarci temporaneamente o definitivamente. Puoi conservarla per informazioni storiche. Questo aggiorna lo stato dell’obiettivo a Inattivo.

  Per informazioni sulla disattivazione degli obiettivi, vedere la sezione &quot;Disattivare gli obiettivi&quot; nell&#39;articolo [Eliminare e disattivare gli obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/goal-management/delete-and-deactivate-goals.md).

* Non è possibile disattivare un obiettivo selezionato o chiuso.
* Puoi riattivare un obiettivo inattivo e continuare a lavorarci.
* Obiettivi Workfront non calcola l’avanzamento sugli obiettivi inattivi.
* Impossibile aggiornare l’avanzamento di un obiettivo inattivo.
* Gli obiettivi inattivi non contribuiscono al calcolo del progresso di altri obiettivi e non vengono presi in considerazione nei grafici.
* Gli obiettivi inattivi hanno una cronologia dei progressi perché una volta erano attivi, a differenza degli obiettivi bozzati.
* Gli obiettivi inattivi vengono visualizzati nelle seguenti aree di Obiettivi Workfront:

   * Elenco obiettivi
   * Sezione Allineamento obiettivo (solo come obiettivi allineati)

### Chiuso {#closed}

* È possibile chiudere un obiettivo quando si desidera indicare che è stato raggiunto o che non si sta più lavorando su di esso né lo si farà in futuro. Per informazioni sulla chiusura degli obiettivi, vedere [Chiudere e riaprire gli obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/goal-management/close-and-reopen-goals.md).

  >[!TIP]
  >
  >Se prevedi di lavorare in un secondo momento su un obiettivo non ancora raggiunto, ti consigliamo di modificare lo stato su Inattivo invece di Chiuso.

* Non puoi chiudere obiettivi che non sono mai stati attivati, come gli obiettivi bozza.
* Puoi riaprire un obiettivo chiuso e continuare a lavorarci.
* Workfront Goals interrompe la registrazione dell&#39;avanzamento su obiettivi chiusi.
* Non è possibile aggiornare l’avanzamento di un obiettivo chiuso.
* Gli obiettivi chiusi vengono visualizzati nella seguente area di Obiettivi Workfront:

   * Elenco obiettivi
   * Sezione Allineamento obiettivo (solo come obiettivi allineati)
   * Nella sezione Grafici vengono inoltre prese in considerazione le informazioni relative agli obiettivi chiusi.
