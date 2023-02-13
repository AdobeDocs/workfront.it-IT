---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: "Visualizza: Società e gruppo home dell'utente assegnato"
description: In questa visualizzazione attività vengono visualizzate la società e il gruppo home del proprietario principale dell'attività. Si tratta di valori che non sono disponibili nell’interfaccia standard, ma che sono accessibili tramite la modalità testo.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 818c1f3a-4e82-4dc3-af86-4f9dcf5c11a4
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---

# Visualizza: Società e gruppo home dell&#39;utente assegnato

In questa visualizzazione attività vengono visualizzate la società e il gruppo home del proprietario principale dell&#39;attività. Si tratta di valori che non sono disponibili nell’interfaccia standard, ma che sono accessibili tramite la modalità testo.

![](assets/view--assigned-user-s-company-and-home-group-350x80.png)

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

## Visualizza la società e il gruppo home dell&#39;utente assegnato

1. Passare a un elenco di attività.
1. Da **Visualizza** menu a discesa, seleziona **Nuova vista**.

1. In **Anteprima a colonne** eliminare tutte le colonne tranne una.
1. Fai clic sull’intestazione della colonna rimanente, quindi fai clic su **Passa alla modalità testo**.
1. Passa il puntatore del mouse sull’area della modalità testo e fai clic su **Fare clic per modificare il testo**.
1. Rimuovi il testo che trovi nella **Modalità testo** e sostituirlo con il seguente codice:
   <pre>column.0.descriptionkey=name<br> column.0.link.linkproperty.0.name=ID<br> column.0.link.linkproperty.0.valuefield=ID<br> column.0.link.linkproperty.0.valueformat=int<br> column.0.link.lookup=link.view<br> column.0.link.value.field=objCode<br> column.0.link.valueformat=val<br> column.0.linkedname=direct<br> column.0.listsort=string(name)<br> column.0.namekey=name.abbr<br> column.0.querysort=name<br> column.0.short=false<br> column.0.stretch=100<br> column.0.valuefield=name<br> column.0.valueformat=HTML<br> column.0.width=150<br> column.1.descriptionkey=assignedto<br> column.1.link.linkproperty.0.name=ID<br> column.1.link.linkproperty.0.valuefield=assignedTo:ID<br> column.1.link.linkproperty.0.valueformat=int<br> column.1.link.lookup=link.view<br> column.1.link.value.field=assignedTo:objCode<br> column.1.link.valueformat=val<br> column.1.linkedname=assignedTo<br> column.1.listsort=nidificato(assignedTo).string(name)<br> column.1.namekey=assignedto<br> column.1.querysort=assignedTo:name<br> column.1.short=false<br> column.1.stretch=0<br> column.1.valuefield=assignedTo:name<br> column.1.valueformat=HTML<br> column.1.width=150<br> column.2.description=Assegnato alla società<br> column.2.displayname=Assegnato alla società<br> column.2.linkedname=assignedTo:company<br> column.2.listsort=nidificato(assignedTo:company).string(name)<br> column.2.namekey=assignedto<br> column.2.querysort=assignedTo:company:name<br> column.2.short=false<br> column.2.stretch=0<br> column.2.valuefield=assignedTo:company:name<br> column.2.valueformat=HTML<br> column.2.width=150<br> column.3.description=Assegnato al gruppo principale<br> column.3.displayname=Assegnato al gruppo home<br> column.3.linkedname=assignedTo:homeGroup<br> column.3.listsort=nidificato(assignedTo:homeGroup).string(name)<br> column.3.namekey=assignedto<br> column.3.querysort=assignedTo:homeGroup:name<br> column.3.short=false<br> column.3.stretch=0<br> column.3.valuefield=assignedTo:homeGroup:name<br> column.3.valueformat=HTML<br> column.3.width=150</pre>

1. Fai clic su **Salva modifiche**.
