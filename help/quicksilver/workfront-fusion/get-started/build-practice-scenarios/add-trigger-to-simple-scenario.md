---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Aggiungere un modulo trigger a uno scenario di base
description: La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione. Questo articolo è stato dichiarato obsoleto, ma contiene un collegamento al nuovo articolo che descrive questa funzionalità.
author: Becky
feature: Workfront Fusion
exl-id: 067ee6a1-f4c1-4602-ac39-0283255cced8
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 0%

---

# Aggiungere un modulo trigger a uno scenario di base

>[!IMPORTANT]
>
>La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione.
>
>Le informazioni contenute in questo articolo sono ora disponibili nell’articolo:
>
>* [Aggiungere un modulo trigger a uno scenario di base](https://experienceleague.adobe.com/docs/workfront-fusion/using/build-practice-scenarios/add-trigger-to-basic-scenario.html)
>
>Aggiorna eventuali segnalibri.
>
>Questo articolo non è più in fase di aggiornamento e verrà rimosso nel prossimo futuro.

I moduli di attivazione vengono posizionati all’inizio di uno scenario. Questi moduli iniziano l’esecuzione di uno scenario quando si verificano criteri specifici in seguito a una modifica in un determinato servizio. La modifica può consistere nella creazione di nuovi record, nell&#39;eliminazione di record, nell&#39;aggiornamento di record e così via.

I moduli di polling controllano il servizio a un intervallo di tempo impostato e restituiscono informazioni sulle modifiche apportate durante tale intervallo. Se non ci sono state modifiche, il trigger non esegue lo scenario.

In questo esempio, aggiungi un modulo trigger che viene eseguito ogni 15 minuti e avvia uno scenario se sono state inviate richieste a una coda specifica. Lo scenario quindi converte tali richieste in un progetto.

In questo esempio viene modificato lo scenario creato in [Crea uno scenario di base](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md).

## Prerequisiti

È necessario creare lo scenario descritto in [Creare uno scenario di base](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) prima di seguire questa procedura.

## Aggiungere e configurare il modulo trigger

### Aggiungere il modulo trigger

1. Apri lo scenario nell’editor dello scenario.
1. Fare clic con il pulsante destro del mouse sul primo modulo (Ricerca) e selezionare **Elimina modulo**.

   Il modulo viene eliminato, lasciando un segnaposto vuoto.

1. Fai clic sul modulo vuoto e seleziona **Adobe Workfront** dall&#39;elenco delle app.
1. Seleziona **Record di controllo**.
1. Assicurati che il modulo utilizzi la stessa connessione degli altri moduli dello scenario.
1. Nel campo Filtro, selezionare **Solo nuovi record**.
1. Nel campo Tipo di record selezionare **Problema**.
1. Nella casella Output selezionare `ID`, `Name` e `Project ID`.
1. Fare clic su **OK** per salvare le impostazioni del modulo.

   Viene visualizzata la finestra Scegli da dove iniziare.

1. Seleziona **Da ora in data**.

### Pianificare il modulo trigger

1. Fare clic sull&#39;orologio nel modulo Record di controllo.

   Viene visualizzata la finestra di impostazione Schedule.

1. Nel campo Esegui scenario selezionare **A intervalli regolari**.

1. Fare clic su **OK**.

### Aggiornare il secondo modulo

Poiché il primo modulo è stato sostituito, il secondo modulo deve essere mappato al nuovo primo modulo.

1. Aprire il modulo Converti oggetto.
1. Nel campo ID problema, elimina il blocco ID nero. Il blocco è nero perché il modulo da cui è stato mappato non è più disponibile.
1. Seleziona il blocco ID sotto il primo modulo (Record di controllo) per mapparlo al secondo modulo.
1. Fare clic su **OK**.

### Test e attivazione

1. Vai all’ambiente Workfront a cui si connette Fusion e aggiungi un problema.
1. Fai clic su **[!UICONTROL Esegui una volta]** nell&#39;angolo inferiore sinistro dell&#39;editor scenari.
1. Esamina l’output per garantire che lo scenario sia stato eseguito come previsto.
1. Quando si è certi che lo scenario funziona come previsto, fare clic sull&#39;interruttore **Pianificazione** in basso a sinistra dello schermo per **Attivato**.

   Questo attiva lo scenario.
1. In [!DNL Workfront Fusion], fai clic su **[!UICONTROL Salva]** nell&#39;angolo inferiore sinistro per salvare l&#39;avanzamento dello scenario.

   >[!IMPORTANT]
   >
   >Risparmia spesso quando affili e testa uno scenario.

## Risorse

* Per ulteriori informazioni sui webhook, vedere [Trigger istantanei (webhook) in [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/webhooks/instant-triggers-webhooks.md).
