---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Visualizza: dettagli utente espansi'
description: Questa visualizzazione utente visualizza informazioni sugli utenti. Oltre al nome, ai livelli di accesso e alla Società, mostra anche gli elenchi dei gruppi, dei team e dei ruoli del lavoro.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 6a978b43-4718-43fb-80b8-844b35e09d06
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '526'
ht-degree: 0%

---

# Visualizza: dettagli utente espansi

Questa visualizzazione utente visualizza informazioni sugli utenti. Oltre al nome, ai livelli di accesso e alla Società, mostra anche gli elenchi dei gruppi, dei team e dei ruoli del lavoro.

![expand_user_view.png](assets/expanded-user-view-350x75.png)

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

## Visualizza dettagli utente espansi

Per applicare questa visualizzazione:

1. Vai a un elenco di utenti.
1. Da **Visualizza** menu a discesa, seleziona **Nuova vista**.

1. In **Anteprima a colonne** eliminare tutte le colonne tranne una.
1. Fai clic sull’intestazione della colonna rimanente, quindi fai clic su **Passa alla modalità testo**.
1. Passa il puntatore del mouse sull’area della modalità testo e fai clic su **Fare clic per modificare il testo**.
1. Rimuovi il testo che trovi nella **Modalità testo** e sostituirlo con il seguente codice:

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: extra tag here that adds extra spaces in Preview)
   </MadCap:conditionalText>
   -->

   <pre>column.0.descriptionkey=name <br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.value.field=objCode<br>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.short=false<br>column.0.stretch=0<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.descriptionkey=accesslevel<br>column.1.link.linkproperty.0.name=ID<br>column.1.link.linkproperty.0.valuefield=accessLevel:ID<br>column.1.link.linkproperty.0.valueformat=int<br>column.1.link.lookup=link.view<br>column.1.link.value.field=accessLevel:objCode<br>column.1.link.valueformat=val<br>column.1.linkedname=accessLevel<br>column.1.listsort=string(displayName)<br>column.1.namekey=accesslevel<br>column.1.querysort=name<br>column.1.short=false<br>column.1.stretch=0<br>column.1.valuefield=accessLevel:displayName<br>column.1.valueformat=HTML<br>column.1.viewalias=accessLevel:displayName<br>column.1.width=100<br>column.2.link.linkproperty.0.name=ID<br>column.2.link.linkproperty.0.valuefield=ID<br>column.2.link.linkproperty.0.valueformat=int<br>column.2.link.lookup=link.view<br>column.2.link.value=val(objCode)<br>column.2.listdelimiter=<br>column.2.listmethod=nidificato(userGroups).lists<br>column.2.namekey=group.plural<br>column.2.stretch=50<br>column.2.type=iterate<br>column.2.valuefield=group:name<br>column.2.valueformat=HTML<br>column.2.width=150<br>column.3.displayname=Teams<br>column.3.listdelimiter=<br>column.3.listmethod=nidificato(teams).lists<br>column.3.textmode=true<br>column.3.type=iterate<br>column.3.valueexpression={name}<br>column.3.valueformat=HTML<br>column.4.link.linkproperty.0.name=ID<br>column.4.link.linkproperty.0.valuefield=ID<br>column.4.link.linkproperty.0.valueformat=int<br>column.4.link.lookup=link.view<br>column.4.link.value=val(objCode)<br>column.4.listdelimiter=<br>column.4.listmethod=nidificato(userRuoli).lists<br>column.4.namekey=jobrole.plural<br>column.4.stretch=50<br>column.4.type=iterate<br>column.4.valuefield=role:name<br>column.4.valueformat=HTML<br>column.4.width=150<br>column.5.descriptionkey=company<br>column.5.link.linkproperty.0.name=ID<br>column.5.link.linkproperty.0.valuefield=company:ID<br>column.5.link.linkproperty.0.valueformat=int<br>column.5.link.lookup=link.view<br>column.5.link.value.field=company:objCode<br>column.5.link.valueformat=val<br>column.5.linkedname=company<br>column.5.listsort=nidificato(company).string(name)<br>column.5.namekey=company<br>column.5.querysort=company:name<br>column.5.short=false<br>column.5.stretch=0<br>column.5.valuefield=company:name<br>column.5.valueformat=HTML<br>column.5.width=150</pre>

1. Fai clic su **Salva visualizzazione**.
