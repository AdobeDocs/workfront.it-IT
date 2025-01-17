---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Aggiungere un webhook a uno scenario di base
description: La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione. Questo articolo è stato dichiarato obsoleto, ma contiene un collegamento al nuovo articolo che descrive questa funzionalità.
author: Becky
feature: Workfront Fusion
exl-id: 6694b883-6f94-449c-bcfe-5a4053e8655a
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 0%

---

# Aggiungere un webhook a uno scenario di base in [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione.
>
>Le informazioni contenute in questo articolo sono ora disponibili nell’articolo:
>
>* [Aggiungere un webhook a uno scenario di base](https://experienceleague.adobe.com/docs/workfront-fusion/using/build-practice-scenarios/add-a-webhook-to-basic-scenario.html)
>
>Aggiorna eventuali segnalibri.
>
>Questo articolo non è più in fase di aggiornamento e verrà rimosso nel prossimo futuro.

I webhook, noti anche come trigger istantanei, sono un tipo specifico di modulo di trigger che può avviare uno scenario ogni volta che viene apportata una modifica, anziché in base a una determinata pianificazione.

In questo esempio, aggiungi un webhook per avviare uno scenario non appena vengono inviate richieste a una coda specifica. Lo scenario quindi converte tali richieste in un progetto.

In questo esempio viene modificato lo scenario creato in [Crea uno scenario di base](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md).

## Prerequisiti

È necessario creare lo scenario descritto in [Creare uno scenario di base](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) prima di seguire questa procedura.

## Aggiungere e configurare il webhook

1. Aprire il modulo Converti oggetto.
1. Nel campo ID problema, elimina il blocco ID nero. Il blocco è nero perché il modulo da cui è stato mappato non è più disponibile.
1. Seleziona il blocco ID sotto il primo modulo (Osserva eventi) per mapparlo al secondo modulo.
1. Fare clic su **OK**.

### Aggiungere il modulo webhook

1. Apri lo scenario nell’editor dello scenario.
1. Fare clic con il pulsante destro del mouse sul primo modulo e selezionare **Elimina modulo**.

   Il modulo viene eliminato, lasciando un segnaposto vuoto.

1. Fai clic sul modulo vuoto e seleziona **Adobe Workfront** dall&#39;elenco delle app.
1. Seleziona **Guarda gli eventi**.
1. Fai clic su **Aggiungi** accanto al campo Webhook.
1. Nel campo Tipo di record, seleziona **Problema**, in modo che il modulo si attivi per le modifiche nei problemi.
1. Nel campo Stato, selezionare **Nuovo stato**. Questo è un campo obbligatorio utilizzato per il filtro, che questo esempio non copre.
1. Nel campo Origine record selezionare **Solo nuovo record**. Questo consente allo scenario di attivarsi quando viene aggiunto un problema, non quando ne viene aggiornato o eliminato uno.
1. Fai clic su **Salva** per salvare la configurazione del modulo.
