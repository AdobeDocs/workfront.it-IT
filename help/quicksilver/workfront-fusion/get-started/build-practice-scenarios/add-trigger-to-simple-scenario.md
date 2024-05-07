---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Aggiungere un modulo trigger a uno scenario di base
description: Scopri come aggiungere un modulo trigger per consentire allo scenario di cercare periodicamente nuove richieste e convertirle in progetti.
author: Becky
feature: Workfront Fusion
source-git-commit: ea3f932e02ad8a9416747d4b9aefe89d087dd414
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---

# Aggiungere un modulo trigger a uno scenario di base

I moduli di attivazione vengono posizionati all’inizio di uno scenario. Questi moduli iniziano l’esecuzione di uno scenario quando si verificano criteri specifici in seguito a una modifica in un determinato servizio. La modifica può consistere nella creazione di nuovi record, nell&#39;eliminazione di record, nell&#39;aggiornamento di record e così via.

I moduli di polling controllano il servizio a un intervallo di tempo impostato e restituiscono informazioni sulle modifiche apportate durante tale intervallo. Se non ci sono state modifiche, il trigger non esegue lo scenario.

In questo esempio, aggiungi un modulo trigger che viene eseguito ogni 15 minuti e avvia uno scenario se sono state inviate richieste a una coda specifica. Lo scenario quindi converte tali richieste in un progetto.

Questo esempio modifica lo scenario creato in [Creare uno scenario di base](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md).

## Prerequisiti

Devi creare lo scenario descritto in [Creare uno scenario di base](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) prima di seguire questa procedura.

## Aggiungere e configurare il modulo trigger

### Aggiungere il modulo trigger

1. Apri lo scenario nell’editor dello scenario.
1. Fai clic con il pulsante destro del mouse sul primo modulo (Ricerca) e seleziona (Cerca) **Elimina modulo**.

   Il modulo viene eliminato, lasciando un segnaposto vuoto.

1. Fai clic sul modulo vuoto e seleziona **Adobe Workfront** dall’elenco delle app.
1. Seleziona **Record di controllo**.
1. Assicurati che il modulo utilizzi la stessa connessione degli altri moduli dello scenario.
1. Nel campo Filtro, seleziona **Solo nuovi record**.
1. Nella casella Output selezionare `ID`, `Name`, e `Project ID`.
1. Clic **OK** per salvare le impostazioni del modulo.

   Viene visualizzata la finestra Scegli da dove iniziare.

1. Seleziona **Da ora in poi**.

### Pianificare il modulo trigger

1. Fare clic sull&#39;orologio nel modulo Record di controllo.

   Viene visualizzata la finestra di impostazione Schedule.

1. Nel campo Esegui scenario selezionare **A intervalli regolari**.

1. Clic **OK**.

### Aggiornare il secondo modulo

Poiché il primo modulo è stato sostituito, il secondo modulo deve essere mappato al nuovo primo modulo.

1. Aprire il modulo Converti oggetto.
1. Nel campo ID problema, elimina il blocco ID nero. Il blocco è nero perché il modulo da cui è stato mappato non è più disponibile.
1. Seleziona il blocco ID sotto il primo modulo (Record di controllo) per mapparlo al secondo modulo.
1. Clic **OK**.

### Test e attivazione

1. Vai all’ambiente Workfront a cui si connette Fusion e aggiungi un problema.
1. Clic **[!UICONTROL Esegui una volta]** nell’angolo inferiore sinistro dell’editor di scenari.
1. Esamina l’output per garantire che lo scenario sia stato eseguito come previsto.
1. Quando si è certi che lo scenario funziona come previsto, fare clic sul pulsante **Pianificazione** in basso a sinistra dello schermo per **On**.

   Questo attiva lo scenario.
1. In entrata [!DNL Workfront Fusion], fai clic su **[!UICONTROL Salva]** nell’angolo in basso a sinistra per salvare i progressi sullo scenario.

   >[!IMPORTANT]
   >
   >Risparmia spesso quando affili e testa uno scenario.

## Risorse

* Per ulteriori informazioni sui webhook, consulta [Trigger istantanei (webhook) in [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/webhooks/instant-triggers-webhooks.md).
