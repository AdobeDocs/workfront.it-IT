---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: "Visualizza: modifica definitivamente la larghezza di una colonna"
description: È possibile modificare temporaneamente la larghezza delle colonne trascinandone i margini in modo che corrispondano alla larghezza desiderata. Per ulteriori informazioni, consulta Modificare la larghezza e l’ordine delle colonne.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 42633036-8e42-4cec-876c-f20a5ece2478
source-git-commit: 261c1b73d785094de4ee8549c856a091920ba04a
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 0%

---

# Visualizza: modifica definitivamente la larghezza di una colonna

<!-- Audited: 1/2024 -->

È possibile modificare temporaneamente la larghezza delle colonne trascinandone i margini in modo che corrispondano alla larghezza desiderata. Per ulteriori informazioni, consulta [Modifica la larghezza e l&#39;ordine delle colonne](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

Per modificare in modo permanente la larghezza di una colonna di qualsiasi vista, è necessario utilizzare la modalità testo nella colonna durante la modifica della vista.

## Requisiti di accesso

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

## Modificare definitivamente la larghezza di una colonna

>[!IMPORTANT]
>
>Se modifichi manualmente la larghezza di una colonna come descritto nella sezione [Modifica temporaneamente la larghezza e l&#39;ordine delle colonne](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md#modify-width-and-order-of-columns-temporarily) nell’articolo [Modifica la larghezza e l&#39;ordine delle colonne](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md) dopo aver modificato in modo permanente la larghezza della colonna, questa viene mantenuta in base al ridimensionamento manuale. In questo caso, la larghezza della colonna aggiornata in base ai passaggi seguenti viene sovrascritta. Dopo aver cancellato la cache o effettuato l’accesso da un altro browser, puoi visualizzare la colonna in base alla larghezza definita nei passaggi seguenti.
>
>Per ulteriori informazioni sulla personalizzazione della larghezza delle colonne quando si utilizza l’interfaccia Text Mode, consulta le definizioni &quot;width&quot; e &quot;stretch&quot; nella sezione [Glossario della terminologia di Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

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


