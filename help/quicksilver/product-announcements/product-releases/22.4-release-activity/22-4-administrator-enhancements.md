---
title: Miglioramenti dell’amministratore 2.4
description: Miglioramenti dell’amministratore 2.4
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 1e62e7b3-14b6-4669-b3e1-ac6507343479
source-git-commit: 80fa784e15c3b4a927ee8ba2d18a80a2d84f4a91
workflow-type: tm+mt
source-wordcount: '869'
ht-degree: 0%

---

# Miglioramenti dell’amministratore 2.4

Questa pagina descrive tutti i miglioramenti apportati dall’amministratore all’ambiente di anteprima con la versione 22.4. Questi miglioramenti saranno resi disponibili la settimana del 3 ottobre 2022.

Per un elenco di tutte le modifiche disponibili con la versione 22.4, vedi [Panoramica sulla versione 22.4](/help/quicksilver/product-announcements/product-releases/22.4-release-activity/22-4-release-overview.md).

## Utilizzare gli stati sbloccati in un processo di approvazione

>[!NOTE]
>
>Questa funzione è stata introdotta per la prima volta nell’ambiente di anteprima durante l’intervallo di tempo di rilascio 22.3. Rilascia alla produzione il 15 settembre 2022.

Per ottenere un maggiore controllo sui processi e gli stati di approvazione del sistema, abbiamo reso possibile creare un processo di approvazione basato sullo stato di un sistema sbloccato. Inoltre, ora puoi sbloccare qualsiasi stato già utilizzato in un processo di approvazione. In precedenza, era necessario bloccare lo stato di un sistema utilizzato in un processo di approvazione. Ciò lo ha reso disponibile per tutti i gruppi, senza la possibilità di rimuoverlo o rinominarlo, in modo che gli amministratori dei gruppi non potessero semplificare l&#39;elenco degli stati del loro gruppo in base alle loro esigenze specifiche.

## Icona Blueprint nel menu principale ora controllata attraverso i modelli di layout

Gli amministratori di sistema possono ora aggiungere o rimuovere l’icona Blueprint nel menu principale tramite la configurazione del modello di layout. Questo offre un maggiore controllo sugli utenti che possono sfogliare il catalogo Blueprint.

L’icona Blueprint viene visualizzata nel menu principale quando:

* All&#39;utente non è assegnato alcun modello di layout

* Nel modello di layout dell&#39;utente è presente l&#39;opzione Blueprint nell&#39;elenco Active Items (Elementi attivi)

* Nel modello di layout dell&#39;utente è presente l&#39;opzione Blueprint nell&#39;elenco Elementi disponibili, l&#39;icona non viene visualizzata nel menu principale.

I modelli di layout esistenti includono automaticamente l’icona Blueprint e gli amministratori possono rimuovere l’icona dai modelli di layout per limitare la visibilità del catalogo Blueprint. I nuovi modelli di layout creati dopo la versione 22.4 includeranno l’icona Blueprint nell’elenco Elementi attivi.

Per ulteriori informazioni, consulta [Configurare l’accesso alle blueprint](/help/quicksilver/administration-and-setup/blueprints/configure-access-to-blueprints.md).

[Visualizza una dimostrazione video di questa funzione](https://video.tv.adobe.com/v/3412382/){target=_blank}

## Personalizzazione dell’intestazione del problema

In qualità di amministratore di gruppo o di Workfront, è ora possibile personalizzare i campi visualizzati nell’intestazione di un problema quando si utilizza un modello di layout.

Questo aggiornamento include i seguenti miglioramenti:

* Rimuovi o ridisponi i campi esistenti dall&#39;intestazione del problema.

* Aggiungi nuovi campi Panoramica dei problemi non modificabili. Non è possibile aggiungere campi o campi personalizzati che è possibile modificare. Puoi anche visualizzare campi modificabili attualmente presenti nell’intestazione del problema (ad esempio, Stato o Percentuale completata).

* L&#39;intestazione del problema può includere fino a cinque campi.

* Ora puoi aggiungere il campo &quot;Risolto da&quot; all’intestazione del problema. Quando un oggetto di risoluzione è associato al problema, il campo &quot;Risolto da&quot; diventa &quot;Problema di risoluzione&quot;, &quot;Attività di risoluzione&quot; o &quot;Progetto di risoluzione&quot;, a seconda del tipo di oggetto associato al problema.

Prima di questa versione, era possibile personalizzare solo le intestazioni di progetto e attività.



Per ulteriori informazioni, consulta [Personalizzare le intestazioni degli oggetti utilizzando un modello di layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

[Visualizza una dimostrazione video di questa funzione](https://video.tv.adobe.com/v/3412383/){target=_blank}

## Personalizzazione dell’intestazione delle attività

In qualità di amministratore di gruppo o di Workfront, è ora possibile personalizzare i campi visualizzati nell’intestazione di un’attività quando si utilizza un modello di layout.

Questo aggiornamento include i seguenti miglioramenti:

* Rimuovere o ridisporre i campi esistenti dall&#39;intestazione dell&#39;attività.

* Aggiungi nuovi campi Panoramica attività non modificabili. Non è possibile aggiungere campi o campi personalizzati che è possibile modificare. È inoltre possibile visualizzare campi modificabili attualmente presenti nell’intestazione dell’attività (ad esempio, Stato o Percentuale completata).

* L’intestazione dell’attività può includere fino a cinque campi.

Prima di questa versione, era possibile personalizzare solo le intestazioni del progetto.

Per ulteriori informazioni, consulta [Personalizzare le intestazioni degli oggetti utilizzando un modello di layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

[Guarda un video dimostrativo di questa funzione.](https://video.tv.adobe.com/v/3412384/){target=_blank}

## Funzionalità opt-in per le funzioni più recenti sulle bacheche

Siamo entusiasti di aprire nuove funzioni per l&#39;opt-in di funzionalità in fase iniziale. Questo strumento opzionale è disponibile per tutte le organizzazioni.

Solo un amministratore di Workfront può scegliere di utilizzare le funzioni iniziali. Quando l’amministratore sceglie le funzioni iniziali, tutti gli utenti dell’organizzazione accedono e le funzioni aggiuntive sono abilitate nell’ambiente Workfront di produzione.

Per ulteriori informazioni, consulta [Funzionalità opt-in in anteprima per le schede Adobe Workfront](/help/quicksilver/agile/get-started-with-boards/boards-early-feature-opt-in.md).

[Guarda un video dimostrativo di questa funzione.](https://video.tv.adobe.com/v/3412386/){target=_blank}

## Nell’editor per il calcolo dei campi del modulo personalizzato vengono visualizzate informazioni di errore

>[!NOTE]
>
>Questa funzione è stata introdotta per la prima volta nell’ambiente di anteprima durante l’intervallo di tempo di rilascio 22.3. Viene rilasciato a Production con la versione 22.4.

La modifica dei calcoli per i campi personalizzati è ora più semplice grazie alle utili informazioni di errore indicate direttamente nel calcolo. Durante la creazione di un campo calcolato in un modulo personalizzato, gli errori vengono evidenziati in rosa. Quando passi il cursore del mouse sulla parte evidenziata, viene visualizzata una descrizione del problema.

Per ulteriori informazioni, consulta [Aggiungere dati calcolati a un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

[Guarda un video dimostrativo di questa funzione.](https://video.tv.adobe.com/v/3412387/){target=_blank}

## Migrazione a Adobe Unified Experience

NOTA: Questa migrazione è stata posticipata al secondo trimestre del 2023. Tutti i clienti interessati riceveranno una notifica in quel momento.

Se l’organizzazione è stata caricata su Adobe Admin Console, l’istanza Workfront verrà migrata all’esperienza unificata di Adobe con la versione 22.4.

L’esperienza unificata di Adobe include:

* Un unico accesso per tutte le applicazioni Adobe tramite Adobe Experience Cloud

* Uno &quot;switcher di organizzazione&quot; per spostarsi tra organizzazioni e ambienti Workfront

* Navigazione con le opzioni per le pagine Workfront, le preferenze Adobe Experience Cloud e il profilo Workfront

Per ulteriori informazioni, consulta [Adobe Unified Experience per Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

[Guarda un video dimostrativo di questa funzione.](https://video.tv.adobe.com/v/3412388/){target=_blank}
