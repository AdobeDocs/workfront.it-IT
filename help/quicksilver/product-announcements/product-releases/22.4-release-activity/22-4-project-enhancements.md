---
title: 22.4 Miglioramenti al progetto
description: 22.4 Miglioramenti al progetto
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 41372dd8-5002-4f8b-a5ac-a577c8b05d11
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '965'
ht-degree: 2%

---

# 22.4 Miglioramenti al progetto

Questa pagina descrive tutti i miglioramenti apportati all’ambiente di anteprima con la versione 22.4 di Project. Questi miglioramenti saranno resi disponibili la settimana del 3 ottobre 2022.

Per un elenco di tutte le modifiche disponibili con la versione 22.4, consulta [Panoramica sulla versione 22.4](/help/quicksilver/product-announcements/product-releases/22.4-release-activity/22-4-release-overview.md).

## Sono ora disponibili i dettagli del predecessore

Per visualizzare i dettagli dei predecessori di un&#39;attività, è ora possibile passare il cursore sul numero del predecessore nella colonna Predecessori. Nella casella dei dettagli vengono visualizzati l&#39;attività e il progetto predecessore a cui si fa riferimento, le date di inizio e fine pianificate per l&#39;attività predecessore e il numero di predecessori e successori dell&#39;attività predecessore. Puoi espandere i dettagli del progetto per visualizzare ulteriori informazioni. Sono incluse ulteriori informazioni per i predecessori tra progetti.

Per ulteriori informazioni, consulta [Creare una relazione predecessore nell&#39;elenco delle attività](/help/quicksilver/manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).

## Assegnare più team a un’attività o a un problema

Per offrire una maggiore flessibilità nella gestione di attività e problemi, è possibile assegnare più team a un’attività o a un problema. In precedenza, era possibile assegnare un solo team a un’attività o a un problema.

>[!NOTE]
>
>Questa funzionalità non è attualmente disponibile nel Bilanciatore dei carichi di lavoro nell’area Team.

Per ulteriori informazioni, consulta [Assegna attività](/help/quicksilver/manage-work/tasks/assign-tasks/assign-tasks.md) e [Assegna problemi](/help/quicksilver/manage-work/issues/manage-issues/assign-issues.md).

## Selezione intelligente degli utenti per i ruoli di progetto nelle aree Modifica e Dettagli

È stato migliorato il modo in cui gli utenti vengono visualizzati quando vengono aggiunti ai seguenti campi del progetto dalla casella Modifica e dalla sezione Dettagli del progetto:

* Proprietario progetto

* Sponsor del progetto

* Responsabile risorse

Ora, quando si aggiunge un utente a uno di questi campi nelle aree Modifica o Dettagli, oltre al nome e all’avatar, vengono visualizzati anche il Ruolo principale e l’e-mail. Questo aiuta a distinguere tra più utenti con nomi simili o identici.

Per ulteriori informazioni, consulta [Modifica Progetti](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md).

NOTA: ulteriori campi utente per progetti, attività e problemi saranno aggiornati con questa funzionalità nelle versioni future.

[Visualizza una dimostrazione video di questa funzione.](https://video.tv.adobe.com/v/3412390/){target=_blank}

## I campi data calcolati vengono sempre salvati in base al Coordinated Universal Time (UTC)

Ora puoi essere sicuro che tutte le funzioni data nei campi calcolati funzionino in modo coerente e producano lo stesso risultato per tutti, indipendentemente da come un’espressione di dati personalizzata viene aggiornata o da dove gli utenti collaborano all’oggetto in tutto il mondo.

Tutti i calcoli vengono ora calcolati e salvati in base a un unico standard, il Coordinated Universal Time (UTC), e non in base alle configurazioni del fuso orario impostate per l’istanza della tua organizzazione e per il tuo profilo utente individuale. Tuttavia, i calcoli vengono visualizzati in un modulo personalizzato basato sui singoli fusi orari impostati dagli utenti nel browser.

In precedenza, le impostazioni di tempo nei calcoli causavano confusione quando variavano in queste situazioni:

* Se qualcuno ha ricalcolato un’espressione di campo calcolato utilizzando &quot;Aggiorna calcoli precedenti&quot; nel generatore di moduli, i risultati della funzione data sono determinati dal fuso orario UTC della tua organizzazione.

* Se qualcuno ha modificato l’oggetto e questo ha causato il ricalcolo dell’espressione del campo calcolato, i risultati della funzione data sono determinati dal fuso orario locale dell’utente. I risultati del campo data calcolata in questo scenario verranno calcolati anche in base all’UTC.

Per ulteriori informazioni, consulta [Utilizzo dei fusi orari](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).

## Miglioramenti al modulo personalizzato: Adobe XD e il filtro rapido

In base al tuo feedback, abbiamo introdotto i seguenti miglioramenti per migliorare la tua esperienza nella gestione dei moduli personalizzati:

* Aggiungi un file Adobe XD per rendere un modulo personalizzato più visivo e informativo. Quando il modulo viene allegato a un oggetto, gli utenti che utilizzano l&#39;oggetto possono visualizzare e interagire con il file XD dall&#39;interno del modulo.

  Per ulteriori informazioni, consulta [Aggiungere o modificare un’immagine o un altro widget di risorse in un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

* Utilizza il filtro rapido per individuare facilmente gli elementi nell’elenco dei campi e dei moduli personalizzati modernizzati. Inoltre, è possibile ottenere un aspetto migliore durante la gestione di moduli e campi.

  Per ulteriori informazioni sul filtro rapido, consulta [Applicare il filtro rapido a un elenco](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md).

[Visualizza una dimostrazione video di questa funzione.](https://video.tv.adobe.com/v/3412469/){target=_blank}

## Beta pubblica: nuova esperienza di filtro per progetti, attività e problemi

I filtri negli elenchi di progetti, attività e problemi sono stati riprogettati per aiutarti a creare e condividere rapidamente i filtri. Le caratteristiche includono:

* Interfaccia &quot;beta builder&quot; intuitiva per la creazione di un nuovo filtro

* Possibilità di contrassegnare un filtro come preferito

* Stacking dei filtri (applicazione di più filtri salvati)

* Duplicazione dei filtri

* Condivisione di filtri

* Rimozione dei filtri condivisi con te


La nuova esperienza di filtro è disponibile anche negli elenchi delle schede orario e nella Pianificazione scenario.

La modalità testo rimane disponibile per la modifica avanzata dei filtri e gli amministratori di sistema possono ancora assegnare filtri predefiniti a tutti gli utenti tramite i modelli di layout.

### Dove sarà disponibile?

* Elenchi progetti/attività/problemi

* Pianificazione scenario

* Schede orario


### Vogliamo il tuo feedback!

Con questa versione beta pubblica, gli utenti hanno la possibilità di inviare feedback direttamente al team che lavora sull’esperienza dei filtri, facendo clic sul pulsante di feedback. Saremo lieti di ricevere informazioni da te e dai tuoi utenti sulla nuova esperienza di filtro nella versione beta pubblica. Se il tuo team desidera incontrare direttamente il prodotto per fornire un feedback, pianifica un incontro qui: https://calendly.com/wf-product-and-design-research/filtersfeedbackpublicbeta?month=2022-08&amp;date=2022-08-25

### Cosa succede dopo?

* Nuova esperienza con raggruppamenti e visualizzazioni (nota anche come colonne)

  Inizieremo a lavorare sulla nuova esperienza per i raggruppamenti e le visualizzazioni (nota anche come colonne) in modo che sia coerente con la nuova esperienza dei filtri e abbia alcune delle stesse funzionalità della nuova esperienza dei filtri.

* Implementare nuovi filtri in altre aree di Adobe Workfront

  Lavoreremo con i team in tutto il prodotto per implementare la nuova esperienza di filtri in altre aree in Workfront.


Desideriamo fornire valore iterativo, in modo da continuare a fornire man mano che le nuove esperienze e altre aree sono pronte. Rimani sintonizzato per aggiornamenti più interessanti.

Per ulteriori informazioni, consulta [Panoramica sui filtri](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md) e [Creare o modificare filtri in Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

[Visualizza una dimostrazione video di questa funzione.](https://video.tv.adobe.com/v/3412391/)
