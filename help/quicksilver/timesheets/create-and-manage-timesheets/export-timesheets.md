---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Esportare un elenco di schede orario
description: In qualità di responsabile persone o approvatore scheda orario, potrebbe essere necessario scaricare un elenco di schede orario per visualizzare rapidamente le informazioni sulle schede orario delle persone di cui sei responsabile. Per farlo, esporta un elenco di schede orario.
author: Lisa
feature: Timesheets
exl-id: cb5b1c6c-7800-48f4-ae2c-c4007a161a6c
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/-bihpKoVoPCwTpAj-SK-RPPFpaCubsyLAfnfSmpTnyI
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
    internal-label: Approvals
  - id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
    internal-label: Timesheets
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 64bb9e6dba8976ba413ec9b58e926da931bba1c5
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 14%
---
# Esportare un elenco di schede orario

<!--Audited: 8/2024-->

In qualità di responsabile persone o approvatore scheda orario, potrebbe essere necessario scaricare un elenco di schede orario per visualizzare rapidamente le informazioni sulle schede orario delle persone di cui sei responsabile. Per farlo, esporta un elenco di schede orario.

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

## Esportare un elenco di schede orario

{{step1-to-timesheets}}

Tutte le schede orario a cui hai accesso vengono visualizzate per impostazione predefinita.

![Elenco schede orario](assets/list-of-all-timesheets.png)

1. (Facoltativo) Per aggiornare il filtro nell’elenco delle schede orario, effettua una delle seguenti operazioni:

   * Seleziona **Le mie approvazioni schede orario** nell&#39;angolo superiore destro della pagina per visualizzare solo le schede orario che hai approvato,

     Oppure

     Seleziona **Le mie schede orario** per visualizzare solo le tue schede orario.

     Questa operazione applica i filtri **Le mie approvazioni schede orario** o **Le mie schede orario** all&#39;elenco delle schede orario.

   * Fai clic sull&#39;icona **Filtro** ![Icona Filtro](assets/filter-nwepng.png) per applicare un filtro o crearne uno nuovo. Per informazioni sulla creazione o l&#39;aggiornamento dei filtri, vedere [Creare o modificare filtri in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

   >[!NOTE]
   >
   >Le opzioni Approvazioni schede attività personali e Schede attività personali non vengono visualizzate nella parte superiore dell&#39;elenco delle schede attività o nell&#39;elenco dei filtri se l&#39;amministratore di Workfront o un amministratore di gruppo ha rimosso tali filtri dai controlli elenco nell&#39;area Configura o dal modello di layout. Per ulteriori informazioni, vedere [Personalizzare filtri, visualizzazioni e raggruppamenti utilizzando un modello di layout](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. (Facoltativo) Fai clic sull&#39;icona **Visualizza** ![Visualizza](assets/view-icon.png) o **Raggruppamento** ![Icona Raggruppamento](assets/grouping.png) per applicare una visualizzazione o un raggruppamento o crearne uno nuovo.

   Per informazioni sulla creazione di filtri, viste o raggruppamenti, vedere i seguenti articoli:

   * [Creare o modificare filtri in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Creare o modificare le visualizzazioni in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Creare raggruppamenti in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Seleziona le schede orario da esportare, quindi fai clic sull&#39;icona **Esporta** ![Esporta](assets/export-38x15.png).

   ![Fare clic sull&#39;icona Esporta](assets/export-timesheets.png)

1. Seleziona il tipo di file in cui desideri esportare l’elenco delle schede orario tra le seguenti opzioni:

   * PDF - Paesaggio
   * Verticale PDF
   * PDF - Altre dimensioni
   * Excel
   * Excel (xlsx)
   * Delimitato in tabella

   Un elenco di schede orario viene scaricato nel computer nel formato selezionato e include le seguenti informazioni sulla scheda orario:

   * Date Range
   * Nome del proprietario
   * Ore totali
   * Quantità di lavoro straordinario
   * Nomi approvatori
   * Stato
