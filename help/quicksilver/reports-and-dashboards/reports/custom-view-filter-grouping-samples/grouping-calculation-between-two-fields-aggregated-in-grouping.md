---
content-type: reference
product-area: reporting;projects
keywords: calcolato,aggregati,avanzato,visualizzazioni
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Raggruppamento: visualizza il risultato dell''aggregazione di più valori calcolati in un raggruppamento'''
description: È possibile utilizzare la modalità testo in una colonna per visualizzare un calcolo tra due campi nella visualizzazione di un rapporto o di un elenco. Ciascuna riga visualizza il calcolo per ciascun oggetto del rapporto o dell’elenco.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e67c0b10-af9f-4657-8f99-8b63ae3c0865
source-git-commit: 89a6d856f9f87a67b6a2ccfb4282f9f6200b977c
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 0%

---

# Raggruppamento: visualizzare il risultato dell&#39;aggregazione di più valori calcolati in un raggruppamento

È possibile utilizzare la modalità testo in una colonna per visualizzare un calcolo tra due campi nella visualizzazione di un rapporto o di un elenco. Ciascuna riga visualizza il calcolo per ciascun oggetto del rapporto o dell’elenco.

Ad esempio, è possibile visualizzare la differenza tra Ore effettive e Ore pianificate in una terza colonna denominata Saldo del lavoro per ogni attività in un rapporto di attività. Per ulteriori informazioni sulle espressioni dati calcolate, consulta [Espressioni dati calcolate](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

È possibile visualizzare il valore aggregato di più elementi di visualizzazione calcolati nella stessa colonna di un raggruppamento aggiungendo un calcolo al gruppo `aggregator` della colonna contenente il valore calcolato. Ad esempio, è possibile aggregare (visualizzare la somma di) la quantità di ore di bilanciamento del lavoro di tutte le attività nel raggruppamento del rapporto o nell&#39;elenco della colonna Saldo del lavoro. Questo articolo descrive come farlo.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Accesso a rapporti, dashboard, calendari</p> <p>Modificare l’accesso a Filtri, Visualizzazioni, Gruppi</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Visualizza il risultato dell&#39;aggregazione di più valori calcolati in un raggruppamento

1. Passa a un rapporto attività e fai clic su **Azioni dei rapporti** > **Modifica**.
1. In **Raggruppamenti** scheda , fai clic su **Aggiungi raggruppamento** e inizia a digitare **Nome progetto** in **Raggruppa il rapporto** > **Primo da** , quindi selezionalo quando viene visualizzato nell’elenco.

1. In **Colonne (visualizzazione)** scheda , fai clic su **Aggiungi colonna**, quindi inizia a digitare **Orari pianificati** in **Mostra in questa colonna** , quindi selezionalo quando viene visualizzato nell’elenco.

   >[!TIP]
   >
   >Inizia sempre ad aggiungere tutte le informazioni utilizzando l’interfaccia Standard prima di modificare le informazioni in modalità testo. Aggiungi i campi più vicini o contenenti la maggior parte delle informazioni per il calcolo che stai tentando di eseguire.

1. In **Riepiloga questa colonna per** campo , seleziona **Somma**, quindi fai clic su **Fine**.
1. Fai clic su **Passa alla modalità testo** nella colonna aggiunta.
1. Passa il puntatore del mouse sull’area della modalità testo e fai clic su **Fare clic per modificare il testo**.
1. Sostituisci il `valuefield ` e `aggregator.valuefield` le linee con le linee evidenziate nel seguente esempio di modalità testo:

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
   valueexpression=CONCAT(ROUND(({workRequired}-{actualWorkRequired})/60,2)," Hours") viewalias=workrequired displayname=Work Balance
   ```

   >[!TIP]
   >
   >Per ottenere il valore aggregato nel raggruppamento in modo da visualizzare la differenza aggregata tra i campi Ore programmate e Ore effettive, inserire la stessa equazione nel campo `aggregator.valuefield` linea. La `aggregator.displayformat` utilizzato per la colonna Ora pianificata converte i minuti in ore. Poiché il campo Ora pianificata è stato utilizzato come segnaposto, non è necessario modificare questa riga.
   >
   >
   >La `minutesAsHoursString` definizione della `aggregator.displayformat` linea significa che non è necessario dividere ogni campo per 60 come fatto sul `valueexpression` per i risultati. In questo `aggregator.valuefield=workRequired` diventa: `aggregator.valueexpression=ROUND(({workRequired}-{actualWorkRequired}),2`.

1. Fai clic su **Salva e chiudi**.
