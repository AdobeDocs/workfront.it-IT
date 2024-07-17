---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Visualizza e raggruppa: visualizza la durata effettiva del progetto aggregata in base alla media in un raggruppamento"
description: È possibile aggiungere la colonna seguente in un report di progetto per visualizzare la durata effettiva aggregata come media in un raggruppamento.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 31794fe9-a04a-437d-8d2e-40e0cb6e6104
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 1%

---

# Visualizza e raggruppa: visualizza la durata effettiva del progetto aggregata in base alla media in un raggruppamento

È possibile aggiungere la colonna seguente in un report di progetto per visualizzare la durata effettiva aggregata come media in un raggruppamento.

![project_with_aggregate_actual_duration_in_grouping_view.png](assets/project-with-aggregate-actual-duration-in-grouping-view-350x65.png)

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
   <td> <p>Richiesta di modifica di una vista </p>
   <p>Pianificare la modifica di un rapporto</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari per modificare un rapporto</p> <p>Modificare l'accesso a Filtri, Viste, Raggruppamenti per modificare una vista</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

## Visualizza la durata effettiva del progetto aggregata in base alla media in un raggruppamento

Per aggiungere questa colonna a una visualizzazione di progetto:

1. (Consigliato) Per ottenere risultati migliori e vedere il valore medio aggregato della Durata effettiva, devi avere un Raggruppamento aggiunto all’elenco o al rapporto del progetto.\
   Per ulteriori informazioni sulla creazione di raggruppamenti, vedere l&#39;articolo [Panoramica sui raggruppamenti in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Passa a una visualizzazione di progetto esistente.
1. Espandere il menu a discesa Visualizza e selezionare **Personalizza visualizzazione**.
1. Fare clic su **Aggiungi colonna**.
1. Fare clic su **Passa alla modalità testo**.
1. Passa il puntatore del mouse sull&#39;area **Mostra in questa colonna** e fai clic su **Fai clic per modificare il testo**.

1. Rimuovere tutto il testo nella casella Modalità testo e sostituirlo con il seguente codice:
   <pre>aggregator.displayformat=composto <br>aggregator.function=AVG <br>aggregator.namekey=view.relatedcolumn <br>aggregator.namekeyargkey=actualduration <br>aggregator.valuefield=actualDurationMinutes <br>aggregator.valueformat=val <br>displayname=Project Actual Duration <br>durationunitfield=durationUnit.value <br>linkedname=project <br>namekey=actualduration <br>namekeyargkey=actualduration <br>querysort=actualDuration Min<br>textmode=true <br>valuefield=actualDurationMinutes <br>valueformat=composto#M:D <br>viewalias=actualduration</pre>

1. Fai clic su **Salva vista**.
