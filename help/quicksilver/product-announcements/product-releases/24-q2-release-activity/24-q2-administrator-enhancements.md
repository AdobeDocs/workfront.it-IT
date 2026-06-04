---
title: Miglioramenti per gli amministratori del secondo trimestre 2024
description: Miglioramenti per gli amministratori del secondo trimestre 2024
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: a297ee8d-d949-45ab-a219-437316fa8fa3
TQID: https://experienceleague.adobe.com/xcYDVGJSTKtR0dRM3EhQf62WokddEzsudevZ6Ur6Wn0
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2:
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 827
ht-degree: 11%

---

# Miglioramenti per gli amministratori del secondo trimestre 2024

Questa pagina descrive tutti i miglioramenti per gli amministratori apportati con la versione del secondo trimestre 2024 all’ambiente di anteprima. Tali miglioramenti saranno resi disponibili nell’ambiente di produzione come indicato.

Per un elenco di tutte le modifiche disponibili al momento nel ciclo di rilascio del secondo trimestre 2024, consulta [Panoramica sulla versione del secondo trimestre 2024](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).

## La logica di visualizzazione e la logica di salto sono ora disponibili nella modalità di anteprima di progettazione moduli

>[!NOTE]
>
>Versione di anteprima: 28 marzo 2024; Produzione per tutti i clienti: 24.4 (11 aprile 2024)

Il designer di moduli personalizzati beta ora consente di testare la logica di visualizzazione e saltare la logica in modalità anteprima. In precedenza, tutti i campi venivano visualizzati nell’anteprima anche quando veniva applicata la logica.

Per ulteriori informazioni sull&#39;anteprima di un modulo personalizzato nel progettista del modulo, vedere [Organizzare e visualizzare in anteprima un modulo con il progettista del modulo](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md).

## Aziende e utenti ora supportano i campi modulo personalizzati avanzati

>[!NOTE]
>
>Versione di anteprima: 14 marzo 2024; Produzione per tutti i clienti: 24.4 (11 aprile 2024)

Le funzioni avanzate dei moduli personalizzati, ad esempio i campi di ricerca esterna e i campi nativi di Workfront, sono ora disponibili quando si allega un modulo personalizzato a un’azienda o a un utente. Le funzioni avanzate sono disponibili nelle pagine Dettagli società e Dettagli utente e non nelle finestre di dialogo Modifica società e Modifica utente. Per utilizzare questi tipi di campi, è necessario creare il modulo personalizzato nel nuovo progettista di moduli.

Per ulteriori informazioni sui campi modulo personalizzato, vedere [Creare un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## L’integrazione JumpSeat è ora disponibile per i nuovi tipi di pacchetto

>[!NOTE]
>
>Versione di anteprima: 26 febbraio 2024; produzione per rilascio rapido: con la versione 24.3 (14 marzo 2024); produzione per tutti i clienti: 24.4 (11 aprile 2024)

L’integrazione JumpSeat esistente è ora disponibile per gli account che utilizzano uno dei nuovi tipi di pacchetto (ad esempio, Select, Prime o Ultimate). Per abilitare l’integrazione, è ancora necessario disporre di un abbonamento JumpSeat attivo.

Per ulteriori informazioni sull&#39;integrazione JumpSeat, vedere [Configurare l&#39;integrazione JumpSeat](/help/quicksilver/administration-and-setup/configure-integrations/configure-jumpseat.md).

## I campi nativi di Workfront sono disponibili nella versione beta di progettazione moduli

>[!NOTE]
>
>Versione di anteprima: 29 febbraio 2024; produzione per rilascio rapido: con la versione 24.3 (14 marzo 2024); produzione per tutti i clienti: 24.4 (11 aprile 2024)

I campi nativi di Workfront sono ora disponibili per l’aggiunta ai moduli personalizzati. Questo nuovo tipo di campo consente di organizzare e presentare i dati agli utenti in modo logico, senza dover ricreare i dati esistenti nei campi personalizzati.

Dopo aver selezionato Campo nativo nell&#39;elenco dei campi dei moduli personalizzati per aggiungere il campo al progettista del modulo, è possibile selezionare qualsiasi campo nativo per gli oggetti del modulo. Ad esempio, se l’elenco Tipi di oggetto nella parte superiore del designer dei moduli mostra Progetto, potrai selezionare campi nativi per i progetti ma non campi specifici delle attività.

Quando il modulo personalizzato viene associato a un oggetto, il campo viene popolato dai dati dell’oggetto. Ad esempio, il campo Descrizione in un modulo personalizzato associato a un progetto acquisirà direttamente la descrizione del progetto. Il campo può mostrare “N/D” se non sono disponibili dati.

I campi nativi utilizzati nei moduli personalizzati diventano disponibili nella libreria dei campi nella finestra di progettazione per essere riutilizzati. Sono inoltre visibili nell’area Configura > Forms personalizzato > Campi per consentire di vedere in quali moduli vengono utilizzati.

Questa funzione è disponibile solo nella versione beta di Progettazione moduli e non nel generatore di moduli legacy.

Per ulteriori informazioni, vedere [Creare un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

[Visualizza una dimostrazione video di questa funzione.](https://video.tv.adobe.com/v/3427702/){target=_blank}

## La mappatura degli attributi è ora disponibile per le organizzazioni che sono migrate ad Adobe IMS

>[!NOTE]
>
>Versione di anteprima: 22 febbraio 2024; Produzione per tutti i clienti: 22 febbraio 2024

Gli amministratori di sistema di Workfront ora possono impostare la mappatura degli attributi utente per l’organizzazione che è stata migrata ad Adobe IMS. Questo consente di passare le informazioni dell’utente in Workfront dal provider SSO (Single Sign-on) dell’organizzazione, in modo che i dati dell’utente non debbano essere immessi sia in Workfront che nel provider SSO.

In precedenza, questa funzionalità era disponibile solo per le organizzazioni che non avevano ancora effettuato l’onboarding in Adobe IMS.

Per istruzioni sulla configurazione della mappatura degli attributi, consulta [Mappare gli attributi utente nell&#39;esperienza unificata di Adobe](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/map-user-attributes.md#map-user-attributes-in-the-adobe-unified-experience) nell&#39;articolo **Mappare gli attributi utente ed eseguire il provisioning automatico dei nuovi utenti**.

## La logica di salto e la logica di visualizzazione sono ora disponibili nella versione beta di Progettazione moduli

>[!NOTE]
>
>Versione di anteprima: 8 febbraio 2024; produzione per rilascio rapido: con la versione 24.2 (15 febbraio 2024); produzione per tutti i clienti: 24.4 (11 aprile 2024)

È ora possibile modificare la logica di visualizzazione e salto esistente e aggiungere una nuova logica ai moduli personalizzati nella versione beta di progettazione moduli. Un generatore di logica di facile utilizzo consente di definire quali campi visualizzare o saltare in base alle selezioni effettuate nel modulo.

Le icone in un campo nell&#39;area di lavoro di progettazione del modulo indicano che la logica è configurata in tale campo o che il campo viene utilizzato nelle regole di logica configurate in altri campi.

Per ulteriori informazioni, vedere [Aggiungere logica di visualizzazione e logica di salto con la finestra di progettazione del modulo](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md).
