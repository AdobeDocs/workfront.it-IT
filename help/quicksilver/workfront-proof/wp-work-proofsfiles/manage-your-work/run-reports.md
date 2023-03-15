---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: Eseguire report in [!DNL Workfront Proof]
description: Workfront Proof consente di visualizzare i rapporti in modo da poter tenere traccia dell’avanzamento del lavoro e dell’efficienza dei team.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 342f9282-b6f5-425e-a7ef-e23bd011d284
source-git-commit: a0d76692f9e9d12ed0d538c1344638dbc208d625
workflow-type: tm+mt
source-wordcount: '691'
ht-degree: 0%

---

# Eseguire report in [!DNL Workfront Proof]


>[!IMPORTANT]
>
>* <span class="previe">La funzionalità di reporting non è più disponibile in [!DNL Workfront Proof]. La scheda di reporting continua a essere visualizzata, ma i dati non sono precisi.</span>
> 
>* Questo articolo fa riferimento alla funzionalità del prodotto standalone [!DNL Workfront Proof]. Per informazioni sulle prove all&#39;interno [!DNL Adobe Workfront], vedi [Copertura](../../../review-and-approve-work/proofing/proofing.md).


Workfront Proof consente di visualizzare i rapporti in modo da poter tenere traccia dell’avanzamento del lavoro e dell’efficienza dei team.

Puoi facilmente visualizzare il numero di bozze create nel tuo [!DNL Workfront Proof] account, quante versioni sono associate a ogni bozza, il tempo di consegna e altro ancora.

## Prerequisiti

La disponibilità di rapporti dipende dal tipo di [!DNL Workfront Proof] livelli di autorizzazione dell&#39;account e dell&#39;utente.

* [Prerequisiti per l’account](#account-prerequisites)
* [Prerequisiti utente](#user-prerequisites)

### Prerequisiti per l’account {#account-prerequisites}

Le informazioni sui rapporti sono disponibili solo con i piani Premium.

### Prerequisiti utente {#user-prerequisites}

Le informazioni di reporting sono disponibili solo per gli utenti con accesso completo a tutte le bozze sul tuo account (ad esempio gli utenti con almeno [Profili delle autorizzazioni di prova in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)).

In questo pannello puoi

* Controllare l&#39;intervallo di tempo dei dati visualizzati
* Analizzare le modifiche nelle metriche nel tempo
* Controlla i dettagli di un punto nel tempo selezionato passando il cursore sopra di esso
* Controlla il numero totale di bozze create nell&#39;intervallo di tempo selezionato
* Controlla il numero medio di versioni incluse nei set di bozze completati

## Visualizzazione dei rapporti {#viewing-reports}

1. Vai a **[!UICONTROL Dashboard]** pagina.
1. Fai clic sul pulsante **[!UICONTROL Rapporti]** scheda .\
   ![proof_reports.png](assets/proof-reports-350x193.png)

1. In **[!UICONTROL Intervallo temporale]** menu a discesa, seleziona se desideri visualizzare informazioni sulle bozze create nelle ultime 24 ore, 7 giorni, 30 giorni, 90 giorni o un periodo di tempo personalizzato.\
   Se selezioni un periodo di tempo personalizzato, seleziona le date di inizio e di fine, quindi fai clic su **[!UICONTROL Applica]**.\
   Vengono visualizzate le seguenti informazioni per il periodo di tempo selezionato:\
   **Prova creata:** Numero di bozze create nel periodo di tempo selezionato.\
   **Versioni per bozza:** Numero medio di versioni per bozza per tutte le bozze completate (Approvate o Approvate con modifiche) nel periodo di tempo selezionato.\
   **Volta Intorno:** Tempo medio dal momento in cui è stata creata la prima versione al momento in cui è stata presa la decisione sulla versione finale.\
   **Data e ora della prima attività:** Tempo medio dalla creazione della bozza all’ora della prima attività della bozza.\
   **Prove in ritardo:** Percentuale media di bozze completate (approvate o approvate con modifiche) con almeno una versione in ritardo nel periodo di tempo selezionato.\
   **Commenti e risposte:** Numero medio di commenti e risposte che sono stati effettuati su tutte le bozze nel periodo di tempo selezionato.

1. (Facoltativo) Seleziona o deseleziona la **[!UICONTROL Mostra gamma min-max]** per determinare se i valori minimo e massimo sono visualizzati nel grafico.\
   Quando questa opzione è selezionata, viene visualizzata un&#39;ombreggiatura blu tra i valori registrati minimo e massimo.

1. (Facoltativo) Puoi filtrare i dati visualizzati, come descritto in [Rapporti sui filtri](#filtering-reports).

## Rapporti sui filtri {#filtering-reports}

Per impostazione predefinita, i dati visualizzati nei rapporti includono tutte le informazioni provenienti dal [!DNL Workfront Proof] sistema. Puoi utilizzare i filtri per mostrare solo le informazioni pertinenti alle tue esigenze.

Per filtrare le informazioni di reporting:

1. Vai a **[!UICONTROL Dashboard]** pagina.
1. Fai clic sul pulsante **[!UICONTROL Rapporti]** scheda .\
   ![proof_reports.png](assets/proof-reports-350x193.png)

1. Esegui un rapporto come descritto in [Visualizzazione dei rapporti](#viewing-reports).
1. Fai clic su **[!UICONTROL Filtro]**.

1. Sul lato sinistro della pagina, seleziona una delle seguenti opzioni di filtro:\
   **[!UICONTROL Tipo di bozza]:** Seleziona il tipo di bozze da includere nel rapporto.\
   **[!UICONTROL Decisioni]:** Selezionare le opzioni per determinare se sono state effettuate solo bozze contenenti determinate decisioni.\
   **[!UICONTROL Destinatari]:** Seleziona i singoli utenti per visualizzare le informazioni relative alle bozze condivise con gli utenti selezionati.\
   **[!UICONTROL Proprietari di bozza]:** Seleziona i singoli utenti per visualizzare le informazioni relative alle bozze di proprietà degli utenti selezionati.\
   **[!UICONTROL Creatori di prove]:** Seleziona i singoli utenti per visualizzare le informazioni relative alle bozze create dagli utenti selezionati.\
   **[!UICONTROL Account]:** Selezionare gli account da includere nel rapporto.

1. Fai clic su **[!UICONTROL Applica]**.
1. (Facoltativo) Seleziona o deseleziona la **[!UICONTROL Mostra gamma min-max]** per determinare se i valori minimo e massimo sono visualizzati nel grafico.\
   Quando questa opzione è selezionata, viene visualizzata un&#39;ombreggiatura blu tra i valori registrati minimo e massimo.

## Stampa dei report

1. Vai a **[!UICONTROL Dashboard]** pagina.
1. Fai clic sul pulsante **[!UICONTROL Rapporti]** scheda , quindi fai clic su **[!UICONTROL Stampa]**.\
   ![proof_reports_print.png](assets/proof-reports-print-350x191.png)

1. Selezionare tra le varie opzioni di stampa disponibili.\
   Le opzioni di stampa variano a seconda del browser e della versione del browser in uso.
