---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Visualizzare le ore totali sul timesheet
description: Puoi visualizzare il numero totale di ore sulla scheda orario. Il numero totale di ore della scheda orario include le ore registrate per progetti, attività, problemi e tutte le ore generali.
author: Lisa
feature: Timesheets
exl-id: ff0823f2-61d0-453f-ae1c-68f0f1465d73
TQID: https://experienceleague.adobe.com/oh6bBQz6sfxCpodHahZXtlMMuYYT-4U7-5MP6TQeuIs
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
  - id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: dbb2e1aee18e6435a79ee2071f0bd5ba84ce2af3
workflow-type: tm+mt
source-wordcount: 476
ht-degree: 10%

---

# Visualizzare le ore totali sul timesheet

<!--Audited: 8/2024-->

Puoi visualizzare il numero totale di ore sulla scheda orario. Il numero totale di ore della scheda orario include le ore registrate per progetti, attività, problemi e tutte le ore generali.

Le ore totali riflettono le ore inviate tramite la scheda orario, l’area Aggiornamenti o l’area Ore per progetti, attività o problemi.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td>Licenza di Adobe Workfront</td> 
   <td> <p>Chiaro o superiore </p>
   <p>Revisione o successiva</p> </td> 
  </tr> 
  <tr> 
   <td>Configurazione del livello di accesso</td> 
   <td> <p>Visualizzare o accedere ad altre attività e problemi</p> </td> 
  </tr> 
  <tr> 
   <td>Autorizzazioni sugli oggetti</td> 
   <td> <p>Visualizza o autorizzazioni superiori per attività e problemi</p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visualizzare le ore totali di una scheda orario nell&#39;intestazione della scheda orario

Puoi visualizzare le ore totali di una scheda orario nell’intestazione della scheda.

![Campo Ore totali](assets/timesheet-total-hours-in-header-highlighted-redesigned.png)

## Visualizza le ore totali sulla scheda orario in un elenco di schede orario

{{step1-to-timesheets}}

Verrà aperta l&#39;area **Schede orario**.

![Elenco schede orario con una scheda orario selezionata](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Facoltativo) Per aggiornare il filtro nell’elenco delle schede orario, effettua una delle seguenti operazioni:

   * Seleziona **Le mie approvazioni schede orario** nell&#39;angolo superiore destro della pagina per visualizzare solo le schede orario che hai approvato

     Oppure

     Seleziona **Le mie schede orario** per visualizzare solo le tue schede orario.

     In questo modo all’elenco delle schede orario vengono applicate le approvazioni delle mie schede orario o i filtri delle mie schede orario.

     ![Pulsanti filtro schede orario personali nella pagina dell&#39;elenco delle schede orario](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * Fai clic sull&#39;icona Filtro ![icona Filtro](assets/filter-nwepng.png) per applicare un filtro diverso o creane uno nuovo. Per informazioni sulla creazione o l&#39;aggiornamento dei filtri, vedere [Creare o modificare filtri in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

   >[!NOTE]
   >
   >Le opzioni Approvazioni schede attività personali e Schede attività personali non vengono visualizzate nella parte superiore dell&#39;elenco delle schede attività o nell&#39;elenco dei filtri se l&#39;amministratore di Workfront o un amministratore di gruppo ha rimosso tali filtri dai controlli elenco nell&#39;area Configura o dal modello di layout. Per ulteriori informazioni, vedere [Personalizzare filtri, visualizzazioni e raggruppamenti utilizzando un modello di layout](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. (Facoltativo) Fai clic sull&#39;icona **Visualizza** ![Visualizza](assets/view-icon.png) o **Raggruppamento** ![Icona Raggruppamento](assets/grouping.png) per applicare una visualizzazione o un raggruppamento diverso o crearne uno nuovo.

   Per informazioni sulla creazione di filtri, viste o raggruppamenti, vedere i seguenti articoli:

   * [Creare o modificare filtri in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Creare o modificare le visualizzazioni in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Creare raggruppamenti in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Il numero totale di ore per ogni scheda orario viene visualizzato nella colonna **Ore totali**.

   ![Colonna ore totali](assets/total-hours-column-highlighted-all-timesheets-list-nwe-350x120.png)

   >[!TIP]
   >
   >Quando si utilizza la visualizzazione Standard per un elenco di schede orario, la colonna Ore totali viene visualizzata in rosso se il tempo registrato per gli elementi della scheda orario supera il numero di ore nell&#39;intervallo di tempo della scheda orario. Per ulteriori informazioni, vedere il campo &quot;Ore totali&quot; in [Glossario della terminologia di Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).
