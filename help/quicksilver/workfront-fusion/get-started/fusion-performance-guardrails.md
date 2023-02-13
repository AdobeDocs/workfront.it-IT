---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: scenario,prestazioni
navigation-topic: get-started-with-workfront-fusion-2-0
title: Protezione delle prestazioni di Adobe Workfront Fusion
description: Adobe Workfront Fusion richiede una licenza Adobe Workfront Fusion oltre a una licenza Adobe Workfront.
author: Becky
feature: Workfront Fusion
exl-id: cdf46eb1-46ba-4707-9063-b76899195a2c
source-git-commit: 229fd48d604385a1bfcaba2fd34eb6f3bbdde7a7
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] protezioni delle prestazioni

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] richiede un [!DNL Adobe Workfront Fusion] oltre a una licenza [!DNL Adobe Workfront license].

L&#39;automazione del lavoro richiede un&#39;elaborazione rapida, quindi [!DNL Adobe Workfront Fusion] è progettato per prestazioni elevate. Poiché gli scenari a lungo termine possono rallentare il ritmo del tuo lavoro, abbiamo progettato [!DNL Workfront Fusion] con protezioni che consentono di mantenere le prestazioni che limitano i tempi di esecuzione, le dimensioni dei dati e altri parametri dello scenario. [!DNL Workfront Fusion] i progettisti devono essere consapevoli di tali protezioni e incorporarle nelle loro pratiche di progettazione.

## Scenari

* Il timeout predefinito di esecuzione dello scenario è **40 minuti**. Quando l’esecuzione raggiunge questo timeout, [!DNL Workfront Fusion] interrompe l&#39;esecuzione dello scenario dopo il ciclo o l&#39;operazione successiva, a seconda dello scenario. Questo costringe lo scenario a interrompersi poco dopo il raggiungimento del limite di 40 minuti
* La dimensione massima di una blueprint dello scenario è **5 MB**, ma si consiglia di mantenere le dimensioni dello scenario sotto **3 MB**.

   I moduli di app che creano o aggiornano dati con un numero elevato di campi possono causare blueprint molto grandi.

   * Quando utilizzi [!DNL Workfront] app, assicurati di selezionare solo i campi necessari per i casi d’uso di creazione o aggiornamento.
   * Quando utilizzi altre app, utilizza moduli API personalizzati per interagire con qualsiasi tipo di record con un numero elevato di campi.

* Sebbene non vi sia un limite per il numero di moduli in uno scenario, gli scenari con più di 150 moduli influiscono negativamente sulle prestazioni del [!DNL Workfront Fusion] sistema. Per questo motivo, si sconsiglia di creare scenari con oltre 150 moduli.

## Operazioni

* Il timeout predefinito dell’operazione è in genere **40 secondi**.

<!--
* The operation timeout for calls to Adobe Workfront is **120 seconds**.
-->

## File

* La capacità totale di elaborazione dei file di Fusion è **1 GB**. Il limite si basa su un costo totale della memoria. Ogni operazione contribuisce a questo costo. Se un singolo file di 400 MB viene scaricato e caricato, il costo totale per la capacità del file sarà di 800 MB.

## Utilizzo della memoria del server

* L&#39;utilizzo della memoria del server per una singola esecuzione è limitato a **1 GB**.

   Molti fattori, come file di grandi dimensioni o moduli complessi, possono influenzare l&#39;utilizzo della memoria del server in modi difficili da prevedere o controllare. Per questo motivo, l&#39;esecuzione dello scenario può superare il limite di memoria di 1 GB, anche se lo scenario segue tutte le altre protezioni delle prestazioni. Se si supera il limite di memoria, l&#39;esecuzione non riesce.

## Webhook

* La dimensione massima predefinita di un payload è **5 MB**.
* I webhook sono limitati a **100 richieste al secondo**. Al raggiungimento di questo limite, Workfront Fusion invia un 429 ([!UICONTROL Troppe richieste]).
* [!DNL Workfront Fusion] memorizza payload webhook per 30 giorni. L&#39;accesso a un payload webhook più di 30 giorni dopo la ricezione restituisce risultati nell&#39;errore &quot;[!UICONTROL Impossibile leggere il file dall&#39;archivio.]&quot;
* I webhook vengono disattivati automaticamente se si applica una delle seguenti funzioni:

   * Il webhook non è stato collegato ad alcuno scenario per più di 5 giorni
   * Il webhook viene utilizzato solo in scenari inattivi, che sono stati inattivi per più di 30 giorni.

* I webhook disattivati vengono eliminati e non registrati automaticamente se non sono connessi ad alcuno scenario e sono stati disattivati per più di 30 giorni.
