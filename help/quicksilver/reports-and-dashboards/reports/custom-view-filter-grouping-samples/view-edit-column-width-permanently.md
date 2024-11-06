---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: "Visualizza: modifica permanente della larghezza di una colonna"
description: È possibile modificare temporaneamente la larghezza delle colonne trascinandone i margini in modo che corrispondano alla larghezza desiderata. Per ulteriori informazioni, consulta Modificare la larghezza e l’ordine delle colonne.
author: Nolan
feature: Reports and Dashboards
exl-id: 42633036-8e42-4cec-876c-f20a5ece2478
source-git-commit: 71c0bf664af66bec7122651c1b62dd1c28022565
workflow-type: tm+mt
source-wordcount: '403'
ht-degree: 0%

---

# Visualizza: modifica definitivamente la larghezza di una colonna

<!-- Audited: 11/2024 -->

È possibile modificare temporaneamente la larghezza delle colonne trascinandone i margini in modo che corrispondano alla larghezza desiderata. Per ulteriori informazioni, vedere [Modificare la larghezza e l&#39;ordine delle colonne](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

Per modificare in modo permanente la larghezza di una colonna di qualsiasi vista, è necessario utilizzare la modalità testo nella colonna durante la modifica della vista.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> <p>Nuovo:<ul><li>Collaboratore per modificare una visualizzazione</li><li>Standard per modificare un rapporto</li></ul></p><p>Oppure</p>Corrente:<ul><li>Richiesta di modifica di una vista</li><li>Pianificare la modifica di un rapporto</li></ul></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari per modificare un rapporto</p> <p>Modificare l'accesso a Filtri, Viste, Raggruppamenti per modificare una vista</p> </td> 
  </tr>  
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Modificare definitivamente la larghezza di una colonna

>[!IMPORTANT]
>
>Se modifichi manualmente la larghezza di una colonna come descritto nella sezione [Modifica temporaneamente la larghezza e l&#39;ordine delle colonne](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md#modify-width-and-order-of-columns-temporarily) nell&#39;articolo [Modifica la larghezza e l&#39;ordine delle colonne](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md) dopo aver modificato definitivamente la larghezza della colonna, la larghezza della colonna viene mantenuta in base al ridimensionamento manuale. In questo caso, la larghezza della colonna aggiornata in base ai passaggi seguenti viene sovrascritta. Dopo aver cancellato la cache o effettuato l’accesso da un altro browser, puoi visualizzare la colonna in base alla larghezza definita nei passaggi seguenti.
>
>Per ulteriori informazioni sulla personalizzazione della larghezza delle colonne durante l&#39;utilizzo dell&#39;interfaccia in modalità testo, vedere le definizioni &quot;width&quot; e &quot;stretch&quot; nel [Glossario della terminologia di Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

1. Consente di passare a un elenco di oggetti.
1. Dal menu a discesa **Visualizza**, fare clic su **Nuova visualizzazione**.

1. Fare clic su **Aggiungi colonna** per aggiungere una nuova colonna.

   Oppure

   Fai clic sull’intestazione di colonna di una colonna esistente.

1. Fare clic su **Passa alla modalità testo**.
1. Fare clic su **Modifica modalità testo**.T
1. Aggiungi il seguente codice alla modalità testo della colonna:

   ```
   width=200
   usewidths=true
   ```

   Per la riga **width**, specifica un numero (in pixel) che rappresenti la larghezza desiderata per la colonna nella visualizzazione.

1. Fai clic su **Fine**, quindi su **Salva visualizzazione**.


