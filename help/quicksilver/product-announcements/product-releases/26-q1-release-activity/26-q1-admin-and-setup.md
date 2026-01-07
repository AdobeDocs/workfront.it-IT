---
title: Miglioramenti per gli amministratori del primo trimestre 2026
description: Miglioramenti per gli amministratori del primo trimestre 2026
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: a49c8f2ad345f0ea8cdfd38ad79c6c0a5f636e95
workflow-type: tm+mt
source-wordcount: '676'
ht-degree: 0%

---

# Miglioramenti per gli amministratori del primo trimestre 2026

Questa pagina descrive i miglioramenti per gli amministratori apportati con la versione del primo trimestre 2026 all’ambiente di anteprima. Questi miglioramenti saranno resi disponibili nell’ambiente di produzione come indicato.

Per un elenco di tutte le modifiche disponibili al momento nel ciclo di rilascio del primo trimestre 2026, consulta [Panoramica sulla versione del primo trimestre 2026](/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-release-overview.md).

## Gestire le priorità nel modello di layout

>[!NOTE]
>
>Anteprima: 2 dicembre 2025
>Versione rapida di produzione: 14 gennaio 2026
>Produzione per tutti: 15 gennaio 2026

È ora possibile abilitare o disabilitare Priorità per utenti specifici nel modello di layout. Se in precedenza Priorità era disabilitata per la tua organizzazione, con questa modifica questa resterà disabilitata nel modello di layout.

Le priorità verranno incluse automaticamente per i tipi di licenza con accesso predefinito alle richieste. Ad esempio, una licenza Collaboratore visualizzerà Richieste, Bacheche e Priorità per impostazione predefinita nel Menu principale, mentre una licenza Esterna visualizzerà solo Documenti e Bacheche perché non ha accesso alla visualizzazione o all’invio di richieste.


Per ulteriori informazioni, vedere [Personalizzare il menu principale utilizzando un modello di layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).

## Verifica la presenza di conflitti tra più moduli per i campi personalizzati calcolati

>[!NOTE]
>
>Anteprima: 18 dicembre 2025
>Versione rapida di produzione: 14 gennaio 2026
>Produzione per tutti: 15 gennaio 2026

Lo stesso campo calcolato può avere formule diverse se associato a moduli personalizzati diversi. Se a un oggetto sono allegati due o più moduli contenenti lo stesso campo calcolato, le formule devono essere identiche in tutti i moduli. La modifica della formula non è consentita se la modifica potrebbe causare un conflitto.

Per fornire visibilità sugli oggetti che potrebbero essere interessati dalla modifica di un’espressione su campi personalizzati, è stata aggiunta un’opzione per verificare la presenza di conflitti. Questa finestra di dialogo mostra tutti gli oggetti che potrebbero essere interessati dalla modifica della formula, raggruppati per tipo di oggetto. È possibile passare ai dettagli di ogni oggetto ed esaminare i campi per decidere se il campo deve essere rimosso da uno dei moduli o se l&#39;espressione deve rimanere invariata.

Per ulteriori informazioni, vedere [Aggiungere campi calcolati a un modulo](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).


## Data di immissione e ID Inserito da archiviati in oggetti personalizzati

>[!NOTE]
>
>Anteprima: 13 novembre 2025
>Versione rapida di produzione: 13 novembre 2025
>Produzione per tutti: 13 novembre 2025

La data di immissione e l’ID immessi vengono ora memorizzati in moduli personalizzati, campi e sezioni. Puoi utilizzare queste opzioni dati nei rapporti come filtri, viste o raggruppamenti. Per visualizzarli nell&#39;elenco di moduli, campi o sezioni personalizzati in Configurazione, aggiungere Data immissione e Nome immesso come colonne in una visualizzazione nuova o esistente.

>[!NOTE]
>
>La data di immissione e immessa per ID sono disponibili solo per i moduli personalizzati, i campi e le sezioni creati il 13 novembre 2025 o dopo tale data.

## Aggiornamenti ai nomi dei pulsanti durante la modifica di un modello di layout

>[!NOTE]
>
>Anteprima: 30 ottobre 2025
>Versione rapida di produzione: 13 novembre 2025
>Produzione per tutti: 15 gennaio 2026

Per garantire maggiore coerenza con altre aree del programma di installazione, ad esempio il progettista di moduli personalizzati, i pulsanti visualizzati durante la modifica di un modello di layout sono stati modificati in **Applica**, **Salva e chiudi** e **Annulla**. La nuova opzione **Applica** consente di salvare le modifiche apportate al modello di layout e continuare a modificarle. In precedenza, le opzioni disponibili erano **Salva** e **Annulla**.

Per ulteriori informazioni, vedere [Creare e gestire modelli di layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

## Gestione dei campi migliorata con il flag Attivo sui campi personalizzati

>[!NOTE]
>
>Anteprima: 30 ottobre 2025
>Versione rapida di produzione: 13 novembre 2025
>Produzione per tutti: 15 gennaio 2026

Quando nel sistema sono presenti numerosi campi personalizzati, la gestione di tali campi nei moduli e nei report personalizzati può essere difficile. Ora puoi contrassegnare i campi personalizzati come inattivi con il nuovo flag **Attivo**. Questo flag è disponibile quando si lavora con un campo in un modulo personalizzato o quando si aggiunge o si modifica un campo dall&#39;elenco Campi.

Se un campo viene contrassegnato come inattivo:

* È escluso da rapporti, filtri, viste o altre posizioni in Workfront in cui puoi aggiungere un campo personalizzato
* Non è disponibile nella libreria dei campi da aggiungere ad altri moduli personalizzati

>[!NOTE]
>
>L’esclusione da rapporti, filtri, viste e raggruppamenti avviene dopo che il campo è diventato inattivo. Gli elementi del rapporto esistenti che utilizzano il campo non vengono modificati o rimossi quando il campo è contrassegnato come inattivo.

Per ulteriori informazioni, vedere [Creare un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).




