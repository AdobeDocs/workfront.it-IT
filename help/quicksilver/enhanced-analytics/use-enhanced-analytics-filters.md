---
title: Applicare i filtri nelle analisi avanzate
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: I filtri nell’area Analisi avanzata di Adobe Workfront consentono di concentrarsi su progetti specifici o su tipi specifici di dati.
author: Nolan
feature: Reports and Dashboards
exl-id: 25854c04-d914-4302-a36b-e8134637efe1
source-git-commit: 6d2494f1ccb2f9b222a953ed8bae922bd0f26389
workflow-type: tm+mt
source-wordcount: '1504'
ht-degree: 0%

---

# Applicare i filtri nelle analisi avanzate

I filtri nell’area Analisi avanzata di Adobe Workfront consentono di concentrarsi su progetti specifici o su tipi specifici di dati. I tipi di filtri utilizzati possono fornire informazioni approfondite su:

* Progetti di tua proprietà
* Visualizzazioni di portfolio o programmi specifiche
* Indicatori prestazioni chiave per un intervallo di tempo specifico (settimana, trimestre, anno fiscale)

Puoi aggiungere e rimuovere i filtri in base alle esigenze e Workfront mantiene i filtri applicati anche se esci.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td>
      <p>Nuovo: Qualsiasi</p>
      <p>oppure</p>
      <p>Corrente: Business o superiore</p></td> 
  </tr>
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td>
      <p>Nuovo: Chiaro o superiore</p>
      <p>oppure</p>
      <p>Corrente: revisione o versione successiva</p>
   </td> 
  </tr>
  <tr> 
   <td>Livello di accesso* </td> 
   <td> <p>Accesso ai progetti in visualizzazione</p> <p>Per visualizzare opzioni di filtro specifiche per i campi del progetto, è inoltre necessario disporre dell'accesso in visualizzazione ad attività, Portfoli e utenti.</p> <p>Nota: se sono selezionate restrizioni nella sezione Imposta restrizioni aggiuntive della finestra di dialogo Modifica livello di accesso, è possibile che dopo l’applicazione del filtro non vengano visualizzate tutte le informazioni nei filtri o nella pagina Analisi avanzata. Per informazioni su come un amministratore di Workfront può modificare il livello di accesso, consulta <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Autorizzazioni oggetto </p> </td> 
   <td> <p>Visualizza</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

## Prerequisiti

Per i prerequisiti per utilizzare Enhanced Analytics, consulta [Prerequisiti](../enhanced-analytics/enhanced-analytics-overview.md#prerequisites) in [Panoramica di analisi avanzate](../enhanced-analytics/enhanced-analytics-overview.md).

## Modificare il filtro dell’intervallo di date {#change-the-date-range-filter}

Per impostazione predefinita, le visualizzazioni nell’area Analisi avanzata mostrano i dati relativi agli ultimi 60 giorni e ai successivi 15 giorni. Puoi selezionare un nuovo intervallo di date e applicarlo a tutte le visualizzazioni nell’area Analisi avanzate. Se esci dalla pagina, l’intervallo di date predefinito viene applicato la volta successiva in cui torni indietro.

>[!TIP]
>
>È inoltre possibile utilizzare i tasti della tastiera per spostarsi, aprire e selezionare un intervallo di date dal widget del calendario.\
>Per ulteriori informazioni, vedere [Scelte rapide da tastiera](../enhanced-analytics/enhanced-analytics-overview.md#keyboard-shortcuts) sezione nell’articolo [Panoramica di analisi avanzate](../enhanced-analytics/enhanced-analytics-overview.md).

Per selezionare un nuovo intervallo di date:

{{step1-to-analytics}}

1. In alto a destra, fai clic sul campo intervallo di date per aprire la visualizzazione calendario.
1. Utilizza le frecce sopra il calendario per individuare il mese della data di inizio, quindi seleziona la data di inizio.

   ![Seleziona intervallo date](assets/filters-select-date-range-350x344.png)

1. Utilizza le frecce sopra il calendario per individuare il mese della data di fine, quindi seleziona la data di fine.
1. (Facoltativo) Per ingrandire un intervallo di date più breve, trascina il mouse su una data specifica di una visualizzazione.

   Tutte le visualizzazioni sullo schermo si aggiornano in base all’intervallo temporale selezionato e accanto ai filtri esistenti viene visualizzato un filtro Intervallo temporale. Questo filtro non viene mantenuto se esci o esci dall’area Analisi avanzate.

   ![Filtro intervallo temporale](assets/timeframe-filter-350x220.png)

## Aggiungi un filtro

Puoi aggiungere filtri in base ai campi predefiniti del progetto, ai campi del modulo personalizzato e ai team principali assegnati ai progetti.

>[!TIP]
>
>È inoltre possibile utilizzare i tasti della tastiera per passare a e aggiungere un nuovo filtro.\
>Per ulteriori informazioni, vedere [Scelte rapide da tastiera](../enhanced-analytics/enhanced-analytics-overview.md#keyboard) sezione nell’articolo [Panoramica di analisi avanzate](../enhanced-analytics/enhanced-analytics-overview.md).

* [Aggiungi un filtro per campo progetto](#add-a-project-field-filter)
* [Aggiungere un filtro modulo personalizzato per un progetto](#add-a-project-custom-form-filter)
* [Aggiungere un filtro Team](#add-a-team-filter)

### Aggiungi un filtro per campo progetto {#add-a-project-field-filter}

I filtri dei campi di Project consentono di filtrare i dati per progetti e attività in base ai valori immessi nei campi inclusi nei progetti per impostazione predefinita.

Sono disponibili i seguenti tipi di filtro per i campi del progetto:

| Campo | Dati visualizzati |
|---|---|
| **Progetto** | Visualizza solo i dati per i progetti selezionati |
| **Programma** | Visualizza i dati solo per i progetti dei programmi selezionati |
| **Portfolio** | Visualizza i dati solo per i progetti nel portfolio selezionato |
| **Condizione** | Visualizza i dati solo per i progetti con le condizioni selezionate più di recente (in target, a rischio o nei guai) |
| **Stato** | Visualizza i dati solo per i progetti con gli stati selezionati più di recente (completo, corrente, in attesa, annullato, ecc.) |
| **Sponsor** | Visualizza i dati solo per i progetti con gli sponsor selezionati |
| **Proprietario progetto** | Visualizza i dati solo per i progetti con i proprietari selezionati |

I filtri dei moduli personalizzati funzionano in modo diverso. Per ulteriori informazioni, consulta [Aggiungere un filtro modulo personalizzato per un progetto](#add-a-project-custom-form-filter).

Per aggiungere un filtro per i campi del progetto:

{{step1-to-analytics}}

1. In alto a sinistra, fai clic su **Aggiungi filtro**, quindi seleziona il tipo di filtro desiderato.

   >[!NOTE]
   >
   >Diversi tipi di filtro visualizzano dati diversi. È possibile utilizzare un solo tipo di filtro in un filtro. Dopo averlo selezionato, un tipo di filtro non è disponibile per l’utilizzo in un altro filtro di campi del progetto.

1. Individuare i valori per i quali si desidera visualizzare i dati immettendo almeno tre caratteri di testo nel **Ricerca** , quindi selezionare ogni valore da includere nel filtro.

   Per selezionare tutti i valori correnti, fare clic su **Seleziona tutto**.

   ![Seleziona valore filtro](assets/select-filter-value-350x251.png)

1. Dopo aver selezionato tutti i valori desiderati, fai clic su **Applica filtro**.

   Il progetto conta sugli aggiornamenti in alto a destra per riflettere i filtri applicati.

1. Ripeti questi passaggi per ogni filtro che desideri aggiungere.

   Man mano che aggiungi i filtri, nelle visualizzazioni sottostanti vengono visualizzati i dati relativi a un massimo di 50 progetti.

   >[!TIP]
   >
   >Per visualizzare i dati di più di 50 progetti visualizzati per impostazione predefinita, puoi:
   >
   >   * Utilizza le frecce in basso a sinistra per visualizzare i successivi 50 progetti in quella visualizzazione.\
   >     ![Freccia di impaginazione](assets/pagination-350x118.png)
   >   
   >   * Utilizza il **Ordina per** in una visualizzazione per visualizzare i progetti in un ordine diverso.\
   >     ![Ordina per menu](assets/sort-by-menu-350x247.png)

   Per modificare l’intervallo di date, consulta [Modificare il filtro dell’intervallo di date](#change-the-date-range-filter).

### Aggiungere un filtro modulo personalizzato per un progetto

Il tipo di filtro modulo personalizzato consente di filtrare i dati per progetti e attività in base ai valori immessi nei campi modulo personalizzato nei progetti. A differenza di altri tipi di filtri di analisi avanzata, è possibile aggiungere più di un filtro modulo personalizzato. Ogni filtro modulo personalizzato contiene i valori immessi solo all’interno del campo selezionato in un modulo personalizzato specifico.

Per aggiungere un filtro modulo personalizzato:

{{step1-to-analytics}}

1. Nell’angolo in alto a sinistra della schermata, fai clic su **Aggiungi filtro**, quindi seleziona **Modulo personalizzato**.

   ![Seleziona filtro modulo personalizzato](assets/select-custom-form-filter-350x271.png)

1. Individuare il modulo personalizzato desiderato immettendo almeno tre caratteri di testo nel **Ricerca** , quindi selezionare il modulo personalizzato.
1. Seleziona il campo desiderato, quindi completa una delle seguenti azioni in base al tipo di campo che stai aggiungendo al filtro:

   >[!NOTE]
   >
   >Non tutti i tipi di campi personalizzati possono essere aggiunti a un filtro. Al momento, la funzione Analisi avanzate supporta solo i tipi di campo elencati di seguito.

   * **Casella di controllo**, **elenco a discesa**, o **pulsante di opzione**: seleziona ogni valore nel campo che desideri includere nel filtro oppure fai clic sul pulsante **Seleziona tutto** casella di controllo.\
     ![Valori casella di controllo](assets/custom-form-filter-checkbox-350x255.png)

   * **Data**: utilizza le frecce per passare a un mese specifico, quindi seleziona la data nel campo che desideri includere nel filtro.\
     ![Valore data](assets/custom-form-filter-date-350x348.png)

   * **Testo**: immetti il testo all’interno del campo da includere nel filtro.\
     ![Valore testo](assets/custom-form-filter-text-350x90.png)

   * **Numero**: immetti il numero all’interno del campo che desideri includere nel filtro.\
     ![Valore numerico](assets/custom-form-filter-number-350x93.png)

1. Dopo aver immesso o selezionato i valori per i quali si desidera filtrare, fare clic su **Applica filtro**.

   Il progetto conta sugli aggiornamenti in alto a destra per riflettere i filtri applicati.

1. Ripeti questi passaggi per ogni filtro che desideri aggiungere.

   Man mano che aggiungi i filtri, nelle visualizzazioni sottostanti vengono visualizzati i dati relativi a un massimo di 50 progetti.

   >[!TIP]
   >
   >Per visualizzare i dati di più di 50 progetti visualizzati per impostazione predefinita, puoi:
   >  
   >   * Utilizza le frecce in basso a sinistra per visualizzare i successivi 50 progetti in quella visualizzazione.\
   >     ![Frecce di impaginazione](assets/pagination-350x118.png)
   >   
   >   * Utilizza il **Ordina per** in una visualizzazione per visualizzare i progetti in un ordine diverso.\
   >     ![Ordina per menu](assets/sort-by-menu-350x247.png)

   Per modificare l’intervallo di date, consulta [Modificare il filtro dell’intervallo di date](#change-the-date-range-filter).

### Aggiungere un filtro Team {#add-a-team-filter}

{{step1-to-analytics}}

1. Nel pannello a sinistra, fai clic su **Persone**.

   ![Seleziona persone](assets/people-area-cropped-qs-350x276.png)

1. In alto a sinistra nella schermata, fai clic su **Aggiungi filtro**, quindi seleziona la **Team** filtro.
1. Individuare i team per i quali si desidera visualizzare i dati immettendo almeno tre caratteri di testo nella **Ricerca** , quindi selezionare ogni team da includere nel filtro. Per selezionare tutti i team, fai clic su **Seleziona tutto**.

   ![Seleziona team](assets/select-team-value-350x253.png)

   >[!NOTE]
   >
   >Tutti i team sono inclusi come opzioni di filtro, indipendentemente dal livello di accesso.

1. Dopo aver selezionato tutti i team desiderati, fai clic su **Applica filtro**.

   Man mano che aggiungi i filtri, i dati vengono visualizzati nelle visualizzazioni di seguito.

   Per modificare l’intervallo di date, consulta [Modificare il filtro dell’intervallo di date](#change-the-date-range-filter).

## Rimuovere un filtro

Puoi rimuovere un filtro in qualsiasi momento. Se rimuovi un filtro, non verrà visualizzato alla prossima visita dell’area Analisi avanzata.

>[!TIP]
>
>È inoltre possibile utilizzare i tasti della tastiera per individuare e rimuovere un filtro esistente.\
>Per ulteriori informazioni, vedere [Scelte rapide da tastiera](../enhanced-analytics/enhanced-analytics-overview.md#keyboard) sezione nell’articolo [Panoramica di analisi avanzate](../enhanced-analytics/enhanced-analytics-overview.md).

Per rimuovere un filtro:

{{step1-to-analytics}}

1. Se desideri rimuovere un campo di progetto o un filtro modulo personalizzato, resta nel **Lavoro** area.

   Oppure

   Per rimuovere un filtro Team, selezionare **Persone** nel pannello a sinistra.

1. Individua il filtro desiderato e fai clic su **X** per rimuoverlo.

   ![Rimuovi](assets/remove-filter-350x213.png)

   Il filtro non è più attivo e non viene visualizzato a meno che non lo si aggiunga nuovamente.
