---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Filtro: eliminare gli elementi in un elenco confrontando due campi'
description: È possibile filtrare gli elementi da un elenco confrontando due dei relativi campi. Ad esempio, è possibile visualizzare solo i task in cui la data di completamento effettivo dell'attività è maggiore della data di completamento pianificata.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 6a41db8e-1456-4031-bf2a-ca6d4111ad44
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---

# Filtro: eliminare gli elementi in un elenco confrontando due campi

È possibile filtrare gli elementi da un elenco confrontando due dei relativi campi. Ad esempio, è possibile visualizzare solo i task in cui la data di completamento effettivo dell&#39;attività è maggiore della data di completamento pianificata.

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

## Filtrare gli articoli confrontando due campi

1. Passare a un elenco di attività.
1. Da **Filtro** menu a discesa, seleziona **Nuovo filtro**.

1. Fai clic su **Aggiungi regola filtro** e aggiungere **Data completamento effettivo** >**Maggiore di** > **Selezionare una data**.

   >[!TIP]
   >
   >Scegliere il modificatore di filtro da utilizzare per il campo selezionato, se disponibile.

1. Fai clic su **Passa alla modalità testo**.
1. In **Impostare regole di filtro per il rapporto** aggiungi il seguente codice:

   ```
   actualCompletionDate=FIELD:plannedCompletionDate<br>actualCompletionDate_Mod=gt
   ```

1. Fai clic su **Fine**, quindi **Salva filtro**.
