---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Riferimento a un modulo personalizzato in un rapporto
description: È possibile fare riferimento ai moduli personalizzati di un oggetto in Viste, Filtri e Gruppi di un rapporto per tale oggetto.
author: Nolan
feature: Reports and Dashboards
exl-id: 8b0d2e7f-cc92-4f43-a91c-ab2b2d8a1c01
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '994'
ht-degree: 2%

---

# Riferimento a un modulo personalizzato in un rapporto

È possibile fare riferimento ai moduli personalizzati di un oggetto in Viste, Filtri e Gruppi di un rapporto per tale oggetto.

È possibile fare riferimento al contenuto dei moduli personalizzati da includere in un rapporto oppure fare riferimento a informazioni sui moduli personalizzati da includere in un rapporto.

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

## Prerequisiti

Il modulo personalizzato deve esistere prima di potervi fare riferimento in un rapporto.

Per ulteriori informazioni sulla creazione di moduli personalizzati, vedere [Creare o modificare un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## Riferimento al contenuto dei moduli personalizzati

È possibile fare riferimento a campi all’interno di moduli personalizzati. Dopo aver applicato un modulo personalizzato a un oggetto, tutti i campi associati a tale modulo personalizzato sono disponibili per essere referenziati in un rapporto come qualsiasi altro campo dell’oggetto.

>[!NOTE]
>
>Per i campi con più opzioni, tutte le opzioni sono disponibili nei filtri e nei prompt del rapporto, incluse quelle nascoste.\
>Per ulteriori informazioni sull’eliminazione delle scelte da un campo personalizzato con più opzioni, consulta l’articolo [Creare o modificare un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

Durante la creazione del rapporto, è sufficiente utilizzare il tipo di oggetto del modulo come origine del campo e utilizzare il nome del campo personalizzato come nome del campo.

Ad esempio, potrebbe essere applicato un modulo personalizzato a tutti i progetti che includono il campo personalizzato **Consulente**. Per creare un rapporto che elenca tutti i progetti in cui Olivia Kim è il consulente, utilizza il **Progetto** tipo di oggetto come origine del campo e utilizzare **Consulente** come nome del campo. Imposta il qualificatore del filtro su **Uguale** Poi digita Olivia Kim.

![](assets/qs-consultant-filter-example-350x126.png)

Per ulteriori informazioni sulla creazione di un rapporto, consulta l’articolo [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Informazioni di riferimento sui moduli personalizzati

È possibile fare riferimento a informazioni sui moduli personalizzati, ad esempio il nome di qualsiasi modulo personalizzato associato a un oggetto.

&#x200B; A seconda dell’elemento (Visualizzazione, Filtro o Raggruppamento), è possibile fare riferimento a:

* Il modulo personalizzato principale applicato a un oggetto:

   Modulo visualizzato per primo nella pagina Dettagli dell’oggetto.

* Tutti i moduli personalizzati (se a un oggetto sono applicati più moduli personalizzati)

È possibile fare riferimento a moduli personalizzati in Viste, Filtri e Gruppi:

* [Riferimento a moduli personalizzati in una visualizzazione rapporto (colonna)](#reference-custom-forms-in-a-report-view-column)
* [Riferimento a moduli personalizzati in un filtro per report](#reference-custom-forms-in-a-report-filter)
* [Riferimento a moduli personalizzati in un raggruppamento di rapporti](#reference-custom-forms-in-a-report-grouping)

### Riferimento a moduli personalizzati in una visualizzazione rapporto (colonna) {#reference-custom-forms-in-a-report-view-column}

Per visualizzare tutti i moduli personalizzati associati a un oggetto:

1. Inizia a creare un rapporto come descritto nell’articolo [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Sulla **Colonne** espandere il tipo di oggetto a cui è applicato il modulo personalizzato a cui si desidera fare riferimento, quindi fare clic su **Nome categoria**.\
   Ad esempio, per visualizzare tutti i moduli personalizzati associati a un’attività, espandere la **Attività** origine campo, quindi fai clic sul pulsante **Nome categoria** nome del campo.\
   ![](assets/qs-category-name-column-350x267.png)

Per visualizzare solo il modulo personalizzato principale associato all’oggetto:

1. Inizia a creare un rapporto come descritto nell’articolo [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Sulla **Colonne** scheda , espandi **Categoria** origine campo, quindi fai clic sul pulsante **Nome** nome del campo.\
   ![](assets/qs-category-name-column-2-350x248.png)

### Riferimento a moduli personalizzati in un filtro per report {#reference-custom-forms-in-a-report-filter}

Per filtrare tutti i moduli personalizzati associati al tipo di oggetto:

1. Inizia a creare un rapporto come descritto nell’articolo [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Sulla **Filtri** scheda, espandi **Categorie**, quindi fai clic su **Nome**.\
   ![](assets/qs-categories-name-filter-350x311.png)

1. Selezionare il qualificatore di condizione che si desidera utilizzare:

   * Blank
   * Not Blank
   * Contiene
   * Non contiene
   * Equal (Case Insensitive)
   * Not Equal

   Per ulteriori informazioni su ciascun qualificatore, consulta l’articolo [Modificatori di filtri e condizioni](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   >[!NOTE]
   >
   >Se il campo a cui si sta filtrando dispone di più opzioni e si utilizza il **Diverso** o **Non contiene** qualificatori, questo filtra i risultati che contengono solo la scelta specificata. Se il campo contiene opzioni aggiuntive, inclusa quella specificata, tali risultati non vengono filtrati dal rapporto. Ciò include il filtro per più Forms personalizzati se sono collegati allo stesso oggetto.

1. Iniziare a digitare il nome del modulo personalizzato su cui si desidera filtrare, quindi fare clic sul nome quando viene visualizzato nell’elenco a discesa.
1. (Facoltativo) Fai clic su **Aggiungi un’altra regola filtro**, quindi ripeti i passaggi 2-4 per creare regole di filtro aggiuntive.
1. Fai clic su **Salva e chiudi**.

Per filtrare solo il modulo personalizzato principale associato al tipo di oggetto:

1. Inizia a creare un rapporto come descritto nell’articolo [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Sulla **Filtri** scheda , espandi **Categoria** origine campo, quindi fai clic sul pulsante **Nome** nome del campo.\
   ![](assets/qs-category-name-filter-350x437.png)

1. Selezionare il qualificatore di condizione che si desidera utilizzare:

   * Blank
   * Not Blank
   * Contiene
   * Non contiene
   * Equal (Case Insensitive)
   * Not Equal

   Per ulteriori informazioni su ciascun qualificatore, consulta l’articolo [Modificatori di filtri e condizioni](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. Iniziare a digitare il nome del modulo personalizzato su cui si desidera filtrare, quindi fare clic sul nome quando viene visualizzato nell’elenco a discesa.
1. (Facoltativo) Fai clic su **Aggiungi un’altra regola filtro**, quindi ripeti i passaggi 2-4 per creare regole di filtro aggiuntive.
1. Fai clic su **Salva e chiudi**.

### Riferimento a moduli personalizzati in un raggruppamento di rapporti {#reference-custom-forms-in-a-report-grouping}

>[!NOTE]
>
>È possibile raggruppare gli elementi solo in base al modulo personalizzato principale associato all’oggetto; non è possibile raggruppare gli elementi in base a tutti i moduli associati all’oggetto.

1. Inizia a creare un rapporto come descritto nell’articolo [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Sulla **Raggruppamenti** scheda, espandi **Categoria**, quindi fai clic su **Nome**.\
   ![](assets/qs-category-name-grouping-350x373.png)
