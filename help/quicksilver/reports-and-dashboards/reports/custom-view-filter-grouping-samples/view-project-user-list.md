---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Visualizza: elenco degli utenti del progetto con ruoli di lavoro'
description: È possibile applicare questa visualizzazione in un elenco o in un rapporto di progetto per visualizzare un elenco degli utenti associati al progetto, nonché un elenco dei ruoli del lavoro che stanno eseguendo sul progetto.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: a3f59f69-7f39-4814-bd2f-7734d620081e
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '460'
ht-degree: 0%

---

# Visualizza: elenco degli utenti del progetto con ruoli di lavoro

È possibile applicare questa visualizzazione in un elenco o in un rapporto di progetto per visualizzare un elenco degli utenti associati al progetto, nonché un elenco dei ruoli del lavoro che stanno eseguendo sul progetto.

Le informazioni contenute in questo rapporto si trovano anche nell’area Persone del progetto.

>[!TIP]
>
>Se per gli utenti non sono elencati ruoli di lavoro ma si è certi che sono associati a ruoli di lavoro nei loro profili utente, ciò potrebbe significare che sono assegnati a attività e problemi, ma potrebbero non essere associati a un ruolo di lavoro nell&#39;attività o nel problema, oppure che gli utenti elencati nel rapporto non sono gli assegnatari in attività e problemi, ma soddisfano altri ruoli del progetto (ad esempio, Proprietario o Sponsor.)

![project_with_user_and_role_information_report.png](assets/project-with-user-and-role-information-report-350x100.png)

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

## Visualizza un elenco di utenti del progetto con ruoli di lavoro

1. Vai a un elenco di progetti.
1. Da **Visualizza** menu a discesa, seleziona **Nuova vista**.

1. In **Anteprima a colonne** eliminare tutte le colonne tranne una.
1. Fai clic sull’intestazione della colonna rimanente, quindi fai clic su **Passa alla modalità testo**.
1. Passa il puntatore del mouse sull’area della modalità testo e fai clic su **Fare clic per modificare il testo**.
1. Rimuovi il testo che trovi nella **Modalità testo** e sostituirlo con il seguente codice:
   <pre>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.section=0<br>column.0.short=false<br>column.0.stretch=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=200<br>column.1.displayname=Utenti del progetto<br>column.1.listdelimiter=&lt;br&gt;<br>column.1.listmethod=nidificato(projectUsers).lists<br>column.1.textmode=true<br>column.1.type=iterate<br>column.1.value eexpression={user}.{name}<br>column.1.valueformat=HTML<br>column.2.displayname=Ruoli progetto<br>column.2.listdelimiter=&lt;br&gt;<br>column.2.listmethod=nidificato(projectUserRuoli).lists<br>column.2.textmode=true<br>column.2.type=iterate<br>column.2.value eexpression={role}.{name}<br>column.2.valueformat=HTML</pre>

1. Fai clic su **Salva visualizzazione**.
