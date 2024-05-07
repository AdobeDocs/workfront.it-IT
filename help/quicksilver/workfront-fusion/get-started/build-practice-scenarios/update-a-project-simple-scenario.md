---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Aggiungere un modulo trigger a uno scenario di base
description: Scopri come aggiungere un modulo trigger per consentire allo scenario di cercare periodicamente nuove richieste e convertirle in progetti.
author: Becky
feature: Workfront Fusion
source-git-commit: 91d3dcde8eda416286c6781f6eef85404fd382c2
workflow-type: tm+mt
source-wordcount: '499'
ht-degree: 0%

---

# Utilizzare una funzione per aggiornare un progetto in uno scenario semplice in [!DNL Adobe Workfront Fusion]

L’aggiornamento di un elemento di lavoro di Workfront è un caso d’uso comune per Workfront Fusion. In questo esempio, utilizzerai una funzione per modificare il nome di un progetto in lettere maiuscole.

Fusion include molti tipi di funzioni che consentono di trasformare ed eseguire logica condizionale sui dati. Per ulteriori informazioni sull&#39;utilizzo delle funzioni, vedere [Mappare le informazioni da un modulo all’altro in Adobe Workfront Fusion](/help/quicksilver/workfront-fusion/mapping/map-information-between-modules.md).

Questo esempio modifica lo scenario creato in [Creare uno scenario di base](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md).

## Prerequisiti

Devi creare lo scenario descritto in [Creare uno scenario di base](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) prima di seguire questa procedura.

## Utilizzare una funzione per aggiornare un progetto

### Aggiungi il modulo Aggiorna record allo scenario

1. Apri lo scenario nell’editor dello scenario.
1. Passa il puntatore del mouse sul cerchio parziale a destra della sezione del modulo, quindi fai clic su **[!UICONTROL Aggiungi un altro modulo]**.
1. Seleziona [!DNL Adobe Workfront] dall’elenco delle applicazioni, scegli il modulo **[!UICONTROL Aggiorna record]**.
1. nel campo ID, seleziona il blocco ID che si trova sotto il modulo Converti oggetto. Questo è l&#39;ID del progetto generato da quel modulo.

   ![ID da oggetto Convert](assets/id-convert-object.png)

1. Nel campo Tipo di record selezionare Progetto, poiché l&#39;oggetto da aggiornare è un progetto.
1. Nell&#39;area Seleziona campi da mappare selezionare Nome.

   Viene aperto un campo Nome.

### Mappa la funzione per l’aggiornamento del nome

Quando questo scenario converte una richiesta in un progetto, il nome del progetto è uguale alla richiesta. La funzione in questo caso prende il nome e le lettere in maiuscolo.

1. Fai clic su **Nome** campo.

   Viene visualizzato il pannello di mappatura.
1. Nel pannello di mappatura, fai clic su **Funzioni di testo e binarie** icona. ![Icona funzioni testo](/help/quicksilver/workfront-fusion/functions/assets/toolbar-icon-text&binary-functions.png)
1. Seleziona la funzione **upper**.

   La funzione viene visualizzata nel campo Nome, inclusa la formattazione dell&#39;input previsto.

   L’input per questo esempio è il nome del problema da cui è stato convertito il progetto.

1. Spostare il cursore tra le parentesi, perché è qui che andrà l&#39;input.
1. Nel pannello di mappatura, fai clic su **output del modulo** icona. ![Icona output modulo](/help/quicksilver/workfront-fusion/functions/assets/toolbar-icon-functions-you-map-from-other-modules.png)
1. Seleziona il blocco del nome restituito dal primo modulo.

   Il blocco del nome viene visualizzato nella funzione.

   ![Blocco nome nella funzione](assets/map-name.png)

1. Scegliere OK per salvare le impostazioni del modulo.

### Test e attivazione

1. Verifica lo scenario facendo clic su **Esegui una volta** nell&#39;angolo inferiore sinistro dello schermo.
1. Esamina l’output per garantire che lo scenario sia stato eseguito come previsto.
1. Quando si è certi che lo scenario funziona come previsto, fare clic sul pulsante **Pianificazione** in basso a sinistra dello schermo per **On**.

   Questo attiva lo scenario. Gli scenari attivi vengono eseguiti in base alla pianificazione impostata nel modulo trigger.
1. In entrata [!DNL Workfront Fusion], fai clic su **[!UICONTROL Salva]** nell’angolo in basso a sinistra per salvare i progressi sullo scenario.

   >[!IMPORTANT]
   >
   >Risparmia spesso quando affili e testa uno scenario.

## Risorse:

* [Mappare gli elementi utilizzando le funzioni in [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/mapping/map-information-between-modules.md)
