---
title: Miglioramenti per gli amministratori del terzo trimestre 2026
description: Miglioramenti per gli amministratori del terzo trimestre 2026
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: f45c946e48b253018648c414915d53eca5a4de80
workflow-type: tm+mt
source-wordcount: '1334'
ht-degree: 5%

---

# Miglioramenti per gli amministratori del terzo trimestre 2026

Questa pagina descrive i miglioramenti per gli amministratori apportati con la versione del terzo trimestre 2026 all’ambiente di anteprima. Tali miglioramenti saranno resi disponibili nell’ambiente di produzione come indicato.

Per un elenco di tutte le modifiche disponibili al momento nel ciclo di rilascio del terzo trimestre 2026, consulta [Panoramica sulla versione del terzo trimestre 2026](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-release-overview.md).

<!--

## Change tracking for unified review and approval

>[!NOTE]
>
>Preview: July 7, 2026
>Production fast release: July 15, 2026
>Production for everyone: July 16, 2026

The Change History page in Workfront now captures activity across unified review and approval workflows, giving administrators a complete governance trail for review and document lifecycle events.

Approval, stage, and participant actions are now tracked. These actions may include:

* Making an approval decision in the Frame.io viewer
* Creating or deleting an approval
* Updating a document such as renaming, moving, or deleting it

Each entry includes the standard tracked fields: date and time, operation, user name (or "system generated"), and object name. Frame.io viewer comments are not included.

This phase of change tracking does not include MCP events. Those will be part of a future release.

For more information, see [View and manage change history](/help/quicksilver/administration-and-setup/manage-enterprise-operations/view-and-manage-change-history.md).

-->

## Campo di ricerca interno che sostituisce il tipo di campo automatico

>[!NOTE]
>
>Anteprima: 7 luglio 2026Versione rapida di produzione: 15 luglio 2026Produzione per tutti: 16 luglio 2026

Il nuovo tipo di campo **Ricerca interna** nei moduli personalizzati fornisce un filtro dinamico. È simile al tipo di campo Automatico e consente agli utenti di cercare e selezionare oggetti Workfront esistenti digitando parte del nome. Il filtro della ricerca interna può fare riferimento al valore in un altro campo del modulo, il che non è possibile con Typeaheads.

La selezione multipla è supportata nelle ricerche interne e questo tipo di campo offre anche prestazioni migliorate per set di dati di grandi dimensioni. Nelle ricerche interne sono supportati i seguenti oggetti Workfront nativi: Progetto, Società, Gruppo, Ruolo, Portfolio, Programma, Team, Modello, Utente, Attività, Problema, Documento e Posizione.

Il tipo di campo di ricerca interna sta sostituendo il tipo di campo Automatico. Puoi convertire rapidamente i campi Typeahead esistenti in ricerche interne facendo clic sul pulsante nelle opzioni di campo a destra. Quando esegui la conversione, i dati storici rimangono nel campo e vengono utilizzati allo stesso modo nei rapporti.

>[!IMPORTANT]
>
>Le integrazioni esterne, come scenari di Workfront Fusion o automazioni basate su API, possono fare riferimento a strutture di campo legacy e richiedere aggiornamenti dopo la conversione. Prima di convertire i campi Typeahead in campi di ricerca interni, è necessario verificare le integrazioni.

Per ulteriori informazioni, vedere [Creare un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Logica del valore predefinita supportata nei campi di riferimento nativi

>[!NOTE]
>
>Anteprima: 7 luglio 2026Versione rapida di produzione: 15 luglio 2026Produzione per tutti: 16 luglio 2026
>
>Questa funzione è disponibile solo per le organizzazioni nei pacchetti Workflow Prime o Ultimate.

Nei moduli personalizzati, i campi di riferimento nativi ora consentono di aggiungere la logica del valore predefinita.

Questo tipo di logica sui campi di riferimento nativi è disponibile solo nell’interfaccia utente e non nell’API Workfront.

Per informazioni, vedere [Aggiungere la logica del valore predefinito a un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md#add-default-value-logic-to-a-custom-form) nell&#39;articolo [Aggiungere regole di logica a moduli e campi personalizzati](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md).

## Aggiornamenti al filtro dei campi nativo nei moduli personalizzati

>[!NOTE]
>
>Anteprima: 7 luglio 2026Versione rapida di produzione: 15 luglio 2026Produzione per tutti: 16 luglio 2026

I filtri di sistema esistenti nei campi nativi vengono ora applicati ai campi nei moduli personalizzati e sono visibili agli amministratori.

Quando aggiungi un campo di riferimento nativo a cui è applicato un filtro di sistema, puoi applicare lo stesso filtro al campo nel modulo personalizzato e modificarlo, se necessario, nella casella Modalità testo.

L’aggiunta di un filtro personalizzato al campo sostituisce il filtro di sistema del campo. Se non si immette un filtro personalizzato, il filtro di sistema viene applicato per impostazione predefinita.

Inoltre, il filtro dinamico è ora disponibile sui campi di riferimento nativi. Un filtro dinamico consente di restringere l’elenco degli elementi in base al valore di un altro campo.

Se, ad esempio, si utilizza `?portfolioID={portfolio}.{ID}` in un filtro di campi di Project e un campo nativo di Portfolio si trova nel modulo personalizzato, nel campo Project vengono visualizzati solo i progetti inclusi nel portfolio selezionato. Se il campo Portfolio viene lasciato vuoto, tutti i progetti saranno disponibili nel campo Progetto.

Per informazioni, vedere [Creare un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Proteggere i nomi dei campi dalla ridenominazione accidentale

>[!NOTE]
>
>Anteprima: 7 luglio 2026Versione rapida di produzione: 15 luglio 2026Produzione per tutti: 16 luglio 2026

Per proteggere le integrazioni e l’integrità dei dati, è stato aggiornato il modo in cui i nomi dei campi possono essere modificati nel pannello delle impostazioni dei campi di un modulo personalizzato.

I nomi dei campi nel pannello delle impostazioni dei campi ora sono di sola lettura per impostazione predefinita. Puoi comunque modificare il nome del campo, ma la ridenominazione richiede un passaggio di conferma esplicito. Anche il campo precedentemente denominato **Name** è stato aggiornato a **API Name** per rispecchiare meglio il suo significato tecnico. Il campo **Label** rimane modificabile.

Per informazioni, vedere [Creare un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#notes-on-field-names-and-labels).

## Visualizzare la cronologia delle modifiche per gli oggetti Workfront

>[!NOTE]
>
>Anteprima: 11 giugno 2026Versione rapida di produzione: 11 giugno 2026Produzione per tutti: 16 luglio 2026

Per semplificare la visualizzazione delle modifiche apportate in un elenco centrale, è stato creato l&#39;elenco Cronologia modifiche. In questo elenco vengono visualizzate informazioni quali l&#39;oggetto, l&#39;operazione e l&#39;origine della modifica, ad esempio un utente o il sistema Workfront.

In precedenza, i registri di audit erano disponibili ma non coprivano gli oggetti.

Per ulteriori informazioni, vedere [Visualizzare e gestire la cronologia modifiche](/help/quicksilver/administration-and-setup/manage-enterprise-operations/view-and-manage-change-history.md).

## Nuova preferenza di sistema per convertire i portfolio di archiviazione legacy in archiviazione cloud Adobe

>[!NOTE]
>
>Anteprima: 11 giugno 2026Produzione per tutti: 11 giugno 2026Fuori pianificazione&rbrack;{type=Neutral}

Gli amministratori di Workfront ora possono convertire i portfolio di archiviazione legacy in archiviazione cloud Adobe direttamente da Preferenze di sistema. Per convertire i portfolio, selezionarli nel nuovo campo Seleziona i portfolio da convertire in storage aziendale e salvare la pagina.

Quando un portfolio viene convertito nell’archiviazione cloud Adobe:

* Non puoi più spostare in questo portfolio i progetti che utilizzano l’archiviazione precedente di Workfront
* Tutti i nuovi progetti creati in questo portfolio utilizzano l’archiviazione cloud Adobe
* Frame.io è il visualizzatore per i documenti che utilizzano l’archiviazione cloud Adobe
* Gli oggetti secondari che utilizzano lo storage legacy Workfront rimangono sullo storage legacy

In precedenza, l’aggiunta di un progetto di archiviazione cloud Adobe a un portfolio di archiviazione legacy convertiva automaticamente il portfolio in archiviazione cloud Adobe.

Per ulteriori informazioni, vedere [Configurare le preferenze di sistema](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

## Il formato Rich Text sostituisce il tipo di campo Testo con formattazione

>[!NOTE]
>
>Anteprima: 28 maggio 2026Versione rapida di produzione: 11 giugno 2026Produzione per tutti: 16 luglio 2026

Il nuovo tipo di campo **Rich text** nei moduli personalizzati è un editor di testo affidabile, con opzioni di formattazione quali apice e pedice, intestazioni e tabelle, oltre alle opzioni tradizionali di grassetto, corsivo, sottolineatura, punti elenco, numerazione, collegamenti ipertestuali e virgolette. Il limite di caratteri rimane 15.000.

Il tipo di campo Rich text sostituisce il tipo di campo Testo con formattazione. Per convertire rapidamente in testo formattato il testo esistente, fai clic sul pulsante nelle opzioni di campo a destra. Quando esegui la conversione, i dati storici rimangono nel campo e vengono utilizzati allo stesso modo nei rapporti.

>[!IMPORTANT]
>
>Le integrazioni esterne, come scenari di Workfront Fusion o automazioni basate su API, possono fare riferimento a strutture di campo legacy e richiedere aggiornamenti dopo la conversione. Prima di convertire i campi in testo formattato, è necessario verificare le integrazioni.

Per ulteriori informazioni, vedere [Creare un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Campi finanziari nativi supportati nei moduli personalizzati

>[!NOTE]
>
>Anteprima: 28 maggio 2026Versione rapida di produzione: 11 giugno 2026Produzione per tutti: 16 luglio 2026

Ora puoi includere i campi finanziari nativi di Workfront nei moduli personalizzati. In precedenza, i campi finanziari non erano supportati.

I campi finanziari disponibili a cui è possibile fare riferimento dipendono dal tipo di modulo.

Per ulteriori informazioni, vedere [Creare un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-workfront-native-fields).

## I moduli personalizzati possono essere condivisi a livello di sistema con autorizzazione ad allegare

>[!NOTE]
>
>Anteprima: 28 maggio 2026Versione rapida di produzione: 11 giugno 2026Produzione per tutti: 16 luglio 2026

Ai moduli personalizzati è stata aggiunta la nuova opzione di condivisione &quot;Tutti nel sistema possono visualizzare e allegare&quot;. Quando si seleziona questa opzione, tutti gli utenti a livello di sistema possono allegare il modulo ad altri oggetti.

La condivisione a livello di sistema elimina la necessità di condividere manualmente i moduli e di aggiornare le autorizzazioni tra gruppi o agenzie quando vengono aggiunti nuovi gruppi.

Per ulteriori informazioni, vedere [Condividi modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).

## Nuova preferenza di sistema per applicare i campi obbligatori durante la modifica in blocco

>[!NOTE]
>
>Anteprima: 28 maggio 2026Versione rapida di produzione: 11 giugno 2026Produzione per tutti: 16 luglio 2026

Attualmente, quando si modificano oggetti in blocco, i campi obbligatori vengono applicati solo quando un utente modifica il campo. Se un campo non viene modificato, viene considerato facoltativo e non convalidato.

Una nuova preferenza di sistema ora consente di applicare i campi obbligatori nella modifica in blocco. Per non consentire il salvataggio di oggetti modificati in blocco a meno che tutti i campi obbligatori non contengano valori, selezionare l&#39;opzione **Applica sempre i campi obbligatori nella modifica in blocco** nella pagina Configurazione > Sistema > Preferenze.

Per ulteriori informazioni, vedere [Configurare le preferenze di sistema](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).
