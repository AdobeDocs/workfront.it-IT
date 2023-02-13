---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Raggruppamento: Sponsor del progetto per ore'
description: Questo raggruppamento di ore organizza ore per lo sponsor del progetto in cui vengono registrate le ore. L’interfaccia standard di Report Builder per i raggruppamenti di ore non fornisce una mappatura al campo Project Sponsor . Per accedere a questo campo è necessario utilizzare l’interfaccia Modalità testo .
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 6b35b0ef-18b7-4121-ae39-d7957d76c04b
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---

# Raggruppamento: Sponsor del progetto per ore

Questo raggruppamento di ore organizza ore per lo sponsor del progetto in cui vengono registrate le ore. L’interfaccia standard di Report Builder per i raggruppamenti di ore non fornisce una mappatura al campo Project Sponsor . Per accedere a questo campo è necessario utilizzare l’interfaccia Modalità testo .

![hour_report_raggruppato_da_sponsor.png](assets/hour-report-grouped-by-sponsor-350x39.png)

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

## Raggruppa per sponsor progetto per ore

Per applicare questo raggruppamento:

1. Vai a un elenco di ore.
1. Da **Raggruppamento** menu a discesa, seleziona **Nuovo raggruppamento**.

1. Fai clic su **Passa alla modalità testo**.
1. Rimuovi il testo nel **Raggruppa il rapporto** area.

1. Sostituisci il testo con il seguente codice:

   <pre>group.0.linkedname=project:sponsor:name<br>group.0.name=<br>group.0.valuefield=project:sponsor:name<br>group.0.valueformat=HTML<br>textmode=true<br></pre>

1. Fai clic su **Salva raggruppamento**.
