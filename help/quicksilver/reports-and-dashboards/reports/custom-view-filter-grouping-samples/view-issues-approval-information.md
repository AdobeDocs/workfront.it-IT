---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Visualizza: problemi relativi alle informazioni di approvazione"'
description: La seguente visualizzazione del problema mostra il processo di approvazione, il passaggio, i nomi degli approvatori e lo stato del problema prima che l'approvazione sia stata rilasciata. Alcuni di questi campi non sono accessibili tramite il generatore di interfacce standard.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 4e123844-a0d6-474b-87fb-d30ed391ad07
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '517'
ht-degree: 0%

---

# Visualizza: problemi relativi alle informazioni di approvazione

La seguente visualizzazione del problema mostra il processo di approvazione, il passaggio, i nomi degli approvatori e lo stato del problema prima che l&#39;approvazione sia stata rilasciata. Alcuni di questi campi non sono accessibili tramite il generatore di interfacce standard.

![custom_issue_view_with_authorization_info.png](assets/custom-issue-view-with-approval-info-350x46.png)

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

## Visualizza i problemi relativi alle informazioni di approvazione

1. Vai a un elenco di problemi.
1. Da **Visualizza** menu a discesa, seleziona **Nuova vista**.

1. In **Anteprima a colonne** eliminare tutte le colonne tranne una.
1. Fai clic sull’intestazione della colonna rimanente, quindi fai clic su **Passa alla modalità testo**.
1. Passa il puntatore del mouse sull’area della modalità testo e fai clic su **Fare clic per modificare il testo**.
1. Rimuovi il testo che trovi nella **Modalità testo** e sostituirlo con il seguente codice:
   <pre style="font-style: normal;">column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.value.field=objCode<br>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.short=false<br>column.0.stretch=40<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=220<br>column.1.descriptionkey=assignedto<br>column.1.linkedname=assignedTo<br>column.1.listsort=nidificato(assignedTo).string(name)<br>column.1.namekey=assignedto<br>column.1.querysort=assignedTo:name<br>column.1.short=true<br>column.1.stretch=0<br>column.1.valuefield=assignedTo:name<br>column.1.valueformat=HTML<br>column.1.width=150<br>column.2.descriptionkey=role<br>column.2.linkedname=role<br>column.2.listsort=nidificato(role).string(name)<br>column.2.namekey=role<br>column.2.querysort=role:name<br>column.2.short=false<br>column.2.stretch=25<br>column.2.valuefield=role:name<br>column.2.valueformat=HTML<br>column.2.width=150<br>column.3.description=Nome del processo di approvazione<br>column.3.linkedname=direct<br>column.3.listsort=string(name)<br>column.3.name=Nome del processo di approvazione<br>column.3.querysort=name<br>column.3.short=false<br>column.3.stretch=35<br>column.3.valuefield=authorizationProcess:name<br>column.3.valueformat=HTML<br>column.3.width=220<br>column.4.description=Nome passaggio approvazione<br>column.4.linkedname=direct<br>column.4.listsort=string(name)<br>column.4.name=Nome del passaggio di approvazione<br>column.4.querysort=name<br>column.4.short=false<br>column.4.stretch=0<br>column.4.valuefield=currentApprovedStep:name<br>column.4.valueformat=HTML<br>column.4.width=220<br>column.5.description=Stato precedente<br>column.5.linkedname=direct<br>column.5.listsort=string(name)<br>column.5.name=Stato precedente<br>column.5.querysort=name<br>column.5.short=false<br>column.5.stretch=0<br>column.5.valueField=previousStatus<br>column.5.valueformat=HTML<br>column.5.width=220<br>column.6.linkedname=direct<br>column.6.listsort=HTML(approversString)<br>column.6.namekey=approver.plural.abbr<br>column.6.querysort=approversString<br>column.6.short=false<br>column.6.stretch=0<br>column.6.valuefield=approversString<br>column.6.valueformat=HTML<br>column.6.viewalias=approver.plural<br>column.6.width=200<br></pre>

1. Fai clic su **Salva visualizzazione**.
