---
title: 22.4 Miglioramenti al progetto
description: 22.4 Miglioramenti al progetto
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 41372dd8-5002-4f8b-a5ac-a577c8b05d11
source-git-commit: 6cd6b1433fb56b92872f0ad80bb1a700fc0854cc
workflow-type: tm+mt
source-wordcount: '967'
ht-degree: 2%

---

# 22.4 Miglioramenti al progetto

Questa pagina descrive tutti i miglioramenti apportati a Project con la versione 22.4 nell’ambiente di anteprima. Questi miglioramenti saranno resi disponibili la settimana del 3 ottobre 2022.

Per un elenco di tutte le modifiche disponibili con la versione 22.4, vedi [Panoramica sulla versione 22.4](/help/quicksilver/product-announcements/product-releases/22.4-release-activity/22-4-release-overview.md).

## Dettagli predecessore ora disponibili

Per visualizzare i dettagli dei predecessori di un&#39;attività, è ora possibile passare il cursore sul numero del predecessore nella colonna Predecessori. Nella casella Dettagli vengono visualizzate l&#39;attività predecessore e il progetto a cui si fa riferimento, le date di inizio e fine pianificate per l&#39;attività predecessore e il numero di predecessori e successori dell&#39;attività predecessore. Puoi espandere i dettagli del progetto per visualizzare ulteriori informazioni sul progetto. Sono incluse ulteriori informazioni per i predecessori tra progetti.

Per ulteriori informazioni, consulta [Creare una relazione predecessore nell&#39;elenco delle attività](/help/quicksilver/manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).

## Assegnare più team a un&#39;attività o a un problema

Per offrirti molta più flessibilità nella gestione di attività e problemi, abbiamo reso possibile assegnare più team a un’attività o a un problema. In precedenza, a un’attività o a un problema poteva essere assegnato un solo team.

>[!NOTE]
>
>Questa funzionalità non è attualmente disponibile nel servizio di bilanciamento del carico di lavoro nell’area Team.

Per ulteriori informazioni, consulta [Assegnare le attività](/help/quicksilver/manage-work/tasks/assign-tasks/assign-tasks.md) e [Assegnare i problemi](/help/quicksilver/manage-work/issues/manage-issues/assign-issues.md).

## Selezione avanzata di utenti per i ruoli di progetto nelle aree Modifica e Dettagli

È stato migliorato il modo in cui gli utenti vengono visualizzati quando li aggiungi ai seguenti campi del progetto dalla casella Modifica e dalla sezione Dettagli del progetto:

* Proprietario progetto

* Sponsor del progetto

* Responsabile risorse

Ora, quando aggiungi un utente a uno qualsiasi di questi campi nelle aree Modifica o Dettagli, oltre al nome e all’avatar, vengono visualizzati anche il relativo Ruolo principale e il relativo messaggio e-mail. Questo aiuta a distinguere tra più utenti con nomi simili o identici.

Per ulteriori informazioni, consulta [Modifica progetti](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md).

NOTA: Campi utente aggiuntivi per progetti, attività e problemi verranno aggiornati con questa funzionalità nelle versioni future.

[Guarda un video dimostrativo di questa funzione.](https://video.tv.adobe.com/v/3412390/){target=_blank}

## I campi data calcolati vengono sempre salvati in base all’ora universale coordinata (UTC)

Ora puoi essere sicuro che tutte le funzioni data nei campi calcolati funzionino in modo coerente e producano lo stesso risultato per tutti, indipendentemente da come viene aggiornata un’espressione dati personalizzata o da dove gli utenti collaborano all’oggetto in tutto il mondo.

Tutti i calcoli vengono ora calcolati e salvati da un unico standard (UTC, Coordinated Universal Time), non dalle configurazioni del fuso orario impostate per l&#39;istanza della tua organizzazione e il tuo profilo utente individuale. Tuttavia, i calcoli vengono visualizzati in un modulo personalizzato in base ai fusi orari dei singoli utenti impostati nel browser.

In precedenza, le impostazioni di tempo nei calcoli causavano confusione quando si verificavano variazioni in queste situazioni:

* Se un utente ha ricalcolato un&#39;espressione di campo calcolata utilizzando &quot;Aggiorna calcoli precedenti&quot; nel generatore di moduli, i risultati della funzione data sono stati determinati dal fuso orario UTC dell&#39;organizzazione.

* Se un utente ha modificato l’oggetto e questo ha causato il ricalcolo dell’espressione di campo calcolata, i risultati della funzione data sono stati determinati dal fuso orario locale dell’utente. Anche i risultati del campo data calcolato in questo scenario vengono calcolati in base all’UTC.

Per ulteriori informazioni, consulta [Utilizzo di fusi orari diversi](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).

## Miglioramenti al modulo personalizzato: Adobe XD e il filtro rapido

In base al tuo feedback, sono stati introdotti i seguenti miglioramenti per migliorare la tua esperienza nella gestione dei moduli personalizzati:

* Aggiungere un file Adobe XD per rendere un modulo personalizzato più visivo e informativo. Quando il modulo è associato a un oggetto, gli utenti che lavorano con esso possono visualizzare e interagire con il file XD all’interno del modulo.

   Per ulteriori informazioni, consulta [Aggiungere o modificare un’immagine o un altro widget di risorse in un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

* Utilizzare il filtro rapido per individuare facilmente gli elementi nell’elenco dei campi e dei moduli personalizzati modernizzati. Inoltre, è possibile migliorare l’aspetto visivo della gestione di moduli e campi.

   Per ulteriori informazioni sul filtro rapido, consulta [Applicare il filtro rapido a un elenco](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md).

[Guarda un video dimostrativo di questa funzione.](https://video.tv.adobe.com/v/3412469/){target=_blank}

## Beta pubblica: nuova esperienza di filtro per progetti, attività e problemi

L’applicazione di filtri agli elenchi di progetti, attività ed problemi è stata riprogettata per facilitare la creazione e la condivisione rapida di filtri. Le funzioni includono:

* Interfaccia intuitiva del &quot;generatore beta&quot; per la creazione di un nuovo filtro

* Possibilità di contrassegnare un filtro come preferito

* Stacking dei filtri (applicazione di più filtri salvati)

* Duplicazione dei filtri

* Condivisione di filtri

* Rimozione di filtri condivisi con te


La nuova esperienza di filtro è disponibile anche negli elenchi delle schede attività e nel Planner scenario.

La modalità testo rimane disponibile per la modifica avanzata dei filtri e gli amministratori di sistema possono ancora assegnare filtri predefiniti per tutti gli utenti tramite i modelli di layout.

### Dove sarà disponibile questo?

* Elenchi progetti/attività/problemi

* Pianificazione scenario

* Schede orario


### Vogliamo il tuo Feedback!

Con questa versione beta pubblica gli utenti hanno la possibilità di inviare feedback direttamente al team che lavora sull’esperienza dei filtri facendo clic sul pulsante di feedback. Non vediamo l’ora di sentire da te e dai tuoi utenti la nuova esperienza di filtro nella versione beta pubblica. Se il tuo team desidera incontrare direttamente il prodotto per fornire feedback aggiuntivi, puoi pianificare una riunione qui: https://calendly.com/wf-product-and-design-research/filtersfeedbackpublicbeta?month=2022-08&amp;date=2022-08-25

### Cosa succede dopo?

* Esperienza Nuovi gruppi e visualizzazioni (noti anche come Colonne)

   Inizieremo a lavorare alla nuova esperienza per raggruppamenti e viste (nota anche come colonne) in modo che sia coerente con la nuova esperienza di filtri e abbia alcune delle stesse grandi funzionalità della nuova esperienza di filtri.

* Implementare nuovi filtri in altre aree di Adobe Workfront

   Lavoreremo con i team di tutto il prodotto per implementare la nuova esperienza di filtro in altre aree in Workfront.


Vogliamo fornirti un valore iterativo, in modo da continuare a offrire man mano che le nuove esperienze e altre aree saranno pronte. Continuate a seguire gli aggiornamenti più interessanti.

Per ulteriori informazioni, consulta [Panoramica sui filtri in Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md) e [Creare o modificare filtri in Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

[Guarda un video dimostrativo di questa funzione.](https://video.tv.adobe.com/v/3412391/)
