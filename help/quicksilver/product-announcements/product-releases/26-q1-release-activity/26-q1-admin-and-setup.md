---
title: Miglioramenti per gli amministratori del primo trimestre 2026
description: Miglioramenti per gli amministratori del primo trimestre 2026
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: a74d036b-e4fa-49e0-bb10-4baf379e1b1c
TQID: https://experienceleague.adobe.com/IYlqpTdS-pJNpBaCeYywassuOaTQdaSZlctxd1J0NPA
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 669
ht-degree: 96%

---

# Miglioramenti per gli amministratori del primo trimestre 2026

Questa pagina descrive i miglioramenti relativi agli Amministratori apportati all’ambiente di anteprima con la versione del primo trimestre 2026. Tali miglioramenti saranno resi disponibili nell’ambiente di produzione come indicato.

Per un elenco di tutte le modifiche disponibili a questo punto del ciclo di rilascio del primo trimestre 2026, consulta [Panoramica delle versioni del primo trimestre 2026](/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-release-overview.md).

## Gestire le priorità nel modello layout

>[!NOTE]
>
>Questa funzione non è al momento disponibile nell’ambiente di anteprima>Anteprima: 2 dicembre 2025>Versione rapida di produzione: 14 gennaio 2026>Produzione per tutti: 15 gennaio 2026


Ora puoi abilitare o disabilitare le Priorità per utenti specifici nel modello layout. Se in precedenza avevi disabilitato le Priorità per la tua organizzazione, con questa modifica tale opzione rimarrà disabilitata nel modello layout.

Le priorità verranno incluse automaticamente per i tipi di licenza con accesso predefinito alle richieste. Ad esempio, una licenza Collaboratore visualizzerà Richieste, Bacheche e Priorità per impostazione predefinita nel Menu principale, mentre una licenza Esterna visualizzerà solo Documenti e Bacheche perché non ha accesso alla visualizzazione o all’invio di richieste.


Per ulteriori informazioni, consulta [Personalizzare il menu principale utilizzando un modello layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).

## Verificare la presenza di conflitti tra più moduli per i campi personalizzati calcolati

>[!NOTE]
>
>Anteprima: 18 dicembre 2025>Rilascio rapido produzione: 14 gennaio 2026>Produzione per tutti: 15 gennaio 2026

Lo stesso campo calcolato può avere formule diverse se associato a moduli personalizzati diversi. Se a un oggetto sono associati due o più moduli contenenti lo stesso campo calcolato, le formule devono essere identiche in tutti i moduli. Modificare una formula non è consentito se può causare un conflitto.

Per fornire visibilità su quali oggetti potrebbero essere interessati dalla modifica di un’espressione nei campi personalizzati, è stata aggiunta un’opzione per verificare la presenza di conflitti. Questa finestra di dialogo mostra tutti gli oggetti che potrebbero essere interessati dalla modifica della formula, raggruppati per tipo di oggetto. Puoi passare ai dettagli relativi a ciascun oggetto ed esaminare i campi per decidere se un campo deve essere rimosso da uno dei moduli o se l’espressione deve rimanere invariata.

Per ulteriori informazioni, consulta [Aggiungere campi calcolati a un modulo](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).


## Data di inserimento e ID dell’autore dell’inserimento memorizzati negli oggetti personalizzati

>[!NOTE]
>
>Anteprima: 13 novembre 2025>Rilascio rapido produzione: 13 novembre 2025>Produzione per tutti: 13 novembre 2025

La data di inserimento e l’ID dell’autore inserimento sono ora memorizzati nelle sezioni, nei campi e nei moduli personalizzati. Puoi utilizzare queste opzioni dati nei rapporti come filtri, viste o raggruppamenti. Per visualizzarli nell’elenco delle sezioni, dei campi o dei moduli personalizzati in Configurazione, aggiungi Data di inserimento e il nome dell’Autore dell’inserimento come colonne in una vista nuova o esistente.

>[!NOTE]
>
>La Data inserimento e l’ID Autore dell’inserimento sono disponibili solo per le sezioni, i campi e i moduli personalizzati creati il 13 novembre 2025 o dopo tale data.

## Aggiornamenti ai nomi dei pulsanti durante la modifica di un modello layout

>[!NOTE]
>
>Anteprima: 30 ottobre 2025>Rilascio rapido produzione: 13 novembre 2025>Produzione per tutti: 15 gennaio 2026

Per garantire maggiore coerenza con altre aree di configurazione, come il designer dei moduli personalizzati, i pulsanti visualizzati durante la modifica di un modello layout sono stati modificati in **Applica**, **Salva e chiudi** e **Annulla**. La nuova opzione **Applica** ti consente di salvare le modifiche apportate al modello layout e continuare a modificare. In precedenza, le opzioni disponibili erano **Salva** e **Annulla**.

Per ulteriori informazioni, consulta [Creare e gestire modelli layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

## Gestione dei campi migliorata con il flag Attivo sui campi personalizzati

>[!NOTE]
>
>Anteprima: 30 ottobre 2025>Rilascio rapido produzione: 13 novembre 2025>Produzione per tutti: 15 gennaio 2026

Quando nel sistema è presente un numero elevato di campi personalizzati, la gestione di tali campi nei rapporti e nei moduli personalizzati può risultare complessa. Ora puoi contrassegnare i campi personalizzati come inattivi con il nuovo flag **Attivo**. Questo flag è disponibile quando utilizzi un campo in un modulo personalizzato o quando aggiungi o modifichi un campo dall’elenco Campi.

Se contrassegni un campo come inattivo:

* Viene escluso da rapporti, filtri, viste o altre posizioni in Workfront in cui puoi aggiungere un campo personalizzato
* Non è disponibile nella libreria dei campi per essere aggiunto ad altri moduli personalizzati

>[!NOTE]
>
>Contrassegnando un campo esistente come inattivo, lo rende non più disponibile per l&#39;uso negli elementi di reporting e nei moduli personalizzati da quel momento in poi. Se il campo inattivo è attualmente in uso in un rapporto o in un modulo, il campo e i relativi dati storici rimangono invariati.

Per ulteriori informazioni, consulta [Aggiungere o modificare un campo personalizzato, un’interruzione di sezione o un widget](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/edit-a-custom-field.md).
