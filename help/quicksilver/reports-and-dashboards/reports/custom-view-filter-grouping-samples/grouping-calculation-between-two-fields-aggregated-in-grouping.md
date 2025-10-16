---
content-type: reference
product-area: reporting;projects
keywords: calcolato,aggregati,avanzato,visualizzazioni
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Raggruppamento: visualizza il risultato dell''aggregazione di più valori calcolati in un raggruppamento'
description: È possibile utilizzare la modalità testo in una colonna per visualizzare un calcolo tra due campi nella visualizzazione di un report o di un elenco. Ogni riga visualizza il calcolo per ogni oggetto nel report o nell'elenco.
author: Nolan
feature: Reports and Dashboards
exl-id: e67c0b10-af9f-4657-8f99-8b63ae3c0865
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 0%

---

# Raggruppamento: visualizza il risultato dell’aggregazione di più valori calcolati in un raggruppamento

<!--Audited: 10/2024-->

È possibile utilizzare la modalità testo in una colonna per visualizzare un calcolo tra due campi nella visualizzazione di un report o di un elenco. Ogni riga visualizza il calcolo per ogni oggetto nel report o nell&#39;elenco.

È ad esempio possibile visualizzare la differenza tra le ore effettive e le ore pianificate in una terza colonna denominata Bilanciamento del lavoro per ogni attività in un report attività. Per ulteriori informazioni sulle espressioni di dati calcolati, vedere [Panoramica delle espressioni di dati calcolati](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

È possibile visualizzare il valore aggregato di più elementi della vista calcolata nella stessa colonna in un raggruppamento aggiungendo un calcolo alla riga `aggregator` della colonna che contiene il valore calcolato. È possibile, ad esempio, aggregare (visualizzare la somma di) la quantità di ore del saldo di lavoro di tutti i task nel raggruppamento del report o nell&#39;elenco della colonna Bilancio di lavoro. Questo articolo descrive come eseguire questa operazione.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> 
   <p>Collaboratore o richiesta di modifica di un filtro </p>
   <p>Standard o piano per modificare un rapporto</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari per modificare un rapporto</p> <p>Modificare l’accesso a Filtri, Viste, Raggruppamenti per modificare un filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p>  </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visualizza il risultato dell&#39;aggregazione di più valori calcolati in un raggruppamento

1. Vai a un report attività, fai clic su **Azioni report** > **Modifica**.
1. Nella scheda **Raggruppamenti**, fai clic su **Aggiungi raggruppamento** e inizia a digitare **Nome progetto** nel campo **Raggruppa per**, quindi seleziona **Progetto > Nome** quando viene visualizzato nell&#39;elenco.

1. Nella scheda **Columns(View)**, fai clic su **Aggiungi colonna**, quindi inizia a digitare **Ore pianificate** nel campo **Mostra in questa colonna**, quindi selezionalo quando viene visualizzato nell&#39;elenco.

   >[!TIP]
   >
   >Inizia sempre ad aggiungere tutte le informazioni utilizzando l&#39;interfaccia Standard prima di modificare le informazioni in modalità testo. Aggiungere i campi più vicini o che contengono la maggior parte delle informazioni che si sta tentando di creare per il calcolo.

1. Nel campo **Riepiloga questa colonna per**, selezionare **Somma**.
1. Fare clic su **Passa alla modalità testo** nella colonna aggiunta, quindi fare clic su **Modifica modalità testo**.
1. Sostituire il testo nella casella con il seguente esempio di modalità testo:

   ```
   valueformat=compound
   aggregator.displayformat=minutesAsHoursString
   aggregator.valueexpression=ROUND(({workRequired}-{actualWorkRequired}),2)
   aggregator.function=SUM
   aggregator.valueformat=val
   aggregator.namekey=workrequired
   linkedname=direct
   textmode=true
   valuefield=workRequired
   namekey=workrequired
   valueexpression=CONCAT(ROUND(({workRequired}-{actualWorkRequired})/60,2)," Hours") 
   viewalias=workrequired 
   displayname=Work Balance
   ```

   >[!TIP]
   >
   >Per ottenere il valore aggregato nel raggruppamento per visualizzare la differenza aggregata tra i campi Ore pianificate e Ore effettive, immettere la stessa equazione nella riga `aggregator.valuefield`. Il valore `aggregator.displayformat` utilizzato per la colonna Ore pianificate converte i minuti in ore. Poiché il campo Ore pianificate è stato utilizzato come segnaposto, non è necessario modificare questa riga.
   >
   >
   >La definizione `minutesAsHoursString` della riga `aggregator.displayformat` indica che non è necessario dividere ogni campo per 60 come fatto il `valueexpression` per i risultati. In questo `aggregator.valuefield=workRequired` diventa: `aggregator.valueexpression=ROUND(({workRequired}-{actualWorkRequired}),2`.
1. Fai clic su **Fine**.
1. Fai clic su **Salva+Chiudi**.
