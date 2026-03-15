---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Vista: modifica permanentemente la larghezza di una colonna'
description: Potete modificare temporaneamente la larghezza delle colonne trascinandone i margini in modo che corrispondano alla larghezza desiderata. Per ulteriori informazioni, consultate Modificare la larghezza e l’ordine delle colonne.
author: Courtney
feature: Reports and Dashboards
exl-id: 42633036-8e42-4cec-876c-f20a5ece2478
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 12%

---

# Visualizzazione: modificare definitivamente la larghezza di una colonna

<!-- Audited: 11/2024 -->

Potete modificare temporaneamente la larghezza delle colonne trascinandone i margini in modo che corrispondano alla larghezza desiderata. Per ulteriori informazioni, vedere [Modificare la larghezza e l&#39;ordine delle colonne](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

Per modificare definitivamente la larghezza di una colonna di una visualizzazione, è necessario utilizzare la modalità testo nella colonna durante la modifica della visualizzazione.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td> 
   <p>Collaboratore o richiesta di modifica di una visualizzazione </p>
   <p>Standard o piano per modificare un report</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso a report, dashboard, calendari</p> <p>Modificare l'accesso a Filtri, Viste, Raggruppamenti per modificare una vista</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
   <td> <p>Gestire le autorizzazioni per un report</p>  </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Modificare definitivamente la larghezza di una colonna

>[!IMPORTANT]
>
>Se si modifica manualmente la larghezza di una colonna come descritto nella sezione [Modificare temporaneamente la larghezza e l&#39;ordine delle colonne](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md#modify-width-and-order-of-columns-temporarily) nell&#39;articolo [Modificare la larghezza e l&#39;ordine delle colonne](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md) dopo aver modificato in modo permanente la larghezza della colonna, la larghezza della colonna viene mantenuta in base al ridimensionamento manuale. In questo caso, la larghezza della colonna aggiornata in base ai passaggi seguenti viene sovrascritta. È possibile visualizzare la colonna in base alla larghezza definita nei passaggi seguenti dopo aver cancellato la cache o effettuato l&#39;accesso da un altro browser.
>
>Per ulteriori informazioni sulla personalizzazione della larghezza delle colonne quando si utilizza l&#39;interfaccia Modalità testo, vedere le definizioni &quot;width&quot; e &quot;stretch&quot; nel [Glossario della terminologia di Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

1. Consente di passare a un elenco di oggetti.
1. Dal menu a discesa **Visualizza**, fai clic su **Nuova vista**.

1. Fai clic su **Aggiungi colonna** per aggiungere una nuova colonna.

   Oppure

   Fare clic sull&#39;intestazione di colonna di una colonna esistente.

1. Fai clic su **Passa alla modalità testo**.
1. Fai Clic Su **Modifica Modalità Testo**.T
1. Aggiungete il codice seguente alla modalità testo della colonna:

   ```
   width=200
   usewidths=true
   ```

   Per la riga **larghezza**, specificare un numero (in pixel) che rappresenti la larghezza della colonna nella visualizzazione.

1. Fai clic su **Fine**, quindi su **Salva vista**.


