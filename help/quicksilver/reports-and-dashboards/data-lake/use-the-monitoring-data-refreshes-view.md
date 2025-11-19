---
product-area: reports and dashboards
navigation-topic: data-connect
title: Utilizzare la visualizzazione Aggiornamenti dati di monitoraggio in Connessione dati
description: Con Data Connect, gli amministratori di Workfront possono accedere ai record dettagliati degli ultimi aggiornamenti apportati alla data del data del data lake durante l’aggiornamento più recente.
author: Jenny
feature: Reports and Dashboards
source-git-commit: 1bcb64fbcdf2cb8b40cb50e5a7d4f5768f3a712f
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 2%

---

# Utilizzare la visualizzazione Aggiornamenti dati di monitoraggio in Connessione dati

La visualizzazione Aggiornamenti dati di monitoraggio visualizza gli aggiornamenti recenti apportati alla data del data del data lake durante l&#39;aggiornamento più recente. I dati di questa visualizzazione vengono aggiornati dopo ogni completamento corretto di un caricamento di dati.

A causa dell&#39;elevato volume di dati e della complessità delle aggregazioni, la visualizzazione Aggiornamenti dati di monitoraggio mostra solo le visualizzazioni oggetto aggiornate nelle ultime 2 settimane. Se in questa visualizzazione manca un tipo di record specifico, è probabile che ciò sia dovuto a una mancanza di attività in tale arco temporale.

>[!NOTE]
>
>In questa visualizzazione viene visualizzata una raccolta dettagliata dei dati forniti dall&#39;applicazione e vengono aggiornate le attività, anziché una cronologia giornaliera o una visualizzazione eventi che visualizza la cronologia delle attività di aggiornamento. Per ottenere i dettagli cronologici dell&#39;attività di aggiornamento, è possibile utilizzare <code>DL_LOAD_TIMESTAMP</code> oggetto data.

## Monitoraggio dei dati Aggiorna le colonne della vista

Le colonne della vista Aggiornamenti dati di monitoraggio contengono le informazioni seguenti:

<table>
    <tr>
        <td><b>Nome colonna</b></td>
        <td><b>Tipo</b></td>
        <td><b>Descrizione</b></td>
    </tr>
    <tr>
        <td>OBJ_TYPE</td>
        <td>Varchar
        </td>
        <td> 
      Tipo di oggetto associato ai record Workfront inviati al data lake. 
        </ul></td>
    </tr>
    <tr>
        <td>CALENDAR_DATE </td>
        <td>Data</td>
        <td>
   Data dell'ultimo aggiornamento dei dati riuscito per il tipo di oggetto visualizzato nella colonna OBJ_TYPE. </td>
    </tr>
        <tr>
        <td>RECORD_LOAD_TIMESTAMP </td>
        <td>Timestamp_NTZ</td>
        <td>
 Data e ora dell'aggiornamento dati più recente per il tipo di oggetto visualizzato nella colonna OBJ_TYPE.  </td>
    </tr>
        <tr>
        <td>PREVIOUS_RECORD_LOAD_TIMESTAMP </td>
        <td>Timestamp_NTZ </td>
        <td>
       Data e ora del secondo aggiornamento più recente dei dati per il tipo di oggetto visualizzato nella colonna OBJ_TYPE. </td>
    </tr>
        <tr>
        <td>MINUTES_SINCE_PREVIOUS_LOAD </td>
        <td>Numero</td>
        <td>
     Il tempo trascorso in minuti dall'ultimo aggiornamento dei dati per il tipo di oggetto. </td>
    </tr>
            <tr>
        <td>CREATO </td>
        <td>Numero </td>
        <td>Conteggio degli eventi del record CREATE acquisiti tra gli aggiornamenti dei dati precedenti e più recenti per il tipo di oggetto.  </td>
    </tr>
                <tr>
        <td>AGGIORNATO</td>
        <td>Numero </td>
        <td>Un conteggio degli eventi del record UPDATE acquisiti tra gli aggiornamenti dei dati precedenti e più recenti per il tipo di oggetto.</td>
    </tr>
                <tr>
        <td>ELIMINATO</td>
        <td>Numero </td>
        <td>Un conteggio degli eventi del record DELETE acquisiti tra gli aggiornamenti dei dati precedenti e più recenti per il tipo di oggetto. </td>
    </tr>
                <tr>
        <td>TOTALE</td>
        <td>Numero </td>
        <td>Un conteggio del numero totale di eventi tra gli aggiornamenti dei dati precedenti e più recenti per il tipo di oggetto. 
        <br> 
        <br><b>Nota</b>: non corrisponde al numero totale di record interessati dagli eventi CREATE, UPDATE o DELETE, poiché lo stesso record può essere CREATO e AGGIORNATO più volte nell'intervallo tra gli aggiornamenti.  </td>
    </tr>
   </table>

