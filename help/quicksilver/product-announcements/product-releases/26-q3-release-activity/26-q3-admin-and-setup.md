---
title: Miglioramenti per gli amministratori del terzo trimestre 2026
description: Miglioramenti per gli amministratori del terzo trimestre 2026
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 34ec779f648db8c3f1a1fe2a76f5b7fda83679a6
workflow-type: tm+mt
source-wordcount: '654'
ht-degree: 1%

---

# Miglioramenti per gli amministratori del terzo trimestre 2026

Questa pagina descrive i miglioramenti per gli amministratori apportati con la versione del terzo trimestre 2026 all’ambiente di anteprima. Tali miglioramenti saranno resi disponibili nell’ambiente di produzione come indicato.

Per un elenco di tutte le modifiche disponibili al momento nel ciclo di rilascio del terzo trimestre 2026, consulta [Panoramica sulla versione del terzo trimestre 2026](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-release-overview.md).

## Visualizzare la cronologia delle modifiche per gli oggetti Workfront

>[!NOTE]
>
>Anteprima: 11 giugno 2026>Versione rapida produzione: 11 giugno 2026>Produzione per tutti: 16 luglio 2026

Per semplificare la visualizzazione delle modifiche apportate in un elenco centrale, è stato creato l&#39;elenco Cronologia modifiche. In questo elenco vengono visualizzate informazioni quali l&#39;oggetto, l&#39;operazione e l&#39;origine della modifica, ad esempio un utente o il sistema Workfront.

In precedenza, i registri di audit erano disponibili ma non coprivano gli oggetti.

Per ulteriori informazioni, vedere [Visualizzare e gestire la cronologia modifiche](/help/quicksilver/administration-and-setup/manage-enterprise-operations/view-and-manage-change-history.md).

## Nuova preferenza di sistema per convertire i portfolio di archiviazione legacy in archiviazione cloud Adobe

>[!NOTE]
>
>Anteprima: 11 giugno 2026>Produzione per tutti: 11 giugno 2026

Gli amministratori di Workfront ora possono convertire i portfolio di archiviazione legacy in archiviazione cloud Adobe direttamente da Preferenze di sistema. Per convertire i portfolio, selezionarli nel nuovo campo Seleziona i portfolio da convertire in storage aziendale e salvare la pagina.

Quando un portfolio viene convertito nell’archiviazione cloud Adobe:

* Non è più possibile spostare in questo portfolio i progetti che utilizzano lo storage legacy Workfront
* Tutti i nuovi progetti creati in questo portfolio utilizzano l’archiviazione cloud Adobe
* Frame.io è il visualizzatore per i documenti che utilizzano l’archiviazione cloud Adobe
* Gli oggetti secondari che utilizzano lo storage legacy Workfront rimangono sullo storage legacy

In precedenza, l’aggiunta di un progetto di archiviazione cloud Adobe a un portfolio di archiviazione legacy convertiva automaticamente il portfolio in archiviazione cloud Adobe.

Per ulteriori informazioni, vedere [Configurare le preferenze di sistema](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

## Testo formattato sostituzione testo con tipo di campo Formattazione

>[!NOTE]
>
>Anteprima: 28 maggio 2026>Rilascio rapido produzione: 11 giugno 2026>Produzione per tutti: 16 luglio 2026

Il nuovo tipo di campo **Rich text** nei moduli personalizzati è un editor di testo affidabile, con opzioni di formattazione quali apice e pedice, intestazioni e tabelle, oltre alle opzioni tradizionali di grassetto, corsivo, sottolineatura, punti elenco, numerazione, collegamenti ipertestuali e virgolette. Il limite di caratteri rimane 15.000.

Il tipo di campo Rich text sostituisce il tipo di campo Testo con formattazione. Per convertire rapidamente in testo formattato il testo esistente, fai clic sul pulsante nelle opzioni di campo a destra. Quando esegui la conversione, i dati storici rimangono nel campo e vengono utilizzati allo stesso modo nei rapporti.

>[!IMPORTANT]
>
>Le integrazioni esterne, come scenari di Workfront Fusion o automazioni basate su API, possono fare riferimento a strutture di campo legacy e richiedere aggiornamenti dopo la conversione. Prima di convertire i campi in testo formattato, è necessario verificare le integrazioni.

Per ulteriori informazioni, vedere [Creare un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Campi finanziari nativi supportati nei moduli personalizzati

>[!NOTE]
>
>Anteprima: 28 maggio 2026>Rilascio rapido produzione: 11 giugno 2026>Produzione per tutti: 16 luglio 2026

Ora puoi includere i campi finanziari nativi di Workfront nei moduli personalizzati. In precedenza, i campi finanziari non erano supportati.

I campi finanziari disponibili a cui è possibile fare riferimento dipendono dal tipo di modulo.

Per ulteriori informazioni, vedere [Creare un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-workfront-native-fields).

## I moduli personalizzati possono essere condivisi a livello di sistema con accesso da allegare

>[!NOTE]
>
>Anteprima: 28 maggio 2026>Rilascio rapido produzione: 11 giugno 2026>Produzione per tutti: 16 luglio 2026

Ai moduli personalizzati è stata aggiunta la nuova opzione di condivisione &quot;Tutti nel sistema possono visualizzare e allegare&quot;. Quando si seleziona questa opzione, tutti gli utenti a livello di sistema possono allegare il modulo ad altri oggetti.

La condivisione a livello di sistema elimina la necessità di condividere manualmente i moduli e di aggiornare le autorizzazioni tra gruppi o agenzie quando vengono aggiunti nuovi gruppi.

Per ulteriori informazioni, vedere [Condividi modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).

## Nuova preferenza di sistema per applicare i campi obbligatori nella modifica in blocco

>[!NOTE]
>
>Anteprima: 28 maggio 2026>Rilascio rapido produzione: 11 giugno 2026>Produzione per tutti: 16 luglio 2026

Attualmente, quando si modificano oggetti in blocco, i campi obbligatori vengono applicati solo quando un utente modifica il campo. Se un campo non viene modificato, viene considerato facoltativo e non convalidato.

Una nuova preferenza di sistema ora consente di applicare i campi obbligatori nella modifica in blocco. Per non consentire il salvataggio di oggetti modificati in blocco a meno che tutti i campi obbligatori non contengano valori, selezionare l&#39;opzione **Applica sempre i campi obbligatori nella modifica in blocco** nella pagina Configurazione > Sistema > Preferenze.

Per ulteriori informazioni, vedere [Configurare le preferenze di sistema](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).
