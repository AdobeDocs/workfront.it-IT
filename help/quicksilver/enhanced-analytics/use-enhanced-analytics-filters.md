---
title: Applicare i filtri nelle analisi avanzate
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: I filtri nell’area Analisi avanzata di Adobe Workfront consentono di concentrarsi su progetti specifici o su tipi specifici di dati.
author: Nolan
feature: Reports and Dashboards
exl-id: 25854c04-d914-4302-a36b-e8134637efe1
source-git-commit: 2a6e767036ae702f6c19dc71cdb11dae8e9e37ea
workflow-type: tm+mt
source-wordcount: '1525'
ht-degree: 0%

---

# Applicare i filtri nelle analisi avanzate

>[!IMPORTANT]
>
>Analisi avanzata è stato rimosso da Workfront il 27 maggio. Workfront Data Connect è una soluzione nuova e alternativa che può essere utilizzata per replicare qualsiasi visualizzazione avanzata di Analytics attualmente in uso. <br>Per ulteriori informazioni, consulta la [Guida all&#39;obsolescenza di Enhanced Analytics](/help/quicksilver/product-announcements/announcements/enhanced-analytics-deprecation.md).


<!-- Audited: 12/2023 -->

I filtri nell’area Analisi avanzata di Adobe Workfront consentono di concentrarsi su progetti specifici o su tipi specifici di dati. I tipi di filtri utilizzati possono fornire insight su:

* Progetti di tua proprietà
* Visualizzazioni di portfolio o programmi specifiche
* Indicatori prestazioni chiave per un intervallo di tempo specifico (settimana, trimestre, anno fiscale)

Puoi aggiungere e rimuovere i filtri in base alle esigenze e Workfront mantiene i filtri applicati anche se esci.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td>
      <p>Nuovo: Qualsiasi</p>
      <p>oppure</p>
      <p>Corrente: Business o superiore</p></td> 
  </tr>
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td>
      <p>Nuovo: Chiaro o superiore</p>
      <p>oppure</p>
      <p>Corrente: revisione o versione successiva</p>
   </td> 
  </tr>
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td> <p>Accesso ai progetti in visualizzazione</p> <p>Per visualizzare opzioni di filtro specifiche per i campi del progetto, è inoltre necessario disporre dell'accesso in visualizzazione ad attività, portafogli e utenti.</p> <p>Nota: se sono selezionate restrizioni nella sezione <strong>Imposta restrizioni aggiuntive</strong> della finestra di dialogo Modifica livello di accesso, è possibile che dopo l'applicazione del filtro non vengano visualizzate tutte le informazioni nei filtri o nella pagina Analisi avanzata.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Autorizzazioni oggetto </p> </td> 
   <td> <p>Visualizza</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

Per i prerequisiti per l&#39;utilizzo di Analisi avanzate, vedere [Prerequisiti](../enhanced-analytics/enhanced-analytics-overview.md#prerequisites) in [Panoramica di Analisi avanzate](../enhanced-analytics/enhanced-analytics-overview.md).

## Modificare il filtro dell’intervallo di date {#change-the-date-range-filter}

Per impostazione predefinita, le visualizzazioni nell’area Analisi avanzata mostrano i dati relativi agli ultimi 60 giorni e ai successivi 15 giorni. Puoi selezionare un nuovo intervallo di date e applicarlo a tutte le visualizzazioni nell’area Analisi avanzate. Se esci dalla pagina, l’intervallo di date predefinito viene applicato la volta successiva in cui torni indietro.

>[!TIP]
>
>È inoltre possibile utilizzare i tasti della tastiera per spostarsi, aprire e selezionare un intervallo di date dal widget del calendario.\
>Per ulteriori informazioni, consulta la sezione [Scelte rapide da tastiera](../enhanced-analytics/enhanced-analytics-overview.md#keyboard-shortcuts) nell&#39;articolo [Panoramica sulle analisi avanzate](../enhanced-analytics/enhanced-analytics-overview.md).

Per selezionare un nuovo intervallo di date:

{{step1-to-analytics}}

1. In alto a destra, fai clic sul campo intervallo di date per aprire la visualizzazione calendario.
1. Utilizza le frecce sopra il calendario per individuare il mese della data di inizio, quindi seleziona la data di inizio.

   ![Seleziona intervallo date](assets/filters-select-date-range-350x344.png)

1. Utilizza le frecce sopra il calendario per individuare il mese della data di fine, quindi seleziona la data di fine.
1. (Facoltativo) Per ingrandire un intervallo di date più breve, trascina il mouse su una data specifica di una visualizzazione.

   Tutte le visualizzazioni sullo schermo si aggiornano in base all’intervallo temporale selezionato e accanto ai filtri esistenti viene visualizzato un filtro Intervallo temporale. Questo filtro non viene mantenuto se esci o esci dall’area Analisi avanzate.

   ![Filtro intervallo di tempo](assets/timeframe-filter-350x220.png)

## Aggiungi un filtro

Puoi aggiungere filtri in base ai campi predefiniti del progetto, ai campi del modulo personalizzato e ai team principali assegnati ai progetti.

>[!TIP]
>
>È inoltre possibile utilizzare i tasti della tastiera per passare a e aggiungere un nuovo filtro.\
>Per ulteriori informazioni, consulta la sezione [Scelte rapide da tastiera](../enhanced-analytics/enhanced-analytics-overview.md#keyboard) nell&#39;articolo [Panoramica sulle analisi avanzate](../enhanced-analytics/enhanced-analytics-overview.md).

* [Aggiungi un filtro per il campo del progetto](#add-a-project-field-filter)
* [Aggiungi un filtro modulo personalizzato per progetto](#add-a-project-custom-form-filter)
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

I filtri dei moduli personalizzati funzionano in modo diverso. Per ulteriori informazioni, vedere [Aggiungere un filtro modulo personalizzato per un progetto](#add-a-project-custom-form-filter).

Per aggiungere un filtro per i campi del progetto:

{{step1-to-analytics}}

1. In alto a sinistra, fai clic su **Aggiungi filtro**, quindi seleziona il tipo di filtro desiderato.

   >[!NOTE]
   >
   >Diversi tipi di filtro visualizzano dati diversi. È possibile utilizzare un solo tipo di filtro in un filtro. Dopo averlo selezionato, un tipo di filtro non è disponibile per l’utilizzo in un altro filtro di campi del progetto.

1. Individuare i valori per i quali si desidera visualizzare i dati immettendo almeno tre caratteri di testo nel campo **Ricerca**, quindi selezionare ogni valore da includere nel filtro.

   Per selezionare tutti i valori correnti, fare clic su **Seleziona tutto**.

   ![Seleziona valore filtro](assets/select-filter-value-350x251.png)

1. Dopo aver selezionato tutti i valori desiderati, fare clic su **Applica filtro**.

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
   >   * Utilizza il menu a discesa **Ordina per** in una visualizzazione per visualizzare i progetti in un ordine diverso.\
   >     ![Ordina per menu](assets/sort-by-menu-350x247.png)

   Per modificare l&#39;intervallo di date, vedere [Modificare il filtro dell&#39;intervallo di date](#change-the-date-range-filter).

### Aggiungere un filtro modulo personalizzato per un progetto

Il tipo di filtro modulo personalizzato consente di filtrare i dati per progetti e attività in base ai valori immessi nei campi modulo personalizzato nei progetti. A differenza di altri tipi di filtri di analisi avanzata, è possibile aggiungere più di un filtro modulo personalizzato. Ogni filtro modulo personalizzato contiene i valori immessi solo all’interno del campo selezionato in un modulo personalizzato specifico.

Per aggiungere un filtro modulo personalizzato:

{{step1-to-analytics}}

1. Nell&#39;angolo in alto a sinistra della schermata, fai clic su **Aggiungi filtro**, quindi seleziona **Modulo personalizzato**.

   ![Seleziona filtro modulo personalizzato](assets/select-custom-form-filter-350x271.png)

1. Individua il modulo personalizzato inserendo almeno tre caratteri di testo nel campo **Ricerca**, quindi seleziona il modulo personalizzato.
1. Seleziona il campo desiderato, quindi completa una delle seguenti azioni in base al tipo di campo che stai aggiungendo al filtro:

   >[!NOTE]
   >
   >Non tutti i tipi di campi personalizzati possono essere aggiunti a un filtro. Al momento, la funzione Analisi avanzate supporta solo i tipi di campo elencati di seguito.

   * **Casella di controllo**, **elenco a discesa** o **pulsante di opzione**: selezionare ogni valore nel campo da includere nel filtro oppure fare clic sulla casella di controllo **Seleziona tutto**.\
     ![Valori casella di controllo](assets/custom-form-filter-checkbox-350x255.png)

   * **Data**: utilizza le frecce per passare a un mese specifico, quindi seleziona la data nel campo che desideri includere nel filtro.\
     ![Valore data](assets/custom-form-filter-date-350x348.png)

   * **Testo**: immetti il testo all&#39;interno del campo che desideri includere nel filtro.\
     ![Valore testo](assets/custom-form-filter-text-350x90.png)

   * **Numero**: immettere il numero nel campo che si desidera includere nel filtro.\
     ![Valore numerico](assets/custom-form-filter-number-350x93.png)

1. Dopo aver immesso o selezionato i valori per cui si desidera filtrare, fare clic su **Applica filtro**.

   Il progetto conta sugli aggiornamenti in alto a destra per riflettere i filtri applicati.

1. Ripeti questi passaggi per ogni filtro che desideri aggiungere.

   Man mano che aggiungi i filtri, nelle visualizzazioni sottostanti vengono visualizzati i dati relativi a un massimo di 50 progetti.

   >[!TIP]
   >
   >Per visualizzare i dati di più di 50 progetti visualizzati per impostazione predefinita, puoi:
   >  
   >   * Utilizza le frecce in basso a sinistra per visualizzare i successivi 50 progetti in quella visualizzazione.\
   >     ![Frecce di paginazione](assets/pagination-350x118.png)
   >   
   >   * Utilizza il menu a discesa **Ordina per** in una visualizzazione per visualizzare i progetti in un ordine diverso.\
   >     ![Ordina per menu](assets/sort-by-menu-350x247.png)

   Per modificare l&#39;intervallo di date, vedere [Modificare il filtro dell&#39;intervallo di date](#change-the-date-range-filter).

### Aggiungere un filtro Team {#add-a-team-filter}

{{step1-to-analytics}}

1. Nel pannello a sinistra, fai clic su **Persone**.

   ![Seleziona persone](assets/people-area-cropped-qs-350x276.png)

1. In alto a sinistra nella schermata, fai clic su **Aggiungi filtro**, quindi seleziona il filtro **Team**.
1. Individuare i team per i quali si desidera visualizzare i dati immettendo almeno tre caratteri di testo nel campo **Ricerca**, quindi selezionare ogni team che si desidera includere nel filtro. Per selezionare tutti i team, fare clic su **Seleziona tutto**.

   ![Seleziona team](assets/select-team-value-350x253.png)

   >[!NOTE]
   >
   >Tutti i team sono inclusi come opzioni di filtro, indipendentemente dal livello di accesso.

1. Dopo aver selezionato tutti i team desiderati, fare clic su **Applica filtro**.

   Man mano che aggiungi i filtri, i dati vengono visualizzati nelle visualizzazioni di seguito.

   Per modificare l&#39;intervallo di date, vedere [Modificare il filtro dell&#39;intervallo di date](#change-the-date-range-filter).

## Rimuovere un filtro

Puoi rimuovere un filtro in qualsiasi momento. Se rimuovi un filtro, non verrà visualizzato alla prossima visita dell’area Analisi avanzata.

>[!TIP]
>
>È inoltre possibile utilizzare i tasti della tastiera per individuare e rimuovere un filtro esistente.\
>Per ulteriori informazioni, consulta la sezione [Scelte rapide da tastiera](../enhanced-analytics/enhanced-analytics-overview.md#keyboard) nell&#39;articolo [Panoramica sulle analisi avanzate](../enhanced-analytics/enhanced-analytics-overview.md).

Per rimuovere un filtro:

{{step1-to-analytics}}

1. Se vuoi rimuovere un campo di progetto o un filtro modulo personalizzato, resta nell&#39;area **Lavoro**.

   Oppure

   Se vuoi rimuovere un filtro Team, seleziona **Persone** nel pannello a sinistra.

1. Individuare il filtro desiderato e fare clic su **X** per rimuoverlo.

   ![Rimuovi](assets/remove-filter-350x213.png)

   Il filtro non è più attivo e non viene visualizzato a meno che non lo si aggiunga nuovamente.
