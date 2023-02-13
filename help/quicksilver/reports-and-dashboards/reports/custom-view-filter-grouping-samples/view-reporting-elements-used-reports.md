---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Visualizza: elementi di reporting utilizzati nei rapporti'
description: In questa visualizzazione vengono visualizzati la visualizzazione, il filtro e il raggruppamento utilizzati per creare ogni rapporto in Adobe Workfront quando lo si utilizza in un elenco di rapporti.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 67f86523-e136-4768-af93-586a107b106f
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 0%

---

# Visualizza: elementi di reporting utilizzati nei rapporti

In questa visualizzazione vengono visualizzati la visualizzazione, il filtro e il raggruppamento utilizzati per creare ogni rapporto in Adobe Workfront quando lo si utilizza in un elenco di rapporti.

È possibile visualizzare le

```
valuefields
```

oppure

```
valueexpressions
```

utilizzato in ogni elemento del rapporto.

![report_with_elements_definitions.png](assets/report-with-elements-definitions-350x130.png)

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

## Visualizzare gli elementi di reporting utilizzati nei rapporti

1. Passa a un elenco di rapporti.
1. Da **Visualizza** menu a discesa, seleziona **Nuova vista**.

1. In **Anteprima a colonne** eliminare tutte le colonne tranne una.
1. Fai clic sull’intestazione della colonna rimanente, quindi fai clic su **Passa alla modalità testo**.
1. Passa il puntatore del mouse sull’area della modalità testo e fai clic su **Fare clic per modificare il testo**.
1. Rimuovi il testo che trovi nella **Modalità testo** e sostituirlo con il seguente codice:
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=string<br>column.0.link.lookup=link.run<br>column.0.link.value=val(objCode)<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=200<br>column.1.descriptionkey=oggttype<br>column.1.listsort=nidificato(view).string(uiObjCode)<br>column.1.namekey=objectType.abbr<br>column.1.querysort=uiObjCode<br>column.1.valuefield=uiObjCode<br>column.1.valueformat=objCodeMessage<br>column.1.width=80<br>column.2.descriptionkey=enteredby<br>column.2.listsort=nidificato(enterBy).string(lastName)<br>column.2.namekey=enteredby.abbr<br>column.2.querysort=enterBy:lastName<br>column.2.valuefield=enterBy:name<br>column.2.valueformat=HTML<br>column.2.width=130<br>column.3.displayname=Definizione del filtro<br>column.3.textmode=true<br>column.3.valuefield=filter:definition<br>column.3.valueformat=HTML<br>column.4.displayname=View definition<br>column.4.textmode=true<br>column.4.valuefield=view:definition<br>column.4.valueformat=HTML<br>column.5.displayname=Definizione di raggruppamento<br>column.5.textmode=true<br>column.5.valueField=groupBy:definition<br>column.5.valueformat=HTML<br></pre>

1. Fai clic su **Salva visualizzazione**.
