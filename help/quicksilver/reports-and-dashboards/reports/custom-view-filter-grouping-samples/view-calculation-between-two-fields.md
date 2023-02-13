---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Visualizza: visualizza il risultato di un calcolo tra due campi in una colonna"'
description: È possibile utilizzare la modalità testo in una colonna per visualizzare un calcolo tra due campi.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 303f8824-311a-4de0-9777-cfa11ecad1e1
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 0%

---

# Visualizza: visualizzare il risultato di un calcolo tra due campi in una colonna

È possibile utilizzare la modalità testo in una colonna per visualizzare un calcolo tra due campi.

Ad esempio, per scoprire il numero di giorni della settimana trascorsi tra due date, è possibile utilizzare la sintassi della modalità testo e le espressioni dati per calcolare questa differenza.\
Ad esempio, è possibile calcolare la differenza del giorno della settimana tra la data di completamento pianificata e la data di completamento effettivo di un&#39;attività e visualizzare il risultato in una colonna.

In questo calcolo è possibile utilizzare altre due date (Inizio effettivo, Completamento effettivo, Inizio previsto, Completamento previsto, Completamento previsto, ecc.).\
Per ulteriori informazioni sulle espressioni dati calcolate, consulta [Espressioni dati calcolate](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

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

## Visualizza il risultato di un calcolo tra due campi in una colonna

Per aggiungere questa colonna a una visualizzazione attività:

1. Passare a un elenco di attività.
1. Da **Visualizza** menu a discesa, fai clic su **Nuova vista**.

1. Fai clic su **Aggiungi colonna**, quindi **Passa alla modalità testo**.

1. Passa il puntatore del mouse sull’area della modalità testo e fai clic su **Fare clic per modificare il testo**.
1. Rimuovi il testo che trovi nella **Modalità testo** e sostituirlo con il seguente codice:
   <pre>displayname=Differenza giornaliera settimanale<br>textmode=true<br>valueexpression=WEEKDAYDIFF({scheduledCompletionDate},{effectiveCompletionDate})<br>valueformat=HTML</pre>

1. (Facoltativo) Per aggregare i valori visualizzati nella visualizzazione in un raggruppamento, segui i passaggi descritti in [Raggruppamento: visualizzare il risultato dell&#39;aggregazione di più valori calcolati in un raggruppamento](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-calculation-between-two-fields-aggregated-in-grouping.md).
1. Fai clic su **Salva**, quindi **Salva visualizzazione**.
