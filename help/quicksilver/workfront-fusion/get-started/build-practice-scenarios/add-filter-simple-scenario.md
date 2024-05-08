---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Aggiungere un filtro a uno scenario di base
description: I filtri ti consentono di garantire che lo scenario avanzi solo se vengono soddisfatte determinate condizioni.
author: Becky
feature: Workfront Fusion
source-git-commit: 5ba5b2e37e2ce58d96d11f24786feef57f8eb638
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 1%

---

# Aggiungere un filtro a uno scenario di base in [!DNL Adobe Workfront Fusion]

I filtri ti consentono di garantire che lo scenario avanzi solo se vengono soddisfatte determinate condizioni.

In questo esempio, aggiungi un filtro allo scenario che consente di creare un nuovo progetto a partire da una richiesta solo se la richiesta è stata inviata a una coda di richieste specifica.

Questo esempio modifica lo scenario creato in [Creare uno scenario di base](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md).

>[!NOTE]
>
>I moduli di attivazione di Workfront includono filtri che consentono l’avvio di uno scenario solo se vengono soddisfatte determinate condizioni. Tuttavia, poiché i filtri tra moduli vengono utilizzati per ogni caso di utilizzo non-trigger e non-Workfront, è importante imparare a utilizzare i filtri tra i moduli. In questo esempio viene utilizzato un filtro tra moduli per la funzionalità che potrebbe essere soddisfatta con un filtro interno al modulo.

## Prerequisiti

Devi creare lo scenario descritto in [Creare uno scenario di base](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) prima di seguire questa procedura.

## Aggiungi un filtro

### Preparare l’aggiunta del filtro

1. Apri il primo scenario.
1. In **Uscite** area, seleziona `Project`.
Ora avresti dovuto `ID`, `Name`, e `Project` selezionato.
1. Scegliere OK per salvare le impostazioni del modulo.
1. Apri Workfront.
1. In Workfront, individua il progetto che rappresenta la coda di richieste con cui lo scenario Fusion lavorerà.

   Il progetto deve trovarsi nello stesso account Workfront per il quale è impostata la connessione Fusion.

1. Prendi nota dell’ID progetto nell’URL.

   Esempio: https://\&lt;mydomain>.my.workfront.com/project/\&lt;projectid>/tasks

### Aggiungere e configurare il filtro

1. Apri lo scenario nell’editor dello scenario.
1. Fai clic sull’icona chiave inglese ![Icona chiave inglese](assets/wrench-icon.png) tra il primo e il secondo modulo e selezionare **Impostare un filtro**.
1. Nel campo Etichetta, immettere un&#39;etichetta per il filtro, ad esempio &quot;Filtra per coda richieste&quot;.
1. In **Condizione** , nel campo superiore, mappa il `projectID` dal primo modulo.

   ![ID progetto mappa](assets/map-proj-id.png)
1. Lascia **Condizione** operatore come Uguale a.
1. Nel campo inferiore della sezione **Condizione** incolla l’ID progetto di cui hai preso nota dall’URL del progetto in [Preparare l’aggiunta del filtro](#prepare-to-add-the-filter).
1. Clic **OK** per salvare le impostazioni del filtro.

### Test e attivazione

1. Vai all’ambiente Workfront a cui si connette Fusion e aggiungi un problema al progetto specificato nel filtro. Aggiungi un altro problema a un altro progetto.
1. Clic **[!UICONTROL Esegui una volta]** nell’angolo inferiore sinistro dell’editor di scenari.
1. Esamina l’output per garantire che lo scenario sia stato eseguito come previsto.

   Entrambi i problemi dovrebbero comparire nell’output del primo scenario, ma solo il problema nel progetto specificato dovrebbe comparire come input nel secondo scenario,
1. Quando si è certi che lo scenario funziona come previsto, fare clic sul pulsante **Pianificazione** in basso a sinistra dello schermo per **On**.

   Questo attiva lo scenario.
1. In entrata [!DNL Workfront Fusion], fai clic su **[!UICONTROL Salva]** nell’angolo in basso a sinistra per salvare i progressi sullo scenario.

   >[!IMPORTANT]
   >
   >Risparmia spesso quando affili e testa uno scenario.

## Risorse

* Per ulteriori informazioni sui filtri, consulta [Aggiungere un filtro a uno scenario](/help/quicksilver/workfront-fusion/scenarios/add-a-filter-to-a-scenario.md).

