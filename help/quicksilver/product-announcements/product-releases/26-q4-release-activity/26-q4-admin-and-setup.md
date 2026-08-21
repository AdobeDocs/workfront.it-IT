---
title: Miglioramenti per gli amministratori del quarto trimestre 2026
description: Miglioramenti per gli amministratori del quarto trimestre 2026
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: db296d9043cb793e1af74bca38197de682f54cb8
workflow-type: tm+mt
source-wordcount: '928'
ht-degree: 1%

---

# Miglioramenti per gli amministratori del quarto trimestre 2026

Questa pagina descrive i miglioramenti per gli amministratori apportati con la versione del quarto trimestre 2026 all’ambiente di anteprima. Tali miglioramenti saranno resi disponibili nell’ambiente di produzione come indicato.

Per un elenco di tutte le modifiche disponibili a questo punto del ciclo di rilascio del quarto trimestre 2026, consulta [Panoramica sulla versione del quarto trimestre 2026](/help/quicksilver/product-announcements/product-releases/26-q4-release-activity/26-q4-release-overview.md).

<!--

## Interface improvements to the Actions list

>[!NOTE]
>
>Preview: August 20, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

The Actions list in the Update Feeds section of the Setup area has an updated look and feel.

The following enhancements are included:

* We removed the Save and Cancel buttons.
* The Track column now appears in the last position.
* We removed the confirmation message that previously displayed when you saved changes in this area.

For information, see [Configure system updates](/help/quicksilver/administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

-->

## Gli amministratori di gruppi possono gestire i profili aziendali

>[!NOTE]
>
>Anteprima: 30 luglio 2026
>Versione rapida di produzione: 13 agosto 2026
>Produzione per tutti: 15 ottobre 2026

Gli amministratori dei gruppi ora possono creare, modificare ed eliminare i profili aziendali per i gruppi che amministrano, senza richiedere l’accesso come amministratore di sistema. Ciò offre alle organizzazioni maggiore flessibilità per delegare la gestione dei profili di business a livello di gruppo.

Per ulteriori informazioni, vedere [Visualizzare e gestire i profili aziendali](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/view-and-manage-business-profiles.md).

## Supporto dei modelli di layout per le visualizzazioni negli elenchi avanzati

>[!NOTE]
>
>Anteprima: 30 luglio 2026
>Versione rapida di produzione: 13 agosto 2026
>Produzione per tutti: 15 ottobre 2026

Le visualizzazioni per gli elenchi avanzati sono ora supportate a livello di sistema tramite un modello di layout. È possibile nascondere le viste di sistema esistenti, assegnare una vista specifica come vista predefinita e aggiungere una vista personalizzata all&#39;elenco delle viste di sistema.

Esempi di elenchi avanzati nel modello di layout sono **Tutte le richieste** e **Assegnazioni avanzate**. Un elenco avanzato presenta un’etichetta &quot;Nuova esperienza&quot; accanto alle visualizzazioni.

Per informazioni, vedere [Personalizzare filtri, visualizzazioni e raggruppamenti utilizzando un modello di layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

## Modifica in blocco dei campi di ricerca esterni

>[!NOTE]
>
>Anteprima: 30 luglio 2026
>Versione rapida di produzione: 13 agosto 2026
>Produzione per tutti: 15 ottobre 2026

Le finestre di dialogo per la modifica in blocco ora consentono di modificare i campi di ricerca esterni. In precedenza ciò non era possibile.

Nelle situazioni in cui un campo di ricerca dipende da un altro campo di ricerca, il campo con la dipendenza non può essere modificato in blocco a meno che il primo campo non sia lo stesso per tutti gli oggetti in fase di modifica.

Ad esempio, un elenco di paesi dipende dalla selezione effettuata per una regione. Se la regione per un progetto è Asia e la regione per un altro progetto è Europa e si modificano in blocco entrambi i progetti, il campo Paese non sarà disponibile perché le regioni non corrispondono. Se modifichi l’area geografica in modo che sia uguale per entrambi i progetti, puoi anche selezionare un paese da utilizzare in entrambi i progetti.

Per informazioni sui campi di ricerca esterni, vedere [Creare un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-external-lookup-fields).

## Logica avanzata supportata nell’anteprima di progettazione moduli personalizzati

>[!NOTE]
>
>Anteprima: 30 luglio 2026
>Versione rapida di produzione: 13 agosto 2026
>Produzione per tutti: 15 ottobre 2026

La modalità di anteprima di progettazione moduli personalizzata ora supporta opzioni di logica avanzate, tra cui logica di visualizzazione avanzata, logica dei valori predefinita, logica di convalida, logica di formattazione e logica di modificabilità. È possibile verificare le formule logiche nell&#39;anteprima del modulo e regolarle in base alle esigenze nel generatore di logica. È inoltre possibile selezionare un oggetto di test (progetto, attività, problema, ecc.) per visualizzare in anteprima il modulo con dati contestuali reali.

In precedenza, in modalità anteprima erano supportate solo le opzioni di base per la logica di visualizzazione e salto.

Tieni presente che questi tipi di logica sono disponibili solo per le organizzazioni nei pacchetti Workflow Prime o Ultimate: visualizzazione avanzata, valore predefinito, formattazione condizionale e modificabilità.

Per ulteriori informazioni, vedere [Aggiungere regole di logica ai moduli e ai campi personalizzati](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md) e [Organizzare e visualizzare in anteprima un modulo](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md).

## Rilevamento delle modifiche per revisione e approvazione unificate

>[!NOTE]
>
>Anteprima: 30 luglio 2026
>Versione rapida di produzione: 13 agosto 2026
>Produzione per tutti: 15 ottobre 2026

La pagina Cronologia modifiche in Workfront ora acquisisce l’attività tra i flussi di lavoro unificati di revisione e approvazione, fornendo agli amministratori un percorso di governance completo per la revisione e la documentazione degli eventi del ciclo di vita.

Ora vengono tracciate le azioni di approvazione, staging e partecipante. Tali azioni possono includere:

* Come prendere una decisione di approvazione nel visualizzatore Frame.io
* Creazione o eliminazione di un’approvazione
* Aggiornare un documento, ad esempio rinominarlo, spostarlo o eliminarlo

Ogni voce include i campi tracciati standard: data e ora, operazione, nome utente (o &quot;generato dal sistema&quot;) e nome oggetto. Vengono acquisite le attività MCP, tra cui LLM (come Claude) che ha effettuato l’aggiornamento. I commenti del visualizzatore Frame.io non sono inclusi.

Per ulteriori informazioni, vedere [Visualizzare e gestire la cronologia modifiche](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/view-and-manage-change-history.md).

## Definire un’applicazione personalizzata come pagina di destinazione nel modello di layout

>[!NOTE]
>
>Anteprima: 30 luglio 2026
>Versione rapida di produzione: 13 agosto 2026
>Produzione per tutti: 15 ottobre 2026

Ora è possibile impostare un’applicazione personalizzata come pagina di destinazione in un modello di layout. Le applicazioni personalizzate già aggiunte al menu principale sono disponibili per l’utilizzo come pagina di destinazione.

Le applicazioni personalizzate devono essere create separatamente prima di diventare disponibili come opzioni del menu principale o della pagina di destinazione.

Per ulteriori informazioni, vedere [Personalizzare la pagina di destinazione utilizzando un modello di layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-landing-page.md) e [Creare applicazioni personalizzate per Workfront con Adobe App Builder](/help/quicksilver/app-builder/app-builder.md).

## Configurare i campi tracciati nella cronologia delle modifiche

>[!NOTE]
>
>Anteprima: 30 luglio 2026
>Versione rapida di produzione: 13 agosto 2026
>Produzione per tutti: 15 ottobre 2026

È possibile aggiungere campi di cui tenere traccia per un particolare tipo di oggetto in Workfront. Quando gli utenti modificano le informazioni in tale campo, il sistema registra le informazioni sulla modifica come voce nella cronologia modifiche.

In precedenza, la schermata Configuration per la definizione dei campi tracciati era di sola visualizzazione.

Per ulteriori informazioni, vedere [Configurare i campi per tenere traccia della cronologia modifiche](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/configure-fields-in-change-history.md).

## Accesso amministrativo alla cronologia modifiche aggiunta ai livelli di accesso

>[!NOTE]
>
>Anteprima: 30 luglio 2026
>Versione rapida di produzione: 13 agosto 2026
>Produzione per tutti: 15 ottobre 2026

Nel livello di accesso Standard è ora possibile definire se gli utenti con tale livello devono avere accesso all&#39;elenco Cronologia modifiche. L&#39;opzione **Cambia cronologia** è disponibile nella sezione **Consenti accesso amministrativo per** nel livello di accesso.

Per ulteriori informazioni, vedere [Concedere agli utenti l&#39;accesso amministrativo ad alcune aree](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md) e [Visualizzare e gestire la cronologia modifiche](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/view-and-manage-change-history.md).


