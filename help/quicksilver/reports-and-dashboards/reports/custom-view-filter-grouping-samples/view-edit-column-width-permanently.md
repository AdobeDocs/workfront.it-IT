---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: "Visualizza: modifica definitivamente la larghezza di una colonna"
description: È possibile modificare temporaneamente la larghezza delle colonne trascinandone i margini in modo che corrispondano alla larghezza desiderata. Per ulteriori informazioni, consulta Modificare la larghezza e l’ordine delle colonne.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 42633036-8e42-4cec-876c-f20a5ece2478
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---

# Visualizza: modifica definitivamente la larghezza di una colonna

È possibile modificare temporaneamente la larghezza delle colonne trascinandone i margini in modo che corrispondano alla larghezza desiderata. Per ulteriori informazioni, consulta [Modifica la larghezza e l&#39;ordine delle colonne](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

È possibile modificare in modo permanente la larghezza di qualsiasi colonna di qualsiasi vista utilizzando la modalità testo nella colonna durante la modifica della vista.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Richiesta di modifica di una vista </p>
   <p>Pianificare la modifica di un rapporto</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari per modificare un rapporto</p> <p>Modificare l'accesso a Filtri, Viste, Raggruppamenti per modificare una vista</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

## Modificare definitivamente la larghezza di una colonna

>[!IMPORTANT]
>
>Se modifichi manualmente la larghezza di una colonna come descritto nella sezione &quot;Modificare temporaneamente la larghezza e l’ordine delle colonne&quot; nell’articolo [Modifica la larghezza e l&#39;ordine delle colonne](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md) dopo aver modificato in modo permanente la larghezza della colonna, questa viene mantenuta in base al ridimensionamento manuale e la larghezza della colonna viene aggiornata in base ai passaggi seguenti. Dopo aver cancellato la cache o effettuato l’accesso da un altro browser, puoi visualizzare la colonna in base alla larghezza definita nei passaggi seguenti.

1. Consente di passare a un elenco di oggetti.
1. Dalla sezione **Visualizza** menu a discesa, fai clic su **Nuova visualizzazione**.

1. Clic **Aggiungi colonna** per aggiungere una nuova colonna.

   Oppure

   Fai clic sull’intestazione di colonna di una colonna esistente.

1. Clic **Passa alla modalità testo**.
1. Passa il puntatore del mouse sull’area della modalità testo e fai clic su **Fare clic per modificare il testo**.
1. Aggiungi il seguente codice alla modalità testo della colonna:

   ```
   width=200
   usewidths=true
   ```

   Per **larghezza** riga, specificare un numero (in pixel) che rappresenti la larghezza della colonna da visualizzare nella visualizzazione.

1. Clic **Salva**, quindi **Salva visualizzazione**.
