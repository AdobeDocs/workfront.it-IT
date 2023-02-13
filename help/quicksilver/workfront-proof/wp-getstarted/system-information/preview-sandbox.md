---
content-type: overview;how-to-procedural
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: system-information
title: Ambiente di test sandbox di anteprima [!DNL Workfront Proof]
description: La Sandbox Anteprima è un ambiente di test che funge da replica dell’ambiente live e viene aggiornato ogni fine settimana per [!DNL Workfront Proof].
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: cdf269c6-39b1-477a-b9ea-03edf2de77f0
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 0%

---

# Ambiente di test sandbox di anteprima [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Questo articolo fa riferimento alla funzionalità del prodotto standalone [!DNL Workfront Proof]. Per informazioni sulle prove all&#39;interno [!DNL Adobe Workfront], vedi [Copertura](../../../review-and-approve-work/proofing/proofing.md).

La Sandbox Anteprima è un ambiente di test che funge da replica dell’ambiente live e viene aggiornato ogni fine settimana per [!DNL Workfront Proof].

## Informazioni sulla sandbox di anteprima

La Sandbox di anteprima funge da ambiente in cui gli utenti della tua organizzazione possono eseguire in modo sicuro il test e lavorare con i dati dell’ambiente di produzione senza influire sull’ambiente di produzione. È ideale per eseguire sessioni di formazione, testare le nuove funzioni e determinare le funzionalità di configurazione.

Inoltre, le nuove funzioni del prodotto vengono caricate nell’ambiente Sandbox di anteprima prima che vengano distribuite nell’ambiente di produzione. Gli utenti possono provare nuove funzionalità senza influire sul flusso di lavoro abituale nell&#39;ambiente di produzione.

La sandbox Anteprima contiene i dati di produzione effettivi. I dati scorrono da Produzione a Anteprima e non al contrario. Si aggiorna ogni weekend, in modo che i dati possano essere fino a una settimana dietro l&#39;ambiente di produzione. Gli elementi creati dopo l’ultimo aggiornamento si trovano nell’ambiente Sandbox di anteprima fino al successivo aggiornamento.

## Accesso alla Sandbox di anteprima

Per impostazione predefinita, in qualità di amministratore di sistema, puoi accedere all’ambiente Sandbox di anteprima. Se non riesci ad accedere all’ambiente Sandbox di anteprima come descritto in questa sezione, contatta il [!DNL Workfront] amministratore o il nostro team di assistenza.

* [Accesso alla Sandbox di anteprima come stand-alone [!DNL Workfront Proof] Cliente](#accessing-the-preview-sandbox-as-a-stand-alone-workfront-proof-customer)
* [Accesso alla Sandbox di anteprima come [!DNL Workfront]+[!DNL Workfront Proof] Cliente](#accessing-the-preview-sandbox-as-a-workfrontworkfront-proof-customer)

### Accesso alla Sandbox di anteprima come stand-alone [!DNL Workfront Proof] Cliente

1. Passa a questo URL:  `https://preview.proofhq.com`.
1. Accedi utilizzando le tue credenziali di anteprima.\
   Le credenziali di anteprima devono corrispondere alle credenziali di produzione, a meno che non siano state modificate in Produzione dopo l’aggiornamento dell’anteprima. Gli accessi vengono sincronizzati solo quando si verifica un aggiornamento, che avviene ogni fine settimana. Non si sincronizzano automaticamente.

### Accesso alla Sandbox di anteprima come [!DNL Workfront+Workfront] Cliente di prova

In qualità di amministratore di sistema, puoi accedere al [!DNL Workfront Proof] Anteprima sandbox tramite [!DNL Workfront] interfaccia.

Per accedere al [!DNL Workfront Proof] Sandbox di anteprima:

1. Accedi al tuo [!DNL Workfront] ambiente.
1. Fai clic su **[!UICONTROL Configurazione]** nella barra di navigazione globale.
1. Fai clic su **[!UICONTROL Sistema]** >**[!UICONTROL Preferenze]**.

1. In **[!UICONTROL Ambienti di test]** sezione, fai clic su **[!UICONTROL Anteprima sandbox]**.

1. Accedi con le tue credenziali di anteprima.\
   Le credenziali di anteprima devono essere uguali alle credenziali di produzione, a meno che non siano state modificate in Produzione dopo l’aggiornamento dell’anteprima. Gli accessi vengono sincronizzati solo quando si verifica un aggiornamento. Non si sincronizzano automaticamente.
1. Fai clic sul pulsante [!DNL Workfront Proof] nella barra di navigazione globale.\
   ![proof_access_proofhq.png](assets/proof-access-proofhq-350x39.png)\
   La [!DNL Workfront Proof] Viene visualizzato l’ambiente di anteprima.

## Ricezione di e-mail dalla Sandbox di anteprima

Le notifiche e-mail non vengono mai attivate dal [!DNL Workfront Proof] Ambiente di anteprima.
