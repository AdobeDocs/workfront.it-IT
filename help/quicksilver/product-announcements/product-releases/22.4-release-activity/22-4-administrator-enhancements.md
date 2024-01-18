---
title: 22.4 Miglioramenti per gli amministratori
description: 22.4 Miglioramenti per gli amministratori
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 1e62e7b3-14b6-4669-b3e1-ac6507343479
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '880'
ht-degree: 0%

---

# 22.4 Miglioramenti per gli amministratori

Questa pagina descrive tutti i miglioramenti per gli amministratori apportati con la versione 22.4 all’ambiente di anteprima. Questi miglioramenti saranno resi disponibili la settimana del 3 ottobre 2022.

Per un elenco di tutte le modifiche disponibili con la versione 22.4, consulta [Panoramica sulla versione 22.4](/help/quicksilver/product-announcements/product-releases/22.4-release-activity/22-4-release-overview.md).

## Utilizzare gli stati sbloccati in un processo di approvazione

>[!NOTE]
>
>Questa funzione è stata introdotta per la prima volta nell’ambiente di anteprima durante l’intervallo di tempo di rilascio 22.3. Viene rilasciato in produzione il 15 settembre 2022.

Per avere un maggiore controllo sui processi e sugli stati di approvazione nel sistema, è stato possibile creare un processo di approvazione basato sullo stato sbloccato del sistema. Inoltre, ora puoi sbloccare qualsiasi stato già utilizzato in un processo di approvazione. In precedenza, era necessario bloccare uno stato di sistema utilizzato in un processo di approvazione. Questo lo ha reso disponibile per tutti i gruppi, senza la possibilità di rimuoverlo o rinominarlo, pertanto gli amministratori dei gruppi non hanno potuto semplificare l’elenco degli stati del gruppo in base alle loro esigenze specifiche.

## Icona Blueprint nel menu principale ora controllata tramite modelli di layout

Ora gli amministratori di sistema possono aggiungere o rimuovere l’icona Blueprint nel menu principale tramite la configurazione del modello di layout. Questo offre un maggiore controllo su chi può sfogliare il catalogo Blueprint.

L&#39;icona Blueprints viene visualizzata nel menu principale quando:

* Nessun modello di layout assegnato all&#39;utente

* Il modello di layout dell&#39;utente include l&#39;opzione Blueprint nell&#39;elenco Elementi attivi

* Il modello di layout dell&#39;utente dispone dell&#39;opzione Blueprint nell&#39;elenco Elementi disponibili; l&#39;icona non viene visualizzata nel menu principale.

I modelli di layout esistenti includono automaticamente l’icona Blueprint e gli amministratori possono rimuovere l’icona dai modelli di layout per limitare la visibilità del catalogo Blueprint. I nuovi modelli di layout creati dopo la versione 22.4 includeranno l’icona Blueprints nell’elenco Active Items (Elementi attivi).

Per ulteriori informazioni, consulta [Configurare l’accesso ai blueprint](/help/quicksilver/administration-and-setup/blueprints/configure-access-to-blueprints.md).

[Visualizza una dimostrazione video di questa funzione](https://video.tv.adobe.com/v/3412382/){target=_blank}

## Personalizzazione intestazione problema

In qualità di amministratore di Workfront o di gruppo, ora puoi personalizzare i campi visualizzati nell’intestazione di un problema quando utilizzi un modello di layout.

Questo aggiornamento include i seguenti miglioramenti:

* Rimuovi o ridisponi i campi esistenti dall’intestazione del problema.

* Aggiungere nuovi campi non modificabili per la panoramica del problema. Non è possibile aggiungere campi personalizzati o campi modificabili. Puoi anche visualizzare i campi modificabili che si trovano attualmente nell’intestazione del problema (ad esempio, Stato o Percentuale di completamento).

* L’intestazione del problema può includere fino a cinque campi.

* Ora puoi aggiungere il campo &quot;Risolto da&quot; all’intestazione del problema. Quando al problema è associato un oggetto di risoluzione, il campo &quot;Risolto da&quot; diventa &quot;Problema di risoluzione&quot;, &quot;Attività di risoluzione&quot; o &quot;Progetto di risoluzione&quot;, a seconda del tipo di oggetto associato al problema.

Prima di questa versione, era possibile personalizzare solo le intestazioni di progetto e di attività.



Per ulteriori informazioni, consulta [Personalizzare le intestazioni degli oggetti utilizzando un modello di layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

[Visualizza una dimostrazione video di questa funzione](https://video.tv.adobe.com/v/3412383/){target=_blank}

## Personalizzazione intestazione attività

In qualità di amministratore di Workfront o di gruppo, ora puoi personalizzare i campi visualizzati nell’intestazione di un’attività quando utilizzi un modello di layout.

Questo aggiornamento include i seguenti miglioramenti:

* Rimuovere o ridisporre i campi esistenti dall&#39;intestazione dell&#39;attività.

* Aggiungere nuovi campi di panoramica attività non modificabili. Non è possibile aggiungere campi personalizzati o campi modificabili. È inoltre possibile visualizzare i campi modificabili attualmente presenti nell&#39;intestazione dell&#39;attività, ad esempio Stato o Percentuale di completamento.

* L&#39;intestazione dell&#39;attività può includere fino a cinque campi.

Prima di questa versione, era possibile personalizzare solo le intestazioni del progetto.

Per ulteriori informazioni, consulta [Personalizzare le intestazioni degli oggetti utilizzando un modello di layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

[Visualizza una dimostrazione video di questa funzione.](https://video.tv.adobe.com/v/3412384/){target=_blank}

## Consenso anticipato per le funzioni più recenti delle bacheche

Siamo entusiasti di aprire nuove funzioni per le schede madri con consenso alle funzioni anticipate. Questo strumento opzionale è disponibile per tutte le organizzazioni.

Solo un amministratore di Workfront può dare il consenso alle funzioni preliminari. Quando l’amministratore acconsente alle funzioni iniziali, tutti gli utenti dell’organizzazione hanno acconsentito e le funzioni aggiuntive sono abilitate nell’ambiente Workfront di produzione.

Per ulteriori informazioni, consulta [Consenso anticipato alle funzioni per le schede madri Adobe Workfront](/help/quicksilver/agile/get-started-with-boards/boards-early-feature-opt-in.md).

[Visualizza una dimostrazione video di questa funzione.](https://video.tv.adobe.com/v/3412386/){target=_blank}

## L’editor di calcolo per i campi modulo personalizzati visualizza le informazioni sull’errore

>[!NOTE]
>
>Questa funzione è stata introdotta per la prima volta nell’ambiente di anteprima durante l’intervallo di tempo di rilascio 22.3. Viene rilasciato in produzione con la versione 22.4.

La modifica dei calcoli per i campi personalizzati è ora più semplice grazie alle utili informazioni sugli errori indicate direttamente nel calcolo. Durante la creazione di un campo calcolato in un modulo personalizzato, gli errori vengono evidenziati in rosa. Quando passi il cursore del mouse sulla parte evidenziata, viene visualizzata una descrizione per descrivere il problema.

Per ulteriori informazioni, consulta [Aggiungere dati calcolati a un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

[Visualizza una dimostrazione video di questa funzione.](https://video.tv.adobe.com/v/3412387/){target=_blank}

## Migrazione ad Adobe Unified Experience

NOTA: questa migrazione è stata posticipata al secondo trimestre del 2023. Tutti i clienti interessati riceveranno una notifica in tale momento.

Se per la tua organizzazione è stato eseguito l’onboarding in Adobe Admin Console, l’istanza di Workfront verrà migrata all’esperienza unificata Adobe con la versione 22.4.

L’esperienza unificata di Adobe include:

* Un singolo accesso per tutte le applicazioni Adobe tramite Adobe Experience Cloud

* Uno &quot;switcher di organizzazione&quot; per spostarsi tra le organizzazioni e gli ambienti Workfront

* Navigazione con opzioni per pagine Workfront, preferenze Adobe Experience Cloud e il tuo profilo Workfront

Per ulteriori informazioni, consulta [Adobe di esperienza unificata per Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

[Visualizza una dimostrazione video di questa funzione.](https://video.tv.adobe.com/v/3412388/){target=_blank}
