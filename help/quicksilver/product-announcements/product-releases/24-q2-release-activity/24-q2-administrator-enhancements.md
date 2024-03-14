---
title: Miglioramenti per gli amministratori del secondo trimestre 2024
description: Miglioramenti per gli amministratori del secondo trimestre 2024
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: a4056eb307c326b99f25406c2d5b87ad6018c754
workflow-type: tm+mt
source-wordcount: '722'
ht-degree: 0%

---

# Miglioramenti per gli amministratori del secondo trimestre 2024

Questa pagina descrive tutti i miglioramenti per gli amministratori apportati con la versione del secondo trimestre 2024 all’ambiente di anteprima. Questi miglioramenti saranno resi disponibili nell’ambiente di produzione come indicato.

Per un elenco di tutte le modifiche disponibili a questo punto nel ciclo di rilascio del secondo trimestre 2024, consulta [Panoramica sulla versione del secondo trimestre 2024](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).

## Aziende e utenti ora supportano i campi modulo personalizzati avanzati

>[!NOTE]
>
>Versione di anteprima: 14 marzo 2024; Produzione per tutti i clienti: 24.4 (aprile 2024)

Le funzioni avanzate dei moduli personalizzati, ad esempio i campi di ricerca esterna e i campi nativi di Workfront, sono ora disponibili quando si allega un modulo personalizzato a un’azienda o a un utente. Le funzioni avanzate sono disponibili nelle pagine Dettagli società e Dettagli utente e non nelle finestre di dialogo Modifica società e Modifica utente. Per utilizzare questi tipi di campi, è necessario creare il modulo personalizzato nel nuovo progettista di moduli.

Per ulteriori informazioni sui campi modulo personalizzati, consulta [Progettare un modulo con il progettista del modulo](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## L’integrazione JumpSeat è ora disponibile per i nuovi tipi di pacchetto

>[!NOTE]
>
>Versione di anteprima: 26 febbraio 2024; produzione per rilascio rapido: con la versione 24.3 (14 marzo 2024); produzione per tutti i clienti: 24.4 (aprile 2024)

L’integrazione JumpSeat esistente è ora disponibile per gli account che utilizzano uno dei nuovi tipi di pacchetto (ad esempio, Select, Prime o Ultimate). Per abilitare l’integrazione, è ancora necessario disporre di un abbonamento JumpSeat attivo.

Per ulteriori informazioni sull’integrazione JumpSeat, consulta [Configurare l’integrazione JumpSeat](/help/quicksilver/administration-and-setup/configure-integrations/configure-jumpseat.md).

## I campi nativi di Workfront sono disponibili nella versione beta di progettazione moduli

>[!NOTE]
>
>Versione di anteprima: 29 febbraio 2024; produzione per rilascio rapido: con la versione 24.3 (14 marzo 2024); produzione per tutti i clienti: 24.4 (aprile 2024)

I campi nativi di Workfront sono ora disponibili per l’aggiunta ai moduli personalizzati. Questo nuovo tipo di campo consente di organizzare e presentare i dati agli utenti in modo logico, senza dover ricreare i dati esistenti nei campi personalizzati.

Dopo aver selezionato Campo nativo nell&#39;elenco dei campi dei moduli personalizzati per aggiungere il campo al progettista del modulo, è possibile selezionare qualsiasi campo nativo per gli oggetti del modulo. Se ad esempio l&#39;elenco Tipi di oggetto nella parte superiore del progettista del modulo mostra Project, sarà possibile selezionare campi nativi per i progetti ma non campi specifici delle attività.

Quando il modulo personalizzato viene allegato a un oggetto, il campo viene popolato dai dati dell’oggetto. Ad esempio, il campo Description (Descrizione) in un modulo personalizzato allegato a un progetto estrae la descrizione del progetto. (Il campo può mostrare &quot;N/D&quot; se non sono disponibili dati).

I campi nativi utilizzati nei moduli personalizzati diventano disponibili nella libreria dei campi nella finestra di progettazione per essere riutilizzati. Sono inoltre visibili nell’area Configura > Forms personalizzato > Campi per consentire di vedere in quali moduli vengono utilizzati.

Questa funzione è disponibile solo nella versione beta di Progettazione moduli e non nel generatore di moduli legacy.

Per ulteriori informazioni, consulta [Progettare un modulo con il progettista del modulo](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

[Visualizza una dimostrazione video di questa funzione.](https://video.tv.adobe.com/v/3427702/){target=_blank}

## La mappatura degli attributi è ora disponibile per le organizzazioni che sono migrate ad Adobe IMS

>[!NOTE]
>
>Versione di anteprima: 22 febbraio 2024; Produzione per tutti i clienti: 22 febbraio 2024

Gli amministratori di sistema di Workfront ora possono impostare la mappatura degli attributi utente per l’organizzazione che è stata migrata ad Adobe IMS. Questo consente di passare le informazioni dell’utente in Workfront dal provider SSO (Single Sign-on) dell’organizzazione, in modo che i dati dell’utente non debbano essere immessi sia in Workfront che nel provider SSO.

In precedenza, questa funzionalità era disponibile solo per le organizzazioni che non avevano ancora effettuato l’onboarding in Adobe IMS.

Per istruzioni sulla configurazione della mappatura degli attributi, consulta [Mappare gli attributi utente nell’esperienza unificata di Adobe](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/map-user-attributes.md#map-user-attributes-in-the-adobe-unified-experience) nell’articolo **Mappare gli attributi utente ed eseguire il provisioning automatico dei nuovi utenti**.

## La logica di salto e la logica di visualizzazione sono ora disponibili nella versione beta di Progettazione moduli

>[!NOTE]
>
>Versione di anteprima: 8 febbraio 2024; produzione per rilascio rapido: con la versione 24.2 (15 febbraio 2024); produzione per tutti i clienti: da definire

È ora possibile modificare la logica di visualizzazione e salto esistente e aggiungere una nuova logica ai moduli personalizzati nella versione beta di progettazione moduli. Un generatore di logica di facile utilizzo consente di definire quali campi visualizzare o saltare in base alle selezioni effettuate nel modulo.

Le icone in un campo nell&#39;area di lavoro di progettazione del modulo indicano che la logica è configurata in tale campo o che il campo viene utilizzato nelle regole di logica configurate in altri campi.

Per ulteriori informazioni, consulta [Aggiungere logica di visualizzazione e logica di salto con il progettista del modulo](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md).