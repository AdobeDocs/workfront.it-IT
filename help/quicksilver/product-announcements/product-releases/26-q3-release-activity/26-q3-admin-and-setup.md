---
title: Miglioramenti per gli amministratori del terzo trimestre 2026
description: Miglioramenti per gli amministratori del terzo trimestre 2026
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: d83d823426b42202e83cb4db64f85d27d4dca0bb
workflow-type: tm+mt
source-wordcount: '857'
ht-degree: 8%

---

# Miglioramenti per gli amministratori del terzo trimestre 2026

Questa pagina descrive i miglioramenti per gli amministratori apportati con la versione del terzo trimestre 2026 all’ambiente di anteprima. Tali miglioramenti saranno resi disponibili nell’ambiente di produzione come indicato.

Per un elenco di tutte le modifiche disponibili al momento nel ciclo di rilascio del terzo trimestre 2026, consulta [Panoramica sulla versione del terzo trimestre 2026](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-release-overview.md).

## Rilevamento delle modifiche per revisione e approvazione unificate

>[!NOTE]
>
>Anteprima: 7 luglio 2026Versione rapida di produzione: 15 luglio 2026Produzione per tutti: 16 luglio 2026

La pagina Cronologia modifiche in Workfront ora acquisisce l’attività tra i flussi di lavoro unificati di revisione e approvazione, fornendo agli amministratori un percorso di governance completo per la revisione e la documentazione degli eventi del ciclo di vita.

Ora vengono tracciate le azioni di approvazione, staging e partecipante. Tali azioni possono includere:

* Come prendere una decisione di approvazione nel visualizzatore Frame.io
* Creazione o eliminazione di un’approvazione
* Aggiornare un documento, ad esempio rinominarlo, spostarlo o eliminarlo

Ogni voce include i campi tracciati standard: data e ora, operazione, nome utente (o &quot;generato dal sistema&quot;) e nome oggetto. I commenti del visualizzatore Frame.io non sono inclusi.

Questa fase del rilevamento delle modifiche non include gli eventi MCP. Questi elementi faranno parte di una versione futura.

Per ulteriori informazioni, vedere [Visualizzare e gestire la cronologia modifiche](/help/quicksilver/administration-and-setup/manage-enterprise-operations/view-and-manage-change-history.md).

<!--

## Internal lookup field replacing Typeahead field type

>[!NOTE]
>
>Preview: July 7, 2026
>Production fast release: July 15, 2026
>Production for everyone: July 16, 2026

The new **Internal lookup** field type in custom forms provides dynamic filtering. It is similar to the Typeahead field type and allows users to search and select existing Workfront objects by typing part of the name. The filter on the internal lookup can reference the value in another field on the form, which is not possible with Typeaheads.

Multi-select is supported on internal lookups, and this field type also provides improved performance for large datasets. The following native Workfront objects are supported in internal lookups: Project, Company, Group, Job Role, Portfolio, Program, Team, Template, User, Task, Issue, Document, and Location.

The Internal lookup field type is replacing the Typeahead field type. You can quickly convert existing Typeahead fields to Internal lookups by clicking the button in the field options on the right. When you convert, historical data remains on the field and it is used the same way in reports.

>[!IMPORTANT]
>
>External integrations such as Workfront Fusion scenarios or API-based automations may reference legacy field structures and require updates after the conversion. You should verify any integrations before converting Typeahead fields to Internal lookup fields.

For more information, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

-->

<!--

## Default value logic supported on native reference fields

>[!NOTE]
>
>Preview: July 7, 2026
>Production fast release: July 15, 2026
>Production for everyone: July 16, 2026
>
>This feature is only available for organizations on the Workflow Prime or Ultimate packages.

In custom forms, native reference fields now allow you to add default value logic.

This logic type on native reference fields is available only in the user interface and not in the Workfront API.

For information, see [Add default value logic to a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md#add-default-value-logic-to-a-custom-form) in the article [Add logic rules to custom forms and fields](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md).

-->

<!--

## Updates to native field filtering in custom forms

>[!NOTE]
>
>Preview: July 7, 2026
>Production fast release: July 15, 2026
>Production for everyone: July 16, 2026

System filters that exist on native fields are now applied to the fields in custom forms and are visible to administrators.

When you add a native reference field that has a system filter applied, you can apply the same filter to the field in the custom form and modify the filter if needed in the Text Mode box.

Adding your own custom filter to the field overrides the system filter for the field. If you do not enter a custom filter, the system filter is applied by default.

Also, dynamic filtering is now available on native reference fields. A dynamic filter allows you to narrow the list of items based on the value of another field.

For example, when you use `?portfolioID={portfolio}.{ID}` in a Project field filter and a Portfolio native field is on the custom form, the Project field shows only projects that are in the selected portfolio. If the Portfolio field is left blank, then all projects are available in the Project field.

For information, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

-->

<!--

## Protect field names from accidental renaming

>[!NOTE]
>
>Preview: July 7, 2026
>Production fast release: July 15, 2026
>Production for everyone: July 16, 2026

To protect integrations and data integrity, we've updated how field names can be edited in the field settings panel of a custom form.

Field names in the field settings panel are now read-only by default. You can still edit the field name, but renaming requires an explicit confirmation step. The field previously called **Name** has also been updated to **API Name** to better reflect its technical significance. The **Label** field remains editable.

For information, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#notes-on-field-names-and-labels).

-->

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
>Anteprima: 11 giugno 2026Produzione per tutti: 11 giugno 2026

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
