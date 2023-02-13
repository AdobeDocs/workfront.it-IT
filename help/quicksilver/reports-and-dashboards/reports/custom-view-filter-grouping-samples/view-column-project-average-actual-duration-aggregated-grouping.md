---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Visualizza e raggruppa: visualizza la durata effettiva del progetto aggregata per la media in un raggruppamento"'
description: È possibile aggiungere la colonna seguente in un rapporto di progetto per visualizzare la Durata effettiva aggregata come media in un raggruppamento.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 31794fe9-a04a-437d-8d2e-40e0cb6e6104
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---

# Visualizza e raggruppa: visualizza la durata effettiva del progetto aggregata per la media in un raggruppamento

È possibile aggiungere la colonna seguente in un rapporto di progetto per visualizzare la Durata effettiva aggregata come media in un raggruppamento.

![project_with_aggregate_effettivo_duration_in_group_view.png](assets/project-with-aggregate-actual-duration-in-grouping-view-350x65.png)

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

## Visualizza il progetto Durata effettiva aggregata per la media in un raggruppamento

Per aggiungere questa colonna a una visualizzazione del progetto:

1. (Consigliato) Per ottenere risultati ottimali e visualizzare il valore medio aggregato della Durata effettiva, è necessario aggiungere un raggruppamento all’elenco o al rapporto del progetto.\
   Per ulteriori informazioni sulla creazione dei gruppi, consulta l’articolo [Panoramica sui raggruppamenti in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Passa a una visualizzazione di progetto esistente.
1. Espandi il menu a discesa Visualizza e seleziona **Personalizza visualizzazione**.
1. Fai clic su **Aggiungi colonna**.
1. Fai clic su **Passa alla modalità testo**.
1. Passa il puntatore del mouse sopra **Mostra in questa colonna** e fai clic su **Fare clic per modificare il testo**.

1. Rimuovere tutto il testo nella casella Modalità testo e sostituirlo con il seguente codice:

   <pre>aggregator.displayformat=composto <br>aggregator.function=AVG <br>aggregator.namekey=view.relatedcolumn <br>aggregator.namekeyargkey=attualduration <br>aggregator.valuefield=realDurationMinutes <br>aggregator.valueformat=val <br>displayname=Durata effettiva del progetto <br>durationunitfield=durationUnit.value <br>linkedname=project <br>namekey=realDuration <br>namekeyargkey=realDuration <br>querysort=realDurationMinutes <br>textmode=true <br>valuefield=realDurationMinutes <br>valueformat=composto#M:D <br>viewalias=currentDuration</pre>

1. Fai clic su **Salva visualizzazione**.
