---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Filtro: visualizza solo gli elementi in uno stato di approvazione"'
description: È possibile visualizzare solo gli elementi con un determinato stato attualmente in sospeso approvazione. Questo funziona allo stesso modo per qualsiasi altro oggetto con uno stato di approvazione.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c1de5193-d3d5-406c-aa68-e6ba6d6751ae
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 1%

---

# Filtro: visualizzare solo gli elementi in uno stato di approvazione

È possibile visualizzare solo gli elementi con un determinato stato attualmente in sospeso approvazione. Questo funziona allo stesso modo per qualsiasi altro oggetto con uno stato di approvazione.

È possibile inserire i seguenti oggetti in uno stato di approvazione:

* Attività
* Problemi
* Progetti

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

## Visualizza solo gli elementi nello stato di approvazione

1. Passa al filtro che desideri personalizzare per un elenco, ad esempio, di progetti.
1. Fai clic su **Aggiungere una regola filtro** per **Stato** campo dell&#39;oggetto dell&#39;elenco.\
   Ad esempio, in un rapporto di progetto, aggiungi **Pianificazione uguale stato**, se desideri visualizzare solo i progetti che si trovano nello stato **Pianificazione - Approvazione in sospeso**.

1. Fai clic su **Passa alla modalità testo**.
1. Modifica la

   ```
   status
   ```

   riga tramite aggiunta **:A** alla chiave a 3 lettere dello stato:
   <pre>status=PLN:A<br>status_Mod=in</pre>

1. Fai clic su **Fine**, quindi **Salva filtro**.

   Nell&#39;elenco vengono visualizzati solo i progetti che si trovano in uno stato Planning - In attesa di approvazione.
