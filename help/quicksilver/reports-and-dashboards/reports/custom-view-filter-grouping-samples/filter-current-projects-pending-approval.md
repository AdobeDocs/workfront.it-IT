---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Filtro: visualizza i progetti correnti in attesa di approvazione"'
description: Il seguente filtro di progetto visualizza i progetti nello stato Attuale - In attesa di approvazione, in cui l’utente connesso è lo sponsor del progetto o il gestore del Portfolio.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 32045aec-acc5-44d2-bad5-7759dc797414
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 0%

---

# Filtro: visualizzare i progetti correnti in attesa di approvazione

Il seguente filtro di progetto visualizza i progetti nello stato Attuale - In attesa di approvazione, in cui l’utente connesso è lo sponsor del progetto o il gestore del Portfolio.

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

## Filtrare i progetti correnti in attesa di approvazione

Per applicare questo filtro:

1. Vai a un elenco di progetti.
1. Da **Filtro** menu a discesa, seleziona **Nuovo filtro**.

1. Fai clic su **Passa alla modalità testo**.
1. In **Impostare regole di filtro per il rapporto** area, copia e incolla il seguente codice:
   <pre>status=CUR:A<br>sponsorID=$$USER.ID<br>O:a:status=CUR:A<br>O:a:portfolio:ownerID=$$USER.ID</pre>

1. Fai clic su **Salva filtro**.
