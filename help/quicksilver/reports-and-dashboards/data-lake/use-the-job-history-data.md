---
product-area: reports and dashboards
navigation-topic: data-connect
title: Utilizzare la visualizzazione Cronologia processo in Connessione dati
description: Con Data Connect, gli amministratori di Workfront possono accedere ai record dettagliati di ogni processo di aggiornamento dei dati nella visualizzazione Cronologia processo.
author: Jenny
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
source-git-commit: 05cf34fe6659c50da76d2478c6e79352346dc9a5
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 0%

---

# Utilizzare la visualizzazione Cronologia processo in Connessione dati

Nella visualizzazione Cronologia job, gli amministratori di Workfront possono accedere ai record dettagliati di ciascun job di aggiornamento dei dati. Questi record forniscono ad insight importanti funzionalità per i processi che consentono di mantenere aggiornati i dati e di stabilire i tempi ideali per l’esecuzione dei processi e l’aggiornamento delle visualizzazioni aziendali.

![Visualizzazione cronologia processo](assets/job-history-overview.png)

Le colonne della vista Cronologia processo contengono le seguenti informazioni:

* **NOME_OGGETTO**: visualizza il nome dell&#39;oggetto associato al processo.
* **SCHEDULED_TIME**: visualizza l&#39;ora di inizio del processo.
* **COMPLETED_TIME**: visualizza l&#39;ora di completamento del processo.
* **ULTIMO_FLAG**: indica se il processo faceva parte dell&#39;aggiornamento più recente.
* **STATO**: visualizza lo stato del processo. Per ulteriori informazioni, vedere la seguente sezione in questo articolo: [Stati dei processi disponibili](#available-job-statuses).
* **LAST_UPDATED**: timestamp dell&#39;ultimo aggiornamento del processo.

>[!NOTE]
>
>La visualizzazione Cronologia processi include i dettagli relativi alle 72 ore precedenti di processi pianificati.


## Stati dei processi disponibili

A ogni processo di connessione dati viene assegnato uno stato che indica se è stato eseguito correttamente, ignorato o non riuscito.

<table>
    <tr>
        <td><b>Stato del processo</b></td>
        <td><b>Definizione</b></td>
    </tr>
    <tr>
        <td>Completato</td>
        <td>Il processo ha elaborato correttamente ogni aggiornamento disponibile e tutti gli aggiornamenti per quel tipo di record ora vengono rispecchiati nel data lake.</td>
    </tr>
    <tr>
        <td>Ignorato</td>
        <td>Il processo è stato ignorato perché non sono presenti aggiornamenti in coda da elaborare per il tipo di record.</td>
    </tr>
    <tr>
        <td>Non riuscito</td>
        <td>Impossibile eseguire il processo. In questi casi, è probabile che non sia stato eseguito il commit dei dati in coda nel data lake. I record che rimangono in coda verranno elaborati nel successivo processo pianificato per quel tipo di record. </td>
    </tr>
   </table>


## Considerazioni sull’esecuzione dei processi e sul comportamento di registrazione

Snowflake utilizza uno strumento di ottimizzazione dell’utilità di pianificazione dei processi che può influenzare il modo in cui l’esecuzione dei processi viene elaborata e registrata nella visualizzazione Cronologia processi. Questo comportamento di registrazione può variare a seconda che siano presenti o meno dati da elaborare.

Ad esempio, se non sono presenti nuove righe da elaborare per un determinato oggetto, può verificarsi uno dei seguenti risultati:

* **Il processo viene eseguito ed è contrassegnato come Ignorato**: Snowflake rileva che non sono presenti righe da elaborare, esegue il processo e lo registra con lo stato Ignorato nella tabella.

* **Processo non eseguito**: Snowflake determina che non sono presenti righe da elaborare, non esegue il processo e lo registra con lo stato Ignorato nella tabella.

  >[!NOTE]
  >
  >Nel secondo caso in cui il processo non viene eseguito, il record più recente per l&#39;oggetto potrebbe riflettere una marca temporale non allineata alla pianificazione prevista.

In altre parole, un processo può essere considerato eseguito anche se non sono state elaborate righe e può essere registrato a seconda del comportamento dell&#39;utilità di pianificazione del processo per quel particolare processo.