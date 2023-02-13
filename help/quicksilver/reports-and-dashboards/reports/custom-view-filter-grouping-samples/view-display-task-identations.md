---
content-type: reference
product-area: reporting;projects;portfolios;programs
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Visualizza: visualizzare i rientri delle attività in un elenco di attività'
description: In questa visualizzazione attività, è possibile aggiungere codice alla colonna Nome attività per visualizzare le attività rientrate in base alla struttura di suddivisione del lavoro del progetto.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: f7f43e1e-db32-48b8-9a23-ff9fa6195386
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---

# Visualizza: visualizzare i rientri delle attività in un elenco di attività

In questa visualizzazione attività, è possibile aggiungere codice alla colonna Nome attività per visualizzare le attività rientrate in base alla struttura di suddivisione del lavoro del progetto.

![](assets/view-text-mode-indentation-task-list-350x171.png)

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

## Visualizza i rientri delle attività in una colonna di un elenco di attività

1. Passare a un elenco di attività.
1. Da **Visualizza** menu a discesa, fai clic su **Nuova vista**.

1. Fai clic su **Aggiungi colonna** e inizia a digitare &quot;Nome attività&quot; nella sezione **Mostra in questa colonna** quindi selezionalo quando viene visualizzato nell’elenco.

1. Dalla nuova colonna, fai clic su **Passa alla modalità testo**.
1. Passa il puntatore del mouse sull’area della modalità testo e fai clic su **Fare clic per modificare il testo**.
1. Rimuovi il testo che trovi nella

   ```
   valuefield=
   ```

   e sostituiscilo con il seguente codice:

   ```
   valueexpression=IF({indent}<1,{name},IF({indent}<2,CONCAT(' - ',{name}),IF({indent}<3,CONCAT(' - - ',{name}),IF({indent}<4,CONCAT(' - - - ',{name}),CONCAT(' - - - - ',{name})))))
   ```

1. Fai clic su **Salva**, quindi **Salva visualizzazione**.
