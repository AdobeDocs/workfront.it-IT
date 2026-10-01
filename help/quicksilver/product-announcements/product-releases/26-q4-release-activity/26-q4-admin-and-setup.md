---
title: Miglioramenti per gli amministratori del quarto trimestre 2026
description: Miglioramenti per gli amministratori del quarto trimestre 2026
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: a29813d3-f0cc-4b60-9396-13b558370803
    internal-label: Product announcements
source-git-commit: 6fb8df06a03ba2189c16585ffb2844f484f4ca1d
workflow-type: tm+mt
source-wordcount: '1666'
ht-degree: 1%
---
# Miglioramenti per gli amministratori del quarto trimestre 2026

Questa pagina descrive i miglioramenti per gli amministratori apportati con la versione del quarto trimestre 2026 all’ambiente di anteprima. Tali miglioramenti saranno resi disponibili nell’ambiente di produzione come indicato.

Per un elenco di tutte le modifiche disponibili a questo punto del ciclo di rilascio del quarto trimestre 2026, consulta [Panoramica sulla versione del quarto trimestre 2026](/help/quicksilver/product-announcements/product-releases/26-q4-release-activity/26-q4-release-overview.md).

## Utilizza l’intelligenza artificiale per generare la localizzazione personalizzata

>[!NOTE]
>
>Anteprima: 1 ottobre 2026
>Versione rapida di produzione: 14 ottobre 2026
>Produzione per tutti: 15 ottobre 2026

Per risparmiare tempo nella traduzione di termini ed etichette di campo personalizzati, è stata aggiunta la possibilità di generare traduzioni AI per la localizzazione personalizzata. Ora, gli amministratori di Workfront possono utilizzare l’intelligenza artificiale per generare traduzioni per testo personalizzato non tradotto o compilare traduzioni aggiuntive per un termine localizzato in precedenza, quindi rivedere e regolare i risultati prima di salvare.

Per ulteriori informazioni, vedere [Configurare la localizzazione personalizzata](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-custom-localization.md).

<!--

## Grant access to MCP Tools

>[!NOTE]
>
>Preview: October 1, 2026
>Production fast release: October 14, 2026
>Production for everyone: October 15, 2026

To make it easier to control secure access to Workfront data, we've added the ability for administrators to configure MCP Tools permissions by access level. Now, you can configure actions a given access level can take through the Workfront MCP.

* No access
* Read
* Create
* Update / Delete

You can edit this access when editing a specific access level, or edit access to MCP tools for multiple access levels at once.

For more information, see [Grant access to MCP Tools](help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-mcp-tools.md).

-->

## Miglioramenti ai modelli di layout

>[!NOTE]
>
>Anteprima: 1 ottobre 2026
>Versione rapida di produzione: 14 ottobre 2026
>Produzione per tutti: 15 ottobre 2026

Sono stati apportati diversi miglioramenti ai modelli di layout:

* Gli amministratori di sistema e di gruppo possono ora scegliere di nascondere o visualizzare gli elementi di sistema nel menu principale, all’interno del modello di layout. Gli elementi di sistema includono i pulsanti Configurazione e Guida.
* È ora possibile riposizionare le applicazioni personalizzate in qualsiasi ordine con le opzioni di menu predefinite di Workfront. Ciò consente di posizionare ogni applicazione nella posizione più appropriata. In precedenza, le applicazioni personalizzate erano sempre gli ultimi elementi nelle opzioni del menu principale del modello di layout e non potevano essere riposizionate.
* È ora possibile nascondere la pagina Dettagli di un oggetto dal pannello di navigazione a sinistra. Un oggetto deve avere almeno un elemento visualizzato nel pannello a sinistra. Se tutti gli altri elementi sono nascosti, non è possibile nascondere l&#39;ultimo elemento rimanente.

Per ulteriori informazioni, vedere [Personalizzare il menu principale utilizzando un modello di layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md) e[Personalizzare il pannello sinistro utilizzando un modello di layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md).

## Esperienza migliorata per l’aggiornamento delle scelte dei campi nel designer di moduli personalizzati

>[!NOTE]
>
>Anteprima: 1 ottobre 2026
>Versione rapida di produzione: 14 ottobre 2026
>Produzione per tutti: 15 ottobre 2026

Quando si utilizzano campi a discesa, pulsanti di scelta e caselle di controllo in Progettazione moduli, è ora possibile aggiungere, modificare ed eliminare le scelte dei campi in un&#39;unica finestra di dialogo. In precedenza, si aggiungevano e modificavano le scelte nel pannello di destra della finestra di progettazione e non c&#39;era molto spazio se si creava un lungo elenco di scelte.

Per informazioni, vedere [Creare un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-radio-buttons-checkbox-groups-and-drop-downs).

## Creare e gestire le sottoscrizioni di eventi all’interno dell’interfaccia di Workfront

Per semplificare la creazione e la gestione degli abbonamenti agli eventi dell’organizzazione, è stata aggiunta l’area Iscrizioni agli eventi a Configurazione. Ora è possibile:

* Visualizza un elenco di sottoscrizioni di eventi esistenti:
* Crea nuove sottoscrizioni di eventi, incluso il filtro in base ai criteri specificati:
* Elimina sottoscrizioni eventi.

<!--ADD LINK WHEN READY-->


## Aggiungere URL di reindirizzamento autorizzati per le integrazioni MCP

>[!NOTE]
>
>Anteprima: 22 settembre 2026
>Versione rapida di produzione: 14 ottobre 2026
>Produzione per tutti: 15 ottobre 2026

Per rendere i server Workfront MCP più flessibili e personalizzabili per la tua organizzazione, abbiamo aggiunto la possibilità di aggiungere URL di callback OAuth personalizzati. Gli amministratori di Workfront ora possono mantenere il inserisco nell&#39;elenco Consentiti di callback degli URL OAuth affidabili per le integrazioni MCP gestito dalla propria organizzazione. Questo consente di connettere piattaforme basate su AI personalizzate il cui URL di callback OAuth è univoco per la tua organizzazione, oltre alle piattaforme supportate in modo nativo da Workfront.

Per ulteriori informazioni, vedere [Aggiungere o rimuovere un URL di reindirizzamento autorizzato](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md#add-or-remove-an-authorized-redirect-url) in [Configurare le preferenze di sistema](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

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

## Imposta un livello di accesso predefinito per gli utenti con provisioning in Adobe Admin Console

>[!NOTE]
>
>Anteprima: 3 settembre 2026
>Versione rapida di produzione: 17 settembre 2026
>Produzione per tutti: 15 ottobre 2026

Ora puoi impostare un livello di accesso predefinito per gli utenti che dispongono del provisioning in Workfront tramite Adobe Admin Console. Un amministratore di Workfront può configurare questa impostazione predefinita in Preferenze di sistema.

In precedenza, Workfront assegnava all’utente un livello di accesso Collaboratore o Richiedente.

Per ulteriori informazioni, vedere [Configurare le preferenze di sistema](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

## Settimane personalizzate in aggiunta ai trimestri personalizzati per i clienti Workfront Planning

>[!NOTE]
>
>Anteprima: 3 settembre 2026
>Versione rapida di produzione: 17 settembre 2026
>Produzione per tutti: 15 ottobre 2026

Se la tua organizzazione ha acquistato un pacchetto Planning, oltre a un pacchetto Flusso di lavoro, ora puoi configurare le settimane personalizzate nello stesso modo in cui configuri i trimestri personalizzati come amministratore Workfront.

Le settimane personalizzate non sono visibili in Workfront. Sono visibili solo nella vista timeline di Workfront Planning.

Per informazioni, vedere [Abilitare i trimestri personalizzati](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md).

## Supporto di file di grandi dimensioni per le integrazioni di documenti personalizzati

>[!NOTE]
>
>Anteprima: 3 settembre 2026
>Versione rapida di produzione: 17 settembre 2026
>Produzione per tutti: 15 ottobre 2026

Le integrazioni personalizzate dei documenti ora supportano i caricamenti a blocchi per i file di grandi dimensioni. Se questa opzione è abilitata, i file di dimensioni superiori a 25 MB vengono suddivisi in blocchi più piccoli e caricati in parallelo, rendendo i caricamenti di file di grandi dimensioni più veloci e affidabili. Gli amministratori possono attivarlo e impostare la dimensione massima del blocco (fino a 100 MB) per integrazione.

Per ulteriori informazioni, consulta [Configura integrazioni di documenti](/help/quicksilver/administration-and-setup/configure-integrations/configure-document-integrations.md).

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


