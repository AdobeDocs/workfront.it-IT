---
title: 23.1 Miglioramenti di Agile
description: 23.1 Miglioramenti di Agile
author: Courtney
draft: Probably
feature: Product Announcements
exl-id: 4bd041a5-a6e3-4fe3-ae23-45980701e904
source-git-commit: f0e21f9b2846c5665474903a2910ce9f41cdf810
workflow-type: tm+mt
source-wordcount: '882'
ht-degree: 0%

---

# 23.1 Miglioramenti di Agile

Questa pagina descrive tutti i miglioramenti apportati ad Agile con la versione 23.1 nell’ambiente di anteprima. Questi miglioramenti saranno resi disponibili nell&#39;ambiente di produzione la settimana del 16 gennaio 2023.

Per un elenco di tutte le modifiche disponibili con la versione 23.1, vedi [Panoramica sulla versione 23.1](/help/quicksilver/product-announcements/product-releases/23.1-release-activity/23-1-release-overview.md).

## Pianificazione dello stato delle schede Workfront

Le nuove funzioni di pianificazione dello Scrum nelle bacheche Adobe Workfront offrono opzioni flessibili per gestire i processi agili. Utilizzando questi strumenti, puoi:

* Tracciare il lavoro in iterazioni o spruzzi
* Utilizzare la velocità per guidare gli impegni del team
* Brano a discesa e tasso di completamento

Le funzioni di pianificazione di Scrum saranno &quot;veloci follow&quot; dopo la versione 23.1.

## Le date di scadenza vengono mappate su carte alla data di completamento pianificata sull’oggetto Workfront

>[!NOTE]
>
>Questa funzione è disponibile solo tramite la funzionalità opt-in per le schede Workfront.

Le date di scadenza delle schede collegate nelle bacheche Workfront ora vengono mappate sulla data di completamento pianificata per l&#39;oggetto Workfront associato. Se si aggiorna la data di scadenza su una scheda, la data di completamento pianificata viene aggiornata sull&#39;attività o sul problema. La modifica della data di completamento prevista cambia anche la data di scadenza sulla carta. In precedenza, la data di scadenza della scheda era una voce manuale e non era mappata ad alcuna data su un&#39;attività o su un problema.

La mappatura delle date si applica anche agli elementi della checklist collegati sincronizzati con le sottoattività.

La data di scadenza delle schede collegate e delle schede ad hoc ora include anche un campo temporale.

Per ulteriori informazioni, consulta [Utilizzare schede collegate sulle bacheche](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

[Visualizza una dimostrazione video di questa funzione](https://video.tv.adobe.com/v/3411952/){target=_blank}

## Le voci della lista di controllo della bacheca e le sottoattività di Workfront sono ora collegate

>[!NOTE]
>
>Questa funzione è disponibile solo tramite la funzionalità opt-in per le schede Workfront.

Quando aggiungete una scheda connessa a una bacheca per un&#39;attività Workfront, tutte le sottoattività vengono importate come voci di checklist sulla scheda. Inoltre, quando si crea una voce di elenco di controllo su una scheda connessa, all&#39;attività Workfront viene aggiunta una sottoattività. Le voci di elenco di controllo sui problemi non sono collegate ad alcun oggetto Workfront.

In precedenza, gli elementi e le sottoattività dell’elenco di controllo non erano collegati. Se si desidera includere una sottoattività sulla bacheca, è possibile importarla come una scheda collegata separata o aggiungere manualmente una voce della lista di controllo a una scheda.

Per ulteriori informazioni, consulta [Utilizzare schede collegate sulle bacheche](/help/quicksilver/agile/get-started-with-boards/connected-cards.md) e [Gestione degli elementi delle liste di controllo sulle schede](/help/quicksilver/agile/get-started-with-boards/manage-checklist-items.md).

[Visualizza una dimostrazione video di questa funzione](https://video.tv.adobe.com/v/3411951/){target=_blank}

## Contatore a schede sulle colonne di bacheca

>[!NOTE]
>
>Questa funzione è disponibile solo tramite la funzionalità opt-in per le schede Workfront.

È disponibile una nuova impostazione di configurazione per attivare un contatore di schede per tutte le colonne di una bacheca. Se si utilizza il limite WIP su una colonna, non viene aggiunto un contatore di schede separato.

Per ulteriori informazioni, consulta [Gestire le colonne della bacheca](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).

## Ricerca e ordinamento nel dashboard delle bacheche

>[!NOTE]
>
>Questa funzione è disponibile solo tramite la funzionalità opt-in per le schede Workfront.

Ora potete ordinare il dashboard delle bacheche in base al nome o alla data della bacheca e cercare una bacheca specifica nell&#39;elenco.

Per ulteriori informazioni, consulta [Utilizzare il dashboard delle bacheche](/help/quicksilver/agile/get-started-with-boards/use-boards-page.md).

## Lo stato viene visualizzato sulla scheda

>[!NOTE]
>
>Questa funzione è disponibile solo tramite la funzionalità opt-in per le schede Workfront.

Se a una scheda di una bacheca viene assegnato uno stato, lo stato viene visualizzato sulla scheda in modo da non dover aprire la scheda per visualizzarne lo stato. Questo miglioramento si applica sia alle schede ad hoc che a quelle collegate.

Per ulteriori informazioni, consulta [Utilizzare schede collegate sulle bacheche](/help/quicksilver/agile/get-started-with-boards/connected-cards.md) e [Aggiunta di una scheda ad hoc a una bacheca](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md).

![stato sulla scheda](/help/quicksilver/product-announcements/product-releases/assets/boards-connected-card-details-110922.png)

## Schede collegabili ora disponibili sulle bacheche

>[!NOTE]
>
>Questa funzione è disponibile solo tramite la funzionalità opt-in per le schede Workfront.

Ora potete inviare un collegamento a una scheda specifica a un altro utente delle bacheche. L&#39;utente deve avere accesso per visualizzare la bacheca prima di poter aprire il collegamento.

Quando aprite una scheda su una bacheca, l&#39;URL del browser si presenta così:

```
https://<Workfront-URL>/boards/<board-id>/card/<card-id>. 
```

Puoi copiare l’URL completo e inviarlo a un altro utente. Accedono direttamente alla scheda aperta quando accedono al collegamento.

In precedenza, i collegamenti erano disponibili per le bacheche ma non per le schede specifiche.

Per informazioni sulle schede, vedi [Aggiunta di una scheda ad hoc a una bacheca](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md) e [Utilizzare schede collegate sulle bacheche](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

## Filtra per connessione sulle bacheche

>[!NOTE]
>
>Questa funzione è disponibile solo tramite la funzionalità opt-in per le schede Workfront.

L&#39;elenco dei filtri su una bacheca ora include l&#39;opzione di filtrare per connessione, che mostra tutte le schede collegate per un progetto specifico. È inoltre possibile filtrare per schede non collegate.

Per ulteriori informazioni, consulta [Filtrare ed eseguire ricerche in una bacheca](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

[Visualizza una dimostrazione video di questa funzione](https://video.tv.adobe.com/v/3412381/){target=_blank}

## Archiviare schede da una bacheca su una pianificazione

>[!NOTE]
>
>Questa funzione è disponibile solo tramite la funzionalità opt-in per le schede Workfront.

Potete configurare una bacheca in modo che le schede siano archiviate o &quot;cadano&quot; dalla bacheca, secondo una pianificazione. Sono disponibili opzioni per impostare le schede in una particolare colonna da archiviare in un certo numero di giorni o settimane. Ad esempio, puoi definire il calo in modo che le schede in una colonna Completato vengano archiviate dopo essere rimaste nella colonna per due settimane.

Se desiderate visualizzare di nuovo le schede dopo che sono cadute dalla bacheca, potete impostare il filtro della bacheca per visualizzare le schede archiviate.

Per ulteriori informazioni, consulta [Configura decadimento scheda](/help/quicksilver/agile/use-boards-agile-planning-tools/configure-card-falloff.md).

[Visualizza una dimostrazione video di questa funzione](https://video.tv.adobe.com/v/3412323/){target=_blank}
