---
title: 23.2 Miglioramenti di Agile
description: 23.2 Miglioramenti di Agile
author: Courtney
draft: Probably
feature: Product Announcements
source-git-commit: 938bccf3b3eedf010b7d1db451c365f6097dc64d
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 23.2 Miglioramenti di Agile

Questa pagina descrive tutti i miglioramenti apportati all’ambiente di anteprima con la versione 23.2. Questi miglioramenti saranno resi disponibili nell’ambiente di produzione con la versione 23.2.

Per un elenco di tutte le modifiche disponibili a questo punto del ciclo di versione 23.2, vedi [Panoramica sulla versione 23.2](/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-release-overview.md).

## Funzionalità di iterazione disponibile nelle schede Adobe Workfront

Diverse nuove funzioni disponibili nelle schede Workfront consentono di utilizzare la funzionalità Scrum agile. Queste funzioni includono:

* Flussi di lavoro per raggruppare bacheche correlate allo stesso team e collaborare sul lavoro
* Un elenco di schede, o backlog di lavoro, con la possibilità di utilizzare le origini per collegare le schede alle attività e ai problemi di Workfront
* Schede di processo di pianificazione e iterazione dell&#39;iterazione

Le raccolte sono state rinominate in flussi di lavoro. I flussi di lavoro consentono di visualizzare i dati in modi diversi. Potete visualizzare gli elementi su schede in un elenco, su una bacheca o su un&#39;iterazione. Le schede in un flusso di lavoro possono essere condivise anche tra più bacheche. È possibile facilitare facilmente i flussi di lavoro utilizzando schede e bacheche in un flusso di lavoro.

Per ulteriori informazioni, consulta [Gestire i flussi di lavoro](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-collections.md), [Creare un’iterazione](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration.md)e [Utilizza l&#39;elenco delle schede](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md). I due articoli successivi non saranno disponibili in Principale fino a quando non pubblicherò il ramo.

## Aggiungere attività e problemi ai flussi di lavoro delle bacheche da elenchi e rapporti

È ora possibile aggiungere attività o problemi esistenti a un flusso di lavoro in Workfront Boards direttamente da una vista a elenco o a rapporti. Tutti gli elementi aggiunti al flusso di lavoro vengono aggiunti all’elenco delle schede come schede non pianificate.

Per ulteriori informazioni, consulta [Aggiungere attività o problemi esistenti a una bacheca](/help/quicksilver/agile/get-started-with-boards/add-card-from-list-to-board.md).


## Orari di accesso alle schede collegate su una bacheca

>[!NOTE]
>
>Questa funzione è disponibile solo tramite la funzionalità opt-in per le schede Workfront.

Ora è possibile accedere alle ore sulle schede collegate, nello stesso modo in cui si verifica un&#39;attività o un problema. Per registrare l&#39;ora è necessario disporre delle autorizzazioni corrette per l&#39;attività o il problema.

Per impostazione predefinita, i campi di registrazione dell&#39;ora non vengono visualizzati sulle schede collegate. È necessario attivare **Ore** nell&#39;area Configura sotto Schede.

Per ulteriori informazioni, consulta [Utilizzare schede collegate sulle bacheche](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

## Aggiungere attività e problemi alle bacheche Workfront da elenchi e rapporti

È ora possibile aggiungere attività o problemi esistenti a una bacheca di Workfront direttamente da una vista a elenco o a rapporti. Tutti gli elementi aggiunti alla bacheca diventeranno schede collegate.

Inoltre, il campo Bacheche è ora disponibile per aggiungere a elenchi e rapporti per attività o problemi. In questo campo vengono visualizzate tutte le bacheche alle quali è stata aggiunta un&#39;attività o un problema.

Per ulteriori informazioni, consulta [Aggiungere attività o problemi esistenti a una bacheca](/help/quicksilver/agile/get-started-with-boards/add-card-from-list-to-board.md).

## Personalizzare la visualizzazione dei campi su una scheda

>[!NOTE]
>
>Questa funzione è disponibile solo tramite la funzionalità opt-in per le schede Workfront.


È ora disponibile la personalizzazione per configurare quali campi vengono visualizzati su una scheda, sia nella visualizzazione completa quando la scheda è aperta, sia nella vista a schede condensate sulla bacheca. Quando disattivi un campo non viene visualizzato in nessuna delle due viste. È inoltre possibile abilitare un campo nella visualizzazione completa e nasconderlo dalla vista a condensa.

Per ulteriori informazioni, consulta [Personalizzare i campi visualizzati su una scheda](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md).

[Visualizza una dimostrazione video di questa funzione](https://video.tv.adobe.com/v/3415710/){target=_blank}

## Definire uno stato predefinito per le schede spostate in una colonna di una bacheca

>[!NOTE]
>
>Questa funzione è disponibile solo tramite la funzionalità opt-in per le schede Workfront.

È ora possibile impostare uno stato predefinito da applicare alle schede spostate in una colonna specifica, selezionando uno stato personalizzato e uno stato di sistema nei criteri colonna. Quando sposti una scheda nella colonna, Workfront tenta innanzitutto di applicare lo stato personalizzato (ad esempio, In attesa di un feedback). Se lo stato personalizzato non è disponibile per quella scheda, Workfront applicherà lo stato del sistema (ad esempio, In attesa). Inoltre, se lo stato dell&#39;attività o del problema connesso viene modificato in stato personalizzato o di sistema impostato nel criterio a colonne, la scheda viene spostata automaticamente nella colonna.

In precedenza, veniva richiesto di selezionare uno stato per ogni scheda spostata nella colonna, se erano disponibili più stati.

Per ulteriori informazioni, consulta [Gestire le colonne](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).

[Visualizza una dimostrazione video di questa funzione](https://video.tv.adobe.com/v/3415711/){target=_blank}

## Raccolte ora disponibili nelle bacheche Adobe Workfront

>[!NOTE]
>
>Questa funzione è disponibile solo tramite la funzionalità opt-in per le schede Workfront.

Ora potete creare raccolte nel dashboard delle bacheche. Una collezione è un gruppo di bacheche per collaborare sul lavoro. Una volta denominata la raccolta, potete aggiungere bacheche alla raccolta utilizzando un set di modelli che offrono impostazioni predefinite, come i nomi delle colonne. È inoltre possibile spostare le schede autonome in una raccolta. Una volta che una bacheca si trova in una raccolta, può essere spostata in un&#39;altra raccolta ma non può diventare una bacheca indipendente.

L&#39;aggiunta di membri a una raccolta funziona come l&#39;aggiunta di membri a una bacheca. Una persona o un team deve essere un membro della raccolta prima di poter essere aggiunto come membri in una bacheca della raccolta.

Per ulteriori informazioni, consulta [Gestire le raccolte](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-collections.md).

[Visualizza una dimostrazione video di questa funzione](https://video.tv.adobe.com/v/3415609/){target=_blank}

## Il campo Stima sulle schede collegate è associato al campo Punti Storia sugli oggetti Workfront

>[!NOTE]
>
>Questa funzione è disponibile solo tramite la funzionalità opt-in per le schede Workfront.

Il campo Stima sulle schede collegate nelle bacheche di Workfront ora viene mappato sul campo Punti della storia per l&#39;oggetto Workfront associato.

Il nuovo campo Punti storia è un campo modulo libero modificabile che è possibile aggiungere a una visualizzazione in un elenco o in un rapporto per attività o problemi. Non è legato alle ore pianificate o alle assegnazioni di team.

In precedenza, la stima della scheda era una voce manuale e non era mappata ad alcun campo su un&#39;attività o un problema.

Inoltre, il campo Stima sulle schede ad hoc e collegate non ha più un limite di caratteri. In precedenza, il numero massimo di caratteri era 99.

Per ulteriori informazioni, consulta [Utilizzare schede collegate sulle bacheche](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

## Scheda Anteprima nella colonna di aspirazione

>[!NOTE]
>
>Questa funzione è disponibile solo tramite la funzionalità opt-in per le schede Workfront.

È ora possibile fare clic su una scheda connessa nella colonna di immissione per visualizzare una versione di sola visualizzazione del suo contenuto. Non è possibile modificare il contenuto della scheda finché la scheda non viene spostata dalla colonna di assunzione in un&#39;altra colonna sulla bacheca.
