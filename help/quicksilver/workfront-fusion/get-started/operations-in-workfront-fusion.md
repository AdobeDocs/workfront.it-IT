---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Operazioni in Adobe Workfront Fusion
description: La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione. Questo articolo è stato dichiarato obsoleto, ma contiene un collegamento al nuovo articolo che descrive questa funzionalità.
author: Becky
feature: Workfront Fusion
exl-id: 34268fb6-e485-42be-b751-3ee79bbf5797
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 0%

---

# Operazioni in [!DNL Adobe Workfront Fusion]



>[!IMPORTANT]
>
>La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione.
>
>Le informazioni contenute in questo articolo sono ora disponibili nell’articolo:
>
>* [Operazioni](https://experienceleague.adobe.com/docs/workfront-fusion/using/set-up-and-manage-fusion/licensing-and-operations-overviews/operations-in-workfront-fusion.html)
>
>Aggiorna eventuali segnalibri.
>
>Questo articolo non è più in fase di aggiornamento e verrà rimosso nel prossimo futuro.

Un&#39;operazione in [!DNL Adobe Workfront Fusion] è un&#39;attività eseguita da un modulo. Ai fini del tracciamento, qualsiasi azione eseguita correttamente da un modulo è un’operazione.

## Considerazioni durante il conteggio del numero di operazioni

* In generale, qualsiasi esecuzione di un’azione eseguita con successo viene considerata un’operazione.

* Il primo modulo di uno scenario viene eseguito una sola volta e viene sempre conteggiato come un’unica operazione, anche se non restituisce un bundle.

* Il numero di volte in cui gli altri moduli vengono eseguiti dipende dal numero di bundle che devono elaborare.  Un’esecuzione di un modulo per un bundle è un’unica operazione. Un’eccezione è il modulo aggregatore, conteggiato come un’unica operazione per set di bundle in fase di elaborazione.

* Le operazioni vengono conteggiate nella fase [!UICONTROL Finalizzazione] dell&#39;esecuzione di uno scenario.

* **non** sono conteggiati come operazioni:

   * Qualsiasi passaggio di filtro.

   * Qualsiasi azione che si verifichi un errore o si arresti.

   * Qualsiasi route non eseguita perché non sono state soddisfatte le regole della route, ad esempio route di fallback o disabilitate.

   * Qualsiasi azione non eseguita, perché un filtro non ha consentito il passaggio dei dati o perché lo scenario è stato interrotto a causa di un errore.

## Limiti operativi

La tua organizzazione potrebbe avere un limite mensile di operazioni. Si basa sul piano [!DNL Workfront] acquistato dalla tua organizzazione. Il piano [!UICONTROL Ultimate] [!DNL Workfront] offre operazioni illimitate.

Se la tua organizzazione dispone di un limite mensile, riceverai una notifica quando ti avvicini al limite. Se superi il limite, [!DNL Workfront] contatterà l&#39;organizzazione per assicurarsi che il piano soddisfi le tue esigenze.

## Visualizza il numero di operazioni eseguite negli ultimi 30 giorni

È possibile visualizzare un grafico che mostra il numero di operazioni eseguite. Questi grafici sono disponibili nelle seguenti posizioni:

* **Dashboard organizzazione**: operazioni utilizzate dall&#39;intera organizzazione
* **Dashboard team**: operazioni utilizzate da scenari di proprietà di questo team (solo [!DNL Adobe Experience Cloud])
* **Pagina dettagli scenario**: operazioni utilizzate da questo scenario ([!DNL Adobe Experience Cloud] solo)
