---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Visualizza: mostra il nome delle attività principali come tutte le maiuscole'
description: È possibile aggiungere questa colonna a una visualizzazione attività per visualizzare il nome delle attività principali in lettere maiuscole.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: bb489920-6b17-4689-b432-b0c28bcb5d10
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 0%

---

# Visualizza: mostra il nome delle attività principali come tutte le maiuscole

È possibile aggiungere questa colonna a una visualizzazione attività per visualizzare il nome delle attività principali in lettere maiuscole.

![](assets/column-task-with-all-caps-parent-350x112.png)

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

## Mostra il nome delle attività principali come tutte maiuscole

Per creare questa colonna in una visualizzazione attività:

1. Passare a un elenco di attività.
1. Da **Visualizza** menu a discesa, seleziona **Personalizza visualizzazione**.\
   Oppure\
   Da **Visualizza** menu a discesa, seleziona **Nuova vista**.

1. In **Anteprima a colonne** fare clic sull&#39;intestazione della colonna che mostra il nome dell&#39;attività nell&#39;elenco.
1. Fai clic su **Passa alla modalità testo**.
1. Passa il puntatore del mouse sull’area della modalità testo e fai clic su **Fare clic per modificare il testo**.
1. Rimuovi il testo che trovi nella **Modalità testo** e sostituirlo con il seguente codice: <pre>descriptionkey=name<br>displayname=Nome attività<br>textmode=true<br>valueexpression=IF({numberOfChildren}>&quot;0&quot;,UPPER({name}),{name})<br>valueformat=HTML<br>width=150<br></pre>

1. Fai clic su **Salva visualizzazione**.
