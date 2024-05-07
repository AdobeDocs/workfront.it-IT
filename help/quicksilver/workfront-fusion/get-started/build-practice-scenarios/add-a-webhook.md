---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Aggiungere un webhook a uno scenario di base
description: I webhook, noti anche come trigger istantanei, sono un tipo specifico di modulo di trigger che può avviare uno scenario ogni volta che viene apportata una modifica, anziché in base a una determinata pianificazione.
author: Becky
feature: Workfront Fusion
source-git-commit: ea3f932e02ad8a9416747d4b9aefe89d087dd414
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 0%

---

# Aggiungere un webhook a uno scenario di base in [!DNL Adobe Workfront Fusion]

I webhook, noti anche come trigger istantanei, sono un tipo specifico di modulo di trigger che può avviare uno scenario ogni volta che viene apportata una modifica, anziché in base a una determinata pianificazione.

In questo esempio, aggiungi un webhook per avviare uno scenario non appena vengono inviate richieste a una coda specifica. Lo scenario quindi converte tali richieste in un progetto.

Questo esempio modifica lo scenario creato in [Creare uno scenario di base](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md).

## Prerequisiti

Devi creare lo scenario descritto in [Creare uno scenario di base](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) prima di seguire questa procedura.

## Aggiungere e configurare il webhook

1. Aprire il modulo Converti oggetto.
1. Nel campo ID problema, elimina il blocco ID nero. Il blocco è nero perché il modulo da cui è stato mappato non è più disponibile.
1. Seleziona il blocco ID sotto il primo modulo (Osserva eventi) per mapparlo al secondo modulo.
1. Clic **OK**.

### Aggiungere il modulo webhook

1. Apri lo scenario nell’editor dello scenario.
1. Fai clic con il pulsante destro del mouse sul primo modulo e seleziona (Gestisci origini dati) **Elimina modulo**.

   Il modulo viene eliminato, lasciando un segnaposto vuoto.

1. Fai clic sul modulo vuoto e seleziona **Adobe Workfront** dall’elenco delle app.
1. Seleziona **Guarda gli eventi**.
1. Clic **Aggiungi** accanto al campo Webhook.
1. nel campo Tipo di record selezionare **Problema**, in modo che il modulo venga attivato per le modifiche nei problemi.
1. Nel campo Stato, seleziona **Nuovo stato**. Questo è un campo obbligatorio utilizzato per il filtro, che questo esempio non copre.
1. Nel campo Origine record selezionare **Solo nuovo record**. Questo consente allo scenario di attivarsi quando viene aggiunto un problema, non quando ne viene aggiornato o eliminato uno.
1. Clic **Salva** per salvare la configurazione del modulo.


