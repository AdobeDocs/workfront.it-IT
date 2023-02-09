---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Visualizza: modificare in modo permanente la larghezza di una colonna"'
description: È possibile modificare temporaneamente la larghezza delle colonne trascinandone i margini per adattarli alla larghezza desiderata. Per ulteriori informazioni, consulta Modificare la larghezza e l’ordine delle colonne.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 42633036-8e42-4cec-876c-f20a5ece2478
source-git-commit: bb348deb9841320a367695845efe0ca36a9a9d8b
workflow-type: tm+mt
source-wordcount: '389'
ht-degree: 0%

---

# Visualizza: modificare in modo permanente la larghezza di una colonna

È possibile modificare temporaneamente la larghezza delle colonne trascinandone i margini per adattarli alla larghezza desiderata. Per ulteriori informazioni, consulta [Modificare la larghezza e l’ordine delle colonne](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

È possibile modificare in modo permanente la larghezza di qualsiasi colonna di una visualizzazione utilizzando la modalità testo nella colonna durante la modifica della visualizzazione.

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

## Modificare definitivamente la larghezza di una colonna

>[!IMPORTANT]
>
>Se modifichi manualmente la larghezza di una colonna come descritto nella sezione &quot;Modificare temporaneamente la larghezza e l’ordine delle colonne&quot; nell’articolo [Modificare la larghezza e l’ordine delle colonne](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md) dopo aver modificato in modo permanente la larghezza della colonna, questa viene mantenuta in base al ridimensionamento manuale e viene sovrascritta la larghezza della colonna in base ai passaggi seguenti. Puoi visualizzare la colonna in base alla larghezza definita nei passaggi seguenti dopo aver cancellato la cache o effettuato l’accesso da un altro browser.

1. Passare a un elenco di oggetti.
1. Da **Visualizza** menu a discesa, fai clic su **Nuova vista**.

1. Fai clic su **Aggiungi colonna** per aggiungere una nuova colonna.

   Oppure

   Fai clic sull’intestazione di colonna di una colonna esistente.

1. Fai clic su **Passa alla modalità testo**.
1. Passa il puntatore del mouse sull’area della modalità testo e fai clic su **Fare clic per modificare il testo**.
1. Aggiungi il codice seguente alla modalità testo della colonna:

   ```
   width=200
   usewidths=true
   ```

   Per **larghezza** linea, specifica un numero (in pixel) che rappresenti la larghezza che la colonna deve visualizzare nella visualizzazione.

1. Fai clic su **Salva**, quindi **Salva visualizzazione**.
