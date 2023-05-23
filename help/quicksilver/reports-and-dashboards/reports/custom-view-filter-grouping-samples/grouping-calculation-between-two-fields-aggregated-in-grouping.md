---
content-type: reference
product-area: reporting;projects
keywords: calcolato,aggregati,avanzato,visualizzazioni
navigation-topic: custom-view-filter-and-grouping-samples
title: "Raggruppamento: visualizza il risultato dell’aggregazione di più valori calcolati in un raggruppamento"
description: È possibile utilizzare la modalità testo in una colonna per visualizzare un calcolo tra due campi nella visualizzazione di un report o di un elenco. Ogni riga visualizza il calcolo per ogni oggetto nel report o nell'elenco.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e67c0b10-af9f-4657-8f99-8b63ae3c0865
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '590'
ht-degree: 0%

---

# Raggruppamento: visualizza il risultato dell’aggregazione di più valori calcolati in un raggruppamento

È possibile utilizzare la modalità testo in una colonna per visualizzare un calcolo tra due campi nella visualizzazione di un report o di un elenco. Ogni riga visualizza il calcolo per ogni oggetto nel report o nell&#39;elenco.

È ad esempio possibile visualizzare la differenza tra le ore effettive e le ore pianificate in una terza colonna denominata Bilanciamento del lavoro per ogni attività in un report attività. Per ulteriori informazioni sulle espressioni di dati calcolati, vedi [Espressioni dati calcolate](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

È possibile visualizzare il valore aggregato di più elementi della vista calcolata nella stessa colonna in un raggruppamento aggiungendo un calcolo alla `aggregator` riga della colonna contenente il valore calcolato. È possibile, ad esempio, aggregare (visualizzare la somma di) la quantità di ore del saldo di lavoro di tutti i task nel raggruppamento del report o nell&#39;elenco della colonna Bilancio di lavoro. Questo articolo descrive come eseguire questa operazione.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Richiesta di modifica di un raggruppamento </p>
   <p>Pianificare la modifica di un rapporto</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari per modificare un rapporto</p> <p>Modifica l'accesso a Filtri, Viste, Raggruppamenti per modificare un raggruppamento</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

## Visualizza il risultato dell&#39;aggregazione di più valori calcolati in un raggruppamento

1. Passare a un report di attività e fare clic su **Azioni report** > **Modifica**.
1. In **Raggruppamenti** , fare clic su **Aggiungi raggruppamento**, e inizia a digitare **Nome progetto** nel **Raggruppa il report** > **Primo da** , quindi selezionarlo quando viene visualizzato nell&#39;elenco.

1. In **Columns(View)** , fare clic su **Aggiungi colonna**, quindi inizia a digitare **Ore pianificate** nel **Mostra in questa colonna** , quindi selezionarlo quando viene visualizzato nell&#39;elenco.

   >[!TIP]
   >
   >Inizia sempre ad aggiungere tutte le informazioni utilizzando l&#39;interfaccia Standard prima di modificare le informazioni in modalità testo. Aggiungere i campi più vicini o che contengono la maggior parte delle informazioni che si sta tentando di creare per il calcolo.

1. In **Riepiloga questa colonna per** campo, seleziona **Somma**, quindi fai clic su **Fine**.
1. Clic **Passa alla modalità testo** nella colonna aggiunta.
1. Passa il puntatore del mouse sull’area della modalità testo e fai clic su **Fare clic per modificare il testo**.
1. Sostituisci il `valuefield ` e `aggregator.valuefield` le righe con le righe evidenziate nel seguente esempio di modalità testo:

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
   >Per ottenere il valore aggregato nel raggruppamento e visualizzare la differenza aggregata tra i campi Ore pianificate e Ore effettive, immettere la stessa equazione nel campo `aggregator.valuefield` linea. Il `aggregator.displayformat` utilizzato per la colonna Ore pianificate converte i minuti in ore. Poiché il campo Ore pianificate è stato utilizzato come segnaposto, non è necessario modificare questa riga.
   >
   >
   >Il `minutesAsHoursString` definizione del `aggregator.displayformat` riga significa che non è necessario dividere ogni campo per 60 come fatto sul `valueexpression` per i risultati. In questo `aggregator.valuefield=workRequired` diventa: `aggregator.valueexpression=ROUND(({workRequired}-{actualWorkRequired}),2`.

1. Clic **Salva+Chiudi**.
