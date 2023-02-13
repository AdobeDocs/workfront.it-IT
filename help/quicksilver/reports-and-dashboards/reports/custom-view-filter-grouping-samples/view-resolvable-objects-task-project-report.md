---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Visualizza: Oggetti risolvibili in un''attività o in un report di progetto"'
description: È possibile visualizzare un elenco di tutti gli oggetti risolvibili in una visualizzazione o in un report di progetto o task.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2b0d8e7c-9211-44e5-9d92-c87a2fe4336d
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 0%

---

# Visualizza: Oggetti risolvibili in un&#39;attività o in un rapporto di progetto

È possibile visualizzare un elenco di tutti gli oggetti risolvibili in una visualizzazione o in un report di progetto o task.

Per ulteriori informazioni sugli oggetti risolvibili, vedere l&#39;articolo [Panoramica sulla risoluzione e risoluzione di oggetti](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

![list_of_resolvables_in_report.png](assets/list-of-resolvables-in-report-350x54.png)

L&#39;applicazione di questa visualizzazione è identica per le attività e i progetti.

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

## Visualizzazione di oggetti risolvibili in un&#39;attività o in un rapporto di progetto

1. Passa a un elenco di attività che sono state convertite da problemi.
1. Da **Visualizza** menu a discesa, seleziona **Nuova vista**.

1. In **Anteprima a colonne** area, fai clic su **Aggiungi colonna**.

1. Fai clic sull’intestazione della nuova colonna, quindi fai clic su **Passa alla modalità testo**.
1. Passa il puntatore del mouse sull’area della modalità testo e fai clic su **Fare clic per modificare il testo**.
1. Rimuovi il testo che trovi nella **Modalità testo** e sostituirlo con il seguente codice:

   <pre>displayname=Resolvables<br>listdelimiter=<br><br>listmethod=nidificato(resolvables).lists<br>textmode=true<br>type=iterate<br>valuefield=name<br>valueformat=HTML<br></pre>

1. Fai clic su **Salva visualizzazione**.\
   Nella nuova colonna viene visualizzato un elenco di tutti gli oggetti risolvibili. I nomi degli oggetti dell’elenco non possono essere collegati direttamente agli oggetti.
