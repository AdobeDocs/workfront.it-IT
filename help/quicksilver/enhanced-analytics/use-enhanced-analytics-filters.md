---
title: Applicazione di filtri in Analisi avanzata
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: I filtri nell’area Analisi avanzata consentono di concentrarsi su progetti specifici o su tipi specifici di dati. I tipi di filtri utilizzati possono fornire informazioni approfondite su - EDIT ME.
author: Nolan
feature: Reports and Dashboards
exl-id: 25854c04-d914-4302-a36b-e8134637efe1
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1501'
ht-degree: 0%

---

# Applicazione di filtri in Analisi avanzata

I filtri nell’area Analisi avanzata consentono di concentrarsi su progetti specifici o su tipi specifici di dati. I tipi di filtri utilizzati possono fornire informazioni approfondite su:

* Progetti di proprietà
* Viste specifiche del portafoglio o del programma
* Indicatori chiave di performance per un periodo di tempo specifico (settimana, trimestre, anno fiscale)

Puoi aggiungere e rimuovere i filtri in base alle esigenze; Adobe Workfront conserva i filtri applicati anche in caso di disconnessione.

## Requisiti di accesso

Per completare questa attività, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <caption style="text-align: left;">
  *Per sapere quale piano, tipo di licenza o accesso si dispone, contattare l'amministratore Workfront.
 </caption> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><a href="https://www.workfront.com/plans" target="_blank">piano Workfront</a>*</p> </td> 
   <td>Aziende o superiore</td> 
  </tr> 
  <tr> 
   <td> <p><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Panoramica sulle licenze di Adobe Workfront</a>*</p> </td> 
   <td> <p>Revisione o superiore</p> </td> 
  </tr> 
  <tr> 
   <td><b>Livello di accesso*</b> </td> 
   <td> <p>Visualizza accesso a progetti</p> <p>È inoltre necessario disporre dell’accesso Visualizza a Attività, Portfoli e Utenti per visualizzare opzioni di filtro per campi di progetto specifiche.</p> <p>Nota: Se sono selezionate delle limitazioni nella sezione Imposta restrizioni aggiuntive della finestra di dialogo Modifica livello di accesso , è possibile che dopo l’applicazione del filtro non vengano visualizzate tutte le informazioni contenute nei filtri o nella pagina Analisi avanzata. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><b>Autorizzazioni oggetto</b> </p> </td> 
   <td> <p>Visualizza</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Prerequisiti

Per i prerequisiti per l’utilizzo di Analytics avanzato, consulta [Prerequisiti](../enhanced-analytics/enhanced-analytics-overview.md#prerequi) in [Panoramica dell’analisi migliorata](../enhanced-analytics/enhanced-analytics-overview.md).

## Modificare il filtro dell’intervallo di date {#change-the-date-range-filter}

Per impostazione predefinita, le visualizzazioni nell’area Analisi avanzata mostrano i dati relativi agli ultimi 60 giorni e ai successivi 15 giorni. Puoi selezionare un nuovo intervallo di date e applicarlo a tutte le visualizzazioni nell’area Analisi avanzata. Se ti allontani dalla pagina, l’intervallo di date predefinito viene applicato alla successiva navigazione.

>[!TIP]
>
>È inoltre possibile utilizzare i tasti della tastiera per accedere, aprire e selezionare un intervallo di date dal widget Calendario.\
>Per ulteriori informazioni, consulta la sezione [Scelte rapide da tastiera](../enhanced-analytics/enhanced-analytics-overview.md#keyboard) sezione dell&#39;articolo [Panoramica dell’analisi migliorata](../enhanced-analytics/enhanced-analytics-overview.md).

Per selezionare un nuovo intervallo di date:

1. Fai clic sull’icona Menu principale ![](assets/main-menu-icon-16x12.png), quindi seleziona **Analytics**.
1. Nell’angolo in alto a destra dello schermo, fai clic sul campo intervallo di date per aprire la visualizzazione calendario.
1. Usa le frecce sopra il calendario per individuare il mese della data di inizio, quindi seleziona la data di inizio.

   ![](assets/filters-select-date-range-350x344.png)

1. Usa le frecce sopra il calendario per individuare il mese della data di fine, quindi seleziona la data di fine.
1. (Facoltativo) Per ingrandire un intervallo di date più piccolo, trascina il mouse da una data specifica all’altra su una delle visualizzazioni.

   Tutte le visualizzazioni sullo schermo vengono aggiornate in base all’intervallo temporale selezionato e accanto a eventuali filtri esistenti viene visualizzato un filtro Timeframe. Questo filtro non viene mantenuto se ci si disconnette o ci si allontana dall&#39;area Analisi avanzata.

   ![](assets/timeframe-filter-350x220.png)

## Aggiungere un filtro

È possibile aggiungere filtri basati sui campi di progetto predefiniti, sui campi Modulo personalizzato e sui team domestici assegnati ai progetti.

>[!TIP]
>
>È inoltre possibile utilizzare i tasti della tastiera per accedere e aggiungere un nuovo filtro.\
>Per ulteriori informazioni, consulta la sezione [Scelte rapide da tastiera](../enhanced-analytics/enhanced-analytics-overview.md#keyboard) sezione dell&#39;articolo [Panoramica dell’analisi migliorata](../enhanced-analytics/enhanced-analytics-overview.md).

* [Aggiungere un filtro per i campi del progetto](#add-a-project-field-filter)
* [Aggiungere un filtro per i campi del progetto](#add-a-project-field-filter)
* [Aggiungere un filtro Team](#add-a-team-filter)

### Aggiungere un filtro per i campi del progetto {#add-a-project-field-filter}

I filtri per i campi del progetto consentono di filtrare i dati per progetti e attività in base ai valori inseriti nei campi inclusi nei progetti per impostazione predefinita.

Sono disponibili i seguenti tipi di filtro per campi del progetto:

| **Progetto** | Visualizza i dati solo per i progetti selezionati |
|---|---|
| **Programma** | Visualizza i dati solo per i progetti nei programmi selezionati |
| **Portfolio** | Visualizza i dati solo per i progetti nei portfolio selezionati |
| **Condizione** | Visualizza i dati solo per i progetti per i quali le condizioni selezionate sono state più di recente (su target, a rischio o in difficoltà) |
| **Stato** | Visualizza i dati solo per i progetti per i quali gli stati selezionati più di recente sono stati selezionati (completi, correnti, in attesa, annullati, ecc.) |
| **Sponsor** | Visualizza i dati solo per i progetti con gli sponsor selezionati |
| **Proprietario progetto** | Visualizza i dati solo per i progetti con i proprietari del progetto selezionati |

{style=&quot;table-layout:auto&quot;}

I filtri modulo personalizzati funzionano diversamente. Per ulteriori informazioni, consulta [Aggiungere un filtro per i campi del progetto](#add-a-project-field-filter).

Per aggiungere un filtro di campo del progetto:

1. Fai clic sull’icona Menu principale ![](assets/main-menu-icon-16x12.png), quindi seleziona **Analytics**.
1. Nell’angolo in alto a sinistra dello schermo, fai clic su **Aggiungi filtro**, quindi seleziona il tipo di filtro desiderato.

   >[!NOTE]
   >
   >Diversi tipi di filtro visualizzano dati diversi. In un filtro puoi utilizzare un solo tipo di filtro. Dopo aver selezionato, un tipo di filtro non è disponibile per l’utilizzo in un altro filtro di campo del progetto.

1. Individua i valori per i quali desideri visualizzare i dati immettendo almeno 3 caratteri di testo nel **Ricerca** , quindi seleziona ogni valore da includere nel filtro.

   Per selezionare tutti i valori correnti, fai clic su **Seleziona tutto**.

   ![](assets/select-filter-value-350x251.png)

1. Dopo aver selezionato tutti i valori desiderati, fai clic su **Applica filtro**.\
   Il conteggio dei progetti nell’angolo in alto a destra della pagina viene aggiornato per riflettere i filtri applicati.
1. Ripeti questi passaggi per ogni filtro che desideri aggiungere.

   Quando aggiungi dei filtri, i dati vengono visualizzati nelle visualizzazioni seguenti per un massimo di 50 progetti.

   >[!TIP]
   >
   >Per visualizzare i dati per più dei 50 progetti visualizzati per impostazione predefinita, puoi effettuare le seguenti operazioni:
   >
   >   
   >   
   >   * Utilizza le frecce nell’angolo in basso a sinistra per visualizzare i successivi 50 progetti in quella visualizzazione.\
      >     ![](assets/pagination-350x118.png)
   >   
   >   * Per visualizzare i progetti in un ordine diverso, utilizza il menu a discesa Ordina per di una visualizzazione.\
      >     ![](assets/sort-by-menu-350x247.png)


   Per regolare l’intervallo di date, vedi [Modificare il filtro dell’intervallo di date](#change-the-date-range-filter).

### Aggiungere un filtro Modulo personalizzato per un progetto

Il tipo di filtro Modulo personalizzato consente di filtrare i dati per progetti e attività in base ai valori immessi nei campi Modulo personalizzato nei progetti. A differenza di altri tipi di filtro di analisi avanzata, è possibile aggiungere più di un filtro Modulo personalizzato. Ogni filtro Modulo personalizzato contiene valori immessi solo all’interno del campo selezionato in un modulo personalizzato specifico.

Per aggiungere un filtro Modulo personalizzato:

1. Fai clic sull’icona Menu principale ![](assets/main-menu-icon-16x12.png), quindi seleziona **Analytics**.
1. Nell’angolo in alto a sinistra dello schermo, fai clic su **Aggiungi filtro**, quindi seleziona **Modulo personalizzato**.

   ![](assets/select-custom-form-filter-350x271.png)

1. Individuare il modulo personalizzato desiderato inserendo almeno 3 caratteri di testo nel campo **Ricerca** , quindi selezionare il modulo personalizzato.
1. Seleziona il campo desiderato, quindi completa una delle azioni seguenti in base al tipo di campo che stai aggiungendo al filtro:

   >[!NOTE]
   >
   >Non è possibile aggiungere a un filtro tutti i tipi di campo Modulo personalizzato. Al momento, l’analisi avanzata supporta solo i tipi di campo elencati sopra.

   * **Casella di controllo**, **a discesa** oppure **pulsante di scelta**: Seleziona ogni valore nel campo selezionato da includere nel filtro oppure fai clic sul pulsante **Seleziona tutto** casella di controllo.\
      ![](assets/custom-form-filter-checkbox-350x255.png)

   * **Data**: Utilizza le frecce per passare a un mese specifico, quindi seleziona la data nel campo selezionato che desideri includere nel filtro.\
      ![](assets/custom-form-filter-date-350x348.png)

   * **Testo**: Immetti il testo all’interno del campo selezionato che desideri includere nel filtro.\
      ![](assets/custom-form-filter-text-350x90.png)

   * **Numero**: Immetti il numero all’interno del campo selezionato che desideri includere nel filtro.\
      ![](assets/custom-form-filter-number-350x93.png)

1. Dopo aver immesso o selezionato i valori per i quali si desidera filtrare, fare clic su **Applica filtro**.

   Il conteggio dei progetti nell’angolo in alto a destra della pagina viene aggiornato per riflettere i filtri applicati.

1. Ripeti questi passaggi per ogni filtro che desideri aggiungere.

   Quando aggiungi dei filtri, i dati vengono visualizzati nelle visualizzazioni seguenti per un massimo di 50 progetti.

   >[!TIP]
   >
   >Per visualizzare i dati per più dei 50 progetti visualizzati per impostazione predefinita, puoi effettuare le seguenti operazioni:
   >
   >   
   >   
   >   * Utilizza le frecce nell’angolo in basso a sinistra per visualizzare i successivi 50 progetti in quella visualizzazione.\
      >     ![](assets/pagination-350x118.png)
   >   
   >   * Per visualizzare i progetti in un ordine diverso, utilizza il menu a discesa Ordina per di una visualizzazione.\
      >     ![](assets/sort-by-menu-350x247.png)


   Per regolare l’intervallo di date, vedi [Modificare il filtro dell’intervallo di date](#change-the-date-range-filter).

### Aggiungere un filtro Team {#add-a-team-filter}

1. Fai clic sull’icona Menu principale ![](assets/main-menu-icon-16x12.png), quindi seleziona **Analytics**.
1. Nel pannello a sinistra, fai clic su **Persone**.

   ![](assets/people-area-cropped-qs-350x276.png)

1. Nell’angolo in alto a sinistra dello schermo, fai clic su **Aggiungi filtro**, quindi seleziona la **Team** filtro.
1. Individua i team per i quali desideri visualizzare i dati immettendo almeno 3 caratteri di testo nel **Ricerca** , quindi seleziona ogni team da includere nel filtro. Per selezionare tutti i team, fai clic su **Seleziona tutto**.

   ![](assets/select-team-value-350x253.png)

   >[!NOTE]
   >
   >Tutti i team sono inclusi come opzioni di filtro, indipendentemente dal livello di accesso.


1. Dopo aver selezionato tutti i team desiderati, fai clic su **Applica filtro**.

   Quando aggiungi dei filtri, i dati vengono visualizzati nelle visualizzazioni seguenti.

   Per regolare l’intervallo di date, vedi [Modificare il filtro dell’intervallo di date](#change-the-date-range-filter).

## Rimuovere un filtro

Puoi rimuovere un filtro in qualsiasi momento. Se rimuovi un filtro, questo non viene visualizzato alla successiva visita dell’area Analisi avanzata.

>[!TIP]
>
>È inoltre possibile utilizzare i tasti della tastiera per individuare e rimuovere un filtro esistente.\
>Per ulteriori informazioni, consulta la sezione [Scelte rapide da tastiera](../enhanced-analytics/enhanced-analytics-overview.md#keyboard) sezione dell&#39;articolo [Panoramica dell’analisi migliorata](../enhanced-analytics/enhanced-analytics-overview.md).

Per rimuovere un filtro:

1. Fai clic sull’icona Menu principale ![](assets/main-menu-icon-16x12.png), quindi seleziona **Analytics**.
1. Se desideri rimuovere un filtro Lavoro, resta nella **Lavoro** area.

   Oppure

   Per rimuovere un filtro Persone, seleziona **Persone** nel pannello a sinistra.

1. Individua il filtro desiderato e fai clic su **X** per rimuoverlo.

   ![](assets/remove-filter-350x213.png)

   Il filtro non è più attivo e non viene visualizzato a meno che non lo si aggiunga di nuovo.
