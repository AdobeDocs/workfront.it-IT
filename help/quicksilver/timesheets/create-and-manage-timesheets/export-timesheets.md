---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Esportare un elenco di fogli presenze
description: In qualità di responsabile delle persone o approvatore della scheda attività, potrebbe essere necessario scaricare un elenco di fogli presenze per visualizzare rapidamente le informazioni sui fogli presenze delle persone di cui sei responsabile. È possibile farlo esportando un elenco di fogli presenze.
author: Alina
feature: Timesheets
exl-id: cb5b1c6c-7800-48f4-ae2c-c4007a161a6c
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 2%

---

# Esportare un elenco di fogli presenze

In qualità di responsabile delle persone o approvatore della scheda attività, potrebbe essere necessario scaricare un elenco di fogli presenze per visualizzare rapidamente le informazioni sui fogli presenze delle persone di cui sei responsabile. È possibile farlo esportando un elenco di fogli presenze.

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
   <td> <p>Revisione o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Visualizza accesso o superiore a Attività e problemi</p> <p>Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizza o autorizzazioni superiori per i fogli presenze</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per sapere quale piano o tipo di licenza hai, contatta il tuo amministratore Workfront.

## Esportare un elenco di fogli presenze

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront.

1. Fai clic su **Schede temporali**. La **Tutto** Il filtro è selezionato per impostazione predefinita.

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Facoltativo) Fai clic sul pulsante **ricerca** icona ![](assets/search-icon.png) e digitare una parola chiave e cercare una scheda attività specifica. Ad esempio, è possibile cercare un intervallo di tempo o il nome del proprietario del set di date.

1. (Facoltativo) Per aggiornare il filtro nell’elenco dei fogli presenze, effettuare una delle seguenti operazioni:

   * Seleziona **Approvazioni foglio presenze personali** nell’angolo in alto a destra della pagina per visualizzare solo i fogli presenze approvati

      Oppure

      Seleziona **Fogli orari personali** per visualizzare solo i fogli presenze.

      Questo applica le approvazioni della scheda attività personale o i filtri della scheda attività personale all&#39;elenco dei fogli presenze.

      ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * Fai clic sull’icona Filtro ![](assets/filter-nwepng.png) per applicare un filtro diverso o crearne uno nuovo. Per informazioni sulla creazione o l’aggiornamento dei filtri, consulta [Creare o modificare filtri in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
   >[!NOTE]
   >
   >Le opzioni Approvazioni schede attività personali e Pagine attività personali non vengono visualizzate nella parte superiore dell&#39;elenco delle schede attività o nell&#39;elenco dei filtri se l&#39;amministratore di Workfront o un amministratore di gruppo hanno rimosso le approvazioni della scheda attività personale e i filtri della scheda attività personale dai controlli elenco nell&#39;area Configurazione o dal modello di layout. Per ulteriori informazioni, consulta i seguenti articoli:
   * [Personalizzare filtri, visualizzazioni e gruppi utilizzando un modello di layout](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)


1. (Facoltativo) Fai clic sul pulsante **Visualizza** ![](assets/view-icon.png) o **Raggruppamento** ![](assets/grouping.png) per applicare una visualizzazione o un raggruppamento diversi o per crearne uno nuovo.

   Per informazioni sulla creazione di filtri, visualizzazioni o raggruppamenti, consulta i seguenti articoli:

   * [Creare o modificare filtri in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Creare o modificare visualizzazioni in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Creare raggruppamenti in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Seleziona i fogli presenze da esportare, quindi fai clic sul pulsante **Esporta**  ![](assets/export-38x15.png) icona.

   ![](assets/all-timesheets-list-with-export-button-nwe-350x262.png)

1. Selezionare il tipo di file in cui si desidera esportare l’elenco dei fogli presenze in dalle opzioni seguenti:

   * PDF Ladscape
   * Verticale PDF
   * PDF altre dimensioni
   * Excel
   * Excel (xlsx)
   * Delimitato da tabulazioni

   Nel formato selezionato viene scaricato nel computer un elenco di fogli presenze con le seguenti informazioni:

   * Intervallo date
   * Nome del proprietario
   * Ore totali
   * Importo straordinario
   * Nomi degli approvatori
   * Stato
