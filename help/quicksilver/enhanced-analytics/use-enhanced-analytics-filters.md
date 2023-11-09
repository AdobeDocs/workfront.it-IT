---
title: Applicare i filtri nelle analisi avanzate
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: I filtri nell’area Analisi avanzata consentono di concentrarsi su progetti specifici o su tipi specifici di dati.
author: Nolan
feature: Reports and Dashboards
exl-id: 25854c04-d914-4302-a36b-e8134637efe1
source-git-commit: bcafa607da733b89747f6b448dd295d9b906d060
workflow-type: tm+mt
source-wordcount: '1484'
ht-degree: 1%

---

# Applicare i filtri nelle analisi avanzate

I filtri nell’area Analisi avanzata consentono di concentrarsi su progetti specifici o su tipi specifici di dati. I tipi di filtri utilizzati possono fornire informazioni approfondite su:

* Progetti di tua proprietà
* Visualizzazioni di portfolio o programmi specifiche
* Indicatori prestazioni chiave per un intervallo di tempo specifico (settimana, trimestre, anno fiscale)

Puoi aggiungere e rimuovere i filtri in base alle esigenze e Adobe Workfront mantiene i filtri applicati anche se esci.

## Requisiti di accesso

Per completare questa attività, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <caption style="text-align: left;">
  *Per informazioni sulla pianificazione, il tipo di licenza o l'accesso disponibili, contattare l'amministratore Workfront.
 </caption> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><a href="https://www.workfront.com/plans" target="_blank">piano Workfront</a>*</p> </td> 
   <td>Business o superiore</td> 
  </tr> 
  <tr> 
   <td> <p><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Panoramica sulle licenze di Adobe Workfront</a>*</p> </td> 
   <td> <p>Revisione o successiva</p> </td> 
  </tr> 
  <tr> 
   <td><b>Livello di accesso*</b> </td> 
   <td> <p>Accesso ai progetti in visualizzazione</p> <p>Per visualizzare opzioni di filtro specifiche per i campi del progetto, è inoltre necessario disporre dell'accesso in visualizzazione ad attività, Portfoli e utenti.</p> <p>Nota: se sono selezionate restrizioni nella sezione Imposta restrizioni aggiuntive della finestra di dialogo Modifica livello di accesso, è possibile che dopo l’applicazione del filtro non vengano visualizzate tutte le informazioni nei filtri o nella pagina Analisi avanzata. Per informazioni su come un amministratore di Workfront può modificare il livello di accesso, consulta <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><b>Autorizzazioni oggetto</b> </p> </td> 
   <td> <p>Visualizza</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Prerequisiti

Per i prerequisiti per utilizzare Enhanced Analytics, consulta [Prerequisiti](../enhanced-analytics/enhanced-analytics-overview.md#prerequi) in [Panoramica di analisi avanzate](../enhanced-analytics/enhanced-analytics-overview.md).

## Modificare il filtro dell’intervallo di date {#change-the-date-range-filter}

Per impostazione predefinita, le visualizzazioni nell’area Analisi avanzata mostrano i dati relativi agli ultimi 60 giorni e ai successivi 15 giorni. Puoi selezionare un nuovo intervallo di date e applicarlo a tutte le visualizzazioni nell’area Analisi avanzate. Se esci dalla pagina, l’intervallo di date predefinito viene applicato la volta successiva in cui torni indietro.

>[!TIP]
>
>È inoltre possibile utilizzare i tasti della tastiera per spostarsi, aprire e selezionare un intervallo di date dal widget del calendario.\
>Per ulteriori informazioni, vedere [Scelte rapide da tastiera](../enhanced-analytics/enhanced-analytics-overview.md#keyboard) sezione nell’articolo [Panoramica di analisi avanzate](../enhanced-analytics/enhanced-analytics-overview.md).

Per selezionare un nuovo intervallo di date:

1. Fai clic sull’icona Menu principale ![](assets/main-menu-icon-16x12.png), quindi seleziona **Analytics**.
1. Nell’angolo in alto a destra dello schermo, fai clic sul campo intervallo di date per aprire la visualizzazione calendario.
1. Utilizza le frecce sopra il calendario per individuare il mese della data di inizio, quindi seleziona la data di inizio.

   ![](assets/filters-select-date-range-350x344.png)

1. Utilizza le frecce sopra il calendario per individuare il mese della data di fine, quindi seleziona la data di fine.
1. (Facoltativo) Per ingrandire un intervallo di date più breve, trascina il mouse su una data specifica di una visualizzazione.

   Tutte le visualizzazioni sullo schermo vengono aggiornate in base all’intervallo di tempo selezionato e accanto ai filtri esistenti viene visualizzato un filtro Intervallo temporale. Questo filtro non viene mantenuto se esci o esci dall’area Analisi avanzate.

   ![](assets/timeframe-filter-350x220.png)

## Aggiungi un filtro

Puoi aggiungere filtri in base ai campi predefiniti del progetto, ai campi del modulo personalizzato e ai team principali assegnati ai progetti.

>[!TIP]
>
>È inoltre possibile utilizzare i tasti della tastiera per passare a e aggiungere un nuovo filtro.\
>Per ulteriori informazioni, vedere [Scelte rapide da tastiera](../enhanced-analytics/enhanced-analytics-overview.md#keyboard) sezione nell’articolo [Panoramica di analisi avanzate](../enhanced-analytics/enhanced-analytics-overview.md).

* [Aggiungi un filtro per campo progetto](#add-a-project-field-filter)
* [Aggiungi un filtro per campo progetto](#add-a-project-field-filter)
* [Aggiungere un filtro Team](#add-a-team-filter)

### Aggiungi un filtro per campo progetto {#add-a-project-field-filter}

I filtri dei campi di Project consentono di filtrare i dati per progetti e attività in base ai valori immessi nei campi inclusi nei progetti per impostazione predefinita.

Sono disponibili i seguenti tipi di filtro per i campi del progetto:

| **Progetto** | Visualizza i dati solo per i progetti selezionati |
|---|---|
| **Programma** | Visualizza i dati solo per i progetti dei programmi selezionati |
| **Portfolio** | Visualizza i dati solo per i progetti nel portfolio selezionato |
| **Condizione** | Visualizza i dati solo per i progetti con le condizioni selezionate più di recente (in target, a rischio o nei guai) |
| **Stato** | Visualizza i dati solo per i progetti con gli stati selezionati più di recente (completo, corrente, in attesa, annullato, ecc.) |
| **Sponsor** | Visualizza i dati solo per i progetti con gli sponsor selezionati |
| **Proprietario progetto** | Visualizza i dati solo per i progetti con i proprietari selezionati |

{style="table-layout:auto"}

I filtri per moduli personalizzati funzionano in modo diverso. Per ulteriori informazioni, consulta [Aggiungi un filtro per campo progetto](#add-a-project-field-filter).

Per aggiungere un filtro per i campi del progetto:

1. Fai clic sull’icona Menu principale ![](assets/main-menu-icon-16x12.png), quindi seleziona **Analytics**.
1. Nell’angolo in alto a sinistra della schermata, fai clic su **Aggiungi filtro**, quindi seleziona il tipo di filtro desiderato.

   >[!NOTE]
   >
   >Diversi tipi di filtro visualizzano dati diversi. È possibile utilizzare un solo tipo di filtro in un filtro. Dopo la selezione, un tipo di filtro non è disponibile per l’utilizzo in un altro filtro di campi del progetto.

1. Individuare i valori per i quali si desidera visualizzare i dati immettendo almeno 3 caratteri di testo nel **Ricerca** , quindi selezionare ogni valore da includere nel filtro.

   Per selezionare tutti i valori correnti, fare clic su **Seleziona tutto**.

   ![](assets/select-filter-value-350x251.png)

1. Dopo aver selezionato tutti i valori desiderati, fai clic su **Applica filtro**.\
   Il conteggio dei progetti nell’angolo in alto a destra della pagina si aggiorna per riflettere i filtri applicati.
1. Ripeti questi passaggi per ogni filtro che desideri aggiungere.

   Man mano che aggiungi i filtri, nelle visualizzazioni sottostanti vengono visualizzati i dati relativi a un massimo di 50 progetti.

   >[!TIP]
   >
   >Per visualizzare i dati di più di 50 progetti visualizzati per impostazione predefinita, puoi:
   >
   >   
   >   
   >   * Utilizza le frecce nell’angolo in basso a sinistra per visualizzare i successivi 50 progetti in tale visualizzazione.\
   >     ![](assets/pagination-350x118.png)
   >   
   >   * Utilizza il menu a discesa Ordina per in una visualizzazione per visualizzare i progetti in un ordine diverso.\
   >     ![](assets/sort-by-menu-350x247.png)
   >   
   >   
   >

   Per modificare l’intervallo di date, consulta [Modificare il filtro dell’intervallo di date](#change-the-date-range-filter).

### Aggiungere un filtro Modulo personalizzato per progetto

Il tipo di filtro Modulo personalizzato consente di filtrare i dati per progetti e attività in base ai valori immessi nei campi Modulo personalizzato dei progetti. A differenza di altri tipi di filtri di analisi avanzata, è possibile aggiungere più di un filtro Modulo personalizzato. Ogni filtro Modulo personalizzato contiene i valori immessi solo all’interno del campo selezionato in un modulo personalizzato specifico.

Per aggiungere un filtro Modulo personalizzato:

1. Fai clic sull’icona Menu principale ![](assets/main-menu-icon-16x12.png), quindi seleziona **Analytics**.
1. Nell’angolo in alto a sinistra della schermata, fai clic su **Aggiungi filtro**, quindi seleziona **Modulo personalizzato**.

   ![](assets/select-custom-form-filter-350x271.png)

1. Individuare il modulo personalizzato desiderato immettendo almeno 3 caratteri di testo nel **Ricerca** , quindi selezionare il modulo personalizzato.
1. Seleziona il campo desiderato, quindi completa una delle seguenti azioni in base al tipo di campo che stai aggiungendo al filtro:

   >[!NOTE]
   >
   >Non tutti i tipi di campo Modulo personalizzato possono essere aggiunti a un filtro. Al momento, la funzione Analisi avanzate supporta solo i tipi di campo elencati sopra.

   * **Casella di controllo**, **elenco a discesa**, o **pulsante di opzione**: seleziona nel campo selezionato ogni valore che desideri includere nel filtro o fai clic sul pulsante **Seleziona tutto** casella di controllo.\
     ![](assets/custom-form-filter-checkbox-350x255.png)

   * **Data**: utilizza le frecce per passare a un mese specifico, quindi seleziona nel campo selezionato la data che desideri includere nel filtro.\
     ![](assets/custom-form-filter-date-350x348.png)

   * **Testo**: immetti il testo all’interno del campo selezionato che desideri includere nel filtro.\
     ![](assets/custom-form-filter-text-350x90.png)

   * **Numero**: immetti all’interno del campo selezionato il numero da includere nel filtro.\
     ![](assets/custom-form-filter-number-350x93.png)

1. Dopo aver immesso o selezionato i valori per i quali si desidera filtrare, fare clic su **Applica filtro**.

   Il conteggio dei progetti nell’angolo in alto a destra della pagina si aggiorna per riflettere i filtri applicati.

1. Ripeti questi passaggi per ogni filtro che desideri aggiungere.

   Man mano che aggiungi i filtri, nelle visualizzazioni sottostanti vengono visualizzati i dati relativi a un massimo di 50 progetti.

   >[!TIP]
   >
   >Per visualizzare i dati di più di 50 progetti visualizzati per impostazione predefinita, puoi:
   >
   >   
   >   
   >   * Utilizza le frecce nell’angolo in basso a sinistra per visualizzare i successivi 50 progetti in tale visualizzazione.\
   >     ![](assets/pagination-350x118.png)
   >   
   >   * Utilizza il menu a discesa Ordina per in una visualizzazione per visualizzare i progetti in un ordine diverso.\
   >     ![](assets/sort-by-menu-350x247.png)
   >   
   >   
   >

   Per modificare l’intervallo di date, consulta [Modificare il filtro dell’intervallo di date](#change-the-date-range-filter).

### Aggiungere un filtro Team {#add-a-team-filter}

1. Fai clic sull’icona Menu principale ![](assets/main-menu-icon-16x12.png), quindi seleziona **Analytics**.
1. Nel pannello a sinistra, fai clic su **Persone**.

   ![](assets/people-area-cropped-qs-350x276.png)

1. Nell’angolo in alto a sinistra della schermata, fai clic su **Aggiungi filtro**, quindi seleziona la **Team** filtro.
1. Individuare i team per i quali si desidera visualizzare i dati immettendo almeno 3 caratteri di testo nella **Ricerca** , quindi selezionare ogni team da includere nel filtro. Per selezionare tutti i team, fai clic su **Seleziona tutto**.

   ![](assets/select-team-value-350x253.png)

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

1. Fai clic sull’icona Menu principale ![](assets/main-menu-icon-16x12.png), quindi seleziona **Analytics**.
1. Se desideri rimuovere un filtro Lavoro, resta nel **Lavoro** area.

   Oppure

   Per rimuovere un filtro Persone, selezionare **Persone** nel pannello a sinistra.

1. Individua il filtro desiderato e fai clic su **X** per rimuoverlo.

   ![](assets/remove-filter-350x213.png)

   Il filtro non è più attivo e non viene visualizzato a meno che non lo si aggiunga nuovamente.
